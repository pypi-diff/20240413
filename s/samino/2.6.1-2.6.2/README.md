# Comparing `tmp/samino-2.6.1.tar.gz` & `tmp/samino-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samino-2.6.1.tar", last modified: Fri Apr 12 22:12:38 2024, max compression
+gzip compressed data, was "samino-2.6.2.tar", last modified: Fri Apr 12 22:21:14 2024, max compression
```

## Comparing `samino-2.6.1.tar` & `samino-2.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-12 22:12:28.000000 samino-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:12:38.091244 samino-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 22:12:28.000000 samino-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/SAsync/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/acm.py
--rw-r--r--   0 runner    (1001) docker     (127)    40417 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.087244 samino-2.6.1/samino/SAsync/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)   198118 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    55364 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-12 22:12:28.000000 samino-2.6.1/samino/SAsync/sockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 22:12:28.000000 samino-2.6.1/samino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-12 22:12:28.000000 samino-2.6.1/samino/acm.py
--rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-04-12 22:12:28.000000 samino-2.6.1/samino/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/samino/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)   197370 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 22:12:28.000000 samino-2.6.1/samino/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    45027 2024-04-12 22:12:28.000000 samino-2.6.1/samino/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-04-12 22:12:28.000000 samino-2.6.1/samino/sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:38.091244 samino-2.6.1/samino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:12:38.000000 samino-2.6.1/samino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:12:38.091244 samino-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 22:12:28.000000 samino-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.053086 samino-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-12 22:21:04.000000 samino-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:21:14.053086 samino-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 22:21:04.000000 samino-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.049086 samino-2.6.2/samino/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.049086 samino-2.6.2/samino/SAsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/acm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40417 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.053086 samino-2.6.2/samino/SAsync/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/lib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/lib/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198118 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/lib/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55364 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-12 22:21:04.000000 samino-2.6.2/samino/SAsync/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 22:21:04.000000 samino-2.6.2/samino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-12 22:21:04.000000 samino-2.6.2/samino/acm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-04-12 22:21:04.000000 samino-2.6.2/samino/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.053086 samino-2.6.2/samino/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196643 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 22:21:04.000000 samino-2.6.2/samino/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45027 2024-04-12 22:21:04.000000 samino-2.6.2/samino/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-04-12 22:21:04.000000 samino-2.6.2/samino/sockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:21:14.053086 samino-2.6.2/samino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:21:14.000000 samino-2.6.2/samino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 22:21:14.000000 samino-2.6.2/samino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:21:14.000000 samino-2.6.2/samino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 22:21:14.000000 samino-2.6.2/samino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:21:14.000000 samino-2.6.2/samino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:21:14.053086 samino-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 22:21:04.000000 samino-2.6.2/setup.py
```

### Comparing `samino-2.6.1/LICENSE` & `samino-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/PKG-INFO` & `samino-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samino
-Version: 2.6.1
+Version: 2.6.2
 Summary: Amino Bots with python!
 Home-page: https://github.com/SirLez/SAmino
 Download-URL: https://github.com/SirLez/SAmino/archive/refs/heads/main.zip
 Author: SirLez
 Author-email: botsirlez@gmail.com
 License: MIT
 Keywords: api,python,python3,python3.x,SirLez,Bovonos,Amino,samino,samino pyS-Amino,samino,samino,samino-bot,samino-bots,samino-bot,ndc,narvii.apps,aminoapps,samino-py,samino,samino-bot,narvii
```

### Comparing `samino-2.6.1/README.md` & `samino-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/acm.py` & `samino-2.6.2/samino/SAsync/acm.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/client.py` & `samino-2.6.2/samino/SAsync/client.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/lib/exception.py` & `samino-2.6.2/samino/SAsync/lib/exception.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/lib/headers.py` & `samino-2.6.2/samino/SAsync/lib/headers.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/lib/objects.py` & `samino-2.6.2/samino/SAsync/lib/objects.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/lib/util.py` & `samino-2.6.2/samino/SAsync/lib/util.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/local.py` & `samino-2.6.2/samino/SAsync/local.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/SAsync/sockets.py` & `samino-2.6.2/samino/SAsync/sockets.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/acm.py` & `samino-2.6.2/samino/acm.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/client.py` & `samino-2.6.2/samino/client.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/lib/exception.py` & `samino-2.6.2/samino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/lib/headers.py` & `samino-2.6.2/samino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/lib/objects.py` & `samino-2.6.2/samino/lib/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1789,34 +1789,14 @@
             try: self.objectDeeplinkUrl.append(x["extData"]["objectDeeplinkUrl"])
             except (KeyError, TypeError): self.objectDeeplinkUrl.append(None)
             try: self.sourceIp.append(x["extData"]["sourceIp"])
             except (KeyError, TypeError): self.sourceIp.append(None)
 
         return self
 
-class UserAchievements:
-    def __init__(self, data):
-        self.json = data
-        self.secondsSpentOfLast24Hours = None
-        self.secondsSpentOfLast7Days = None
-        self.numberOfFollowersCount = None
-        self.numberOfPostsCreated = None
-
-    @property
-    def UserAchievements(self):
-        try: self.secondsSpentOfLast24Hours = self.json["secondsSpentOfLast24Hours"]
-        except (KeyError, TypeError): pass
-        try: self.secondsSpentOfLast7Days = self.json["secondsSpentOfLast7Days"]
-        except (KeyError, TypeError): pass
-        try: self.numberOfFollowersCount = self.json["numberOfMembersCount"]
-        except (KeyError, TypeError): pass
-        try: self.numberOfPostsCreated = self.json["numberOfPostsCreated"]
-        except (KeyError, TypeError): pass
-
-        return self
 
 class UserSavedBlogs:
     def __init__(self, data):
         _object = []
 
         self.json = data
 
@@ -4336,18 +4316,19 @@
         self.duration = data.get("api:duration")
         self.timestamp = data.get("api:timestamp")
 
 
 class Achievements:
     def __init__(self, data):
         self.json = data
-        self.secondsSpentOfLast24Hours = data.get("secondsSpentOfLast24Hours")
-        self.secondsSpentOfLast7Days = data.get("secondsSpentOfLast7Days")
-        self.numberOfPostsCreated = data.get("numberOfPostsCreated")
-        self.numberOfMembersCount = data.get("numberOfMembersCount")
+        achievements = data.get("achievements", {})
+        self.secondsSpentOfLast24Hours = achievements.get("secondsSpentOfLast24Hours")
+        self.secondsSpentOfLast7Days = achievements.get("secondsSpentOfLast7Days")
+        self.numberOfPostsCreated = achievements.get("numberOfPostsCreated")
+        self.numberOfMembersCount = achievements.get("numberOfMembersCount")
 
 
 class ReplyMessage:
     def __init__(self, data):
         self.messageId = data.get("messageId")
         self.content = data.get("content")
         self.clientRefId = data.get("clientRefId")
```

### Comparing `samino-2.6.1/samino/lib/sessions.py` & `samino-2.6.2/samino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/lib/util.py` & `samino-2.6.2/samino/lib/util.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/local.py` & `samino-2.6.2/samino/local.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino/sockets.py` & `samino-2.6.2/samino/sockets.py`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/samino.egg-info/PKG-INFO` & `samino-2.6.2/samino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samino
-Version: 2.6.1
+Version: 2.6.2
 Summary: Amino Bots with python!
 Home-page: https://github.com/SirLez/SAmino
 Download-URL: https://github.com/SirLez/SAmino/archive/refs/heads/main.zip
 Author: SirLez
 Author-email: botsirlez@gmail.com
 License: MIT
 Keywords: api,python,python3,python3.x,SirLez,Bovonos,Amino,samino,samino pyS-Amino,samino,samino,samino-bot,samino-bots,samino-bot,ndc,narvii.apps,aminoapps,samino-py,samino,samino-bot,narvii
```

### Comparing `samino-2.6.1/samino.egg-info/SOURCES.txt` & `samino-2.6.2/samino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `samino-2.6.1/setup.py` & `samino-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="samino",
-    version="2.6.1",
+    version="2.6.2",
     url="https://github.com/SirLez/SAmino",
     download_url="https://github.com/SirLez/SAmino/archive/refs/heads/main.zip",
     description="Amino Bots with python!",
     long_description=README,
     long_description_content_type="text/markdown",
     author="SirLez",
     author_email="botsirlez@gmail.com",
```

