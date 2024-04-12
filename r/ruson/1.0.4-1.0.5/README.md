# Comparing `tmp/ruson-1.0.4.tar.gz` & `tmp/ruson-1.0.5.tar.gz`

## Comparing `ruson-1.0.4.tar` & `ruson-1.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 ruson-1.0.4/Cargo.toml
--rw-r--r--   0     1001      127     3237 2024-01-16 11:38:00.000000 ruson-1.0.4/.github/workflows/pypi.yml
--rw-r--r--   0     1001      127     1984 2024-01-16 11:38:00.000000 ruson-1.0.4/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4699 2024-01-16 11:38:00.000000 ruson-1.0.4/.gitignore
--rw-r--r--   0     1001      127     6459 2024-01-16 11:38:00.000000 ruson-1.0.4/README.md
--rw-r--r--   0     1001      127      201 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/__init__.py
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/core/__init__.py
--rw-r--r--   0     1001      127      140 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/core/config.py
--rw-r--r--   0     1001      127     1009 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/core/instance.py
--rw-r--r--   0     1001      127    18549 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/core/ruson_doc.py
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/__init__.py
--rw-r--r--   0     1001      127     1114 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/client.py
--rw-r--r--   0     1001      127      389 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/client.pyi
--rw-r--r--   0     1001      127     5657 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/collection.py
--rw-r--r--   0     1001      127     2971 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/collection.pyi
--rw-r--r--   0     1001      127      723 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/database.py
--rw-r--r--   0     1001      127      211 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/database.pyi
--rw-r--r--   0     1001      127     2138 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/results.py
--rw-r--r--   0     1001      127      944 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/results.pyi
--rw-r--r--   0     1001      127      172 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/session.py
--rw-r--r--   0     1001      127       19 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/session.pyi
--rw-r--r--   0     1001      127     2795 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/types.py
--rw-r--r--   0     1001      127     8211 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/driver/types.pyi
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/ruson/py.typed
--rw-r--r--   0     1001      127    17404 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/bson_binding.rs
--rw-r--r--   0     1001      127     2404 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/client_binding.rs
--rw-r--r--   0     1001      127    13492 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/collection_binding.rs
--rw-r--r--   0     1001      127     1111 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/database_biding.rs
--rw-r--r--   0     1001      127     5730 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/document_binding.rs
--rw-r--r--   0     1001      127     3908 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/index_binding.rs
--rw-r--r--   0     1001      127     3409 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/iterator_binding.rs
--rw-r--r--   0     1001      127     6403 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/mod.rs
--rw-r--r--   0     1001      127     1048 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/results_binding.rs
--rw-r--r--   0     1001      127      444 2024-01-16 11:38:00.000000 ruson-1.0.4/src/bindings/utils.rs
--rw-r--r--   0     1001      127    10666 2024-01-16 11:38:00.000000 ruson-1.0.4/src/interface.rs
--rw-r--r--   0     1001      127      431 2024-01-16 11:38:00.000000 ruson-1.0.4/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/__init__.py
--rw-r--r--   0     1001      127     1432 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/conftest.py
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/__init__.py
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_aggregate.py
--rw-r--r--   0     1001      127      642 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_connection.py
--rw-r--r--   0     1001      127      386 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_count.py
--rw-r--r--   0     1001      127     1173 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_delete.py
--rw-r--r--   0     1001      127      673 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_distinct.py
--rw-r--r--   0     1001      127      407 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_drop.py
--rw-r--r--   0     1001      127     2474 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_find.py
--rw-r--r--   0     1001      127     1343 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_indexes.py
--rw-r--r--   0     1001      127     1049 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_insert.py
--rw-r--r--   0     1001      127     1477 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_update.py
--rw-r--r--   0     1001      127     1570 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_core/test_upsert.py
--rw-r--r--   0     1001      127        0 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_driver/__init__.py
--rw-r--r--   0     1001      127     1073 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_driver/test_client.py
--rw-r--r--   0     1001      127    11664 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_driver/test_collection.py
--rw-r--r--   0     1001      127      638 2024-01-16 11:38:00.000000 ruson-1.0.4/tests/test_driver/test_db.py
--rw-r--r--   0     1001      127    47876 2024-01-16 11:38:05.000000 ruson-1.0.4/Cargo.lock
--rw-r--r--   0     1001      127      756 2024-01-16 11:38:00.000000 ruson-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 ruson-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 ruson-1.0.5/Cargo.toml
+-rw-r--r--   0     1001      127     3187 2024-04-12 23:00:10.000000 ruson-1.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0     1001      127     1984 2024-04-12 23:00:10.000000 ruson-1.0.5/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4699 2024-04-12 23:00:10.000000 ruson-1.0.5/.gitignore
+-rw-r--r--   0     1001      127     6459 2024-04-12 23:00:10.000000 ruson-1.0.5/README.md
+-rw-r--r--   0     1001      127      201 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/__init__.py
+-rw-r--r--   0     1001      127      140 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/config.py
+-rw-r--r--   0     1001      127     1009 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/instance.py
+-rw-r--r--   0     1001      127    18549 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/ruson_doc.py
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/__init__.py
+-rw-r--r--   0     1001      127     1114 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/client.py
+-rw-r--r--   0     1001      127      389 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/client.pyi
+-rw-r--r--   0     1001      127     5657 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/collection.py
+-rw-r--r--   0     1001      127     2971 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/collection.pyi
+-rw-r--r--   0     1001      127      723 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/database.py
+-rw-r--r--   0     1001      127      211 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/database.pyi
+-rw-r--r--   0     1001      127     2138 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/results.py
+-rw-r--r--   0     1001      127      944 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/results.pyi
+-rw-r--r--   0     1001      127      172 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/session.py
+-rw-r--r--   0     1001      127       19 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/session.pyi
+-rw-r--r--   0     1001      127     2795 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/types.py
+-rw-r--r--   0     1001      127     8211 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/types.pyi
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/py.typed
+-rw-r--r--   0     1001      127    17604 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/bson_binding.rs
+-rw-r--r--   0     1001      127     2404 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/client_binding.rs
+-rw-r--r--   0     1001      127    13492 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/collection_binding.rs
+-rw-r--r--   0     1001      127     1111 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/database_biding.rs
+-rw-r--r--   0     1001      127     5730 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/document_binding.rs
+-rw-r--r--   0     1001      127     3908 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/index_binding.rs
+-rw-r--r--   0     1001      127     3409 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/iterator_binding.rs
+-rw-r--r--   0     1001      127     6403 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/mod.rs
+-rw-r--r--   0     1001      127     1048 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/results_binding.rs
+-rw-r--r--   0     1001      127      444 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/utils.rs
+-rw-r--r--   0     1001      127    10666 2024-04-12 23:00:10.000000 ruson-1.0.5/src/interface.rs
+-rw-r--r--   0     1001      127      431 2024-04-12 23:00:10.000000 ruson-1.0.5/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/__init__.py
+-rw-r--r--   0     1001      127     1432 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_aggregate.py
+-rw-r--r--   0     1001      127      642 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_connection.py
+-rw-r--r--   0     1001      127      386 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_count.py
+-rw-r--r--   0     1001      127     1173 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_delete.py
+-rw-r--r--   0     1001      127      673 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_distinct.py
+-rw-r--r--   0     1001      127      407 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_drop.py
+-rw-r--r--   0     1001      127     2474 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_find.py
+-rw-r--r--   0     1001      127     1343 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_indexes.py
+-rw-r--r--   0     1001      127     1049 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_insert.py
+-rw-r--r--   0     1001      127     1477 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_update.py
+-rw-r--r--   0     1001      127     1570 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_upsert.py
+-rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/__init__.py
+-rw-r--r--   0     1001      127     1073 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_client.py
+-rw-r--r--   0     1001      127    11664 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_collection.py
+-rw-r--r--   0     1001      127      638 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_db.py
+-rw-r--r--   0     1001      127    48136 2024-04-12 23:00:14.000000 ruson-1.0.5/Cargo.lock
+-rw-r--r--   0     1001      127      756 2024-04-12 23:00:10.000000 ruson-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 ruson-1.0.5/PKG-INFO
```

### Comparing `ruson-1.0.4/.github/workflows/pypi.yml` & `ruson-1.0.5/.github/workflows/pypi.yml`

 * *Files 5% similar despite different names*

```diff
@@ -91,20 +91,19 @@
               with:
                   name: wheels
                   path: dist
 
     release:
         name: Release
         runs-on: ubuntu-latest
-        if: "startsWith(github.ref, 'refs/tags/')"
         needs: [linux, windows, macos, sdist]
         steps:
             - uses: actions/download-artifact@v3
               with:
                   name: wheels
             - name: Publish to PyPI
               uses: PyO3/maturin-action@v1
               env:
                   MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
               with:
                   command: upload
-                  args: --non-interactive --skip-existing *
+                  args: --non-interactive --skip-existing *
```

### Comparing `ruson-1.0.4/.github/workflows/test.yml` & `ruson-1.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/.gitignore` & `ruson-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/README.md` & `ruson-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/core/instance.py` & `ruson-1.0.5/ruson/core/instance.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/core/ruson_doc.py` & `ruson-1.0.5/ruson/core/ruson_doc.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/client.py` & `ruson-1.0.5/ruson/driver/client.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/collection.py` & `ruson-1.0.5/ruson/driver/collection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/collection.pyi` & `ruson-1.0.5/ruson/driver/collection.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/database.py` & `ruson-1.0.5/ruson/driver/database.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/results.py` & `ruson-1.0.5/ruson/driver/results.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/results.pyi` & `ruson-1.0.5/ruson/driver/results.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/types.py` & `ruson-1.0.5/ruson/driver/types.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/ruson/driver/types.pyi` & `ruson-1.0.5/ruson/driver/types.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/bson_binding.rs` & `ruson-1.0.5/src/bindings/bson_binding.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-use std::{fmt::Display, num::ParseIntError};
+use std::{fmt::Display, num::ParseIntError, time::SystemTime};
 
 use mongodb::{self, bson};
 
 use super::utils::PyNone;
 use pyo3::{
     prelude::*,
-    types::{PyBool, PyBytes, PyDateTime, PyFloat, PyInt, PyList, PyString, PyType},
+    types::{timezone_utc, PyBool, PyBytes, PyDateTime, PyFloat, PyInt, PyList, PyString, PyType},
 };
 
 use super::document_binding::Document;
 
 const BINARY_SUBTYPE_USER_DEFINED: u8 = 0x80;
 
 #[pyclass(frozen, module = "ruson.types")]
@@ -440,16 +440,20 @@
                     subtype: binary_subtype,
                     bytes: v.bytes,
                 };
                 value.into_py(py)
             }
             bson::Bson::ObjectId(v) => ObjectId { id: v.bytes() }.into_py(py),
             bson::Bson::DateTime(v) => {
-                let timestamp = v.timestamp_millis() as f64 / 60.0;
-                let value = PyDateTime::from_timestamp(py, timestamp, None);
+                let duration = v
+                    .to_system_time()
+                    .duration_since(SystemTime::UNIX_EPOCH)
+                    .unwrap();
+                let timestamp = duration.as_secs_f64();
+                let value = PyDateTime::from_timestamp(py, timestamp, Some(timezone_utc(py)));
                 match value {
                     Ok(v) => v.into_py(py),
                     Err(e) => e.into_py(py),
                 }
             }
             bson::Bson::Decimal128(v) => {
                 let value = Decimal128 { bytes: v.bytes() };
```

### Comparing `ruson-1.0.4/src/bindings/client_binding.rs` & `ruson-1.0.5/src/bindings/client_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/collection_binding.rs` & `ruson-1.0.5/src/bindings/collection_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/database_biding.rs` & `ruson-1.0.5/src/bindings/database_biding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/document_binding.rs` & `ruson-1.0.5/src/bindings/document_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/index_binding.rs` & `ruson-1.0.5/src/bindings/index_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/iterator_binding.rs` & `ruson-1.0.5/src/bindings/iterator_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/mod.rs` & `ruson-1.0.5/src/bindings/mod.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/bindings/results_binding.rs` & `ruson-1.0.5/src/bindings/results_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/src/interface.rs` & `ruson-1.0.5/src/interface.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/conftest.py` & `ruson-1.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_connection.py` & `ruson-1.0.5/tests/test_core/test_connection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_delete.py` & `ruson-1.0.5/tests/test_core/test_delete.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_distinct.py` & `ruson-1.0.5/tests/test_core/test_distinct.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_find.py` & `ruson-1.0.5/tests/test_core/test_find.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_indexes.py` & `ruson-1.0.5/tests/test_core/test_indexes.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_insert.py` & `ruson-1.0.5/tests/test_core/test_insert.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_update.py` & `ruson-1.0.5/tests/test_core/test_update.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_core/test_upsert.py` & `ruson-1.0.5/tests/test_core/test_upsert.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_driver/test_client.py` & `ruson-1.0.5/tests/test_driver/test_client.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_driver/test_collection.py` & `ruson-1.0.5/tests/test_driver/test_collection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/tests/test_driver/test_db.py` & `ruson-1.0.5/tests/test_driver/test_db.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/Cargo.lock` & `ruson-1.0.5/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.7"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
@@ -43,34 +43,34 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -114,70 +114,67 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bson"
-version = "2.8.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88c18b51216e1f74b9d769cead6ace2f82b965b807e3d73330aabe9faec31c84"
+checksum = "4d43b38e074cc0de2957f10947e376a1d88b9c4dbab340b590800cc1b2e066b2"
 dependencies = [
  "ahash",
  "base64 0.13.1",
  "bitvec",
  "hex",
- "indexmap 1.9.3",
+ "indexmap",
  "js-sys",
  "once_cell",
  "rand",
  "serde",
  "serde_bytes",
  "serde_json",
  "time",
  "uuid",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
@@ -389,15 +386,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -434,52 +431,46 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
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
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-
-[[package]]
-name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -501,17 +492,17 @@
  "libc",
  "match_cfg",
  "winapi",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.59"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6a67363e2aa4443928ce15e57ebae94fd8949958fd1223c4cfc0cd473ad7539"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -551,82 +542,72 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
-dependencies = [
- "autocfg",
- "hashbrown 0.12.3",
-]
-
-[[package]]
-name = "indexmap"
-version = "2.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "ipconfig"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b58db92f96b720de98181bbbe63c831e87005ab460c1bf306eb2622b4707997f"
 dependencies = [
- "socket2 0.5.5",
+ "socket2 0.5.6",
  "widestring",
- "windows-sys",
+ "windows-sys 0.48.0",
  "winreg",
 ]
 
 [[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.67"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -638,17 +619,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lru-cache"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e24f1ad8321ca0e8a1e0ac13f23cb668e6f5466c2c57319f6a5cf1cc8e3b1c"
 dependencies = [
@@ -675,52 +656,52 @@
 dependencies = [
  "cfg-if",
  "digest",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mongodb"
-version = "2.8.0"
+version = "2.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46c30763a5c6c52079602be44fa360ca3bfacee55fca73f4734aecd23706a7f2"
+checksum = "ef206acb1b72389b49bc9985efe7eb1f8a9bb18e5680d262fac26c07f44025f1"
 dependencies = [
  "async-trait",
  "base64 0.13.1",
  "bitflags",
  "bson",
  "chrono",
  "derivative",
@@ -756,18 +737,24 @@
  "trust-dns-resolver",
  "typed-builder",
  "uuid",
  "webpki-roots",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -829,17 +816,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -853,17 +840,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.76"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.2"
@@ -953,17 +940,17 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
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
 name = "radium"
 version = "0.7.0"
@@ -1017,29 +1004,30 @@
 dependencies = [
  "hostname",
  "quick-error",
 ]
 
 [[package]]
 name = "ring"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "688c63d65483050968b2a8937f7995f443e27041a0f7700aa59b0822aedebb74"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
+ "cfg-if",
  "getrandom",
  "libc",
  "spin",
  "untrusted",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ruson"
-version = "1.0.4"
+version = "1.0.5"
 dependencies = [
  "mongodb",
  "pyo3",
  "pyo3-asyncio",
  "serde",
  "tokio",
 ]
@@ -1061,15 +1049,15 @@
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "semver 1.0.21",
+ "semver 1.0.22",
 ]
 
 [[package]]
 name = "rustc_version_runtime"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d31b7153270ebf48bf91c65ae5b0c00e749c4cfad505f66530ac74950249582f"
@@ -1107,17 +1095,17 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
@@ -1138,29 +1126,29 @@
 checksum = "1d7eb9ef2c18661902cc47e535f9bc51b78acd254da71d375c2f6720d9a40403"
 dependencies = [
  "semver-parser",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.21"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -1168,30 +1156,30 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_with"
@@ -1253,36 +1241,36 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.12.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2593d31f82ead8df961d8bd23a64c2ccf2eb5dd34b0a34bfb4dd54011c72009e"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f7916fc008ca5542385b89a3d3ce689953c143e9304a9bf8beec1de48994c0d"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -1319,17 +1307,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1342,64 +1330,66 @@
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.31"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f657ba42c3f86e7680e53c8cd3af8abbe56b5491790b46e22e19c0d57463583e"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
+ "num-conv",
  "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26197e33420244aeb70c3e8c78376ca46571bc4e701e4791c2cd9f57dcb3a43f"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1412,39 +1402,39 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.35.1"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c89b4efa943be685f629b149f53829423f8f5531ea21249408e8e2f8671ec104"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.5.5",
+ "socket2 0.5.6",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -1527,29 +1517,29 @@
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f2528f27a9eb2b21e69c95319b30bd0efd85d09c379741b0f78ea1d86be2416"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
@@ -1571,17 +1561,17 @@
  "form_urlencoded",
  "idna 0.5.0",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.6.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e395fcf16a7a3d8127ec99782007af141946b4795001f876d54fb0d55978560"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "version_check"
@@ -1593,77 +1583,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "webpki-roots"
-version = "0.25.3"
+version = "0.25.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1778a42e8b3b90bff8d0f5032bf22250792889a5cdc752aa0020c84abe3aaf10"
+checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
 
 [[package]]
 name = "widestring"
-version = "1.0.2"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
+checksum = "7219d36b6eac893fa81e84ebe06485e7dcbb616177469b142df14f1f4deb1311"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -1685,27 +1675,36 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.5",
  "windows_aarch64_msvc 0.48.5",
@@ -1714,119 +1713,126 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
@@ -1847,9 +1853,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
```

### Comparing `ruson-1.0.4/pyproject.toml` & `ruson-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ruson-1.0.4/PKG-INFO` & `ruson-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ruson
-Version: 1.0.4
+Version: 1.0.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pydantic >=2.5
 Requires-Dist: pytz
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
```

