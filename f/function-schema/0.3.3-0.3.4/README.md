# Comparing `tmp/function_schema-0.3.3.tar.gz` & `tmp/function_schema-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_schema-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "function_schema-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `function_schema-0.3.3.tar` & `function_schema-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4208 2024-04-09 06:48:17.632099 function_schema-0.3.3/README.md
--rw-r--r--   0        0        0      192 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/__init__.py
--rw-r--r--   0        0        0     1338 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/cli.py
--rw-r--r--   0        0        0     5964 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/core.py
--rw-r--r--   0        0        0      872 2024-04-09 06:48:17.632099 function_schema-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 function_schema-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4208 2024-04-13 09:20:19.340353 function_schema-0.3.4/README.md
+-rw-r--r--   0        0        0      192 2024-04-13 09:20:19.340353 function_schema-0.3.4/function_schema/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-13 09:20:19.340353 function_schema-0.3.4/function_schema/cli.py
+-rw-r--r--   0        0        0     6306 2024-04-13 09:20:19.340353 function_schema-0.3.4/function_schema/core.py
+-rw-r--r--   0        0        0      872 2024-04-13 09:20:19.340353 function_schema-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 function_schema-0.3.4/PKG-INFO
```

### Comparing `function_schema-0.3.3/README.md` & `function_schema-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `function_schema-0.3.3/function_schema/cli.py` & `function_schema-0.3.4/function_schema/cli.py`

 * *Files identical despite different names*

### Comparing `function_schema-0.3.3/function_schema/core.py` & `function_schema-0.3.4/function_schema/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import platform
 import packaging.version
 
 current_version = packaging.version.parse(platform.python_version())
 py_310 = packaging.version.parse("3.10")
 
 if current_version >= py_310:
-    import types
     from types import UnionType
 else:
     UnionType = typing.Union  # type: ignore
 
 
 def get_function_schema(
     func: typing.Annotated[typing.Callable, "The function to get the schema for"],
@@ -110,28 +109,34 @@
 
         schema["properties"][name] = {
             "type": guess_type(T),
             "description": description,  # type: ignore
         }
 
         if enum_ is not None:
-            schema["properties"][name]["enum"] = [t for t in enum_]
+            schema["properties"][name]["enum"] = [t for t in enum_ if t is not None]
 
         if default_value is not inspect._empty:
             schema["properties"][name]["default"] = default_value
 
         if (
             typing.get_origin(T) is not typing.Literal
             and not isinstance(None, T)
             and default_value is inspect._empty
         ):
             schema["required"].append(name)
 
+        if typing.get_origin(T) is typing.Literal:
+            if all(typing.get_args(T)):
+                schema["required"].append(name)
+
     parms_key = "input_schema" if format == "claude" else "parameters"
 
+    schema["required"] = list(set(schema["required"]))
+
     return {
         "name": func.__name__,
         "description": inspect.getdoc(func),
         parms_key: schema,
     }
 
 
@@ -144,32 +149,37 @@
 
     # special case
     if T is typing.Any:
         return {}
 
     origin = typing.get_origin(T)
 
+    if origin is typing.Annotated:
+        return guess_type(typing.get_args(T)[0])
+
     # hacking around typing modules, `typing.Union` and `types.UnitonType`
-    if origin is typing.Union or origin is UnionType:
+    if origin in [typing.Union, UnionType]:
         union_types = [t for t in typing.get_args(T) if t is not type(None)]
-        _types = []
-        for union_type in union_types:
-            _types.append(guess_type(union_type))
-        _types = [t for t in _types if t is not None]  # exclude None
+        _types = [
+            guess_type(union_type)
+            for union_type in union_types
+            if guess_type(union_type) is not None
+        ]
 
         # number contains integer in JSON schema
         if "number" in _types and "integer" in _types:
             _types.remove("integer")
 
         if len(_types) == 1:
             return _types[0]
         return _types
 
     if origin is typing.Literal:
-        return "string"
+        type_args = typing.Union[tuple(type(arg) for arg in typing.get_args(T))]
+        return guess_type(type_args)
     elif origin is list or origin is tuple:
         return "array"
     elif origin is dict:
         return "object"
 
     if not isinstance(T, type):
         return
```

### Comparing `function_schema-0.3.3/pyproject.toml` & `function_schema-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "function-schema"
-version = "0.3.3"
+version = "0.3.4"
 requires-python = ">= 3.9"
 description = "A small utility to generate JSON schemas for python functions."
 readme = "README.md"
 license = {text = "MIT License"}
 authors = [
   {name = "Changkyun Kim", email = "comfuture@gmail.com"}
 ]
```

### Comparing `function_schema-0.3.3/PKG-INFO` & `function_schema-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-schema
-Version: 0.3.3
+Version: 0.3.4
 Summary: A small utility to generate JSON schemas for python functions.
 Keywords: json-schema,function,documentation,openai,utility
 Author-email: Changkyun Kim <comfuture@gmail.com>
 Maintainer-email: Changkyun Kim <comfuture@gmail.com>
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

