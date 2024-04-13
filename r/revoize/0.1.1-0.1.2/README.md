# Comparing `tmp/revoize-0.1.1.tar.gz` & `tmp/revoize-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revoize-0.1.1.tar", max compression
+gzip compressed data, was "revoize-0.1.2.tar", max compression
```

## Comparing `revoize-0.1.1.tar` & `revoize-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1068 2024-04-11 09:42:11.101682 revoize-0.1.1/LICENSE
--rw-r--r--   0        0        0     3239 2024-04-13 18:10:23.269317 revoize-0.1.1/README.md
--rw-r--r--   0        0        0     3439 2024-04-13 18:13:38.366984 revoize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       67 2024-04-11 09:42:11.103545 revoize-0.1.1/revoize/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 09:42:11.103593 revoize-0.1.1/revoize/api/__init__.py
--rw-r--r--   0        0        0    10299 2024-04-11 09:42:11.104027 revoize-0.1.1/revoize/api/client.py
--rw-r--r--   0        0        0      209 2024-04-11 09:42:11.104307 revoize-0.1.1/revoize/api/exceptions.py
--rw-r--r--   0        0        0     1186 2024-04-11 09:42:11.104589 revoize-0.1.1/revoize/api/utils.py
--rw-r--r--   0        0        0       45 2024-04-11 09:42:11.104871 revoize-0.1.1/revoize/auth/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-11 09:42:11.105060 revoize-0.1.1/revoize/auth/auth.py
--rw-r--r--   0        0        0      103 2024-04-11 09:42:11.105306 revoize-0.1.1/revoize/auth/exceptions.py
--rw-r--r--   0        0        0      143 2024-04-11 09:42:11.105495 revoize-0.1.1/revoize/defaults.py
--rw-r--r--   0        0        0      555 2024-04-11 09:42:11.105770 revoize-0.1.1/revoize/schema/__init__.py
--rw-r--r--   0        0        0     2996 2024-04-11 09:42:11.106046 revoize-0.1.1/revoize/schema/schema.py
--rw-r--r--   0        0        0     3901 1970-01-01 00:00:00.000000 revoize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 09:42:11.101682 revoize-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3239 2024-04-13 18:10:23.269317 revoize-0.1.2/README.md
+-rw-r--r--   0        0        0     3431 2024-04-13 18:25:33.772158 revoize-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-04-11 09:42:11.103545 revoize-0.1.2/revoize/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:42:11.103593 revoize-0.1.2/revoize/api/__init__.py
+-rw-r--r--   0        0        0    10299 2024-04-11 09:42:11.104027 revoize-0.1.2/revoize/api/client.py
+-rw-r--r--   0        0        0      209 2024-04-11 09:42:11.104307 revoize-0.1.2/revoize/api/exceptions.py
+-rw-r--r--   0        0        0     1186 2024-04-11 09:42:11.104589 revoize-0.1.2/revoize/api/utils.py
+-rw-r--r--   0        0        0       45 2024-04-11 09:42:11.104871 revoize-0.1.2/revoize/auth/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-11 09:42:11.105060 revoize-0.1.2/revoize/auth/auth.py
+-rw-r--r--   0        0        0      103 2024-04-11 09:42:11.105306 revoize-0.1.2/revoize/auth/exceptions.py
+-rw-r--r--   0        0        0     1488 2024-04-11 09:42:11.106524 revoize-0.1.2/revoize/cli/enhance.py
+-rw-r--r--   0        0        0      143 2024-04-11 09:42:11.105495 revoize-0.1.2/revoize/defaults.py
+-rw-r--r--   0        0        0      555 2024-04-11 09:42:11.105770 revoize-0.1.2/revoize/schema/__init__.py
+-rw-r--r--   0        0        0     2996 2024-04-11 09:42:11.106046 revoize-0.1.2/revoize/schema/schema.py
+-rw-r--r--   0        0        0     3901 1970-01-01 00:00:00.000000 revoize-0.1.2/PKG-INFO
```

### Comparing `revoize-0.1.1/LICENSE` & `revoize-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/README.md` & `revoize-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/pyproject.toml` & `revoize-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "revoize"
-version = "0.1.1"
+version = "0.1.2"
 description = "Revoize Python SDK"
 authors = ["Revoize <office@revoize.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 1 - Planning"
 ]
@@ -35,15 +35,15 @@
 pytest-mock = "^3.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-revoize-enhance = "revoize.scripts.enhance_cli:_enhance"
+revoize-enhance = "revoize.cli.enhance:_enhance"
 
 [tool.black]
 line-length = 88
 target-version = ["py311"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `revoize-0.1.1/revoize/api/client.py` & `revoize-0.1.2/revoize/api/client.py`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/revoize/api/utils.py` & `revoize-0.1.2/revoize/api/utils.py`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/revoize/auth/auth.py` & `revoize-0.1.2/revoize/auth/auth.py`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/revoize/schema/__init__.py` & `revoize-0.1.2/revoize/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/revoize/schema/schema.py` & `revoize-0.1.2/revoize/schema/schema.py`

 * *Files identical despite different names*

### Comparing `revoize-0.1.1/PKG-INFO` & `revoize-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revoize
-Version: 0.1.1
+Version: 0.1.2
 Summary: Revoize Python SDK
 License: MIT
 Author: Revoize
 Author-email: office@revoize.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
```

