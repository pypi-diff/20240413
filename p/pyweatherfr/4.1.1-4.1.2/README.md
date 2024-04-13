# Comparing `tmp/pyweatherfr-4.1.1.tar.gz` & `tmp/pyweatherfr-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.1.1.tar", last modified: Sat Apr 13 13:50:21 2024, max compression
+gzip compressed data, was "pyweatherfr-4.1.2.tar", last modified: Sat Apr 13 13:58:55 2024, max compression
```

## Comparing `pyweatherfr-4.1.1.tar` & `pyweatherfr-4.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.808243 pyweatherfr-4.1.1/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36527 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.808243 pyweatherfr-4.1.1/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:51.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36627 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:27.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/setup.py
```

### Comparing `pyweatherfr-4.1.1/LICENSE.txt` & `pyweatherfr-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.1/PKG-INFO` & `pyweatherfr-4.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.1
+Version: 4.1.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.1/README.md` & `pyweatherfr-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.1/pyweatherfr/args.py` & `pyweatherfr-4.1.2/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.1/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.1.2/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -788,18 +788,18 @@
 
 
 
 def resume(latitude, longitude, tz):
     retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
-    date_debut = (datetime.datetime.now() + datetime.timedelta(days=-1*compute_args().past)).strftime("%Y-%m-%d")
-    date_fin = (datetime.datetime.now() + datetime.timedelta(days=3)).strftime("%Y-%m-%d")
+    date_debut = (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=-1*compute_args().past)).strftime("%Y-%m-%d")
+    date_fin = (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=3)).strftime("%Y-%m-%d")
     if compute_args().past!=0:
-        date_fin = (datetime.datetime.now() + datetime.timedelta(days=-1)).strftime("%Y-%m-%d")    
+        date_fin = (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=-1)).strftime("%Y-%m-%d")    
     params = {
         "timezone": tz,
         "start_date": date_debut,
 	    "end_date": date_fin,
         "latitude": latitude,
         "longitude": longitude,
         "daily": [
@@ -874,19 +874,19 @@
             "weather_code",
             "snowfall",
             "relative_humidity_2m",
             "sunshine_duration",
             "cloud_cover",
             "is_day"
         ],
-        "start_date": (datetime.datetime.now() + datetime.timedelta(days=day)).strftime(
+        "start_date": (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=day)).strftime(
             "%Y-%m-%d"
         ),
         "end_date": (
-            datetime.datetime.now() + datetime.timedelta(days=day + 1)
+            datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=day + 1)
         ).strftime("%Y-%m-%d"),
     }
     print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
     response = responses[0]
     hourly = response.Hourly()
     hourly_temperature_2m = hourly.Variables(0).ValuesAsNumpy()
```

### Comparing `pyweatherfr-4.1.1/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.1.2/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.1
+Version: 4.1.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.1/setup.py` & `pyweatherfr-4.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.1.1",
+    version="4.1.2",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

