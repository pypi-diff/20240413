# Comparing `tmp/simple-value-object-2.0.tar.gz` & `tmp/simple_value_object-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-value-object-2.0.tar", last modified: Thu Oct 27 21:28:27 2022, max compression
+gzip compressed data, was "simple_value_object-3.0.tar", last modified: Sat Apr 13 21:21:15 2024, max compression
```

## Comparing `simple-value-object-2.0.tar` & `simple_value_object-3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 21:28:27.319559 simple-value-object-2.0/
--rw-rw-r--   0 root         (0) root         (0)      315 2022-10-27 17:21:41.000000 simple-value-object-2.0/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)     1057 2022-09-19 20:07:23.000000 simple-value-object-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4050 2022-10-27 21:28:27.319559 simple-value-object-2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3360 2022-10-27 17:21:41.000000 simple-value-object-2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-27 21:28:27.319559 simple-value-object-2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      877 2022-10-27 17:21:41.000000 simple-value-object-2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 21:28:27.315559 simple-value-object-2.0/simple_value_object/
--rw-rw-r--   0 root         (0) root         (0)      477 2022-10-27 17:21:41.000000 simple-value-object-2.0/simple_value_object/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      176 2022-10-27 17:21:41.000000 simple-value-object-2.0/simple_value_object/decorators.py
--rw-rw-r--   0 root         (0) root         (0)      612 2022-10-27 17:27:23.000000 simple-value-object-2.0/simple_value_object/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     4306 2022-10-27 17:21:57.000000 simple-value-object-2.0/simple_value_object/value_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 21:28:27.315559 simple-value-object-2.0/simple_value_object.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4050 2022-10-27 21:28:27.000000 simple-value-object-2.0/simple_value_object.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2022-10-27 21:28:27.000000 simple-value-object-2.0/simple_value_object.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 21:28:27.000000 simple-value-object-2.0/simple_value_object.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-10-27 21:28:27.000000 simple-value-object-2.0/simple_value_object.egg-info/top_level.txt
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.311469 simple_value_object-3.0/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple_value_object-3.0/AUTHORS
+-rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple_value_object-3.0/LICENSE
+-rw-r--r--   0 quique    (1000) quique    (1000)     3836 2024-04-13 21:21:15.307469 simple_value_object-3.0/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3107 2024-04-13 21:09:50.000000 simple_value_object-3.0/README.md
+-rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-04-13 21:21:15.311469 simple_value_object-3.0/setup.cfg
+-rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:20:52.000000 simple_value_object-3.0/setup.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.307469 simple_value_object-3.0/simple_value_object/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-04-13 20:49:58.000000 simple_value_object-3.0/simple_value_object/__init__.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      233 2024-04-13 20:49:19.000000 simple_value_object-3.0/simple_value_object/decorators.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 20:49:45.000000 simple_value_object-3.0/simple_value_object/exceptions.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3725 2024-04-13 20:58:57.000000 simple_value_object-3.0/simple_value_object/value_object.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.307469 simple_value_object-3.0/simple_value_object.egg-info/
+-rw-r--r--   0 quique    (1000) quique    (1000)     3836 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/SOURCES.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/dependency_links.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/top_level.txt
```

### Comparing `simple-value-object-2.0/LICENSE` & `simple_value_object-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-value-object-2.0/setup.py` & `simple_value_object-3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup
 
 from simple_value_object import get_version
 
 
 setup(
-    name='simple-value-object',
+    name="simple-value-object",
     version=get_version(),
-    license='MIT/X11',
-    author='Quique Porta',
-    author_email='quiqueporta@gmail.com',
-    description='A simple mixin to create Value Objects',
-    long_description=open('README.rst').read(),
-    url='https://github.com/quiqueporta/value-object',
-    download_url='https://github.com/quiqueporta/simple-value-object/releases',
-    keywords=['python', 'ddd'],
-    packages=['simple_value_object'],
+    license="MIT/X11",
+    author="Quique Porta",
+    author_email="me@quiqueporta.com",
+    description="A simple library to create Value Objects",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/quiqueporta/value-object",
+    download_url="https://github.com/quiqueporta/simple-value-object/releases",
+    keywords=["python", "ddd"],
+    packages=["simple_value_object"],
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Topic :: Utilities',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Topic :: Utilities",
     ],
 )
```

