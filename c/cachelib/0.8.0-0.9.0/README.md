# Comparing `tmp/cachelib-0.8.0.tar.gz` & `tmp/cachelib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cachelib-0.8.0.tar", last modified: Tue Jun 14 01:53:00 2022, max compression
+gzip compressed data, was "dist/cachelib-0.9.0.tar", last modified: Sun Jun 26 17:53:28 2022, max compression
```

## Comparing `cachelib-0.8.0.tar` & `cachelib-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2809 2022-06-14 01:46:19.000000 cachelib-0.8.0/CHANGES.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1475 2022-03-12 20:20:34.000000 cachelib-0.8.0/LICENSE.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      155 2022-03-12 20:20:34.000000 cachelib-0.8.0/MANIFEST.in
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2272 2022-06-14 01:53:00.000000 cachelib-0.8.0/PKG-INFO
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      948 2022-03-12 20:20:34.000000 cachelib-0.8.0/README.rst
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/docs/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      634 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/Makefile
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      103 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/base.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)       45 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/changes.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1670 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/conf.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      111 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/file.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      254 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/index.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)       71 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/license.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      795 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/make.bat
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      126 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/memcached.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      114 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/redis.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      131 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/simple.rst
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      114 2022-03-12 20:20:34.000000 cachelib-0.8.0/docs/uwsgi.rst
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/requirements/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2996 2022-06-14 01:43:28.000000 cachelib-0.8.0/requirements/dev.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1389 2022-04-16 16:55:25.000000 cachelib-0.8.0/requirements/docs.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      738 2022-06-14 01:43:28.000000 cachelib-0.8.0/requirements/tests.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      310 2022-06-14 01:43:28.000000 cachelib-0.8.0/requirements/typing.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1865 2022-06-14 01:53:00.000000 cachelib-0.8.0/setup.cfg
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)       53 2022-03-12 20:20:34.000000 cachelib-0.8.0/setup.py
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      447 2022-06-14 01:45:40.000000 cachelib-0.8.0/src/cachelib/__init__.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     6713 2022-03-12 20:20:34.000000 cachelib-0.8.0/src/cachelib/base.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)    11188 2022-04-16 16:55:25.000000 cachelib-0.8.0/src/cachelib/file.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     7147 2022-03-12 20:20:34.000000 cachelib-0.8.0/src/cachelib/memcached.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)        0 2022-03-12 20:20:34.000000 cachelib-0.8.0/src/cachelib/py.typed
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     5490 2022-06-14 01:43:28.000000 cachelib-0.8.0/src/cachelib/redis.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3117 2022-06-14 01:43:28.000000 cachelib-0.8.0/src/cachelib/serializers.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3481 2022-03-12 20:20:34.000000 cachelib-0.8.0/src/cachelib/simple.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2563 2022-03-12 20:20:34.000000 cachelib-0.8.0/src/cachelib/uwsgi.py
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib.egg-info/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2272 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib.egg-info/PKG-INFO
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      963 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib.egg-info/SOURCES.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)        1 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib.egg-info/dependency_links.txt
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)        9 2022-06-14 01:53:00.000000 cachelib-0.8.0/src/cachelib.egg-info/top_level.txt
-drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-14 01:53:00.000000 cachelib-0.8.0/tests/
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      332 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/clear.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3042 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/common.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2532 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/conftest.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      346 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/has.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1886 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_base_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3726 2022-03-20 15:48:39.000000 cachelib-0.8.0/tests/test_file_system_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      962 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_interface_uniformity.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      490 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_memcached_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1020 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_redis_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1649 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_simple_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1063 2022-03-12 20:20:34.000000 cachelib-0.8.0/tests/test_uwsgi_cache.py
--rw-r--r--   0 gfvante   (1000) gfvante   (1000)      803 2022-04-16 16:55:25.000000 cachelib-0.8.0/tox.ini
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3176 2022-06-26 17:37:21.000000 cachelib-0.9.0/CHANGES.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1475 2022-03-12 20:20:34.000000 cachelib-0.9.0/LICENSE.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      155 2022-06-25 20:21:53.000000 cachelib-0.9.0/MANIFEST.in
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2272 2022-06-26 17:53:28.000000 cachelib-0.9.0/PKG-INFO
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      948 2022-06-25 20:21:53.000000 cachelib-0.9.0/README.rst
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/docs/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      634 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/Makefile
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      103 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/base.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)       45 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/changes.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1670 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/conf.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      111 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/file.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      254 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/index.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)       71 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/license.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      795 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/make.bat
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      126 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/memcached.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      114 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/redis.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      131 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/simple.rst
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      114 2022-03-12 20:20:34.000000 cachelib-0.9.0/docs/uwsgi.rst
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/requirements/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2996 2022-06-25 20:21:53.000000 cachelib-0.9.0/requirements/dev.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1389 2022-06-25 20:21:53.000000 cachelib-0.9.0/requirements/docs.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      738 2022-06-25 20:21:53.000000 cachelib-0.9.0/requirements/tests.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      310 2022-06-25 20:21:53.000000 cachelib-0.9.0/requirements/typing.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1865 2022-06-26 17:53:28.000000 cachelib-0.9.0/setup.cfg
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)       53 2022-03-12 20:20:34.000000 cachelib-0.9.0/setup.py
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      447 2022-06-26 17:36:38.000000 cachelib-0.9.0/src/cachelib/__init__.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     6713 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/base.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)    11642 2022-06-25 20:21:57.000000 cachelib-0.9.0/src/cachelib/file.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     7147 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/memcached.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)        0 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/py.typed
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     5945 2022-06-26 17:46:46.000000 cachelib-0.9.0/src/cachelib/redis.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3117 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/serializers.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3481 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/simple.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2563 2022-06-25 20:21:53.000000 cachelib-0.9.0/src/cachelib/uwsgi.py
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib.egg-info/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2272 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib.egg-info/PKG-INFO
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      963 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib.egg-info/SOURCES.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)        1 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib.egg-info/dependency_links.txt
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)        9 2022-06-26 17:53:28.000000 cachelib-0.9.0/src/cachelib.egg-info/top_level.txt
+drwxr-xr-x   0 gfvante   (1000) gfvante   (1000)        0 2022-06-26 17:53:28.000000 cachelib-0.9.0/tests/
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      332 2022-03-12 20:20:34.000000 cachelib-0.9.0/tests/clear.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3042 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/common.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     2532 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/conftest.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      346 2022-03-12 20:20:34.000000 cachelib-0.9.0/tests/has.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1886 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/test_base_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     3726 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/test_file_system_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      968 2022-06-26 17:34:24.000000 cachelib-0.9.0/tests/test_interface_uniformity.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      490 2022-03-12 20:20:34.000000 cachelib-0.9.0/tests/test_memcached_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1026 2022-06-26 17:34:24.000000 cachelib-0.9.0/tests/test_redis_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1649 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/test_simple_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)     1063 2022-06-25 20:21:53.000000 cachelib-0.9.0/tests/test_uwsgi_cache.py
+-rw-r--r--   0 gfvante   (1000) gfvante   (1000)      803 2022-06-25 20:21:53.000000 cachelib-0.9.0/tox.ini
```

### Comparing `cachelib-0.8.0/CHANGES.rst` & `cachelib-0.9.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Version 0.9.0
+-------------
+
+Released 2022-06-26
+
+- Add separate internal read/write clients to ``RedisCache`` to improve compatibility with flask-caching. :pr:`159`
+- Fix bug where cache entries would expire immediately when ``RedisCache.add``
+  was called without timeout. :pr:`157`
+- Improve ``FileSystemCache.set`` compatibility with Windows systems. :pr:`158`
+
+
 Version 0.8.0
 -------------
 
 Released 2022-06-13
 
 - Remove deprecated ``RedisCache.load_object`` and ``RedisCache.dump_object``. :pr:`147`
```

### Comparing `cachelib-0.8.0/LICENSE.rst` & `cachelib-0.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/PKG-INFO` & `cachelib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachelib
-Version: 0.8.0
+Version: 0.9.0
 Summary: A collection of cache libraries in the same API interface.
 Home-page: https://github.com/pallets/cachelib/
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://cachelib.readthedocs.io/
```

### Comparing `cachelib-0.8.0/README.rst` & `cachelib-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/docs/Makefile` & `cachelib-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/docs/conf.py` & `cachelib-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/docs/make.bat` & `cachelib-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/requirements/dev.txt` & `cachelib-0.9.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/requirements/docs.txt` & `cachelib-0.9.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/requirements/tests.txt` & `cachelib-0.9.0/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/setup.cfg` & `cachelib-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib/base.py` & `cachelib-0.9.0/src/cachelib/base.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib/file.py` & `cachelib-0.9.0/src/cachelib/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import errno
 import logging
 import os
 import platform
+import stat
 import struct
 import tempfile
 import typing as _t
 from contextlib import contextmanager
 from hashlib import md5
 from pathlib import Path
 from time import sleep
@@ -41,34 +42,46 @@
     serializer = FileSystemSerializer()
 
     def __init__(
         self,
         cache_dir: str,
         threshold: int = 500,
         default_timeout: int = 300,
-        mode: int = 0o600,
+        mode: _t.Optional[int] = None,
         hash_method: _t.Any = md5,
     ):
         BaseCache.__init__(self, default_timeout)
         self._path = cache_dir
         self._threshold = threshold
         self._hash_method = hash_method
+
+        # Mode set by user takes precedence. If no mode has
+        # been given, we need to set the correct default based
+        # on user platform.
         self._mode = mode
+        if self._mode is None:
+            self._mode = self._get_compatible_platform_mode()
 
         try:
             os.makedirs(self._path)
         except OSError as ex:
             if ex.errno != errno.EEXIST:
                 raise
 
         # If there are many files and a zero threshold,
         # the list_dir can slow initialisation massively
         if self._threshold != 0:
             self._update_count(value=len(list(self._list_dir())))
 
+    def _get_compatible_platform_mode(self) -> int:
+        mode = 0o600  # nix systems
+        if platform.system() == "Windows":
+            mode = stat.S_IWRITE
+        return mode
+
     @property
     def _file_count(self) -> int:
         return self.get(self._fs_count_file) or 0
 
     def _update_count(
         self, delta: _t.Optional[int] = None, value: _t.Optional[int] = None
     ) -> None:
```

### Comparing `cachelib-0.8.0/src/cachelib/memcached.py` & `cachelib-0.9.0/src/cachelib/memcached.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib/redis.py` & `cachelib-0.9.0/src/cachelib/redis.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,14 +22,16 @@
                             specified on :meth:`~BaseCache.set`. A timeout of
                             0 indicates that the cache never expires.
     :param key_prefix: A prefix that should be added to all keys.
 
     Any additional keyword arguments will be passed to ``redis.Redis``.
     """
 
+    _read_client: _t.Any = None
+    _write_client: _t.Any = None
     serializer = RedisSerializer()
 
     def __init__(
         self,
         host: _t.Any = "localhost",
         port: int = 6379,
         password: _t.Optional[str] = None,
@@ -44,98 +46,103 @@
         if isinstance(host, str):
             try:
                 import redis
             except ImportError as err:
                 raise RuntimeError("no redis module found") from err
             if kwargs.get("decode_responses", None):
                 raise ValueError("decode_responses is not supported by RedisCache.")
-            self._client = redis.Redis(
+            self._write_client = self._read_client = redis.Redis(
                 host=host, port=port, password=password, db=db, **kwargs
             )
         else:
-            self._client = host
+            self._read_client = self._write_client = host
         self.key_prefix = key_prefix or ""
 
     def _normalize_timeout(self, timeout: _t.Optional[int]) -> int:
+        """Normalize timeout by setting it to default of 300 if
+        not defined (None) or -1 if explicitly set to zero.
+
+        :param timeout: timeout to normalize.
+        """
         timeout = BaseCache._normalize_timeout(self, timeout)
         if timeout == 0:
             timeout = -1
         return timeout
 
     def get(self, key: str) -> _t.Any:
-        return self.serializer.loads(self._client.get(self.key_prefix + key))
+        return self.serializer.loads(self._read_client.get(self.key_prefix + key))
 
     def get_many(self, *keys: str) -> _t.List[_t.Any]:
         if self.key_prefix:
             prefixed_keys = [self.key_prefix + key for key in keys]
         else:
             prefixed_keys = list(keys)
-        return [self.serializer.loads(x) for x in self._client.mget(prefixed_keys)]
+        return [self.serializer.loads(x) for x in self._read_client.mget(prefixed_keys)]
 
-    def set(
-        self, key: str, value: _t.Any, timeout: _t.Optional[int] = None
-    ) -> _t.Optional[bool]:
+    def set(self, key: str, value: _t.Any, timeout: _t.Optional[int] = None) -> _t.Any:
         timeout = self._normalize_timeout(timeout)
         dump = self.serializer.dumps(value)
         if timeout == -1:
-            result = self._client.set(name=self.key_prefix + key, value=dump)
+            result = self._write_client.set(name=self.key_prefix + key, value=dump)
         else:
-            result = self._client.setex(
+            result = self._write_client.setex(
                 name=self.key_prefix + key, value=dump, time=timeout
             )
         return result
 
-    def add(self, key: str, value: _t.Any, timeout: _t.Optional[int] = None) -> bool:
+    def add(self, key: str, value: _t.Any, timeout: _t.Optional[int] = None) -> _t.Any:
         timeout = self._normalize_timeout(timeout)
         dump = self.serializer.dumps(value)
-        return self._client.setnx(
-            name=self.key_prefix + key, value=dump
-        ) and self._client.expire(name=self.key_prefix + key, time=timeout)
+        created = self._write_client.setnx(name=self.key_prefix + key, value=dump)
+        # handle case where timeout is explicitly set to zero
+        if created and timeout != -1:
+            self._write_client.expire(name=self.key_prefix + key, time=timeout)
+        return created
 
     def set_many(
         self, mapping: _t.Dict[str, _t.Any], timeout: _t.Optional[int] = None
     ) -> _t.List[_t.Any]:
         timeout = self._normalize_timeout(timeout)
         # Use transaction=False to batch without calling redis MULTI
         # which is not supported by twemproxy
-        pipe = self._client.pipeline(transaction=False)
+        pipe = self._write_client.pipeline(transaction=False)
 
         for key, value in mapping.items():
             dump = self.serializer.dumps(value)
             if timeout == -1:
                 pipe.set(name=self.key_prefix + key, value=dump)
             else:
                 pipe.setex(name=self.key_prefix + key, value=dump, time=timeout)
         results = pipe.execute()
         return [k for k, was_set in zip(mapping.keys(), results) if was_set]
 
     def delete(self, key: str) -> bool:
-        return bool(self._client.delete(self.key_prefix + key))
+        return bool(self._write_client.delete(self.key_prefix + key))
 
     def delete_many(self, *keys: str) -> _t.List[_t.Any]:
         if not keys:
             return []
         if self.key_prefix:
             prefixed_keys = [self.key_prefix + key for key in keys]
         else:
             prefixed_keys = [k for k in keys]
-        self._client.delete(*prefixed_keys)
+        self._write_client.delete(*prefixed_keys)
         return [k for k in prefixed_keys if not self.has(k)]
 
     def has(self, key: str) -> bool:
-        return bool(self._client.exists(self.key_prefix + key))
+        return bool(self._read_client.exists(self.key_prefix + key))
 
     def clear(self) -> bool:
         status = 0
         if self.key_prefix:
-            keys = self._client.keys(self.key_prefix + "*")
+            keys = self._read_client.keys(self.key_prefix + "*")
             if keys:
-                status = self._client.delete(*keys)
+                status = self._write_client.delete(*keys)
         else:
-            status = self._client.flushdb()
+            status = self._write_client.flushdb()
         return bool(status)
 
-    def inc(self, key: str, delta: int = 1) -> _t.Optional[int]:
-        return self._client.incr(name=self.key_prefix + key, amount=delta)
+    def inc(self, key: str, delta: int = 1) -> _t.Any:
+        return self._write_client.incr(name=self.key_prefix + key, amount=delta)
 
-    def dec(self, key: str, delta: int = 1) -> _t.Optional[int]:
-        return self._client.incr(name=self.key_prefix + key, amount=-delta)
+    def dec(self, key: str, delta: int = 1) -> _t.Any:
+        return self._write_client.incr(name=self.key_prefix + key, amount=-delta)
```

### Comparing `cachelib-0.8.0/src/cachelib/serializers.py` & `cachelib-0.9.0/src/cachelib/serializers.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib/simple.py` & `cachelib-0.9.0/src/cachelib/simple.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib/uwsgi.py` & `cachelib-0.9.0/src/cachelib/uwsgi.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/src/cachelib.egg-info/PKG-INFO` & `cachelib-0.9.0/src/cachelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachelib
-Version: 0.8.0
+Version: 0.9.0
 Summary: A collection of cache libraries in the same API interface.
 Home-page: https://github.com/pallets/cachelib/
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://cachelib.readthedocs.io/
```

### Comparing `cachelib-0.8.0/src/cachelib.egg-info/SOURCES.txt` & `cachelib-0.9.0/src/cachelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/common.py` & `cachelib-0.9.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/conftest.py` & `cachelib-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/test_base_cache.py` & `cachelib-0.9.0/tests/test_base_cache.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/test_file_system_cache.py` & `cachelib-0.9.0/tests/test_file_system_cache.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/test_interface_uniformity.py` & `cachelib-0.9.0/tests/test_interface_uniformity.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @pytest.fixture(autouse=True)
 def create_cache_list(request, tmpdir):
     mc = MemcachedCache()
     mc._client.flush_all()
     rc = RedisCache(port=6360)
-    rc._client.flushdb()
+    rc._write_client.flushdb()
     request.cls.cache_list = [FileSystemCache(tmpdir), mc, rc, SimpleCache()]
 
 
 @pytest.mark.usefixtures("redis_server", "memcached_server")
 class TestInterfaceUniformity:
     def test_types_have_all_base_methods(self):
         public_api_methods = [
```

### Comparing `cachelib-0.8.0/tests/test_redis_cache.py` & `cachelib-0.9.0/tests/test_redis_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         super().__init__(*args, **kwargs)
 
 
 @pytest.fixture(autouse=True, params=[RedisCache, CustomCache])
 def cache_factory(request):
     def _factory(self, *args, **kwargs):
         rc = request.param(*args, port=6360, **kwargs)
-        rc._client.flushdb()
+        rc._write_client.flushdb()
         return rc
 
     request.cls.cache_factory = _factory
 
 
 @pytest.mark.usefixtures("redis_server")
 class TestRedisCache(CommonTests, ClearTests, HasTests):
```

### Comparing `cachelib-0.8.0/tests/test_simple_cache.py` & `cachelib-0.9.0/tests/test_simple_cache.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tests/test_uwsgi_cache.py` & `cachelib-0.9.0/tests/test_uwsgi_cache.py`

 * *Files identical despite different names*

### Comparing `cachelib-0.8.0/tox.ini` & `cachelib-0.9.0/tox.ini`

 * *Files identical despite different names*

