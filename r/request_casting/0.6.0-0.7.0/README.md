# Comparing `tmp/request_casting-0.6.0.tar.gz` & `tmp/request_casting-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_casting-0.6.0.tar", max compression
+gzip compressed data, was "request_casting-0.7.0.tar", max compression
```

## Comparing `request_casting-0.6.0.tar` & `request_casting-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-11-16 04:37:37.767416 request_casting-0.6.0/LICENSE
--rw-r--r--   0        0        0     6448 2023-12-05 04:37:24.872798 request_casting-0.6.0/README.md
--rw-r--r--   0        0        0     1067 2023-12-14 19:40:12.808533 request_casting-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      147 2023-12-14 19:39:56.243533 request_casting-0.6.0/request_casting/__init__.py
--rw-r--r--   0        0        0      424 2023-12-14 19:40:51.679534 request_casting-0.6.0/request_casting/locale/en/LC_MESSAGES/request_casting.mo
--rw-r--r--   0        0        0      738 2023-11-16 04:37:37.769416 request_casting-0.6.0/request_casting/locale/en.po
--rw-r--r--   0        0        0      524 2023-12-14 19:40:51.677534 request_casting-0.6.0/request_casting/locale/es/LC_MESSAGES/request_casting.mo
--rw-r--r--   0        0        0     1335 2023-12-14 19:40:51.675534 request_casting-0.6.0/request_casting/locale/es.po
--rw-r--r--   0        0        0      772 2023-12-14 19:40:51.671534 request_casting-0.6.0/request_casting/locale/request_casting.pot
--rw-r--r--   0        0        0     1456 2023-12-14 18:57:46.423268 request_casting-0.6.0/request_casting/poethepoet.py
--rw-r--r--   0        0        0     9272 2023-12-14 19:38:56.288531 request_casting-0.6.0/request_casting/request_casting.py
--rw-r--r--   0        0        0     7063 1970-01-01 00:00:00.000000 request_casting-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 05:09:34.943254 request_casting-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6959 2024-04-13 09:04:13.327080 request_casting-0.7.0/README.md
+-rw-r--r--   0        0        0     1068 2024-04-13 09:07:17.951096 request_casting-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      145 2024-04-13 09:00:46.326904 request_casting-0.7.0/request_casting/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-13 09:04:37.035082 request_casting-0.7.0/request_casting/locale/en/LC_MESSAGES/request_casting.mo
+-rw-r--r--   0        0        0      738 2024-04-13 05:09:34.945254 request_casting-0.7.0/request_casting/locale/en.po
+-rw-r--r--   0        0        0      524 2024-04-13 09:04:37.032082 request_casting-0.7.0/request_casting/locale/es/LC_MESSAGES/request_casting.mo
+-rw-r--r--   0        0        0     1335 2024-04-13 05:09:34.945254 request_casting-0.7.0/request_casting/locale/es.po
+-rw-r--r--   0        0        0      772 2024-04-13 09:04:37.025082 request_casting-0.7.0/request_casting/locale/request_casting.pot
+-rw-r--r--   0        0        0     1456 2024-04-13 05:09:34.945254 request_casting-0.7.0/request_casting/poethepoet.py
+-rw-r--r--   0        0        0     9617 2024-04-13 08:53:17.862866 request_casting-0.7.0/request_casting/request_casting.py
+-rw-r--r--   0        0        0     7474 1970-01-01 00:00:00.000000 request_casting-0.7.0/PKG-INFO
```

### Comparing `request_casting-0.6.0/LICENSE` & `request_casting-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `request_casting-0.6.0/README.md` & `request_casting-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,27 @@
 ```
 You'll get this answers
 ``` 
 curl http://localhost:8000/myview/?a=2011-10-05T14:48:00.000Z   => a will be a datetime with timezone
 curl http://localhost:8000/myview/?a=2021-1-1   => a will be None
 ```
 
+### RequestEmail
+Use this method inside a view to get a validated email
+
+```python
+    # ... The same as RequestBool example
+    a=request_casting.RequestEmail(request, "a")
+```
+You'll get this answers
+``` 
+curl http://localhost:8000/myview/?a=hi@hi.com   => a will be an email
+curl http://localhost:8000/myview/?a=hi.hi.com   => a will be None
+```
+
 ### RequestInteger
 
 Use this method inside a view to get a casted Integer
 
 ```python
     # ... The same as RequestBool example
     a=request_casting.RequestInteger(request, "a")
@@ -221,14 +234,21 @@
 
 ## Test module
 
 Run `poe coverage` to test module.
 
 ## Changelog
 
+### 0.7.0 (2024-04-13)
+- Using pydicts-0.16.0
+- Added RequestEmail method
+
+### 0.6.0 (2023-12-14)
+- Using pydicts-0.11.0 library to capture errors and fix bugs
+
 ### 0.5.0 (2023-12-05)
 - Added support to request_casting with json formats (APICLIENT)
 
 ### 0.4.0 (2023-12-05)
 - Migrated to pydicts-0.9.0
 
 ### 0.3.0 (2023-12-04)
```

### Comparing `request_casting-0.6.0/pyproject.toml` & `request_casting-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "request_casting"
-version = "0.6.0"
+version = "0.7.0"
 description = "Provide method to cast django request data for POST and GET methods"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3.0 license"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">3.8,<4.0"
-pydicts = ">=0.11.0"
+python = ">3.10,<4.0"
+pydicts = ">=0.16.0"
 
 [tool.poetry.group.dev.dependencies]
-poetry = ">=1.5.1"
-poethepoet = ">=0.22.0"
-django = ">=4.2.7"
-djangorestframework = ">=3.14.0"
-coverage = ">=7.3.2"
+poetry = ">=1.8.2"
+poethepoet = ">=0.25.0"
+django = ">=5.0.4"
+djangorestframework = ">=3.15.1"
+coverage = ">=7.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 release = { script = "request_casting.poethepoet:release" }
```

### Comparing `request_casting-0.6.0/request_casting/locale/en.po` & `request_casting-0.7.0/request_casting/locale/en.po`

 * *Files identical despite different names*

### Comparing `request_casting-0.6.0/request_casting/locale/es/LC_MESSAGES/request_casting.mo` & `request_casting-0.7.0/request_casting/locale/es/LC_MESSAGES/request_casting.mo`

 * *Files identical despite different names*

### Comparing `request_casting-0.6.0/request_casting/locale/es.po` & `request_casting-0.7.0/request_casting/locale/es.po`

 * *Files identical despite different names*

### Comparing `request_casting-0.6.0/request_casting/locale/request_casting.pot` & `request_casting-0.7.0/request_casting/locale/request_casting.pot`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-12-14 20:40+0100\n"
+"POT-Creation-Date: 2024-04-13 11:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `request_casting-0.6.0/request_casting/poethepoet.py` & `request_casting-0.7.0/request_casting/poethepoet.py`

 * *Files identical despite different names*

### Comparing `request_casting-0.6.0/request_casting/request_casting.py` & `request_casting-0.7.0/request_casting/request_casting.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,14 +200,28 @@
         dictionary=request.data
         
     if not field in dictionary:
         return default
         
     
     return casts.str2dtaware(dictionary.get(field), "JsUtcIso",  timezone_string, ignore_exception=True, ignore_exception_value=default)
+    
+def RequestEmail(request, field, default=None):
+    if request.method=="GET":
+        dictionary=request.GET
+    else:
+        dictionary=request.data
+        
+    if not field in dictionary:
+        return default
+        
+    if casts.is_email(dictionary.get(field)):
+        return dictionary.get(field)
+    else:
+        return default
 
 def RequestString(request, field, default=None):
     if request.method=="GET":
         dictionary=request.GET
     else:
         dictionary=request.data
```

### Comparing `request_casting-0.6.0/PKG-INFO` & `request_casting-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: request_casting
-Version: 0.6.0
+Version: 0.7.0
 Summary: Provide method to cast django request data for POST and GET methods
 License: GPL-3.0 license
 Author: turulomio
 Author-email: turulomio@yahoo.es
-Requires-Python: >3.8,<4.0
+Requires-Python: >3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydicts (>=0.11.0)
+Requires-Dist: pydicts (>=0.16.0)
 Description-Content-Type: text/markdown
 
 # request_casting
 Python module that allows to cast django request data for POST and GET methods easyly
 
 Allows you to capture errors in parameters and give them default values, to protect your application with little code and easy to read.
 
@@ -105,14 +103,27 @@
 ```
 You'll get this answers
 ``` 
 curl http://localhost:8000/myview/?a=2011-10-05T14:48:00.000Z   => a will be a datetime with timezone
 curl http://localhost:8000/myview/?a=2021-1-1   => a will be None
 ```
 
+### RequestEmail
+Use this method inside a view to get a validated email
+
+```python
+    # ... The same as RequestBool example
+    a=request_casting.RequestEmail(request, "a")
+```
+You'll get this answers
+``` 
+curl http://localhost:8000/myview/?a=hi@hi.com   => a will be an email
+curl http://localhost:8000/myview/?a=hi.hi.com   => a will be None
+```
+
 ### RequestInteger
 
 Use this method inside a view to get a casted Integer
 
 ```python
     # ... The same as RequestBool example
     a=request_casting.RequestInteger(request, "a")
@@ -238,14 +249,21 @@
 
 ## Test module
 
 Run `poe coverage` to test module.
 
 ## Changelog
 
+### 0.7.0 (2024-04-13)
+- Using pydicts-0.16.0
+- Added RequestEmail method
+
+### 0.6.0 (2023-12-14)
+- Using pydicts-0.11.0 library to capture errors and fix bugs
+
 ### 0.5.0 (2023-12-05)
 - Added support to request_casting with json formats (APICLIENT)
 
 ### 0.4.0 (2023-12-05)
 - Migrated to pydicts-0.9.0
 
 ### 0.3.0 (2023-12-04)
```

