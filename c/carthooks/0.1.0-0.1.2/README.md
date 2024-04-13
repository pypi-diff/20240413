# Comparing `tmp/carthooks-0.1.0.tar.gz` & `tmp/carthooks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carthooks-0.1.0.tar", last modified: Wed Mar 20 01:48:28 2024, max compression
+gzip compressed data, was "carthooks-0.1.2.tar", last modified: Sat Apr 13 09:43:55 2024, max compression
```

## Comparing `carthooks-0.1.0.tar` & `carthooks-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:28.271074 carthooks-0.1.0/
--rw-r--r--   0 wanglei    (501) staff       (20)      342 2024-03-20 01:48:28.269076 carthooks-0.1.0/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)       13 2024-03-16 12:24:42.000000 carthooks-0.1.0/README.md
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:28.265612 carthooks-0.1.0/carthooks/
--rw-r--r--   0 wanglei    (501) staff       (20)       23 2024-03-19 06:34:01.000000 carthooks-0.1.0/carthooks/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)     3828 2024-03-19 16:53:06.000000 carthooks-0.1.0/carthooks/sdk.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:28.268279 carthooks-0.1.0/carthooks.egg-info/
--rw-r--r--   0 wanglei    (501) staff       (20)      342 2024-03-20 01:48:28.000000 carthooks-0.1.0/carthooks.egg-info/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)      221 2024-03-20 01:48:28.000000 carthooks-0.1.0/carthooks.egg-info/SOURCES.txt
--rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-03-20 01:48:28.000000 carthooks-0.1.0/carthooks.egg-info/dependency_links.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       17 2024-03-20 01:48:28.000000 carthooks-0.1.0/carthooks.egg-info/requires.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       10 2024-03-20 01:48:28.000000 carthooks-0.1.0/carthooks.egg-info/top_level.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-03-20 01:48:28.271636 carthooks-0.1.0/setup.cfg
--rw-r--r--   0 wanglei    (501) staff       (20)      579 2024-03-16 12:22:39.000000 carthooks-0.1.0/setup.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:43:55.645559 carthooks-0.1.2/
+-rw-r--r--   0 wanglei    (501) staff       (20)      338 2024-04-13 09:43:55.644463 carthooks-0.1.2/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)       13 2024-03-16 12:24:42.000000 carthooks-0.1.2/README.md
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:43:55.640668 carthooks-0.1.2/carthooks/
+-rw-r--r--   0 wanglei    (501) staff       (20)       23 2024-03-19 06:34:01.000000 carthooks-0.1.2/carthooks/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5310 2024-04-12 10:38:19.000000 carthooks-0.1.2/carthooks/sdk.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:43:55.643595 carthooks-0.1.2/carthooks.egg-info/
+-rw-r--r--   0 wanglei    (501) staff       (20)      338 2024-04-13 09:43:55.000000 carthooks-0.1.2/carthooks.egg-info/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)      221 2024-04-13 09:43:55.000000 carthooks-0.1.2/carthooks.egg-info/SOURCES.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-04-13 09:43:55.000000 carthooks-0.1.2/carthooks.egg-info/dependency_links.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       17 2024-04-13 09:43:55.000000 carthooks-0.1.2/carthooks.egg-info/requires.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       10 2024-04-13 09:43:55.000000 carthooks-0.1.2/carthooks.egg-info/top_level.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-04-13 09:43:55.645755 carthooks-0.1.2/setup.cfg
+-rw-r--r--   0 wanglei    (501) staff       (20)      531 2024-04-13 09:40:50.000000 carthooks-0.1.2/setup.py
```

### Comparing `carthooks-0.1.0/carthooks/sdk.py` & `carthooks-0.1.2/carthooks/sdk.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import requests
+import os
 
 class Result:
     def __init__(self, response):
+        self.trace_id = None
+        self.meta = None
         try:
             self.response = response.json()
             self.data = self.response.get('data')
             self.error = self.response.get("error")
             self.trace_id = self.response.get("traceId")
             self.meta = self.response.get("meta")
             if self.error:
@@ -14,64 +17,87 @@
             else:
                 self.success = True
         except:
             self.data = None
             self.error = response.text
             self.success = False
 
+    def __getitem__(self, key):
+        return self.data.get(key)
+
     def __str__(self) -> str:
-        return f"CarthooksResult(success={self.success}, data={self.data}, error={self.error}, trace_id={self.trace_id}, meta={self.meta})"
+        return f"CarthooksResult(success={self.success}, data={self.data}, error={self.error})"
 
 class Client:
-    def __init__(self, base_url="https://api.carthooks.com"):
-        self.base_url = base_url
+    def __init__(self):
+        self.base_url = os.getenv('CARTHOOKS_API_URL')
+        if self.base_url == None:
+            self.base_url = "https://api.carthooks.com"
         self.headers = {
             'Content-Type': 'application/json',
         }
 
-    def set_access_token(self, access_token):
+    def setAccessToken(self, access_token):
         self.headers['Authorization'] = f'Bearer {access_token}'
 
-    def get_items(self, app_id, collection_id, limit=20, page=1, **options):
+    def getItems(self, app_id, collection_id, limit=20, page=1, **options):
         options['pagination[page]'] = page
         options['pagination[pageSize]'] = limit
-        print("options", options)
-        response = requests.get(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items', headers=self.headers, params=options)
+        url = f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items'
+        print(options)
+        response = requests.get(url, headers=self.headers, params=options)
+        return Result(response)
+    
+    def getItemById(self, app_id, collection_id, item_id, fields=None):
+        response = requests.get(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}', headers=self.headers)
+        return Result(response)
+    
+
+# POST    /open/api/v1/apps/:app_id/collections/:entity_id/items/:row_id/subform/:field_id/     OpenAPI.CreateSubItem
+# PUT     /open/api/v1/apps/:app_id/collections/:entity_id/items/:row_id/subform/:field_id/items/:sub_row_id/:sub_row_id     OpenAPI.UpdateSubItem
+# DELETE  /open/api/v1/apps/:app_id/collections/:entity_id/items/:row_id/subform/:field_id/items/:sub_row_id/:sub_row_id     OpenAPI.DeleteSubItem
+    def createSubItem(self, app_id, collection_id, item_id, field_id, data):
+        response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/subform/{field_id}', headers=self.headers, json={'data': data})
+        return Result(response)
+    
+    def updateSubItem(self, app_id, collection_id, item_id, field_id, sub_item_id, data):
+        print("data", data)
+        response = requests.put(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/subform/{field_id}/items/{sub_item_id}', headers=self.headers, json={'data': data})
         return Result(response)
     
-    def get_item_by_id(self, app_id, collection_id, item_id, fields):
-        response = requests.get(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}', headers=self.headers, params={'fields': fields})
+    def deleteSubItem(self, app_id, collection_id, item_id, field_id, sub_item_id):
+        response = requests.delete(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/subform/{field_id}/items/{sub_item_id}', headers=self.headers)
         return Result(response)
     
-    def get_submission_token(self, app_id, collection_id, options):
+    def getSubmissionToken(self, app_id, collection_id, options):
         response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/submission-token', headers=self.headers, json=options)
         return Result(response)
     
-    def update_submission_token(self, app_id, collection_id, item_id, options):
+    def updateSubmissionToken(self, app_id, collection_id, item_id, options):
         response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/update-token', headers=self.headers, json=options)
         return Result(response)
     
-    def create_item(self, app_id, collection_id, data):
+    def createItem(self, app_id, collection_id, data):
         response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items', headers=self.headers, json={'data': data})
         return Result(response)
     
-    def update_item(self, app_id, collection_id, item_id, data):
+    def updateItem(self, app_id, collection_id, item_id, data):
         response = requests.put(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}', headers=self.headers, json={'data': data})
         return Result(response)
     
-    def lock_item(self, app_id, collection_id, item_id, lock_timeout=600, lock_id=None, subject=None):
+    def lockItem(self, app_id, collection_id, item_id, lock_timeout=600, lock_id=None, subject=None):
         response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/lock', 
                                  headers=self.headers, json={'lockTimeout': lock_timeout, 'lockId': lock_id, 'lockSubject': subject}) 
         return Result(response)
     
-    def unlock_item(self, app_id, collection_id, item_id, lock_id=None):
+    def unlockItem(self, app_id, collection_id, item_id, lock_id=None):
         response = requests.post(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}/unlock', headers=self.headers, json={'lockId': lock_id})
         return Result(response)
     
-    def delete_item(self, app_id, collection_id, item_id):
+    def deleteItem(self, app_id, collection_id, item_id):
         response = requests.delete(f'{self.base_url}/v1/apps/{app_id}/collections/{collection_id}/items/{item_id}', headers=self.headers)
         return Result(response)
     
     def get_upload_token(self):
         response = requests.post(f'{self.base_url}/v1/uploads/token', headers=self.headers)
         return Result(response)
```

