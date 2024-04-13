# Comparing `tmp/fnsecure-0.1.1.tar.gz` & `tmp/fnsecure-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnsecure-0.1.1.tar", max compression
+gzip compressed data, was "fnsecure-0.1.2.tar", max compression
```

## Comparing `fnsecure-0.1.1.tar` & `fnsecure-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2024-04-06 17:49:07.773963 fnsecure-0.1.1/LICENSE
--rw-r--r--   0        0        0     8949 2024-04-13 09:11:02.004860 fnsecure-0.1.1/README.md
--rw-r--r--   0        0        0       32 2024-04-06 18:09:40.402186 fnsecure-0.1.1/fnsecure/conditions/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-06 18:09:40.423186 fnsecure-0.1.1/fnsecure/conditions/conditions.py
--rw-r--r--   0        0        0      185 2024-04-13 09:12:46.198030 fnsecure-0.1.1/fnsecure/errors/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-07 06:23:49.793771 fnsecure-0.1.1/fnsecure/errors/errors.py
--rw-r--r--   0        0        0      133 2024-04-13 10:03:58.871455 fnsecure-0.1.1/fnsecure/exceptions/__init__.py
--rw-r--r--   0        0        0     6964 2024-04-13 09:12:46.318030 fnsecure-0.1.1/fnsecure/exceptions/exceptions.py
--rw-r--r--   0        0        0     4512 2024-04-13 09:12:46.314030 fnsecure-0.1.1/fnsecure/exceptions/functions.py
--rw-r--r--   0        0        0       50 2024-04-13 09:12:46.192030 fnsecure-0.1.1/fnsecure/fnsecure.py
--rw-r--r--   0        0        0      212 2024-04-13 09:12:46.197030 fnsecure-0.1.1/fnsecure/shared/__init__.py
--rw-r--r--   0        0        0     2562 2024-04-06 18:09:47.407199 fnsecure-0.1.1/fnsecure/shared/common.py
--rw-r--r--   0        0        0     2014 2024-04-06 18:09:47.410199 fnsecure-0.1.1/fnsecure/shared/exception_types.py
--rw-r--r--   0        0        0      462 2024-04-13 10:06:12.071629 fnsecure-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9487 1970-01-01 00:00:00.000000 fnsecure-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-06 17:49:07.773963 fnsecure-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8941 2024-04-13 13:29:28.334381 fnsecure-0.1.2/README.md
+-rw-r--r--   0        0        0       32 2024-04-06 18:09:40.402186 fnsecure-0.1.2/fnsecure/conditions/__init__.py
+-rw-r--r--   0        0        0     1281 2024-04-06 18:09:40.423186 fnsecure-0.1.2/fnsecure/conditions/conditions.py
+-rw-r--r--   0        0        0      185 2024-04-13 09:12:46.198030 fnsecure-0.1.2/fnsecure/errors/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-07 06:23:49.793771 fnsecure-0.1.2/fnsecure/errors/errors.py
+-rw-r--r--   0        0        0      133 2024-04-13 10:03:58.871455 fnsecure-0.1.2/fnsecure/exceptions/__init__.py
+-rw-r--r--   0        0        0     6964 2024-04-13 09:12:46.318030 fnsecure-0.1.2/fnsecure/exceptions/exceptions.py
+-rw-r--r--   0        0        0     4512 2024-04-13 09:12:46.314030 fnsecure-0.1.2/fnsecure/exceptions/functions.py
+-rw-r--r--   0        0        0       71 2024-04-13 10:20:15.474726 fnsecure-0.1.2/fnsecure/fnsecure.py
+-rw-r--r--   0        0        0      212 2024-04-13 09:12:46.197030 fnsecure-0.1.2/fnsecure/shared/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-13 13:27:21.806985 fnsecure-0.1.2/fnsecure/shared/common.py
+-rw-r--r--   0        0        0     2014 2024-04-06 18:09:47.410199 fnsecure-0.1.2/fnsecure/shared/exception_types.py
+-rw-r--r--   0        0        0      462 2024-04-13 13:44:50.941778 fnsecure-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9479 1970-01-01 00:00:00.000000 fnsecure-0.1.2/PKG-INFO
```

### Comparing `fnsecure-0.1.1/LICENSE` & `fnsecure-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/README.md` & `fnsecure-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 ```python
 from fnsecure.exceptions import handle
 from fnsecure.shared import ExceptionHandler
 from fnsecure.exceptions.functions import RetryWithFunction
 
 @handle(
-    "always_fail",
+    "foo",
     [
         ExceptionHandler(
             Exception, RetryWithFunction(lambda *args, **kwargs: "success", (), {})
         )
     ],
 )
 def function_using_foo():
```

### Comparing `fnsecure-0.1.1/fnsecure/conditions/conditions.py` & `fnsecure-0.1.2/fnsecure/conditions/conditions.py`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/fnsecure/errors/errors.py` & `fnsecure-0.1.2/fnsecure/errors/errors.py`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/fnsecure/exceptions/exceptions.py` & `fnsecure-0.1.2/fnsecure/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/fnsecure/exceptions/functions.py` & `fnsecure-0.1.2/fnsecure/exceptions/functions.py`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/fnsecure/shared/common.py` & `fnsecure-0.1.2/fnsecure/shared/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Type
+from typing import Dict, List, Type
 
 from .exception_types import ExceptionHandler
 
 
 @dataclass
 class FunctionDescriptor:
     """
@@ -27,18 +27,15 @@
 class Context:
     """
     Manages a given context and it contains all managed functions in this
     context.
     """
 
     def __init__(self) -> None:
-        self.a = 10
         self._functions: Dict[str, FunctionDescriptor] = {}
-        self._handler_group_attr_name = "_handler_list"
-        self._last_caller_attr_name = "_last_caller_name"
 
     def register(self, func_desc: FunctionDescriptor) -> None:
         """Register a function if it is not registered already."""
         _func = self._functions.get(func_desc.name, None)
         if _func:
             return
```

### Comparing `fnsecure-0.1.1/fnsecure/shared/exception_types.py` & `fnsecure-0.1.2/fnsecure/shared/exception_types.py`

 * *Files identical despite different names*

### Comparing `fnsecure-0.1.1/PKG-INFO` & `fnsecure-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnsecure
-Version: 0.1.1
+Version: 0.1.2
 Summary: Make python functions more secure and descriptive.
 License: GNU GENERAL PUBLIC LICENSE  Version 2
 Author: richard-rikk
 Author-email: rikk.richard@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -211,15 +211,15 @@
 
 ```python
 from fnsecure.exceptions import handle
 from fnsecure.shared import ExceptionHandler
 from fnsecure.exceptions.functions import RetryWithFunction
 
 @handle(
-    "always_fail",
+    "foo",
     [
         ExceptionHandler(
             Exception, RetryWithFunction(lambda *args, **kwargs: "success", (), {})
         )
     ],
 )
 def function_using_foo():
```

