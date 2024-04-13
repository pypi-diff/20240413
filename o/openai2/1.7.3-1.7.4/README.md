# Comparing `tmp/openai2-1.7.3.tar.gz` & `tmp/openai2-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai2-1.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai2-1.7.3.tar` & `openai2-1.7.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7.3/LICENSE
--rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 openai2-1.7.3/README.md
--rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 openai2-1.7.3/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 openai2-1.7.3/_core/chat.py
--rw-r--r--   0        0        0     2285 2024-04-07 02:46:07.785077 openai2-1.7.3/_core/chat_in_cmd.py
--rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 openai2-1.7.3/_core/group_chat.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 openai2-1.7.3/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7.3/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7.3/licenses/openai/LICENSE
--rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 openai2-1.7.3/openai2.py
--rw-r--r--   0        0        0      805 2024-04-07 04:00:23.156252 openai2-1.7.3/pyproject.toml
--rw-r--r--   0        0        0    14158 1970-01-01 00:00:00.000000 openai2-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7.4/LICENSE
+-rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 openai2-1.7.4/README.md
+-rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 openai2-1.7.4/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 openai2-1.7.4/_core/chat.py
+-rw-r--r--   0        0        0     2286 2024-04-08 06:59:43.786636 openai2-1.7.4/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 openai2-1.7.4/_core/group_chat.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 openai2-1.7.4/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7.4/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7.4/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 openai2-1.7.4/openai2.py
+-rw-r--r--   0        0        0      804 2024-04-13 08:15:29.737274 openai2-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0    14157 1970-01-01 00:00:00.000000 openai2-1.7.4/PKG-INFO
```

### Comparing `openai2-1.7.3/LICENSE` & `openai2-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7.3/README.md` & `openai2-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `openai2-1.7.3/_core/chat.py` & `openai2-1.7.4/_core/chat.py`

 * *Files identical despite different names*

### Comparing `openai2-1.7.3/_core/chat_in_cmd.py` & `openai2-1.7.4/_core/chat_in_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 from .chat import Chat, AKPool
 from arts.cooltypes import moduledb
-from arts import openai2
 
 
-mdb = moduledb.DB(openai2, depth=3)['chat_in_cmd']
+mdb = moduledb.DB('https://pypi.org/project/openai2', depth=3)['chat_in_cmd']
 apikeys: moduledb.File = mdb['apikeys']['data_1']
 apikeys.setdefault('list', [])
 record: moduledb.File = mdb['records']['chat_1']
 record.setdefault('messages', [])
 
 
 def chat_in_cmd(apikeys:list, newchat=False, model='gpt-4-1106-preview', msg_max_count=30):
```

### Comparing `openai2-1.7.3/_core/group_chat.py` & `openai2-1.7.4/_core/group_chat.py`

 * *Files identical despite different names*

### Comparing `openai2-1.7.3/licenses/openai/LICENSE` & `openai2-1.7.4/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7.3/pyproject.toml` & `openai2-1.7.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.7.3"
+version = "1.7.4"
 description = "ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。"
-dependencies = ["arts>=2024.4.3.3"]
+dependencies = ["arts>=2024.4.13"]
 keywords = ["openai", "chatgpt", "openai2"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.7.3/PKG-INFO` & `openai2-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.7.3
+Version: 1.7.4
 Summary: ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 Keywords: openai,chatgpt,openai2
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: arts>=2024.4.3.3
+Requires-Dist: arts>=2024.4.13
 Project-URL: HomePage, https://github.com/lcctoor/arts/tree/main/arts/openai2
 
 # 项目描述
 
 ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 
 # 作者
```

