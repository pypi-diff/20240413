# Comparing `tmp/samino-2.6.0.tar.gz` & `tmp/samino-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samino-2.6.0.tar", last modified: Sun Mar 31 18:21:27 2024, max compression
+gzip compressed data, was "samino-2.6.1.tar", last modified: Fri Apr 12 22:12:38 2024, max compression
```

## Comparing `samino-2.6.0.tar` & `samino-2.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.084529 samino-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-31 18:21:13.000000 samino-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-31 18:21:27.084529 samino-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-31 18:21:13.000000 samino-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.076529 samino-2.6.0/samino/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.080530 samino-2.6.0/samino/SAsync/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/acm.py
--rw-r--r--   0 runner    (1001) docker     (127)    40417 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.080530 samino-2.6.0/samino/SAsync/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/lib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/lib/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)   198118 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/lib/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    55364 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-03-31 18:21:13.000000 samino-2.6.0/samino/SAsync/sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-31 18:21:13.000000 samino-2.6.0/samino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-31 18:21:13.000000 samino-2.6.0/samino/acm.py
--rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-03-31 18:21:13.000000 samino-2.6.0/samino/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.080530 samino-2.6.0/samino/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)   198118 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-31 18:21:13.000000 samino-2.6.0/samino/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    44851 2024-03-31 18:21:13.000000 samino-2.6.0/samino/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-03-31 18:21:13.000000 samino-2.6.0/samino/sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:27.084529 samino-2.6.0/samino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-31 18:21:27.000000 samino-2.6.0/samino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-31 18:21:27.000000 samino-2.6.0/samino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:21:27.000000 samino-2.6.0/samino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 18:21:27.000000 samino-2.6.0/samino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 18:21:27.000000 samino-2.6.0/samino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:21:27.084529 samino-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-31 18:21:13.000000 samino-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-12 22:12:28.000000 samino-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:12:38.091244 samino-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 22:12:28.000000 samino-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/SAsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/acm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40417 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/SAsync/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198118 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55364 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 22:12:28.000000 samino-2.6.1/samino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-12 22:12:28.000000 samino-2.6.1/samino/acm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-04-12 22:12:28.000000 samino-2.6.1/samino/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/samino/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   197370 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45027 2024-04-12 22:12:28.000000 samino-2.6.1/samino/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-04-12 22:12:28.000000 samino-2.6.1/samino/sockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/samino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:12:38.091244 samino-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 22:12:28.000000 samino-2.6.1/setup.py
```

### Comparing `samino-2.6.0/LICENSE` & `samino-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/PKG-INFO` & `samino-2.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samino
-Version: 2.6.0
+Version: 2.6.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/SirLez/SAmino
 Download-URL: https://github.com/SirLez/SAmino/archive/refs/heads/main.zip
 Author: SirLez
 Author-email: botsirlez@gmail.com
 License: MIT
 Keywords: api,python,python3,python3.x,SirLez,Bovonos,Amino,samino,samino pyS-Amino,samino,samino,samino-bot,samino-bots,samino-bot,ndc,narvii.apps,aminoapps,samino-py,samino,samino-bot,narvii
```

### Comparing `samino-2.6.0/README.md` & `samino-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/acm.py` & `samino-2.6.1/samino/SAsync/acm.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/client.py` & `samino-2.6.1/samino/SAsync/client.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/lib/exception.py` & `samino-2.6.1/samino/SAsync/lib/exception.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/lib/headers.py` & `samino-2.6.1/samino/SAsync/lib/headers.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/lib/objects.py` & `samino-2.6.1/samino/SAsync/lib/objects.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/lib/util.py` & `samino-2.6.1/samino/SAsync/lib/util.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/local.py` & `samino-2.6.1/samino/SAsync/local.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/SAsync/sockets.py` & `samino-2.6.1/samino/SAsync/sockets.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/acm.py` & `samino-2.6.1/samino/acm.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/client.py` & `samino-2.6.1/samino/client.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/lib/exception.py` & `samino-2.6.1/samino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/lib/headers.py` & `samino-2.6.1/samino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/lib/objects.py` & `samino-2.6.1/samino/lib/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,15 @@
     @property
     def RecentBlogs(self):
         try: self.nextPageToken = self.json["paging"]["nextPageToken"]
         except (KeyError, TypeError): pass
         try: self.prevPageToken = self.json["paging"]["prevPageToken"]
         except (KeyError, TypeError): pass
 
-        return BlogList(self.json["blogList"], self.nextPageToken, self.prevPageToken).BlogList
+        return BlogList(self.json["blogList"] if "blogList" in self.json else self.json, self.nextPageToken, self.prevPageToken).BlogList
 
 class BlogCategoryList:
     def __init__(self, data):
         self.json = data
         self.status = []
         self.modifiedTime = []
         self.icon = []
@@ -4317,107 +4317,97 @@
 
 ##############################################
 
 
 class Login:
     def __init__(self, data):
         self.json = data
-        self.uid = data["auid"]
-        self.sid = data["sid"]
-        self.nickname = data["account"]["nickname"]
-        self.aminoId = data["account"]["aminoId"]
+        self.uid = data.get("auid")
+        self.sid = data.get("sid")
+        account_info = data.get("account", {})
+        self.nickname = account_info.get("nickname")
+        self.amino_id = account_info.get("aminoId")
+
 
 class Json:
     def __init__(self, data):
+        self.json_data = data
+        self.message = data.get("api:message")
+        self.status_code = data.get("api:statuscode")
+        self.duration = data.get("api:duration")
+        self.timestamp = data.get("api:timestamp")
+
+
+class Achievements:
+    def __init__(self, data):
         self.json = data
-        try:
-            self.message = data["api:message"]
-            self.statusCode = data["api:statuscode"]
-            self.duration = data["api:duration"]
-            self.timestamp = data["api:timestamp"]
-        except (TypeError, KeyError): pass
+        self.secondsSpentOfLast24Hours = data.get("secondsSpentOfLast24Hours")
+        self.secondsSpentOfLast7Days = data.get("secondsSpentOfLast7Days")
+        self.numberOfPostsCreated = data.get("numberOfPostsCreated")
+        self.numberOfMembersCount = data.get("numberOfMembersCount")
 
 
 class ReplyMessage:
     def __init__(self, data):
-        try: self.messageId = data["messageId"]
-        except KeyError: self.messageId = None
-        try: self.content = data["content"]
-        except KeyError: self.content = None
-        try:  self.clientRefId = data["clientRefId"]
-        except KeyError: self.clientRefId = None
-        try: self.author: UserProfile = UserProfile(data["author"])
-        except KeyError: self.author = None
-        try: self.replyMessage: ReplyMessage = ReplyMessage(data["extensions"]["replyMessage"])
-        except KeyError: self.replyMessage = None
+        self.messageId = data.get("messageId")
+        self.content = data.get("content")
+        self.clientRefId = data.get("clientRefId")
+        self.author = UserProfile(data.get("author")) if "author" in data else None
+        self.replyMessage = (
+            ReplyMessage(data["extensions"]["replyMessage"])
+            if "extensions" in data and "replyMessage" in data["extensions"]
+            else None
+        )
 
 
 class BubbleTemplates:
     def __init__(self, data):
         self.json = data
-        self.templateId = []
-        self.materialUrl = []
-        self.name = []
-        for x in data:
-            try: self.templateId.append(x["templateId"])
-            except (KeyError): self.templateId.append(None)
-            try: self.materialUrl.append(x["materialUrl"])
-            except (KeyError): self.materialUrl.append(None)
-            try: self.name.append(x["name"])
-            except (KeyError): self.name.append(None)
-            try: self.config = BubbleConfig(x["config"])
-            except (KeyError): self.config = BubbleConfig({})
+        self.templateId = [x.get("templateId") for x in data]
+        self.materialUrl = [x.get("materialUrl") for x in data]
+        self.name = [x.get("name") for x in data]
+        self.config = [
+            BubbleConfig(x.get("config", {})) for x in data
+        ]
 
 
 class Account:
     def __init__(self, data):
         self.json = data
-
-        try: self.email = data["email"]
-        except (KeyError): self.email = None
-        try: self.icon = data["icon"]
-        except (KeyError): self.icon = None
-        try: self.nickname = data["nickname"]
-        except (KeyError): self.nickname = None
-        try: self.aminoId = data["aminoId"]
-        except (KeyError): self.aminoId = None
-        try: self.userId = data["uid"]
-        except (KeyError): self.userId = None
+        self.email = data.get("email")
+        self.icon = data.get("icon")
+        self.nickname = data.get("nickname")
+        self.aminoId = data.get("aminoId")
+        self.userId = data.get("uid")
 
 
 class ItemList:
     def __init__(self, data):
         self.json = data
-
         self.objectId = []
         self.imageUrl = []
         self.adCampaignId = []
         self.deepLink = []
         self.objectType = []
         self.scenarioType = []
         self.reqId = []
         self.adUnitId = []
         self.uiPos = []
 
-    @property
-    def ItemList(self):
+        self._populate_item_list()
+
+    def _populate_item_list(self):
         for x in self.json:
-            try: self.objectId.append(x["objectId"])
-            except (KeyError, TypeError): self.objectId.append(None)
-            try: self.imageUrl.append(x["imageUrl"])
-            except (KeyError, TypeError): self.imageUrl.append(None)
-            try: self.adCampaignId.append(x["adCampaignId"])
-            except (KeyError, TypeError): self.adCampaignId.append(None)
-            try: self.deepLink.append(x["deepLink"])
-            except (KeyError, TypeError): self.deepLink.append(None)
-            try: self.objectType.append(x["objectType"])
-            except (KeyError, TypeError): self.objectType.append(None)
-            try: self.scenarioType.append(x["strategyInfo"]["scenarioType"])
-            except (KeyError, TypeError): self.scenarioType.append(None)
-            try: self.reqId.append(x["strategyInfo"]["reqId"])
-            except (KeyError, TypeError): self.reqId.append(None)
-            try: self.uiPos.append(x["strategyInfo"]["uiPos"])
-            except (KeyError, TypeError): self.reqId.append(None)
-            try: self.adUnitId.append(x["strategyInfo"]["adUnitId"])
-            except (KeyError, TypeError): self.reqId.append(None)
+            self.objectId.append(x.get("objectId"))
+            self.imageUrl.append(x.get("imageUrl"))
+            self.adCampaignId.append(x.get("adCampaignId"))
+            self.deepLink.append(x.get("deepLink"))
+            self.objectType.append(x.get("objectType"))
+            strategy_info = x.get("strategyInfo", {})
+            self.scenarioType.append(strategy_info.get("scenarioType"))
+            self.reqId.append(strategy_info.get("reqId"))
+            self.uiPos.append(strategy_info.get("uiPos"))
+            self.adUnitId.append(strategy_info.get("adUnitId"))
 
+    @property
+    def ItemList(self):
         return self
```

### Comparing `samino-2.6.0/samino/lib/sessions.py` & `samino-2.6.1/samino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/lib/util.py` & `samino-2.6.1/samino/lib/util.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino/local.py` & `samino-2.6.1/samino/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,15 +1205,15 @@
             "/community/stats/web-user-active-time", data, webRequest=True
         )
 
     def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
         req = self.getRequest(
             f"/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
         )
-        return RecentBlogs(req["BlogList"]).RecentBlogs
+        return RecentBlogs(req["blogList"]).RecentBlogs
 
     def publish_to_featured(
             self,
             time: int,
             userId: str = None,
             chatId: str = None,
             blogId: str = None,
@@ -1268,7 +1268,13 @@
         elif chatId:
             endpoint = f"chat/thread/{chatId}"
         else:
             raise TypeError("Please Specify Object ID")
 
         req = self.postRequest(f"/x{self.comId}/s/{endpoint}/admin", data)
         return Json(req)
+
+    def get_achievements(self):
+        req = self.getRequest(
+            f"/x{self.comId}/s/user-profile/{self.uid}/achievements"
+        )
+        return Achievements(req)
```

### Comparing `samino-2.6.0/samino/sockets.py` & `samino-2.6.1/samino/sockets.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/samino.egg-info/PKG-INFO` & `samino-2.6.1/samino.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samino
-Version: 2.6.0
+Version: 2.6.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/SirLez/SAmino
 Download-URL: https://github.com/SirLez/SAmino/archive/refs/heads/main.zip
 Author: SirLez
 Author-email: botsirlez@gmail.com
 License: MIT
 Keywords: api,python,python3,python3.x,SirLez,Bovonos,Amino,samino,samino pyS-Amino,samino,samino,samino-bot,samino-bots,samino-bot,ndc,narvii.apps,aminoapps,samino-py,samino,samino-bot,narvii
```

### Comparing `samino-2.6.0/samino.egg-info/SOURCES.txt` & `samino-2.6.1/samino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `samino-2.6.0/setup.py` & `samino-2.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="samino",
-    version="2.6.0",
+    version="2.6.1",
     url="https://github.com/SirLez/SAmino",
     download_url="https://github.com/SirLez/SAmino/archive/refs/heads/main.zip",
     description="Amino Bots with python!",
     long_description=README,
     long_description_content_type="text/markdown",
     author="SirLez",
     author_email="botsirlez@gmail.com",
```

