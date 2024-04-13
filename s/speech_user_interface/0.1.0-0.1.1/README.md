# Comparing `tmp/speech_user_interface-0.1.0.tar.gz` & `tmp/speech_user_interface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_user_interface-0.1.0.tar", max compression
+gzip compressed data, was "speech_user_interface-0.1.1.tar", max compression
```

## Comparing `speech_user_interface-0.1.0.tar` & `speech_user_interface-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      674 2024-04-13 05:05:12.290656 speech_user_interface-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      213 2024-04-12 18:33:44.439267 speech_user_interface-0.1.0/README.md
--rw-r--r--   0        0        0     1424 2024-04-13 07:42:21.715869 speech_user_interface-0.1.0/speech_user_interface/__init__.py
--rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.0/speech_user_interface/compare_strings.py
--rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.0/speech_user_interface/CONSTANTS.py
--rw-r--r--   0        0        0  1013772 2024-03-24 08:49:43.043726 speech_user_interface-0.1.0/speech_user_interface/data/nasdaq_screener_1711270178562.csv
--rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.0/speech_user_interface/load_vosk_model.py
--rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.0/speech_user_interface/read_in_speech.py
--rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.0/speech_user_interface/send_text_to_chatgpt.py
--rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.0/speech_user_interface/speak_text.py
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 speech_user_interface-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2024-04-13 07:52:53.383223 speech_user_interface-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      510 2024-04-13 07:52:05.052795 speech_user_interface-0.1.1/README.md
+-rw-r--r--   0        0        0     1424 2024-04-13 07:42:21.715869 speech_user_interface-0.1.1/speech_user_interface/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.1/speech_user_interface/compare_strings.py
+-rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.1/speech_user_interface/CONSTANTS.py
+-rw-r--r--   0        0        0  1013772 2024-03-24 08:49:43.043726 speech_user_interface-0.1.1/speech_user_interface/data/nasdaq_screener_1711270178562.csv
+-rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.1/speech_user_interface/load_vosk_model.py
+-rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.1/speech_user_interface/read_in_speech.py
+-rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.1/speech_user_interface/send_text_to_chatgpt.py
+-rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.1/speech_user_interface/speak_text.py
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 speech_user_interface-0.1.1/PKG-INFO
```

### Comparing `speech_user_interface-0.1.0/pyproject.toml` & `speech_user_interface-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speech_user_interface"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["David Piper <dbpiper@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 sui = "speech_user_interface:main"
```

### Comparing `speech_user_interface-0.1.0/speech_user_interface/__init__.py` & `speech_user_interface-0.1.1/speech_user_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.0/speech_user_interface/data/nasdaq_screener_1711270178562.csv` & `speech_user_interface-0.1.1/speech_user_interface/data/nasdaq_screener_1711270178562.csv`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.0/speech_user_interface/load_vosk_model.py` & `speech_user_interface-0.1.1/speech_user_interface/load_vosk_model.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.0/speech_user_interface/read_in_speech.py` & `speech_user_interface-0.1.1/speech_user_interface/read_in_speech.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.0/PKG-INFO` & `speech_user_interface-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech_user_interface
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: David Piper
 Author-email: dbpiper@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -20,14 +20,26 @@
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-levenshtein (>=0.25.1,<0.26.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: vosk (>=0.3.45,<0.4.0)
 Description-Content-Type: text/markdown
 
-# souce_code_to_pdf
+# speech_user_interface
 
-To run source_code_to_pdf from source you must have Poetry installed.
+You need to define a function to run like this:
 
-Then you can install it by running `poetry lock && poetry install`
-To run it you then run `poetry run souce_code_to_pdf`
+```
+def default_function_to_run(input_text: str):
+    reponse_text = send_text_to_chatgpt(input_text)
+    speak_text(reponse_text)
+
+
+main(function_to_run=default_function_to_run):
+
+```
+
+This one is configured by default but it can be anything. We run in a cycle
+until "exit the program" is said and that exits the infinite loop. We just keep
+reading input and passing that to the `function_to_run` this can do anything
+with this input.
```

