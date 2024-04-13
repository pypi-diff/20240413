# Comparing `tmp/invokelint-0.9.1.tar.gz` & `tmp/invokelint-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokelint-0.9.1.tar", last modified: Thu Mar 28 15:33:24 2024, max compression
+gzip compressed data, was "invokelint-0.9.2.tar", last modified: Fri Mar 29 12:20:33 2024, max compression
```

## Comparing `invokelint-0.9.1.tar` & `invokelint-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.490357 invokelint-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-28 15:32:15.000000 invokelint-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 15:32:15.000000 invokelint-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-03-28 15:33:24.490357 invokelint-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-03-28 15:32:15.000000 invokelint-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.486357 invokelint-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-28 15:32:15.000000 invokelint-0.9.1/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.490357 invokelint-0.9.1/invokelint/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.490357 invokelint-0.9.1/invokelint/path/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/path/filter_duplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/path/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/ruff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-28 15:32:15.000000 invokelint-0.9.1/invokelint/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.490357 invokelint-0.9.1/invokelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-03-28 15:33:24.000000 invokelint-0.9.1/invokelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-28 15:33:24.000000 invokelint-0.9.1/invokelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:33:24.000000 invokelint-0.9.1/invokelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:33:23.000000 invokelint-0.9.1/invokelint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-28 15:33:24.000000 invokelint-0.9.1/invokelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 15:33:24.000000 invokelint-0.9.1/invokelint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-03-28 15:32:15.000000 invokelint-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-28 15:33:24.494356 invokelint-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 15:32:15.000000 invokelint-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:33:24.490357 invokelint-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test__clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-28 15:32:15.000000 invokelint-0.9.1/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.414440 invokelint-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-29 12:19:39.000000 invokelint-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-29 12:19:39.000000 invokelint-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-03-29 12:20:33.414440 invokelint-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-03-29 12:19:39.000000 invokelint-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.410440 invokelint-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-29 12:19:39.000000 invokelint-0.9.2/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.410440 invokelint-0.9.2/invokelint/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.414440 invokelint-0.9.2/invokelint/path/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/path/filter_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/path/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/ruff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-29 12:19:39.000000 invokelint-0.9.2/invokelint/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.414440 invokelint-0.9.2/invokelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-03-29 12:20:33.000000 invokelint-0.9.2/invokelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-29 12:20:33.000000 invokelint-0.9.2/invokelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:20:33.000000 invokelint-0.9.2/invokelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:20:32.000000 invokelint-0.9.2/invokelint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-29 12:20:33.000000 invokelint-0.9.2/invokelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 12:20:33.000000 invokelint-0.9.2/invokelint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-03-29 12:19:39.000000 invokelint-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-29 12:20:33.414440 invokelint-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-29 12:19:39.000000 invokelint-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:20:33.414440 invokelint-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test__clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-29 12:19:39.000000 invokelint-0.9.2/tests/test_test.py
```

### Comparing `invokelint-0.9.1/LICENSE` & `invokelint-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/PKG-INFO` & `invokelint-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.9.1/README.md` & `invokelint-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/docs/CONTRIBUTING.md` & `invokelint-0.9.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/_clean.py` & `invokelint-0.9.2/invokelint/_clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/dist.py` & `invokelint-0.9.2/invokelint/dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/lint.py` & `invokelint-0.9.2/invokelint/lint.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/path/__init__.py` & `invokelint-0.9.2/invokelint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/path/filter_duplication.py` & `invokelint-0.9.2/invokelint/path/filter_duplication.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/path/setuptools.py` & `invokelint-0.9.2/invokelint/path/setuptools.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/ruff.py` & `invokelint-0.9.2/invokelint/ruff.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     if show_fixes:
         list_options.append("--show-fixes")
     options = " " + " ".join(list_options) if list_options else ""
     run_in_pty(context, "ruff check{} {}".format(options, " ".join(PYTHON_DIRS_EXCLUDING_TEST)))
     return run_in_pty(context, "ruff check{} --ignore S101 {}".format(options, " ".join(EXISTING_TEST_PACKAGES)))
 
 
-def fmt(context: "Context", *, check: bool = False, diff: bool = False) -> "Result":
+def fmt(context: "Context", *, diff: bool = False) -> "Result":
     """Lints code with Ruff."""
     list_options = []
-    if check:
-        list_options.append("--check")
     if diff:
         list_options.append("--diff")
     options = " " + " ".join(list_options) if list_options else ""
     return run_in_pty(context, "ruff format{} {}".format(options, " ".join(PYTHON_DIRS)))
```

### Comparing `invokelint-0.9.1/invokelint/run.py` & `invokelint-0.9.2/invokelint/run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint/style.py` & `invokelint-0.9.2/invokelint/style.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,19 @@
     with suppress(UnexpectedExit):
         ruff_commands.chk(context, show_fixes=True)
     return ruff_commands.chk(context, fix=True, show_fixes=True)
 
 
 # Reason: Compatibility with semgrep task to be called from lint.fast().. pylint: disable=unused-argument
 def call_ruff_fmt(context: Context, *, check: bool = False, **kwargs: Any) -> Result:  # noqa: ARG001
-    return ruff_commands.fmt(context, check=check, diff=True)
+    if check:
+        return ruff_commands.fmt(context, diff=check)
+    with suppress(UnexpectedExit):
+        ruff_commands.fmt(context, diff=True)
+    return ruff_commands.fmt(context)
 
 
 @task(
     help={
         "check": "Checks if source is formatted without applying changes",
         "ruff": "Leave ruff warnings",
         "by_ruff": "Formats code by ruff",
```

### Comparing `invokelint-0.9.1/invokelint/test.py` & `invokelint-0.9.2/invokelint/test.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/invokelint.egg-info/PKG-INFO` & `invokelint-0.9.2/invokelint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.9.1/invokelint.egg-info/SOURCES.txt` & `invokelint-0.9.2/invokelint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/pyproject.toml` & `invokelint-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invokelint"
-version = "0.9.1"
+version = "0.9.2"
 description = "Invokes Python dev tools at once."
 readme = "README.md"
 # Dependency: setuptools>=61.0.0 requires Python 3.7
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
     "autoflake",
@@ -174,14 +174,17 @@
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
 ]
 
 [tool.ruff]
 line-length = 119
+target-version = "py37"
+
+[tool.ruff.lint]
 select = [
     "F",  # Pyflakes
     "E",  # pycodestyle
     "W",  # pycodestyle
     "C90",  # mccabe
     # "I",  # isort
     "N",  # pep8-naming
@@ -235,11 +238,10 @@
     "COM812",  # Trailing comma missing
     "PT001",  # Use `@pytest.fixture()` over `@pytest.fixture`
     "PT006",  # Wrong name(s) type in `@pytest.mark.parametrize`, expected `tuple`
     "SIM108",  # Use ternary operator `extra_context = {} if extra_context is None else request.param` instead of `if`-`else`-block
     "UP015",  # Unnecessary open mode parameters
     "UP037",  # Remove quotes from type annotation
 ]
-target-version = "py37"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101"]
```

### Comparing `invokelint-0.9.1/tests/test__clean.py` & `invokelint-0.9.2/tests/test__clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/tests/test_dist.py` & `invokelint-0.9.2/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/tests/test_lint.py` & `invokelint-0.9.2/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/tests/test_run.py` & `invokelint-0.9.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.9.1/tests/test_style.py` & `invokelint-0.9.2/tests/test_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF = [
     *LIST_COMMAND_EXPECTED_STYLE_COMMON,
     f"isort {PYTHON_DIR}",
     f"black {PYTHON_DIR}",
 ]
 LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF_BY_RUFF = [
     *LIST_COMMAND_EXPECTED_STYLE_COMMON,
-    f"ruff format --diff {PYTHON_DIR}",
+    f"ruff format {PYTHON_DIR}",
 ]
 LIST_COMMAND_EXPECTED_STYLE = [
     *LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF,
     "ruff check --fix --show-fixes --ignore S101 tests",
 ]
 LIST_COMMAND_EXPECTED_STYLE_BY_RUFF = [
     *LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF_BY_RUFF,
@@ -39,15 +39,15 @@
     *LIST_COMMAND_EXPECTED_STYLE_CHECK_COMMON,
     f"isort --check-only --diff {PYTHON_DIR}",
     f"black --check --diff {PYTHON_DIR}",
     "ruff check --show-fixes --ignore S101 tests",
 ]
 LIST_COMMAND_EXPECTED_STYLE_CHECK_BY_RUFF = [
     *LIST_COMMAND_EXPECTED_STYLE_CHECK_COMMON,
-    f"ruff format --check --diff {PYTHON_DIR}",
+    f"ruff format --diff {PYTHON_DIR}",
     "ruff check --show-fixes --ignore S101 tests",
 ]
 
 
 def test_style(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     check_list_result(fmt(context), LIST_COMMAND_EXPECTED_STYLE)
```

### Comparing `invokelint-0.9.1/tests/test_test.py` & `invokelint-0.9.2/tests/test_test.py`

 * *Files identical despite different names*

