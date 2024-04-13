# Comparing `tmp/free_bandcamp_downloader-0.1.6.tar.gz` & `tmp/free_bandcamp_downloader-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_bandcamp_downloader-0.1.6.tar", max compression
+gzip compressed data, was "free_bandcamp_downloader-0.1.7.tar", max compression
```

## Comparing `free_bandcamp_downloader-0.1.6.tar` & `free_bandcamp_downloader-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1666 2024-03-23 20:25:36.157679 free_bandcamp_downloader-0.1.6/README.md
--rw-r--r--   0        0        0      221 2024-03-23 20:25:36.157679 free_bandcamp_downloader-0.1.6/free_bandcamp_downloader/__init__.py
--rw-r--r--   0        0        0    15739 2024-03-23 20:25:36.157679 free_bandcamp_downloader-0.1.6/free_bandcamp_downloader/__main__.py
--rw-r--r--   0        0        0      567 2024-03-23 20:25:36.157679 free_bandcamp_downloader-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 free_bandcamp_downloader-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1666 2024-04-13 03:12:13.935622 free_bandcamp_downloader-0.1.7/README.md
+-rw-r--r--   0        0        0      221 2024-04-13 03:12:13.935622 free_bandcamp_downloader-0.1.7/free_bandcamp_downloader/__init__.py
+-rw-r--r--   0        0        0    16488 2024-04-13 03:12:13.935622 free_bandcamp_downloader-0.1.7/free_bandcamp_downloader/__main__.py
+-rw-r--r--   0        0        0      567 2024-04-13 03:12:13.935622 free_bandcamp_downloader-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 free_bandcamp_downloader-0.1.7/PKG-INFO
```

### Comparing `free_bandcamp_downloader-0.1.6/README.md` & `free_bandcamp_downloader-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `free_bandcamp_downloader-0.1.6/free_bandcamp_downloader/__main__.py` & `free_bandcamp_downloader-0.1.7/free_bandcamp_downloader/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,15 +231,33 @@
         album_data = self._get_album_data_from_soup(soup)
 
         logger.debug(f"Album data: {album_data}")
 
         tralbum_data = soup.find("script", {"data-tralbum": True}).attrs["data-tralbum"]
         tralbum_data = json.loads(tralbum_data)
 
-        if tralbum_data["current"]["minimum_price"] == 0:
+        if not tralbum_data["hasAudio"]:
+            raise BCFreeDownloadError(f"{url} has no audio. Skipping...")
+
+        head_data = soup.head.find("script", {"type": "application/ld+json"}, recursive=False).string
+        head_data = json.loads(head_data)
+        # track releases have this inAlbum key even if they're standalone
+        head_data = head_data.get("inAlbum", head_data)["albumRelease"]
+        # iterate through every additionalProperty of every albumRelease until we get
+        # the one that corresponds to the track release (t) or album release (a)
+        # physical releases are p, and discography offers are b, so this should be fine
+        head_data = next(obj for obj in head_data
+            if next(obj2["value"] for obj2 in obj["additionalProperty"]
+                if obj2["name"] == "item_type"
+            ) in ("t", "a")
+        )
+        if not "offers" in head_data:
+            raise BCFreeDownloadError(f"{url} has no digital download. Skipping...")
+
+        if head_data["offers"]["price"] == 0.0:
             if tralbum_data["current"]["require_email"]:
                 logger.info(f"{url} requires email")
                 email_post_url = urljoin(url, "/email_download")
                 r = self.session.post(
                     email_post_url,
                     data={
                         "encoding_name": "none",
@@ -253,19 +271,14 @@
                 r.raise_for_status()
                 r = r.json()
                 if not r["ok"]:
                     raise ValueError(f"Bad response when sending email address: {r}")
                 self.mail_album_data[url] = album_data
             else:
                 logger.info(f"{url} does not require email")
-                if not tralbum_data["freeDownloadPage"]:
-                    logger.warning(
-                        "Album has no download link (probably has no tracks). Skipping..."
-                    )
-                    return
                 self._download_file(
                     tralbum_data["freeDownloadPage"], self.options.format, album_data
                 )
         else:
             raise BCFreeDownloadError(f"{url} is not free")
 
     def download_label(self, url: str, force: bool = False):
```

### Comparing `free_bandcamp_downloader-0.1.6/pyproject.toml` & `free_bandcamp_downloader-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "free-bandcamp-downloader"
-version = "0.1.6"
+version = "0.1.7"
 description = "Download free and name-your-price albums from Bandcamp"
 authors = ["7x11x13 <x7x11x13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 bcdl-free = "free_bandcamp_downloader.__main__:main"
```

### Comparing `free_bandcamp_downloader-0.1.6/PKG-INFO` & `free_bandcamp_downloader-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: free-bandcamp-downloader
-Version: 0.1.6
+Version: 0.1.7
 Summary: Download free and name-your-price albums from Bandcamp
 License: MIT
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

