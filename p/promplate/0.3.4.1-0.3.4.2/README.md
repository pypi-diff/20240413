# Comparing `tmp/promplate-0.3.4.1.tar.gz` & `tmp/promplate-0.3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.4.1.tar", max compression
+gzip compressed data, was "promplate-0.3.4.2.tar", max compression
```

## Comparing `promplate-0.3.4.1.tar` & `promplate-0.3.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.1/promplate/__init__.py
--rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.1/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2309 2024-04-05 09:30:17.923274 promplate-0.3.4.1/promplate/chain/callback.py
--rw-r--r--   0        0        0    17320 2024-04-06 09:47:54.814935 promplate-0.3.4.1/promplate/chain/node.py
--rw-r--r--   0        0        0     1308 2024-02-06 11:24:26.943042 promplate-0.3.4.1/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.1/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1043 2024-02-06 11:24:26.944273 promplate-0.3.4.1/promplate/llm/base.py
--rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.1/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4125 2024-02-06 11:24:26.945287 promplate-0.3.4.1/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     6002 2024-02-28 11:45:48.661575 promplate-0.3.4.1/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.1/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1633 2024-04-06 09:41:46.823783 promplate-0.3.4.1/promplate/prompt/builder.py
--rw-r--r--   0        0        0     3216 2024-02-06 11:24:26.947313 promplate-0.3.4.1/promplate/prompt/chat.py
--rw-r--r--   0        0        0     7309 2024-04-10 09:05:12.114869 promplate-0.3.4.1/promplate/prompt/template.py
--rw-r--r--   0        0        0     3386 2024-04-06 08:33:51.420912 promplate-0.3.4.1/promplate/prompt/utils.py
--rw-r--r--   0        0        0     1600 2024-04-10 09:07:39.122808 promplate-0.3.4.1/pyproject.toml
--rw-r--r--   0        0        0     1995 2024-04-06 10:35:03.295230 promplate-0.3.4.1/README.md
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.2/promplate/__init__.py
+-rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.2/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2309 2024-04-05 09:30:17.923274 promplate-0.3.4.2/promplate/chain/callback.py
+-rw-r--r--   0        0        0    17376 2024-04-13 09:47:44.901981 promplate-0.3.4.2/promplate/chain/node.py
+-rw-r--r--   0        0        0     1308 2024-02-06 11:24:26.943042 promplate-0.3.4.2/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.2/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1043 2024-02-06 11:24:26.944273 promplate-0.3.4.2/promplate/llm/base.py
+-rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.2/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4125 2024-02-06 11:24:26.945287 promplate-0.3.4.2/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     6002 2024-02-28 11:45:48.661575 promplate-0.3.4.2/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.2/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-06 09:41:46.823783 promplate-0.3.4.2/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     3216 2024-02-06 11:24:26.947313 promplate-0.3.4.2/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7309 2024-04-10 09:05:12.114869 promplate-0.3.4.2/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3386 2024-04-06 08:33:51.420912 promplate-0.3.4.2/promplate/prompt/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-13 09:44:20.298486 promplate-0.3.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1995 2024-04-06 10:35:03.295230 promplate-0.3.4.2/README.md
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.2/PKG-INFO
```

### Comparing `promplate-0.3.4.1/promplate/chain/callback.py` & `promplate-0.3.4.2/promplate/chain/callback.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/chain/node.py` & `promplate-0.3.4.2/promplate/chain/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     def result(self, result):
         self.__setitem__("__result__", result)
 
     @result.deleter
     def result(self):
         self.__delitem__("__result__")
 
+    def __str__(self):
+        return str({**self})
+
 
 Process = Callable[[ChainContext], Context | None]
 
 AsyncProcess = Callable[[ChainContext], Awaitable[Context | None]]
 
 
 class AbstractNode(Protocol):
```

### Comparing `promplate-0.3.4.1/promplate/chain/utils.py` & `promplate-0.3.4.2/promplate/chain/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/llm/base.py` & `promplate-0.3.4.2/promplate/llm/base.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/llm/openai/v0.py` & `promplate-0.3.4.2/promplate/llm/openai/v0.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/llm/openai/v1.py` & `promplate-0.3.4.2/promplate/llm/openai/v1.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/prompt/builder.py` & `promplate-0.3.4.2/promplate/prompt/builder.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/prompt/chat.py` & `promplate-0.3.4.2/promplate/prompt/chat.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/prompt/template.py` & `promplate-0.3.4.2/promplate/prompt/template.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/promplate/prompt/utils.py` & `promplate-0.3.4.2/promplate/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/pyproject.toml` & `promplate-0.3.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promplate"
-version = "0.3.4.1"
+version = "0.3.4.2"
 description = "Prompt engineering framework for humans"
 homepage = "https://promplate.dev/"
 documentation = "https://docs.py.promplate.dev/"
 repository = "https://github.com/promplate/core"
 authors = ["Muspi Merol <me@promplate.dev>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `promplate-0.3.4.1/README.md` & `promplate-0.3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.1/PKG-INFO` & `promplate-0.3.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.4.1
+Version: 0.3.4.2
 Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
 Author-email: me@promplate.dev
 Requires-Python: >=3.10,<4.0
```

