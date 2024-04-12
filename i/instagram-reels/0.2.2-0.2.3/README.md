# Comparing `tmp/instagram_reels-0.2.2.tar.gz` & `tmp/instagram_reels-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_reels-0.2.2.tar", max compression
+gzip compressed data, was "instagram_reels-0.2.3.tar", max compression
```

## Comparing `instagram_reels-0.2.2.tar` & `instagram_reels-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1090 2024-02-24 03:05:17.828838 instagram_reels-0.2.2/LICENSE
--rw-r--r--   0        0        0     1798 2024-02-29 05:23:02.292536 instagram_reels-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-02-29 05:24:00.029750 instagram_reels-0.2.2/instagram_reels/__init__.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/__init__.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/__init__.py
--rw-r--r--   0        0        0      947 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/client/MediaInfoClient.py
--rw-r--r--   0        0        0     2832 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/client/ReelsClient.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/client/__init__.py
--rw-r--r--   0        0        0     2317 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/parser/MediaInfoParser.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/parser/__init__.py
--rw-r--r--   0        0        0      957 2024-02-24 02:39:11.040861 instagram_reels-0.2.2/instagram_reels/api/private/service/MediaInfoService.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/private/service/__init__.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/__init__.py
--rw-r--r--   0        0        0     4550 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/client/MediaInfoClient.py
--rw-r--r--   0        0        0      665 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/client/ReelsClient.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/client/__init__.py
--rw-r--r--   0        0        0      233 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/model/InstagramSettingDataClass.py
--rw-r--r--   0        0        0      249 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/model/InstagramSettingsParamsDataClass.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/model/__init__.py
--rw-r--r--   0        0        0     2066 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/parser/MediaInfoParser.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/parser/__init__.py
--rw-r--r--   0        0        0      613 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/service/CrossSiteRequestTokenService.py
--rw-r--r--   0        0        0      563 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/service/DynamicTokenService.py
--rw-r--r--   0        0        0     6607 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/service/InstagramApiParamsService.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/service/__init__.py
--rw-r--r--   0        0        0     1540 2024-02-24 02:39:11.044862 instagram_reels-0.2.2/instagram_reels/api/public/util/BitMapUtil.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/api/public/util/__init__.py
--rw-r--r--   0        0        0      261 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/IReelsClient.py
--rw-r--r--   0        0        0      185 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/JsonParser.py
--rw-r--r--   0        0        0      118 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/__init__.py
--rw-r--r--   0        0        0      352 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/InstagramShortUser.py
--rw-r--r--   0        0        0      258 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/ReelAuthor.py
--rw-r--r--   0        0        0      500 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/ReelModel.py
--rw-r--r--   0        0        0      225 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/ReelPreview.py
--rw-r--r--   0        0        0      241 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/ReelVideo.py
--rw-r--r--   0        0        0      114 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/common/model/__init__.py
--rw-r--r--   0        0        0      251 2024-02-29 05:23:02.296537 instagram_reels-0.2.2/instagram_reels/main/InstagramAPIClient.py
--rw-r--r--   0        0        0     1380 2024-02-29 05:23:02.296537 instagram_reels-0.2.2/instagram_reels/main/InstagramAPIClientImpl.py
--rw-r--r--   0        0        0        0 2024-02-29 05:24:00.037750 instagram_reels-0.2.2/instagram_reels/main/__init__.py
--rw-r--r--   0        0        0      112 2024-02-24 02:39:11.048862 instagram_reels-0.2.2/instagram_reels/reels/__init__.py
--rw-r--r--   0        0        0      823 2024-02-29 05:23:02.296537 instagram_reels-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 instagram_reels-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-02-24 03:05:17.828838 instagram_reels-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1798 2024-02-29 05:23:02.292536 instagram_reels-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 22:37:36.700610 instagram_reels-0.2.3/instagram_reels/__init__.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/__init__.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/__init__.py
+-rw-r--r--   0        0        0      947 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/client/MediaInfoClient.py
+-rw-r--r--   0        0        0     2832 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/client/ReelsClient.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/client/__init__.py
+-rw-r--r--   0        0        0     2317 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/parser/MediaInfoParser.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/parser/__init__.py
+-rw-r--r--   0        0        0      957 2024-02-24 02:39:11.040861 instagram_reels-0.2.3/instagram_reels/api/private/service/MediaInfoService.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/private/service/__init__.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/__init__.py
+-rw-r--r--   0        0        0     4550 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/client/MediaInfoClient.py
+-rw-r--r--   0        0        0      665 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/client/ReelsClient.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/client/__init__.py
+-rw-r--r--   0        0        0      233 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/model/InstagramSettingDataClass.py
+-rw-r--r--   0        0        0      249 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/model/InstagramSettingsParamsDataClass.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/model/__init__.py
+-rw-r--r--   0        0        0     2157 2024-04-12 22:36:40.163456 instagram_reels-0.2.3/instagram_reels/api/public/parser/MediaInfoParser.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/parser/__init__.py
+-rw-r--r--   0        0        0      613 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/service/CrossSiteRequestTokenService.py
+-rw-r--r--   0        0        0      563 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/service/DynamicTokenService.py
+-rw-r--r--   0        0        0     6607 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/service/InstagramApiParamsService.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/service/__init__.py
+-rw-r--r--   0        0        0     1540 2024-02-24 02:39:11.044862 instagram_reels-0.2.3/instagram_reels/api/public/util/BitMapUtil.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/api/public/util/__init__.py
+-rw-r--r--   0        0        0      261 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/IReelsClient.py
+-rw-r--r--   0        0        0      185 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/JsonParser.py
+-rw-r--r--   0        0        0      118 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/InstagramShortUser.py
+-rw-r--r--   0        0        0      258 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/ReelAuthor.py
+-rw-r--r--   0        0        0      500 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/ReelModel.py
+-rw-r--r--   0        0        0      225 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/ReelPreview.py
+-rw-r--r--   0        0        0      241 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/ReelVideo.py
+-rw-r--r--   0        0        0      114 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/common/model/__init__.py
+-rw-r--r--   0        0        0      251 2024-02-29 05:23:02.296537 instagram_reels-0.2.3/instagram_reels/main/InstagramAPIClient.py
+-rw-r--r--   0        0        0     1380 2024-02-29 05:23:02.296537 instagram_reels-0.2.3/instagram_reels/main/InstagramAPIClientImpl.py
+-rw-r--r--   0        0        0        0 2024-04-12 22:37:36.708611 instagram_reels-0.2.3/instagram_reels/main/__init__.py
+-rw-r--r--   0        0        0      112 2024-02-24 02:39:11.048862 instagram_reels-0.2.3/instagram_reels/reels/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-12 22:36:40.163456 instagram_reels-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 instagram_reels-0.2.3/PKG-INFO
```

### Comparing `instagram_reels-0.2.2/LICENSE` & `instagram_reels-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/README.md` & `instagram_reels-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/private/client/MediaInfoClient.py` & `instagram_reels-0.2.3/instagram_reels/api/private/client/MediaInfoClient.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/private/client/ReelsClient.py` & `instagram_reels-0.2.3/instagram_reels/api/private/client/ReelsClient.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/private/parser/MediaInfoParser.py` & `instagram_reels-0.2.3/instagram_reels/api/private/parser/MediaInfoParser.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/private/service/MediaInfoService.py` & `instagram_reels-0.2.3/instagram_reels/api/private/service/MediaInfoService.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/client/MediaInfoClient.py` & `instagram_reels-0.2.3/instagram_reels/api/public/client/MediaInfoClient.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/client/ReelsClient.py` & `instagram_reels-0.2.3/instagram_reels/api/public/client/ReelsClient.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/parser/MediaInfoParser.py` & `instagram_reels-0.2.3/instagram_reels/api/public/parser/MediaInfoParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         try:
             content: dict = json.loads(raw_json).get("data").get("xdt_shortcode_media")
         except JSONDecodeError as e:
             raise Exception(f"Error on parse json from instagram web api. Exception: {e}")
         return ReelModel(
             media_id=content.get("id"),
             code=content.get("shortcode"),
-            description=content.get("edge_media_to_caption").get("edges")[0].get("node").get("text"),
+            description="" if content.get("edge_media_to_caption", {}).get("edges", []) == [] else content.get("edge_media_to_caption", {}).get("edges", [])[0].get("node", {}).get("text", ""),
             duration=content.get("video_duration"),
             like_count=content["edge_media_preview_like"]["count"],
             view_count=content["video_view_count"],
             play_count=content["video_play_count"],
             author=ReelAuthor(
                 user_id=content["owner"]["id"],
                 username=content["owner"]["username"],
```

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/service/CrossSiteRequestTokenService.py` & `instagram_reels-0.2.3/instagram_reels/api/public/service/CrossSiteRequestTokenService.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/service/DynamicTokenService.py` & `instagram_reels-0.2.3/instagram_reels/api/public/service/DynamicTokenService.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/service/InstagramApiParamsService.py` & `instagram_reels-0.2.3/instagram_reels/api/public/service/InstagramApiParamsService.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/api/public/util/BitMapUtil.py` & `instagram_reels-0.2.3/instagram_reels/api/public/util/BitMapUtil.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/instagram_reels/main/InstagramAPIClientImpl.py` & `instagram_reels-0.2.3/instagram_reels/main/InstagramAPIClientImpl.py`

 * *Files identical despite different names*

### Comparing `instagram_reels-0.2.2/pyproject.toml` & `instagram_reels-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instagram-reels"
-version = "0.2.2"
+version = "0.2.3"
 description = "Instagram Reels Downloader"
 authors = ["Николай Витальевич Никоноров <nnv@bitt.moe>"]
 readme = "README.md"
 packages = [{include = "instagram_reels"}]
 repository = "https://gitlab.com/bitt_moe/instagram/reels_downloader"
 
 [tool.poetry.dependencies]
```

### Comparing `instagram_reels-0.2.2/PKG-INFO` & `instagram_reels-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-reels
-Version: 0.2.2
+Version: 0.2.3
 Summary: Instagram Reels Downloader
 Home-page: https://gitlab.com/bitt_moe/instagram/reels_downloader
 Author: Николай Витальевич Никоноров
 Author-email: nnv@bitt.moe
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

