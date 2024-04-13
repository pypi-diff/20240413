# Comparing `tmp/picle-0.5.1.tar.gz` & `tmp/picle-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picle-0.5.1.tar", max compression
+gzip compressed data, was "picle-0.5.2.tar", max compression
```

## Comparing `picle-0.5.1.tar` & `picle-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.5.1/LICENSE
--rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.5.1/picle/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.5.1/picle/cache.py
--rw-r--r--   0        0        0     5347 2024-04-07 03:30:27.671853 picle-0.5.1/picle/models.py
--rw-r--r--   0        0        0    33606 2024-04-07 03:30:27.672845 picle-0.5.1/picle/picle.py
--rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.5.1/picle/utils.py
--rw-r--r--   0        0        0     1659 2024-04-07 03:30:37.436704 picle-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.5.1/README.md
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 picle-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.5.2/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.5.2/picle/__init__.py
+-rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.5.2/picle/cache.py
+-rw-r--r--   0        0        0     5267 2024-04-13 21:16:46.255110 picle-0.5.2/picle/models.py
+-rw-r--r--   0        0        0    34002 2024-04-07 05:51:45.023230 picle-0.5.2/picle/picle.py
+-rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.5.2/picle/utils.py
+-rw-r--r--   0        0        0     1659 2024-04-13 21:17:02.565143 picle-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.5.2/README.md
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 picle-0.5.2/PKG-INFO
```

### Comparing `picle-0.5.1/LICENSE` & `picle-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `picle-0.5.1/picle/cache.py` & `picle-0.5.2/picle/cache.py`

 * *Files identical despite different names*

### Comparing `picle-0.5.1/picle/models.py` & `picle-0.5.2/picle/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,21 +117,17 @@
     @staticmethod
     def formatter_kv(data: dict) -> str:
         """
         Function to format dictionary result as a key: value output
 
         :param data: dictionary to format
         """
-        return "\n".join(
-            [
-                f" {k}: {v}" for k, v in data.items()
-            ]
-        )        
-        
-        
+        return "\n".join([f" {k}: {v}" for k, v in data.items()])
+
+
 class Outputters(BaseModel):
     rich_json: Union[dict, list] = Field(
         None,
         description="Pretty print JSON string using Rich",
         json_schema_extra={"function": "outputter_rich_json"},
     )
     rich_print: Any = Field(
```

### Comparing `picle-0.5.1/picle/picle.py` & `picle-0.5.2/picle/picle.py`

 * *Files 2% similar despite different names*

```diff
@@ -624,24 +624,27 @@
                     # run model "run" function if it exits
                     model = command[-1]["model"]
                     if command_arguments and hasattr(model, "run"):
                         # validate command argument values
                         self._validate_values(command)
                         # call first command using collected arguments only
                         if index == 0:
-                            ret = model.run(
+                            kw = {
                                 **self.shell_defaults,
                                 **command_defaults,
                                 **command_arguments,
-                            )
+                            }
+                            ret = model.run(**kw)
                         # pipe results through subsequent commands
                         else:
-                            ret = model.run(
-                                ret, **command_defaults, **command_arguments
-                            )
+                            kw = {
+                                **command_defaults,
+                                **command_arguments,
+                            }
+                            ret = model.run(ret, **kw)
                         # run processors from PicleConfig if any for first command only
                         if index == 0:
                             if hasattr(model, "PicleConfig") and hasattr(
                                 model.PicleConfig, "processors"
                             ):
                                 for processor in model.PicleConfig.processors:
                                     if callable(processor):
@@ -683,45 +686,51 @@
                         )
                         # check if last field refers to callable e.g. function
                         if last_field.annotation is Callable:
                             method_name = last_field.get_default()
                             if method_name and hasattr(model, method_name):
                                 # call first command using collected arguments only
                                 if index == 0:
-                                    ret = getattr(model, method_name)(
+                                    kw = {
                                         **self.shell_defaults,
                                         **command_defaults,
                                         **command_arguments,
-                                    )
+                                    }
+                                    ret = getattr(model, method_name)(**kw)
                                 # pipe results through subsequent commands
                                 else:
-                                    ret = getattr(model, method_name)(
-                                        ret, **command_defaults, **command_arguments
-                                    )
+                                    kw = {
+                                        **command_defaults,
+                                        **command_arguments,
+                                    }
+                                    ret = getattr(model, method_name)(ret, **kw)
                             else:
                                 self.write(
                                     f"Model '{model.__name__}' has no '{method_name}' "
                                     f"method defined for '{last_field_name}' Callable field"
                                 )
                         # check if last field has `function` parameter defined
                         elif json_schema_extra.get("function"):
                             method_name = json_schema_extra["function"]
                             if hasattr(model, method_name):
                                 # call first command using collected arguments only
                                 if index == 0:
-                                    ret = getattr(model, method_name)(
+                                    kw = {
                                         **self.shell_defaults,
                                         **command_defaults,
                                         **command_arguments,
-                                    )
+                                    }
+                                    ret = getattr(model, method_name)(**kw)
                                 # pipe results through subsequent commands
                                 else:
-                                    ret = getattr(model, method_name)(
-                                        ret, **command_defaults, **command_arguments
-                                    )
+                                    kw = {
+                                        **command_defaults,
+                                        **command_arguments,
+                                    }
+                                    ret = getattr(model, method_name)(ret, **kw)
                             else:
                                 self.write(
                                     f"Model '{model.__name__}' has no '{method_name}' "
                                     f"method defined for '{last_field_name}' function"
                                 )
                         else:
                             self.write(
```

### Comparing `picle-0.5.1/pyproject.toml` & `picle-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "picle"
-version = "0.5.1"
+version = "0.5.2"
 description = "Python Interactive Command Line Shells"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/picle"
 repository = "https://github.com/dmulyalin/picle"
 documentation = "https://dmulyalin.github.io/picle/"
```

### Comparing `picle-0.5.1/README.md` & `picle-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `picle-0.5.1/PKG-INFO` & `picle-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picle
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python Interactive Command Line Shells
 Home-page: https://github.com/dmulyalin/picle
 License: MIT
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

