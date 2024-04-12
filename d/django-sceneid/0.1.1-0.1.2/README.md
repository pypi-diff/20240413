# Comparing `tmp/django-sceneid-0.1.1.tar.gz` & `tmp/django-sceneid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-sceneid-0.1.1.tar", last modified: Wed Jul 13 09:41:17 2022, max compression
+gzip compressed data, was "django-sceneid-0.1.2.tar", last modified: Fri Apr 12 22:34:06 2024, max compression
```

## Comparing `django-sceneid-0.1.1.tar` & `django-sceneid-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.515163 django-sceneid-0.1.1/
--rw-r--r--   0 matthew    (501) staff       (20)      227 2022-07-13 09:40:14.000000 django-sceneid-0.1.1/CHANGELOG.md
--rw-r--r--   0 matthew    (501) staff       (20)     1479 2021-05-06 22:27:46.000000 django-sceneid-0.1.1/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      170 2021-05-08 17:10:44.000000 django-sceneid-0.1.1/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     9310 2022-07-13 09:41:17.514786 django-sceneid-0.1.1/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     7384 2022-07-13 09:40:14.000000 django-sceneid-0.1.1/README.md
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.505012 django-sceneid-0.1.1/django_sceneid.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)     9310 2022-07-13 09:41:17.000000 django-sceneid-0.1.1/django_sceneid.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      739 2022-07-13 09:41:17.000000 django-sceneid-0.1.1/django_sceneid.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2022-07-13 09:41:17.000000 django-sceneid-0.1.1/django_sceneid.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       63 2022-07-13 09:41:17.000000 django-sceneid-0.1.1/django_sceneid.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)        8 2022-07-13 09:41:17.000000 django-sceneid-0.1.1/django_sceneid.egg-info/top_level.txt
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.508686 django-sceneid-0.1.1/sceneid/
--rw-r--r--   0 matthew    (501) staff       (20)       68 2022-07-13 09:40:14.000000 django-sceneid-0.1.1/sceneid/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      343 2021-05-08 13:39:00.000000 django-sceneid-0.1.1/sceneid/apps.py
--rw-r--r--   0 matthew    (501) staff       (20)     1362 2021-05-07 18:23:18.000000 django-sceneid-0.1.1/sceneid/client.py
--rw-r--r--   0 matthew    (501) staff       (20)     1270 2021-05-08 15:21:25.000000 django-sceneid-0.1.1/sceneid/forms.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.510096 django-sceneid-0.1.1/sceneid/migrations/
--rw-r--r--   0 matthew    (501) staff       (20)      770 2021-05-07 21:42:16.000000 django-sceneid-0.1.1/sceneid/migrations/0001_initial.py
--rw-r--r--   0 matthew    (501) staff       (20)        0 2021-05-07 21:33:16.000000 django-sceneid-0.1.1/sceneid/migrations/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      260 2021-05-07 21:42:10.000000 django-sceneid-0.1.1/sceneid/models.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.498568 django-sceneid-0.1.1/sceneid/static/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.498760 django-sceneid-0.1.1/sceneid/static/sceneid/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.511502 django-sceneid-0.1.1/sceneid/static/sceneid/images/
--rw-r--r--   0 matthew    (501) staff       (20)     1524 2021-05-07 22:51:50.000000 django-sceneid-0.1.1/sceneid/static/sceneid/images/login-large.png
--rw-r--r--   0 matthew    (501) staff       (20)      469 2021-05-07 22:51:19.000000 django-sceneid-0.1.1/sceneid/static/sceneid/images/login-small.png
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.499119 django-sceneid-0.1.1/sceneid/templates/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.512108 django-sceneid-0.1.1/sceneid/templates/sceneid/
--rw-r--r--   0 matthew    (501) staff       (20)     1177 2021-05-08 15:06:59.000000 django-sceneid-0.1.1/sceneid/templates/sceneid/connect.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.513216 django-sceneid-0.1.1/sceneid/templates/sceneid/tags/
--rw-r--r--   0 matthew    (501) staff       (20)      154 2021-05-07 23:02:11.000000 django-sceneid-0.1.1/sceneid/templates/sceneid/tags/login_button_large.html
--rw-r--r--   0 matthew    (501) staff       (20)      153 2021-05-07 23:01:49.000000 django-sceneid-0.1.1/sceneid/templates/sceneid/tags/login_button_small.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-07-13 09:41:17.513974 django-sceneid-0.1.1/sceneid/templatetags/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2021-05-07 22:55:59.000000 django-sceneid-0.1.1/sceneid/templatetags/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      905 2021-05-08 01:21:09.000000 django-sceneid-0.1.1/sceneid/templatetags/sceneid_tags.py
--rw-r--r--   0 matthew    (501) staff       (20)      442 2021-05-08 01:34:53.000000 django-sceneid-0.1.1/sceneid/urls.py
--rw-r--r--   0 matthew    (501) staff       (20)     8013 2021-05-08 13:42:09.000000 django-sceneid-0.1.1/sceneid/views.py
--rw-r--r--   0 matthew    (501) staff       (20)       38 2022-07-13 09:41:17.515352 django-sceneid-0.1.1/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1269 2022-07-13 09:40:31.000000 django-sceneid-0.1.1/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.788555 django-sceneid-0.1.2/
+-rw-r--r--   0 matthew    (501) staff       (20)      323 2024-04-12 22:33:07.000000 django-sceneid-0.1.2/CHANGELOG.md
+-rw-r--r--   0 matthew    (501) staff       (20)     1479 2021-05-06 22:27:46.000000 django-sceneid-0.1.2/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      170 2021-05-08 17:10:44.000000 django-sceneid-0.1.2/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)     9427 2024-04-12 22:34:06.788164 django-sceneid-0.1.2/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     7384 2022-07-13 09:40:14.000000 django-sceneid-0.1.2/README.md
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.778023 django-sceneid-0.1.2/django_sceneid.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)     9427 2024-04-12 22:34:06.000000 django-sceneid-0.1.2/django_sceneid.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      739 2024-04-12 22:34:06.000000 django-sceneid-0.1.2/django_sceneid.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2024-04-12 22:34:06.000000 django-sceneid-0.1.2/django_sceneid.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       60 2024-04-12 22:34:06.000000 django-sceneid-0.1.2/django_sceneid.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        8 2024-04-12 22:34:06.000000 django-sceneid-0.1.2/django_sceneid.egg-info/top_level.txt
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.782479 django-sceneid-0.1.2/sceneid/
+-rw-r--r--   0 matthew    (501) staff       (20)       68 2022-07-13 09:40:14.000000 django-sceneid-0.1.2/sceneid/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      343 2021-05-08 13:39:00.000000 django-sceneid-0.1.2/sceneid/apps.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1362 2021-05-07 18:23:18.000000 django-sceneid-0.1.2/sceneid/client.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1270 2021-05-08 15:21:25.000000 django-sceneid-0.1.2/sceneid/forms.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.783539 django-sceneid-0.1.2/sceneid/migrations/
+-rw-r--r--   0 matthew    (501) staff       (20)      770 2021-05-07 21:42:16.000000 django-sceneid-0.1.2/sceneid/migrations/0001_initial.py
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2021-05-07 21:33:16.000000 django-sceneid-0.1.2/sceneid/migrations/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      260 2021-05-07 21:42:10.000000 django-sceneid-0.1.2/sceneid/models.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.772198 django-sceneid-0.1.2/sceneid/static/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.772307 django-sceneid-0.1.2/sceneid/static/sceneid/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.784381 django-sceneid-0.1.2/sceneid/static/sceneid/images/
+-rw-r--r--   0 matthew    (501) staff       (20)     1524 2021-05-07 22:51:50.000000 django-sceneid-0.1.2/sceneid/static/sceneid/images/login-large.png
+-rw-r--r--   0 matthew    (501) staff       (20)      469 2021-05-07 22:51:19.000000 django-sceneid-0.1.2/sceneid/static/sceneid/images/login-small.png
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.772556 django-sceneid-0.1.2/sceneid/templates/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.784970 django-sceneid-0.1.2/sceneid/templates/sceneid/
+-rw-r--r--   0 matthew    (501) staff       (20)     1177 2021-05-08 15:06:59.000000 django-sceneid-0.1.2/sceneid/templates/sceneid/connect.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.786620 django-sceneid-0.1.2/sceneid/templates/sceneid/tags/
+-rw-r--r--   0 matthew    (501) staff       (20)      154 2021-05-07 23:02:11.000000 django-sceneid-0.1.2/sceneid/templates/sceneid/tags/login_button_large.html
+-rw-r--r--   0 matthew    (501) staff       (20)      153 2021-05-07 23:01:49.000000 django-sceneid-0.1.2/sceneid/templates/sceneid/tags/login_button_small.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-04-12 22:34:06.787488 django-sceneid-0.1.2/sceneid/templatetags/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2021-05-07 22:55:59.000000 django-sceneid-0.1.2/sceneid/templatetags/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      905 2021-05-08 01:21:09.000000 django-sceneid-0.1.2/sceneid/templatetags/sceneid_tags.py
+-rw-r--r--   0 matthew    (501) staff       (20)      442 2021-05-08 01:34:53.000000 django-sceneid-0.1.2/sceneid/urls.py
+-rw-r--r--   0 matthew    (501) staff       (20)     8013 2021-05-08 13:42:09.000000 django-sceneid-0.1.2/sceneid/views.py
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2024-04-12 22:34:06.788665 django-sceneid-0.1.2/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1380 2024-04-12 22:33:21.000000 django-sceneid-0.1.2/setup.py
```

### Comparing `django-sceneid-0.1.1/LICENSE` & `django-sceneid-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/PKG-INFO` & `django-sceneid-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sceneid
-Version: 0.1.1
+Version: 0.1.2
 Summary: SceneID authentication for Django
 Home-page: https://github.com/demozoo/django-sceneid/
 Author: Matt Westcott
 Author-email: matt@west.co.tt
 License: BSD
 Description: django-sceneid
         ==============
@@ -151,13 +151,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `django-sceneid-0.1.1/README.md` & `django-sceneid-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/django_sceneid.egg-info/PKG-INFO` & `django-sceneid-0.1.2/django_sceneid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sceneid
-Version: 0.1.1
+Version: 0.1.2
 Summary: SceneID authentication for Django
 Home-page: https://github.com/demozoo/django-sceneid/
 Author: Matt Westcott
 Author-email: matt@west.co.tt
 License: BSD
 Description: django-sceneid
         ==============
@@ -151,13 +151,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `django-sceneid-0.1.1/django_sceneid.egg-info/SOURCES.txt` & `django-sceneid-0.1.2/django_sceneid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/client.py` & `django-sceneid-0.1.2/sceneid/client.py`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/forms.py` & `django-sceneid-0.1.2/sceneid/forms.py`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/migrations/0001_initial.py` & `django-sceneid-0.1.2/sceneid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/static/sceneid/images/login-large.png` & `django-sceneid-0.1.2/sceneid/static/sceneid/images/login-large.png`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/templates/sceneid/connect.html` & `django-sceneid-0.1.2/sceneid/templates/sceneid/connect.html`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/templatetags/sceneid_tags.py` & `django-sceneid-0.1.2/sceneid/templatetags/sceneid_tags.py`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/sceneid/views.py` & `django-sceneid-0.1.2/sceneid/views.py`

 * *Files identical despite different names*

### Comparing `django-sceneid-0.1.1/setup.py` & `django-sceneid-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="django-sceneid",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(exclude=('tests',)),
     include_package_data=True,
     test_suite="tests",
     url="https://github.com/demozoo/django-sceneid/",
 
     author="Matt Westcott",
     author_email="matt@west.co.tt",
@@ -21,21 +21,24 @@
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Topic :: Internet :: WWW/HTTP",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'Django>=3.0,<5',
+        'Django>=3.0',
         'requests>=2,<3',
     ],
     extras_require={
         "testing": [
             'responses>=0.14,<0.21',
         ]
     },
```

