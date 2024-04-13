# Comparing `tmp/sense-data-0.5.9.tar.gz` & `tmp/sense-data-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense-data-0.5.9.tar", last modified: Fri Apr  1 12:55:01 2022, max compression
+gzip compressed data, was "sense-data-0.7.0.tar", last modified: Sat Apr 13 15:01:31 2024, max compression
```

## Comparing `sense-data-0.5.9.tar` & `sense-data-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-01 12:55:01.928115 sense-data-0.5.9/
--rw-rw-r--   0 work      (1000) work      (1000)      210 2022-04-01 12:55:01.928115 sense-data-0.5.9/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)    12401 2022-03-30 11:47:52.000000 sense-data-0.5.9/README.md
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-01 12:55:01.928115 sense-data-0.5.9/sense_data/
--rw-rw-r--   0 work      (1000) work      (1000)       60 2022-03-30 15:10:43.000000 sense-data-0.5.9/sense_data/__init__.py
--rw-rw-r--   0 work      (1000) work      (1000)    10725 2022-03-30 11:47:52.000000 sense-data-0.5.9/sense_data/client.py
--rw-rw-r--   0 work      (1000) work      (1000)     1368 2022-03-30 14:53:41.000000 sense-data-0.5.9/sense_data/decorator.py
--rw-rw-r--   0 work      (1000) work      (1000)     7350 2022-03-30 11:47:52.000000 sense-data-0.5.9/sense_data/dictobj.py
--rw-rw-r--   0 work      (1000) work      (1000)    16330 2022-03-30 11:47:52.000000 sense-data-0.5.9/sense_data/stock_pb2.py
--rw-rw-r--   0 work      (1000) work      (1000)    19257 2022-03-30 11:47:52.000000 sense-data-0.5.9/sense_data/stock_pb2_grpc.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-01 12:55:01.928115 sense-data-0.5.9/sense_data.egg-info/
--rw-rw-r--   0 work      (1000) work      (1000)      210 2022-04-01 12:55:01.000000 sense-data-0.5.9/sense_data.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1000) work      (1000)      368 2022-04-01 12:55:01.000000 sense-data-0.5.9/sense_data.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1000) work      (1000)        1 2022-04-01 12:55:01.000000 sense-data-0.5.9/sense_data.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1000) work      (1000)       40 2022-04-01 12:55:01.000000 sense-data-0.5.9/sense_data.egg-info/requires.txt
--rw-rw-r--   0 work      (1000) work      (1000)       11 2022-04-01 12:55:01.000000 sense-data-0.5.9/sense_data.egg-info/top_level.txt
--rw-rw-r--   0 work      (1000) work      (1000)       38 2022-04-01 12:55:01.928115 sense-data-0.5.9/setup.cfg
--rw-rw-r--   0 work      (1000) work      (1000)     1013 2022-04-01 12:53:11.000000 sense-data-0.5.9/setup.py
-drwxrwxr-x   0 work      (1000) work      (1000)        0 2022-04-01 12:55:01.928115 sense-data-0.5.9/test/
--rw-rw-r--   0 work      (1000) work      (1000)     4606 2022-03-30 11:47:52.000000 sense-data-0.5.9/test/test_client.py
--rw-rw-r--   0 work      (1000) work      (1000)      741 2022-03-30 11:47:52.000000 sense-data-0.5.9/test/test_pool.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:01:31.451461 sense-data-0.7.0/
+-rw-rw-r--   0 work      (1000) work      (1000)      152 2024-04-13 15:01:31.451461 sense-data-0.7.0/PKG-INFO
+-rw-rw-r--   0 work      (1000) work      (1000)    12401 2022-03-30 11:47:52.000000 sense-data-0.7.0/README.md
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:01:31.447461 sense-data-0.7.0/sense_data/
+-rw-rw-r--   0 work      (1000) work      (1000)       60 2022-04-06 05:53:08.000000 sense-data-0.7.0/sense_data/__init__.py
+-rw-rw-r--   0 work      (1000) work      (1000)    11075 2024-04-13 14:45:15.000000 sense-data-0.7.0/sense_data/client.py
+-rw-rw-r--   0 work      (1000) work      (1000)     1368 2022-03-30 14:53:41.000000 sense-data-0.7.0/sense_data/decorator.py
+-rw-rw-r--   0 work      (1000) work      (1000)     7350 2022-03-30 11:47:52.000000 sense-data-0.7.0/sense_data/dictobj.py
+-rw-rw-r--   0 work      (1000) work      (1000)    16330 2022-03-30 11:47:52.000000 sense-data-0.7.0/sense_data/stock_pb2.py
+-rw-rw-r--   0 work      (1000) work      (1000)    19257 2022-03-30 11:47:52.000000 sense-data-0.7.0/sense_data/stock_pb2_grpc.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:01:31.451461 sense-data-0.7.0/sense_data.egg-info/
+-rw-rw-r--   0 work      (1000) work      (1000)      152 2024-04-13 15:01:31.000000 sense-data-0.7.0/sense_data.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1000) work      (1000)      368 2024-04-13 15:01:31.000000 sense-data-0.7.0/sense_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1000) work      (1000)        1 2024-04-13 15:01:31.000000 sense-data-0.7.0/sense_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       40 2024-04-13 15:01:31.000000 sense-data-0.7.0/sense_data.egg-info/requires.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       11 2024-04-13 15:01:31.000000 sense-data-0.7.0/sense_data.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1000) work      (1000)       38 2024-04-13 15:01:31.451461 sense-data-0.7.0/setup.cfg
+-rw-rw-r--   0 work      (1000) work      (1000)     1013 2024-04-13 14:45:29.000000 sense-data-0.7.0/setup.py
+drwxrwxr-x   0 work      (1000) work      (1000)        0 2024-04-13 15:01:31.451461 sense-data-0.7.0/test/
+-rw-rw-r--   0 work      (1000) work      (1000)     4606 2022-03-30 11:47:52.000000 sense-data-0.7.0/test/test_client.py
+-rw-rw-r--   0 work      (1000) work      (1000)      741 2022-03-30 11:47:52.000000 sense-data-0.7.0/test/test_pool.py
```

### Comparing `sense-data-0.5.9/README.md` & `sense-data-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/sense_data/client.py` & `sense-data-0.7.0/sense_data/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Email: weix@sensedeal.ai                                 
 Last modified: 2018.12.20 18:25 
 Description:                                            
 '''
 
 import json
 import datetime
+import logging
 from sense_data.dictobj import *
 from sense_data import stock_pb2
 from sense_data.decorator import catch_except_log
 
 
 def _dict_list_model(list_dict, model_class):
     _dct_list = []
@@ -259,14 +260,15 @@
         _response = stub.get_code_by_name(stock_pb2.Request(entity_name=name))
         return json.loads(_response.txt)
 
     # 20广彬用
     @catch_except_log
     def get_detail_info_by_name(self, name, stub=None):
         _response = stub.get_detail_info_by_name(stock_pb2.Request(entity_name=name))
+        logging.debug("get_detail_info_by_name response: %s" % _response.txt)
         return json.loads(_response.txt)
 
     # 21广彬用
     @catch_except_log
     def get_company_role_info(self, code, stub=None):
         _response = stub.get_company_role_info(stock_pb2.Request(stock_code=code))
         return json.loads(_response.txt)
@@ -278,14 +280,19 @@
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
@@ -298,9 +305,10 @@
 
 
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

### Comparing `sense-data-0.5.9/sense_data/decorator.py` & `sense-data-0.7.0/sense_data/decorator.py`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/sense_data/dictobj.py` & `sense-data-0.7.0/sense_data/dictobj.py`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/sense_data/stock_pb2.py` & `sense-data-0.7.0/sense_data/stock_pb2.py`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/sense_data/stock_pb2_grpc.py` & `sense-data-0.7.0/sense_data/stock_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/setup.py` & `sense-data-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ]
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read().encode("bytes")
 
 setup(
     name='sense-data',
-    version='0.5.9',
+    version='0.7.0',
     packages=['sense_data'],
     #packages=find_packages('client_rpc'),  # 包含所有sense_data中的包
     #package_dir = {'':'client_rpc'},   # 告诉distutils包都在sense_data下
     include_package_data = True,
     install_requires=requirements,
```

### Comparing `sense-data-0.5.9/test/test_client.py` & `sense-data-0.7.0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `sense-data-0.5.9/test/test_pool.py` & `sense-data-0.7.0/test/test_pool.py`

 * *Files identical despite different names*

