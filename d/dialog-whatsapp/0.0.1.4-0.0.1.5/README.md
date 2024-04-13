# Comparing `tmp/dialog_whatsapp-0.0.1.4.tar.gz` & `tmp/dialog_whatsapp-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_whatsapp-0.0.1.4.tar", max compression
+gzip compressed data, was "dialog_whatsapp-0.0.1.5.tar", max compression
```

## Comparing `dialog_whatsapp-0.0.1.4.tar` & `dialog_whatsapp-0.0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      442 2024-04-09 21:44:14.527027 dialog_whatsapp-0.0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-09 21:44:14.527225 dialog_whatsapp-0.0.1.4/dialog_whatsapp/__init__.py
--rw-r--r--   0        0        0     5288 2024-04-10 12:58:00.262410 dialog_whatsapp-0.0.1.4/dialog_whatsapp/plugin.py
--rw-r--r--   0        0        0     1931 2024-04-10 12:58:05.999480 dialog_whatsapp-0.0.1.4/dialog_whatsapp/responses.py
--rw-r--r--   0        0        0     1467 2024-04-10 13:01:25.860692 dialog_whatsapp-0.0.1.4/dialog_whatsapp/settings.py
--rw-r--r--   0        0        0      415 2024-04-10 12:58:59.585292 dialog_whatsapp-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      442 2024-04-09 21:44:14.527027 dialog_whatsapp-0.0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 21:44:14.527225 dialog_whatsapp-0.0.1.5/dialog_whatsapp/__init__.py
+-rw-r--r--   0        0        0     5292 2024-04-12 20:16:52.888594 dialog_whatsapp-0.0.1.5/dialog_whatsapp/plugin.py
+-rw-r--r--   0        0        0     1931 2024-04-10 12:58:05.999480 dialog_whatsapp-0.0.1.5/dialog_whatsapp/responses.py
+-rw-r--r--   0        0        0     1467 2024-04-10 13:01:25.860692 dialog_whatsapp-0.0.1.5/dialog_whatsapp/settings.py
+-rw-r--r--   0        0        0      439 2024-04-12 20:19:02.932568 dialog_whatsapp-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.5/PKG-INFO
```

### Comparing `dialog_whatsapp-0.0.1.4/dialog_whatsapp/plugin.py` & `dialog_whatsapp-0.0.1.5/dialog_whatsapp/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     create_session(identifier=session_id)
 
     llm = DialogLLM(
         config=PROJECT_CONFIG,
         session_id=session_id,
         dataset=DATASET,
-        llm_key=OPENAI_API_KEY
+        llm_api_key=OPENAI_API_KEY
     )
     logger.info(f"Project config: {PROJECT_CONFIG}")
     processed_message = llm.process(message)
     processed_message = processed_message["text"]
     logger.info("Processed message: %s", processed_message)
 
     # Generate the audio here
```

### Comparing `dialog_whatsapp-0.0.1.4/dialog_whatsapp/responses.py` & `dialog_whatsapp-0.0.1.5/dialog_whatsapp/responses.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.4/dialog_whatsapp/settings.py` & `dialog_whatsapp-0.0.1.5/dialog_whatsapp/settings.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.4/PKG-INFO` & `dialog_whatsapp-0.0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dialog-whatsapp
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: 
 Author: Vinicius Mesel
 Author-email: 4984147+vmesel@users.noreply.github.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dialog-lib (>=0.0.1.3,<0.0.2.0)
 Description-Content-Type: text/markdown
 
 # [talkd/dialog](https://github.com/talkdai/dialog) WhatsApp plugin
 
 [talkd/dialog](https://github.com/talkdai/dialog) plugin for integration with whatsapp, simplifying communication with the whatsapp api
 
 ### Sample variables to be used inside the .env file
```

