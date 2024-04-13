# Comparing `tmp/get_rankings-0.8.tar.gz` & `tmp/get_rankings-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_rankings-0.8.tar", last modified: Sun Sep 25 17:57:12 2022, max compression
+gzip compressed data, was "get_rankings-0.9.tar", last modified: Sat Apr 13 11:50:11 2024, max compression
```

## Comparing `get_rankings-0.8.tar` & `get_rankings-0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2022-09-25 17:57:12.569810 get_rankings-0.8/
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       92 2022-09-25 17:44:16.000000 get_rankings-0.8/AUTHORS
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)    35149 2022-09-25 17:42:54.000000 get_rankings-0.8/LICENSE
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1515 2022-09-25 17:57:12.569810 get_rankings-0.8/PKG-INFO
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      995 2022-09-25 17:55:44.000000 get_rankings-0.8/README.md
-drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2022-09-25 17:57:12.569810 get_rankings-0.8/get_rankings/
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)        1 2022-09-22 06:46:18.000000 get_rankings-0.8/get_rankings/__init__.py
--rwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)     8753 2022-09-25 17:45:30.000000 get_rankings-0.8/get_rankings/get_rankings.py
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      857 2022-09-25 16:31:35.000000 get_rankings-0.8/get_rankings/hash_cache.py
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1775 2022-09-25 16:59:09.000000 get_rankings-0.8/get_rankings/tools.py
-drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2022-09-25 17:57:12.569810 get_rankings-0.8/get_rankings.egg-info/
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1515 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/PKG-INFO
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      355 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/SOURCES.txt
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)        1 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/dependency_links.txt
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       64 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/entry_points.txt
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       75 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/requires.txt
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       13 2022-09-25 17:57:12.000000 get_rankings-0.8/get_rankings.egg-info/top_level.txt
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       38 2022-09-25 17:57:12.569810 get_rankings-0.8/setup.cfg
--rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      964 2022-09-25 17:42:31.000000 get_rankings-0.8/setup.py
+drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2024-04-13 11:50:11.440687 get_rankings-0.9/
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       92 2022-09-25 17:57:46.000000 get_rankings-0.9/AUTHORS
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)    35149 2022-09-25 17:57:46.000000 get_rankings-0.9/LICENSE
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1515 2024-04-13 11:50:11.440687 get_rankings-0.9/PKG-INFO
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      995 2022-09-25 17:57:46.000000 get_rankings-0.9/README.md
+drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2024-04-13 11:50:11.440687 get_rankings-0.9/get_rankings/
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)        1 2022-09-22 06:46:18.000000 get_rankings-0.9/get_rankings/__init__.py
+-rwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)     9246 2024-04-13 11:46:07.000000 get_rankings-0.9/get_rankings/get_rankings.py
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      857 2022-09-25 17:57:46.000000 get_rankings-0.9/get_rankings/hash_cache.py
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1775 2022-09-25 17:57:46.000000 get_rankings-0.9/get_rankings/tools.py
+drwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)        0 2024-04-13 11:50:11.440687 get_rankings-0.9/get_rankings.egg-info/
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)     1515 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/PKG-INFO
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      370 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/SOURCES.txt
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)        1 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/dependency_links.txt
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       64 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/entry_points.txt
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       75 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/requires.txt
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       13 2024-04-13 11:50:11.000000 get_rankings-0.9/get_rankings.egg-info/top_level.txt
+-rwxr-xr-x   0 gdacosta  (1000) gdacosta  (1000)       80 2022-09-22 06:28:50.000000 get_rankings-0.9/publish_pip.sh
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)       38 2024-04-13 11:50:11.440687 get_rankings-0.9/setup.cfg
+-rw-r--r--   0 gdacosta  (1000) gdacosta  (1000)      964 2024-04-13 11:47:30.000000 get_rankings-0.9/setup.py
```

### Comparing `get_rankings-0.8/LICENSE` & `get_rankings-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `get_rankings-0.8/PKG-INFO` & `get_rankings-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_rankings
-Version: 0.8
+Version: 0.9
 Summary: DBLP ranking using CORE Rank and SJR
 Home-page: https://gitlab.irit.fr/sepia-pub/da-costa/get-rankings
 Author: Georges Da Costa
 Author-email: georges.da-costa@irit.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `get_rankings-0.8/README.md` & `get_rankings-0.9/README.md`

 * *Files identical despite different names*

### Comparing `get_rankings-0.8/get_rankings/get_rankings.py` & `get_rankings-0.9/get_rankings/get_rankings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 import logging
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 import os
+import sys
 import datetime
 from dateutil.parser import parse as parsedate
 from bs4 import BeautifulSoup
 import pandas as pd
 import argparse
 import re
+import shutil
 
 from get_rankings.hash_cache import load_hash_caches, save_hash_caches, default_cache
 from get_rankings.tools import levenshtein, download, get_in_ordered_list
 
 
 def comp_lower(a, b):
     return isinstance(a, str) and isinstance(b, str) and a.lower() == b.lower()
@@ -44,14 +46,16 @@
             year = a.find("span", itemprop="datePublished").text
             venue, second_name, _ = a["id"].split("/")
             res.append([venue, name, second_name, year])
     return soup.title.text, res
 
 
 def get_core_year(year):
+    if year >= 2023:
+        return "CORE2023"
     if year >= 2021:
         return "CORE2021"
     if year >= 2020:
         return "CORE2020"
     if year >= 2018:
         return "CORE2018"
     if year >= 2017:
@@ -94,33 +98,38 @@
     def close(self):
         save_hash_caches(self.ranking_caches, "sjr")
 
     def get_issn(self, acronym):
         data = download("https://dblp.org/db/journals/%s/index.html" % acronym)
         soup = BeautifulSoup(data, "html.parser")
         full_name = soup.find("h1").text
-        issn = soup.find(
-            "a", attrs={"href": re.compile("^https://portal.issn.org/resource/ISSN/")}
-        ).text
+        try:
+            issn = soup.find(
+                "a", attrs={"href": re.compile("^https://portal.issn.org/resource/ISSN/")}
+            ).text
+        except:
+            issn = None
         return (full_name, issn)
 
     def get(self, name, second_name, year):
         if (name, second_name) in self.ranking_caches:
             rankings = self.ranking_caches[(name, second_name)]
         else:
             _ , issn = self.get_issn(second_name)
             rankings = self.get_sjr_rank(issn)
             self.ranking_caches[(name, second_name)] = rankings
-        rank = get_in_ordered_list(rankings, int(year))
+        rank = None if rankings is None else get_in_ordered_list(rankings, int(year))
         if rank is None:
             return ["J", name, second_name, int(year), None, None, None]
         else:
             return ["J", name, second_name, int(year), rank[1], None, rank[2]]
 
     def get_sjr_rank(self, name):
+        if name is None:
+            return None
         url = "https://www.scimagojr.com/journalsearch.php?q=%s" % name.replace(
             " ", "+"
         )
         data = download(url)
         sjr_soup = BeautifulSoup(data, "html.parser")
 
         revues = sjr_soup.find("div", class_="search_results")
@@ -168,15 +177,15 @@
 
     sjr = Sjr()
     core_ranking_caches = load_hash_caches("core")
 
     parser = argparse.ArgumentParser(
         description="Get ranking from DBLP and show a small summary"
     )
-    parser.add_argument("url", help="DBLP url")
+    parser.add_argument("url", help="DBLP url (or use clear-cache to clear the cache, is should be done regularly)")
     parser.add_argument("--start", type=int, default=-1, help="starting year")
     parser.add_argument("--end", type=int, default=10000, help="ending year")
     parser.add_argument(
         "-o", metavar=("output.csv"), default=None, help="output csv file"
     )
     parser.add_argument(
         "-d", action="store_true", help="display conference and journal list"
@@ -202,14 +211,21 @@
     url = args.url
     end_year = args.end
     csv_output = args.o
     start_year = args.start
     display_list = args.d
     logging.basicConfig(level=args.loglevel, format="%(levelname)s %(message)s")
 
+    if args.url == 'clear-cache':
+        cache_dir = default_cache()
+        print("Cleaning the cache :", cache_dir);
+        shutil.rmtree(cache_dir)
+        print("Cache clear");
+        sys.exit(0)
+    
     username, elements = get_dblp(url)
 
     # Keeps only elements in the requested range
     elements = [elem for elem in elements if start_year <= int(elem[-1]) <= end_year]
 
     print(username)
     result = []
```

### Comparing `get_rankings-0.8/get_rankings/hash_cache.py` & `get_rankings-0.9/get_rankings/hash_cache.py`

 * *Files identical despite different names*

### Comparing `get_rankings-0.8/get_rankings/tools.py` & `get_rankings-0.9/get_rankings/tools.py`

 * *Files identical despite different names*

### Comparing `get_rankings-0.8/get_rankings.egg-info/PKG-INFO` & `get_rankings-0.9/get_rankings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-rankings
-Version: 0.8
+Version: 0.9
 Summary: DBLP ranking using CORE Rank and SJR
 Home-page: https://gitlab.irit.fr/sepia-pub/da-costa/get-rankings
 Author: Georges Da Costa
 Author-email: georges.da-costa@irit.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `get_rankings-0.8/setup.py` & `get_rankings-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get_rankings",
-    version="0.8",
+    version="0.9",
     author="Georges Da Costa",
     author_email="georges.da-costa@irit.fr",
     description="DBLP ranking using CORE Rank and SJR",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.irit.fr/sepia-pub/da-costa/get-rankings",
     packages=setuptools.find_packages(),
```

