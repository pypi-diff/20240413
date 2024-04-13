# Comparing `tmp/lemmymodbot-test-0.6.0a3.tar.gz` & `tmp/lemmymodbot-test-0.6.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemmymodbot-test-0.6.0a3.tar", last modified: Fri Mar 22 06:48:43 2024, max compression
+gzip compressed data, was "lemmymodbot-test-0.6.0a6.tar", last modified: Fri Mar 22 06:46:19 2024, max compression
```

## Comparing `lemmymodbot-test-0.6.0a3.tar` & `lemmymodbot-test-0.6.0a6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.195136 lemmymodbot-test-0.6.0a3/lemmymodbot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.195136 lemmymodbot-test-0.6.0a3/lemmymodbot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/api/matrix_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/api/photodna_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.195136 lemmymodbot-test-0.6.0a3/lemmymodbot/data/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/data/monitor_persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.195136 lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/extract_links_from_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/spam_image_bootstrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-22 06:48:43.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-22 06:48:43.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 06:48:43.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-22 06:48:43.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/lemmymodbot/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/ml/bag_of_words.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/ml/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/account_age_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/blacklist_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/mime_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/phash_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/photodna_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/spam_image_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/title_conformity_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/toxicity_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/lemmymodbot/processors/user_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:48:43.199136 lemmymodbot-test-0.6.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 06:43:47.000000 lemmymodbot-test-0.6.0a3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.545419 lemmymodbot-test-0.6.0a6/lemmymodbot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.549419 lemmymodbot-test-0.6.0a6/lemmymodbot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/api/matrix_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/api/photodna_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.549419 lemmymodbot-test-0.6.0a6/lemmymodbot/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/data/monitor_persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.549419 lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/extract_links_from_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/spam_image_bootstrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-22 06:46:19.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-22 06:46:19.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 06:46:19.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-22 06:46:19.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.549419 lemmymodbot-test-0.6.0a6/lemmymodbot/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/ml/bag_of_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/ml/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/account_age_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/blacklist_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/mime_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/phash_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/photodna_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/spam_image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/title_conformity_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/toxicity_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/lemmymodbot/processors/user_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:46:19.553419 lemmymodbot-test-0.6.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 06:44:51.000000 lemmymodbot-test-0.6.0a6/tests/test.py
```

### Comparing `lemmymodbot-test-0.6.0a3/README.md` & `lemmymodbot-test-0.6.0a6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 <p align="center">
     <a href="#" rel="noopener">
         <img width=150px src="assets/bot-logo.svg" ></img>
     </a>
     <h1 align="center">
         Lemmy Mod Bot
     </h1>
-    <p align="center">
-        A web API designed to efficiently manage and schedule volunteer firefighters.
-    </p>
 </p>
 <div align="center">
 
 [![Build](https://github.com/BenMMcLean/LemmyModBot/actions/workflows/build.yml/badge.svg)](https://github.com/BenMMcLean/LemmyModBot/actions/workflows/build.yml) 
 [![Unit Test](https://github.com/BenMMcLean/LemmyModBot/actions/workflows/test.yml/badge.svg)](https://github.com/BenMMcLean/LemmyModBot/actions/workflows/test.yml)
 
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
                              _[_a_s_s_e_t_s_/_b_o_t_-_l_o_g_o_._s_v_g_]
                           ************ LLeemmmmyy MMoodd BBoott ************
- A web API designed to efficiently manage and schedule volunteer firefighters.
     [![Build](https://github.com/BenMMcLean/LemmyModBot/actions/workflows/
    build.yml/badge.svg)](https://github.com/BenMMcLean/LemmyModBot/actions/
  workflows/build.yml) [![Unit Test](https://github.com/BenMMcLean/LemmyModBot/
      actions/workflows/test.yml/badge.svg)](https://github.com/BenMMcLean/
                     LemmyModBot/actions/workflows/test.yml)
 A Lemmy bot written in Python that allows you to automatically moderate
 communities from toxicity, duplicate posts, and CSAM content. This bot is a
```

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/api/matrix_client.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/api/matrix_client.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/api/photodna_client.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/api/photodna_client.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/data/base.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/data/base.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/data/monitor_persistence.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/data/monitor_persistence.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/extract_links_from_markdown.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/extract_links_from_markdown.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/helpers/spam_image_bootstrapper.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/helpers/spam_image_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/lemmymodbot_test.egg-info/SOURCES.txt` & `lemmymodbot-test-0.6.0a6/lemmymodbot/lemmymodbot_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/ml/bag_of_words.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/ml/bag_of_words.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/ml/classifier.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/ml/classifier.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/__init__.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/account_age_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/account_age_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/base.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/base.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/blacklist_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/blacklist_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/mime_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/mime_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/phash_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/phash_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/photodna_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/photodna_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/spam_image_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/spam_image_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/title_conformity_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/title_conformity_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/toxicity_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/toxicity_processor.py`

 * *Files identical despite different names*

### Comparing `lemmymodbot-test-0.6.0a3/lemmymodbot/processors/user_processor.py` & `lemmymodbot-test-0.6.0a6/lemmymodbot/processors/user_processor.py`

 * *Files identical despite different names*

