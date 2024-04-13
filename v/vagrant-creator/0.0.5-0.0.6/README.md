# Comparing `tmp/vagrant-creator-0.0.5.tar.gz` & `tmp/vagrant-creator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagrant-creator-0.0.5.tar", last modified: Fri Apr 12 15:53:18 2024, max compression
+gzip compressed data, was "vagrant-creator-0.0.6.tar", last modified: Sat Apr 13 17:56:36 2024, max compression
```

## Comparing `vagrant-creator-0.0.5.tar` & `vagrant-creator-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.778756 vagrant-creator-0.0.5/
--rw-rw-rw-   0        0        0     1636 2024-04-12 15:53:18.777742 vagrant-creator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      975 2024-04-12 15:49:21.000000 vagrant-creator-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 15:53:18.778756 vagrant-creator-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1104 2024-04-12 15:50:36.000000 vagrant-creator-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.772836 vagrant-creator-0.0.5/vagrant_creator/
--rw-rw-rw-   0        0        0        1 2024-04-12 07:39:23.000000 vagrant-creator-0.0.5/vagrant_creator/__init__.py
--rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.5/vagrant_creator/vagrant_creator.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.777742 vagrant-creator-0.0.5/vagrant_creator.egg-info/
--rw-rw-rw-   0        0        0     1636 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 17:56:36.073195 vagrant-creator-0.0.6/
+-rw-rw-rw-   0        0        0     3722 2024-04-13 17:56:36.072194 vagrant-creator-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2024-04-13 17:54:38.000000 vagrant-creator-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 17:56:36.073195 vagrant-creator-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-04-13 17:56:27.000000 vagrant-creator-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 17:56:36.065195 vagrant-creator-0.0.6/vagrant_creator/
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:39:23.000000 vagrant-creator-0.0.6/vagrant_creator/__init__.py
+-rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.6/vagrant_creator/vagrant_creator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 17:56:36.071194 vagrant-creator-0.0.6/vagrant_creator.egg-info/
+-rw-rw-rw-   0        0        0     3722 2024-04-13 17:56:35.000000 vagrant-creator-0.0.6/vagrant_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-13 17:56:36.000000 vagrant-creator-0.0.6/vagrant_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 17:56:35.000000 vagrant-creator-0.0.6/vagrant_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-13 17:56:35.000000 vagrant-creator-0.0.6/vagrant_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-13 17:56:35.000000 vagrant-creator-0.0.6/vagrant_creator.egg-info/top_level.txt
```

### Comparing `vagrant-creator-0.0.5/setup.py` & `vagrant-creator-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name='vagrant-creator',
-    version='0.0.5',
+    version='0.0.6',
     author='Chandula Jayathilake',
     author_email='chandulaj3000@gmail.com',
     description='A tool to generate Vagrant init files with custom configurations',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ChandulaJ/vagrant-creator',
     license='MIT',
```

### Comparing `vagrant-creator-0.0.5/vagrant_creator/vagrant_creator.py` & `vagrant-creator-0.0.6/vagrant_creator/vagrant_creator.py`

 * *Files identical despite different names*

