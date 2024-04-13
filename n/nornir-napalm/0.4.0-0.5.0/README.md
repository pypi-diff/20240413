# Comparing `tmp/nornir_napalm-0.4.0.tar.gz` & `tmp/nornir_napalm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_napalm-0.4.0.tar", max compression
+gzip compressed data, was "nornir_napalm-0.5.0.tar", max compression
```

## Comparing `nornir_napalm-0.4.0.tar` & `nornir_napalm-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11343 2022-07-12 22:03:27.501240 nornir_napalm-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/__init__.py
--rw-r--r--   0        0        0     1639 2023-02-09 01:20:54.828948 nornir_napalm-0.4.0/nornir_napalm/plugins/connections/__init__.py
--rw-r--r--   0        0        0      470 2023-03-28 17:39:55.345838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/__init__.py
--rw-r--r--   0        0        0      596 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_cli.py
--rw-r--r--   0        0        0     1767 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_configure.py
--rw-r--r--   0        0        0      995 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_confirm_commit.py
--rw-r--r--   0        0        0     1427 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_get.py
--rw-r--r--   0        0        0     1433 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_ping.py
--rw-r--r--   0        0        0      674 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_rollback.py
--rw-r--r--   0        0        0     1040 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_validate.py
--rw-r--r--   0        0        0      801 2023-03-28 17:39:55.353838 nornir_napalm-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 nornir_napalm-0.4.0/setup.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 nornir_napalm-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-07-12 22:03:27.501240 nornir_napalm-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.5.0/nornir_napalm/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.5.0/nornir_napalm/plugins/__init__.py
+-rw-r--r--   0        0        0     1639 2023-02-09 01:20:54.828948 nornir_napalm-0.5.0/nornir_napalm/plugins/connections/__init__.py
+-rw-r--r--   0        0        0      470 2023-03-28 17:39:55.345838 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-13 03:50:45.143153 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_cli.py
+-rw-r--r--   0        0        0     1767 2023-03-28 17:39:55.349838 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_configure.py
+-rw-r--r--   0        0        0      995 2023-03-28 17:39:55.349838 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_confirm_commit.py
+-rw-r--r--   0        0        0     1427 2022-07-12 22:03:27.565240 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_get.py
+-rw-r--r--   0        0        0     1433 2022-07-12 22:03:27.565240 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_ping.py
+-rw-r--r--   0        0        0      674 2023-03-28 17:39:55.349838 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_rollback.py
+-rw-r--r--   0        0        0     1040 2022-07-12 22:03:27.565240 nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_validate.py
+-rw-r--r--   0        0        0      804 2024-04-13 03:50:45.147153 nornir_napalm-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nornir_napalm-0.5.0/PKG-INFO
```

### Comparing `nornir_napalm-0.4.0/LICENSE` & `nornir_napalm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/connections/__init__.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_cli.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import List
+from typing import Any, List
 
 from nornir.core.task import Result, Task
 
 from nornir_napalm.plugins.connections import CONNECTION_NAME
 
 
-def napalm_cli(task: Task, commands: List[str]) -> Result:
+def napalm_cli(task: Task, commands: List[str], **kwargs: Any) -> Result:
     """
     Run commands on remote devices using napalm
 
     Arguments:
       commands: commands to execute
-
+      **kwargs: placeholder for user added arguments
     Returns:
       Result object with the following attributes set:
         * result (``dict``): result of the commands execution
     """
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    result = device.cli(commands)
+    result = device.cli(commands, **kwargs)
     return Result(host=task.host, result=result)
```

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_configure.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_configure.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_confirm_commit.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_confirm_commit.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_get.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_get.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_ping.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_ping.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_rollback.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_rollback.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_validate.py` & `nornir_napalm-0.5.0/nornir_napalm/plugins/tasks/napalm_validate.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.4.0/pyproject.toml` & `nornir_napalm-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "nornir_napalm"
-version = "0.4.0"
+version = "0.5.0"
 description = "NAPALM's plugins for nornir"
 authors = ["David Barroso <dbarrosop@dravetech.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.plugins."nornir.plugins.connections"]
 "napalm" = "nornir_napalm.plugins.connections:Napalm"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-napalm = "^4"
+python = ">=3.8,<4.0"
+napalm = "^5"
 nornir = { version = "~3", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
-black = "^22.6.0"
-mypy = "1.0.0"
+black = "24.3.0"
+mypy = "1.9.0"
 pylama = "8.4.1"
-pytest = "7.2.1"
-nbval = "*"
+pytest = "^8.1.1"
+nbval = "^0.11.0"
 jupyter = "^1"
-sphinx = "^4"
+sphinx = "^7"
 sphinxcontrib-napoleon = "^0.7"
-nbsphinx = "^0.8"
-sphinx-issues = "^3.0"
-sphinx_rtd_theme = "^1.0"
+nbsphinx = "^0.9"
+sphinx-issues = "^4"
+sphinx_rtd_theme = "^2"
 nornir_utils = { version = "*", allow-prereleases = true }
-pytest-cov = "4.0.0"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `nornir_napalm-0.4.0/PKG-INFO` & `nornir_napalm-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: nornir-napalm
-Version: 0.4.0
+Name: nornir_napalm
+Version: 0.5.0
 Summary: NAPALM's plugins for nornir
 License: Apache-2.0
 Author: David Barroso
 Author-email: dbarrosop@dravetech.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: napalm (>=4,<5)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: napalm (>=5,<6)
 Requires-Dist: nornir (>=3,<4)
```

