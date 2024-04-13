# Comparing `tmp/arjun-2.2.5.tar.gz` & `tmp/arjun-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arjun-2.2.5.tar", last modified: Mon Apr  1 03:53:50 2024, max compression
+gzip compressed data, was "arjun-2.2.6.tar", last modified: Sat Apr 13 04:57:17 2024, max compression
```

## Comparing `arjun-2.2.5.tar` & `arjun-2.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/
--rw-r--r--   0 d3v       (1000) d3v       (1000)    34523 2024-03-30 05:46:47.000000 arjun-2.2.5/LICENSE
--rw-r--r--   0 d3v       (1000) d3v       (1000)     4049 2024-04-01 03:53:50.707270 arjun-2.2.5/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)     3203 2024-03-30 05:46:47.000000 arjun-2.2.5/README.md
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/arjun/
--rw-r--r--   0 d3v       (1000) d3v       (1000)       22 2024-04-01 03:10:03.000000 arjun-2.2.5/arjun/__init__.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)    10563 2024-04-01 03:31:44.000000 arjun-2.2.5/arjun/__main__.py
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/arjun/core/
--rw-r--r--   0 d3v       (1000) d3v       (1000)        0 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/__init__.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     5143 2024-03-30 06:17:51.000000 arjun-2.2.5/arjun/core/anomaly.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      776 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/bruter.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      691 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/colors.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)       84 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/config.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1993 2024-03-30 06:17:48.000000 arjun-2.2.5/arjun/core/error_handler.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     2259 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/exporter.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     3370 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/importer.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      598 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/core/prompt.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     2734 2024-04-01 03:19:01.000000 arjun-2.2.5/arjun/core/requester.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     8471 2024-04-01 03:48:40.000000 arjun-2.2.5/arjun/core/utils.py
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/arjun/db/
--rw-r--r--   0 d3v       (1000) d3v       (1000)   153175 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/db/large.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)    96595 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/db/medium.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)     6505 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/db/small.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)     3051 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/db/special.json
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/arjun/plugins/
--rw-r--r--   0 d3v       (1000) d3v       (1000)        0 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/plugins/__init__.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      513 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/plugins/commoncrawl.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     2020 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/plugins/heuristic.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      479 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/plugins/otx.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)      801 2024-03-30 05:46:47.000000 arjun-2.2.5/arjun/plugins/wayback.py
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-01 03:53:50.707270 arjun-2.2.5/arjun.egg-info/
--rw-r--r--   0 d3v       (1000) d3v       (1000)     4049 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)      721 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/SOURCES.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/dependency_links.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       46 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/entry_points.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/not-zip-safe
--rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/requires.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        6 2024-04-01 03:53:50.000000 arjun-2.2.5/arjun.egg-info/top_level.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2024-04-01 03:53:50.707270 arjun-2.2.5/setup.cfg
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1473 2024-03-30 05:46:47.000000 arjun-2.2.5/setup.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.353124 arjun-2.2.6/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)    34523 2024-04-13 04:55:45.000000 arjun-2.2.6/LICENSE
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     4049 2024-04-13 04:57:17.353124 arjun-2.2.6/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     3203 2024-04-13 04:55:45.000000 arjun-2.2.6/README.md
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.349791 arjun-2.2.6/arjun/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       22 2024-04-13 04:56:46.000000 arjun-2.2.6/arjun/__init__.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)    10563 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/__main__.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.353124 arjun-2.2.6/arjun/core/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/__init__.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     5143 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/anomaly.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      776 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/bruter.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      691 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/colors.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       84 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/config.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1993 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/error_handler.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     2259 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/exporter.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     3370 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/importer.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      598 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/prompt.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     2734 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/requester.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     8471 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/core/utils.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.353124 arjun-2.2.6/arjun/db/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)   153175 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/db/large.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)    96595 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/db/medium.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     6505 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/db/small.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     3051 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/db/special.json
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.353124 arjun-2.2.6/arjun/plugins/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/plugins/__init__.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      513 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/plugins/commoncrawl.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     2020 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/plugins/heuristic.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      479 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/plugins/otx.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      801 2024-04-13 04:55:45.000000 arjun-2.2.6/arjun/plugins/wayback.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2024-04-13 04:57:17.353124 arjun-2.2.6/arjun.egg-info/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     4049 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      721 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/SOURCES.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/dependency_links.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       46 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/entry_points.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/not-zip-safe
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/requires.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        6 2024-04-13 04:57:17.000000 arjun-2.2.6/arjun.egg-info/top_level.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2024-04-13 04:57:17.353124 arjun-2.2.6/setup.cfg
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1473 2024-04-13 04:55:45.000000 arjun-2.2.6/setup.py
```

### Comparing `arjun-2.2.5/LICENSE` & `arjun-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/PKG-INFO` & `arjun-2.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arjun
-Version: 2.2.5
+Version: 2.2.6
 Summary: HTTP parameter discovery suite
 Home-page: https://github.com/s0md3v/Arjun
-Download-URL: https://github.com/s0md3v/Arjun/archive/v2.2.5.zip
+Download-URL: https://github.com/s0md3v/Arjun/archive/v2.2.6.zip
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: arjun,bug bounty,http,pentesting,security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: arjun Version: 2.2.5 Summary: HTTP parameter
+Metadata-Version: 2.1 Name: arjun Version: 2.2.6 Summary: HTTP parameter
 discovery suite Home-page: https://github.com/s0md3v/Arjun Download-URL: https:
-//github.com/s0md3v/Arjun/archive/v2.2.5.zip Author: Somdev Sangwan Author-
+//github.com/s0md3v/Arjun/archive/v2.2.6.zip Author: Somdev Sangwan Author-
 email: s0md3v@gmail.com License: GNU General Public License v3 (GPLv3)
 Keywords: arjun,bug bounty,http,pentesting,security Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Operating
 System :: OS Independent Classifier: Topic :: Security Classifier: License ::
 OSI Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3.4 Description-Content-Type: text/markdown License-File:
```

### Comparing `arjun-2.2.5/README.md` & `arjun-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/__main__.py` & `arjun-2.2.6/arjun/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,19 +131,19 @@
 
         # params from response must be extracted before factors but displayed later
         found, words_exist = heuristic(response_1, wordlist)
 
         factors = define(response_1, response_2, fuzz, fuzz[::-1], wordlist)
         zzuf = "z" + random_str(6)
         response_3 = requester(request, {zzuf[:-1]: zzuf[::-1][:-1]})
-        while factors:
+        while True:
             reason = compare(response_3, factors, {zzuf[:-1]: zzuf[::-1][:-1]})[2]
             if not reason:
                 break
-            factors[reason] = []
+            factors[reason] = False
         if single_url:
             print('%s Analysing HTTP response for potential parameter names' % run)
         if found:
             num = len(found)
             if words_exist:
                  print('%s Heuristic scanner found %i parameters' % (good, num))
             else:
```

### Comparing `arjun-2.2.5/arjun/core/anomaly.py` & `arjun-2.2.6/arjun/core/anomaly.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/bruter.py` & `arjun-2.2.6/arjun/core/bruter.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/colors.py` & `arjun-2.2.6/arjun/core/colors.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/error_handler.py` & `arjun-2.2.6/arjun/core/error_handler.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/exporter.py` & `arjun-2.2.6/arjun/core/exporter.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/importer.py` & `arjun-2.2.6/arjun/core/importer.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/prompt.py` & `arjun-2.2.6/arjun/core/prompt.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/requester.py` & `arjun-2.2.6/arjun/core/requester.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/core/utils.py` & `arjun-2.2.6/arjun/core/utils.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/db/large.txt` & `arjun-2.2.6/arjun/db/large.txt`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/db/medium.txt` & `arjun-2.2.6/arjun/db/medium.txt`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/db/small.txt` & `arjun-2.2.6/arjun/db/small.txt`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/db/special.json` & `arjun-2.2.6/arjun/db/special.json`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/plugins/commoncrawl.py` & `arjun-2.2.6/arjun/plugins/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/plugins/heuristic.py` & `arjun-2.2.6/arjun/plugins/heuristic.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun/plugins/wayback.py` & `arjun-2.2.6/arjun/plugins/wayback.py`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/arjun.egg-info/PKG-INFO` & `arjun-2.2.6/arjun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arjun
-Version: 2.2.5
+Version: 2.2.6
 Summary: HTTP parameter discovery suite
 Home-page: https://github.com/s0md3v/Arjun
-Download-URL: https://github.com/s0md3v/Arjun/archive/v2.2.5.zip
+Download-URL: https://github.com/s0md3v/Arjun/archive/v2.2.6.zip
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: arjun,bug bounty,http,pentesting,security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: arjun Version: 2.2.5 Summary: HTTP parameter
+Metadata-Version: 2.1 Name: arjun Version: 2.2.6 Summary: HTTP parameter
 discovery suite Home-page: https://github.com/s0md3v/Arjun Download-URL: https:
-//github.com/s0md3v/Arjun/archive/v2.2.5.zip Author: Somdev Sangwan Author-
+//github.com/s0md3v/Arjun/archive/v2.2.6.zip Author: Somdev Sangwan Author-
 email: s0md3v@gmail.com License: GNU General Public License v3 (GPLv3)
 Keywords: arjun,bug bounty,http,pentesting,security Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Operating
 System :: OS Independent Classifier: Topic :: Security Classifier: License ::
 OSI Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3.4 Description-Content-Type: text/markdown License-File:
```

### Comparing `arjun-2.2.5/arjun.egg-info/SOURCES.txt` & `arjun-2.2.6/arjun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arjun-2.2.5/setup.py` & `arjun-2.2.6/setup.py`

 * *Files identical despite different names*

