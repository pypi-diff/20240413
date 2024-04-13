# Comparing `tmp/galapy_core-0.2.0.tar.gz` & `tmp/galapy_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galapy_core-0.2.0.tar", max compression
+gzip compressed data, was "galapy_core-0.2.1.tar", max compression
```

## Comparing `galapy_core-0.2.0.tar` & `galapy_core-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-10 02:38:11.989631 galapy_core-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-10 02:40:16.917509 galapy_core-0.2.0/galapy_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:40:16.924086 galapy_core-0.2.0/galapy_core/accounts.py
--rw-r--r--   0        0        0    19258 2024-04-11 18:47:25.035325 galapy_core-0.2.0/galapy_core/assets.py
--rw-r--r--   0        0        0      971 2024-04-11 19:53:15.372470 galapy_core-0.2.0/galapy_core/core.py
--rw-r--r--   0        0        0      160 2024-04-11 18:34:19.554350 galapy_core-0.2.0/galapy_core/generators/README.md
--rw-r--r--   0        0        0       34 2024-04-11 18:08:11.489360 galapy_core-0.2.0/galapy_core/generators/__init__.py
--rw-r--r--   0        0        0     1601 2024-04-11 18:34:30.553299 galapy_core-0.2.0/galapy_core/generators/price.py
--rw-r--r--   0        0        0     1219 2024-04-10 04:08:01.496749 galapy_core-0.2.0/galapy_core/generators.py
--rw-r--r--   0        0        0    12575 2024-04-10 04:09:23.792177 galapy_core-0.2.0/galapy_core/handlers.py
--rw-r--r--   0        0        0     7141 2024-04-11 19:05:22.667607 galapy_core-0.2.0/galapy_core/market_data.py
--rw-r--r--   0        0        0     9499 2024-04-11 19:07:14.900484 galapy_core-0.2.0/galapy_core/metrics.py
--rw-r--r--   0        0        0     8142 2024-04-11 19:07:36.802779 galapy_core-0.2.0/galapy_core/orders.py
--rw-r--r--   0        0        0    11285 2024-04-11 18:17:58.304006 galapy_core-0.2.0/galapy_core/portfolio.py
--rw-r--r--   0        0        0      485 2024-04-11 20:11:43.242607 galapy_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 galapy_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-10 02:38:11.989631 galapy_core-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 02:40:16.917509 galapy_core-0.2.1/galapy_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:40:16.924086 galapy_core-0.2.1/galapy_core/accounts.py
+-rw-r--r--   0        0        0    19258 2024-04-11 18:47:25.035325 galapy_core-0.2.1/galapy_core/assets.py
+-rw-r--r--   0        0        0      970 2024-04-13 10:18:36.757485 galapy_core-0.2.1/galapy_core/core.py
+-rw-r--r--   0        0        0      160 2024-04-11 18:34:19.554350 galapy_core-0.2.1/galapy_core/generators/README.md
+-rw-r--r--   0        0        0       34 2024-04-11 18:08:11.489360 galapy_core-0.2.1/galapy_core/generators/__init__.py
+-rw-r--r--   0        0        0     1601 2024-04-11 18:34:30.553299 galapy_core-0.2.1/galapy_core/generators/price.py
+-rw-r--r--   0        0        0     1219 2024-04-10 04:08:01.496749 galapy_core-0.2.1/galapy_core/generators.py
+-rw-r--r--   0        0        0    12575 2024-04-10 04:09:23.792177 galapy_core-0.2.1/galapy_core/handlers.py
+-rw-r--r--   0        0        0     7141 2024-04-11 19:05:22.667607 galapy_core-0.2.1/galapy_core/market_data.py
+-rw-r--r--   0        0        0     9525 2024-04-13 10:19:14.605147 galapy_core-0.2.1/galapy_core/metrics.py
+-rw-r--r--   0        0        0     8142 2024-04-11 19:07:36.802779 galapy_core-0.2.1/galapy_core/orders.py
+-rw-r--r--   0        0        0    11285 2024-04-11 18:17:58.304006 galapy_core-0.2.1/galapy_core/portfolio.py
+-rw-r--r--   0        0        0      485 2024-04-13 10:19:27.163570 galapy_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 galapy_core-0.2.1/PKG-INFO
```

### Comparing `galapy_core-0.2.0/galapy_core/assets.py` & `galapy_core-0.2.1/galapy_core/assets.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/core.py` & `galapy_core-0.2.1/galapy_core/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supamodel._core import BaseModel
+from supamodel._abc import BaseModel
 
 from galapy_core.assets import AssetClient
 from galapy_core.market_data import MarketDataClient
 from galapy_core.metrics import MetricClient
 from galapy_core.portfolio import PortfolioClient
```

### Comparing `galapy_core-0.2.0/galapy_core/generators/price.py` & `galapy_core-0.2.1/galapy_core/generators/price.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/generators.py` & `galapy_core-0.2.1/galapy_core/generators.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/handlers.py` & `galapy_core-0.2.1/galapy_core/handlers.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/market_data.py` & `galapy_core-0.2.1/galapy_core/market_data.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/metrics.py` & `galapy_core-0.2.1/galapy_core/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     AsyncFilterRequestBuilder,
     AsyncRequestBuilder,
 )
 from postgrest._sync.request_builder import SyncRequestBuilder
 from postgrest.base_request_builder import BaseFilterRequestBuilder
 from rich import print
 from supabase.client import PostgrestAPIError
+from supamodel._abc import BaseModel
 
 # from postgrest._async import AsyncPostgrestClient
 from supamodel._client import client as supabase
-from supamodel._core import BaseModel, Metric, TimeData
+from supamodel._core import Metric, TimeData
 from supamodel.utils import expose_dual_runtimes
 
 num_entries = 100  # Number of entries to generate
 start_date = datetime(2023, 1, 1)  # Start date for timestamps
 end_date = datetime(2023, 12, 31)  # End date for timestamps
 metric_types = [
     "balance",
```

### Comparing `galapy_core-0.2.0/galapy_core/orders.py` & `galapy_core-0.2.1/galapy_core/orders.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/galapy_core/portfolio.py` & `galapy_core-0.2.1/galapy_core/portfolio.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.0/PKG-INFO` & `galapy_core-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galapy-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: The backend and DB interactive layer for the GalaPy project
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ccxt (>=4.2.93,<5.0.0)
```

