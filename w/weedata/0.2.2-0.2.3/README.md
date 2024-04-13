# Comparing `tmp/weedata-0.2.2.tar.gz` & `tmp/weedata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weedata-0.2.2.tar", last modified: Wed Apr 10 00:19:45 2024, max compression
+gzip compressed data, was "weedata-0.2.3.tar", last modified: Sat Apr 13 16:03:22 2024, max compression
```

## Comparing `weedata-0.2.2.tar` & `weedata-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.114628 weedata-0.2.2/
--rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    18951 2024-04-10 00:19:45.111628 weedata-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    15977 2024-04-10 00:18:06.000000 weedata-0.2.2/README.md
--rw-rw-rw-   0        0        0     1417 2024-04-10 00:15:00.000000 weedata-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 00:19:45.115628 weedata-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 00:19:44.901607 weedata-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 00:19:44.962619 weedata-0.2.2/src/weedata/
--rw-rw-rw-   0        0        0      497 2024-03-09 02:13:09.000000 weedata-0.2.2/src/weedata/__init__.py
--rw-rw-rw-   0        0        0    31685 2024-03-25 21:24:11.000000 weedata-0.2.2/src/weedata/client.py
--rw-rw-rw-   0        0        0    15497 2024-03-23 21:38:50.000000 weedata-0.2.2/src/weedata/fields.py
--rw-rw-rw-   0        0        0     9591 2024-03-09 14:46:27.000000 weedata-0.2.2/src/weedata/model.py
--rw-rw-rw-   0        0        0     8012 2024-02-27 13:14:36.000000 weedata-0.2.2/src/weedata/queries.py
-drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.106628 weedata-0.2.2/src/weedata.egg-info/
--rw-rw-rw-   0        0        0    18951 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.085628 weedata-0.2.2/tests/
--rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.2/tests/test_base.py
--rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.2/tests/test_connection.py
--rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.2/tests/test_delete.py
--rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.2/tests/test_fields.py
--rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.2/tests/test_queries.py
--rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.2/tests/test_save.py
--rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.2/tests/test_update.py
+drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.374601 weedata-0.2.3/
+-rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    19037 2024-04-13 16:03:22.368601 weedata-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16059 2024-04-13 16:00:55.000000 weedata-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-13 16:01:14.000000 weedata-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 16:03:22.375601 weedata-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 16:03:21.416551 weedata-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 16:03:21.495567 weedata-0.2.3/src/weedata/
+-rw-rw-rw-   0        0        0      497 2024-04-13 16:01:26.000000 weedata-0.2.3/src/weedata/__init__.py
+-rw-rw-rw-   0        0        0    31685 2024-03-25 21:24:11.000000 weedata-0.2.3/src/weedata/client.py
+-rw-rw-rw-   0        0        0    15500 2024-04-13 15:58:34.000000 weedata-0.2.3/src/weedata/fields.py
+-rw-rw-rw-   0        0        0     9591 2024-03-09 14:46:27.000000 weedata-0.2.3/src/weedata/model.py
+-rw-rw-rw-   0        0        0     8012 2024-02-27 13:14:36.000000 weedata-0.2.3/src/weedata/queries.py
+drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.359601 weedata-0.2.3/src/weedata.egg-info/
+-rw-rw-rw-   0        0        0    19037 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.116601 weedata-0.2.3/tests/
+-rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.3/tests/test_base.py
+-rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.3/tests/test_connection.py
+-rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.3/tests/test_delete.py
+-rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.3/tests/test_fields.py
+-rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.3/tests/test_queries.py
+-rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.3/tests/test_save.py
+-rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.3/tests/test_update.py
```

### Comparing `weedata-0.2.2/LICENSE` & `weedata-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/PKG-INFO` & `weedata-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.2
+Version: 0.2.3
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -479,14 +479,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.3
+1. bugfix: TextField/BlobField/JSONField initial params not worked.   
+
+
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.   
 
 
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
```

### Comparing `weedata-0.2.2/README.md` & `weedata-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -429,14 +429,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.3
+1. bugfix: TextField/BlobField/JSONField initial params not worked.   
+
+
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.   
 
 
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
```

### Comparing `weedata-0.2.2/pyproject.toml` & `weedata-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "weedata"
-version = "0.2.2"
+version = "0.2.3"
 description = "an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 keywords = ["peewee", "ORM", "ODM", "google cloud datastore", "MongoDB", "redis"]
 dependencies = [
 #  "google-cloud-datastore",
```

### Comparing `weedata-0.2.2/src/weedata/client.py` & `weedata-0.2.3/src/weedata/client.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/src/weedata/fields.py` & `weedata-0.2.3/src/weedata/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,20 +345,20 @@
 
 FixedCharField = CharField
 UUIDField = CharField
 
 class TextField(CharField):
     def __init__(self, **kwargs):
         kwargs.setdefault('index', False)
-        super().__init__(*kwargs)
+        super().__init__(**kwargs)
 
 class BlobField(Field):
     def __init__(self, **kwargs):
         kwargs.setdefault('index', False)
-        super().__init__(*kwargs)
+        super().__init__(**kwargs)
         
     def check_type(self, value):
         return isinstance(value, bytes)
     def db_value(self, value):
         return value
     def python_value(self, value):
         return value
@@ -385,15 +385,15 @@
                 return datetime.datetime.fromisoformat(value)
         else:
             return value
 
 class JSONField(Field):
     def __init__(self, **kwargs):
         kwargs.setdefault('index', False)
-        super().__init__(*kwargs)
+        super().__init__(**kwargs)
 
     def check_type(self, value):
         json_types = [type(None), bool, int, float, str, list, dict, tuple]
         return any(isinstance(value, json_type) for json_type in json_types)
     def db_value(self, value):
         if self.bytes_store:
             return json.dumps(value).encode('utf-8')
```

### Comparing `weedata-0.2.2/src/weedata/model.py` & `weedata-0.2.3/src/weedata/model.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/src/weedata/queries.py` & `weedata-0.2.3/src/weedata/queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/src/weedata.egg-info/PKG-INFO` & `weedata-0.2.3/src/weedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.2
+Version: 0.2.3
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -479,14 +479,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.3
+1. bugfix: TextField/BlobField/JSONField initial params not worked.   
+
+
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.   
 
 
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
```

### Comparing `weedata-0.2.2/tests/test_base.py` & `weedata-0.2.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_connection.py` & `weedata-0.2.3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_delete.py` & `weedata-0.2.3/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_fields.py` & `weedata-0.2.3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_queries.py` & `weedata-0.2.3/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_save.py` & `weedata-0.2.3/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.2/tests/test_update.py` & `weedata-0.2.3/tests/test_update.py`

 * *Files identical despite different names*

