# Comparing `tmp/cachebox-2.2.1.tar.gz` & `tmp/cachebox-2.2.2.tar.gz`

## Comparing `cachebox-2.2.1.tar` & `cachebox-2.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 cachebox-2.2.1/Cargo.toml
--rw-r--r--   0     1001      127     2737 2024-04-05 07:59:32.000000 cachebox-2.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127       30 2024-04-05 07:59:32.000000 cachebox-2.2.1/.gitignore
--rw-r--r--   0     1001      127     2787 2024-04-05 07:59:32.000000 cachebox-2.2.1/CHANGELOG.md
--rw-r--r--   0     1001      127     1064 2024-04-05 07:59:32.000000 cachebox-2.2.1/LICENSE
--rw-r--r--   0     1001      127      784 2024-04-05 07:59:32.000000 cachebox-2.2.1/Makefile
--rw-r--r--   0     1001      127    12348 2024-04-05 07:59:32.000000 cachebox-2.2.1/README.md
--rw-r--r--   0     1001      127      599 2024-04-05 07:59:32.000000 cachebox-2.2.1/cachebox/__init__.py
--rw-r--r--   0     1001      127    14930 2024-04-05 07:59:32.000000 cachebox-2.2.1/cachebox/_cachebox.pyi
--rw-r--r--   0     1001      127        0 2024-04-05 07:59:32.000000 cachebox-2.2.1/cachebox/py.typed
--rw-r--r--   0     1001      127     7458 2024-04-05 07:59:32.000000 cachebox-2.2.1/cachebox/utils.py
--rw-r--r--   0     1001      127     1646 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/base.rs
--rw-r--r--   0     1001      127     7544 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/cache.rs
--rw-r--r--   0     1001      127     8284 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/fifocache.rs
--rw-r--r--   0     1001      127     7861 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/lfucache.rs
--rw-r--r--   0     1001      127     8371 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/lrucache.rs
--rw-r--r--   0     1001      127      389 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/mod.rs
--rw-r--r--   0     1001      127     8109 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/rrcache.rs
--rw-r--r--   0     1001      127    10255 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/ttlcache.rs
--rw-r--r--   0     1001      127    10844 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/classes/vttlcache.rs
--rw-r--r--   0     1001      127    36577 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/internal/caches.rs
--rw-r--r--   0     1001      127      235 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/internal/mod.rs
--rw-r--r--   0     1001      127      614 2024-04-05 07:59:32.000000 cachebox-2.2.1/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-05 07:59:32.000000 cachebox-2.2.1/tests/__init__.py
--rw-r--r--   0     1001      127     2925 2024-04-05 07:59:32.000000 cachebox-2.2.1/tests/test_cached.py
--rw-r--r--   0     1001      127    14261 2024-04-05 07:59:32.000000 cachebox-2.2.1/tests/test_caches.py
--rw-r--r--   0     1001      127    10057 2024-04-05 07:59:32.000000 cachebox-2.2.1/Cargo.lock
--rw-r--r--   0     1001      127      975 2024-04-05 07:59:32.000000 cachebox-2.2.1/pyproject.toml
--rw-r--r--   0        0        0    13152 1970-01-01 00:00:00.000000 cachebox-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 cachebox-2.2.2/Cargo.toml
+-rw-r--r--   0     1001      127     2737 2024-04-13 13:12:12.000000 cachebox-2.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127       31 2024-04-13 13:12:12.000000 cachebox-2.2.2/.gitignore
+-rw-r--r--   0     1001      127     3020 2024-04-13 13:12:12.000000 cachebox-2.2.2/CHANGELOG.md
+-rw-r--r--   0     1001      127     1064 2024-04-13 13:12:12.000000 cachebox-2.2.2/LICENSE
+-rw-r--r--   0     1001      127      784 2024-04-13 13:12:12.000000 cachebox-2.2.2/Makefile
+-rw-r--r--   0     1001      127    12348 2024-04-13 13:12:12.000000 cachebox-2.2.2/README.md
+-rw-r--r--   0     1001      127      599 2024-04-13 13:12:12.000000 cachebox-2.2.2/cachebox/__init__.py
+-rw-r--r--   0     1001      127    14925 2024-04-13 13:12:12.000000 cachebox-2.2.2/cachebox/_cachebox.pyi
+-rw-r--r--   0     1001      127        0 2024-04-13 13:12:12.000000 cachebox-2.2.2/cachebox/py.typed
+-rw-r--r--   0     1001      127     7458 2024-04-13 13:12:12.000000 cachebox-2.2.2/cachebox/utils.py
+-rw-r--r--   0     1001      127     1644 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/base.rs
+-rw-r--r--   0     1001      127     7579 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/cache.rs
+-rw-r--r--   0     1001      127     8288 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/fifocache.rs
+-rw-r--r--   0     1001      127     7863 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/lfucache.rs
+-rw-r--r--   0     1001      127     8369 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/lrucache.rs
+-rw-r--r--   0     1001      127      389 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/mod.rs
+-rw-r--r--   0     1001      127     8213 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/rrcache.rs
+-rw-r--r--   0     1001      127    10425 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/ttlcache.rs
+-rw-r--r--   0     1001      127    10880 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/classes/vttlcache.rs
+-rw-r--r--   0     1001      127    36520 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/internal/caches.rs
+-rw-r--r--   0     1001      127      235 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/internal/mod.rs
+-rw-r--r--   0     1001      127      612 2024-04-13 13:12:12.000000 cachebox-2.2.2/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-13 13:12:12.000000 cachebox-2.2.2/tests/__init__.py
+-rw-r--r--   0     1001      127     2925 2024-04-13 13:12:12.000000 cachebox-2.2.2/tests/test_cached.py
+-rw-r--r--   0     1001      127    14261 2024-04-13 13:12:12.000000 cachebox-2.2.2/tests/test_caches.py
+-rw-r--r--   0     1001      127     9505 2024-04-13 13:12:12.000000 cachebox-2.2.2/Cargo.lock
+-rw-r--r--   0     1001      127     1039 2024-04-13 13:12:12.000000 cachebox-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0    13221 1970-01-01 00:00:00.000000 cachebox-2.2.2/PKG-INFO
```

### Comparing `cachebox-2.2.1/.github/workflows/CI.yml` & `cachebox-2.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/CHANGELOG.md` & `cachebox-2.2.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.2] - 2024-04-13
+
+### Changed
+- The behavior of the `__repr__` function has been changed and improved.
+- Improve `RRCache` performance.
+
+### Internal
+- `pyo3` updated and features changed.
+- Use `fastrand` instead of `rand`.
+
 ## [2.2.1] - 2024-04-05
 
 ### Fixed
 - Fix `RuntimeError` when you passing a cache implemetation to its own methods.
 
 ### Internal
 - Update Rust dependecies
```

### Comparing `cachebox-2.2.1/LICENSE` & `cachebox-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/Makefile` & `cachebox-2.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/README.md` & `cachebox-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/cachebox/__init__.py` & `cachebox-2.2.2/cachebox/__init__.py`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/cachebox/_cachebox.pyi` & `cachebox-2.2.2/cachebox/_cachebox.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,14 @@
             >>> cache = TTLCache(0, 10) # unlimited-size cache, 10 ttl value
             >>> cache = TTLCache(100, 5, {"key1": "value1", "key2": "value2"}) # initialize from dict or any iterable object
         """
         ...
 
     @property
     def ttl(self) -> float: ...
-    
     def get_with_expire(
         self, key: KT, default: DT = None
     ) -> typing.Tuple[typing.Union[VT, DT], float]:
         """
         Works like `.get()`, but also returns the remaining expiration.
 
         Example::
```

### Comparing `cachebox-2.2.1/cachebox/utils.py` & `cachebox-2.2.2/cachebox/utils.py`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/src/classes/base.rs` & `cachebox-2.2.2/src/classes/base.rs`

 * *Files 6% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 }
 
 #[macro_use]
 mod macros {
     #[macro_export]
     macro_rules! pyany_to_hash {
         ($key:expr, $py:expr) => {{
-            let _ref = $key.as_ref($py);
+            let _ref = $key.bind($py);
             _ref.hash()
         }};
     }
 }
```

### Comparing `cachebox-2.2.1/src/classes/cache.rs` & `cachebox-2.2.2/src/classes/cache.rs`

 * *Files 7% similar despite different names*

```diff
@@ -152,24 +152,26 @@
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let read = self.inner.read();
+        if read.maxsize == 0 {
+            format!("Cache({}, capacity={})", read.len(), read.capacity())
+        } else {
+            format!(
+                "Cache({} / {}, capacity={})",
+                read.len(),
+                read.maxsize,
+                read.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
@@ -213,15 +215,15 @@
 
     fn drain(&self, n: usize) -> PyResult<()> {
         let _ = n;
         Err(pyo3::exceptions::PyNotImplementedError::new_err(()))
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             self.inner.write().update(dict.iter().map(|(key, val)| {
                 Ok::<(isize, base::KeyValuePair), PyErr>((
                     unsafe { key.hash().unwrap_unchecked() },
```

### Comparing `cachebox-2.2.1/src/classes/fifocache.rs` & `cachebox-2.2.2/src/classes/lrucache.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 use parking_lot::RwLock;
 use pyo3::prelude::*;
 
 use crate::classes::base;
 use crate::internal;
 
 #[pyclass(extends=base::BaseCacheImpl, subclass, module = "cachebox._cachebox")]
-pub struct FIFOCache {
-    pub inner: RwLock<internal::FIFOCache<isize, base::KeyValuePair>>,
+pub struct LRUCache {
+    pub inner: RwLock<internal::LRUCache<isize, base::KeyValuePair>>,
 }
 
 #[pymethods]
-impl FIFOCache {
+impl LRUCache {
     #[new]
     #[pyo3(signature=(maxsize, iterable=None, *, capacity=0))]
     fn __new__(
         py: Python<'_>,
         maxsize: usize,
         iterable: Option<PyObject>,
         capacity: usize,
     ) -> PyResult<(Self, base::BaseCacheImpl)> {
         let (slf, base) = (
-            FIFOCache {
-                inner: RwLock::new(internal::FIFOCache::new(maxsize, capacity)),
+            LRUCache {
+                inner: RwLock::new(internal::LRUCache::new(maxsize, capacity)),
             },
             base::BaseCacheImpl {},
         );
 
         if let Some(x) = iterable {
             slf.update(py, x)?;
         }
@@ -66,25 +66,25 @@
     fn insert(&self, py: Python<'_>, key: PyObject, value: PyObject) -> PyResult<()> {
         self.__setitem__(py, key, value)
     }
 
     fn __getitem__(&self, py: Python<'_>, key: PyObject) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
-        match self.inner.read().get(&hash) {
+        match self.inner.write().get(&hash) {
             Some(x) => Ok(x.1.clone()),
             None => Err(pyo3::exceptions::PyKeyError::new_err(key)),
         }
     }
 
     #[pyo3(signature=(key, default=None))]
     fn get(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
-        match self.inner.read().get(&hash) {
+        match self.inner.write().get(&hash) {
             Some(val) => Ok(val.1.clone()),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
 
     fn __delitem__(&self, py: Python<'_>, key: PyObject) -> PyResult<()> {
         let hash = pyany_to_hash!(key, py)?;
@@ -112,97 +112,94 @@
         map1.ne(&map2)
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.get(x).unwrap().0.clone())
+            .map(|x| read.fast_get(x).unwrap().0.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn keys(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.get(x).unwrap().0.clone())
+            .map(|x| read.fast_get(x).unwrap().0.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn values(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.get(x).unwrap().1.clone())
+            .map(|x| read.fast_get(x).unwrap().1.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn items(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecItemsIterator>> {
         let read = slf.inner.read();
         let view: Vec<(PyObject, PyObject)> = read
             .sorted_keys()
             .map(|x| {
-                let val = read.get(x).unwrap();
+                let val = read.fast_get(x).unwrap();
                 (val.0.clone(), val.1.clone())
             })
             .collect();
 
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let read = self.inner.read();
+        if read.maxsize == 0 {
+            format!("LRUCache({}, capacity={})", read.len(), read.capacity())
+        } else {
+            format!(
+                "LRUCache({} / {}, capacity={})",
+                read.len(),
+                read.maxsize,
+                read.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(x) => Ok(x.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -235,15 +232,15 @@
     }
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             self.inner.write().update(dict.iter().map(|(key, val)| {
                 Ok::<(isize, base::KeyValuePair), PyErr>((
                     unsafe { key.hash().unwrap_unchecked() },
@@ -279,17 +276,17 @@
         Ok(())
     }
 
     fn __clear__(&self) {
         self.inner.write().clear(false);
     }
 
-    fn first(&self) -> Option<PyObject> {
+    fn least_recently_used(&self) -> Option<PyObject> {
         let read = self.inner.read();
-        Some(read.get(read.first()?)?.0.clone())
+        Some(read.fast_get(read.least_recently_used()?)?.0.clone())
     }
 
-    fn last(&self) -> Option<PyObject> {
+    fn most_recently_used(&self) -> Option<PyObject> {
         let read = self.inner.read();
-        Some(read.get(read.last()?)?.0.clone())
+        Some(read.fast_get(read.most_recently_used()?)?.0.clone())
     }
 }
```

### Comparing `cachebox-2.2.1/src/classes/lfucache.rs` & `cachebox-2.2.2/src/classes/lfucache.rs`

 * *Files 15% similar despite different names*

```diff
@@ -153,42 +153,39 @@
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let read = self.inner.read();
+        if read.maxsize == 0 {
+            format!("LFUCache({}, capacity={})", read.len(), read.capacity())
+        } else {
+            format!(
+                "LFUCache({} / {}, capacity={})",
+                read.len(),
+                read.maxsize,
+                read.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(x) => Ok(x.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -221,15 +218,15 @@
     }
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             self.inner.write().update(dict.iter().map(|(key, val)| {
                 Ok::<(isize, base::KeyValuePair), PyErr>((
                     unsafe { key.hash().unwrap_unchecked() },
```

### Comparing `cachebox-2.2.1/src/classes/lrucache.rs` & `cachebox-2.2.2/src/classes/fifocache.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 use parking_lot::RwLock;
 use pyo3::prelude::*;
 
 use crate::classes::base;
 use crate::internal;
 
 #[pyclass(extends=base::BaseCacheImpl, subclass, module = "cachebox._cachebox")]
-pub struct LRUCache {
-    pub inner: RwLock<internal::LRUCache<isize, base::KeyValuePair>>,
+pub struct FIFOCache {
+    pub inner: RwLock<internal::FIFOCache<isize, base::KeyValuePair>>,
 }
 
 #[pymethods]
-impl LRUCache {
+impl FIFOCache {
     #[new]
     #[pyo3(signature=(maxsize, iterable=None, *, capacity=0))]
     fn __new__(
         py: Python<'_>,
         maxsize: usize,
         iterable: Option<PyObject>,
         capacity: usize,
     ) -> PyResult<(Self, base::BaseCacheImpl)> {
         let (slf, base) = (
-            LRUCache {
-                inner: RwLock::new(internal::LRUCache::new(maxsize, capacity)),
+            FIFOCache {
+                inner: RwLock::new(internal::FIFOCache::new(maxsize, capacity)),
             },
             base::BaseCacheImpl {},
         );
 
         if let Some(x) = iterable {
             slf.update(py, x)?;
         }
@@ -66,39 +66,39 @@
     fn insert(&self, py: Python<'_>, key: PyObject, value: PyObject) -> PyResult<()> {
         self.__setitem__(py, key, value)
     }
 
     fn __getitem__(&self, py: Python<'_>, key: PyObject) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
-        match self.inner.write().get(&hash) {
+        match self.inner.read().get(&hash) {
             Some(x) => Ok(x.1.clone()),
             None => Err(pyo3::exceptions::PyKeyError::new_err(key)),
         }
     }
 
     #[pyo3(signature=(key, default=None))]
     fn get(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
-        match self.inner.write().get(&hash) {
+        match self.inner.read().get(&hash) {
             Some(val) => Ok(val.1.clone()),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
 
     fn __delitem__(&self, py: Python<'_>, key: PyObject) -> PyResult<()> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(_) => Ok(()),
             None => Err(pyo3::exceptions::PyKeyError::new_err(key)),
         }
     }
-    
+
     fn __contains__(&self, py: Python<'_>, key: PyObject) -> PyResult<bool> {
         let hash = pyany_to_hash!(key, py)?;
         Ok(self.inner.read().contains_key(&hash))
     }
 
     fn __eq__(&self, other: &Self) -> bool {
         let map1 = self.inner.read();
@@ -112,97 +112,94 @@
         map1.ne(&map2)
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.fast_get(x).unwrap().0.clone())
+            .map(|x| read.get(x).unwrap().0.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn keys(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.fast_get(x).unwrap().0.clone())
+            .map(|x| read.get(x).unwrap().0.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn values(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecOneValueIterator>> {
         let read = slf.inner.read();
         let view: Vec<PyObject> = read
             .sorted_keys()
-            .map(|x| read.fast_get(x).unwrap().1.clone())
+            .map(|x| read.get(x).unwrap().1.clone())
             .collect();
 
         let iter = base::VecOneValueIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
     fn items(slf: PyRef<'_, Self>) -> PyResult<Py<base::VecItemsIterator>> {
         let read = slf.inner.read();
         let view: Vec<(PyObject, PyObject)> = read
             .sorted_keys()
             .map(|x| {
-                let val = read.fast_get(x).unwrap();
+                let val = read.get(x).unwrap();
                 (val.0.clone(), val.1.clone())
             })
             .collect();
 
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let read = self.inner.read();
+        if read.maxsize == 0 {
+            format!("FIFOCache({}, capacity={})", read.len(), read.capacity())
+        } else {
+            format!(
+                "FIFOCache({} / {}, capacity={})",
+                read.len(),
+                read.maxsize,
+                read.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(x) => Ok(x.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -235,15 +232,15 @@
     }
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             self.inner.write().update(dict.iter().map(|(key, val)| {
                 Ok::<(isize, base::KeyValuePair), PyErr>((
                     unsafe { key.hash().unwrap_unchecked() },
@@ -279,17 +276,17 @@
         Ok(())
     }
 
     fn __clear__(&self) {
         self.inner.write().clear(false);
     }
 
-    fn least_recently_used(&self) -> Option<PyObject> {
+    fn first(&self) -> Option<PyObject> {
         let read = self.inner.read();
-        Some(read.fast_get(read.least_recently_used()?)?.0.clone())
+        Some(read.get(read.first()?)?.0.clone())
     }
 
-    fn most_recently_used(&self) -> Option<PyObject> {
+    fn last(&self) -> Option<PyObject> {
         let read = self.inner.read();
-        Some(read.fast_get(read.most_recently_used()?)?.0.clone())
+        Some(read.get(read.last()?)?.0.clone())
     }
 }
```

### Comparing `cachebox-2.2.1/src/classes/rrcache.rs` & `cachebox-2.2.2/src/classes/rrcache.rs`

 * *Files 22% similar despite different names*

```diff
@@ -172,42 +172,43 @@
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let read = self.inner.read();
+        if read.parent.maxsize == 0 {
+            format!(
+                "RRCache({}, capacity={})",
+                read.parent.len(),
+                read.parent.capacity()
+            )
+        } else {
+            format!(
+                "RRCache({} / {}, capacity={})",
+                read.parent.len(),
+                read.parent.maxsize,
+                read.parent.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().parent.capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().parent.clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().parent.remove(&hash) {
             Some(x) => Ok(x.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -240,15 +241,15 @@
     }
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             self.inner.write().update(dict.iter().map(|(key, val)| {
                 Ok::<(isize, base::KeyValuePair), PyErr>((
                     unsafe { key.hash().unwrap_unchecked() },
```

### Comparing `cachebox-2.2.1/src/classes/ttlcache.rs` & `cachebox-2.2.2/src/classes/ttlcache.rs`

 * *Files 4% similar despite different names*

```diff
@@ -191,42 +191,46 @@
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow_mut();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let mut write = self.inner.write();
+        write.expire();
+        if write.maxsize == 0 {
+            format!(
+                "TTLCache({}, ttl={:?}, capacity={})",
+                write.len(),
+                write.ttl,
+                write.capacity()
+            )
+        } else {
+            format!(
+                "TTLCache({} / {}, ttl={:?}, capacity={})",
+                write.len(),
+                write.maxsize,
+                write.ttl,
+                write.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(x) => Ok(x.value.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -259,15 +263,15 @@
     }
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     fn update(&self, py: Python<'_>, iterable: PyObject) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             let mut write = self.inner.write();
             write.expire();
```

### Comparing `cachebox-2.2.1/src/classes/vttlcache.rs` & `cachebox-2.2.2/src/classes/vttlcache.rs`

 * *Files 6% similar despite different names*

```diff
@@ -189,42 +189,40 @@
         let iter = base::VecItemsIterator {
             view: view.into_iter(),
         };
 
         Py::new(slf.py(), iter)
     }
 
-    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-        let class_name: &str = slf.get_type().name()?;
-        let borrowed = slf.borrow_mut();
-        Ok(format!(
-            "{}({} / {}, capacity={})",
-            class_name,
-            borrowed.__len__(),
-            borrowed.maxsize(),
-            borrowed.capacity()
-        ))
+    fn __repr__(&self) -> String {
+        let mut write = self.inner.write();
+        write.expire();
+        if write.maxsize == 0 {
+            format!("VTTLCache({}, capacity={})", write.len(), write.capacity())
+        } else {
+            format!(
+                "VTTLCache({} / {}, capacity={})",
+                write.len(),
+                write.maxsize,
+                write.capacity()
+            )
+        }
     }
 
     fn capacity(&self) -> usize {
         self.inner.read().capacity()
     }
 
     #[pyo3(signature=(*, reuse=false))]
     fn clear(&self, reuse: bool) {
         self.inner.write().clear(reuse);
     }
 
     #[pyo3(signature=(key, default=None))]
-    fn pop(
-        &self,
-        py: Python<'_>,
-        key: PyObject,
-        default: Option<PyObject>,
-    ) -> PyResult<PyObject> {
+    fn pop(&self, py: Python<'_>, key: PyObject, default: Option<PyObject>) -> PyResult<PyObject> {
         let hash = pyany_to_hash!(key, py)?;
 
         match self.inner.write().remove(&hash) {
             Some(x) => Ok(x.value.1),
             None => Ok(default.unwrap_or_else(|| py.None())),
         }
     }
@@ -259,15 +257,15 @@
 
     fn drain(&self, n: usize) -> usize {
         self.inner.write().drain(n)
     }
 
     #[pyo3(signature=(iterable, ttl=None))]
     fn update(&self, py: Python<'_>, iterable: PyObject, ttl: Option<f32>) -> PyResult<()> {
-        let obj = iterable.as_ref(py);
+        let obj = iterable.bind(py);
 
         if obj.is_instance_of::<pyo3::types::PyDict>() {
             let dict = obj.downcast::<pyo3::types::PyDict>()?;
 
             let mut write = self.inner.write();
             write.expire();
```

### Comparing `cachebox-2.2.1/src/internal/caches.rs` & `cachebox-2.2.2/src/internal/caches.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use rand::seq::IteratorRandom;
 use std::collections::VecDeque;
 use std::time;
 
 use ahash::AHashMap;
 
 /// Fixed-size (or can be not) cache implementation without any policy,
 /// So only can be fixed-size, or unlimited size cache
@@ -402,15 +401,15 @@
     pub fn least_frequently_used(&self) -> Option<K> {
         if self.inner.is_empty() {
             None
         } else {
             let mut vector: Vec<_> = self.counter.iter().map(|(t, n)| (*n, *t)).collect();
             // vector.sort_unstable_by_key(|(n, _)| *n);
             vector.sort_unstable_by(|(n, _), (m, _)| n.cmp(m));
-            
+
             let (_, least_frequently_used_key) = vector[0];
             Some(least_frequently_used_key)
         }
     }
 
     pub fn insert(&mut self, key: K, value: V) -> pyo3::PyResult<()> {
         if self.maxsize > 0 && self.inner.len() >= self.maxsize && self.inner.get(&key).is_none() {
@@ -563,15 +562,15 @@
         Ok(())
     }
 
     pub fn popitem(&mut self) -> Option<V> {
         if self.parent.is_empty() {
             None
         } else {
-            let key = *self.parent.keys().choose(&mut rand::thread_rng()).unwrap();
+            let key = *fastrand::choice(self.parent.keys()).unwrap();
             self.parent.remove(&key)
         }
     }
 
     pub fn drain(&mut self, n: usize) -> usize {
         let mut c = 0usize;
         for _ in 0..n {
```

### Comparing `cachebox-2.2.1/src/lib.rs` & `cachebox-2.2.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 // Internal implementations
 mod classes;
 mod internal;
 
 #[pymodule]
 #[pyo3(name = "_cachebox")]
-fn _cachebox(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _cachebox(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add("__author__", "aWolverP")?;
     m.add_class::<classes::BaseCacheImpl>()?;
     m.add_class::<classes::Cache>()?;
     m.add_class::<classes::FIFOCache>()?;
     m.add_class::<classes::LFUCache>()?;
     m.add_class::<classes::LRUCache>()?;
```

### Comparing `cachebox-2.2.1/tests/test_cached.py` & `cachebox-2.2.2/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/tests/test_caches.py` & `cachebox-2.2.2/tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `cachebox-2.2.1/Cargo.lock` & `cachebox-2.2.2/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -25,44 +25,56 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cachebox"
-version = "2.2.1"
+version = "2.2.2"
 dependencies = [
  "ahash",
+ "fastrand",
  "parking_lot",
  "pyo3",
- "rand",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "fastrand"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+
+[[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
@@ -111,128 +123,101 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
-name = "ppv-lite86"
-version = "0.2.17"
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "rand"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
-dependencies = [
- "libc",
- "rand_chacha",
- "rand_core",
-]
-
-[[package]]
-name = "rand_chacha"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
-dependencies = [
- "ppv-lite86",
- "rand_core",
-]
-
-[[package]]
-name = "rand_core"
-version = "0.6.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
@@ -247,25 +232,14 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "syn"
 version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
@@ -281,17 +255,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -371,9 +345,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn",
 ]
```

### Comparing `cachebox-2.2.1/pyproject.toml` & `cachebox-2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["maturin>=1.4,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "cachebox"
-version = "2.2.1"
+version = "2.2.2"
 description = "The fastest memoizing and caching Python library written in Rust"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["caching", "cached", "cachetools", "cachebox", "cache", "in-memory-caching", "memoizing"]
 authors = [
   {email = "awolverp@gmail.com"},
   {name = "awolverp"}
 ]
 
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS',
     'Typing :: Typed',
 ]
```

### Comparing `cachebox-2.2.1/PKG-INFO` & `cachebox-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: cachebox
-Version: 2.2.1
+Version: 2.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Typing :: Typed
 License-File: LICENSE
```

