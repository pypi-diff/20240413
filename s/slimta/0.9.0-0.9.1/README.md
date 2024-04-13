# Comparing `tmp/slimta-0.9.0.tar.gz` & `tmp/slimta-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slimta-0.9.0.tar", last modified: Sun Nov  6 21:15:44 2022, max compression
+gzip compressed data, was "slimta-0.9.1.tar", last modified: Sat Apr 13 20:08:14 2024, max compression
```

## Comparing `slimta-0.9.0.tar` & `slimta-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 21:15:44.375728 slimta-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-06 21:15:33.000000 slimta-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-06 21:15:33.000000 slimta-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-11-06 21:15:44.375728 slimta-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-11-06 21:15:33.000000 slimta-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-06 21:15:44.375728 slimta-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-11-06 21:15:33.000000 slimta-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 21:15:44.371729 slimta-0.9.0/slimta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 21:15:44.371729 slimta-0.9.0/slimta/app/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 21:15:44.375728 slimta-0.9.0/slimta/app/etc/
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/etc/init-lsb.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/etc/init-systemd.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/etc/logging.yaml.sample
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/etc/slimta.yaml.sample
--rw-r--r--   0 runner    (1001) docker     (121)    10258 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/importutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/listeners.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     7013 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    21107 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/state.py
--rw-r--r--   0 runner    (1001) docker     (121)    11056 2022-11-06 21:15:33.000000 slimta-0.9.0/slimta/app/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 21:15:44.371729 slimta-0.9.0/slimta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-06 21:15:44.000000 slimta-0.9.0/slimta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:08:14.365650 slimta-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 20:08:06.000000 slimta-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 20:08:06.000000 slimta-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-13 20:08:14.365650 slimta-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-13 20:08:06.000000 slimta-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-13 20:08:14.365650 slimta-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-13 20:08:06.000000 slimta-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:08:14.357650 slimta-0.9.1/slimta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:08:14.361650 slimta-0.9.1/slimta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:08:14.361650 slimta-0.9.1/slimta/app/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/etc/init-lsb.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/etc/init-systemd.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/etc/logging.yaml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/etc/slimta.yaml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/importutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21107 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-13 20:08:06.000000 slimta-0.9.1/slimta/app/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:08:14.361650 slimta-0.9.1/slimta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 20:08:14.000000 slimta-0.9.1/slimta.egg-info/top_level.txt
```

### Comparing `slimta-0.9.0/LICENSE.md` & `slimta-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/PKG-INFO` & `slimta-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: slimta
-Version: 0.9.0
+Version: 0.9.1
 Summary: Configurable MTA based on the python-slimta library.
 Home-page: http://slimta.org/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: optional
 License-File: LICENSE.md
+Requires-Dist: python-slimta[spf]~=5.0
+Requires-Dist: pysasl<1.1
+Requires-Dist: passlib
+Requires-Dist: PyYAML
+Provides-Extra: optional
+Requires-Dist: python-slimta[aws,disk,redis]~=5.0; extra == "optional"
 
 #### [Project Homepage][1]
 #### [Usage Manual][2]
 
 --------------------
 
 About
```

### Comparing `slimta-0.9.0/README.md` & `slimta-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/setup.py` & `slimta-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,30 @@
 with open('README.md') as f:
     readme = f.read()
 
 with open('LICENSE.md') as f:
     license = f.read()
 
 setup(name='slimta',
-      version='0.9.0',
+      version='0.9.1',
       author='Ian Good',
       author_email='ian@icgood.net',
       description='Configurable MTA based on the python-slimta library.',
       long_description=readme + license,
       long_description_content_type='text/markdown',
       license='MIT',
       url='http://slimta.org/',
       python_requires='~=3.11',
       include_package_data=True,
       packages=find_namespace_packages(include=['slimta.*']),
-      install_requires=['python-slimta[spf] ~= 5.0', 'passlib', 'PyYAML'],
+      install_requires=[
+          'python-slimta[spf] ~= 5.0',
+          'pysasl < 1.1',
+          'passlib',
+          'PyYAML'],
       extras_require={
           'optional': ['python-slimta[redis,aws,disk] ~= 5.0']},
       entry_points={'console_scripts': [
               'slimta = slimta.app.main:main',
               'slimta-setup = slimta.app.setup:setup']},
       classifiers=['Development Status :: 3 - Alpha',
                    'Topic :: Communications :: Email :: Mail Transport Agents',
```

### Comparing `slimta-0.9.0/slimta/app/__init__.py` & `slimta-0.9.1/slimta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/config.py` & `slimta-0.9.1/slimta/app/config.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/etc/init-lsb.tmpl` & `slimta-0.9.1/slimta/app/etc/init-lsb.tmpl`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/etc/slimta.yaml.sample` & `slimta-0.9.1/slimta/app/etc/slimta.yaml.sample`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/helpers.py` & `slimta-0.9.1/slimta/app/helpers.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/importutil.py` & `slimta-0.9.1/slimta/app/importutil.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/listeners.py` & `slimta-0.9.1/slimta/app/listeners.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/logging.py` & `slimta-0.9.1/slimta/app/logging.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/lookup.py` & `slimta-0.9.1/slimta/app/lookup.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/main.py` & `slimta-0.9.1/slimta/app/main.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/setup.py` & `slimta-0.9.1/slimta/app/setup.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/state.py` & `slimta-0.9.1/slimta/app/state.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta/app/validation.py` & `slimta-0.9.1/slimta/app/validation.py`

 * *Files identical despite different names*

### Comparing `slimta-0.9.0/slimta.egg-info/PKG-INFO` & `slimta-0.9.1/slimta.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: slimta
-Version: 0.9.0
+Version: 0.9.1
 Summary: Configurable MTA based on the python-slimta library.
 Home-page: http://slimta.org/
 Author: Ian Good
 Author-email: ian@icgood.net
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: optional
 License-File: LICENSE.md
+Requires-Dist: python-slimta[spf]~=5.0
+Requires-Dist: pysasl<1.1
+Requires-Dist: passlib
+Requires-Dist: PyYAML
+Provides-Extra: optional
+Requires-Dist: python-slimta[aws,disk,redis]~=5.0; extra == "optional"
 
 #### [Project Homepage][1]
 #### [Usage Manual][2]
 
 --------------------
 
 About
```

### Comparing `slimta-0.9.0/slimta.egg-info/SOURCES.txt` & `slimta-0.9.1/slimta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

