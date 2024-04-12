# Comparing `tmp/vulcan_utils-1.11.6.tar.gz` & `tmp/vulcan_utils-1.11.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.6.tar", last modified: Fri Apr 12 21:15:14 2024, max compression
+gzip compressed data, was "vulcan_utils-1.11.7.tar", last modified: Fri Apr 12 21:59:45 2024, max compression
```

## Comparing `vulcan_utils-1.11.6.tar` & `vulcan_utils-1.11.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.284408 vulcan_utils-1.11.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.398424 vulcan_utils-1.11.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11.6/LICENSE` & `vulcan_utils-1.11.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/PKG-INFO` & `vulcan_utils-1.11.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.6
+Version: 1.11.7
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
```

### Comparing `vulcan_utils-1.11.6/tests/test_decorator.py` & `vulcan_utils-1.11.7/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/tests/test_encoder.py` & `vulcan_utils-1.11.7/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/tests/test_formatter.py` & `vulcan_utils-1.11.7/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/tests/test_logger.py` & `vulcan_utils-1.11.7/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/tests/test_printable.py` & `vulcan_utils-1.11.7/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/vulcan_utils/decorator.py` & `vulcan_utils-1.11.7/vulcan_utils/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,16 @@
     """
     A collection of decorators designed to enhance function capabilities with additional behaviors such as logging,
     retrying on exceptions, converting return values to JSON, and rate-limiting function calls.his class primarily 
     serves as a namespace for decorator methods.
 
     This class implements static and class methods to provide utility functions that can be applied to other functions
     to log details about their calls and results, retry execution on failures, serialize outputs to JSON, and limit
-    the rate of function execution. T
-
-    Methods:
-        log: Decorates a function to log its call and return details, including execution time.
-        retry: Decorates a function to retry execution a specified number of times upon failure.
-        to_json: Decorates a function to serialize its return value to a JSON string using a custom encoder.
-        rate_limit: Decorates a function to limit its call rate to a specified threshold over a given time interval.
-    """
+    the rate of function execution.
+     """
 
     @staticmethod
     def _call_message(func: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
         """
         Constructs a log message string for function calls, including function name,
         positional arguments, and keyword arguments.
```

### Comparing `vulcan_utils-1.11.6/vulcan_utils/encoder.py` & `vulcan_utils-1.11.7/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/vulcan_utils/formatter.py` & `vulcan_utils-1.11.7/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/vulcan_utils/logger.py` & `vulcan_utils-1.11.7/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/vulcan_utils/printable.py` & `vulcan_utils-1.11.7/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.6/vulcan_utils.egg-info/PKG-INFO` & `vulcan_utils-1.11.7/vulcan_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.6
+Version: 1.11.7
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
```

