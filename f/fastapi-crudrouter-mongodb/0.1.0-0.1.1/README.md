# Comparing `tmp/fastapi-crudrouter-mongodb-0.1.0.tar.gz` & `tmp/fastapi-crudrouter-mongodb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-crudrouter-mongodb-0.1.0.tar", last modified: Sun Mar 31 16:00:42 2024, max compression
+gzip compressed data, was "fastapi-crudrouter-mongodb-0.1.1.tar", last modified: Sat Apr 13 10:00:26 2024, max compression
```

## Comparing `fastapi-crudrouter-mongodb-0.1.0.tar` & `fastapi-crudrouter-mongodb-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.736642 fastapi-crudrouter-mongodb-0.1.0/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/LICENSE
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     5322 2024-03-31 16:00:42.736642 fastapi-crudrouter-mongodb-0.1.0/PKG-INFO
--rw-r--r--   0 pierro    (1000) pierro    (1000)     3906 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/README.md
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/
--rw-r--r--   0 pierro    (1000) pierro    (1000)      397 2024-03-31 15:57:46.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/
--rw-r--r--   0 pierro    (1000) pierro    (1000)      247 2024-03-30 18:41:34.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/
--rw-r--r--   0 pierro    (1000) pierro    (1000)      132 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)      478 2024-03-30 18:15:56.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)      291 2024-03-30 18:40:43.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/__init__.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       85 2024-03-30 16:32:05.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/deleted_mongo_model.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     2194 2024-03-30 18:11:29.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/mongo_model.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1005 2024-03-30 16:34:08.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)    10169 2024-03-31 12:06:46.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     2612 2024-03-30 16:32:05.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     5279 2024-03-30 16:29:20.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)      220 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     5630 2024-03-31 11:47:18.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1377 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     3159 2024-03-31 12:06:28.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)       83 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     7473 2024-03-31 12:06:28.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1377 2024-03-30 16:26:48.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)     4336 2024-03-31 11:45:16.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)       86 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.736642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/utils/
--rw-r--r--   0 pierro    (1000) pierro    (1000)       66 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/utils/__init__.py
--rw-r--r--   0 pierro    (1000) pierro    (1000)      494 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/utils/deprecated_util.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-03-31 16:00:42.732642 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/
--rwxr-xr-x   0 pierro    (1000) pierro    (1000)     5322 2024-03-31 16:00:42.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
--rwxr-xr-x   0 pierro    (1000) pierro    (1000)     1567 2024-03-31 16:00:42.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
--rwxr-xr-x   0 pierro    (1000) pierro    (1000)        1 2024-03-31 16:00:42.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
--rwxr-xr-x   0 pierro    (1000) pierro    (1000)       31 2024-03-31 16:00:42.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/requires.txt
--rwxr-xr-x   0 pierro    (1000) pierro    (1000)       27 2024-03-31 16:00:42.000000 fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2024-03-31 16:00:42.736642 fastapi-crudrouter-mongodb-0.1.0/setup.cfg
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1699 2024-03-31 15:57:41.000000 fastapi-crudrouter-mongodb-0.1.0/setup.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/LICENSE
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5682 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/PKG-INFO
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     4266 2024-04-01 10:54:56.000000 fastapi-crudrouter-mongodb-0.1.1/README.md
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.684469 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      397 2024-04-13 09:59:03.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.684469 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      247 2024-03-30 18:41:34.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.684469 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      132 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      478 2024-03-30 18:15:56.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      291 2024-03-30 18:40:43.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/__init__.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       85 2024-03-30 16:32:05.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/deleted_mongo_model.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     3218 2024-04-09 11:11:47.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/mongo_model.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1005 2024-03-30 16:34:08.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)    10169 2024-03-31 12:06:46.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     2612 2024-03-30 16:32:05.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     5279 2024-03-30 16:29:20.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      220 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     5630 2024-03-31 11:47:18.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1377 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     3159 2024-03-31 12:06:28.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)       83 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     7473 2024-03-31 12:06:28.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1377 2024-03-30 16:26:48.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     4336 2024-03-31 11:45:16.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)       86 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/utils/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)       66 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/utils/__init__.py
+-rw-r--r--   0 pierro    (1000) pierro    (1000)      494 2024-03-29 17:59:02.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/utils/deprecated_util.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2024-04-13 10:00:26.684469 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/
+-rwxr-xr-x   0 pierro    (1000) pierro    (1000)     5682 2024-04-13 10:00:26.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
+-rwxr-xr-x   0 pierro    (1000) pierro    (1000)     1567 2024-04-13 10:00:26.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
+-rwxr-xr-x   0 pierro    (1000) pierro    (1000)        1 2024-04-13 10:00:26.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pierro    (1000) pierro    (1000)       31 2024-04-13 10:00:26.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/requires.txt
+-rwxr-xr-x   0 pierro    (1000) pierro    (1000)       27 2024-04-13 10:00:26.000000 fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2024-04-13 10:00:26.688470 fastapi-crudrouter-mongodb-0.1.1/setup.cfg
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1699 2024-04-13 09:58:58.000000 fastapi-crudrouter-mongodb-0.1.1/setup.py
```

### Comparing `fastapi-crudrouter-mongodb-0.1.0/LICENSE` & `fastapi-crudrouter-mongodb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/PKG-INFO` & `fastapi-crudrouter-mongodb-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: pierre@duveau.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -49,98 +49,104 @@
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id (for previous versions of Pydantic) : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
+- For Pydantic v2 : [Stackoverflow](https://stackoverflow.com/questions/76686267/what-is-the-new-way-to-declare-mongo-objectid-with-pydantic-v2-0)
 
 ---
 
-Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
+Are you exhausted from constantly rewriting basic CRUD routes? Do you find yourself needing to swiftly prototype features for presentations or hackathons? Well, rejoice! Introducing  [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/), your ultimate solution.
+
+As a complement to FastAPI's APIRouter, the [FastAPI](https://fastapi.tiangolo.com/) CRUDRouter for MongoDB 🌱 takes care of the heavy lifting for you. It automatically generates and documents your CRUD routes with minimal effort. Simply provide your model and your database connection, and you're good to go!
 
-As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
-generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
-```bash
-pip install fastapi-crudrouter-mongodb
+---
+
+
+```
+ pip install fastapi-crudrouter-mongodb
 ```
 
+
 ## Basic Usage
 
-I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
+---
+
+I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb :seedling:.
 
-```python
-from datetime import datetime
-from typing import List, Optional, Union
+```py linenums="1"
+from typing import Annotated
 from fastapi import FastAPI
-from pydantic import Field
-from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
+from fastapi_crudrouter_mongodb import (
+    ObjectId,
+    MongoObjectId,
+    MongoModel,
+    CRUDRouter,
+)
 import motor.motor_asyncio
 
-
 # Database connection using motor
-client = motor.motor_asyncio.AsyncIOMotorClient(
-    "mongodb://localhost:27017/local")
+client = motor.motor_asyncio.AsyncIOMotorClient("mongodb://localhost:27017/local")
 
+# store the database in a global variable
 db = client.local
 
-# Models
-class MessageModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    message: str
-    user_id: MongoObjectId
-    created_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    updated_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-
-class AddressModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    street: str
-    city: str
-    state: str
-    zip: str
-
+# Database Model
 class UserModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
+    id: Annotated[ObjectId, MongoObjectId] | None = None
     name: str
     email: str
-    addresses: Optional[List[AddressModel]]
-    messages: Optional[Union[List[MessageModel], MessageModel]] = None
+    password: str
 
 
 # Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
-messages_lookup = CRUDLookup(
-        model=MessageModel,
-        collection_name="messages",
-        prefix="messages",
-        local_field="_id",
-        foreign_field="user_id"
-    )
 
-users_controller = CRUDRouter(
+users_router = CRUDRouter(
     model=UserModel,
     db=db,
     collection_name="users",
-    lookups=[messages_lookup],
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
-app.include_router(users_controller)
+app.include_router(users_router)
 ```
 
+## Advanced Usage
+
+fastapi-crudrouter-mongodb offers several functionalities designed to maximize the benefits of your auto-generated CRUD routes. Here are some key highlights:
+
+- Automatic Lookups 
+- Automatic Embeds
+- Ability to provide **Custom** out schema
+- Ability to **Disable** specific routes
+- Ability to **Add custom dependencies** to specific routes
+
+
 ## OpenAPI Support
 
-By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
+---
+
+### "Automatic OpenAPI Documentation"
+
+>By default, the CRUDRouter automatically documents all generated routes in accordance with the OpenAPI specification.
+
+The default routes generated by the CRUDRouter are displayed in the OpenAPI documentation generated by the system.
+
+![CRUDRouter OpenAPI schema](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example.png)
+
 
-Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
+The CRUDRouter can dynamically generate comprehensive documentation based on the provided models.
 
-![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
+![CRUDRouter OpenAPI schema details](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example-details.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.1.0/README.md` & `fastapi-crudrouter-mongodb-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -17,96 +17,102 @@
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id (for previous versions of Pydantic) : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
+- For Pydantic v2 : [Stackoverflow](https://stackoverflow.com/questions/76686267/what-is-the-new-way-to-declare-mongo-objectid-with-pydantic-v2-0)
 
 ---
 
-Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
+Are you exhausted from constantly rewriting basic CRUD routes? Do you find yourself needing to swiftly prototype features for presentations or hackathons? Well, rejoice! Introducing  [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/), your ultimate solution.
+
+As a complement to FastAPI's APIRouter, the [FastAPI](https://fastapi.tiangolo.com/) CRUDRouter for MongoDB 🌱 takes care of the heavy lifting for you. It automatically generates and documents your CRUD routes with minimal effort. Simply provide your model and your database connection, and you're good to go!
 
-As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
-generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
-```bash
-pip install fastapi-crudrouter-mongodb
+---
+
+
+```
+ pip install fastapi-crudrouter-mongodb
 ```
 
+
 ## Basic Usage
 
-I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
+---
+
+I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb :seedling:.
 
-```python
-from datetime import datetime
-from typing import List, Optional, Union
+```py linenums="1"
+from typing import Annotated
 from fastapi import FastAPI
-from pydantic import Field
-from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
+from fastapi_crudrouter_mongodb import (
+    ObjectId,
+    MongoObjectId,
+    MongoModel,
+    CRUDRouter,
+)
 import motor.motor_asyncio
 
-
 # Database connection using motor
-client = motor.motor_asyncio.AsyncIOMotorClient(
-    "mongodb://localhost:27017/local")
+client = motor.motor_asyncio.AsyncIOMotorClient("mongodb://localhost:27017/local")
 
+# store the database in a global variable
 db = client.local
 
-# Models
-class MessageModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    message: str
-    user_id: MongoObjectId
-    created_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    updated_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-
-class AddressModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    street: str
-    city: str
-    state: str
-    zip: str
-
+# Database Model
 class UserModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
+    id: Annotated[ObjectId, MongoObjectId] | None = None
     name: str
     email: str
-    addresses: Optional[List[AddressModel]]
-    messages: Optional[Union[List[MessageModel], MessageModel]] = None
+    password: str
 
 
 # Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
-messages_lookup = CRUDLookup(
-        model=MessageModel,
-        collection_name="messages",
-        prefix="messages",
-        local_field="_id",
-        foreign_field="user_id"
-    )
 
-users_controller = CRUDRouter(
+users_router = CRUDRouter(
     model=UserModel,
     db=db,
     collection_name="users",
-    lookups=[messages_lookup],
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
-app.include_router(users_controller)
+app.include_router(users_router)
 ```
 
+## Advanced Usage
+
+fastapi-crudrouter-mongodb offers several functionalities designed to maximize the benefits of your auto-generated CRUD routes. Here are some key highlights:
+
+- Automatic Lookups 
+- Automatic Embeds
+- Ability to provide **Custom** out schema
+- Ability to **Disable** specific routes
+- Ability to **Add custom dependencies** to specific routes
+
+
 ## OpenAPI Support
 
-By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
+---
+
+### "Automatic OpenAPI Documentation"
+
+>By default, the CRUDRouter automatically documents all generated routes in accordance with the OpenAPI specification.
+
+The default routes generated by the CRUDRouter are displayed in the OpenAPI documentation generated by the system.
+
+![CRUDRouter OpenAPI schema](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example.png)
+
 
-Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
+The CRUDRouter can dynamically generate comprehensive documentation based on the provided models.
 
-![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
+![CRUDRouter OpenAPI schema details](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example-details.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/PKG-INFO` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: pierre@duveau.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -49,98 +49,104 @@
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id (for previous versions of Pydantic) : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
+- For Pydantic v2 : [Stackoverflow](https://stackoverflow.com/questions/76686267/what-is-the-new-way-to-declare-mongo-objectid-with-pydantic-v2-0)
 
 ---
 
-Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
+Are you exhausted from constantly rewriting basic CRUD routes? Do you find yourself needing to swiftly prototype features for presentations or hackathons? Well, rejoice! Introducing  [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/), your ultimate solution.
+
+As a complement to FastAPI's APIRouter, the [FastAPI](https://fastapi.tiangolo.com/) CRUDRouter for MongoDB 🌱 takes care of the heavy lifting for you. It automatically generates and documents your CRUD routes with minimal effort. Simply provide your model and your database connection, and you're good to go!
 
-As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
-generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
-```bash
-pip install fastapi-crudrouter-mongodb
+---
+
+
+```
+ pip install fastapi-crudrouter-mongodb
 ```
 
+
 ## Basic Usage
 
-I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
+---
+
+I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb :seedling:.
 
-```python
-from datetime import datetime
-from typing import List, Optional, Union
+```py linenums="1"
+from typing import Annotated
 from fastapi import FastAPI
-from pydantic import Field
-from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
+from fastapi_crudrouter_mongodb import (
+    ObjectId,
+    MongoObjectId,
+    MongoModel,
+    CRUDRouter,
+)
 import motor.motor_asyncio
 
-
 # Database connection using motor
-client = motor.motor_asyncio.AsyncIOMotorClient(
-    "mongodb://localhost:27017/local")
+client = motor.motor_asyncio.AsyncIOMotorClient("mongodb://localhost:27017/local")
 
+# store the database in a global variable
 db = client.local
 
-# Models
-class MessageModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    message: str
-    user_id: MongoObjectId
-    created_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    updated_at: Optional[str] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-
-class AddressModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
-    street: str
-    city: str
-    state: str
-    zip: str
-
+# Database Model
 class UserModel(MongoModel):
-    id: Optional[MongoObjectId] = Field()
+    id: Annotated[ObjectId, MongoObjectId] | None = None
     name: str
     email: str
-    addresses: Optional[List[AddressModel]]
-    messages: Optional[Union[List[MessageModel], MessageModel]] = None
+    password: str
 
 
 # Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
-messages_lookup = CRUDLookup(
-        model=MessageModel,
-        collection_name="messages",
-        prefix="messages",
-        local_field="_id",
-        foreign_field="user_id"
-    )
 
-users_controller = CRUDRouter(
+users_router = CRUDRouter(
     model=UserModel,
     db=db,
     collection_name="users",
-    lookups=[messages_lookup],
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
-app.include_router(users_controller)
+app.include_router(users_router)
 ```
 
+## Advanced Usage
+
+fastapi-crudrouter-mongodb offers several functionalities designed to maximize the benefits of your auto-generated CRUD routes. Here are some key highlights:
+
+- Automatic Lookups 
+- Automatic Embeds
+- Ability to provide **Custom** out schema
+- Ability to **Disable** specific routes
+- Ability to **Add custom dependencies** to specific routes
+
+
 ## OpenAPI Support
 
-By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
+---
+
+### "Automatic OpenAPI Documentation"
+
+>By default, the CRUDRouter automatically documents all generated routes in accordance with the OpenAPI specification.
+
+The default routes generated by the CRUDRouter are displayed in the OpenAPI documentation generated by the system.
+
+![CRUDRouter OpenAPI schema](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example.png)
+
 
-Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
+The CRUDRouter can dynamically generate comprehensive documentation based on the provided models.
 
-![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
+![CRUDRouter OpenAPI schema details](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/assets/img/openapi-basic-example-details.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.1.0/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt` & `fastapi-crudrouter-mongodb-0.1.1/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.1.0/setup.py` & `fastapi-crudrouter-mongodb-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fastapi-crudrouter-mongodb",
-    version="0.1.0",
+    version="0.1.1",
     author="Pierre DUVEAU",
     author_email="pierre@duveau.org",
     description="A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pierrod/fastapi-crudrouter-mongodb",
     packages=find_packages(),
```

