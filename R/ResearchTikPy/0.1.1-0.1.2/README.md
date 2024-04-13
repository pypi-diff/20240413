# Comparing `tmp/ResearchTikPy-0.1.1.tar.gz` & `tmp/ResearchTikPy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ResearchTikPy-0.1.1.tar", last modified: Fri Apr 12 17:46:19 2024, max compression
+gzip compressed data, was "researchtikpy-0.1.2.tar", last modified: Sat Apr 13 15:59:22 2024, max compression
```

## Comparing `ResearchTikPy-0.1.1.tar` & `ResearchTikPy-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:46:19.253895 ResearchTikPy-0.1.1/
--rw-rw-rw-   0        0        0      383 2024-04-12 17:46:19.253895 ResearchTikPy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10915 2024-04-12 14:05:31.000000 ResearchTikPy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 17:46:19.252896 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/
--rw-rw-rw-   0        0        0      383 2024-04-12 17:46:19.000000 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-12 17:46:19.000000 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:46:19.000000 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 17:46:19.000000 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:46:19.000000 ResearchTikPy-0.1.1/ResearchTikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 17:46:19.254890 ResearchTikPy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      541 2024-04-12 17:45:51.000000 ResearchTikPy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:59:22.669587 researchtikpy-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      413 2024-04-13 15:59:22.668573 researchtikpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11190 2024-04-13 15:23:28.000000 researchtikpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 15:59:22.667243 researchtikpy-0.1.2/ResearchTikPy.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-13 15:59:22.000000 researchtikpy-0.1.2/ResearchTikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-04-13 15:59:22.000000 researchtikpy-0.1.2/ResearchTikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:59:22.000000 researchtikpy-0.1.2/ResearchTikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-13 15:59:22.000000 researchtikpy-0.1.2/ResearchTikPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-13 15:59:22.000000 researchtikpy-0.1.2/ResearchTikPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 15:59:22.666092 researchtikpy-0.1.2/researchtikpy/
+-rw-rw-rw-   0        0        0      577 2024-04-13 15:15:29.000000 researchtikpy-0.1.2/researchtikpy/__init__.py
+-rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.2/researchtikpy/get_followers.py
+-rw-rw-rw-   0        0        0     2782 2024-04-13 15:01:43.000000 researchtikpy-0.1.2/researchtikpy/get_following.py
+-rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.2/researchtikpy/get_liked_videos.py
+-rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.2/researchtikpy/get_pinned_videos.py
+-rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.2/researchtikpy/get_token.py
+-rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.2/researchtikpy/get_users_info.py
+-rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.2/researchtikpy/get_video_comments.py
+-rw-rw-rw-   0        0        0     3576 2024-04-13 15:02:43.000000 researchtikpy-0.1.2/researchtikpy/get_videos_hashtag.py
+-rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.2/researchtikpy/get_videos_info.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:59:22.670588 researchtikpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      541 2024-04-13 15:33:46.000000 researchtikpy-0.1.2/setup.py
```

### Comparing `ResearchTikPy-0.1.1/README.md` & `researchtikpy-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 
-
+![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)
+![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
+![PyPI Version](https://img.shields.io/pypi/v/ResearchTikPy.svg)
+![License](https://img.shields.io/badge/license-MIT-green.svg)
+![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/julian-hohner-71a93b163/)
+[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/J_H_ohner)
 
 
 <p align="middle">
   <img src="/images/Package_logo.png" width="400" /> <!-- Adjust width as needed -->
 </p>
 
 ResearchTikPy is a Python library designed to facilitate access to [TikTok's Research API](https://developers.tiktok.com/products/research-api/), providing a simple and intuitive interface for collecting data on videos, users, comments, and more. This library is intended for academic and research purposes, aiming to streamline the data collection process from TikTok without directly interfering with the API.
@@ -24,16 +29,14 @@
 
 ### Word of Caution 
 
 1. Splitting your requests into smaller chunks is generally advised to avoid longer fetching times and data loss.
 2. Read [TikTok's guide](https://developers.tiktok.com/doc/about-research-api/) about the research API to inform you about restrictions, daily quotas and FAQs.
 3. Feel free to contact me or submit a question in case you encounter bugs or errors!
    
-![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/julian-hohner-71a93b163/)
-[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/J_H_ohner)
 
 ## Installation
 
 Currently, ResearchTikPy is not available on PyPI, so it needs to be installed directly from the source:
 
 ```bash
 git clone https://github.com/HohnerJulian/ResearchTikPy.git
```

### Comparing `ResearchTikPy-0.1.1/setup.py` & `researchtikpy-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ResearchTikPy",
-    version="0.1.1",
+    version="0.1.2",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "requests", "pandas" 
     ],
     author="Julian Hohner",
     author_email="daswaeldchen@gmail.com",
```

