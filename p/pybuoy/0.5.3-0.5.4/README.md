# Comparing `tmp/pybuoy-0.5.3.tar.gz` & `tmp/pybuoy-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuoy-0.5.3.tar", max compression
+gzip compressed data, was "pybuoy-0.5.4.tar", max compression
```

## Comparing `pybuoy-0.5.3.tar` & `pybuoy-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-11-19 16:30:07.255293 pybuoy-0.5.3/LICENSE
--rw-r--r--   0        0        0     1906 2023-11-19 16:30:07.255451 pybuoy-0.5.3/README.rst
--rw-r--r--   0        0        0      102 2023-11-19 16:30:07.258800 pybuoy-0.5.3/pybuoy/__init__.py
--rw-r--r--   0        0        0      508 2023-11-19 16:30:07.258929 pybuoy-0.5.3/pybuoy/api/base.py
--rw-r--r--   0        0        0     4258 2023-11-19 16:30:07.259046 pybuoy-0.5.3/pybuoy/api/forecasts.py
--rw-r--r--   0        0        0     2067 2023-11-19 16:30:07.259131 pybuoy-0.5.3/pybuoy/api/realtime.py
--rw-r--r--   0        0        0      315 2023-11-19 16:30:07.259219 pybuoy-0.5.3/pybuoy/api/stations.py
--rw-r--r--   0        0        0     1031 2023-11-19 16:30:07.259309 pybuoy-0.5.3/pybuoy/buoy.py
--rw-r--r--   0        0        0      645 2023-11-19 16:30:07.259391 pybuoy-0.5.3/pybuoy/const.py
--rw-r--r--   0        0        0      380 2023-11-19 16:30:07.259478 pybuoy-0.5.3/pybuoy/endpoints.py
--rw-r--r--   0        0        0      473 2023-11-19 16:30:07.259553 pybuoy-0.5.3/pybuoy/exceptions.py
--rw-r--r--   0        0        0    20984 2023-11-19 16:30:07.259719 pybuoy-0.5.3/pybuoy/mixins/noaa.xsl
--rw-r--r--   0        0        0     5646 2023-11-19 16:30:07.259884 pybuoy-0.5.3/pybuoy/mixins/parser.py
--rw-r--r--   0        0        0      468 2023-11-19 16:30:07.260027 pybuoy-0.5.3/pybuoy/observation/__init__.py
--rw-r--r--   0        0        0     1745 2023-11-19 16:30:07.260131 pybuoy-0.5.3/pybuoy/observation/meta.py
--rw-r--r--   0        0        0     9314 2023-11-19 16:30:07.260296 pybuoy-0.5.3/pybuoy/observation/observation.py
--rw-r--r--   0        0        0     2205 2023-11-19 16:30:07.260423 pybuoy-0.5.3/pybuoy/observation/observation_datum.py
--rw-r--r--   0        0        0     2362 2023-11-19 16:30:07.260574 pybuoy-0.5.3/pybuoy/observation/observations.py
--rw-r--r--   0        0        0        0 2023-11-19 16:30:07.260625 pybuoy-0.5.3/pybuoy/py.typed
--rw-r--r--   0        0        0     3937 2023-11-19 16:30:07.260749 pybuoy-0.5.3/pybuoy/unit_mappings.py
--rw-r--r--   0        0        0     1554 2024-01-16 01:21:48.293424 pybuoy-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 pybuoy-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-19 16:30:07.255293 pybuoy-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1906 2023-11-19 16:30:07.255451 pybuoy-0.5.4/README.rst
+-rw-r--r--   0        0        0      102 2023-11-19 16:30:07.258800 pybuoy-0.5.4/pybuoy/__init__.py
+-rw-r--r--   0        0        0      508 2023-11-19 16:30:07.258929 pybuoy-0.5.4/pybuoy/api/base.py
+-rw-r--r--   0        0        0     4258 2023-11-19 16:30:07.259046 pybuoy-0.5.4/pybuoy/api/forecasts.py
+-rw-r--r--   0        0        0     2051 2024-03-31 16:47:54.227931 pybuoy-0.5.4/pybuoy/api/realtime.py
+-rw-r--r--   0        0        0      315 2023-11-19 16:30:07.259219 pybuoy-0.5.4/pybuoy/api/stations.py
+-rw-r--r--   0        0        0     1031 2023-11-19 16:30:07.259309 pybuoy-0.5.4/pybuoy/buoy.py
+-rw-r--r--   0        0        0      646 2024-04-13 05:35:44.765848 pybuoy-0.5.4/pybuoy/const.py
+-rw-r--r--   0        0        0      380 2023-11-19 16:30:07.259478 pybuoy-0.5.4/pybuoy/endpoints.py
+-rw-r--r--   0        0        0      462 2024-03-31 16:47:54.228321 pybuoy-0.5.4/pybuoy/exceptions.py
+-rw-r--r--   0        0        0    20984 2023-11-19 16:30:07.259719 pybuoy-0.5.4/pybuoy/mixins/noaa.xsl
+-rw-r--r--   0        0        0     5647 2024-03-31 16:47:54.228514 pybuoy-0.5.4/pybuoy/mixins/parser.py
+-rw-r--r--   0        0        0      468 2023-11-19 16:30:07.260027 pybuoy-0.5.4/pybuoy/observation/__init__.py
+-rw-r--r--   0        0        0     1745 2023-11-19 16:30:07.260131 pybuoy-0.5.4/pybuoy/observation/meta.py
+-rw-r--r--   0        0        0     9314 2023-11-19 16:30:07.260296 pybuoy-0.5.4/pybuoy/observation/observation.py
+-rw-r--r--   0        0        0     2205 2023-11-19 16:30:07.260423 pybuoy-0.5.4/pybuoy/observation/observation_datum.py
+-rw-r--r--   0        0        0     2350 2024-03-31 16:47:54.228698 pybuoy-0.5.4/pybuoy/observation/observations.py
+-rw-r--r--   0        0        0        0 2023-11-19 16:30:07.260625 pybuoy-0.5.4/pybuoy/py.typed
+-rw-r--r--   0        0        0     3934 2024-03-31 16:47:54.228896 pybuoy-0.5.4/pybuoy/unit_mappings.py
+-rw-r--r--   0        0        0     1416 2024-04-13 05:35:35.720753 pybuoy-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 pybuoy-0.5.4/PKG-INFO
```

### Comparing `pybuoy-0.5.3/LICENSE` & `pybuoy-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/README.rst` & `pybuoy-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/api/forecasts.py` & `pybuoy-0.5.4/pybuoy/api/forecasts.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/api/realtime.py` & `pybuoy-0.5.4/pybuoy/api/realtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 
 class Realtime(ApiBase):
     @overload
     def get(
         self,
         station_id: str,
         dataset: Literal["spec"],
-    ) -> WaveSummaryObservations:
-        ...
+    ) -> WaveSummaryObservations: ...
 
     @overload
     def get(
         self, station_id: str, dataset: Literal["txt"] = "txt"
-    ) -> MeteorologicalObservations:
-        ...
+    ) -> MeteorologicalObservations: ...
 
     # TODO: consider mapping str literal to dataset
     def get(
         self,
         station_id: str,
         dataset: RealtimeDatasetsValues = RealtimeDatasets.txt.value,
     ):
```

### Comparing `pybuoy-0.5.3/pybuoy/buoy.py` & `pybuoy-0.5.4/pybuoy/buoy.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/const.py` & `pybuoy-0.5.4/pybuoy/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pybuoy constants."""
+
 from enum import Enum
 from typing import Literal
 
 from pybuoy.endpoints import API_PATH as API_PATH  # noqa: F401
 
 
 class Endpoints(Enum):
@@ -31,8 +32,8 @@
     "swdir",
     "swdir2",
     "swr1",
     "swr2",
     "txt",
 ]
 
-__version__ = "0.5.2"
+__version__ = "0.5.4"
```

### Comparing `pybuoy-0.5.3/pybuoy/mixins/noaa.xsl` & `pybuoy-0.5.4/pybuoy/mixins/noaa.xsl`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/mixins/parser.py` & `pybuoy-0.5.4/pybuoy/mixins/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provide the ParserMixin class."""
+
 from collections import defaultdict
 from datetime import datetime as dt
 from os.path import dirname, join
 from typing import Any
 from xml.etree.ElementTree import Element, fromstring
 
 import lxml.etree as ET  # type: ignore
```

### Comparing `pybuoy-0.5.3/pybuoy/observation/meta.py` & `pybuoy-0.5.4/pybuoy/observation/meta.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/observation/observation.py` & `pybuoy-0.5.4/pybuoy/observation/observation.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/observation/observation_datum.py` & `pybuoy-0.5.4/pybuoy/observation/observation_datum.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.3/pybuoy/observation/observations.py` & `pybuoy-0.5.4/pybuoy/observation/observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,14 @@
         # Insert the '...' inbetween the 3rd and 4th item
         values.insert(3, "...")
         # Convert the list to a string joined by commas
         array_as_string = ", ".join(values)
         return f"Observations([{array_as_string}])"
 
 
-class MeteorologicalObservations(BaseObservations[MeteorologicalObservation]):
-    ...
+class MeteorologicalObservations(BaseObservations[MeteorologicalObservation]): ...
 
 
-class WaveSummaryObservations(BaseObservations[WaveSummaryObservation]):
-    ...
+class WaveSummaryObservations(BaseObservations[WaveSummaryObservation]): ...
 
 
-class ForecastObservations(BaseObservations[ForecastObservation]):
-    ...
+class ForecastObservations(BaseObservations[ForecastObservation]): ...
```

### Comparing `pybuoy-0.5.3/pybuoy/unit_mappings.py` & `pybuoy-0.5.4/pybuoy/unit_mappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Mapping key to unit for Observation."""
+
 # https://www.ndbc.noaa.gov/measdes.shtml
 from enum import Enum
 from typing import TypedDict
 
 NO_NUMERIC_VALUE = "MM"
 NO_TEXT_VALUE = "N/A"
 
 
-class BaseKey(Enum):
-    ...
+class BaseKey(Enum): ...
 
 
 class ForecastKey(BaseKey):
     wind_direction = "Wind Direction"
     wave_height = "Wave Height"
     wind_speed = "Wind Speed"
     wind_speed_gust = "Wind Speed Gust"
```

### Comparing `pybuoy-0.5.3/pyproject.toml` & `pybuoy-0.5.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybuoy"
-version = "0.5.3"
+version = "0.5.4"
 authors = ["Kyle J. Burda <kylejbdev@gmail.com>"]
 classifiers=[
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.11",
 ]
 description = "Python wrapper for NOAA and NDBC REST web services."
 documentation = "https://pybuoy.readthedocs.io"
@@ -14,53 +14,44 @@
 readme = "README.rst"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/clairBuoyant/pybuoy"
 "Bug Tracker" = "https://github.com/clairBuoyant/pybuoy/issues"
 
 [tool.poetry.dependencies]
-lxml = "^5.1.0"
+lxml = "^5.2.1"
 python = "^3.11"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.1"
-flake8 = "^7.0.0"
-isort = { version = "^5.13.2", extras = ["pyproject"]}
-mypy = "^1.8.0"
-pre-commit = "^3.6.0"
-pytest = "^7.4.4"
+ruff = "^0.3.4"
+mypy = "^1.9.0"
+pre-commit = "^3.7.0"
+pytest = "^8.1.1"
 types-requests = "^2.31.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.9.10"
 Sphinx = "^7.2.6"
 
-[tool.black]
+[tool.ruff]
+exclude = [
+  ".git",
+  ".github",
+  ".mypy_cache",
+  ".pytest_cache",
+  ".venv",
+  "dist",
+  "htmlcov",
+]
 line-length = 88
-target_version = ['py310']
-exclude = '''
-(
-  /(
-    \.git
-    | \.github
-    | \.mypy_cache
-    | \.pytest_cache
-    | dist
-    | htmlcov
-    | .venv
-  )/
-)
-'''
-
-[tool.isort]
-profile="black"
+target-version = "py311"
 
 [tool.mypy]
 namespace_packages = true
 explicit_package_bases = true
 exclude = '''
 (
   /(
@@ -69,15 +60,15 @@
     | docs/source/conf.py
     | .venv
   )/
 )
 '''
 
 [tool.pytest.ini_options]
-minversion = "7.0"
+minversion = "8.0"
 testpaths = [
-    "tests",
+  "tests",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pybuoy-0.5.3/PKG-INFO` & `pybuoy-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pybuoy
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python wrapper for NOAA and NDBC REST web services.
 License: GPL-3.0-or-later
 Keywords: NDBC,NOAA,api,buoy,weather,wrapper
 Author: Kyle J. Burda
 Author-email: kylejbdev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/clairBuoyant/pybuoy/issues
 Project-URL: Documentation, https://pybuoy.readthedocs.io
 Project-URL: Source Code, https://github.com/clairBuoyant/pybuoy
 Description-Content-Type: text/x-rst
 
 =====================================
```

