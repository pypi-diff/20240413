# Comparing `tmp/pyiter-0.8.2.tar.gz` & `tmp/pyiter-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiter-0.8.2.tar", last modified: Tue Mar 19 12:17:44 2024, max compression
+gzip compressed data, was "pyiter-0.8.3.tar", last modified: Sat Apr 13 12:58:53 2024, max compression
```

## Comparing `pyiter-0.8.2.tar` & `pyiter-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-03-19 12:17:44.052007 pyiter-0.8.2/
--rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.2/LICENSE-APACHE
--rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.2/LICENSE-MIT
--rw-r--r--   0 yish      (1000) yish      (1000)     2911 2024-03-19 12:17:44.052007 pyiter-0.8.2/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)     2357 2023-10-13 08:58:58.000000 pyiter-0.8.2/README.md
--rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.2/pyproject.toml
--rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-03-19 12:17:44.052007 pyiter-0.8.2/setup.cfg
--rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-03-19 12:16:58.000000 pyiter-0.8.2/setup.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-03-19 12:17:44.042007 pyiter-0.8.2/src/
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-03-19 12:17:44.042007 pyiter-0.8.2/src/pyiter/
--rw-r--r--   0 yish      (1000) yish      (1000)      315 2023-09-26 11:16:46.000000 pyiter-0.8.2/src/pyiter/__init__.py
--rw-r--r--   0 yish      (1000) yish      (1000)    92561 2024-03-19 12:16:17.000000 pyiter-0.8.2/src/pyiter/sequence.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-03-19 12:17:44.052007 pyiter-0.8.2/src/pyiter.egg-info/
--rw-r--r--   0 yish      (1000) yish      (1000)     2911 2024-03-19 12:17:44.000000 pyiter-0.8.2/src/pyiter.egg-info/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-03-19 12:17:44.000000 pyiter-0.8.2/src/pyiter.egg-info/SOURCES.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-03-19 12:17:44.000000 pyiter-0.8.2/src/pyiter.egg-info/dependency_links.txt
--rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-03-19 12:17:44.000000 pyiter-0.8.2/src/pyiter.egg-info/requires.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-03-19 12:17:44.000000 pyiter-0.8.2/src/pyiter.egg-info/top_level.txt
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/
+-rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.3/LICENSE-APACHE
+-rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.3/LICENSE-MIT
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-13 12:58:53.648203 pyiter-0.8.3/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)     2346 2024-04-13 12:58:27.000000 pyiter-0.8.3/README.md
+-rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.3/pyproject.toml
+-rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-13 12:58:53.648203 pyiter-0.8.3/setup.cfg
+-rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-13 12:58:02.000000 pyiter-0.8.3/setup.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/pyiter/
+-rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.8.3/src/pyiter/__init__.py
+-rw-r--r--   0 yish      (1000) yish      (1000)    93117 2024-04-08 05:32:25.000000 pyiter-0.8.3/src/pyiter/sequence.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/pyiter.egg-info/
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/SOURCES.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/dependency_links.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/requires.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/top_level.txt
```

### Comparing `pyiter-0.8.2/LICENSE-APACHE` & `pyiter-0.8.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.2/LICENSE-MIT` & `pyiter-0.8.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.2/PKG-INFO` & `pyiter-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.2
+Version: 0.8.3
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
@@ -30,15 +30,15 @@
 ```bash
 pip install pyiter
 ```
 
 ## Quickstart
 
 ```python
-from pyiter import iterate as it
+from pyiter import it
 from tqdm import tqdm
 
 
 text = ["hello", "world"]
 it(text).map(str.upper).to_list()
 # ['HELLO', 'WORLD']
```

### Comparing `pyiter-0.8.2/README.md` & `pyiter-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```bash
 pip install pyiter
 ```
 
 ## Quickstart
 
 ```python
-from pyiter import iterate as it
+from pyiter import it
 from tqdm import tqdm
 
 
 text = ["hello", "world"]
 it(text).map(str.upper).to_list()
 # ['HELLO', 'WORLD']
```

### Comparing `pyiter-0.8.2/setup.py` & `pyiter-0.8.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyiter',
-    version='0.8.2',
+    version='0.8.3',
     keywords=['linq', 'iterator', 'typing', 'lazy evaluation', 'type inference'],
     description='PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt '
                 'and Rust . Enables strong typing and type inference for iterative operations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='YISH',
     author_email="mokeyish@hotmail.com",
```

### Comparing `pyiter-0.8.2/src/pyiter/sequence.py` & `pyiter-0.8.3/src/pyiter/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -2175,26 +2175,52 @@
         Example 1:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).join(', ')
         'a, b, c'
         """
         return separator.join(self)
     
-
+    @overload
+    def progress(self) -> Sequence[T]:
+        ...
+    @overload
+    def progress(self, progress_func: Union[Literal['tqdm'], Literal['tqdm_rich']]) -> Sequence[T]:
+        ...
+    @overload
     def progress(self, progress_func: Callable[[Iterable[T]], Iterable[T]]) -> Sequence[T]:
+        ...
+    def progress(self, progress_func: Union[Callable[[Iterable[T]], Iterable[T]], Literal['tqdm'], Literal['tqdm_rich'], None ] = None) -> Sequence[T]:
         """
         Returns a Sequence that enable a progress bar for the given Sequence.
         
         Example 1:
         >>> from tqdm import tqdm
         >>> from time import sleep
         >>> it(range(10)).progress(lambda x: tqdm(x, total=len(x))).parallel_map(lambda x: sleep(0.), max_workers=5).to_list() and None
         >>> for _ in it(list(range(10))).progress(lambda x: tqdm(x, total=len(x))).to_list(): pass
         """
-        return ProgressTransform(self, progress_func).as_sequence()
+        if progress_func is not None and callable(progress_func):
+            return ProgressTransform(self, progress_func).as_sequence()
+        
+        def import_tqdm():
+            if progress_func == 'tqdm_rich':
+                from tqdm.rich import tqdm
+            else:
+                from tqdm import tqdm
+            return tqdm
+
+        try:
+            tqdm = import_tqdm()
+        except ImportError:
+            from pip import main as pip
+            pip(['install', 'tqdm'])
+            tqdm = import_tqdm()
+        
+        return it(tqdm(self, total=len(self)))
+        
     
     def typing_as(self, typ: Type[R]) -> Sequence[R]:
         """
         Cast the element as specific Type to gain code completion base on type annotations.
         """
         el = self.first_not_none_of_or_none()
         if el is None or isinstance(el, typ) or not isinstance(el, dict):
@@ -2430,37 +2456,30 @@
         self._max_workers = max_workers
         self._executor = executor
         self._chunksize = chunksize
     
     def __do_iter__(self) -> Iterator[R]:
         import os
 
-        def create_executor(max_workers: int, ):
+        def create_executor(max_workers: int):
             if self._executor == 'Process':
                 from concurrent.futures import ProcessPoolExecutor
                 return ProcessPoolExecutor(max_workers=max_workers)
             else:
                 from concurrent.futures import ThreadPoolExecutor
                 return ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='PyIter worker')
 
-        size = len(self._iter)
         chunksize = self._chunksize
         max_workers = self._max_workers or min(32, (os.cpu_count() or 1) + 4)
-        batch_count = -1 * (-size // chunksize)
-        max_workers = min(max_workers, batch_count)
-
         batch_size = max_workers * chunksize
-
-        if batch_size < size:
-            for batch in it(self._iter).chunked(batch_size):
-                with create_executor(max_workers) as executor:
-                    yield from executor.map(self._transformer, batch, chunksize=chunksize)
-        else:
+        
+        for batch in self._iter.chunked(batch_size):
             with create_executor(max_workers) as executor:
-                yield from executor.map(self._transformer, self._iter, chunksize=chunksize)
+                yield from executor.map(self._transformer, batch, chunksize=chunksize)
+
 
 
 class IndexedValue(NamedTuple, Generic[T]):
     val: T
     idx: int
     
     def __repr__(self) -> str:
```

### Comparing `pyiter-0.8.2/src/pyiter.egg-info/PKG-INFO` & `pyiter-0.8.3/src/pyiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.2
+Version: 0.8.3
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
@@ -30,15 +30,15 @@
 ```bash
 pip install pyiter
 ```
 
 ## Quickstart
 
 ```python
-from pyiter import iterate as it
+from pyiter import it
 from tqdm import tqdm
 
 
 text = ["hello", "world"]
 it(text).map(str.upper).to_list()
 # ['HELLO', 'WORLD']
```

