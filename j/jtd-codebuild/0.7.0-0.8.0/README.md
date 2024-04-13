# Comparing `tmp/jtd_codebuild-0.7.0.tar.gz` & `tmp/jtd_codebuild-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtd_codebuild-0.7.0.tar", max compression
+gzip compressed data, was "jtd_codebuild-0.8.0.tar", max compression
```

## Comparing `jtd_codebuild-0.7.0.tar` & `jtd_codebuild-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1056 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/LICENSE
--rw-r--r--   0        0        0     9327 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/__init__.py
--rw-r--r--   0        0        0      364 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/__main__.py
--rw-r--r--   0        0        0     1520 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/bundle.py
--rw-r--r--   0        0        0     2067 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/codebuild.py
--rw-r--r--   0        0        0      577 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/config.py
--rw-r--r--   0        0        0      188 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/generators/__init__.py
--rw-r--r--   0        0        0     2142 2024-01-12 18:42:59.420363 jtd_codebuild-0.7.0/jtd_codebuild/generators/generator.py
--rw-r--r--   0        0        0    12254 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/generators/python_generator.py
--rw-r--r--   0        0        0     1620 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/generators/typescript_generator.py
--rw-r--r--   0        0        0     2044 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/inheritance.py
--rw-r--r--   0        0        0     2303 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/loaders.py
--rw-r--r--   0        0        0        0 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/.gitignore
--rw-r--r--   0        0        0      600 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/jtd-codebuild.json
--rw-r--r--   0        0        0      134 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/book.jtd.yaml
--rw-r--r--   0        0        0      191 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/user.jtd.yaml
--rw-r--r--   0        0        0       41 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/src/schema.jtd.yaml
--rw-r--r--   0        0        0       38 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/.gitignore
--rw-r--r--   0        0        0      626 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/jtd-codebuild.json
--rw-r--r--   0        0        0      433 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/book.jtd.yaml
--rw-r--r--   0        0        0      191 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/user.jtd.yaml
--rw-r--r--   0        0        0      239 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/src/dtos/io.jtd.yaml
--rw-r--r--   0        0        0       41 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/src/schema.jtd.yaml
--rw-r--r--   0        0        0        3 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_3/.gitignore
--rw-r--r--   0        0        0      142 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_3/jtd-codebuild.json
--rw-r--r--   0        0        0       41 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_3/src/schema.jtd.yaml
--rw-r--r--   0        0        0        3 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_4/.gitignore
--rw-r--r--   0        0        0      648 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_4/jtd-codebuild.json
--rw-r--r--   0        0        0      471 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_4/src/definitions/io.jtd.yaml
--rw-r--r--   0        0        0       41 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_4/src/schema.jtd.yaml
--rw-r--r--   0        0        0     1619 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_1.py
--rw-r--r--   0        0        0      837 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_2.py
--rw-r--r--   0        0        0      519 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_3.py
--rw-r--r--   0        0        0      837 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_4.py
--rw-r--r--   0        0        0     3211 2024-01-12 18:42:59.424363 jtd_codebuild-0.7.0/jtd_codebuild/utils.py
--rw-r--r--   0        0        0     2599 2024-01-12 18:43:19.188157 jtd_codebuild-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10105 1970-01-01 00:00:00.000000 jtd_codebuild-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10115 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/__main__.py
+-rw-r--r--   0        0        0     1520 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/bundle.py
+-rw-r--r--   0        0        0     2067 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/codebuild.py
+-rw-r--r--   0        0        0      577 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/config.py
+-rw-r--r--   0        0        0      188 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/__init__.py
+-rw-r--r--   0        0        0     2142 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/generator.py
+-rw-r--r--   0        0        0    12254 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/python_generator.py
+-rw-r--r--   0        0        0     1620 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/typescript_generator.py
+-rw-r--r--   0        0        0     2044 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/inheritance.py
+-rw-r--r--   0        0        0     2303 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/.gitignore
+-rw-r--r--   0        0        0      600 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/jtd-codebuild.json
+-rw-r--r--   0        0        0      134 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/book.jtd.yaml
+-rw-r--r--   0        0        0      191 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/user.jtd.yaml
+-rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/schema.jtd.yaml
+-rw-r--r--   0        0        0       38 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/.gitignore
+-rw-r--r--   0        0        0      626 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/jtd-codebuild.json
+-rw-r--r--   0        0        0      433 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/book.jtd.yaml
+-rw-r--r--   0        0        0      191 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/user.jtd.yaml
+-rw-r--r--   0        0        0      239 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/dtos/io.jtd.yaml
+-rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/schema.jtd.yaml
+-rw-r--r--   0        0        0        3 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/.gitignore
+-rw-r--r--   0        0        0      142 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/jtd-codebuild.json
+-rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/src/schema.jtd.yaml
+-rw-r--r--   0        0        0        3 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/.gitignore
+-rw-r--r--   0        0        0      648 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/jtd-codebuild.json
+-rw-r--r--   0        0        0      471 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/src/definitions/io.jtd.yaml
+-rw-r--r--   0        0        0       41 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/src/schema.jtd.yaml
+-rw-r--r--   0        0        0     1619 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_1.py
+-rw-r--r--   0        0        0      837 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_2.py
+-rw-r--r--   0        0        0      519 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_3.py
+-rw-r--r--   0        0        0      837 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_4.py
+-rw-r--r--   0        0        0     3211 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/utils.py
+-rw-r--r--   0        0        0     1870 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11479 1970-01-01 00:00:00.000000 jtd_codebuild-0.8.0/PKG-INFO
```

### Comparing `jtd_codebuild-0.7.0/LICENSE` & `jtd_codebuild-0.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 01Joseph-Hwang10
+Copyright 2023 01Joseph-Hwang10
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `jtd_codebuild-0.7.0/README.md` & `jtd_codebuild-0.8.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # JSON Type Definition Code Build
 
+[![PyPI version](https://badge.fury.io/py/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild)
+[![Testsuite](https://github.com/01Joseph-Hwang10/jtd-codebuild/workflows/Test%20and%20Lint/badge.svg)](https://github.com/01Joseph-Hwang10/jtd-codebuild/actions?query=workflow%3A"Test+and+Lint")
+[![Python version](https://img.shields.io/pypi/pyversions/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild)
+[![Project Status](https://img.shields.io/pypi/status/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild/)
+[![Supported Interpreters](https://img.shields.io/pypi/implementation/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild/)
+[![License](https://img.shields.io/pypi/l/jtd-codebuild.svg)](https://github.com/pawelzny/jtd-codebuild/blob/master/LICENSE)
+
 jtd-codebuild is a tool for generating language specific schemas and interfaces code from JSON Type Definition IDL files in either yaml or json format.
 
 This tool is built on top of [`jtd-codegen`](https://jsontypedef.com/) so check out the documentation if you don't have a clue about JSON Type Definition.
 
 ## Prerequisites
 
 - [jtd-codegen](https://jsontypedef.com/docs/jtd-codegen/)
```

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/bundle.py` & `jtd_codebuild-0.8.0/jtd_codebuild/bundle.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/codebuild.py` & `jtd_codebuild-0.8.0/jtd_codebuild/codebuild.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/config.py` & `jtd_codebuild-0.8.0/jtd_codebuild/config.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/generators/generator.py` & `jtd_codebuild-0.8.0/jtd_codebuild/generators/generator.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/generators/python_generator.py` & `jtd_codebuild-0.8.0/jtd_codebuild/generators/python_generator.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/generators/typescript_generator.py` & `jtd_codebuild-0.8.0/jtd_codebuild/generators/typescript_generator.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/inheritance.py` & `jtd_codebuild-0.8.0/jtd_codebuild/inheritance.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/loaders.py` & `jtd_codebuild-0.8.0/jtd_codebuild/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # Recursively load all definitions
     for root, dirs, files in itertools.chain(*map(os.walk, definition_paths)):
         for file in files:
             if file_is_yaml(file) or file_is_json(file):
                 filepath = join(root, file)
                 with open(filepath, "r") as f:
                     definition_parts = (
-                        yaml.load(f, Loader=yaml.FullLoader)
+                        yaml.load(f, Loader=yaml.SafeLoader)
                         if file_is_yaml(file)
                         else json.load(f)
                     )
                     for definition_name, definition in definition_parts.items():
                         if definition_name in definitions:
                             raise ValueError(
                                 f"Definition name {definition_name} already exists."
@@ -62,11 +62,11 @@
         The root schema.
     """
     config = get_config(cwd)
     schema_path = os.path.join(cwd, config["root-schema-path"])
 
     with open(schema_path, "r") as f:
         return (
-            yaml.load(f, Loader=yaml.FullLoader)
+            yaml.load(f, Loader=yaml.SafeLoader)
             if file_is_yaml(schema_path)
             else json.load(f)
         )
```

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_1/jtd-codebuild.json` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/jtd-codebuild.json`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_2/jtd-codebuild.json` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/jtd-codebuild.json`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/fixtures/example_project_4/jtd-codebuild.json` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/jtd-codebuild.json`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_1.py` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_1.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_2.py` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_2.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_3.py` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_3.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/tests/test_example_project_4.py` & `jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_4.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/jtd_codebuild/utils.py` & `jtd_codebuild-0.8.0/jtd_codebuild/utils.py`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.7.0/PKG-INFO` & `jtd_codebuild-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 Metadata-Version: 2.1
 Name: jtd-codebuild
-Version: 0.7.0
+Version: 0.8.0
 Summary: Tool for generating language specific schemas and interfaces code from JSON Type Definition IDL files in yaml format. Powered by jtd-codegen.
 License: MIT
 Author: 01Joseph-Hwang10
 Author-email: joseph95501@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
 Requires-Dist: case-converter (>=1.1.0,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # JSON Type Definition Code Build
 
+[![PyPI version](https://badge.fury.io/py/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild)
+[![Testsuite](https://github.com/01Joseph-Hwang10/jtd-codebuild/workflows/Test%20and%20Lint/badge.svg)](https://github.com/01Joseph-Hwang10/jtd-codebuild/actions?query=workflow%3A"Test+and+Lint")
+[![Python version](https://img.shields.io/pypi/pyversions/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild)
+[![Project Status](https://img.shields.io/pypi/status/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild/)
+[![Supported Interpreters](https://img.shields.io/pypi/implementation/jtd-codebuild.svg)](https://pypi.org/project/jtd-codebuild/)
+[![License](https://img.shields.io/pypi/l/jtd-codebuild.svg)](https://github.com/pawelzny/jtd-codebuild/blob/master/LICENSE)
+
 jtd-codebuild is a tool for generating language specific schemas and interfaces code from JSON Type Definition IDL files in either yaml or json format.
 
 This tool is built on top of [`jtd-codegen`](https://jsontypedef.com/) so check out the documentation if you don't have a clue about JSON Type Definition.
 
 ## Prerequisites
 
 - [jtd-codegen](https://jsontypedef.com/docs/jtd-codegen/)
```

