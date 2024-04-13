# Comparing `tmp/ykenan_file-0.2.3.tar.gz` & `tmp/ykenan_file-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.2.3.tar", last modified: Thu Aug 17 01:46:18 2023, max compression
+gzip compressed data, was "ykenan_file-0.2.4.tar", last modified: Sat Apr 13 05:31:14 2024, max compression
```

## Comparing `ykenan_file-0.2.3.tar` & `ykenan_file-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-17 01:46:18.335027 ykenan_file-0.2.3/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2023-08-17 01:46:18.335027 ykenan_file-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.2.3/README.md
--rw-rw-rw-   0        0        0      716 2023-08-17 01:44:06.000000 ykenan_file-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       65 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-17 01:46:18.335027 ykenan_file-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-17 01:46:18.150826 ykenan_file-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-17 01:46:18.321026 ykenan_file-0.2.3/src/ykenan_file/
--rw-rw-rw-   0        0        0      274 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0    10813 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/src/ykenan_file/_create_.py
--rw-rw-rw-   0        0        0     3689 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/src/ykenan_file/_read_.py
--rw-rw-rw-   0        0        0    12944 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/src/ykenan_file/_static_method_.py
--rw-rw-rw-   0        0        0     3870 2023-08-17 01:43:58.000000 ykenan_file-0.2.3/src/ykenan_file/_thread_file_.py
--rw-rw-rw-   0        0        0      293 2023-08-05 04:07:23.000000 ykenan_file-0.2.3/src/ykenan_file/_util_.py
-drwxrwxrwx   0        0        0        0 2023-08-17 01:46:18.334027 ykenan_file-0.2.3/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      827 2023-08-17 01:46:18.000000 ykenan_file-0.2.3/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-08-17 01:46:18.000000 ykenan_file-0.2.3/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-17 01:46:18.000000 ykenan_file-0.2.3/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-17 01:46:18.000000 ykenan_file-0.2.3/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-17 01:46:18.000000 ykenan_file-0.2.3/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 05:31:14.431608 ykenan_file-0.2.4/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      924 2024-04-13 05:31:14.430604 ykenan_file-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.2.4/README.md
+-rw-rw-rw-   0        0        0      716 2024-04-13 05:17:43.000000 ykenan_file-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-04-13 05:14:05.000000 ykenan_file-0.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 05:31:14.431608 ykenan_file-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 05:31:14.393605 ykenan_file-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 05:31:14.415603 ykenan_file-0.2.4/src/ykenan_file/
+-rw-rw-rw-   0        0        0      274 2023-08-05 04:07:23.000000 ykenan_file-0.2.4/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0    10813 2023-08-05 04:07:23.000000 ykenan_file-0.2.4/src/ykenan_file/_create_.py
+-rw-rw-rw-   0        0        0     3689 2023-08-05 04:07:23.000000 ykenan_file-0.2.4/src/ykenan_file/_read_.py
+-rw-rw-rw-   0        0        0    12944 2023-08-05 04:07:23.000000 ykenan_file-0.2.4/src/ykenan_file/_static_method_.py
+-rw-rw-rw-   0        0        0     3870 2023-08-17 01:43:58.000000 ykenan_file-0.2.4/src/ykenan_file/_thread_file_.py
+-rw-rw-rw-   0        0        0      293 2023-08-05 04:07:23.000000 ykenan_file-0.2.4/src/ykenan_file/_util_.py
+drwxrwxrwx   0        0        0        0 2024-04-13 05:31:14.430604 ykenan_file-0.2.4/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      924 2024-04-13 05:31:14.000000 ykenan_file-0.2.4/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-13 05:31:14.000000 ykenan_file-0.2.4/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 05:31:14.000000 ykenan_file-0.2.4/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-13 05:31:14.000000 ykenan_file-0.2.4/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 05:31:14.000000 ykenan_file-0.2.4/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.2.3/LICENSE` & `ykenan_file-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.3/PKG-INFO` & `ykenan_file-0.2.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.2.3
+Version: 0.2.4
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ykenan-log>=0.2.1
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: requests>=2.30.0
 
 # ykenan_file
 
 > **`File read and write operations`**
 
 This is a simple log package. You can see
 [Github-ykenan_file](https://github.com/YuZhengM/ykenan_file)
```

### Comparing `ykenan_file-0.2.3/pyproject.toml` & `ykenan_file-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
+requires = ["setuptools>=42", "ykenan-log>=0.2.1", "pandas>=1.5.3", "requests>=2.30.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
+dependencies = ["ykenan-log>=0.2.1", "pandas>=1.5.3", "requests>=2.30.0"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 github = "https://github.com/YuZhengM/ykenan_file"
```

### Comparing `ykenan_file-0.2.3/src/ykenan_file/_create_.py` & `ykenan_file-0.2.4/src/ykenan_file/_create_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.3/src/ykenan_file/_read_.py` & `ykenan_file-0.2.4/src/ykenan_file/_read_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.3/src/ykenan_file/_static_method_.py` & `ykenan_file-0.2.4/src/ykenan_file/_static_method_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.3/src/ykenan_file/_thread_file_.py` & `ykenan_file-0.2.4/src/ykenan_file/_thread_file_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.3/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.2.4/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
-Name: ykenan-file
-Version: 0.2.3
+Name: ykenan_file
+Version: 0.2.4
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ykenan-log>=0.2.1
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: requests>=2.30.0
 
 # ykenan_file
 
 > **`File read and write operations`**
 
 This is a simple log package. You can see
 [Github-ykenan_file](https://github.com/YuZhengM/ykenan_file)
```

