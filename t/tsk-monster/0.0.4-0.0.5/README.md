# Comparing `tmp/tsk_monster-0.0.4.tar.gz` & `tmp/tsk_monster-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.4.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.5.tar", max compression
```

## Comparing `tsk_monster-0.0.4.tar` & `tsk_monster-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1860 2024-04-11 14:01:09.357007 tsk_monster-0.0.4/README.md
--rw-r--r--   0        0        0      583 2024-04-11 14:01:41.433991 tsk_monster-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3303 2024-04-11 14:01:09.367251 tsk_monster-0.0.4/tsk_monster/__init__.py
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 tsk_monster-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-04-13 17:54:51.881731 tsk_monster-0.0.5/README.md
+-rw-r--r--   0        0        0      583 2024-04-13 17:55:49.028637 tsk_monster-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3424 2024-04-13 17:23:43.548774 tsk_monster-0.0.5/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 tsk_monster-0.0.5/PKG-INFO
```

### Comparing `tsk_monster-0.0.4/pyproject.toml` & `tsk_monster-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsk-monster"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Gilad Kutiel <giladk@mobileye.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Homepage = "https://tsk.monster"
 Documentation = "https://tsk.monster"
```

### Comparing `tsk_monster-0.0.4/tsk_monster/__init__.py` & `tsk_monster-0.0.5/tsk_monster/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,152 @@
-import asyncio
 import logging
-from collections import defaultdict, deque
+import os
+import queue
+import threading
+from collections import defaultdict
+from concurrent.futures import Future, ProcessPoolExecutor
 from dataclasses import dataclass
+from functools import partial
 from pathlib import Path
-from typing import (Any, AsyncGenerator, Awaitable, Callable, Iterable, List,
-                    Union)
+from typing import Any, Callable, Generator, List
 
 lg = logging.getLogger(__name__)
 
 
 @dataclass
 class need:
     val: Any
 
 
 @dataclass
-class make:
+class prod:
     val: Any
 
 
-def changed(path: Path):
-    try:
-        tsk = path.with_suffix('.tsk')
-        if not tsk.exists():
-            return True
+@dataclass
+class Job:
+    description: str
+    gen: Generator[need | prod | Callable, None, None]
 
-        return tsk.stat().st_mtime < path.stat().st_mtime
-    finally:
-        tsk.touch()
+    def __repr__(self):
+        return self.description
 
 
-def none(items: Iterable[bool]):
-    return not any(items)
+def run(*jobs: Job):
+    q = queue.Queue[Job]()
+    needs = defaultdict(list)
+    prods = set()
 
+    def worker():
+        def add2q(job: Job):
+            def _(future: Future):
+                future.result()
+                q.put(job)
+                q.task_done()
 
-@dataclass
-class Tsk:
-    name: str
-    gen: AsyncGenerator[Union[need, make, "Tsk"], None]
+            return _
 
-    def __repr__(self):
-        return self.name
+        with ProcessPoolExecutor() as executor:
+            while True:
+                job = q.get()
 
+                try:
+                    item = next(job.gen)
 
-def tsk(
-        description: str, *,
-        action: str | Callable[[], Awaitable],
-        needs: List[Path] = [],
-        makes: List[Path] = []):
-
-    def str2action(s: str):
-        async def action():
-            p = await asyncio.create_subprocess_shell(s)
-            print(p)
-            await p.communicate()
+                    if isinstance(item, Callable):
+                        lg.info(f'Submitting: {job}')
+                        future = executor.submit(item)
+                        future.add_done_callback(add2q(job))
 
-        return action
+                    if isinstance(item, need):
+                        lg.debug(f'{job} needs {item.val}')
 
-    if isinstance(action, str):
-        action = str2action(action)
+                        if item.val in prods:
+                            q.put(job)
+                            q.task_done()
+                        else:
+                            needs[item.val].append(job)
 
-    async def gen():
-        always_run = len(needs) == len(makes) == 0
+                    if isinstance(item, prod):
+                        lg.debug(f'{job} produced {item.val}')
 
-        for n in needs:
-            yield need(n)
+                        prods.add(item.val)
+                        q.put(job)
+                        q.task_done()
 
-        if any(map(changed, needs)) or not all(map(Path.exists, makes)) or always_run:
-            lg.info(f'STARTING: {description}')
-            await action()
-            lg.info(f'DONE: {description}')
+                        jobs = needs.pop(item.val, [])
 
-        else:
-            lg.info(f'SKIPPING: {description}')
+                        for job in jobs:
+                            q.put(job)
+                            q.task_done()
 
-        for m in makes:
-            lg.debug(f'Creating {m} {m.exists()}')
+                except StopIteration:
+                    lg.info(f'Done {job}')
+                    q.task_done()
 
-            if m.exists():
-                yield make(m)
-            else:
-                lg.warning(f'Failed to create {m}.')
+    threading.Thread(
+        target=worker,
+        daemon=True).start()
 
-    return Tsk(description, gen())
+    for job in jobs:
+        q.put(job)
 
+    q.join()
 
-async def runner(tsks: Iterable[Tsk], parallelism=100):
+    lg.info('All work completed')
 
-    tsks = deque(tsks)
-    wait = defaultdict(list)
-    done = set()
 
-    while tsks:
-        batch = [
-            tsks.popleft()
-            for _ in range(min(parallelism, len(tsks)))]
+def changed(path: Path):
+    try:
+        tsk = path.with_suffix('.tsk')
+        if not tsk.exists():
+            return True
+
+        return tsk.stat().st_mtime < path.stat().st_mtime
+    finally:
+        tsk.touch()
+
 
-        results = await asyncio.gather(
-            *(anext(tsk.gen) for tsk in batch),
-            return_exceptions=True)
+@dataclass
+class Cmd:
+    description: str
+    action: Callable[[], Any]
+
+    def __repr__(self) -> str:
+        return self.description
 
-        assert len(batch) == len(results)
 
-        for tsk, res in zip(batch, results):
-            lg.debug(f'{tsk} -> {res}')
+Paths = List[Path | str] | List[Path]
 
-            if isinstance(res, need):
-                if res.val in done:
-                    tsks.append(tsk)
-                else:
-                    wait[res.val].append(tsk)
-                continue
 
-            if isinstance(res, make):
-                done.add(res.val)
-                for w in wait.pop(res.val, []):
-                    tsks.append(w)
+def to_paths(paths: Paths) -> List[Path]:
+    return [Path(p) if isinstance(p, str) else p for p in paths]
 
-                tsks.append(tsk)
-                continue
 
-            if isinstance(res, Tsk):
-                tsks.append(res)
-                tsks.append(tsk)
-                continue
+def tsk(
+        cmd: str | Cmd, *,
+        needs: Paths = [],
+        prods: Paths = []):
 
-            if isinstance(res, StopAsyncIteration):
-                pass
+    if isinstance(cmd, str):
+        cmd = Cmd(cmd, partial(os.system, cmd))
 
-            if not isinstance(res, (need, make, Tsk, StopAsyncIteration)):
-                lg.error(f'Failed to run {tsk.name}: {res}')
+    needs = to_paths(needs)
+    prods = to_paths(prods)
 
-    if wait:
-        lg.warning(f'Could not run all tasks: {wait.values()}')
-        return
+    def gen():
+        for n in needs:
+            yield need(n)
 
-    lg.info('All tasks finished.')
+        if any(map(changed, needs)) or not all(map(Path.exists, prods)):
+            yield cmd.action
 
+        else:
+            lg.info(f'SKIPPING: {cmd.description}')
+
+        for m in prods:
+            if m.exists():
+                yield prod(m)
+            else:
+                raise Exception(f'{cmd} failed to produce {m}.')
 
-def run(*tsks: Tsk, parallelism=1):
-    asyncio.run(runner(tsks, parallelism=parallelism))
+    return Job(cmd.description, gen())
```

