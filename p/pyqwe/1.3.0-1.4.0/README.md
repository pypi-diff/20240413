# Comparing `tmp/pyqwe-1.3.0.tar.gz` & `tmp/pyqwe-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqwe-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyqwe-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyqwe-1.3.0.tar` & `pyqwe-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.3.0/.env.example
--rw-r--r--   0        0        0     1160 2024-03-30 13:38:11.669728 pyqwe-1.3.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.3.0/LICENSE
--rw-r--r--   0        0        0     3010 2024-04-03 09:00:07.846648 pyqwe-1.3.0/README.md
--rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.3.0/flask_example/module.py
--rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.3.0/flask_example/package/__init__.py
--rw-r--r--   0        0        0      936 2024-03-30 13:38:11.669969 pyqwe-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1773 2024-04-03 09:11:21.840056 pyqwe-1.3.0/pyqwe/__init__.py
--rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.3.0/pyqwe/exceptions.py
--rw-r--r--   0        0        0     3876 2024-04-02 10:10:43.435476 pyqwe-1.3.0/pyqwe/helpers.py
--rw-r--r--   0        0        0      750 2024-04-03 09:11:15.406720 pyqwe-1.3.0/pyqwe/parser.py
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 pyqwe-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.4.0/.env.example
+-rw-r--r--   0        0        0     1180 2024-04-13 12:33:51.476960 pyqwe-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3010 2024-04-03 09:00:07.846648 pyqwe-1.4.0/README.md
+-rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.4.0/flask_example/module.py
+-rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.4.0/flask_example/package/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-13 12:34:23.232337 pyqwe-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1823 2024-04-13 12:46:27.873884 pyqwe-1.4.0/pyqwe/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.4.0/pyqwe/exceptions.py
+-rw-r--r--   0        0        0     3901 2024-04-13 12:45:28.704133 pyqwe-1.4.0/pyqwe/helpers.py
+-rw-r--r--   0        0        0      750 2024-04-03 09:11:15.406720 pyqwe-1.4.0/pyqwe/parser.py
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 pyqwe-1.4.0/PKG-INFO
```

### Comparing `pyqwe-1.3.0/.gitignore` & `pyqwe-1.4.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -62,8 +62,10 @@
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
 #Pipfile.lock
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 /venv/
+/venv_3_8
+/venv_3_9
 /.env
```

### Comparing `pyqwe-1.3.0/LICENSE` & `pyqwe-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqwe-1.3.0/README.md` & `pyqwe-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqwe-1.3.0/pyproject.toml` & `pyqwe-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pyqwe"
 description = 'Run commands set in the pyproject.toml file'
 authors = [{ name = "David Carmichael", email = "david@uilix.com" }]
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version"]
 
 [project.scripts]
 pyqwe = "pyqwe:main"
```

### Comparing `pyqwe-1.3.0/pyqwe/__init__.py` & `pyqwe-1.4.0/pyqwe/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sys
-import tomllib
 from pathlib import Path
 
 from .helpers import _run, _split_runner, Colr
 from .parser import ArgumentParser
 
-__version__ = "1.3.0"
+try:
+    import tomllib
+except ImportError:
+    try:
+        import toml as tomllib
+    except ImportError:
+        raise ImportError("pyqwe requires toml, install it with 'pip install toml'")
 
-# sr = start of runner
-# er = end of runner
-# runner = sr:er
-# flask = app:run
-# will invoke the run function in the app module
+__version__ = "1.4.0"
 
 _cwd = Path().cwd()
 _pyproject_file = _cwd / "pyproject.toml"
 
 if not _pyproject_file.exists():
     raise FileNotFoundError("pyproject.toml not found")
```

### Comparing `pyqwe-1.3.0/pyqwe/helpers.py` & `pyqwe-1.4.0/pyqwe/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import typing as t
 import importlib
 import importlib.util
 import os
 import shlex
 import subprocess
 import sys
 from pathlib import Path
@@ -35,22 +36,22 @@
     return _replace_env_vars
 
 
 def _no_traceback_eh(exc_type, exc_val, traceback):
     pass
 
 
-def _split_runner(runner_: str) -> tuple:
+def _split_runner(runner_: str) -> t.Tuple:
     r = runner_.split(":")
     sr = r[0]  # start or runner
     er = r[1]  # end of runner
     return sr, er
 
 
-def _identify_sr(sr_: str, _cwd: Path) -> tuple[Path, str]:
+def _identify_sr(sr_: str, _cwd: Path) -> t.Tuple[Path, str]:
     if sr_.endswith(".py"):
         sr_.replace(".py", "")
 
     if "." in sr_:
         if sys.platform == "win32":
             sr = _cwd / sr_.replace(".", "\\")
 
@@ -73,15 +74,15 @@
 
 def _path_to_module(path: Path) -> str:
     file_ = path.stem
     path_ = path.parent
     return f"{path_.name}.{file_}"
 
 
-def _extract_env_vars(r: str) -> list[str]:
+def _extract_env_vars(r: str) -> t.List[str]:
     if "{{" and "}}" in r:
         return [i.split("}}")[0].replace(" ", "") for i in r.split("{{") if "}}" in i]
     return []
 
 
 def _import_python_dotenv() -> bool:
     try:
```

### Comparing `pyqwe-1.3.0/pyqwe/parser.py` & `pyqwe-1.4.0/pyqwe/parser.py`

 * *Files identical despite different names*

### Comparing `pyqwe-1.3.0/PKG-INFO` & `pyqwe-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyqwe
-Version: 1.3.0
+Version: 1.4.0
 Summary: Run commands set in the pyproject.toml file
 Author-email: David Carmichael <david@uilix.com>
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pyqwe-extra-dotenv ; extra == "dotenv"
 Project-URL: Source, https://github.com/CheeseCake87/pyqwe
 Provides-Extra: dotenv
 
 # 🏎️💨 pyqwe
```

