# Comparing `tmp/davtelepot-2.9.8.tar.gz` & `tmp/davtelepot-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davtelepot-2.9.8.tar", last modified: Sun Dec 17 09:22:29 2023, max compression
+gzip compressed data, was "davtelepot-2.9.9.tar", last modified: Wed Feb 14 18:32:27 2024, max compression
```

## Comparing `davtelepot-2.9.8.tar` & `davtelepot-2.9.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/
--rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.9.8/LICENSE
--rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.9.8/MANIFEST.in
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-12-17 09:22:29.191687 davtelepot-2.9.8/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.9.8/README.md
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/davtelepot/
--rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-12-17 09:21:44.000000 davtelepot-2.9.8/davtelepot/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-08-07 18:19:33.000000 davtelepot-2.9.8/davtelepot/__main__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    73001 2023-08-07 18:19:33.000000 davtelepot-2.9.8/davtelepot/administration_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   112800 2023-11-12 10:56:16.000000 davtelepot-2.9.8/davtelepot/api.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-01-06 09:30:24.000000 davtelepot-2.9.8/davtelepot/api_helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.9.8/davtelepot/authorization.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-08-07 18:19:33.000000 davtelepot-2.9.8/davtelepot/bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     8393 2023-08-07 18:19:33.000000 davtelepot-2.9.8/davtelepot/cli.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/davtelepot/data/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.9.8/davtelepot/data/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.9.8/davtelepot/database.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.9.8/davtelepot/helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.9.8/davtelepot/ietf_language_tags.csv
--rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.9.8/davtelepot/languages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    48464 2023-08-07 18:19:33.000000 davtelepot-2.9.8/davtelepot/messages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.9.8/davtelepot/suggestions.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/davtelepot/tools/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.9.8/davtelepot/tools/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.9.8/davtelepot/tools/merge_files.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.9.8/davtelepot/useful_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    51146 2023-12-17 09:20:20.000000 davtelepot-2.9.8/davtelepot/utilities.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/davtelepot.egg-info/
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-12-17 09:22:29.000000 davtelepot-2.9.8/davtelepot.egg-info/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-12-17 09:22:29.000000 davtelepot-2.9.8/davtelepot.egg-info/SOURCES.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-12-17 09:22:29.000000 davtelepot-2.9.8/davtelepot.egg-info/dependency_links.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-12-17 09:22:29.000000 davtelepot-2.9.8/davtelepot.egg-info/requires.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-12-17 09:22:29.000000 davtelepot-2.9.8/davtelepot.egg-info/top_level.txt
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-12-17 09:22:29.191687 davtelepot-2.9.8/examples/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.9.8/examples/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.9.8/examples/a_simple_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.9.8/examples/more_bots_together.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.9.8/examples/webhook_powered_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-12-17 09:22:29.191687 davtelepot-2.9.8/setup.cfg
--rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.9.8/setup.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.082665 davtelepot-2.9.9/
+-rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.9.9/LICENSE
+-rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.9.9/MANIFEST.in
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2024-02-14 18:32:27.078662 davtelepot-2.9.9/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.9.9/README.md
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.078662 davtelepot-2.9.9/davtelepot/
+-rw-rw-r--   0 davte     (1000) davte     (1000)      747 2024-02-14 18:31:20.000000 davtelepot-2.9.9/davtelepot/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-08-07 18:19:33.000000 davtelepot-2.9.9/davtelepot/__main__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    73001 2023-08-07 18:19:33.000000 davtelepot-2.9.9/davtelepot/administration_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   112800 2023-11-12 10:56:16.000000 davtelepot-2.9.9/davtelepot/api.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-01-06 09:30:24.000000 davtelepot-2.9.9/davtelepot/api_helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.9.9/davtelepot/authorization.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   143369 2024-02-14 18:31:20.000000 davtelepot-2.9.9/davtelepot/bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     8393 2023-08-07 18:19:33.000000 davtelepot-2.9.9/davtelepot/cli.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.078662 davtelepot-2.9.9/davtelepot/data/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.9.9/davtelepot/data/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.9.9/davtelepot/database.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.9.9/davtelepot/helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.9.9/davtelepot/ietf_language_tags.csv
+-rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.9.9/davtelepot/languages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    48464 2023-08-07 18:19:33.000000 davtelepot-2.9.9/davtelepot/messages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.9.9/davtelepot/suggestions.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.078662 davtelepot-2.9.9/davtelepot/tools/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.9.9/davtelepot/tools/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.9.9/davtelepot/tools/merge_files.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.9.9/davtelepot/useful_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    51146 2024-02-14 18:31:17.000000 davtelepot-2.9.9/davtelepot/utilities.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.078662 davtelepot-2.9.9/davtelepot.egg-info/
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2024-02-14 18:32:27.000000 davtelepot-2.9.9/davtelepot.egg-info/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)      795 2024-02-14 18:32:27.000000 davtelepot-2.9.9/davtelepot.egg-info/SOURCES.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)        1 2024-02-14 18:32:27.000000 davtelepot-2.9.9/davtelepot.egg-info/dependency_links.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2024-02-14 18:32:27.000000 davtelepot-2.9.9/davtelepot.egg-info/requires.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2024-02-14 18:32:27.000000 davtelepot-2.9.9/davtelepot.egg-info/top_level.txt
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2024-02-14 18:32:27.078662 davtelepot-2.9.9/examples/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.9.9/examples/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.9.9/examples/a_simple_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.9.9/examples/more_bots_together.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.9.9/examples/webhook_powered_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)       38 2024-02-14 18:32:27.082665 davtelepot-2.9.9/setup.cfg
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.9.9/setup.py
```

### Comparing `davtelepot-2.9.8/PKG-INFO` & `davtelepot-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.8
+Version: 2.9.9
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.8/README.md` & `davtelepot-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/__init__.py` & `davtelepot-2.9.9/davtelepot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ```
 """
 
 __author__ = "Davide Testa"
 __email__ = "davide@davte.it"
 __credits__ = ["Marco Origlia", "Nick Lee @Nickoala"]
 __license__ = "GNU General Public License v3.0"
-__version__ = "2.9.8"
+__version__ = "2.9.9"
 __maintainer__ = "Davide Testa"
 __contact__ = "t.me/davte"
 
 from davtelepot import (administration_tools, api, authorization,
                         bot, helper, languages, messages, suggestions,
                         useful_tools, utilities)
```

### Comparing `davtelepot-2.9.8/davtelepot/administration_tools.py` & `davtelepot-2.9.9/davtelepot/administration_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/api.py` & `davtelepot-2.9.9/davtelepot/api.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/api_helper.py` & `davtelepot-2.9.9/davtelepot/api_helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/authorization.py` & `davtelepot-2.9.9/davtelepot/authorization.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/bot.py` & `davtelepot-2.9.9/davtelepot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -2133,34 +2133,39 @@
         Telegram may not preserve the original file name and MIME type: the
             file's MIME type and name (if available) should be stored when the
             File object is received.
         """
         file = await self.getFile(file_id=file_id)
         if file is None or isinstance(file, Exception):
             logging.error(f"{file}")
-            return
+            return file
         file_bytes = await async_get(
             url=(
                 f"https://api.telegram.org/file/"
                 f"bot{self.token}/"
                 f"{file['file_path']}"
             ),
             mode='raw'
         )
         path = path or self.path
-        while file_name is None:
+        if file_name is None:
             file_name = get_secure_key(length=10)
-            if os.path.exists(f"{path}/{file_name}"):
-                file_name = None
+        file_complete_path = os.path.join(path, file_name)
+        while os.path.exists(file_complete_path):
+            file_complete_path = file_complete_path + '1'
         try:
-            with open(f"{path}/{file_name}", 'wb') as local_file:
+            with open(file_complete_path, 'wb') as local_file:
                 local_file.write(file_bytes)
         except Exception as e:
             logging.error(f"File download failed due to {e}")
-        return
+            return e
+        return dict(file_id=file_id,
+                    file_name=file_name,
+                    path=path,
+                    file_complete_path=file_complete_path)
 
     def translate_inline_query_answer_result(self, record,
                                              update=None, user_record=None):
         """Translate title and message text fields of inline query result.
 
         This method does not alter original `record`. This way, default
         inline query result is kept multilingual although single results
```

### Comparing `davtelepot-2.9.8/davtelepot/cli.py` & `davtelepot-2.9.9/davtelepot/cli.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/database.py` & `davtelepot-2.9.9/davtelepot/database.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/helper.py` & `davtelepot-2.9.9/davtelepot/helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/ietf_language_tags.csv` & `davtelepot-2.9.9/davtelepot/ietf_language_tags.csv`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/languages.py` & `davtelepot-2.9.9/davtelepot/languages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/messages.py` & `davtelepot-2.9.9/davtelepot/messages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/suggestions.py` & `davtelepot-2.9.9/davtelepot/suggestions.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/tools/merge_files.py` & `davtelepot-2.9.9/davtelepot/tools/merge_files.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/useful_tools.py` & `davtelepot-2.9.9/davtelepot/useful_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot/utilities.py` & `davtelepot-2.9.9/davtelepot/utilities.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/davtelepot.egg-info/PKG-INFO` & `davtelepot-2.9.9/davtelepot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.8
+Version: 2.9.9
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.8/davtelepot.egg-info/SOURCES.txt` & `davtelepot-2.9.9/davtelepot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/examples/a_simple_bot.py` & `davtelepot-2.9.9/examples/a_simple_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/examples/more_bots_together.py` & `davtelepot-2.9.9/examples/more_bots_together.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/examples/webhook_powered_bot.py` & `davtelepot-2.9.9/examples/webhook_powered_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.8/setup.py` & `davtelepot-2.9.9/setup.py`

 * *Files identical despite different names*

