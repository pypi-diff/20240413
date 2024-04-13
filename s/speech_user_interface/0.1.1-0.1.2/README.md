# Comparing `tmp/speech_user_interface-0.1.1.tar.gz` & `tmp/speech_user_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_user_interface-0.1.1.tar", max compression
+gzip compressed data, was "speech_user_interface-0.1.2.tar", max compression
```

## Comparing `speech_user_interface-0.1.1.tar` & `speech_user_interface-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      674 2024-04-13 07:52:53.383223 speech_user_interface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      510 2024-04-13 07:52:05.052795 speech_user_interface-0.1.1/README.md
--rw-r--r--   0        0        0     1424 2024-04-13 07:42:21.715869 speech_user_interface-0.1.1/speech_user_interface/__init__.py
--rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.1/speech_user_interface/compare_strings.py
--rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.1/speech_user_interface/CONSTANTS.py
--rw-r--r--   0        0        0  1013772 2024-03-24 08:49:43.043726 speech_user_interface-0.1.1/speech_user_interface/data/nasdaq_screener_1711270178562.csv
--rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.1/speech_user_interface/load_vosk_model.py
--rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.1/speech_user_interface/read_in_speech.py
--rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.1/speech_user_interface/send_text_to_chatgpt.py
--rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.1/speech_user_interface/speak_text.py
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 speech_user_interface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2024-04-13 07:59:19.471447 speech_user_interface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      510 2024-04-13 07:52:05.052795 speech_user_interface-0.1.2/README.md
+-rw-r--r--   0        0        0     1744 2024-04-13 07:59:12.579294 speech_user_interface-0.1.2/speech_user_interface/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.2/speech_user_interface/compare_strings.py
+-rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.2/speech_user_interface/CONSTANTS.py
+-rw-r--r--   0        0        0  1013772 2024-03-24 08:49:43.043726 speech_user_interface-0.1.2/speech_user_interface/data/nasdaq_screener_1711270178562.csv
+-rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.2/speech_user_interface/load_vosk_model.py
+-rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.2/speech_user_interface/read_in_speech.py
+-rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.2/speech_user_interface/send_text_to_chatgpt.py
+-rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.2/speech_user_interface/speak_text.py
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 speech_user_interface-0.1.2/PKG-INFO
```

### Comparing `speech_user_interface-0.1.1/pyproject.toml` & `speech_user_interface-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speech_user_interface"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["David Piper <dbpiper@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 sui = "speech_user_interface:main"
```

### Comparing `speech_user_interface-0.1.1/speech_user_interface/data/nasdaq_screener_1711270178562.csv` & `speech_user_interface-0.1.2/speech_user_interface/data/nasdaq_screener_1711270178562.csv`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.1/speech_user_interface/load_vosk_model.py` & `speech_user_interface-0.1.2/speech_user_interface/load_vosk_model.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.1/speech_user_interface/read_in_speech.py` & `speech_user_interface-0.1.2/speech_user_interface/read_in_speech.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.1/PKG-INFO` & `speech_user_interface-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech_user_interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: David Piper
 Author-email: dbpiper@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

