# Comparing `tmp/literal_dict-1.0.0.tar.gz` & `tmp/literal_dict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literal_dict-1.0.0.tar", last modified: Thu Jan 25 12:38:15 2024, max compression
+gzip compressed data, was "literal_dict-1.0.1.tar", last modified: Sat Apr 13 15:22:19 2024, max compression
```

## Comparing `literal_dict-1.0.0.tar` & `literal_dict-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       70 2024-01-24 14:18:16.224904 literal_dict-1.0.0/README.md
--rw-r--r--   0        0        0      637 2024-01-25 12:38:15.859596 literal_dict-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1190 2024-01-25 12:29:34.533132 literal_dict-1.0.0/src/literal_dict.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 literal_dict-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2823 2024-04-13 15:14:24.786745 literal_dict-1.0.1/README.md
+-rw-r--r--   0        0        0      637 2024-04-13 15:22:19.825087 literal_dict-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1664 2024-04-13 14:33:47.507045 literal_dict-1.0.1/src/literal_dict.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 literal_dict-1.0.1/PKG-INFO
```

### Comparing `literal_dict-1.0.0/pyproject.toml` & `literal_dict-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "literal-dict"
-version = "1.0.0"
+version = "1.0.1"
 description = "Use JavaScript-like object definition syntax in Python"
 authors = [
     { name = "Muspi Merol", email = "me@muspimerol.site" },
 ]
 dependencies = []
 requires-python = ">=3.6"
 readme = "README.md"
```

### Comparing `literal_dict-1.0.0/src/literal_dict.py` & `literal_dict-1.0.1/src/literal_dict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from inspect import currentframe
-from typing import Generic, Mapping, Sequence, Type, TypeVar, Union, cast
+from typing import Callable, Generic, Mapping, Sequence, TypeVar, Union, cast
 
 T = TypeVar("T")
 D = TypeVar("D", bound=Mapping)
 
 
 class DictBuilder(Generic[D]):
-    def __init__(self, mapping_type: Type[D] = dict):
-        self.mapping_type = mapping_type
+    def __init__(self, mapping_constructor: Callable[[dict], D] = dict):
+        self.constructor = mapping_constructor
 
     def __getitem__(self, args: Union[slice, T, Sequence[Union[slice, T]]]) -> D:
         if not isinstance(args, tuple):
             args = (args,)  # type: ignore
 
         frame = currentframe()
         assert frame, "Unable to get the current frame."
@@ -25,9 +25,19 @@
                 assert isinstance(arg.start, str), "Key must be a string"
                 obj[arg.start] = arg.stop
             else:
                 for name, var in caller_frame.f_locals.items():
                     if var is arg:
                         obj[name] = arg
                         break
+                else:
+                    for name, var in caller_frame.f_globals.items():
+                        if var is arg:
+                            obj[name] = arg
+                            break
+                    else:
+                        for name, var in caller_frame.f_builtins.items():
+                            if var is arg:
+                                obj[name] = arg
+                                break
 
-        return self.mapping_type(obj) if self.mapping_type is not dict else obj  # type: ignore
+        return self.constructor(obj) if self.constructor is not dict else obj  # type: ignore
```

