# Comparing `tmp/lapa_authentication-0.0.6.tar.gz` & `tmp/lapa_authentication-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_authentication-0.0.6.tar", last modified: Sat Mar 16 12:27:50 2024, max compression
+gzip compressed data, was "lapa_authentication-0.0.7.tar", last modified: Fri Apr 12 17:06:27 2024, max compression
```

## Comparing `lapa_authentication-0.0.6.tar` & `lapa_authentication-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/lapa_authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/lapa_authentication/data/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/data/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/lapa_authentication/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/entity/Models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/lapa_authentication/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/utils/CommonEnums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/utils/Helper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/lapa_authentication/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/lapa_authentication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-16 12:27:50.000000 lapa_authentication-0.0.6/lapa_authentication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-16 12:27:50.000000 lapa_authentication-0.0.6/lapa_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 12:27:50.000000 lapa_authentication-0.0.6/lapa_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 12:27:50.000000 lapa_authentication-0.0.6/lapa_authentication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-16 12:27:50.000000 lapa_authentication-0.0.6/lapa_authentication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 12:27:50.395834 lapa_authentication-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-16 12:27:42.000000 lapa_authentication-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.221861 lapa_authentication-0.0.7/lapa_authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/lapa_authentication/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/lapa_authentication/pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/pydantic_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/pydantic_models/pydantic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/lapa_authentication/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/routes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/lapa_authentication/routes/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/lapa_authentication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-12 17:06:27.000000 lapa_authentication-0.0.7/lapa_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 17:06:27.000000 lapa_authentication-0.0.7/lapa_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:06:27.000000 lapa_authentication-0.0.7/lapa_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 17:06:27.000000 lapa_authentication-0.0.7/lapa_authentication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 17:06:27.000000 lapa_authentication-0.0.7/lapa_authentication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:06:27.225861 lapa_authentication-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 17:06:18.000000 lapa_authentication-0.0.7/setup.py
```

### Comparing `lapa_authentication-0.0.6/PKG-INFO` & `lapa_authentication-0.0.7/lapa_authentication.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa_authentication
-Version: 0.0.6
+Name: lapa-authentication
+Version: 0.0.7
 Summary: authentication service for my personal server.
 Home-page: https://github.com/lavvsharma/lapa_authentication
 Author: Lav Sharma, thePmSquare
 Author-email: lavsharma2016@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,19 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.7
+
+- overhaul register logic.
+- overhaul tablename import logic.
+
 ### v0.0.6
 
 - syntax error fix in main.py.
 
 ### v0.0.5
 
 - update database tables.
```

### Comparing `lapa_authentication-0.0.6/README.md` & `lapa_authentication-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.7
+
+- overhaul register logic.
+- overhaul tablename import logic.
+
 ### v0.0.6
 
 - syntax error fix in main.py.
 
 ### v0.0.5
 
 - update database tables.
```

### Comparing `lapa_authentication-0.0.6/lapa_authentication.egg-info/PKG-INFO` & `lapa_authentication-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa-authentication
-Version: 0.0.6
+Name: lapa_authentication
+Version: 0.0.7
 Summary: authentication service for my personal server.
 Home-page: https://github.com/lavvsharma/lapa_authentication
 Author: Lav Sharma, thePmSquare
 Author-email: lavsharma2016@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,19 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.7
+
+- overhaul register logic.
+- overhaul tablename import logic.
+
 ### v0.0.6
 
 - syntax error fix in main.py.
 
 ### v0.0.5
 
 - update database tables.
```

### Comparing `lapa_authentication-0.0.6/lapa_authentication.egg-info/SOURCES.txt` & `lapa_authentication-0.0.7/lapa_authentication.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 lapa_authentication/main.py
 lapa_authentication.egg-info/PKG-INFO
 lapa_authentication.egg-info/SOURCES.txt
 lapa_authentication.egg-info/dependency_links.txt
 lapa_authentication.egg-info/requires.txt
 lapa_authentication.egg-info/top_level.txt
 lapa_authentication/data/config.ini
-lapa_authentication/entity/Models.py
-lapa_authentication/entity/__init__.py
-lapa_authentication/utils/CommonEnums.py
-lapa_authentication/utils/Helper.py
-lapa_authentication/utils/__init__.py
+lapa_authentication/pydantic_models/__init__.py
+lapa_authentication/pydantic_models/pydantic_models.py
+lapa_authentication/routes/__init__.py
+lapa_authentication/routes/core.py
+lapa_authentication/routes/utility.py
```

### Comparing `lapa_authentication-0.0.6/setup.py` & `lapa_authentication-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_authentication"
 
 setup(
     name=package_name,
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     package_data={
         package_name: ["data/*"],
     },
     install_requires=[
         "uvicorn>=0.24.0.post1",
         "fastapi>=0.104.1",
         "square_logger~=1.0",
-        "bcrypt>=4.1.2",
         "pydantic>=2.5.3",
-        "lapa_database_structure>=0.0.4",
-        "lapa_database_helper>=0.0.3",
         "lapa_commons>=0.0.1",
-        "email_validator>=2.0.0",
+        "bcrypt>=4.1.2",
+        "pyjwt>=2.8.0"
     ],
     extras_require={},
     author="Lav Sharma, thePmSquare",
     author_email="lavsharma2016@gmail.com, thepmsquare@gmail.com",
     description="authentication service for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
```

