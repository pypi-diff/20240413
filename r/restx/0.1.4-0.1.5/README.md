# Comparing `tmp/restx-0.1.4.tar.gz` & `tmp/restx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restx-0.1.4.tar", max compression
+gzip compressed data, was "restx-0.1.5.tar", max compression
```

## Comparing `restx-0.1.4.tar` & `restx-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-13 08:36:11.424182 restx-0.1.4/LICENSE
--rw-r--r--   0        0        0       83 2024-04-13 10:09:24.428188 restx-0.1.4/README.md
--rw-r--r--   0        0        0     1160 2024-04-13 17:15:01.061193 restx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 08:02:36.161963 restx-0.1.4/restx/__init__.py
--rwxr-xr-x   0        0        0     1834 2024-04-13 16:41:40.187903 restx-0.1.4/restx/cli.py
--rw-r--r--   0        0        0      140 2024-04-13 16:17:32.113654 restx-0.1.4/restx/enums.py
--rw-r--r--   0        0        0     2780 2024-04-13 16:51:00.611191 restx-0.1.4/restx/utils.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 restx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 17:51:18.207713 restx-0.1.5/LICENSE
+-rw-r--r--   0        0        0      259 2024-04-13 17:51:18.207713 restx-0.1.5/README.md
+-rw-r--r--   0        0        0     1160 2024-04-13 17:51:18.207713 restx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 17:51:18.207713 restx-0.1.5/restx/__init__.py
+-rwxr-xr-x   0        0        0     1834 2024-04-13 17:51:18.207713 restx-0.1.5/restx/cli.py
+-rw-r--r--   0        0        0      140 2024-04-13 17:51:18.207713 restx-0.1.5/restx/enums.py
+-rw-r--r--   0        0        0     2780 2024-04-13 17:51:18.207713 restx-0.1.5/restx/utils.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 restx-0.1.5/PKG-INFO
```

### Comparing `restx-0.1.4/LICENSE` & `restx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `restx-0.1.4/pyproject.toml` & `restx-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "A CLI app for performing RESTX operations via HTTP requests."
 include = [
   "LICENSE",
 ]
 license = "MIT"
 name = "restx"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 httpx = "^0.27.0"
 python = ">=3.10,<4.0"
 rich = "^13.7.1"
 typer = "^0.12.3"
```

### Comparing `restx-0.1.4/restx/cli.py` & `restx-0.1.5/restx/cli.py`

 * *Files identical despite different names*

### Comparing `restx-0.1.4/restx/utils.py` & `restx-0.1.5/restx/utils.py`

 * *Files identical despite different names*

### Comparing `restx-0.1.4/PKG-INFO` & `restx-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: restx
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI app for performing RESTX operations via HTTP requests.
 License: MIT
 Author: Arjun Umathanu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # RESTX
+
 RESTX - A CLI app for performing RESTX operations via HTTP/HTTPS requests.
 
+[![CI/CD](https://github.com/fullstack-spiderman/restx/actions/workflows/ci.yml/badge.svg?event=push)](https://github.com/fullstack-spiderman/restx/actions/workflows/ci.yml)
+
```

