# Comparing `tmp/pytest_toolkit-0.1.0.tar.gz` & `tmp/pytest_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_toolkit-0.1.0.tar", last modified: Sat Apr 13 16:48:34 2024, max compression
+gzip compressed data, was "pytest_toolkit-0.1.1.tar", last modified: Sat Apr 13 16:56:20 2024, max compression
```

## Comparing `pytest_toolkit-0.1.0.tar` & `pytest_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:48:34.567985 pytest_toolkit-0.1.0/
--rw-r--r--   0 lev        (501) staff       (20)     2511 2024-04-13 16:48:34.567722 pytest_toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 lev        (501) staff       (20)     2179 2024-04-13 16:45:30.000000 pytest_toolkit-0.1.0/README.md
-drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:48:34.564615 pytest_toolkit-0.1.0/pytest_toolkit/
--rw-r--r--   0 lev        (501) staff       (20)       65 2024-04-13 14:16:02.000000 pytest_toolkit-0.1.0/pytest_toolkit/__init__.py
--rw-r--r--   0 lev        (501) staff       (20)      446 2024-04-13 16:12:06.000000 pytest_toolkit-0.1.0/pytest_toolkit/configure.py
--rw-r--r--   0 lev        (501) staff       (20)      348 2024-04-13 14:45:21.000000 pytest_toolkit-0.1.0/pytest_toolkit/constants.py
--rw-r--r--   0 lev        (501) staff       (20)       43 2024-04-13 14:19:35.000000 pytest_toolkit-0.1.0/pytest_toolkit/errors.py
--rw-r--r--   0 lev        (501) staff       (20)     4568 2024-04-13 16:13:23.000000 pytest_toolkit-0.1.0/pytest_toolkit/json.py
-drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:48:34.567348 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/
--rw-r--r--   0 lev        (501) staff       (20)     2511 2024-04-13 16:48:34.000000 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 lev        (501) staff       (20)      498 2024-04-13 16:48:34.000000 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 lev        (501) staff       (20)        1 2024-04-13 16:48:34.000000 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 lev        (501) staff       (20)       22 2024-04-13 16:48:34.000000 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/requires.txt
--rw-r--r--   0 lev        (501) staff       (20)       21 2024-04-13 16:48:34.000000 pytest_toolkit-0.1.0/pytest_toolkit.egg-info/top_level.txt
--rw-r--r--   0 lev        (501) staff       (20)       38 2024-04-13 16:48:34.568026 pytest_toolkit-0.1.0/setup.cfg
--rw-r--r--   0 lev        (501) staff       (20)      757 2024-04-13 11:50:10.000000 pytest_toolkit-0.1.0/setup.py
-drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:48:34.566857 pytest_toolkit-0.1.0/tests/
--rw-r--r--   0 lev        (501) staff       (20)        0 2024-04-13 13:37:15.000000 pytest_toolkit-0.1.0/tests/__init__.py
--rw-r--r--   0 lev        (501) staff       (20)        0 2024-04-13 13:37:15.000000 pytest_toolkit-0.1.0/tests/conftest.py
--rw-r--r--   0 lev        (501) staff       (20)     1413 2024-04-13 15:02:36.000000 pytest_toolkit-0.1.0/tests/test_difference.py
--rw-r--r--   0 lev        (501) staff       (20)      279 2024-04-13 14:26:47.000000 pytest_toolkit-0.1.0/tests/test_doesnt_matter.py
--rw-r--r--   0 lev        (501) staff       (20)      729 2024-04-13 16:44:42.000000 pytest_toolkit-0.1.0/tests/test_json.py
--rw-r--r--   0 lev        (501) staff       (20)      468 2024-04-13 14:20:51.000000 pytest_toolkit-0.1.0/tests/test_json_default.py
--rw-r--r--   0 lev        (501) staff       (20)     1426 2024-04-13 15:22:40.000000 pytest_toolkit-0.1.0/tests/test_json_error.py
+drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:56:20.450744 pytest_toolkit-0.1.1/
+-rw-r--r--   0 lev        (501) staff       (20)     2561 2024-04-13 16:56:20.450504 pytest_toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 lev        (501) staff       (20)     2229 2024-04-13 16:55:22.000000 pytest_toolkit-0.1.1/README.md
+drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:56:20.447188 pytest_toolkit-0.1.1/pytest_toolkit/
+-rw-r--r--   0 lev        (501) staff       (20)       65 2024-04-13 14:16:02.000000 pytest_toolkit-0.1.1/pytest_toolkit/__init__.py
+-rw-r--r--   0 lev        (501) staff       (20)      446 2024-04-13 16:12:06.000000 pytest_toolkit-0.1.1/pytest_toolkit/configure.py
+-rw-r--r--   0 lev        (501) staff       (20)      348 2024-04-13 14:45:21.000000 pytest_toolkit-0.1.1/pytest_toolkit/constants.py
+-rw-r--r--   0 lev        (501) staff       (20)       43 2024-04-13 14:19:35.000000 pytest_toolkit-0.1.1/pytest_toolkit/errors.py
+-rw-r--r--   0 lev        (501) staff       (20)     4568 2024-04-13 16:13:23.000000 pytest_toolkit-0.1.1/pytest_toolkit/json.py
+drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:56:20.450151 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/
+-rw-r--r--   0 lev        (501) staff       (20)     2561 2024-04-13 16:56:20.000000 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 lev        (501) staff       (20)      498 2024-04-13 16:56:20.000000 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 lev        (501) staff       (20)        1 2024-04-13 16:56:20.000000 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 lev        (501) staff       (20)       22 2024-04-13 16:56:20.000000 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/requires.txt
+-rw-r--r--   0 lev        (501) staff       (20)       21 2024-04-13 16:56:20.000000 pytest_toolkit-0.1.1/pytest_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 lev        (501) staff       (20)       38 2024-04-13 16:56:20.450788 pytest_toolkit-0.1.1/setup.cfg
+-rw-r--r--   0 lev        (501) staff       (20)      757 2024-04-13 16:56:12.000000 pytest_toolkit-0.1.1/setup.py
+drwxr-xr-x   0 lev        (501) staff       (20)        0 2024-04-13 16:56:20.449658 pytest_toolkit-0.1.1/tests/
+-rw-r--r--   0 lev        (501) staff       (20)        0 2024-04-13 13:37:15.000000 pytest_toolkit-0.1.1/tests/__init__.py
+-rw-r--r--   0 lev        (501) staff       (20)        0 2024-04-13 13:37:15.000000 pytest_toolkit-0.1.1/tests/conftest.py
+-rw-r--r--   0 lev        (501) staff       (20)     1413 2024-04-13 15:02:36.000000 pytest_toolkit-0.1.1/tests/test_difference.py
+-rw-r--r--   0 lev        (501) staff       (20)      279 2024-04-13 14:26:47.000000 pytest_toolkit-0.1.1/tests/test_doesnt_matter.py
+-rw-r--r--   0 lev        (501) staff       (20)      729 2024-04-13 16:44:42.000000 pytest_toolkit-0.1.1/tests/test_json.py
+-rw-r--r--   0 lev        (501) staff       (20)      468 2024-04-13 14:20:51.000000 pytest_toolkit-0.1.1/tests/test_json_default.py
+-rw-r--r--   0 lev        (501) staff       (20)     1426 2024-04-13 15:22:40.000000 pytest_toolkit-0.1.1/tests/test_json_error.py
```

### Comparing `pytest_toolkit-0.1.0/PKG-INFO` & `pytest_toolkit-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful utils for testing
 Home-page: https://github.com/lev4ek0/pytest_toolkit
 Author: Lev Belous
 Author-email: leva22.08.01@inbox.ru
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: deepdiff
@@ -22,35 +22,44 @@
     pip install pytest-toolkit
     ```
     ```
     pytest tests/
     ```
 2. Get started 
     ```
-    The advantage is in having clear understanding of difference between response.json and static json. For example
-    {'Значение или тип элемента изменены': {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}} == {}
+    The advantage is in having clear understanding of difference between 
+    response.json and static json. For example
+    {
+        'Значение или тип элемента изменены': 
+        {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}
+    } == {}
     Its easy to see that value of key 'example1' changed from 'example1' to 'example2'.
     ```
     ```
     from pytest_toolkit import get_diff
 
     def test():
         response = client.get(url)
         assert get_diff(result_dict=response.json()) == {}
     ```
 3. Static files search
     ```
     1. You need to create static directory in tests/
-    2. If you create filename test_a.py with test_b function, you need to create "a" directory in static directory and "b.json" in directory "a". Library will automatically find a file for get_diff function
-    3. If you don't have directory "a" in static files, library will try to find file "b.json" in "default" directory first
+    2. If you create filename test_a.py with test_b function, you need to 
+    create "a" directory in static directory and "b.json" in directory "a". 
+    Library will automatically find a file for get_diff function
+    3. If you don't have directory "a" in static files, library will try
+    to find file "b.json" in "default" directory first
     ```
 4. DOESNT_MATTER
     ```
-    1. If you don't care about value of dictionary, but you need a key, you can write "DOESNT_MATTER" in value and library will skip checking of this field.
-    2. If you need to have a constraint for value, you can write python code, for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
+    1. If you don't care about value of dictionary, but you need a key, you
+    can write "DOESNT_MATTER" in value and library will skip checking of this field.
+    2. If you need to have a constraint for value, you can write python code,
+    for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
     ```
 5. Check directory tests for more information and examples
 6. Coverage
     ```
     ---------- coverage: platform darwin, python 3.12.1-final-0 ----------
     Name                          Stmts   Miss  Cover
     -------------------------------------------------
```

### Comparing `pytest_toolkit-0.1.0/README.md` & `pytest_toolkit-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,44 @@
     pip install pytest-toolkit
     ```
     ```
     pytest tests/
     ```
 2. Get started 
     ```
-    The advantage is in having clear understanding of difference between response.json and static json. For example
-    {'Значение или тип элемента изменены': {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}} == {}
+    The advantage is in having clear understanding of difference between 
+    response.json and static json. For example
+    {
+        'Значение или тип элемента изменены': 
+        {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}
+    } == {}
     Its easy to see that value of key 'example1' changed from 'example1' to 'example2'.
     ```
     ```
     from pytest_toolkit import get_diff
 
     def test():
         response = client.get(url)
         assert get_diff(result_dict=response.json()) == {}
     ```
 3. Static files search
     ```
     1. You need to create static directory in tests/
-    2. If you create filename test_a.py with test_b function, you need to create "a" directory in static directory and "b.json" in directory "a". Library will automatically find a file for get_diff function
-    3. If you don't have directory "a" in static files, library will try to find file "b.json" in "default" directory first
+    2. If you create filename test_a.py with test_b function, you need to 
+    create "a" directory in static directory and "b.json" in directory "a". 
+    Library will automatically find a file for get_diff function
+    3. If you don't have directory "a" in static files, library will try
+    to find file "b.json" in "default" directory first
     ```
 4. DOESNT_MATTER
     ```
-    1. If you don't care about value of dictionary, but you need a key, you can write "DOESNT_MATTER" in value and library will skip checking of this field.
-    2. If you need to have a constraint for value, you can write python code, for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
+    1. If you don't care about value of dictionary, but you need a key, you
+    can write "DOESNT_MATTER" in value and library will skip checking of this field.
+    2. If you need to have a constraint for value, you can write python code,
+    for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
     ```
 5. Check directory tests for more information and examples
 6. Coverage
     ```
     ---------- coverage: platform darwin, python 3.12.1-final-0 ----------
     Name                          Stmts   Miss  Cover
     -------------------------------------------------
```

### Comparing `pytest_toolkit-0.1.0/pytest_toolkit/json.py` & `pytest_toolkit-0.1.1/pytest_toolkit/json.py`

 * *Files identical despite different names*

### Comparing `pytest_toolkit-0.1.0/pytest_toolkit.egg-info/PKG-INFO` & `pytest_toolkit-0.1.1/pytest_toolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful utils for testing
 Home-page: https://github.com/lev4ek0/pytest_toolkit
 Author: Lev Belous
 Author-email: leva22.08.01@inbox.ru
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: deepdiff
@@ -22,35 +22,44 @@
     pip install pytest-toolkit
     ```
     ```
     pytest tests/
     ```
 2. Get started 
     ```
-    The advantage is in having clear understanding of difference between response.json and static json. For example
-    {'Значение или тип элемента изменены': {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}} == {}
+    The advantage is in having clear understanding of difference between 
+    response.json and static json. For example
+    {
+        'Значение или тип элемента изменены': 
+        {"root['example1']": {'new_value': 'example2', 'old_value': 'example1'}}
+    } == {}
     Its easy to see that value of key 'example1' changed from 'example1' to 'example2'.
     ```
     ```
     from pytest_toolkit import get_diff
 
     def test():
         response = client.get(url)
         assert get_diff(result_dict=response.json()) == {}
     ```
 3. Static files search
     ```
     1. You need to create static directory in tests/
-    2. If you create filename test_a.py with test_b function, you need to create "a" directory in static directory and "b.json" in directory "a". Library will automatically find a file for get_diff function
-    3. If you don't have directory "a" in static files, library will try to find file "b.json" in "default" directory first
+    2. If you create filename test_a.py with test_b function, you need to 
+    create "a" directory in static directory and "b.json" in directory "a". 
+    Library will automatically find a file for get_diff function
+    3. If you don't have directory "a" in static files, library will try
+    to find file "b.json" in "default" directory first
     ```
 4. DOESNT_MATTER
     ```
-    1. If you don't care about value of dictionary, but you need a key, you can write "DOESNT_MATTER" in value and library will skip checking of this field.
-    2. If you need to have a constraint for value, you can write python code, for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
+    1. If you don't care about value of dictionary, but you need a key, you
+    can write "DOESNT_MATTER" in value and library will skip checking of this field.
+    2. If you need to have a constraint for value, you can write python code,
+    for example "DOESNT_MATTER > 9" and library will check response.json() value is more than 9.
     ```
 5. Check directory tests for more information and examples
 6. Coverage
     ```
     ---------- coverage: platform darwin, python 3.12.1-final-0 ----------
     Name                          Stmts   Miss  Cover
     -------------------------------------------------
```

### Comparing `pytest_toolkit-0.1.0/setup.py` & `pytest_toolkit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pytest_toolkit",  # package name
-    version="0.1.0",  # version
+    version="0.1.1",  # version
     author="Lev Belous",
     author_email="leva22.08.01@inbox.ru",
     description="Useful utils for testing",  # short description
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lev4ek0/pytest_toolkit",  # package URL
     install_requires=[
```

### Comparing `pytest_toolkit-0.1.0/tests/test_difference.py` & `pytest_toolkit-0.1.1/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `pytest_toolkit-0.1.0/tests/test_json.py` & `pytest_toolkit-0.1.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pytest_toolkit-0.1.0/tests/test_json_error.py` & `pytest_toolkit-0.1.1/tests/test_json_error.py`

 * *Files identical despite different names*

