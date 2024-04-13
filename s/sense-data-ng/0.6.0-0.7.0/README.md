# Comparing `tmp/sense-data-ng-0.6.0.tar.gz` & `tmp/sense-data-ng-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense-data-ng-0.6.0.tar", last modified: Wed Apr  6 05:53:42 2022, max compression
+gzip compressed data, was "sense-data-ng-0.7.0.tar", last modified: Sat Apr 13 15:03:17 2024, max compression
```

## Comparing `sense-data-ng-0.6.0.tar` & `sense-data-ng-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-06 05:53:42.136150 sense-data-ng-0.6.0/
--rw-rw-r--   0 work      (1000) work      (1000)      213 2022-04-06 05:53:42.136150 sense-data-ng-0.6.0/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)    12401 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/README.md
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-06 05:53:42.132149 sense-data-ng-0.6.0/sense_data/
--rw-rw-r--   0 work      (1000) work      (1000)       60 2022-04-06 05:53:08.000000 sense-data-ng-0.6.0/sense_data/__init__.py
--rw-rw-r--   0 work      (1000) work      (1000)    10818 2022-04-06 05:53:08.000000 sense-data-ng-0.6.0/sense_data/client.py
--rw-rw-r--   0 work      (1000) work      (1000)     1368 2022-03-30 14:53:41.000000 sense-data-ng-0.6.0/sense_data/decorator.py
--rw-rw-r--   0 work      (1000) work      (1000)     7350 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/sense_data/dictobj.py
--rw-rw-r--   0 work      (1000) work      (1000)    16330 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/sense_data/stock_pb2.py
--rw-rw-r--   0 work      (1000) work      (1000)    19257 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/sense_data/stock_pb2_grpc.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-06 05:53:42.136150 sense-data-ng-0.6.0/sense_data_ng.egg-info/
--rw-rw-r--   0 work      (1000) work      (1000)      213 2022-04-06 05:53:41.000000 sense-data-ng-0.6.0/sense_data_ng.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)      383 2022-04-06 05:53:42.000000 sense-data-ng-0.6.0/sense_data_ng.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1000) work      (1000)        1 2022-04-06 05:53:41.000000 sense-data-ng-0.6.0/sense_data_ng.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1000) work      (1000)       40 2022-04-06 05:53:41.000000 sense-data-ng-0.6.0/sense_data_ng.egg-info/requires.txt
--rw-rw-r--   0 work      (1000) work      (1000)       11 2022-04-06 05:53:41.000000 sense-data-ng-0.6.0/sense_data_ng.egg-info/top_level.txt
--rw-rw-r--   0 work      (1000) work      (1000)       38 2022-04-06 05:53:42.136150 sense-data-ng-0.6.0/setup.cfg
--rw-rw-r--   0 work      (1000) work      (1000)     1016 2022-04-06 05:53:08.000000 sense-data-ng-0.6.0/setup.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-06 05:53:42.136150 sense-data-ng-0.6.0/test/
--rw-rw-r--   0 work      (1000) work      (1000)     4606 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/test/test_client.py
--rw-rw-r--   0 work      (1000) work      (1000)      741 2022-03-30 11:47:52.000000 sense-data-ng-0.6.0/test/test_pool.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:03:17.707363 sense-data-ng-0.7.0/
+-rw-rw-r--   0 work      (1000) work      (1000)      155 2024-04-13 15:03:17.707363 sense-data-ng-0.7.0/PKG-INFO
+-rw-rw-r--   0 work      (1000) work      (1000)    12401 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/README.md
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:03:17.703363 sense-data-ng-0.7.0/sense_data/
+-rw-rw-r--   0 work      (1000) work      (1000)       60 2022-04-06 05:53:08.000000 sense-data-ng-0.7.0/sense_data/__init__.py
+-rw-rw-r--   0 work      (1000) work      (1000)    11075 2024-04-13 14:45:15.000000 sense-data-ng-0.7.0/sense_data/client.py
+-rw-rw-r--   0 work      (1000) work      (1000)     1368 2022-03-30 14:53:41.000000 sense-data-ng-0.7.0/sense_data/decorator.py
+-rw-rw-r--   0 work      (1000) work      (1000)     7350 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/sense_data/dictobj.py
+-rw-rw-r--   0 work      (1000) work      (1000)    16330 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/sense_data/stock_pb2.py
+-rw-rw-r--   0 work      (1000) work      (1000)    19257 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/sense_data/stock_pb2_grpc.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:03:17.703363 sense-data-ng-0.7.0/sense_data_ng.egg-info/
+-rw-rw-r--   0 work      (1000) work      (1000)      155 2024-04-13 15:03:17.000000 sense-data-ng-0.7.0/sense_data_ng.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1000) work      (1000)      383 2024-04-13 15:03:17.000000 sense-data-ng-0.7.0/sense_data_ng.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1000) work      (1000)        1 2024-04-13 15:03:17.000000 sense-data-ng-0.7.0/sense_data_ng.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       40 2024-04-13 15:03:17.000000 sense-data-ng-0.7.0/sense_data_ng.egg-info/requires.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       11 2024-04-13 15:03:17.000000 sense-data-ng-0.7.0/sense_data_ng.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       38 2024-04-13 15:03:17.707363 sense-data-ng-0.7.0/setup.cfg
+-rw-rw-r--   0 work      (1000) work      (1000)     1016 2024-04-13 15:03:14.000000 sense-data-ng-0.7.0/setup.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:03:17.703363 sense-data-ng-0.7.0/test/
+-rw-rw-r--   0 work      (1000) work      (1000)     4606 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/test/test_client.py
+-rw-rw-r--   0 work      (1000) work      (1000)      741 2022-03-30 11:47:52.000000 sense-data-ng-0.7.0/test/test_pool.py
```

### Comparing `sense-data-ng-0.6.0/README.md` & `sense-data-ng-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/sense_data/client.py` & `sense-data-ng-0.7.0/sense_data/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,14 +280,19 @@
         _response = stub.get_infos_by_terms(stock_pb2.Request(entity_name=_names_list))
         return json.loads(_response.txt)
 
     # 23广彬用
     @catch_except_log
     def get_multi_market_info_by_name(self, name, stub=None):
         _response = stub.get_multi_market_info_by_name(stock_pb2.Request(entity_name=name))
+        try:
+            result = json.loads(_response.txt)
+        except:
+            logging.warning("json loads error: get_multi_market_info_by_name:%s" % _response.txt)
+            return []
         return json.loads(_response.txt)
 
     # 24广彬用
     @catch_except_log
     def get_main_market_info_by_name(self, name, stub=None):
         _response = stub.get_main_market_info_by_name(stock_pb2.Request(entity_name=name))
         return json.loads(_response.txt)
@@ -300,9 +305,10 @@
 
 
 if __name__ == '__main__':
     import sense_core as sd
     sd.log_init_config(root_path=sd.config('log_path'))
     sense_data = SenseDataService()
     # r = sense_data.get_detail_info_by_name('石化油服')
-    r = sense_data.get_stock_price_day('600871', '2019-7-20', '2019-7-22')
+    # r = sense_data.get_stock_price_day('600871', '2019-7-20', '2019-7-22')
+    r = sense_data.get_market_info_by_stock_code('001337')
     print(r)
```

### Comparing `sense-data-ng-0.6.0/sense_data/decorator.py` & `sense-data-ng-0.7.0/sense_data/decorator.py`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/sense_data/dictobj.py` & `sense-data-ng-0.7.0/sense_data/dictobj.py`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/sense_data/stock_pb2.py` & `sense-data-ng-0.7.0/sense_data/stock_pb2.py`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/sense_data/stock_pb2_grpc.py` & `sense-data-ng-0.7.0/sense_data/stock_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/setup.py` & `sense-data-ng-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ]
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read().encode("bytes")
 
 setup(
     name='sense-data-ng',
-    version='0.6.0',
+    version='0.7.0',
     packages=['sense_data'],
     #packages=find_packages('client_rpc'),  # 包含所有sense_data中的包
     #package_dir = {'':'client_rpc'},   # 告诉distutils包都在sense_data下
     include_package_data = True,
     install_requires=requirements,
```

### Comparing `sense-data-ng-0.6.0/test/test_client.py` & `sense-data-ng-0.7.0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `sense-data-ng-0.6.0/test/test_pool.py` & `sense-data-ng-0.7.0/test/test_pool.py`

 * *Files identical despite different names*

