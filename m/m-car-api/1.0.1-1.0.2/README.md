# Comparing `tmp/m_car_api-1.0.1.tar.gz` & `tmp/m_car_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_car_api-1.0.1.tar", last modified: Sat Apr 13 09:24:25 2024, max compression
+gzip compressed data, was "m_car_api-1.0.2.tar", last modified: Sat Apr 13 10:20:41 2024, max compression
```

## Comparing `m_car_api-1.0.1.tar` & `m_car_api-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 09:24:25.514035 m_car_api-1.0.1/
--rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 09:24:25.513706 m_car_api-1.0.1/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-13 09:24:25.514107 m_car_api-1.0.1/setup.cfg
--rw-r--r--   0 cbrand     (501) staff       (20)     2204 2024-04-13 09:24:06.000000 m_car_api-1.0.1/setup.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 09:24:25.509130 m_car_api-1.0.1/src/
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 09:24:25.510454 m_car_api-1.0.1/src/m_car_api/
--rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-05 15:37:45.000000 m_car_api-1.0.1/src/m_car_api/__init__.py
--rw-r--r--   0 cbrand     (501) staff       (20)     5380 2024-04-05 15:46:22.000000 m_car_api-1.0.1/src/m_car_api/api.py
--rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.0.1/src/m_car_api/const.py
--rw-r--r--   0 cbrand     (501) staff       (20)     9716 2024-04-05 13:58:25.000000 m_car_api-1.0.1/src/m_car_api/objects.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 09:24:25.512092 m_car_api-1.0.1/src/m_car_api/test/
--rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.0.1/src/m_car_api/test/test_miles_api.py
--rw-r--r--   0 cbrand     (501) staff       (20)      661 2024-04-05 15:37:11.000000 m_car_api-1.0.1/src/m_car_api/test/test_objects.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 09:24:25.512394 m_car_api-1.0.1/src/m_car_api.egg-info/
--rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)      441 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/SOURCES.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/dependency_links.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/namespace_packages.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.0.1/src/m_car_api.egg-info/not-zip-safe
--rw-r--r--   0 cbrand     (501) staff       (20)      271 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/requires.txt
--rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-13 09:24:25.000000 m_car_api-1.0.1/src/m_car_api.egg-info/top_level.txt
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.517841 m_car_api-1.0.2/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 10:20:41.517547 m_car_api-1.0.2/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-13 10:20:41.517892 m_car_api-1.0.2/setup.cfg
+-rw-r--r--   0 cbrand     (501) staff       (20)     2204 2024-04-13 10:20:23.000000 m_car_api-1.0.2/setup.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.510144 m_car_api-1.0.2/src/
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.512600 m_car_api-1.0.2/src/m_car_api/
+-rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-05 15:37:45.000000 m_car_api-1.0.2/src/m_car_api/__init__.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     5378 2024-04-13 10:20:15.000000 m_car_api-1.0.2/src/m_car_api/api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.0.2/src/m_car_api/const.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     9716 2024-04-05 13:58:25.000000 m_car_api-1.0.2/src/m_car_api/objects.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.515805 m_car_api-1.0.2/src/m_car_api/test/
+-rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.0.2/src/m_car_api/test/test_miles_api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)      661 2024-04-05 15:37:11.000000 m_car_api-1.0.2/src/m_car_api/test/test_objects.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.516164 m_car_api-1.0.2/src/m_car_api.egg-info/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)      441 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.0.2/src/m_car_api.egg-info/not-zip-safe
+-rw-r--r--   0 cbrand     (501) staff       (20)      271 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/requires.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/top_level.txt
```

### Comparing `m_car_api-1.0.1/PKG-INFO` & `m_car_api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `m_car_api-1.0.1/setup.py` & `m_car_api-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def get_package_dir() -> Dict[str, str]:
     if not os.path.isdir("src"):
         return {}
     return {"": "src"}
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 requirements = ["requests", "pydantic>=2", "mujson", "pyproj"]
 test_requirements = [
     "black>=19.10b0",
     "coverage>=5.1,<7",
     "faker>=18,<19",
     "flake8>=5.0.4,<6",
     "mypy>=0.961",
```

### Comparing `m_car_api-1.0.1/src/m_car_api/api.py` & `m_car_api-1.0.2/src/m_car_api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def vehicles(
         self,
         lat: float,
         lon: float,
         latitude_delta: float,
         longitude_delta: float,
         query: VehicleQuery | None = None,
-    ) -> dict[str, Any]:
+    ) -> list[Vehicle]:
         return self.vehicles_return(
             lat=lat,
             lon=lon,
             latitude_delta=latitude_delta,
             longitude_delta=longitude_delta,
             query=query,
         ).vehicles
@@ -145,15 +145,15 @@
             latitude_delta=lat_delta,
             longitude_delta=lon_delta,
             query=query,
         )
 
     def vehicles_meters_around_location(
         self, lat: float, lon: float, meters: float, query: VehicleQuery | None = None
-    ) -> dict[str, Any]:
+    ) -> list[Vehicle]:
         return self.vehicles_return_meters_around_location(
             lat=lat,
             lon=lon,
             meters=meters,
             query=query,
         ).vehicles
```

### Comparing `m_car_api-1.0.1/src/m_car_api/const.py` & `m_car_api-1.0.2/src/m_car_api/const.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.1/src/m_car_api/objects.py` & `m_car_api-1.0.2/src/m_car_api/objects.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.1/src/m_car_api/test/test_miles_api.py` & `m_car_api-1.0.2/src/m_car_api/test/test_miles_api.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.1/src/m_car_api/test/test_objects.py` & `m_car_api-1.0.2/src/m_car_api/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.1/src/m_car_api.egg-info/PKG-INFO` & `m_car_api-1.0.2/src/m_car_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

