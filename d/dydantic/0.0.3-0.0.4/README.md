# Comparing `tmp/dydantic-0.0.3.tar.gz` & `tmp/dydantic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dydantic-0.0.3.tar", max compression
+gzip compressed data, was "dydantic-0.0.4.tar", max compression
```

## Comparing `dydantic-0.0.3.tar` & `dydantic-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.3/LICENSE
--rw-r--r--   0        0        0     2600 2024-04-06 13:28:56.991037 dydantic-0.0.3/README.md
--rw-r--r--   0        0        0     1979 2024-04-06 13:32:51.195176 dydantic-0.0.3/dydantic/__init__.py
--rw-r--r--   0        0        0    18163 2024-04-06 14:35:44.161983 dydantic-0.0.3/dydantic/_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.3/dydantic/py.typed
--rw-r--r--   0        0        0     1312 2024-04-06 15:00:14.289100 dydantic-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 dydantic-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2847 2024-04-12 23:11:08.576469 dydantic-0.0.4/README.md
+-rw-r--r--   0        0        0     1979 2024-04-08 06:06:13.745492 dydantic-0.0.4/dydantic/__init__.py
+-rw-r--r--   0        0        0    18614 2024-04-12 23:39:20.289421 dydantic-0.0.4/dydantic/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.4/dydantic/py.typed
+-rw-r--r--   0        0        0     1312 2024-04-12 23:39:20.289839 dydantic-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 dydantic-0.0.4/PKG-INFO
```

### Comparing `dydantic-0.0.3/LICENSE` & `dydantic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.3/README.md` & `dydantic-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # dydantic
 
+[![Documentation](https://img.shields.io/badge/docs-hinthornw.github.io%2Fdydantic-blue)](https://hinthornw.github.io/dydantic/) [![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-black?logo=github)](https://github.com/hinthornw/dydantic)
+
 <p align="left">
   <img src="https://raw.githubusercontent.com/hinthornw/dydantic/main/docs/docs/static/img/dyno.svg" width="100" alt="dyno">
 </p>
 
+
 Dydantic is a Python library for dynamically generating Pydantic models from JSON schemas. It provides a convenient way to create Pydantic models on-the-fly based on the structure defined in a JSON schema.
 
 ## Features
 
 - Automatically generate Pydantic models from JSON schemas
 - Support for nested objects and referenced definitions
 - Customizable model configurations, base classes, and validators
```

### Comparing `dydantic-0.0.3/dydantic/__init__.py` & `dydantic-0.0.4/dydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.3/dydantic/_utils.py` & `dydantic-0.0.4/dydantic/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,15 +327,15 @@
             ...         },
             ...     },
             ... }
             >>> Matrix = create_model_from_schema(json_schema)
             >>> matrix = Matrix(value=[[1, 2, 3], [4, 5, 6], [7, 8, 9]])
             >>> matrix
             Matrix(value=[[1, 2, 3], [4, 5, 6], [7, 8, 9]])
-    
+
     """  # noqa: E501
     model_name = json_schema.get("title", "DynamicModel")
     field_definitions = {
         name: _json_schema_to_pydantic_field(
             name, prop, json_schema.get("required", []), root_schema or json_schema
         )
         for name, prop in (json_schema.get("properties", {}) or {}).items()
@@ -454,22 +454,35 @@
         else:
             ref_schema = root_schema
             start_idx = 1
         for path in ref_path[start_idx:]:
             ref_schema = ref_schema[path]
         return _json_schema_to_pydantic_type(ref_schema, root_schema, name_=name_)
 
-    any_of_schemas = json_schema.get("anyOf")
+    any_of_schemas = []
+    if "anyOf" in json_schema or "oneOf" in json_schema:
+        any_of_schemas = json_schema.get("anyOf", []) + json_schema.get("oneOf", [])
     if any_of_schemas:
         any_of_types = [
             _json_schema_to_pydantic_type(schema, root_schema)
             for schema in any_of_schemas
         ]
         return Union[tuple(any_of_types)]
 
+    all_of_schemas = json_schema.get("allOf")
+    if all_of_schemas:
+        all_of_types = [
+            _json_schema_to_pydantic_type(schema, root_schema)
+            for schema in all_of_schemas
+        ]
+        if len(all_of_types) == 1:
+            return all_of_types[0]
+        breakpoint()
+        return tuple(all_of_types)
+
     type_ = json_schema.get("type")
 
     if type_ == "string":
         return str
     elif type_ == "integer":
         return int
     elif type_ == "number":
```

### Comparing `dydantic-0.0.3/pyproject.toml` & `dydantic-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dydantic"
-version = "0.0.3"
+version = "0.0.4"
 description = "Dynamically generate pydantic models from JSON schema."
 authors = ["William Fu-Hinthorn <13333726+hinthornw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dydantic-0.0.3/PKG-INFO` & `dydantic-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dydantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dynamically generate pydantic models from JSON schema.
 License: MIT
 Author: William Fu-Hinthorn
 Author-email: 13333726+hinthornw@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2,<3)
 Description-Content-Type: text/markdown
 
 # dydantic
 
+[![Documentation](https://img.shields.io/badge/docs-hinthornw.github.io%2Fdydantic-blue)](https://hinthornw.github.io/dydantic/) [![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-black?logo=github)](https://github.com/hinthornw/dydantic)
+
 <p align="left">
   <img src="https://raw.githubusercontent.com/hinthornw/dydantic/main/docs/docs/static/img/dyno.svg" width="100" alt="dyno">
 </p>
 
+
 Dydantic is a Python library for dynamically generating Pydantic models from JSON schemas. It provides a convenient way to create Pydantic models on-the-fly based on the structure defined in a JSON schema.
 
 ## Features
 
 - Automatically generate Pydantic models from JSON schemas
 - Support for nested objects and referenced definitions
 - Customizable model configurations, base classes, and validators
```

