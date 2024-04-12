# Comparing `tmp/vulcan_utils-1.11.5.tar.gz` & `tmp/vulcan_utils-1.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.5.tar", last modified: Fri Apr 12 21:06:26 2024, max compression
+gzip compressed data, was "vulcan_utils-1.11.6.tar", last modified: Fri Apr 12 21:15:14 2024, max compression
```

## Comparing `vulcan_utils-1.11.5.tar` & `vulcan_utils-1.11.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:06:26.706986 vulcan_utils-1.11.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-12 21:06:26.706986 vulcan_utils-1.11.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:06:26.706986 vulcan_utils-1.11.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:06:26.702986 vulcan_utils-1.11.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:06:26.702986 vulcan_utils-1.11.5/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 21:06:18.000000 vulcan_utils-1.11.5/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:06:26.706986 vulcan_utils-1.11.5/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-12 21:06:26.000000 vulcan_utils-1.11.5/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:06:26.000000 vulcan_utils-1.11.5/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:06:26.000000 vulcan_utils-1.11.5/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 21:06:26.000000 vulcan_utils-1.11.5/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:06:26.000000 vulcan_utils-1.11.5/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.284408 vulcan_utils-1.11.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 21:15:04.000000 vulcan_utils-1.11.6/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:15:14.288408 vulcan_utils-1.11.6/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:15:14.000000 vulcan_utils-1.11.6/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11.5/LICENSE` & `vulcan_utils-1.11.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/PKG-INFO` & `vulcan_utils-1.11.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.5
+Version: 1.11.6
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
 
 Vulcan Utils is a Python package designed to enhance the logging capabilities of Python applications. It simplifies the logging process by automatically including critical details like the caller's filename and line number, making it easier to trace the source of log entries. The package supports a range of features including customizable log levels, colored logs, and conditional logging, tailored to improve both the development and debugging processes.
 
 **Requires Python 3.9 or higher**
 
-[View the full technical documentation here](https://vulcan-logger.readthedocs.io/en/latest/)
+[View the full technical documentation here](https://vulcan-utils.readthedocs.io/en/latest/)
 
 [View the PyPi project here](https://pypi.org/project/vulcan-utils/)
 
 ![Vulcan Utils](https://raw.githubusercontent.com/nodadyoushutup/vulcan-logger/main/docs/img/examples.png)
 
 ## Features
 - **Caller Information**: Vulcan Utils enriches every log entry with the caller's filename and line number, significantly easing the debugging process by providing immediate context for each message.
```

### Comparing `vulcan_utils-1.11.5/tests/test_decorator.py` & `vulcan_utils-1.11.6/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/tests/test_encoder.py` & `vulcan_utils-1.11.6/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/tests/test_formatter.py` & `vulcan_utils-1.11.6/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/tests/test_logger.py` & `vulcan_utils-1.11.6/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/tests/test_printable.py` & `vulcan_utils-1.11.6/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils/decorator.py` & `vulcan_utils-1.11.6/vulcan_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils/encoder.py` & `vulcan_utils-1.11.6/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils/formatter.py` & `vulcan_utils-1.11.6/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils/logger.py` & `vulcan_utils-1.11.6/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils/printable.py` & `vulcan_utils-1.11.6/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.5/vulcan_utils.egg-info/PKG-INFO` & `vulcan_utils-1.11.6/vulcan_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.5
+Version: 1.11.6
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
 
 Vulcan Utils is a Python package designed to enhance the logging capabilities of Python applications. It simplifies the logging process by automatically including critical details like the caller's filename and line number, making it easier to trace the source of log entries. The package supports a range of features including customizable log levels, colored logs, and conditional logging, tailored to improve both the development and debugging processes.
 
 **Requires Python 3.9 or higher**
 
-[View the full technical documentation here](https://vulcan-logger.readthedocs.io/en/latest/)
+[View the full technical documentation here](https://vulcan-utils.readthedocs.io/en/latest/)
 
 [View the PyPi project here](https://pypi.org/project/vulcan-utils/)
 
 ![Vulcan Utils](https://raw.githubusercontent.com/nodadyoushutup/vulcan-logger/main/docs/img/examples.png)
 
 ## Features
 - **Caller Information**: Vulcan Utils enriches every log entry with the caller's filename and line number, significantly easing the debugging process by providing immediate context for each message.
```

