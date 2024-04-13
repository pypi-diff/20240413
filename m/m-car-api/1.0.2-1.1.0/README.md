# Comparing `tmp/m_car_api-1.0.2.tar.gz` & `tmp/m_car_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_car_api-1.0.2.tar", last modified: Sat Apr 13 10:20:41 2024, max compression
+gzip compressed data, was "m_car_api-1.1.0.tar", last modified: Sat Apr 13 12:39:34 2024, max compression
```

## Comparing `m_car_api-1.0.2.tar` & `m_car_api-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.517841 m_car_api-1.0.2/
--rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 10:20:41.517547 m_car_api-1.0.2/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-13 10:20:41.517892 m_car_api-1.0.2/setup.cfg
--rw-r--r--   0 cbrand     (501) staff       (20)     2204 2024-04-13 10:20:23.000000 m_car_api-1.0.2/setup.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.510144 m_car_api-1.0.2/src/
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.512600 m_car_api-1.0.2/src/m_car_api/
--rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-05 15:37:45.000000 m_car_api-1.0.2/src/m_car_api/__init__.py
--rw-r--r--   0 cbrand     (501) staff       (20)     5378 2024-04-13 10:20:15.000000 m_car_api-1.0.2/src/m_car_api/api.py
--rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.0.2/src/m_car_api/const.py
--rw-r--r--   0 cbrand     (501) staff       (20)     9716 2024-04-05 13:58:25.000000 m_car_api-1.0.2/src/m_car_api/objects.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.515805 m_car_api-1.0.2/src/m_car_api/test/
--rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.0.2/src/m_car_api/test/test_miles_api.py
--rw-r--r--   0 cbrand     (501) staff       (20)      661 2024-04-05 15:37:11.000000 m_car_api-1.0.2/src/m_car_api/test/test_objects.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 10:20:41.516164 m_car_api-1.0.2/src/m_car_api.egg-info/
--rw-r--r--   0 cbrand     (501) staff       (20)     1533 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)      441 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/SOURCES.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/dependency_links.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/namespace_packages.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.0.2/src/m_car_api.egg-info/not-zip-safe
--rw-r--r--   0 cbrand     (501) staff       (20)      271 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/requires.txt
--rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-13 10:20:41.000000 m_car_api-1.0.2/src/m_car_api.egg-info/top_level.txt
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 12:39:34.636599 m_car_api-1.1.0/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1746 2024-04-13 12:39:34.636307 m_car_api-1.1.0/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-13 12:39:34.636651 m_car_api-1.1.0/setup.cfg
+-rw-r--r--   0 cbrand     (501) staff       (20)     2369 2024-04-13 12:38:41.000000 m_car_api-1.1.0/setup.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 12:39:34.631018 m_car_api-1.1.0/src/
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 12:39:34.632631 m_car_api-1.1.0/src/m_car_api/
+-rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-05 15:37:45.000000 m_car_api-1.1.0/src/m_car_api/__init__.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     5371 2024-04-13 12:34:39.000000 m_car_api-1.1.0/src/m_car_api/api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.1.0/src/m_car_api/const.py
+-rw-r--r--   0 cbrand     (501) staff       (20)      467 2024-04-13 12:37:15.000000 m_car_api-1.1.0/src/m_car_api/objects.py
+-rw-r--r--   0 cbrand     (501) staff       (20)    11122 2024-04-13 12:34:26.000000 m_car_api-1.1.0/src/m_car_api/objects_pydantic_1.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     9884 2024-04-13 12:36:48.000000 m_car_api-1.1.0/src/m_car_api/objects_pydantic_2.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 12:39:34.634384 m_car_api-1.1.0/src/m_car_api/test/
+-rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.1.0/src/m_car_api/test/test_miles_api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)      661 2024-04-05 15:37:11.000000 m_car_api-1.1.0/src/m_car_api/test/test_objects.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 12:39:34.634705 m_car_api-1.1.0/src/m_car_api.egg-info/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1746 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)      513 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.1.0/src/m_car_api.egg-info/not-zip-safe
+-rw-r--r--   0 cbrand     (501) staff       (20)      344 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/requires.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-13 12:39:34.000000 m_car_api-1.1.0/src/m_car_api.egg-info/top_level.txt
```

### Comparing `m_car_api-1.0.2/PKG-INFO` & `m_car_api-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.0.2
+Version: 1.1.0
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,24 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: requests
-Requires-Dist: pydantic>=2
 Requires-Dist: mujson
 Requires-Dist: pyproj
+Requires-Dist: pydantic
 Provides-Extra: test
 Requires-Dist: black>=19.10b0; extra == "test"
 Requires-Dist: coverage<7,>=5.1; extra == "test"
 Requires-Dist: faker<19,>=18; extra == "test"
 Requires-Dist: flake8<6,>=5.0.4; extra == "test"
 Requires-Dist: mypy>=0.961; extra == "test"
 Requires-Dist: pre-commit<4,>=3; extra == "test"
 Requires-Dist: pytest-cases<4,>=3.1.1; extra == "test"
 Requires-Dist: pytest-html; extra == "test"
 Requires-Dist: pytest<8,>=7; extra == "test"
 Requires-Dist: pytest-mock<4,>=3.5.1; extra == "test"
 Requires-Dist: python-dotenv<2,>=1; extra == "test"
 Requires-Dist: python-semantic-release<9,>=8; extra == "test"
 Requires-Dist: twine<4,>=3.1.1; extra == "test"
+Provides-Extra: pydantic-1
+Requires-Dist: pydantic<2,>=1; extra == "pydantic-1"
+Requires-Dist: pydantic_computed; extra == "pydantic-1"
+Provides-Extra: pydantic-2
+Requires-Dist: pydantic<3,>=2; extra == "pydantic-2"
```

### Comparing `m_car_api-1.0.2/setup.py` & `m_car_api-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 
 def get_package_dir() -> Dict[str, str]:
     if not os.path.isdir("src"):
         return {}
     return {"": "src"}
 
 
-__version__ = "1.0.2"
-requirements = ["requests", "pydantic>=2", "mujson", "pyproj"]
+__version__ = "1.1.0"
+requirements = ["requests", "mujson", "pyproj", "pydantic"]
+pydantic_1 = ["pydantic>=1,<2", "pydantic_computed"]
+pydantic_2 = ["pydantic>=2,<3"]
 test_requirements = [
     "black>=19.10b0",
     "coverage>=5.1,<7",
     "faker>=18,<19",
     "flake8>=5.0.4,<6",
     "mypy>=0.961",
     "pre-commit>=3,<4",
@@ -68,11 +70,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    extras_require={"test": test_requirements},
+    extras_require={
+        "test": test_requirements,
+        "pydantic_1": pydantic_1,
+        "pydantic_2": pydantic_2,
+    },
     project_urls={"GitHub": "https://github.com/cbrand/m_car_api"},
     namespace_packages=list_namespace_packages(),
 )
```

### Comparing `m_car_api-1.0.2/src/m_car_api/api.py` & `m_car_api-1.1.0/src/m_car_api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
-from typing import Any
+import mujson
 import requests
-from base64 import b64decode
 from urllib.parse import urljoin
 from pyproj import Geod
 
 from m_car_api.const import U_HEL_URL_PATH, V_URL_PATH, DEFAULT_ROOT_URL
 from m_car_api.objects import (
     DeviceInfo,
     Vehicle,
     VehicleQuery,
     VehicleReturn,
-    APIReturn,
+    parse_vehicles_payload,
 )
 
 geod = Geod(ellps="WGS84")
 
 
 class SubAPI:
     def __init__(self, mapi: MApi) -> None:
@@ -61,15 +60,16 @@
         )
         params["deviceKey"] = self.device_key
         response = requests.get(vehicles_url, params=params)
         response.raise_for_status()
         return response.text
 
     def vehicles_return(self) -> VehicleReturn:
-        result = APIReturn[VehicleReturn].model_validate_json(self.raw_json_response())
+        payload = mujson.loads(self.raw_json_response())
+        result = parse_vehicles_payload(payload)
         if result.result != "OK":
             raise ValueError(result.message)
         return result.data
 
 
 class MApi:
     def __init__(self, device_key: str, root_url: str = DEFAULT_ROOT_URL) -> None:
```

### Comparing `m_car_api-1.0.2/src/m_car_api/const.py` & `m_car_api-1.1.0/src/m_car_api/const.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.2/src/m_car_api/objects.py` & `m_car_api-1.1.0/src/m_car_api/objects_pydantic_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
 import mujson
 from datetime import datetime
 from typing import Any, Generic, Literal, NamedTuple, TypeVar
 from pydantic import BaseModel, Field, computed_field
 
 
+def parse_vehicles_payload(payload: Any) -> APIReturn[VehicleReturn]:
+    return APIReturn[VehicleReturn].model_validate(payload)
+
+
 class DeviceInfo(NamedTuple):
     owner_name: str = "unknown"
     device_info1: str = "Linux"
     device_info2: str = "amd64"
     os_info1: str = "Linux"
     os_info2: str = "6.8.2-generic"
     app_version: str = "4.31+(210440)"
```

### Comparing `m_car_api-1.0.2/src/m_car_api/test/test_miles_api.py` & `m_car_api-1.1.0/src/m_car_api/test/test_miles_api.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.2/src/m_car_api/test/test_objects.py` & `m_car_api-1.1.0/src/m_car_api/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.0.2/src/m_car_api.egg-info/PKG-INFO` & `m_car_api-1.1.0/src/m_car_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.0.2
+Version: 1.1.0
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,24 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: requests
-Requires-Dist: pydantic>=2
 Requires-Dist: mujson
 Requires-Dist: pyproj
+Requires-Dist: pydantic
 Provides-Extra: test
 Requires-Dist: black>=19.10b0; extra == "test"
 Requires-Dist: coverage<7,>=5.1; extra == "test"
 Requires-Dist: faker<19,>=18; extra == "test"
 Requires-Dist: flake8<6,>=5.0.4; extra == "test"
 Requires-Dist: mypy>=0.961; extra == "test"
 Requires-Dist: pre-commit<4,>=3; extra == "test"
 Requires-Dist: pytest-cases<4,>=3.1.1; extra == "test"
 Requires-Dist: pytest-html; extra == "test"
 Requires-Dist: pytest<8,>=7; extra == "test"
 Requires-Dist: pytest-mock<4,>=3.5.1; extra == "test"
 Requires-Dist: python-dotenv<2,>=1; extra == "test"
 Requires-Dist: python-semantic-release<9,>=8; extra == "test"
 Requires-Dist: twine<4,>=3.1.1; extra == "test"
+Provides-Extra: pydantic-1
+Requires-Dist: pydantic<2,>=1; extra == "pydantic-1"
+Requires-Dist: pydantic_computed; extra == "pydantic-1"
+Provides-Extra: pydantic-2
+Requires-Dist: pydantic<3,>=2; extra == "pydantic-2"
```

