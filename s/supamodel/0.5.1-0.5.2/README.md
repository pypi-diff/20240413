# Comparing `tmp/supamodel-0.5.1.tar.gz` & `tmp/supamodel-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.5.1.tar", max compression
+gzip compressed data, was "supamodel-0.5.2.tar", max compression
```

## Comparing `supamodel-0.5.1.tar` & `supamodel-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.5.1/README.md
--rw-r--r--   0        0        0      851 2024-04-11 20:50:11.018016 supamodel-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-10 06:14:30.018688 supamodel-0.5.1/supamodel/__init__.py
--rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.5.1/supamodel/_abc.py
--rw-r--r--   0        0        0      291 2024-04-11 18:39:05.846694 supamodel-0.5.1/supamodel/_client.py
--rw-r--r--   0        0        0     8016 2024-04-11 18:59:20.927159 supamodel-0.5.1/supamodel/_core.py
--rw-r--r--   0        0        0      674 2024-04-11 18:39:19.350451 supamodel-0.5.1/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.5.1/supamodel/_types.py
--rw-r--r--   0        0        0     1488 2024-04-11 18:28:24.659195 supamodel-0.5.1/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.5.1/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.5.1/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.5.1/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.5.1/supamodel/supa.py
--rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.5.1/supamodel/supa_builder.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.5.1/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.5.1/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.5.1/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-11 19:20:04.370291 supamodel-0.5.1/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1336 2024-04-11 20:28:40.425359 supamodel-0.5.1/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.5.1/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.5.1/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11732 2024-04-11 20:48:42.298833 supamodel-0.5.1/supamodel/trading/tokens.py
--rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.5.1/supamodel/utils.py
--rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 supamodel-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3743 2024-04-12 18:11:41.266181 supamodel-0.5.2/README.md
+-rw-r--r--   0        0        0      874 2024-04-13 10:17:35.839837 supamodel-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-10 06:14:30.018688 supamodel-0.5.2/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.5.2/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-11 18:39:05.846694 supamodel-0.5.2/supamodel/_client.py
+-rw-r--r--   0        0        0     8016 2024-04-11 18:59:20.927159 supamodel-0.5.2/supamodel/_core.py
+-rw-r--r--   0        0        0      674 2024-04-11 18:39:19.350451 supamodel-0.5.2/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.5.2/supamodel/_types.py
+-rw-r--r--   0        0        0     1488 2024-04-11 18:28:24.659195 supamodel-0.5.2/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.5.2/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.5.2/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.5.2/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.5.2/supamodel/supa.py
+-rw-r--r--   0        0        0     3281 2024-04-12 18:18:16.342146 supamodel-0.5.2/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.5.2/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.5.2/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.5.2/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-11 19:20:04.370291 supamodel-0.5.2/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1336 2024-04-11 20:28:40.425359 supamodel-0.5.2/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.5.2/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.5.2/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11732 2024-04-11 20:48:42.298833 supamodel-0.5.2/supamodel/trading/tokens.py
+-rw-r--r--   0        0        0    17202 2024-04-13 07:22:12.056006 supamodel-0.5.2/supamodel/utils.py
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 supamodel-0.5.2/PKG-INFO
```

### Comparing `supamodel-0.5.1/README.md` & `supamodel-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Usage
 Once completed, you will be able to use SupaModel to define your own models that map to tables in your Supabase database. You can then create, read, update, and delete records in your database using these models.
 
 ## Future Work
 The project is still in its early stages, and there is a lot of work to be done. Future plans include adding more field types, relationships between models, and advanced query capabilities.
 
 
-## Orms vs supabase-py vs SupaModel
+## Orms vs `supabase-py` vs SupaModel
 
 
 You're absolutely right! Providing users with the flexibility to think about and interact with data in different ways is crucial for a robust and user-friendly library like supabase-py. Accommodating both composition-level thinking and aggregate/object-oriented thinking allows users to approach problems in a way that best suits their needs and preferences.
 
 Here are a few ideas to help achieve this balance:
 
 High-level table operations: Provide methods and classes that allow users to perform operations on entire tables, such as querying, filtering, sorting, and aggregating data. This enables users to think about data at a higher level and work with sets of records efficiently.
```

### Comparing `supamodel-0.5.1/pyproject.toml` & `supamodel-0.5.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
 pendulum = ">=2.0.0,<4.0.0"
@@ -17,24 +17,25 @@
 supabase = "^2.4.1"
 pandas = "^2.2.1"
 solana = "^0.33.0"
 orjson = "^3.10.0"
 diskcache = "^5.6.3"
 typer = "^0.12.3"
 solders = "^0.21.0"
+ormsgpack = "^1.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-testmon = "^2.1.1"
 devtools = "^0.12.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Create ruff configuration
 [tool.ruff]
 fixable = ["ALL"]
-ignore = ["F401"]
+# ignore = ["F401"]
 
 
 # docstring_code_format = false
```

### Comparing `supamodel-0.5.1/supamodel/_abc.py` & `supamodel-0.5.2/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/_core.py` & `supamodel-0.5.2/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/_logging.py` & `supamodel-0.5.2/supamodel/_logging.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/config.py` & `supamodel-0.5.2/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/enums.py` & `supamodel-0.5.2/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/exceptions.py` & `supamodel-0.5.2/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/supa.py` & `supamodel-0.5.2/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/supa_builder.py` & `supamodel-0.5.2/supamodel/supa_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,30 +6,20 @@
 
 The `SupaModel` class is used to represent a model that is stored in a Supabase database. We'll also have DecoratedRequestBuilders and SupaTypes in this module. They'll represent components that are used to interact with the Supabase API.
 
 
 """
 
 import uuid
-from typing import Any, Dict, Generic, List, Optional, TypeVar
+from typing import Any, Generic, TypeVar
 
-from postgrest._sync.request_builder import SyncQueryRequestBuilder
-from postgrest.base_request_builder import (
-    APIResponse,
-    BaseFilterRequestBuilder,
-    BaseRPCRequestBuilder,
-    BaseSelectRequestBuilder,
-    QueryArgs,
-    SingleAPIResponse,
-    _ReturnT,
-)
-from pydantic import BaseModel, ConfigDict, Field, field_serializer
+from postgrest._sync.request_builder import SyncRequestBuilder
 
 from supamodel._abc import Data, Dataset
-from supamodel._client import supabase
+from supamodel._client import client as supabase
 from supamodel.utils import cached_classattr, tableize
 
 RespT = TypeVar("RespT", bound=Data)
 
 
 class ResponseModel(Data, Generic[RespT]):
     data: list[dict[str, Any]] | None = []
@@ -67,15 +57,15 @@
 class SupaTable(Data):
 
     @classmethod
     def table_name(cls) -> str:
         return tableize(cls.__name__)
 
     @cached_classattr
-    def table(cls) -> SyncQueryRequestBuilder:
+    def table(cls) -> SyncRequestBuilder:
         return supabase.table(cls.table_name())
 
     @cached_classattr
     def class_type(cls):
         """
         Returns the class type of an instance created from the model. It must be an instance so tha we don't get the parent class type.
 
@@ -95,47 +85,27 @@
         return type(instance)
 
     @cached_classattr
     def dataset(cls):
         """
         Returns the dataset associated with the class.
         """
-        return Dataset[cls.class_type]
+        return Dataset[cls.resolved_type]
 
 
-class SupaRecord(Data):
+class SupaRecord(SupaTable):
     id: uuid.UUID | None = None
 
-    @classmethod
-    def table_name(cls) -> str:
-        return tableize(cls.__name__)
-
-    @cached_classattr
-    def table(cls) -> SyncQueryRequestBuilder:
-        return supabase.table(cls.table_name())
-
-    @cached_classattr
-    def class_type(cls):
-        """
-        Returns the class type of an instance created from the model. It must be an instance so tha we don't get the parent class type.
+    def save(self):
 
-        It would get ModelMetaClass instead of the current model normally instead.
-        """
-        instance = cls.model_construct({})
-        return type(instance)
+        return self.table.insert(self.model_dump(exclude_none=True, mode="json"))
 
-    @cached_classattr
-    def resolved_type(cls):
-        """
-        Returns the resolved type of an instance created from the model. It must be an instance so that we don't get the parent class type.
+    def delete(self):
+        return self.table.delete().eq("id", self.id).execute()
 
-        It would get ModelMetaClass instead of the current model normally instead.
-        """
-        instance = cls.model_construct({})
-        return type(instance)
+    def upsert(self):
+        return self.table.upsert(self.model_dump(exclude_none=True, mode="json"))
 
-    @cached_classattr
-    def dataset(cls):
-        """
-        Returns the dataset associated with the class.
-        """
-        return Dataset[cls.class_type]
+    def update(self):
+        json_model = self.model_dump(exclude_none=True, mode="json")
+        id = json_model.pop("id", None)
+        return self.table.eq("id", id).update(json_model)
```

### Comparing `supamodel-0.5.1/supamodel/trading/clock.py` & `supamodel-0.5.2/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/trading/exchange.py` & `supamodel-0.5.2/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/trading/market_data.py` & `supamodel-0.5.2/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/trading/order_management.py` & `supamodel-0.5.2/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/trading/portfolio.py` & `supamodel-0.5.2/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/trading/tokens.py` & `supamodel-0.5.2/supamodel/trading/tokens.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.1/supamodel/utils.py` & `supamodel-0.5.2/supamodel/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,50 +26,79 @@
 from concurrent.futures import ThreadPoolExecutor
 from functools import cached_property, wraps
 from pathlib import Path
 from typing import Any, Callable, Coroutine, TypeVar, cast
 
 import diskcache
 import orjson as json
+import ormsgpack as msgpack
+import pendulum as pdm
 import sniffio
 import typer
 from diskcache import UNKNOWN, Cache as LocalCache, memoize_stampede
 from inflector import Inflector
 from pydantic import BaseModel
 from sniffio import current_async_library
 
 # ---------------------------------------------------------
 # Cache utilities
 # ---------------------------------------------------------
 
 
+def default_json(obj):
+    if isinstance(obj, pdm.DateTime):
+        return obj.to_iso8601_string()
+    if isinstance(obj, Path):
+        return str(obj)
+    if isinstance(obj, BaseModel):
+        return obj.model_dump(mode="json", exclude_none=True)
+    if isinstance(obj, set):
+        return list(obj)
+    raise TypeError(f"Type {obj.__class__.__name__} is not JSON serializable")
+
+
+def default_msgpack(obj):
+    if isinstance(obj, pdm.DateTime):
+        return obj.to_iso8601_string()
+    if isinstance(obj, Path):
+        return str(obj)
+    if isinstance(obj, BaseModel):
+        return obj.model_dump(mode="json", exclude_none=True)
+    if isinstance(obj, set):
+        return list(obj)
+    raise TypeError(f"Type {obj.__class__.__name__} is not msgpack serializable")
+
+
 class JSONDisk(diskcache.Disk):
     def __init__(self, directory, compress_level=1, **kwargs):
         self.compress_level = compress_level
         super().__init__(directory, **kwargs)
 
     def put(self, key):
         json_bytes = json.dumps(
             key,
+            default=default_json,
             option=json.OPT_SERIALIZE_UUID
             | json.OPT_SORT_KEYS
             | json.OPT_NON_STR_KEYS
-            | json.OPT_SERIALIZE_DATACLASS,
+            | json.OPT_SERIALIZE_DATACLASS
+            | json.OPT_SERIALIZE_NUMPY,
         )
         data = zlib.compress(json_bytes, self.compress_level)
         return super().put(data)
 
     def get(self, key, raw):
         data = super().get(key, raw)
         return json.loads(zlib.decompress(data).decode("utf-8"))
 
     def store(self, value, read, key=UNKNOWN):
         if not read:
             json_bytes = json.dumps(
                 value,
+                default=default_json,
                 option=json.OPT_SERIALIZE_UUID
                 | json.OPT_SORT_KEYS
                 | json.OPT_NON_STR_KEYS
                 | json.OPT_SERIALIZE_DATACLASS,
             )
             value = zlib.compress(json_bytes, self.compress_level)
         return super().store(value, read, key=key)
@@ -77,14 +106,59 @@
     def fetch(self, mode, filename, value, read):
         data = super().fetch(mode, filename, value, read)
         if not read:
             data = json.loads(zlib.decompress(data).decode("utf-8"))
         return data
 
 
+class MsgPackDisk(diskcache.Disk):
+    def __init__(self, directory, compress_level=1, **kwargs):
+        self.compress_level = compress_level
+        super().__init__(directory, **kwargs)
+
+    def serialize(self, value):
+        return msgpack.packb(
+            value,
+            default=default_msgpack,
+            option=msgpack.OPT_NAIVE_UTC
+            | msgpack.OPT_SERIALIZE_NUMPY
+            | msgpack.OPT_SERIALIZE_PYDANTIC
+            | msgpack.OPT_SORT_KEYS,
+        )
+
+    def deserialize(self, data):
+        return msgpack.unpackb(
+            data,
+            option=msgpack.OPT_NAIVE_UTC
+            | msgpack.OPT_SERIALIZE_NUMPY
+            | msgpack.OPT_SERIALIZE_PYDANTIC
+            | msgpack.OPT_SORT_KEYS,
+        )
+
+    def deserialize_compressed(self, data):
+        return self.deserialize(zlib.decompress(data))
+
+    def serialize_compressed(self, value):
+        return zlib.compress(self.serialize(value), self.compress_level)
+
+    def put(self, key):
+        return super().put(key)
+
+    def get(self, key, raw):
+        return super().get(key, raw)
+
+    def store(self, value, read, key=...):
+        if not read:
+            value = self.serialize_compressed(value)
+        return super().store(value, read, key)
+
+    def fetch(self, mode, filename, value, read):
+        return super().fetch(mode, filename, value, read)
+
+
 class AppConfig(BaseModel):
     APP_NAME: str = "galapy"
     HOME: Path = Path.home()
     APP_DIR: str = typer.get_app_dir(APP_NAME, force_posix=True)
 
     @cached_property
     def app_dir(self) -> Path:
```

### Comparing `supamodel-0.5.1/PKG-INFO` & `supamodel-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: inflector (>=3.1.1,<4.0.0)
 Requires-Dist: loguru (>=0.5.0,<1.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: orjson (>=3.10.0,<4.0.0)
+Requires-Dist: ormsgpack (>=1.4.2,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pendulum (>=2.0.0,<4.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0,<=3.0.0)
 Requires-Dist: pydantic[email] (>=2.7.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: solana (>=0.33.0,<0.34.0)
 Requires-Dist: solders (>=0.21.0,<0.22.0)
@@ -36,15 +37,15 @@
 ## Usage
 Once completed, you will be able to use SupaModel to define your own models that map to tables in your Supabase database. You can then create, read, update, and delete records in your database using these models.
 
 ## Future Work
 The project is still in its early stages, and there is a lot of work to be done. Future plans include adding more field types, relationships between models, and advanced query capabilities.
 
 
-## Orms vs supabase-py vs SupaModel
+## Orms vs `supabase-py` vs SupaModel
 
 
 You're absolutely right! Providing users with the flexibility to think about and interact with data in different ways is crucial for a robust and user-friendly library like supabase-py. Accommodating both composition-level thinking and aggregate/object-oriented thinking allows users to approach problems in a way that best suits their needs and preferences.
 
 Here are a few ideas to help achieve this balance:
 
 High-level table operations: Provide methods and classes that allow users to perform operations on entire tables, such as querying, filtering, sorting, and aggregating data. This enables users to think about data at a higher level and work with sets of records efficiently.
```
