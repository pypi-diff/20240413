# Comparing `tmp/migoapiclient-1.1.3.tar.gz` & `tmp/migoapiclient-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.3.tar", last modified: Thu Apr 11 09:16:35 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.4.tar", last modified: Sat Apr 13 04:27:00 2024, max compression
```

## Comparing `migoapiclient-1.1.3.tar` & `migoapiclient-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/
--rw-rw-rw-   0        0        0     3900 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.783522 migoapiclient-1.1.3/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.3/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    11016 2024-04-11 09:09:30.000000 migoapiclient-1.1.3/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.3/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.785522 migoapiclient-1.1.3/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-11 09:14:34.000000 migoapiclient-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.785522 migoapiclient-1.1.3/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/
+-rw-rw-rw-   0        0        0     3900 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.074589 migoapiclient-1.1.4/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.4/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    11272 2024-04-13 04:25:08.000000 migoapiclient-1.1.4/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.4/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.077588 migoapiclient-1.1.4/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-13 04:27:00.000000 migoapiclient-1.1.4/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-13 04:25:39.000000 migoapiclient-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.076588 migoapiclient-1.1.4/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.4/src/__init__.py
```

### Comparing `migoapiclient-1.1.3/PKG-INFO` & `migoapiclient-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.3
+Version: 1.1.4
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.3/README.md` & `migoapiclient-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.3/migoapiclient/api_client.py` & `migoapiclient-1.1.4/migoapiclient/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,32 +43,30 @@
 
     def try_get(self, url, error_count: int = 0, **kwargs):
         """
         尝试重发get请求
         """
         while error_count <= self.retry_count:
             try:
-                kwargs['timeout'] = self.timeout
-                res_data = self.get(url, **kwargs)
+                res_data = self.get(url, timeout=self.timeout, **kwargs)
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
                 return self.try_get(url, error_count, **kwargs)
         raise Exception('已经尝试请求：{}次，服务器依然没有响应'.format(self.retry_count))
 
     def try_post(self, url: str, error_count: int = 0, **kwargs):
         """
         尝试重发post请求
         """
         while error_count <= self.retry_count:
             try:
-                kwargs['timeout'] = self.timeout
-                res_data = self.post(url, **kwargs)
+                res_data = self.post(url, timeout=self.timeout, **kwargs)
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
                 time.sleep(error_count)
                 return self.try_post(url, error_count, **kwargs)
@@ -91,18 +89,19 @@
         self.headers = {
             'AUTH-KEY': auth_key,
             'CURRENT-USER-NAME': 'system',
             'CURRENT-USER-ID': '100001'
         }
         self.log_manager = LogFileManager(log_path)
 
-    def res_callback(self, response_data: dict):
+    def res_callback(self, res: Response):
         """
         响应回调
         """
+        response_data = res.json()
         if response_data['code'] != 200:
             raise Exception(response_data['message'])
         return response_data
 
     def migo_try_get(self, url, migo_shop_id, data_type: str, error_count: int = 0, **kwargs):
         """
         自定义发get请求
@@ -139,24 +138,23 @@
         """
         获取店铺授权信息
         :param migo_shop_id 米果店铺ID
         """
         uri = f'/data-collection-service/node/auths/{migo_shop_id}'
         return self.migo_try_get(self.host + uri, migo_shop_id, '获取店铺授权信息')
 
-    def get_node_info_list(self, migo_shop_id: int = None):
+    def get_node_info_list(self, migo_shop_id: int = 0):
         """
         获取节点信息列表
         :param migo_shop_id 米果店铺ID
         """
         post_data = {
-            "nodeConfigId": self.node_id
+            "nodeConfigId": self.node_id,
+            "shopId": migo_shop_id
         }
-        if migo_shop_id:
-            post_data['shopId'] = migo_shop_id
         uri = f'/data-collection-service/node/search'
         response_data = self.migo_try_post(self.host + uri, migo_shop_id, '获取节点信息列表', json=post_data)
         if migo_shop_id:
             response_data['data'] = response_data['data'][0]  # 如果是查询单个店铺的话，数据解析成字典
         return response_data
 
     def post_auth_data(self, migo_shop_id, **kwargs):
@@ -239,33 +237,32 @@
                 '',
                 post_data,
                 str(e),
             )
             self.log_manager.write_request_error_log(msg)
             raise e
 
-    def post_info_log(self, msg: str, data_type: str, node_id: str, shop_id: str, log_data: dict = None,
+    def post_info_log(self, msg: str, data_type: str, shop_id: str, log_data: dict = None,
                       log_params: dict = None, log_stack: str = None):
         """
         上传日志
         :param msg 信息
         :param data_type 数据类型
-        :param node_id 节点ID
         :param shop_id 店铺ID
         :param log_data 请求的post参数
         :param log_params 请求的get参数
         :param log_stack 日志其他信息
         """
         uri = '/data-collection-service/node/logsave'
         post_data = {
             "data": [
                 {
                     "id": str(time.time()).replace('.', ''),
                     "shopId": shop_id,
-                    "nodeId": node_id,
+                    "nodeId": self.node_id,
                     "dataType": data_type,
                     "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
                     "logData": json.dumps(log_data),
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": msg
                 }
@@ -286,7 +283,18 @@
         uri = '/data-collection-service/node/es/query'
         post_data = {
             'sourceStrings': column_list,
             'queryString': json.dumps(es_query),
             'indexName': table_name
         }
         return self.migo_try_post(self.host + uri, 0, '获取节点信息', 0, json=post_data)
+
+    def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None):
+        """
+        上传日志
+        :param msg 信息
+        :param shop_id 店铺ID
+        :param definition_info 策略信息
+        """
+        data_type = '调度任务失败'
+        return self.post_info_log(msg, data_type, shop_id, definition_info)
+
```

### Comparing `migoapiclient-1.1.3/migoapiclient/file_manager.py` & `migoapiclient-1.1.4/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.3/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.4/migoapiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.3
+Version: 1.1.4
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.3/setup.py` & `migoapiclient-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

