# Comparing `tmp/proq-0.0.2.tar.gz` & `tmp/proq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proq-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "proq-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `proq-0.0.2.tar` & `proq-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1012 2024-03-30 12:06:16.543927 proq-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1024 2024-03-30 12:06:16.547927 proq-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3097 2024-03-30 12:06:16.547927 proq-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2024-03-30 12:06:16.547927 proq-0.0.2/LICENSE
--rw-r--r--   0        0        0      925 2024-03-30 12:06:16.547927 proq-0.0.2/README.md
--rw-r--r--   0        0        0      779 2024-03-30 12:06:16.547927 proq-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       64 2024-03-30 12:06:16.547927 proq-0.0.2/src/proq/__init__.py
--rw-r--r--   0        0        0      372 2024-03-30 12:06:16.547927 proq-0.0.2/src/proq/collectible.py
--rw-r--r--   0        0        0       62 2024-03-30 12:06:16.547927 proq-0.0.2/src/proq/common.py
--rw-r--r--   0        0        0     1631 2024-03-30 12:06:16.547927 proq-0.0.2/src/proq/proq.py
--rw-r--r--   0        0        0     1133 2024-03-30 12:06:16.547927 proq-0.0.2/src/proq/queue.py
--rw-r--r--   0        0        0     2955 2024-03-30 12:06:16.547927 proq-0.0.2/tests/test_proq.py
--rw-r--r--   0        0        0      951 2024-03-30 12:06:16.547927 proq-0.0.2/tests/test_queue.py
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 proq-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1012 2024-04-13 10:26:32.651677 proq-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1024 2024-04-13 10:26:32.651677 proq-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3097 2024-04-13 10:26:32.651677 proq-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2024-04-13 10:26:32.651677 proq-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1214 2024-04-13 10:26:32.651677 proq-0.0.3/README.md
+-rw-r--r--   0        0        0      803 2024-04-13 10:26:32.651677 proq-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/collectible.py
+-rw-r--r--   0        0        0       62 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/common.py
+-rw-r--r--   0        0        0     1682 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/proq.py
+-rw-r--r--   0        0        0     1726 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/transform.py
+-rw-r--r--   0        0        0     1800 2024-04-13 10:26:32.651677 proq-0.0.3/src/proq/transform_parallel.py
+-rw-r--r--   0        0        0     3245 2024-04-13 10:26:32.651677 proq-0.0.3/tests/test_proq.py
+-rw-r--r--   0        0        0     1142 2024-04-13 10:26:32.651677 proq-0.0.3/tests/test_transform.py
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 proq-0.0.3/PKG-INFO
```

### Comparing `proq-0.0.2/.github/workflows/python-package.yml` & `proq-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `proq-0.0.2/.github/workflows/python-publish.yml` & `proq-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proq-0.0.2/.gitignore` & `proq-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `proq-0.0.2/LICENSE` & `proq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proq-0.0.2/README.md` & `proq-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Process Queue
 
 Simplify data processing using pipelines.
 
-- Inline - create the numbers 1-10, square them, then sum the results:
+- Inline
 
 ```python
+# Create the numbers 1-10, square them, then sum the results
 result = proq.create(range(11)).map(lambda x: x ** 2).reduce(lambda x, y: x + y).next()
 ```
 
 - Procedurally
 
 ```python
 # Create a square numbers proq and split into two
@@ -22,14 +23,27 @@
 
 # Iterate over the results
 for d1, d2 in zip(data1_neg, data2_plus_1):
     print(d1, d2, d1 + d2)
     assert d1 + d2 == 1
 ```
 
+- In parallel
+
+```python
+# Get prime numbers under 1,000,000 - calculation happens concurrently
+primes = (
+    proq.create(range(1000001))
+        .par_map(lambda x: x, is_prime(x))
+        .filter(lambda x, is_prime: is_prime)
+        .map(lambda x, is_prime: x)
+        .collect()
+)
+```
+
 # Installation
 
 ```bash
 pip install proq
 ```
 
 # Development
```

### Comparing `proq-0.0.2/pyproject.toml` & `proq-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"]
 dynamic = ["version", "description"]
+dependencies = ["dill"]
 
 [project.urls]
 Home = "https://github.com/gabay/proq"
 "Bug Tracker" = "https://github.com/gabay/proq/issues"
 
 [project.optional-dependencies]
 dev = ["black", "mypy"]
```

### Comparing `proq-0.0.2/src/proq/proq.py` & `proq-0.0.3/src/proq/proq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from __future__ import annotations
 
 import functools
 import itertools
 from typing import Callable, Iterable
 
-from . import collectible
+from . import collectible, transform, transform_parallel
 from .common import T, U
 
 
 def create(objects: Iterable[T]) -> Proq[T]:
     return Proq(objects)
 
 
 class Proq(collectible.Collectible[T]):
     def __init__(self, items: Iterable[T]):
-        self.items = iter(items)
-
-    def __next__(self) -> T:
-        return next(self.items)
+        self.items = items
+        super().__init__(iter(items))
 
     def append(self, items: Iterable[T]) -> Proq[T]:
-        return Proq(itertools.chain(self.items, items))
+        return Proq(itertools.chain(self, items))
 
     def prepend(self, items: Iterable[T]) -> Proq[T]:
-        return Proq(itertools.chain(items, self.items))
+        return Proq(itertools.chain(items, self))
 
     def flatten(self: Proq[Iterable[T]]) -> Proq[T]:
-        return Proq(itertools.chain(*self.items))
+        return Proq(transform.Flatten(self))
 
     def map(self, f: Callable[[T], U]) -> Proq[U]:
-        return Proq(map(f, self.items))
+        return Proq(transform.Map(f, self))
 
-    def flat_map(self, f: Callable[[T], Iterable[U]]) -> Proq[U]:
-        return Proq(itertools.chain(*map(f, self.items)))
+    def flat_map(self, f: Callable[[T], Iterable[U]]) -> Proq[Iterable[U]]:
+        return self.map(f).flatten()
 
     def foreach(self, f: Callable[[T], U]) -> Proq[T]:
         def _foreach(item: T) -> T:
             f(item)
             return item
 
         return self.map(_foreach)
 
     def filter(self, f: Callable[[T], bool]) -> Proq[T]:
-        return Proq(filter(f, self.items))
+        return Proq(transform.Filter(f, self))
 
     def reduce(self, f: Callable[[T, T], T], initial: T | None = None) -> Proq[T]:
         if initial is None:
-            return Proq(functools.reduce(f, self.items) for _ in range(1))
-        return Proq(functools.reduce(f, self.items, initial) for _ in range(1))
+            return Proq(transform.Reduce(f, self))
+        return Proq(transform.ReduceInitial(f, self, initial))
 
     def tee(self, n: int = 2) -> tuple[Proq[T], ...]:
-        return tuple(Proq(iterator) for iterator in itertools.tee(self.items, n))
+        return tuple(Proq(iterator) for iterator in itertools.tee(self, n))
+
+    def par_map(self, f: Callable[[T], U]) -> Proq[U]:
+        return Proq(transform_parallel.ParallelMap(f, self))
```

### Comparing `proq-0.0.2/tests/test_proq.py` & `proq-0.0.3/tests/test_proq.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
 
 def test_proq_tee_duplicates_items():
     a, b = proq.create([0, 1, 2, 3]).tee()
     assert a.collect() == b.collect() == [0, 1, 2, 3]
 
 
+def test_proq_par_map_modifies_output():
+    assert proq.create([0, 1, 2, 3]).par_map(lambda x: x + 1).collect() == [1, 2, 3, 4]
+
+
 #
 # Lazy Evaluation
 #
 def test_proq_map_is_lazy():
     p = proq.create([1, 2]).map(_raise_runtime_foo)
     with pytest.raises(RuntimeError, match="foo"):
         p.next()
@@ -88,14 +92,20 @@
 
 def test_proq_reduce_is_lazy():
     p = proq.create([1, 2]).reduce(_raise_runtime_foo)
     with pytest.raises(RuntimeError, match="foo"):
         p.next()
 
 
+def test_proq_par_map_is_lazy():
+    p = proq.create([1, 2]).par_map(_raise_runtime_foo)
+    with pytest.raises(RuntimeError, match="foo"):
+        p.next()
+
+
 def _raise_runtime_foo(*_):
     raise RuntimeError("foo")
 
 
 #
 # Allowed inputs
 #
```

### Comparing `proq-0.0.2/PKG-INFO` & `proq-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: proq
-Version: 0.0.2
+Version: 0.0.3
 Summary: Process Queue
 Author-email: Roi Gabay <roigby@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Dist: dill
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Bug Tracker, https://github.com/gabay/proq/issues
 Project-URL: Home, https://github.com/gabay/proq
 Provides-Extra: dev
 Provides-Extra: test
 
 # Process Queue
 
 Simplify data processing using pipelines.
 
-- Inline - create the numbers 1-10, square them, then sum the results:
+- Inline
 
 ```python
+# Create the numbers 1-10, square them, then sum the results
 result = proq.create(range(11)).map(lambda x: x ** 2).reduce(lambda x, y: x + y).next()
 ```
 
 - Procedurally
 
 ```python
 # Create a square numbers proq and split into two
@@ -41,14 +43,27 @@
 
 # Iterate over the results
 for d1, d2 in zip(data1_neg, data2_plus_1):
     print(d1, d2, d1 + d2)
     assert d1 + d2 == 1
 ```
 
+- In parallel
+
+```python
+# Get prime numbers under 1,000,000 - calculation happens concurrently
+primes = (
+    proq.create(range(1000001))
+        .par_map(lambda x: x, is_prime(x))
+        .filter(lambda x, is_prime: is_prime)
+        .map(lambda x, is_prime: x)
+        .collect()
+)
+```
+
 # Installation
 
 ```bash
 pip install proq
 ```
 
 # Development
```

