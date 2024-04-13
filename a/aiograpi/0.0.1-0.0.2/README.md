# Comparing `tmp/aiograpi-0.0.1.tar.gz` & `tmp/aiograpi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiograpi-0.0.1.tar", last modified: Tue Feb 27 15:15:52 2024, max compression
+gzip compressed data, was "aiograpi-0.0.2.tar", last modified: Sat Apr 13 15:16:39 2024, max compression
```

## Comparing `aiograpi-0.0.1.tar` & `aiograpi-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-02-27 15:15:52.016000 aiograpi-0.0.1/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1805 2024-02-27 15:15:52.015831 aiograpi-0.0.1/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)    10750 2024-02-27 14:37:36.000000 aiograpi-0.0.1/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-02-27 15:15:52.003894 aiograpi-0.0.1/aiograpi/
--rw-r--r--   0 adw0rd     (501) staff       (20)     3388 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2772 2024-02-27 14:43:44.000000 aiograpi-0.0.1/aiograpi/config.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6434 2024-01-10 02:33:51.000000 aiograpi-0.0.1/aiograpi/exceptions.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    17120 2024-01-29 15:44:23.000000 aiograpi-0.0.1/aiograpi/extractors.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-02-27 15:15:52.015151 aiograpi-0.0.1/aiograpi/mixins/
--rw-r--r--   0 adw0rd     (501) staff       (20)        0 2023-11-08 14:15:14.000000 aiograpi-0.0.1/aiograpi/mixins/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     7375 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/account.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10497 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/album.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    27054 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/auth.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1572 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/bloks.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    23109 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/mixins/challenge.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10755 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/clip.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6417 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/collection.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    18050 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/comment.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22262 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/direct.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3310 2024-02-27 14:43:44.000000 aiograpi-0.0.1/aiograpi/mixins/fbsearch.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8094 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/graphql.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    15850 2024-02-27 14:35:11.000000 aiograpi-0.0.1/aiograpi/mixins/hashtag.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8652 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/highlight.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10800 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/mixins/igtv.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     6375 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/insights.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16629 2024-02-27 14:35:11.000000 aiograpi-0.0.1/aiograpi/mixins/location.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    37689 2024-02-27 14:40:53.000000 aiograpi-0.0.1/aiograpi/mixins/media.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16756 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/mixins/notification.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2665 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/password.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22755 2024-02-27 14:45:02.000000 aiograpi-0.0.1/aiograpi/mixins/photo.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    24133 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/private.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10104 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/mixins/public.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     1611 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/share.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    12340 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/signup.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11479 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3132 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/mixins/timeline.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4039 2023-11-28 11:31:19.000000 aiograpi-0.0.1/aiograpi/mixins/totp.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2871 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/track.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    35110 2024-02-27 14:46:39.000000 aiograpi-0.0.1/aiograpi/mixins/user.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    33612 2024-02-27 14:33:28.000000 aiograpi-0.0.1/aiograpi/mixins/video.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4150 2023-11-22 18:01:30.000000 aiograpi-0.0.1/aiograpi/reqwests.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8476 2023-10-10 17:45:34.000000 aiograpi-0.0.1/aiograpi/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    12090 2024-01-29 15:44:23.000000 aiograpi-0.0.1/aiograpi/types.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2992 2024-02-27 14:43:45.000000 aiograpi-0.0.1/aiograpi/utils.py
--rw-r--r--   0 adw0rd     (501) staff       (20)      311 2023-11-22 18:01:30.000000 aiograpi-0.0.1/aiograpi/zones.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-02-27 15:15:52.005037 aiograpi-0.0.1/aiograpi.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1805 2024-02-27 15:15:51.000000 aiograpi-0.0.1/aiograpi.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)     1177 2024-02-27 15:15:51.000000 aiograpi-0.0.1/aiograpi.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2024-02-27 15:15:51.000000 aiograpi-0.0.1/aiograpi.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)      100 2024-02-27 15:15:51.000000 aiograpi-0.0.1/aiograpi.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2024-02-27 15:15:51.000000 aiograpi-0.0.1/aiograpi.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2024-02-27 15:15:52.016069 aiograpi-0.0.1/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     2532 2024-02-27 14:37:36.000000 aiograpi-0.0.1/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.682994 aiograpi-0.0.2/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1056 2024-03-02 23:24:00.000000 aiograpi-0.0.2/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1729 2024-04-13 15:16:39.682699 aiograpi-0.0.2/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10756 2024-03-04 10:06:34.000000 aiograpi-0.0.2/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.669865 aiograpi-0.0.2/aiograpi/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     3541 2024-03-03 00:22:37.000000 aiograpi-0.0.2/aiograpi/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2772 2024-02-27 14:43:44.000000 aiograpi-0.0.2/aiograpi/config.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     6839 2024-03-03 00:20:42.000000 aiograpi-0.0.2/aiograpi/exceptions.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    19241 2024-03-03 01:00:05.000000 aiograpi-0.0.2/aiograpi/extractors.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.682034 aiograpi-0.0.2/aiograpi/mixins/
+-rw-r--r--   0 adw0rd     (501) staff       (20)        0 2023-11-08 14:15:14.000000 aiograpi-0.0.2/aiograpi/mixins/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     7375 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/account.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10509 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/album.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    27252 2024-03-03 01:43:10.000000 aiograpi-0.0.2/aiograpi/mixins/auth.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1572 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/bloks.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    23109 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/challenge.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10767 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/clip.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     6441 2024-03-03 00:01:17.000000 aiograpi-0.0.2/aiograpi/mixins/collection.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    18105 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/comment.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    22459 2024-03-02 23:18:03.000000 aiograpi-0.0.2/aiograpi/mixins/direct.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     3310 2024-02-27 14:43:44.000000 aiograpi-0.0.2/aiograpi/mixins/fbsearch.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8142 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/graphql.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    15880 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/hashtag.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8652 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/highlight.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10812 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/igtv.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     6430 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/insights.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    16761 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/location.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    37772 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/media.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)      496 2024-03-03 00:24:12.000000 aiograpi-0.0.2/aiograpi/mixins/multiple_accounts.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2257 2024-03-03 01:57:36.000000 aiograpi-0.0.2/aiograpi/mixins/note.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    16438 2024-03-02 22:36:16.000000 aiograpi-0.0.2/aiograpi/mixins/notification.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2665 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/password.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    22899 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/photo.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    24114 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/private.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10183 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/public.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1611 2024-02-27 14:33:28.000000 aiograpi-0.0.2/aiograpi/mixins/share.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    12525 2024-03-02 22:25:43.000000 aiograpi-0.0.2/aiograpi/mixins/signup.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    11639 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/story.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     3132 2024-02-27 14:43:45.000000 aiograpi-0.0.2/aiograpi/mixins/timeline.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4039 2023-11-28 11:31:19.000000 aiograpi-0.0.2/aiograpi/mixins/totp.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2896 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/mixins/track.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    36854 2024-03-03 00:59:58.000000 aiograpi-0.0.2/aiograpi/mixins/user.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    33721 2024-04-13 15:14:01.000000 aiograpi-0.0.2/aiograpi/mixins/video.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4148 2024-03-02 23:19:15.000000 aiograpi-0.0.2/aiograpi/reqwests.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8476 2023-10-10 17:45:34.000000 aiograpi-0.0.2/aiograpi/story.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    15233 2024-03-03 01:41:07.000000 aiograpi-0.0.2/aiograpi/types.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2992 2024-02-27 14:43:45.000000 aiograpi-0.0.2/aiograpi/utils.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)      311 2023-11-22 18:01:30.000000 aiograpi-0.0.2/aiograpi/zones.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2024-04-13 15:16:39.670833 aiograpi-0.0.2/aiograpi.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1729 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1246 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)      100 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2024-04-13 15:16:39.000000 aiograpi-0.0.2/aiograpi.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2024-04-13 15:16:39.683049 aiograpi-0.0.2/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2436 2024-04-13 15:15:48.000000 aiograpi-0.0.2/setup.py
```

### Comparing `aiograpi-0.0.1/PKG-INFO` & `aiograpi-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: aiograpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/aiograpi
 Author: Mr.Robot
 Author-email: mr.robot@example.org
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 Asynchronous Instagram Private API wrapper.
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `aiograpi-0.0.1/README.md` & `aiograpi-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+# aiograpi - Asynchronous Instagram API for Python
+
 If you want to work with aiograpi (business interests), we strongly advise you to prefer [HikerAPI](https://hikerapi.com/p/KhMxYMSn) project.
 However, you won't need to spend weeks or even months setting it up.
 The best service available today is [HikerAPI](https://hikerapi.com/p/KhMxYMSn), which handles 4–5 million daily requests, provides support around-the-clock, and offers partners a special rate.
 In many instances, our clients tried to save money and preferred aiograpi, but in our experience, they ultimately returned to [HikerAPI](https://hikerapi.com/p/KhMxYMSn) after spending much more time and money.
 It will be difficult to find good accounts, good proxies, or resolve challenges, and IG will ban your accounts.
 
 The aiograpi more suits for testing or research than a working business!
 
 ### We recommend using our services:
 
 * [LamaTok](https://lamatok.com/p/X0HatoxX) for TikTok API 🔥
 * [HikerAPI](https://hikerapi.com/p/KhMxYMSn) for Instagram API ⚡⚡⚡
 * [DataLikers](https://datalikers.com/p/XPhrh0Y3) for Instagram Datasets 🚀
 
-[![Package](https://github.com/subzeroid/aiograpi/actions/workflows/python-package.yml/badge.svg?branch=master&1)](https://github.com/subzeroid/aiograpi/actions/workflows/python-package.yml)
+[![Package](https://github.com/subzeroid/aiograpi/actions/workflows/python-package.yml/badge.svg?branch=main&1)](https://github.com/subzeroid/aiograpi/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aiograpi)](https://pypi.org/project/aiograpi/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiograpi)
 ![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)
 
 
 Features:
 
@@ -29,39 +31,39 @@
 * Login by username and password, sessionid and support 2FA
 * Managing messages and threads for Direct and attach files
 * Download and upload a Photo, Video, IGTV, Reels, Albums and Stories
 * Work with Users, Posts, Comments, Insights, Collections, Location and Hashtag
 * Insights by account, posts and stories
 * Like, following, commenting, editing account (Bio) and much more else
 
-# aiograpi - Unofficial Instagram API for Python
+-----
 
-Fast and effective Instagram Private API wrapper (public+private requests and challenge resolver) without selenium. Use the most recent version of the API from Instagram, which was obtained using reverse-engineering with Charles Proxy and [Proxyman](https://proxyman.io/).
+Asynchronous Instagram Private API wrapper without selenium. Use the most recent version of the API from Instagram, which was obtained using reverse-engineering with Charles Proxy and [Proxyman](https://proxyman.io/).
 
 *Instagram API valid for **27 Feb 2024** (last reverse-engineering check)*
 
 Support **Python >= 3.10**
 
 For any other languages (e.g. C++, C#, F#, D, [Golang](https://github.com/subzeroid/instagrapi-rest/tree/main/golang), Erlang, Elixir, Nim, Haskell, Lisp, Closure, Julia, R, Java, Kotlin, Scala, OCaml, JavaScript, Crystal, Ruby, Rust, [Swift](https://github.com/subzeroid/instagrapi-rest/tree/main/swift), Objective-C, Visual Basic, .NET, Pascal, Perl, Lua, PHP and others), I suggest using [instagrapi-rest](https://github.com/subzeroid/instagrapi-rest)
 
 [Support Chat in Telegram](https://t.me/instagrapi)
-![](https://gist.githubusercontent.com/m8rge/4c2b36369c9f936c02ee883ca8ec89f1/raw/c03fd44ee2b63d7a2a195ff44e9bb071e87b4a40/telegram-single-path-24px.svg) and [GitHub Discussions](https://github.com/subzeroid/instagrapi/discussions)
+![](https://gist.githubusercontent.com/m8rge/4c2b36369c9f936c02ee883ca8ec89f1/raw/c03fd44ee2b63d7a2a195ff44e9bb071e87b4a40/telegram-single-path-24px.svg) and [GitHub Discussions](https://github.com/subzeroid/aiograpi/discussions)
 
 
 ## Features
 
 1. Performs [Web API](https://subzeroid.github.io/aiograpi/usage-guide/fundamentals.html) or [Mobile API](https://subzeroid.github.io/aiograpi/usage-guide/fundamentals.html) requests depending on the situation (to avoid Instagram limits)
 2. [Login](https://subzeroid.github.io/aiograpi/usage-guide/interactions.html) by username and password, including 2FA and by sessionid (and uses Authorization header instead Cookies)
 3. [Challenge Resolver](https://subzeroid.github.io/aiograpi/usage-guide/challenge_resolver.html) have Email and SMS handlers
 4. Support [upload](https://subzeroid.github.io/aiograpi/usage-guide/media.html) a Photo, Video, IGTV, Reels, Albums and Stories
 5. Support work with [User](https://subzeroid.github.io/aiograpi/usage-guide/user.html), [Media](https://subzeroid.github.io/aiograpi/usage-guide/media.html), [Comment](https://subzeroid.github.io/aiograpi/usage-guide/comment.html), [Insights](https://subzeroid.github.io/aiograpi/usage-guide/insight.html), [Collections](https://subzeroid.github.io/aiograpi/usage-guide/collection.html), [Location](https://subzeroid.github.io/aiograpi/usage-guide/location.html) (Place), [Hashtag](https://subzeroid.github.io/aiograpi/usage-guide/hashtag.html) and [Direct Message](https://subzeroid.github.io/aiograpi/usage-guide/direct.html) objects
 6. [Like](https://subzeroid.github.io/aiograpi/usage-guide/media.html), [Follow](https://subzeroid.github.io/aiograpi/usage-guide/user.html), [Edit account](https://subzeroid.github.io/aiograpi/usage-guide/account.html) (Bio) and much more else
 7. [Insights](https://subzeroid.github.io/aiograpi/usage-guide/insight.html) by account, posts and stories
 8. [Build stories](https://subzeroid.github.io/aiograpi/usage-guide/story.html) with custom background, font animation, link sticker and mention users
-9. In the next release, account registration and captcha passing will appear
+9. Account [registration](https://github.com/subzeroid/aiograpi/blob/main/aiograpi/mixins/signup.py) and captcha passing will appear
 
 ### Installation
 
 ```
 pip install aiograpi
 ```
```

### Comparing `aiograpi-0.0.1/aiograpi/__init__.py` & `aiograpi-0.0.2/aiograpi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,42 +6,46 @@
 from aiograpi.mixins.auth import LoginMixin
 from aiograpi.mixins.bloks import BloksMixin
 from aiograpi.mixins.challenge import ChallengeResolveMixin
 from aiograpi.mixins.clip import DownloadClipMixin, UploadClipMixin
 from aiograpi.mixins.collection import CollectionMixin
 from aiograpi.mixins.comment import CommentMixin
 from aiograpi.mixins.direct import DirectMixin
-from aiograpi.mixins.track import TrackMixin
 from aiograpi.mixins.fbsearch import FbSearchMixin
+from aiograpi.mixins.graphql import GraphQLRequestMixin
 from aiograpi.mixins.hashtag import HashtagMixin
 from aiograpi.mixins.highlight import HighlightMixin
 from aiograpi.mixins.igtv import DownloadIGTVMixin, UploadIGTVMixin
 from aiograpi.mixins.insights import InsightsMixin
 from aiograpi.mixins.location import LocationMixin
 from aiograpi.mixins.media import MediaMixin
+from aiograpi.mixins.multiple_accounts import MultipleAccountsMixin
+from aiograpi.mixins.note import NoteMixin
 from aiograpi.mixins.notification import NotificationMixin
 from aiograpi.mixins.password import PasswordMixin
 from aiograpi.mixins.photo import DownloadPhotoMixin, UploadPhotoMixin
 from aiograpi.mixins.private import PrivateRequestMixin
 from aiograpi.mixins.public import (
     ProfilePublicMixin,
     PublicRequestMixin,
     TopSearchesPublicMixin,
 )
-from aiograpi.mixins.graphql import GraphQLRequestMixin
 from aiograpi.mixins.share import ShareMixin
 from aiograpi.mixins.signup import SignUpMixin
 from aiograpi.mixins.story import StoryMixin
 from aiograpi.mixins.timeline import ReelsMixin
 from aiograpi.mixins.totp import TOTPMixin
+from aiograpi.mixins.track import TrackMixin
 from aiograpi.mixins.user import UserMixin
 from aiograpi.mixins.video import DownloadVideoMixin, UploadVideoMixin
 
 
 class Client(
+    MultipleAccountsMixin,
+    NoteMixin,
     GraphQLRequestMixin,
     PublicRequestMixin,
     ChallengeResolveMixin,
     PrivateRequestMixin,
     TopSearchesPublicMixin,
     ProfilePublicMixin,
     LoginMixin,
```

### Comparing `aiograpi-0.0.1/aiograpi/config.py` & `aiograpi-0.0.2/aiograpi/config.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/exceptions.py` & `aiograpi-0.0.2/aiograpi/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,18 @@
     """
 
 
 class BadPassword(PrivateError):
     ...
 
 
+class BadCredentials(PrivateError):
+    ...
+
+
 class PleaseWaitFewMinutes(PrivateError):
     ...
 
 
 class UnknownError(PrivateError):
     ...
 
@@ -313,14 +317,18 @@
     ...
 
 
 class InvalidNonce(PrivateError):
     ...
 
 
+class NoteNotFound(NotFoundError):
+    reason = "Not found"
+
+
 class ConsentRequired(PrivateError):
     ...
 
 
 class GeoBlockRequired(PrivateError):
     ...
 
@@ -379,7 +387,21 @@
 
 class ConnectProxyError(ProxyError):
     """ProxyError is raised due to a HTTP 401 response"""
 
 
 class AuthRequiredProxyError(ProxyError):
     """ProxyError is raised due to a HTTP 407 response"""
+
+
+class UnsupportedError(ClientError):
+    def __init__(self, value, items):
+        message = f'Unsupported value="{value}" {items}'
+        super().__init__(message)
+
+
+class UnsupportedSettingValue(UnsupportedError):
+    ...
+
+
+class PreLoginRequired(ClientError):
+    message = "Login required"
```

### Comparing `aiograpi-0.0.1/aiograpi/extractors.py` & `aiograpi-0.0.2/aiograpi/extractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
+import datetime
 import logging
 
-# from copy import deepcopy
-
 import orjson
 
 from .types import (
     About,
     Account,
     Collection,
     Comment,
     DirectMedia,
     DirectMessage,
     DirectResponse,
     DirectShortThread,
     DirectThread,
+    Guide,
     Hashtag,
     Highlight,
     Location,
-    Guide,
     Media,
     MediaOembed,
+    MediaXma,
+    ReplyMessage,
     Resource,
     Story,
     StoryLink,
     StoryMedia,
     StoryMention,
     Track,
     User,
     UserShort,
     Usertag,
 )
 from .utils import InstagramIdCodec, json_value
 
+# from copy import deepcopy
+
 
 MEDIA_TYPES_GQL = {"GraphImage": 1, "GraphVideo": 2, "GraphSidecar": 8, "StoryVideo": 2}
 
 logger = logging.getLogger(__name__)
 
 
 def extract_media_v1(media):
@@ -85,14 +88,33 @@
         resources=[
             extract_resource_v1(edge) for edge in media.get("carousel_media", [])
         ],
         **media,
     )
 
 
+def extract_media_v1_xma(media):
+    """Extract media from Private API"""
+    # media = deepcopy(data)
+    # media["media_type"] = 10
+    media["video_url"] = media.get("target_url", "")
+    media["title"] = media.get("title_text", "")
+    media["preview_url"] = media.get("preview_url", "")
+    media["preview_url_mime_type"] = media.get("preview_url_mime_type", "")
+    media["header_icon_url"] = media.get("header_icon_url", "")
+    media["header_icon_width"] = media.get("header_icon_width", 0)
+    media["header_icon_height"] = media.get("header_icon_height", 0)
+    media["header_title_text"] = media.get("header_title_text", "")
+    media["preview_media_fbid"] = media.get("preview_media_fbid", "")
+
+    return MediaXma(
+        **media,
+    )
+
+
 def extract_media_gql(media):
     """Extract media from GraphQL"""
     # media = deepcopy(data)
     user = extract_user_short(media["owner"])
     # if "full_name" in user:
     #     user = extract_user_short(user)
     # else:
@@ -331,29 +353,65 @@
     return DirectShortThread(**data)
 
 
 def extract_direct_response(data):
     return DirectResponse(**data)
 
 
+def extract_reply_message(data):
+    data["id"] = data.get("item_id")
+    if "media_share" in data:
+        ms = data["media_share"]
+        if not ms.get("code"):
+            ms["code"] = InstagramIdCodec.encode(ms["id"])
+        data["media_share"] = extract_media_v1(ms)
+    if "media" in data:
+        data["media"] = extract_direct_media(data["media"])
+    clip = data.get("clip", {})
+    if clip:
+        if "clip" in clip:
+            # Instagram ¯\_(ツ)_/¯
+            clip = clip.get("clip")
+        data["clip"] = extract_media_v1(clip)
+
+    data["timestamp"] = datetime.datetime.fromtimestamp(data["timestamp"] // 1_000_000)
+    data["user_id"] = str(data["user_id"])
+
+    return ReplyMessage(**data)
+
+
 def extract_direct_message(data):
     data["id"] = data.get("item_id")
+    if "replied_to_message" in data:
+        data["reply"] = extract_reply_message(data["replied_to_message"])
     if "media_share" in data:
         ms = data["media_share"]
         if not ms.get("code"):
             ms["code"] = InstagramIdCodec.encode(ms["id"])
         data["media_share"] = extract_media_v1(ms)
     if "media" in data:
         data["media"] = extract_direct_media(data["media"])
+    if "voice_media" in data:
+        if "media" in data["voice_media"]:
+            data["media"] = extract_direct_media(data["voice_media"]["media"])
     clip = data.get("clip", {})
     if clip:
         if "clip" in clip:
             # Instagram ¯\_(ツ)_/¯
             clip = clip.get("clip")
         data["clip"] = extract_media_v1(clip)
+    xma_media_share = data.get("xma_media_share", {})
+    if xma_media_share:
+        data["xma_share"] = extract_media_v1_xma(xma_media_share[0])
+
+    data["timestamp"] = datetime.datetime.fromtimestamp(
+        int(data["timestamp"]) // 1_000_000
+    )
+    data["user_id"] = str(data.get("user_id", ""))
+
     return DirectMessage(**data)
 
 
 def extract_direct_media(media):
     # media = deepcopy(data)
     if versions := media.get("video_versions", []):
         # Select Best Quality by Resolutiuon
@@ -367,14 +425,15 @@
         )[-1]["url"]
     if "user" in media:
         media["user"] = extract_user_short(media.get("user"))
     return DirectMedia(**media)
 
 
 def extract_account(data):
+    data["pk"] = str(data["pk"])
     data["external_url"] = data.get("external_url") or None
     return Account(**data)
 
 
 def extract_hashtag_gql(data):
     data["media_count"] = data.get("edge_hashtag_to_media", {}).get("count")
     data["profile_pic_url"] = data.get("profile_pic_url") or None
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/account.py` & `aiograpi-0.0.2/aiograpi/mixins/account.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/album.py` & `aiograpi-0.0.2/aiograpi/mixins/album.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
                     """
                     await asyncio.sleep(configure_timeout)
                     continue
                 raise e
             else:
                 if configured:
                     media = configured.get("media")
-                    self.expose()
+                    await self.expose()
                     return extract_media_v1(media)
         raise (configure_exception or AlbumConfigureError)(
             response=self.last_response, **self.last_json
         )
 
     async def album_configure(
         self,
@@ -270,15 +270,15 @@
                 {"user_id": tag.user.pk, "position": [tag.x, tag.y]} for tag in usertags
             ]
             childs[0]["usertags"] = dumps({"in": usertags})
         data = {
             "timezone_offset": str(self.timezone_offset),
             "source_type": "4",
             "creation_logger_session_id": self.client_session_id,
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "caption": caption,
             "client_sidecar_id": upload_id,
             "upload_id": upload_id,
             # "location": self.build_location(name, lat, lng, address),
             "suggested_venue_position": -1,
             "device": self.device,
             "is_suggested_venue": False,
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/auth.py` & `aiograpi-0.0.2/aiograpi/mixins/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import base64
-import json
 
 # import datetime
 import hashlib
 import hmac
+import json
 import random
 import re
 import time
 import uuid
 from pathlib import Path
 from typing import Dict, List
 from uuid import uuid4
 
 from pydantic import ValidationError
 
 from aiograpi import config
 from aiograpi.exceptions import (
+    BadCredentials,
     ClientThrottledError,
     PleaseWaitFewMinutes,
     PrivateError,
     ReloginAttemptExceeded,
     TwoFactorRequired,
 )
 from aiograpi.utils import dumps, gen_token, generate_jazoest
@@ -372,17 +373,22 @@
             2FA verification code
 
         Returns
         -------
         bool
             A boolean value
         """
-        self.username = username
-        self.password = password
-        # self.init()
+
+        if not self.username or not self.password:
+            if username is None or password is None:
+                raise BadCredentials("Both username and password must be provided.")
+
+            self.username = username
+            self.password = password
+
         if relogin:
             self.authorization_data = {}
             self.private.headers.pop("Authorization", None)
             self.private.cookies.clear()
             if self.relogin_attempt > 1:
                 raise ReloginAttemptExceeded()
             self.relogin_attempt += 1
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/bloks.py` & `aiograpi-0.0.2/aiograpi/mixins/bloks.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/challenge.py` & `aiograpi-0.0.2/aiograpi/mixins/challenge.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
-import json
 import hashlib
+import json
 import logging
 import random
 import time
 from enum import Enum
 from typing import Dict
 
 from aiograpi import reqwests
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/clip.py` & `aiograpi-0.0.2/aiograpi/mixins/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                     """
                     await asyncio.sleep(configure_timeout)
                     continue
                 raise e
             else:
                 if configured:
                     media = self.last_json.get("media")
-                    self.expose()
+                    await self.expose()
                     return extract_media_v1(media)
         raise ClipConfigureError(response=self.last_response, **self.last_json)
 
     async def clip_configure(
         self,
         upload_id: str,
         thumbnail: Path,
@@ -244,15 +244,15 @@
             {"user_id": tag.user.pk, "position": [tag.x, tag.y]} for tag in usertags
         ]
         data = {
             # "igtv_ads_toggled_on": "0",
             "filter_type": "0",
             "timezone_offset": str(self.timezone_offset),
             "media_folder": "ScreenRecorder",
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "source_type": "4",
             # "title": title,
             "caption": caption,
             "usertags": json.dumps({"in": usertags}),
             "date_time_original": date_time_original(time.localtime()),
             "clips_share_preview_to_feed": feed_show,
             "upload_id": upload_id,
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/collection.py` & `aiograpi-0.0.2/aiograpi/mixins/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from aiograpi.exceptions import CollectionNotFound, PrivateError
+from aiograpi.exceptions import CollectionNotFound, PreLoginRequired, PrivateError
 from aiograpi.extractors import extract_collection, extract_media_v1
 from aiograpi.types import Collection, Media
 
 
 class CollectionMixin:
     """
     Helpers for collection
@@ -137,15 +137,15 @@
                 )
             except PrivateError as e:
                 raise e
             except Exception as e:
                 self.logger.exception(e)
                 break
             for item in result["items"]:
-                if last_media_pk and last_media_pk == item["media"]["pk"]:
+                if last_media_pk and last_media_pk == item.pk:
                     found_last_media_pk = True
                     break
                 total_items.append(extract_media_v1(item.get("media", item)))
             if (amount and len(total_items) >= amount) or found_last_media_pk:
                 break
             if not result.get("more_available"):
                 break
@@ -168,15 +168,16 @@
             If True then save to collection, otherwise unsave
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_id(media_id)
         data = {
             "module_name": "feed_timeline",
             "radio_type": "wifi-none",
         }
         if collection_pk:
             data["added_collection_ids"] = f"[{int(collection_pk)}]"
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/comment.py` & `aiograpi-0.0.2/aiograpi/mixins/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import random
 from typing import List, Optional, Tuple
 
-from aiograpi.exceptions import (
+from aiograpi.exceptions import (  # CommentsDisabled,
     ClientError,
     ClientLoginRequired,
     ClientNotFoundError,
-    # CommentsDisabled,
     CommentNotFound,
     MediaNotFound,
+    PreLoginRequired,
     PrivateError,
 )
 from aiograpi.extractors import extract_comment
-from aiograpi.types import Comment
-from aiograpi.utils import generate_jazoest, dumps
 from aiograpi.mixins.graphql import GQL_STUFF
+from aiograpi.types import Comment
+from aiograpi.utils import dumps, generate_jazoest
 
 
 class CommentMixin:
     """
     Helpers for managing comments on a Media
     """
 
@@ -396,15 +396,16 @@
             String to be posted on the media
 
         Returns
         -------
         Comment
             An object of Comment type
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         data = {
             "delivery_class": "organic",
             "feed_position": "0",
             "container_module": "self_comments_v2_feed_contextual_self_profile",
             "user_breadcrumb": self.gen_user_breadcrumb(len(text)),
             "idempotence_token": self.generate_uuid(),
             "comment_text": text,
@@ -429,15 +430,16 @@
             If liked, whether or not to unlike. Default is False
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         comment_pk = int(comment_pk)
         data = {
             "is_carousel_bumped_post": "false",
             "container_module": "feed_contextual_self_profile",
             "feed_position": str(random.randint(0, 6)),
         }
         name = "unlike" if revert else "like"
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/direct.py` & `aiograpi-0.0.2/aiograpi/mixins/direct.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import random
 import re
 import time
 from pathlib import Path
 from typing import List, Optional
 
-from aiograpi.exceptions import ClientNotFoundError, DirectThreadNotFound
+from aiograpi.exceptions import (
+    ClientNotFoundError,
+    DirectThreadNotFound,
+    PreLoginRequired,
+)
 from aiograpi.extractors import (
     extract_direct_message,
     extract_direct_response,
     extract_direct_short_thread,
     extract_direct_thread,
 )
 from aiograpi.types import (
@@ -50,15 +54,16 @@
             Maximum number of media to return, default is 20
 
         Returns
         -------
         List[DirectThread]
             A list of objects of DirectThread
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         params = {
             "visual_message_return_type": "unseen",
             "thread_message_limit": "10",
             "persistentBadging": "true",
             "limit": "20",
         }
         if selected_filter:
@@ -100,15 +105,16 @@
             Maximum number of media to return, default is 20
 
         Returns
         -------
         List[DirectThread]
             A list of objects of DirectThread
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         params = {
             "visual_message_return_type": "unseen",
             "persistentBadging": "true",
         }
         cursor = None
         threads = []
         # self.private_request("direct_v2/get_presence/")
@@ -141,15 +147,16 @@
             Maximum number of media to return, default is 20
 
         Returns
         -------
         DirectThread
             An object of DirectThread
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         params = {
             "visual_message_return_type": "unseen",
             "direction": "older",
             "seq_id": "40065",  # 59663
             "limit": "20",
         }
         cursor = None
@@ -189,15 +196,16 @@
             Maximum number of media to return, default is 20
 
         Returns
         -------
         List[DirectMessage]
             A list of objects of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         return await self.direct_thread(thread_id, amount).messages
 
     async def direct_answer(self, thread_id: int, text: str) -> DirectMessage:
         """
         Post a message on a Direct Message thread
 
         Parameters
@@ -209,15 +217,16 @@
             String to be posted on the thread
 
         Returns
         -------
         DirectMessage
             An object of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         return await self.direct_send(text, [], [int(thread_id)])
 
     async def direct_send(
         self, text: str, user_ids: List[int] = [], thread_ids: List[int] = []
     ) -> DirectMessage:
         """
         Send a direct message to list of users or threads
@@ -234,15 +243,16 @@
             List of unique identifier of Direct Message thread id
 
         Returns
         -------
         DirectMessage
             An object of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         assert (user_ids or thread_ids) and not (
             user_ids and thread_ids
         ), "Specify user_ids or thread_ids, but not both"
         method = "text"
         token = self.generate_mutation_token()
         kwargs = {
             "action": "send_item",
@@ -338,15 +348,16 @@
             List of unique identifier of Direct Message thread id
 
         Returns
         -------
         DirectMessage
             An object of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         assert (user_ids or thread_ids) and not (
             user_ids and thread_ids
         ), "Specify user_ids or thread_ids, but not both"
         method = f"configure_{content_type}"
         token = self.generate_mutation_token()
         nav_chains = [
             "6xQ:direct_media_picker_photos_fragment:1,5rG:direct_thread:2,5ME:direct_quick_camera_fragment:3,5ME:direct_quick_camera_fragment:4,4ju:reel_composer_preview:5,5rG:direct_thread:6,5rG:direct_thread:7,6xQ:direct_media_picker_photos_fragment:8,5rG:direct_thread:9",
@@ -497,15 +508,16 @@
             List of unique identifier of Users id
 
         Returns
         -------
         DirectMessage
             An object of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         token = self.generate_mutation_token()
         media_id = await self.media_id(media_id)
         recipient_users = dumps([[int(uid) for uid in user_ids]])
         data = {
             "recipient_users": recipient_users,
             "action": "send_item",
             "is_shh_mode": 0,
@@ -540,15 +552,16 @@
             List of unique identifier of Users id
 
         Returns
         -------
         DirectMessage
             An object of DirectMessage
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         assert (user_ids or thread_ids) and not (
             user_ids and thread_ids
         ), "Specify user_ids or thread_ids, but not both"
         story_id = await self.media_id(story_id)
         story_pk = await self.media_pk(story_id)
         token = self.generate_mutation_token()
         data = {
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/fbsearch.py` & `aiograpi-0.0.2/aiograpi/mixins/fbsearch.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/graphql.py` & `aiograpi-0.0.2/aiograpi/mixins/graphql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import asyncio
 import logging
 import time
+
 import orjson
 
 from aiograpi import reqwests
-from aiograpi.utils import random_delay
 from aiograpi.exceptions import (
-    ClientUnauthorizedError,
+    AboutUsError,
+    AccountSuspended,
+    ChallengeRequired,
     ClientBadRequestError,
     ClientConnectionError,
     ClientError,
     ClientForbiddenError,
     ClientJSONDecodeError,
     ClientLoginRequired,
     ClientNotFoundError,
     ClientThrottledError,
-    ChallengeRequired,
-    AccountSuspended,
-    TermsUnblock,
+    ClientUnauthorizedError,
     TermsAccept,
-    AboutUsError,
+    TermsUnblock,
 )
-
+from aiograpi.utils import random_delay
 
 GRAPHQL_API_URL = "https://www.instagram.com/api/graphql"
 
 GQL_STUFF = {
     "av": "17841464591314721",
     "__d": "www",
     "__user": "0",
@@ -118,16 +118,18 @@
     ):
         kwargs = dict(
             data=data,
             params=params,
             headers=headers,
             return_json=return_json,
         )
-        assert retries_count <= 10, "Retries count is too high"
-        assert retries_timeout <= 600, "Retries timeout is too high"
+        if retries_count > 10:
+            raise Exception("Retries count is too high")
+        if retries_timeout > 600:
+            raise Exception("Retries timeout is too high")
         self.inject_sessionid_to_public()
         for iteration in range(retries_count):
             try:
                 if self.delay_range:
                     await random_delay(delay_range=self.delay_range)
                 return await self._send_graphql_request(**kwargs)
             except (
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/hashtag.py` & `aiograpi-0.0.2/aiograpi/mixins/hashtag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import base64
 from typing import List, Tuple
 
 import orjson
 
-from aiograpi.utils import dumps
-from aiograpi.exceptions import ClientUnauthorizedError
-from aiograpi.exceptions import ClientError, HashtagNotFound, WrongCursorError
+from aiograpi.exceptions import (
+    ClientError,
+    ClientUnauthorizedError,
+    HashtagNotFound,
+    PreLoginRequired,
+    WrongCursorError,
+)
 from aiograpi.extractors import (
     extract_hashtag_gql,
     extract_hashtag_v1,
     extract_media_v1,
 )
 from aiograpi.types import Hashtag, Media
+from aiograpi.utils import dumps
 
 
 class HashtagMixin:
     """
     Helpers for managing Hashtag
     """
 
@@ -490,15 +495,16 @@
         unfollow: bool, optional
             Unfollow when True
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         name = "unfollow" if unfollow else "follow"
         data = self.with_action_data({"user_id": self.user_id})
         result = await self.private_request(
             f"web/tags/{name}/{hashtag}/", domain="www.instagram.com", data=data
         )
         return result["status"] == "ok"
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/highlight.py` & `aiograpi-0.0.2/aiograpi/mixins/highlight.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/igtv.py` & `aiograpi-0.0.2/aiograpi/mixins/igtv.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                     """
                     await asyncio.sleep(configure_timeout)
                     continue
                 raise e
             else:
                 if configured:
                     media = self.last_json.get("media")
-                    self.expose()
+                    await self.expose()
                     return extract_media_v1(media)
         raise IGTVConfigureError(response=self.last_response, **self.last_json)
 
     async def igtv_configure(
         self,
         upload_id: str,
         thumbnail: Path,
@@ -248,15 +248,15 @@
             {"user_id": tag.user.pk, "position": [tag.x, tag.y]} for tag in usertags
         ]
         data = {
             "igtv_ads_toggled_on": "0",
             "filter_type": "0",
             "timezone_offset": str(self.timezone_offset),
             "media_folder": "ScreenRecorder",
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "source_type": "4",
             "title": title,
             "caption": caption,
             "usertags": json.dumps({"in": usertags}),
             "date_time_original": date_time_original(time.localtime()),
             "igtv_share_preview_to_feed": "1",
             "upload_id": upload_id,
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/insights.py` & `aiograpi-0.0.2/aiograpi/mixins/insights.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import asyncio
 from typing import Dict, List
 
-from aiograpi.exceptions import ClientError, MediaError, UserError
+from aiograpi.exceptions import (
+    ClientError,
+    MediaError,
+    PreLoginRequired,
+    UnsupportedError,
+    UserError,
+)
 from aiograpi.utils import json_value
 
-
 POST_TYPES = ("ALL", "CAROUSEL_V2", "IMAGE", "SHOPPING", "VIDEO")
 TIME_FRAMES = (
     "ONE_WEEK",
     "ONE_MONTH",
     "THREE_MONTHS",
     "SIX_MONTHS",
     "ONE_YEAR",
@@ -68,24 +73,22 @@
             Timeout between pages iterations, default is 2
 
         Returns
         -------
         List[Dict]
             List of dictionaries of response from the call
         """
-        assert (
-            post_type in POST_TYPES
-        ), f'Unsupported post_type="{post_type}" {POST_TYPES}'
-        assert (
-            time_frame in TIME_FRAMES
-        ), f'Unsupported time_frame="{time_frame}" {TIME_FRAMES}'
-        assert (
-            data_ordering in DATA_ORDERS
-        ), f'Unsupported data_ordering="{data_ordering}" {DATA_ORDERS}'
-        assert self.user_id, "Login required"
+        if post_type not in POST_TYPES:
+            raise UnsupportedError(post_type, POST_TYPES)
+        if time_frame not in TIME_FRAMES:
+            raise UnsupportedError(time_frame, TIME_FRAMES)
+        if data_ordering not in DATA_ORDERS:
+            raise UnsupportedError(data_ordering, DATA_ORDERS)
+        if not self.user_id:
+            raise PreLoginRequired
         medias = []
         cursor = None
         data = {
             "surface": "post_grid",
             "doc_id": 2345520318892697,
             "locale": "en_US",
             "vc_policy": "insights_policy",
@@ -146,15 +149,16 @@
         Get insights for account
 
         Returns
         -------
         Dict
             A dictionary of response from the call
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         data = {
             "surface": "account",
             "doc_id": 2449243051851783,
             "locale": "en_US",
             "vc_policy": "insights_policy",
             "strip_nulls": False,
             "strip_defaults": False,
@@ -186,15 +190,16 @@
             PK for the album you want to download
 
         Returns
         -------
         Dict
             A dictionary with insights data
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_pk = await self.media_pk(media_pk)
         data = {
             "surface": "post",
             "doc_id": 3221905377882880,
             "locale": "en_US",
             "vc_policy": "insights_policy",
             "strip_nulls": False,
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/location.py` & `aiograpi-0.0.2/aiograpi/mixins/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import base64
 import json
 from typing import List, Tuple
 
-from aiograpi.exceptions import (
-    ClientNotFoundError,
-    LocationNotFound,
-    WrongCursorError,
-)
-from aiograpi.extractors import extract_location, extract_media_v1, extract_guide_v1
+from aiograpi.exceptions import ClientNotFoundError, LocationNotFound, WrongCursorError
+from aiograpi.extractors import extract_guide_v1, extract_location, extract_media_v1
 from aiograpi.types import Guide, Location, Media
 
 tab_keys_a1 = ("edge_location_to_top_posts", "edge_location_to_media")
 tab_keys_v1 = ("ranked", "recent")
 
 
 class LocationMixin:
@@ -60,17 +56,16 @@
             An object of location
 
         Returns
         -------
         Location
             An object of Location
         """
-        assert location and isinstance(
-            location, Location
-        ), f'Location is wrong "{location}" ({type(location)})'
+        if not (location and isinstance(location, Location)):
+            raise Exception(f'Location is wrong "{location}" ({type(location)})')
         if location.pk and not location.lat:
             # search lat and lng
             info = await self.location_info(location.pk)
             location.lat = info.lat
             location.lng = info.lng
         if not location.external_id and location.lat:
             # search extrernal_id and external_id_source
@@ -211,17 +206,18 @@
             End Cursor, default value is None
 
         Returns
         -------
         Tuple[List[Media], str]
             List of objects of Media and end_cursor
         """
-        assert (
-            tab_key in tab_keys_a1
-        ), f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+        if tab_key not in tab_keys_a1:
+            raise Exception(
+                f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+            )
         unique_set = set()
         medias = []
         end_cursor = None
         result = await self.public_a1_request(
             f"/explore/locations/{location_pk}/",
             params={"max_id": end_cursor} if end_cursor else {},
         )
@@ -258,17 +254,18 @@
             Tab Key, default value is ""
 
         Returns
         -------
         List[Media]
             List of objects of Media
         """
-        assert (
-            tab_key in tab_keys_a1
-        ), f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+        if tab_key not in tab_keys_a1:
+            raise Exception(
+                f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+            )
         medias, _ = await self.location_medias_a1_chunk(
             location_pk, amount, sleep, tab_key
         )
         if amount:
             medias = medias[:amount]
         return medias
 
@@ -293,17 +290,18 @@
             Max ID, default value is None
 
         Returns
         -------
         Tuple[List[Media], str]
             List of objects of Media and max_id
         """
-        assert (
-            tab_key in tab_keys_v1
-        ), f'You must specify one of the options for "tab_key" {tab_keys_v1}'
+        if tab_key not in tab_keys_v1:
+            raise Exception(
+                f'You must specify one of the options for "tab_key" {tab_keys_v1}'
+            )
         data = {
             "_uuid": self.uuid,
             "session_id": self.client_session_id,
             "tab": tab_key,
         }
         if max_id:
             try:
@@ -350,17 +348,18 @@
             Tab Key, default value is ""
 
         Returns
         -------
         List[Media]
             List of objects of Media
         """
-        assert (
-            tab_key in tab_keys_v1
-        ), f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+        if tab_key not in tab_keys_v1:
+            raise Exception(
+                f'You must specify one of the options for "tab_key" {tab_keys_a1}'
+            )
         medias, _ = await self.location_medias_v1_chunk(
             location_pk=location_pk, tab_key=tab_key
         )
         if amount:
             medias = medias[:amount]
         return medias
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/media.py` & `aiograpi-0.0.2/aiograpi/mixins/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from urllib.parse import urlparse
 
 from aiograpi.exceptions import (
     ClientError,
     ClientLoginRequired,
     ClientNotFoundError,
     MediaNotFound,
+    PreLoginRequired,
     PrivateError,
 )
 from aiograpi.extractors import (
     extract_location,
     extract_media_gql,
     extract_media_oembed,
     extract_media_v1,
     extract_user_short,
 )
-from aiograpi.types import Location, Media, UserShort, Usertag
-from aiograpi.utils import InstagramIdCodec, json_value, dumps, generate_jazoest
 from aiograpi.mixins.graphql import GQL_STUFF
+from aiograpi.types import Location, Media, UserShort, Usertag
+from aiograpi.utils import InstagramIdCodec, dumps, generate_jazoest, json_value
 
 
 class MediaMixin:
     """
     Helpers for media
     """
 
@@ -45,17 +46,16 @@
 
         Example
         -------
         2277033926878261772 -> 2277033926878261772_1903424587
         """
         media_id = str(media_pk)
         if "_" not in media_id:
-            assert media_id.isdigit(), (
-                "media_id must been contain digits, now %s" % media_id
-            )
+            if not media_id.isdigit():
+                raise Exception("media_id must been contain digits, now %s" % media_id)
             user = await self.media_user(media_id)
             media_id = "%s_%s" % (media_id, user.pk)
         return media_id
 
     @staticmethod
     async def media_pk(media_id: str) -> str:
         """
@@ -276,15 +276,16 @@
             Unique identifier of the media
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_id(media_id)
         result = await self.private_request(
             f"media/{media_id}/delete/", self.with_default_data({"media_id": media_id})
         )
         return result.get("did_delete")
 
     async def media_edit(
@@ -312,25 +313,26 @@
             Location tag for this upload, default is None
 
         Returns
         -------
         Dict
             A dictionary of response from the call
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_id(media_id)
         media = await self.media_info(media_id)
         usertags = [
             {"user_id": tag.user.pk, "position": [tag.x, tag.y]} for tag in usertags
         ]
         data = {
             "caption_text": caption,
             "container_module": "edit_media_info",
             "feed_position": "0",
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "usertags": json.dumps({"in": usertags}),
             "is_carousel_bumped_post": "false",
         }
         if media.product_type == "igtv":
             if not title:
                 try:
                     title, caption = caption.split("\n", 1)
@@ -391,15 +393,16 @@
             If liked, whether or not to unlike. Default is False
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_pk(media_id)
         data = {
             "inventory_source": "media_or_ad",
             "media_id": media_id,
             "radio_type": "wifi-none",
             "is_carousel_bumped_post": "false",
             "container_module": "feed_timeline",
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/notification.py` & `aiograpi-0.0.2/aiograpi/mixins/notification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from aiograpi.exceptions import UnsupportedSettingValue
+
 MUTE_ALL_ITEMS = ("cancel", "15_minutes", "1_hour", "2_hour", "4_hour", "8_hour")
 SETTING_VALUE_ITEMS = ("off", "following_only", "everyone")
 
 try:
     from typing import Literal
 
     MUTE_ALL = Literal[MUTE_ALL_ITEMS]
@@ -76,17 +78,16 @@
         setting_value: MUTE_ALL
             Value of settings, default "8_hour"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in MUTE_ALL_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {MUTE_ALL_ITEMS}'
+        if setting_value not in MUTE_ALL_ITEMS:
+            raise UnsupportedSettingValue(setting_value, MUTE_ALL_ITEMS)
         return await self.notification_settings("mute_all", setting_value)
 
     async def notification_likes(self, setting_value: SETTING_VALUE = "off") -> bool:
         """
         Manage Likes Notification Settings
 
         Parameters
@@ -94,17 +95,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("likes", setting_value)
 
     async def notification_like_and_comment_on_photo_user_tagged(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Like And Comment On Photo User Tagged Settings
@@ -114,17 +114,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings(
             "like_and_comment_on_photo_user_tagged", setting_value
         )
 
     async def notification_user_tagged(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
@@ -136,17 +135,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("user_tagged", setting_value)
 
     async def notification_comments(self, setting_value: SETTING_VALUE = "off") -> bool:
         """
         Manage Comments Notification Settings
 
         Parameters
@@ -154,17 +152,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("comments", setting_value)
 
     async def notification_comment_likes(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Comment Likes Notification Settings
@@ -174,17 +171,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("comment_likes", setting_value)
 
     async def notification_first_post(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage First Post Notification Settings
@@ -194,17 +190,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("first_post", setting_value)
 
     async def notification_new_follower(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage New Follower Notification Settings
@@ -214,17 +209,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("new_follower", setting_value)
 
     async def notification_follow_request_accepted(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Follow Request Accepted Notification Settings
@@ -234,17 +228,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings(
             "follow_request_accepted", setting_value
         )
 
     async def notification_connection(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
@@ -256,17 +249,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings(
             "connection_notification", setting_value
         )
 
     async def notification_tagged_in_bio(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
@@ -278,17 +270,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("tagged_in_bio", setting_value)
 
     async def notification_pending_direct_share(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Pending Direct Share Notification Settings
@@ -298,17 +289,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("pending_direct_share", setting_value)
 
     async def notification_direct_share_activity(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Direct Share Activity Notification Settings
@@ -318,17 +308,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("direct_share_activity", setting_value)
 
     async def notification_direct_group_requests(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Direct Group Requests Notification Settings
@@ -338,17 +327,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("direct_group_requests", setting_value)
 
     async def notification_video_call(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Video Call Notification Settings
@@ -358,17 +346,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("video_call", setting_value)
 
     async def notification_rooms(self, setting_value: SETTING_VALUE = "off") -> bool:
         """
         Manage Rooms Notification Settings
 
         Parameters
@@ -376,17 +363,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("rooms", setting_value)
 
     async def notification_live_broadcast(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Live Broadcast Notification Settings
@@ -396,17 +382,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("live_broadcast", setting_value)
 
     async def notification_felix_upload_result(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Felix Upload Result Notification Settings
@@ -416,17 +401,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("felix_upload_result", setting_value)
 
     async def notification_view_count(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage View Count Notification Settings
@@ -436,17 +420,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("view_count", setting_value)
 
     async def notification_fundraiser_creator(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Fundraiser Creator Notification Settings
@@ -456,17 +439,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("fundraiser_creator", setting_value)
 
     async def notification_fundraiser_supporter(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Fundraiser Supporter Notification Settings
@@ -476,17 +458,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("fundraiser_supporter", setting_value)
 
     async def notification_reminders(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Notification Reminders Settings
@@ -496,17 +477,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("notification_reminders", setting_value)
 
     async def notification_announcements(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Announcements Notification Settings
@@ -516,17 +496,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("announcements", setting_value)
 
     async def notification_report_updated(
         self, setting_value: SETTING_VALUE = "off"
     ) -> bool:
         """
         Manage Report Updated Notification Settings
@@ -536,17 +515,16 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("report_updated", setting_value)
 
     async def notification_login(self, setting_value: SETTING_VALUE = "off") -> bool:
         """
         Manage Login Notification Settings
 
         Parameters
@@ -554,11 +532,10 @@
         setting_value: SETTING_VALUE
             Value of settings, default "off"
 
         Returns
         -------
         bool
         """
-        assert (
-            setting_value in SETTING_VALUE_ITEMS
-        ), f'Unsupported setting_value="{setting_value}" {SETTING_VALUE_ITEMS}'
+        if setting_value not in SETTING_VALUE_ITEMS:
+            raise UnsupportedSettingValue(setting_value, SETTING_VALUE_ITEMS)
         return await self.notification_settings("login_notification", setting_value)
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/password.py` & `aiograpi-0.0.2/aiograpi/mixins/password.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/photo.py` & `aiograpi-0.0.2/aiograpi/mixins/photo.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
         Returns
         -------
         Path
             Path for the file downloaded
         """
         media = await self.media_info(media_pk)
-        assert media.media_type == 1, "Must been photo"
+        if media.media_type != 1:
+            raise Exception("Must been photo")
         filename = "{username}_{media_pk}".format(
             username=media.user.username, media_pk=media_pk
         )
         return await self.photo_download_by_url(media.thumbnail_url, filename, folder)
 
     async def photo_download_by_url(
         self, url: str, filename: str = "", folder: Path = ""
@@ -131,18 +132,20 @@
         to_album: bool, optional
 
         Returns
         -------
         tuple
             (Upload ID for the media, width, height)
         """
-        assert isinstance(path, Path), f"Path must been Path, now {path} ({type(path)})"
+        if not isinstance(path, Path):
+            raise Exception(f"Path must been Path, now {path} ({type(path)})")
         # upload_id = 516057248854759
         upload_id = upload_id or str(int(time.time() * 1000))
-        assert path, "Not specified path to photo"
+        if not path:
+            raise Exception("Not specified path to photo")
         waterfall_id = str(uuid4())
         # upload_name example: '1576102477530_0_7823256191'
         upload_name = "{upload_id}_0_{rand}".format(
             upload_id=upload_id, rand=random.randint(1000000000, 9999999999)
         )
         # media_type: "2" when from video/igtv/album thumbnail, "1" - upload photo only
         rupload_params = {
@@ -221,25 +224,25 @@
             An object of Media class
         """
         path = Path(path)
         upload_id, width, height = await self.photo_rupload(path, upload_id)
         for attempt in range(10):
             self.logger.debug(f"Attempt #{attempt} to configure Photo: {path}")
             await asyncio.sleep(3)
-            if self.photo_configure(
+            if await self.photo_configure(
                 upload_id,
                 width,
                 height,
                 caption,
                 usertags,
                 location,
                 extra_data=extra_data,
             ):
                 media = self.last_json.get("media")
-                self.expose()
+                await self.expose()
                 return extract_media_v1(media)
         raise PhotoConfigureError(response=self.last_response, **self.last_json)
 
     async def photo_configure(
         self,
         upload_id: str,
         width: int,
@@ -285,15 +288,15 @@
             "nav_chain": "8rL:self_profile:4,ProfileMediaTabFragment:self_profile:5,UniversalCreationMenuFragment:universal_creation_menu:7,ProfileMediaTabFragment:self_profile:8,MediaCaptureFragment:tabbed_gallery_camera:9,Dd3:photo_filter:10,FollowersShareFragment:metadata_followers_share:11",
             "date_time_original": date_time_original(time.localtime()),
             "date_time_digitalized": date_time_original(time.localtime()),
             "creation_logger_session_id": self.client_session_id,
             "scene_capture_type": "standard",
             "software": config.SOFTWARE.format(**self.device_settings),
             "multi_sharing": "1",
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "media_folder": "Camera",
             "source_type": "4",
             "caption": caption,
             "upload_id": upload_id,
             "device": self.device,
             "usertags": json.dumps({"in": usertags}),
             "edits": {
@@ -367,15 +370,15 @@
                 links,
                 hashtags,
                 stickers,
                 medias,
                 extra_data=extra_data,
             ):
                 media = self.last_json.get("media")
-                self.expose()
+                await self.expose()
                 return Story(
                     links=links,
                     mentions=mentions,
                     hashtags=hashtags,
                     locations=locations,
                     stickers=stickers,
                     medias=medias,
@@ -592,15 +595,16 @@
                         **sticker_extra,
                     }
                 )
                 if sticker.type == "gif":
                     data["has_animated_sticker"] = "1"
         if medias:
             for feed_media in medias:
-                assert feed_media.media_pk, "Required StoryMedia.media_pk"
+                if not feed_media.media_pk:
+                    raise Exception("Required StoryMedia.media_pk")
                 # if not feed_media.user_id:
                 #     user = self.media_user(feed_media.media_pk)
                 #     feed_media.user_id = user.pk
                 item = {
                     "x": feed_media.x,
                     "y": feed_media.y,
                     "z": feed_media.z,
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/private.py` & `aiograpi-0.0.2/aiograpi/mixins/private.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import asyncio
 import json
 import logging
 import random
 import time
+
 import orjson
 
-from aiograpi import reqwests
-from aiograpi import config
+from aiograpi import config, reqwests
 from aiograpi.exceptions import (
+    AuthRequiredProxyError,
     BadPassword,
     ChallengeRequired,
     CheckpointRequired,
     ClientBadRequestError,
     ClientConnectionError,
-    GeoBlockRequired,
-    HashtagPageWarning,
-    UserNotFound,
+    ClientErrorWithTitle,
     ClientForbiddenError,
     ClientJSONDecodeError,
     ClientNotFoundError,
     ClientRequestTimeout,
+    ClientStatusFail,
     ClientThrottledError,
+    ClientUnknownError,
+    CommentsDisabled,
+    ConnectProxyError,
     ConsentRequired,
     FeedbackRequired,
+    GeoBlockRequired,
+    HashtagPageWarning,
+    InvalidMediaId,
+    InvalidTargetUser,
     LoginRequired,
+    MediaUnavailable,
     PleaseWaitFewMinutes,
     PrivateAccount,
     ProxyAddressIsBlocked,
     RateLimitError,
     SentryBlock,
     TwoFactorRequired,
-    InvalidTargetUser,
-    CommentsDisabled,
-    InvalidMediaId,
-    MediaUnavailable,
     UnknownError,
+    UserNotFound,
     VideoTooLongException,
-    ClientStatusFail,
-    ClientErrorWithTitle,
-    ClientUnknownError,
-    AuthRequiredProxyError,
-    ConnectProxyError,
 )
 from aiograpi.utils import dumps, generate_signature, random_delay
 
 
 async def manual_input_code(self, username: str, choice=None):
     """
     Manual security code helper
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/public.py` & `aiograpi-0.0.2/aiograpi/mixins/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import asyncio
+import json
 import logging
 import time
-import json
 
 import orjson
 
 from aiograpi import reqwests
 from aiograpi.exceptions import (
-    ClientUnauthorizedError,
+    AboutUsError,
+    AccountSuspended,
+    ChallengeRequired,
     ClientBadRequestError,
     ClientConnectionError,
     ClientError,
     ClientForbiddenError,
     ClientGraphqlError,
     ClientJSONDecodeError,
     ClientLoginRequired,
     ClientNotFoundError,
     ClientThrottledError,
-    ChallengeRequired,
-    AccountSuspended,
-    TermsUnblock,
+    ClientUnauthorizedError,
     TermsAccept,
-    AboutUsError,
+    TermsUnblock,
 )
 from aiograpi.utils import random_delay
 
 
 class PublicRequestMixin:
     public_requests_count = 0
     PUBLIC_API_URL = "https://www.instagram.com/"
@@ -68,16 +68,18 @@
     ):
         kwargs = dict(
             data=data,
             params=params,
             headers=headers,
             return_json=return_json,
         )
-        assert retries_count <= 10, "Retries count is too high"
-        assert retries_timeout <= 600, "Retries timeout is too high"
+        if retries_count > 10:
+            raise Exception("Retries count is too high")
+        if retries_timeout > 600:
+            raise Exception("Retries timeout is too high")
         for iteration in range(retries_count):
             try:
                 if self.delay_range:
                     await random_delay(delay_range=self.delay_range)
                 return await self._send_public_request(url, **kwargs)
             except (
                 ClientLoginRequired,
@@ -198,15 +200,16 @@
         variables,
         query_hash=None,
         query_id=None,
         data=None,
         params=None,
         headers=None,
     ):
-        assert query_id or query_hash, "Must provide valid one of: query_id, query_hash"
+        if not (query_id or query_hash):
+            raise Exception("Must provide valid one of: query_id, query_hash")
         default_params = {"variables": json.dumps(variables, separators=(",", ":"))}
         if query_id:
             # 17851374694183129
             default_params["query_id"] = query_id
         if query_hash:
             # 7dd9a7e2160524fd85f50317462cff9f
             default_params["query_hash"] = query_hash
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/share.py` & `aiograpi-0.0.2/aiograpi/mixins/share.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/signup.py` & `aiograpi-0.0.2/aiograpi/mixins/signup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,38 @@
         email: str = "",
         phone_number: str = "",
         full_name: str = "",
         year: int = None,
         month: int = None,
         day: int = None,
     ) -> UserShort:
-        assert email or phone_number, "Use email or phone_number"
+        if not (email or phone_number):
+            raise Exception("Use email or phone_number")
         check = await self.check_username(username)
-        assert check.get("available"), f"Username is't available ({check})"
+        if not check.get("available"):
+            raise Exception(f"Username is't available ({check})")
         kwargs = {
             "username": username,
             "password": password,
             "full_name": full_name,
             "year": year,
             "month": month,
             "day": day,
         }
         if email:
             kwargs["email"] = email
             check = await self.check_email(email)
-            assert check.get("valid"), f"Email not valid ({check})"
-            assert check.get("available"), f"Email not available ({check})"
+            if not check.get("valid"):
+                raise Exception(f"Email not valid ({check})")
+            if not check.get("available"):
+                raise Exception(f"Email not available ({check})")
             config = await self.get_signup_config()
             sent = await self.send_verify_email(email)
-            assert sent.get("email_sent"), "Email not sent ({sent})"
+            if not sent.get("email_sent"):
+                raise Exception("Email not sent ({sent})")
             # send code confirmation
             code = ""
             for attempt in range(1, 11):
                 code = await self.challenge_code_handler(
                     username, ChallengeChoice.EMAIL
                 )
                 if code:
@@ -61,19 +66,19 @@
             kwargs["email_code"] = self.check_confirmation_code(email, code).get(
                 "signup_code"
             )
         if phone_number:
             kwargs["phone_number"] = phone_number
             config = await self.get_signup_config()
             check = await self.check_phone_number(phone_number)
-            assert check.get("status") == "ok", f"Phone number not valid ({check})"
+            if check.get("status") != "ok":
+                raise Exception(f"Phone number not valid ({check})")
             sms = await self.send_signup_sms_code(phone_number)
-            assert (
-                check.get("status") == "ok"
-            ), f"Error when verify phone number ({sms})"
+            if check.get("status") != "ok":
+                raise Exception(f"Error when verify phone number ({sms})")
             if "verification_code" in sms:
                 # when you have multiple accounts
                 code = sms["verification_code"]
             else:
                 for attempt in range(1, 11):
                     code = await self.challenge_code_handler(
                         username, ChallengeChoice.SMS
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/story.py` & `aiograpi-0.0.2/aiograpi/mixins/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 from pathlib import Path
 from typing import List
 from urllib.parse import urlparse
 
 from aiograpi import config
 from aiograpi.exceptions import (
     ClientNotFoundError,
-    UserNotFound,
-    StoryNotFound,
+    PreLoginRequired,
     PrivateError,
+    StoryNotFound,
+    UserNotFound,
 )
-from aiograpi.extractors import (
-    extract_story_gql,
-    extract_story_v1,
-    extract_user_short,
-)
+from aiograpi.extractors import extract_story_gql, extract_story_v1, extract_user_short
 from aiograpi.types import Story, UserShort
 
 
 class StoryMixin:
     def story_pk_from_url(self, url: str) -> str:
         """
         Get Story (media) PK from URL
@@ -94,15 +91,16 @@
             Unique identifier of the story
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_id(story_pk)
         return await self.media_delete(media_id)
 
     async def users_stories_gql(
         self, user_ids: List[str], amount: int = 0
     ) -> List[UserShort]:
         """
@@ -119,15 +117,16 @@
         -------
         List[UserShort]
             A list of objects of UserShort for each user_id
         """
         self.inject_sessionid_to_public()
 
         def _userid_chunks():
-            assert user_ids is not None
+            if user_ids is None:
+                raise Exception("Undefined user_ids")
             user_ids_per_query = 50
             for i in range(0, len(user_ids), user_ids_per_query):
                 end = i + user_ids_per_query
                 yield user_ids[i:end]
 
         stories_un = {}
         for userid_chunk in _userid_chunks():
@@ -280,15 +279,16 @@
 
         Returns
         -------
         Path
             Path for the file downloaded
         """
         fname = urlparse(url).path.rsplit("/", 1)[1].strip()
-        assert fname, "The URL must contain the path to the file (mp4 or jpg)"
+        if not fname:
+            raise Exception("The URL must contain the path to the file (mp4 or jpg)")
         filename = "%s.%s" % (filename, fname.rsplit(".", 1)[1]) if filename else fname
         path = Path(folder) / filename
         response = await self.public.get(url)
         response.raise_for_status()
         with open(path, "wb") as f:
             f.write(response.read())
         return path.resolve()
@@ -347,15 +347,16 @@
             If liked, whether or not to unlike. Default is False
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         media_id = await self.media_id(story_id)
         data = {
             "media_id": media_id,
             "_uid": str(self.user_id),
             "source_of_like": "button",
             "tray_session_id": self.tray_session_id,
             "viewer_session_id": self.client_session_id,
@@ -398,9 +399,10 @@
             "_uuid": self.uuid,
         }
         result = await self.private_request(
             "creatives/sticker_tray/",
             data=data,
             with_signature=True,
         )
-        assert result["status"] == "ok"
+        if result["status"] != "ok":
+            raise Exception("Sticker not ok")
         return result
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/timeline.py` & `aiograpi-0.0.2/aiograpi/mixins/timeline.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/totp.py` & `aiograpi-0.0.2/aiograpi/mixins/totp.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/mixins/track.py` & `aiograpi-0.0.2/aiograpi/mixins/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any, Dict
 from pathlib import Path
+from typing import Any, Dict
 from urllib.parse import urlparse
 
 from aiograpi import reqwests
 from aiograpi.exceptions import ClientError, TrackNotFound
 
 
 class TrackMixin:
@@ -25,15 +25,16 @@
 
         Returns
         -------
         Path
             Path for the file downloaded
         """
         fname = urlparse(url).path.rsplit("/", 1)[1].strip()
-        assert fname, """The URL must contain the path to the file (m4a or mp3)."""
+        if not fname:
+            raise Exception("The URL must contain the path to the file (m4a or mp3).")
         filename = "%s.%s" % (filename, fname.rsplit(".", 1)[1]) if filename else fname
         path = Path(folder) / filename
         response = await reqwests.get(url, timeout=self.request_timeout)
         response.raise_for_status()
         with open(path, "wb") as f:
             f.write(response.read())
         return path.resolve()
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/user.py` & `aiograpi-0.0.2/aiograpi/mixins/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 from orjson import JSONDecodeError
 
 from aiograpi.exceptions import (
     ClientError,
     ClientJSONDecodeError,
     ClientLoginRequired,
     ClientNotFoundError,
-    UserNotFound,
-    PrivateError,
     ClientStatusFail,
     IsRegulatedC18Error,
+    PreLoginRequired,
+    PrivateError,
+    UserNotFound,
 )
 from aiograpi.extractors import (
+    extract_about_v1,
+    extract_guide_v1,
     extract_user_gql,
     extract_user_short,
     extract_user_v1,
-    extract_guide_v1,
-    extract_about_v1,
 )
-from aiograpi.types import About, Guide, Relationship, User, UserShort
+from aiograpi.types import (
+    About,
+    Guide,
+    Relationship,
+    RelationshipShort,
+    User,
+    UserShort,
+)
 from aiograpi.utils import dumps, json_value
 
-
 logger = logging.getLogger(__name__)
 
 
 class UserMixin:
     async def user_id_from_username(self, username: str) -> str:
         """
         Get full media id
@@ -338,31 +345,41 @@
         -------
         True if new feed exist ,
         After Login or load Settings always return False
         """
         results = await self.private_request("feed/new_feed_posts_exist/")
         return results.get("new_feed_posts_exist", False)
 
-    async def user_friendships_v1(self, user_ids: List[str]) -> dict:
+    async def user_friendships_v1(self, user_ids: List[str]) -> List[RelationshipShort]:
         """
         Get user friendship status
 
         Parameters
         ----------
         user_ids: List[str]
-            List of user id of an instagram account
+            List of user ID of an instagram account
 
         Returns
         -------
-        dict
+        List[RelationshipShort]
+           List of RelationshipShorts with requested user_ids
         """
+        user_ids_str = ",".join(user_ids)
         result = await self.private_request(
-            "friendships/show_many/", data={"user_ids": user_ids}
+            "friendships/show_many/",
+            data={"user_ids": user_ids_str, "_uuid": self.uuid},
+            with_signature=False,
         )
-        return result["friendship_statuses"]
+        assert result.get("status", "") == "ok"
+
+        relationships = []
+        for user_id, status in result.get("friendship_statuses", {}).items():
+            relationships.append(RelationshipShort(user_id=user_id, **status))
+
+        return relationships
 
     async def user_friendship_v1(self, user_id: str) -> Relationship:
         """
         Get user friendship status
 
         Parameters
         ----------
@@ -372,20 +389,58 @@
         Returns
         -------
         Relationship
             An object of Relationship type
         """
 
         try:
-            results = await self.private_request(f"friendships/show/{user_id}/")
-            return Relationship(**results)
+            result = await self.private_request(f"friendships/show/{user_id}/")
+            assert result.get("status", "") == "ok"
+
+            return Relationship(user_id=user_id, **result)
         except ClientError as e:
             self.logger.exception(e)
             return None
 
+    async def search_users_v1(self, query: str, count: int) -> List[UserShort]:
+        """
+        Search users by a query (Private Mobile API)
+        Parameters
+        ----------
+        query: str
+            Query to search
+        count: int
+            The count of search results
+        Returns
+        -------
+        List[UserShort]
+            List of users
+        """
+        results = await self.private_request(
+            "users/search/", params={"query": query, "count": count}
+        )
+        users = results.get("users", [])
+        return [extract_user_short(user) for user in users]
+
+    async def search_users(self, query: str, count: int = 50) -> List[UserShort]:
+        """
+        Search users by a query
+        Parameters
+        ----------
+        query: str
+            Query string to search
+        count: int
+            The count of search results
+        Returns
+        -------
+        List[UserShort]
+            List of User short object
+        """
+        return await self.search_users_v1(query, count)
+
     async def search_followers_v1(self, user_id: str, query: str) -> List[UserShort]:
         """
         Search users by followers (Private Mobile API)
 
         Parameters
         ----------
         user_id: str
@@ -853,15 +908,16 @@
         user_id: str
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         if user_id in self._users_following.get(self.user_id, []):
             self.logger.debug("User %s already followed", user_id)
             return False
         data = self.with_action_data({"user_id": user_id})
         result = await self.private_request(f"friendships/create/{user_id}/", data)
         if self.user_id in self._users_following:
@@ -877,15 +933,16 @@
         user_id: str
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": user_id})
         result = await self.private_request(f"friendships/destroy/{user_id}/", data)
         if self.user_id in self._users_following:
             self._users_following[self.user_id].pop(user_id, None)
         return result["friendship_status"]["following"] is False
 
@@ -898,15 +955,16 @@
         user_id: str
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": str(user_id)})
         result = await self.private_request(
             f"friendships/remove_follower/{user_id}/", data
         )
         if self.user_id in self._users_followers:
             self._users_followers[self.user_id].pop(user_id, None)
@@ -1016,15 +1074,16 @@
             Unfavorite when True
 
         Returns
         -------
         bool
             A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": user_id, "_uid": self.user_id})
         name = "unfavorite" if disable else "favorite"
         result = await self.private_request(f"friendships/{name}/{user_id}/", data)
         return result["status"] == "ok"
 
     async def disable_posts_notifications(self, user_id: str) -> bool:
@@ -1056,15 +1115,16 @@
             Unfavorite when True
 
         Returns
         -------
         bool
         A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": user_id, "_uid": self.user_id})
         name = "unfavorite" if revert else "favorite"
         result = await self.private_request(
             f"friendships/{name}_for_igtv/{user_id}/", data
         )
         return result["status"] == "ok"
@@ -1098,15 +1158,16 @@
             Unfavorite when True
 
         Returns
         -------
         bool
         A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": user_id, "_uid": self.user_id})
         name = "unfavorite" if revert else "favorite"
         result = await self.private_request(
             f"friendships/{name}_for_clips/{user_id}/", data
         )
         return result["status"] == "ok"
@@ -1140,15 +1201,16 @@
             Unfavorite when True
 
         Returns
         -------
         bool
         A boolean value
         """
-        assert self.user_id, "Login required"
+        if not self.user_id:
+            raise PreLoginRequired
         user_id = str(user_id)
         data = self.with_action_data({"user_id": user_id, "_uid": self.user_id})
         name = "unfavorite" if revert else "favorite"
         result = await self.private_request(
             f"friendships/{name}_for_stories/{user_id}/", data
         )
         return result["status"] == "ok"
```

### Comparing `aiograpi-0.0.1/aiograpi/mixins/video.py` & `aiograpi-0.0.2/aiograpi/mixins/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
         Returns
         -------
         Path
             Path for the file downloaded
         """
         media = await self.media_info(media_pk)
-        assert media.media_type == 2, "Must been video"
+        if media.media_type != 2:
+            raise Exception("Must been video")
         filename = "{username}_{media_pk}".format(
             username=media.user.username, media_pk=media_pk
         )
         return await self.video_download_by_url(media.video_url, filename, folder)
 
     async def video_download_by_url(
         self, url: str, filename: str = "", folder: Path = ""
@@ -147,15 +148,16 @@
         to_direct: bool, optional
 
         Returns
         -------
         tuple
             (Upload ID for the media, width, height)
         """
-        assert isinstance(path, Path), f"Path must been Path, now {path} ({type(path)})"
+        if not isinstance(path, Path):
+            raise Exception(f"Path must been Path, now {path} ({type(path)})")
         upload_id = str(int(time.time() * 1000))
         width, height, duration, thumbnail = analyze_video(path, thumbnail)
         waterfall_id = str(uuid4())
         # upload_name example: '1576102477530_0_7823256191'
         upload_name = "{upload_id}_0_{rand}".format(
             upload_id=upload_id, rand=random.randint(1000000000, 9999999999)
         )
@@ -284,15 +286,15 @@
                     """
                     await asyncio.sleep(10)
                     continue
                 raise e
             else:
                 if configured:
                     media = configured.get("media")
-                    self.expose()
+                    await self.expose()
                     return extract_media_v1(media)
         raise VideoConfigureError(response=self.last_response, **self.last_json)
 
     async def video_configure(
         self,
         upload_id: str,
         width: int,
@@ -338,15 +340,15 @@
             {"user_id": tag.user.pk, "position": [tag.x, tag.y]} for tag in usertags
         ]
         data = {
             "multi_sharing": "1",
             "creation_logger_session_id": self.client_session_id,
             "upload_id": upload_id,
             "source_type": "4",
-            "location": self.location_build(location),
+            "location": await self.location_build(location),
             "poster_frame_index": 0,
             "length": duration,
             "audio_muted": False,
             "usertags": dumps({"in": usertags}),
             "filter_type": "0",
             "date_time_original": date_time_original(time.localtime()),
             "timezone_offset": str(self.timezone_offset),
@@ -436,15 +438,15 @@
                     {"message": "Transcode not finished yet.", "status": "fail"}
                     """
                     await asyncio.sleep(10)
                     continue
                 raise e
             if configured:
                 media = configured.get("media")
-                self.expose()
+                await self.expose()
                 return Story(
                     links=links,
                     mentions=mentions,
                     hashtags=hashtags,
                     locations=locations,
                     stickers=stickers,
                     medias=medias,
@@ -731,15 +733,16 @@
                         **sticker_extra,
                     }
                 )
                 if sticker.type == "gif":
                     data["has_animated_sticker"] = "1"
         if medias:
             for feed_media in medias:
-                assert feed_media.media_pk, "Required StoryMedia.media_pk"
+                if not feed_media.media_pk:
+                    raise Exception("Required StoryMedia.media_pk")
                 # if not feed_media.user_id:
                 #     user = await self.media_user(feed_media.media_pk)
                 #     feed_media.user_id = user.pk
                 item = {
                     "x": feed_media.x,
                     "y": feed_media.y,
                     "z": feed_media.z,
```

### Comparing `aiograpi-0.0.1/aiograpi/reqwests.py` & `aiograpi-0.0.2/aiograpi/reqwests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import httpx
 import orjson
 import zstandard as zstd
-
 from httpx import (
-    HTTPError,
-    RequestError,
-    TransportError,
-    TimeoutException,
+    CloseError,
+    ConnectError,
     ConnectTimeout,
-    ReadTimeout,
-    WriteTimeout,
-    PoolTimeout,
+    CookieConflict,
+    DecodingError,
+    HTTPError,
+    HTTPStatusError,
+    InvalidURL,
+    LocalProtocolError,
     NetworkError,
-    ConnectError,
-    ReadError,
-    WriteError,
-    CloseError,
+    PoolTimeout,
     ProtocolError,
-    LocalProtocolError,
-    RemoteProtocolError,
     ProxyError,
-    UnsupportedProtocol,
-    DecodingError,
+    ReadError,
+    ReadTimeout,
+    RemoteProtocolError,
+    RequestError,
+    TimeoutException,
     TooManyRedirects,
-    HTTPStatusError,
-    InvalidURL,
-    CookieConflict,
+    TransportError,
+    UnsupportedProtocol,
+    WriteError,
+    WriteTimeout,
 )
-from httpx._decoders import SUPPORTED_DECODERS, ContentDecoder
 from httpx._client import ClientState
-
+from httpx._decoders import SUPPORTED_DECODERS, ContentDecoder
 
 httpx.Response.json = lambda self: orjson.loads(self.content)
 
 
 class ZstdDecoder(ContentDecoder):
     def __init__(self) -> None:
         self.decompressor = zstd.ZstdDecompressor().decompressobj()
```

### Comparing `aiograpi-0.0.1/aiograpi/story.py` & `aiograpi-0.0.2/aiograpi/story.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi/types.py` & `aiograpi-0.0.2/aiograpi/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 
-from pydantic import BaseModel, FilePath, ValidationError, validator  # ConfigDict
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    FilePath,
+    HttpUrl,
+    ValidationError,
+    validator,
+)
+
+
+class TypesBaseModel(BaseModel):
+    model_config = ConfigDict(
+        coerce_numbers_to_str=True
+    )  # (jarrodnorwell) fixed city_id issue
 
 
 def validate_external_url(cls, v):
     if v is None or (v.startswith("http") and "://" in v) or isinstance(v, str):
         return v
     raise ValidationError("external_url must been URL or string")
 
 
-# class TypesBaseModel(BaseModel):
-#     model_config = ConfigDict(
-#         coerce_numbers_to_str=True
-#     )
-
-
-class Resource(BaseModel):
+class Resource(TypesBaseModel):
     pk: str
-    video_url: Optional[str] = None  # for Video and IGTV
-    thumbnail_url: str
+    video_url: Optional[HttpUrl] = None  # for Video and IGTV
+    thumbnail_url: HttpUrl
     media_type: int
     image_versions: List[dict] = []
     video_versions: List[dict] = []
 
 
-class User(BaseModel):
+class BioLink(TypesBaseModel):
+    link_id: str
+    url: str
+    lynx_url: Optional[str] = None
+    link_type: Optional[str] = None
+    title: Optional[str] = None
+    is_pinned: Optional[bool] = None
+    open_external_url_with_in_app_browser: Optional[bool] = None
+
+
+class User(TypesBaseModel):
     pk: str
     username: str
     full_name: Optional[str] = None
     is_private: Optional[bool] = None
-    profile_pic_url: str
-    profile_pic_url_hd: Optional[str] = None
+    profile_pic_url: HttpUrl
+    profile_pic_url_hd: Optional[HttpUrl] = None
     is_verified: Optional[bool] = None
     media_count: Optional[int] = None
     follower_count: Optional[int] = None
     following_count: Optional[int] = None
     biography: Optional[str] = ""
+    bio_links: List[BioLink] = []
     external_url: Optional[str] = None
     account_type: Optional[int] = None
     is_business: Optional[bool] = None
 
     public_email: Optional[str] = None
     contact_phone_number: Optional[str] = None
     public_phone_country_code: Optional[str] = None
@@ -58,312 +76,369 @@
     zip: Optional[str] = None
     instagram_location_id: Optional[str] = None
     interop_messaging_user_fbid: Optional[str] = None
 
     _external_url = validator("external_url", allow_reuse=True)(validate_external_url)
 
 
-class About(BaseModel):
+class About(TypesBaseModel):
     username: Optional[str] = ""
     is_verified: Optional[bool] = False
     country: Optional[str] = ""
     date: Optional[str] = ""
     former_usernames: Optional[str] = ""
 
 
-class Account(BaseModel):
+class Account(TypesBaseModel):
     pk: str
     username: str
     full_name: str
     is_private: bool
-    profile_pic_url: str
+    profile_pic_url: HttpUrl
     is_verified: bool
     biography: Optional[str] = ""
     external_url: Optional[str] = None
     is_business: bool
     birthday: Optional[str] = None
     phone_number: Optional[str] = None
     gender: Optional[int] = None
     email: Optional[str] = None
 
     _external_url = validator("external_url", allow_reuse=True)(validate_external_url)
 
 
-class UserShort(BaseModel):
+class UserShort(TypesBaseModel):
+    def __hash__(self):
+        return hash(self.pk)
+
+    def __eq__(self, other):
+        if isinstance(other, UserShort):
+            return self.pk == other.pk
+        return NotImplemented
+
     pk: str
     username: Optional[str] = None
     full_name: Optional[str] = ""
-    profile_pic_url: Optional[str] = None
-    profile_pic_url_hd: Optional[str] = None
+    profile_pic_url: Optional[HttpUrl] = None
+    profile_pic_url_hd: Optional[HttpUrl] = None
     is_private: Optional[bool] = None
     is_verified: Optional[bool] = None
 
 
-class Usertag(BaseModel):
+class Usertag(TypesBaseModel):
     user: UserShort
     x: float
     y: float
 
 
-class Location(BaseModel):
+class Location(TypesBaseModel):
     pk: Optional[int] = None
     name: str
     phone: Optional[str] = ""
     website: Optional[str] = ""
     category: Optional[str] = ""
     hours: Optional[dict] = {}  # opening hours
     address: Optional[str] = ""
     city: Optional[str] = ""
     zip: Optional[str] = ""
     lng: Optional[float] = None
     lat: Optional[float] = None
-    external_id: Optional[str] = None
+    external_id: Optional[int] = None
     external_id_source: Optional[str] = None
     # address_json: Optional[dict] = {}
     # profile_pic_url: Optional[str] = None
     # directory: Optional[dict] = {}
 
 
-class Media(BaseModel):
-    pk: str
+class Media(TypesBaseModel):
+    pk: Union[str, int]
     id: str
     code: str
     taken_at: datetime
     taken_at_ts: int
     media_type: int
+    image_versions2: Optional[dict] = {}
     product_type: Optional[str] = ""  # igtv or feed
-    thumbnail_url: Optional[str] = None
+    thumbnail_url: Optional[HttpUrl] = None
     location: Optional[Location] = None
     user: UserShort
     comment_count: Optional[int] = 0
     comments_disabled: Optional[bool] = False
+    commenting_disabled_for_viewer: Optional[bool] = False
     like_count: int
     play_count: Optional[int] = None
     has_liked: Optional[bool] = None
     caption_text: str
     accessibility_caption: Optional[str] = None
     usertags: List[Usertag]
     sponsor_tags: Optional[List[UserShort]] = []
-    video_url: Optional[str] = None  # for Video and IGTV
+    video_url: Optional[HttpUrl] = None  # for Video and IGTV
     view_count: Optional[int] = 0  # for Video and IGTV
     video_duration: Optional[float] = 0.0  # for Video and IGTV
     title: Optional[str] = ""
     resources: List[Resource] = []
     image_versions: List[dict] = []
     video_versions: List[dict] = []
     clips_metadata: dict = {}
     video_dash_manifest: Optional[str] = ""
     like_and_view_counts_disabled: Optional[bool] = None
     coauthor_producers: Optional[list] = []
     is_paid_partnership: Optional[bool] = None
 
 
-class MediaOembed(BaseModel):
+class MediaXma(TypesBaseModel):
+    # media_type: int
+    video_url: HttpUrl  # for Video and IGTV
+    title: Optional[str] = ""
+    preview_url: Optional[HttpUrl] = None
+    preview_url_mime_type: Optional[str] = None
+    header_icon_url: Optional[HttpUrl] = None
+    header_icon_width: Optional[int] = None
+    header_icon_height: Optional[int] = None
+    header_title_text: Optional[str] = None
+    preview_media_fbid: Optional[str] = None
+
+
+class MediaOembed(TypesBaseModel):
     title: str
     author_name: str
     author_url: str
     author_id: str
     media_id: str
     provider_name: str
-    provider_url: str
+    provider_url: HttpUrl
     type: str
     width: Optional[int] = None
     height: Optional[int] = None
     html: str
-    thumbnail_url: str
+    thumbnail_url: HttpUrl
     thumbnail_width: int
     thumbnail_height: int
     can_view: Optional[bool] = None
 
 
-class Collection(BaseModel):
+class Collection(TypesBaseModel):
     id: str
     name: str
     type: str
     media_count: int
 
 
-class Comment(BaseModel):
+class Comment(TypesBaseModel):
     pk: str
     text: str
     user: UserShort
     created_at_utc: datetime
     content_type: str
     status: str
+    replied_to_comment_id: Optional[str] = None
     has_liked: Optional[bool] = None
     like_count: Optional[int] = None
 
 
-class Hashtag(BaseModel):
+class Hashtag(TypesBaseModel):
     id: Optional[str] = None
     name: str
     media_count: Optional[int] = None
     allow_following: Optional[bool] = None
-    profile_pic_url: Optional[str] = None
+    profile_pic_url: Optional[HttpUrl] = None
 
 
-class StoryMention(BaseModel):
+class StoryMention(TypesBaseModel):
     user: UserShort
     x: Optional[float] = None
     y: Optional[float] = None
     width: Optional[float] = None
     height: Optional[float] = None
+    rotation: Optional[float] = None
 
 
-class StoryMedia(BaseModel):
+class StoryMedia(TypesBaseModel):
     # Instagram does not return the feed_media object when requesting story,
     # so you will have to make an additional request to get media and this is overhead:
     # media: Media
     x: float = 0.5
     y: float = 0.4997396
     z: float = 0
     width: float = 0.8
     height: float = 0.60572916
     rotation: float = 0.0
     is_pinned: Optional[bool] = None
     is_hidden: Optional[bool] = None
     is_sticker: Optional[bool] = None
     is_fb_sticker: Optional[bool] = None
-    media_pk: str
-    user_id: Optional[str] = None
+    media_pk: int
+    user_id: Optional[int] = None
     product_type: Optional[str] = None
     media_code: Optional[str] = None
 
 
-class StoryHashtag(BaseModel):
+class StoryHashtag(TypesBaseModel):
     hashtag: Hashtag
     x: Optional[float] = None
     y: Optional[float] = None
     width: Optional[float] = None
     height: Optional[float] = None
+    rotation: Optional[float] = None
 
 
-class StoryLocation(BaseModel):
+class StoryLocation(TypesBaseModel):
     location: Location
     x: Optional[float] = None
     y: Optional[float] = None
     width: Optional[float] = None
     height: Optional[float] = None
+    rotation: Optional[float] = None
 
 
-class StoryStickerLink(BaseModel):
-    url: Optional[str] = None
+class StoryStickerLink(TypesBaseModel):
+    url: Optional[HttpUrl] = None
     link_title: Optional[str] = None
     link_type: Optional[str] = None
     display_url: Optional[str] = None
 
 
-class StorySticker(BaseModel):
+class StorySticker(TypesBaseModel):
     id: Optional[str] = None
     type: Optional[str] = "gif"
     x: float
     y: float
     z: Optional[int] = 1000005
     width: float
     height: float
     rotation: Optional[float] = 0.0
     story_link: Optional[StoryStickerLink] = None
     extra: Optional[dict] = {}
 
 
-class StoryBuild(BaseModel):
+class StoryBuild(TypesBaseModel):
     mentions: List[StoryMention]
     path: FilePath
     paths: List[FilePath] = []
     stickers: List[StorySticker] = []
 
 
-class StoryLink(BaseModel):
-    webUri: str
+class StoryLink(TypesBaseModel):
+    webUri: HttpUrl
     x: float = 0.5126011
     y: float = 0.5168225
     z: float = 0.0
     width: float = 0.50998676
     height: float = 0.25875
     rotation: float = 0.0
 
 
-class Story(BaseModel):
+class Story(TypesBaseModel):
     pk: str
     id: str
     code: str
     taken_at: datetime
     media_type: Optional[int] = None
+    imported_taken_at: Optional[datetime] = None
+    media_type: int
     product_type: Optional[str] = ""
-    thumbnail_url: Optional[str] = None
+    thumbnail_url: Optional[HttpUrl] = None
     user: UserShort
-    video_url: Optional[str] = None  # for Video and IGTV
+    video_url: Optional[HttpUrl] = None  # for Video and IGTV
     video_duration: Optional[float] = 0.0  # for Video and IGTV
     sponsor_tags: Optional[List[UserShort]] = []
+    is_paid_partnership: Optional[bool]
     mentions: List[StoryMention]
     links: List[StoryLink]
     hashtags: List[StoryHashtag]
     locations: List[StoryLocation]
     stickers: List[StorySticker]
     medias: List[StoryMedia] = []
 
 
-class Guide(BaseModel):
+class Guide(TypesBaseModel):
     id: Optional[str] = None
     title: Optional[str] = None
     description: str
     cover_media: Media
     feedback_item: Optional[dict] = None
 
 
-class DirectMedia(BaseModel):
+class DirectMedia(TypesBaseModel):
     id: str
     media_type: int
-    user: Optional[UserShort]
-    thumbnail_url: Optional[str] = None
-    video_url: Optional[str] = None
+    user: Optional[UserShort] = None
+    thumbnail_url: Optional[HttpUrl] = None
+    video_url: Optional[HttpUrl] = None
+    audio_url: Optional[HttpUrl] = None
 
 
-class DirectMessage(BaseModel):
+class ReplyMessage(TypesBaseModel):
+    id: str
+    user_id: Optional[str] = None
+    timestamp: datetime
+    item_type: Optional[str] = None
+    is_sent_by_viewer: Optional[bool] = None
+    is_shh_mode: Optional[bool] = None
+    text: Optional[str] = None
+    link: Optional[dict] = None
+    animated_media: Optional[dict] = None
+    media: Optional[DirectMedia] = None
+    visual_media: Optional[dict] = None
+    media_share: Optional[Media] = None
+    reel_share: Optional[dict] = None
+    story_share: Optional[dict] = None
+    felix_share: Optional[dict] = None
+    xma_share: Optional[MediaXma] = None
+    clip: Optional[Media] = None
+    placeholder: Optional[dict] = None
+
+
+class DirectMessage(TypesBaseModel):
     id: str  # e.g. 28597946203914980615241927545176064
     user_id: Optional[str] = None
-    thread_id: Optional[str]  # e.g. 340282366841710300949128531777654287254
+    thread_id: Optional[int] = None  # e.g. 340282366841710300949128531777654287254
     timestamp: datetime
     item_type: Optional[str] = None
+    is_sent_by_viewer: Optional[bool] = None
     is_shh_mode: Optional[bool] = None
     reactions: Optional[dict] = None
     text: Optional[str] = None
+    reply: Optional[ReplyMessage] = None
     link: Optional[dict] = None
+    animated_media: Optional[dict] = None
     media: Optional[DirectMedia] = None
+    visual_media: Optional[dict] = None
     media_share: Optional[Media] = None
     reel_share: Optional[dict] = None
     story_share: Optional[dict] = None
     felix_share: Optional[dict] = None
-    clip: Optional[Media]
+    xma_share: Optional[MediaXma] = None
+    clip: Optional[Media] = None
     placeholder: Optional[dict] = None
 
 
-class DirectResponse(BaseModel):
+class DirectResponse(TypesBaseModel):
     unseen_count: Optional[int] = None
     unseen_count_ts: Optional[int] = None
     status: Optional[str] = None
 
 
-class DirectShortThread(BaseModel):
+class DirectShortThread(TypesBaseModel):
     id: str
     users: List[UserShort]
     named: bool
     thread_title: str
     pending: bool
     thread_type: str
     viewer_id: str
     is_group: bool
 
 
-class DirectThread(BaseModel):
+class DirectThread(TypesBaseModel):
     pk: str  # thread_v2_id, e.g. 17898572618026348
     id: str  # thread_id, e.g. 340282366841510300949128268610842297468
     messages: List[DirectMessage]
     users: List[UserShort]
-    inviter: Optional[UserShort]
+    inviter: Optional[UserShort] = None
     left_users: List[UserShort] = []
     admin_user_ids: list
     last_activity_at: datetime
     muted: bool
     is_pin: Optional[bool] = None
     named: bool
     canonical: bool
@@ -376,15 +451,15 @@
     is_group: bool
     mentions_muted: bool
     approval_required_for_new_members: bool
     input_mode: int
     business_thread_folder: int
     read_state: int
     is_close_friend_thread: bool
-    assigned_admin_id: str
+    assigned_admin_id: int
     shh_mode_enabled: bool
     last_seen_at: dict
 
     def is_seen(self, user_id: str):
         """Have I seen this thread?
         :param user_id: You account user_id
         """
@@ -394,62 +469,88 @@
             (int(v["timestamp"]) - own_timestamp) > 0
             for k, v in self.last_seen_at.items()
             if k != user_id
         ]
         return not any(timestamps)
 
 
-class Relationship(BaseModel):
+class Relationship(TypesBaseModel):
+    user_id: str
     blocking: bool
     followed_by: bool
     following: bool
     incoming_request: bool
     is_bestie: bool
     is_blocking_reel: bool
     is_muting_reel: bool
     is_private: bool
     is_restricted: bool
     muting: bool
     outgoing_request: bool
     status: str
 
 
-class Highlight(BaseModel):
+class RelationshipShort(TypesBaseModel):
+    user_id: str
+    following: bool
+    incoming_request: bool
+    is_bestie: bool
+    is_feed_favorite: bool
+    is_private: bool
+    is_restricted: bool
+    outgoing_request: bool
+
+
+class Highlight(TypesBaseModel):
     pk: str  # 17895485401104052
     id: str  # highlight:17895485401104052
     latest_reel_media: int
     cover_media: dict
     user: UserShort
     title: str
     created_at: datetime
     is_pinned_highlight: bool
     media_count: int
     media_ids: List[int] = []
     items: List[Story] = []
 
 
-class Share(BaseModel):
+class Share(TypesBaseModel):
     pk: str
     type: str
 
 
-class Track(BaseModel):
+class Track(TypesBaseModel):
     id: str
     title: str
     subtitle: str
     display_artist: str
-    audio_cluster_id: str
-    artist_id: Optional[str] = None
-    cover_artwork_uri: str
-    cover_artwork_thumbnail_uri: str
-    progressive_download_url: Optional[str] = None
-    fast_start_progressive_download_url: Optional[str] = None
-    reactive_audio_download_url: Optional[str] = None
+    audio_cluster_id: int
+    artist_id: Optional[int] = None
+    cover_artwork_uri: Optional[HttpUrl] = None
+    cover_artwork_thumbnail_uri: Optional[HttpUrl] = None
+    progressive_download_url: Optional[HttpUrl] = None
+    fast_start_progressive_download_url: Optional[HttpUrl] = None
+    reactive_audio_download_url: Optional[HttpUrl] = None
     highlight_start_times_in_ms: List[int]
     is_explicit: bool
     dash_manifest: str
+    uri: Optional[HttpUrl] = None
     has_lyrics: bool
-    audio_asset_id: str
+    audio_asset_id: int
     duration_in_ms: int
     dark_message: Optional[str] = None
     allows_saving: bool
     territory_validity_periods: Optional[dict] = None
+
+
+class Note(TypesBaseModel):
+    id: str
+    text: str
+    user_id: str
+    user: UserShort
+    audience: int
+    created_at: datetime
+    expires_at: datetime
+    is_emoji_only: bool
+    has_translation: bool
+    note_style: int
```

### Comparing `aiograpi-0.0.1/aiograpi/utils.py` & `aiograpi-0.0.2/aiograpi/utils.py`

 * *Files identical despite different names*

### Comparing `aiograpi-0.0.1/aiograpi.egg-info/PKG-INFO` & `aiograpi-0.0.2/aiograpi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: aiograpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous Instagram Private API wrapper
 Home-page: https://github.com/subzeroid/aiograpi
 Author: Mr.Robot
 Author-email: mr.robot@example.org
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader,instagram-note
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 Asynchronous Instagram Private API wrapper.
 
 Use the most recent version of the API from Instagram.
 
 Features:
```

### Comparing `aiograpi-0.0.1/aiograpi.egg-info/SOURCES.txt` & `aiograpi-0.0.2/aiograpi.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 aiograpi/__init__.py
 aiograpi/config.py
 aiograpi/exceptions.py
 aiograpi/extractors.py
 aiograpi/reqwests.py
@@ -28,14 +29,16 @@
 aiograpi/mixins/graphql.py
 aiograpi/mixins/hashtag.py
 aiograpi/mixins/highlight.py
 aiograpi/mixins/igtv.py
 aiograpi/mixins/insights.py
 aiograpi/mixins/location.py
 aiograpi/mixins/media.py
+aiograpi/mixins/multiple_accounts.py
+aiograpi/mixins/note.py
 aiograpi/mixins/notification.py
 aiograpi/mixins/password.py
 aiograpi/mixins/photo.py
 aiograpi/mixins/private.py
 aiograpi/mixins/public.py
 aiograpi/mixins/share.py
 aiograpi/mixins/signup.py
```

### Comparing `aiograpi-0.0.1/setup.py` & `aiograpi-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 4. Support work with User, Media, Insights, Collections, Location (Place), Hashtag and Direct objects
 5. Like, Follow, Edit account (Bio) and much more else
 6. Insights by account, posts and stories
 7. Build stories with custom background, font animation, swipe up link and mention users
 """
 
 requirements = [
-    "httpx==0.26.0",
-    "orjson==3.9.10",
-    "pydantic==2.5.2",
+    "httpx==0.27.0",
+    "orjson==3.10.0",
+    "pydantic==2.7.0",
     "moviepy==1.0.3",
-    "pycryptodomex==3.14.1",
-    "zstandard==0.21.0",
+    "pycryptodomex==3.20.0",
+    "zstandard==0.22.0",
 ]
 
 setup(
     name="aiograpi",
-    version="0.0.1",
+    version="0.0.2",
     author="Mr.Robot",
     author_email="mr.robot@example.org",
     license="MIT",
     url="https://github.com/subzeroid/aiograpi",
     install_requires=requirements,
     keywords=[
         "instagram private api",
@@ -69,13 +69,11 @@
     python_requires=">=3.10",
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

