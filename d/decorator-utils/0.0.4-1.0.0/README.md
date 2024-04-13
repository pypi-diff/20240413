# Comparing `tmp/decorator_utils-0.0.4.tar.gz` & `tmp/decorator_utils-1.0.0.tar.gz`

## Comparing `decorator_utils-0.0.4.tar` & `decorator_utils-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/decorator_utils/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/README.md
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 decorator_utils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/__init__.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/metadata.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/wrapper.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/README.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/PKG-INFO
```

### Comparing `decorator_utils-0.0.4/.github/workflows/publish-pypi.yaml` & `decorator_utils-1.0.0/.github/workflows/publish-pypi.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     environment: release
     permissions:
       id-token: write
 
     steps:
       - uses: actions/checkout@v4
 
-      - name: Interpreter setup
+      - name: Setup
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
 
       - name: Build
         run: |
           python3 -m pip install build --user
```

### Comparing `decorator_utils-0.0.4/LICENSE` & `decorator_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator_utils-0.0.4/pyproject.toml` & `decorator_utils-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `decorator_utils-0.0.4/PKG-INFO` & `decorator_utils-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: decorator-utils
-Version: 0.0.4
+Version: 1.0.0
 Summary: Simple and useful decorator utilities.
 Project-URL: Repository, https://github.com/stickm4n/decorator-utils
 Project-URL: Documentation, https://github.com/stickm4n/decorator-utils/wiki
 Project-URL: Issues, https://github.com/stickm4n/decorator-utils/issues
 Author-email: "Julio C. Galindo" <jcgalindo.jcgh@gmail.com>
 License: MIT License
         
@@ -36,7 +36,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+decorator-utils
+===============
+
+
+Installation
+------------
+
+```shell
+python3 -m pip install decorator-utils
+```
+
+Usage
+-----
+
+```python
+from random import randint
+
+from decorator_utils import function_wrapper
+
+
+@function_wrapper(pre_cb=lambda i: print(f'Calling with param {i}'),
+                  post_cb=lambda r, i: print(f'Function call result `{r}` with param `{i}`'))
+def random_int(increment):
+    number = randint(0, 10)
+    print(f'-> Generated number {number}')
+
+    return number + increment
+
+
+if __name__ == '__main__':
+    n = randint(0, 10)
+
+    random_int(n)
+```
```

