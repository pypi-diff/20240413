# Comparing `tmp/mqi_sspd_api-0.0.3.tar.gz` & `tmp/mqi_sspd_api-0.0.5.tar.gz`

## Comparing `mqi_sspd_api-0.0.3.tar` & `mqi_sspd_api-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/examples/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/examples/set_current.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/mqi/v1/__init__.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/mqi/v1/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/examples/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/examples/set_current.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/mqi/v1/__init__.py
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/mqi/v1/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/PKG-INFO
```

### Comparing `mqi_sspd_api-0.0.3/mqi/v1/api.py` & `mqi_sspd_api-0.0.5/mqi/v1/api.py`

 * *Files identical despite different names*

### Comparing `mqi_sspd_api-0.0.3/LICENSE` & `mqi_sspd_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mqi_sspd_api-0.0.3/PKG-INFO` & `mqi_sspd_api-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.3
 Name: mqi_sspd_api
-Version: 0.0.3
+Version: 0.0.5
 Summary: This is the official API of the MQI biasing box
 Project-URL: Homepage, https://github.com/MQI-Software/mqi-api
 Project-URL: Issues, https://github.com/MQI-Software/mqi-api/issues
 Author-email: Filip Zlatoidsky <fillatino@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
+Requires-Dist: rel
+Requires-Dist: websocket-client
 Description-Content-Type: text/markdown
 
 # MQI Managing Module API
 
 This is the official API made for the MQI biasing box.
```

