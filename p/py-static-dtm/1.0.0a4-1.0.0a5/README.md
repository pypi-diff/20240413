# Comparing `tmp/py_static_dtm-1.0.0a4.tar.gz` & `tmp/py_static_dtm-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_static_dtm-1.0.0a4.tar", last modified: Sat Apr 13 18:38:02 2024, max compression
+gzip compressed data, was "py_static_dtm-1.0.0a5.tar", last modified: Sat Apr 13 18:41:35 2024, max compression
```

## Comparing `py_static_dtm-1.0.0a4.tar` & `py_static_dtm-1.0.0a5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.842959 py_static_dtm-1.0.0a4/.github/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/.github/workflows/
--rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.github/workflows/lint.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.github/workflows/test.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.gitignore
--rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a4/.pre-commit-config.yaml
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/.vscode/
--rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.vscode/settings.json
--rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a4/README.md
--rwxrwxr-x   0 ben       (1000) ben       (1000)      374 2024-04-13 18:37:19.000000 py_static_dtm-1.0.0a4/build_and_publish.sh
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/docs/
--rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/docs/Haifa Sea With Tests Points.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      986 2024-04-13 17:46:30.000000 py_static_dtm-1.0.0a4/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/setup.cfg
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/src/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/src/py_static_dtm/
--rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/kml_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1161 2024-04-13 16:49:18.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/polygon_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)        6 2024-04-13 17:46:11.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/py.typed
--rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/static_dtm.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      714 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/top_level.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/tests/
--rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/HaifaSea.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a4/tests/conftest.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/haifa_points.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      370 2024-04-13 16:50:43.000000 py_static_dtm-1.0.0a4/tests/test_example_simple_usage.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/test_fastkml_poc.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a4/tests/test_stress_static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.420338 py_static_dtm-1.0.0a5/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.412338 py_static_dtm-1.0.0a5/.github/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.416338 py_static_dtm-1.0.0a5/.github/workflows/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/.github/workflows/lint.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/.github/workflows/test.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/.gitignore
+-rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a5/.pre-commit-config.yaml
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.416338 py_static_dtm-1.0.0a5/.vscode/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/.vscode/settings.json
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:41:35.420338 py_static_dtm-1.0.0a5/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a5/README.md
+-rwxrwxr-x   0 ben       (1000) ben       (1000)      375 2024-04-13 18:40:08.000000 py_static_dtm-1.0.0a5/build_and_publish.sh
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.416338 py_static_dtm-1.0.0a5/docs/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/docs/Haifa Sea With Tests Points.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      986 2024-04-13 17:46:30.000000 py_static_dtm-1.0.0a5/pyproject.toml
+-rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 18:41:35.420338 py_static_dtm-1.0.0a5/setup.cfg
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.412338 py_static_dtm-1.0.0a5/src/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.416338 py_static_dtm-1.0.0a5/src/py_static_dtm/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/src/py_static_dtm/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/src/py_static_dtm/kml_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1181 2024-04-13 18:40:09.000000 py_static_dtm-1.0.0a5/src/py_static_dtm/polygon_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)        7 2024-04-13 18:40:08.000000 py_static_dtm-1.0.0a5/src/py_static_dtm/py.typed
+-rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a5/src/py_static_dtm/static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.420338 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:41:35.000000 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      714 2024-04-13 18:41:35.000000 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 18:41:35.000000 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 18:41:35.000000 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 18:41:35.000000 py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/top_level.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:41:35.420338 py_static_dtm-1.0.0a5/tests/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/tests/HaifaSea.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a5/tests/conftest.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/tests/haifa_points.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      503 2024-04-13 18:40:09.000000 py_static_dtm-1.0.0a5/tests/test_example_simple_usage.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a5/tests/test_fastkml_poc.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a5/tests/test_stress_static_dtm.py
```

### Comparing `py_static_dtm-1.0.0a4/.gitignore` & `py_static_dtm-1.0.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/.pre-commit-config.yaml` & `py_static_dtm-1.0.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/LICENSE` & `py_static_dtm-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/PKG-INFO` & `py_static_dtm-1.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a4/README.md` & `py_static_dtm-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/docs/Haifa Sea With Tests Points.kml` & `py_static_dtm-1.0.0a5/docs/Haifa Sea With Tests Points.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/pyproject.toml` & `py_static_dtm-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/src/py_static_dtm/kml_utils.py` & `py_static_dtm-1.0.0a5/src/py_static_dtm/kml_utils.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/src/py_static_dtm/polygon_utils.py` & `py_static_dtm-1.0.0a5/src/py_static_dtm/polygon_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 
 
 class CoordinateSystem(enum.Enum):
     GCS = enum.auto
     UTM = enum.auto
 
 
-def gcs_to_utm(lon_lat_alt: Tuple[float, float, float]) -> Tuple[float, float, float]:
+def gcs_to_utm(
+        lon_lat_alt: Tuple[float, float, float]) -> Tuple[float, float, float]:
     ISRAEL_ZONE = 36
     longitude, latitude, altitude = lon_lat_alt
     _proj = Proj(proj="utm", zone=ISRAEL_ZONE, ellps="WGS84")
     x, y = _proj(longitude, latitude)
     return x, y, altitude
 
 
-def gcs_polygon_to_utm_polygon(gcs_polygon: shapely.Polygon) -> shapely.Polygon:
+def gcs_polygon_to_utm_polygon(
+        gcs_polygon: shapely.Polygon) -> shapely.Polygon:
     utm_coordinates = tuple(gcs_to_utm(c) for c in gcs_polygon.exterior.coords)
     utm_polygon = shapely.Polygon(utm_coordinates)
     return utm_polygon
 
 
 def convert_polygon_to_utm(
-    polygon: shapely.Polygon, coordinate_system: CoordinateSystem
-) -> shapely.Polygon:
+        polygon: shapely.Polygon,
+        coordinate_system: CoordinateSystem) -> shapely.Polygon:
     if coordinate_system == CoordinateSystem.GCS:
         return gcs_polygon_to_utm_polygon(polygon)
     elif coordinate_system == CoordinateSystem.UTM:
         return polygon
     else:
         raise NotImplementedError(
             f"Polygons using {coordinate_system} coordinate system "
-            "is not supported yet."
-        )
+            "is not supported yet.")
```

### Comparing `py_static_dtm-1.0.0a4/src/py_static_dtm/static_dtm.py` & `py_static_dtm-1.0.0a5/src/py_static_dtm/static_dtm.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/PKG-INFO` & `py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/SOURCES.txt` & `py_static_dtm-1.0.0a5/src/py_static_dtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/tests/HaifaSea.kml` & `py_static_dtm-1.0.0a5/tests/HaifaSea.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/tests/conftest.py` & `py_static_dtm-1.0.0a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/tests/haifa_points.py` & `py_static_dtm-1.0.0a5/tests/haifa_points.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/tests/test_fastkml_poc.py` & `py_static_dtm-1.0.0a5/tests/test_fastkml_poc.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a4/tests/test_stress_static_dtm.py` & `py_static_dtm-1.0.0a5/tests/test_stress_static_dtm.py`

 * *Files identical despite different names*

