# Comparing `tmp/langchain_zhipu-4.0.9.tar.gz` & `tmp/langchain_zhipu-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_zhipu-4.0.9.tar", max compression
+gzip compressed data, was "langchain_zhipu-4.1.0.tar", max compression
```

## Comparing `langchain_zhipu-4.0.9.tar` & `langchain_zhipu-4.1.0.tar`

### file list

```diff
@@ -1,42 +1,52 @@
--rw-r--r--   0        0        0     2096 2024-02-26 11:52:24.870421 langchain_zhipu-4.0.9/README.md
--rw-r--r--   0        0        0      379 2024-02-22 12:09:53.357907 langchain_zhipu-4.0.9/langchain_zhipu/__init__.py
--rw-r--r--   0        0        0       23 2024-02-26 13:40:32.447868 langchain_zhipu-4.0.9/langchain_zhipu/__version__.py
--rw-r--r--   0        0        0     2377 2024-02-22 08:33:38.324554 langchain_zhipu-4.0.9/langchain_zhipu/_client.py
--rw-r--r--   0        0        0    13547 2024-02-22 12:19:29.728982 langchain_zhipu-4.0.9/langchain_zhipu/_langchain.py
--rw-r--r--   0        0        0      147 2024-02-19 23:37:05.213086 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 23:37:05.213266 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3118 2024-02-19 23:37:05.213455 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      451 2024-02-19 23:37:05.213573 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/chat.py
--rw-r--r--   0        0        0     2790 2024-02-19 23:37:05.213698 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1633 2024-02-19 23:37:05.213813 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/embeddings.py
--rw-r--r--   0        0        0     2323 2024-02-19 23:37:05.213919 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/files.py
--rw-r--r--   0        0        0        0 2024-02-19 23:37:05.214014 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      311 2024-02-19 23:37:05.214128 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0     3470 2024-02-19 23:37:05.214386 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1818 2024-02-19 23:37:05.214688 langchain_zhipu-4.0.9/langchain_zhipu/api_resource/images.py
--rw-r--r--   0        0        0        0 2024-02-19 23:37:05.214904 langchain_zhipu-4.0.9/langchain_zhipu/core/__init__.py
--rw-r--r--   0        0        0      406 2024-02-19 23:37:05.215106 langchain_zhipu-4.0.9/langchain_zhipu/core/_base_api.py
--rw-r--r--   0        0        0     3392 2024-02-26 12:55:46.556760 langchain_zhipu-4.0.9/langchain_zhipu/core/_base_type.py
--rw-r--r--   0        0        0     2038 2024-02-19 23:37:05.215406 langchain_zhipu-4.0.9/langchain_zhipu/core/_errors.py
--rw-r--r--   0        0        0     1384 2024-02-19 23:37:05.215550 langchain_zhipu-4.0.9/langchain_zhipu/core/_files.py
--rw-r--r--   0        0        0    12233 2024-02-26 13:39:28.734676 langchain_zhipu-4.0.9/langchain_zhipu/core/_http_client.py
--rw-r--r--   0        0        0      713 2024-02-19 23:37:05.215895 langchain_zhipu-4.0.9/langchain_zhipu/core/_jwt_token.py
--rw-r--r--   0        0        0     1694 2024-02-26 13:10:19.131744 langchain_zhipu-4.0.9/langchain_zhipu/core/_request_opt.py
--rw-r--r--   0        0        0     3394 2024-02-26 12:55:22.507049 langchain_zhipu-4.0.9/langchain_zhipu/core/_response.py
--rw-r--r--   0        0        0     4085 2024-02-19 23:37:05.216591 langchain_zhipu-4.0.9/langchain_zhipu/core/_sse_client.py
--rw-r--r--   0        0        0      443 2024-02-19 23:37:05.216921 langchain_zhipu-4.0.9/langchain_zhipu/core/_utils.py
--rw-r--r--   0        0        0        0 2024-02-19 23:37:05.217118 langchain_zhipu-4.0.9/langchain_zhipu/types/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 23:37:05.217315 langchain_zhipu-4.0.9/langchain_zhipu/types/chat/__init__.py
--rw-r--r--   0        0        0      568 2024-02-22 12:17:26.273679 langchain_zhipu-4.0.9/langchain_zhipu/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      879 2024-02-22 12:17:35.294111 langchain_zhipu-4.0.9/langchain_zhipu/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1226 2024-02-22 12:39:57.588214 langchain_zhipu-4.0.9/langchain_zhipu/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-02-19 23:37:05.218155 langchain_zhipu-4.0.9/langchain_zhipu/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      446 2024-02-22 12:17:04.731595 langchain_zhipu-4.0.9/langchain_zhipu/types/embeddings.py
--rw-r--r--   0        0        0      550 2024-02-22 12:17:12.204895 langchain_zhipu-4.0.9/langchain_zhipu/types/file_object.py
--rw-r--r--   0        0        0      244 2024-02-19 23:37:05.218970 langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1051 2024-02-22 12:17:48.809661 langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1121 2024-02-22 12:17:42.726835 langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-02-19 23:37:05.219789 langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      394 2024-02-22 12:17:19.893034 langchain_zhipu-4.0.9/langchain_zhipu/types/image.py
--rw-r--r--   0        0        0      728 2024-02-26 13:40:28.226778 langchain_zhipu-4.0.9/pyproject.toml
--rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 langchain_zhipu-4.0.9/PKG-INFO
+-rw-r--r--   0        0        0     3069 2024-03-27 14:16:13.949508 langchain_zhipu-4.1.0/README.md
+-rw-r--r--   0        0        0      597 2024-04-09 02:43:26.661836 langchain_zhipu-4.1.0/langchain_zhipu/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-12 15:32:12.526696 langchain_zhipu-4.1.0/langchain_zhipu/__version__.py
+-rw-r--r--   0        0        0     2579 2024-03-28 15:59:03.809176 langchain_zhipu-4.1.0/langchain_zhipu/_client.py
+-rw-r--r--   0        0        0      147 2024-04-12 15:34:05.266385 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:05.266769 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/__init__.py
+-rw-r--r--   0        0        0     3118 2024-04-12 15:34:05.267060 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/async_completions.py
+-rw-r--r--   0        0        0      451 2024-04-12 15:34:05.267290 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/chat.py
+-rw-r--r--   0        0        0     2790 2024-04-12 15:34:05.267521 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/completions.py
+-rw-r--r--   0        0        0     1633 2024-04-12 15:34:05.267759 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/embeddings.py
+-rw-r--r--   0        0        0     2323 2024-04-12 15:34:05.267978 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/files.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:05.268207 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-12 15:34:05.268459 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0     3470 2024-04-12 15:34:05.269395 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/fine_tuning/jobs.py
+-rw-r--r--   0        0        0     1818 2024-04-12 15:34:05.269837 langchain_zhipu-4.1.0/langchain_zhipu/api_resource/images.py
+-rw-r--r--   0        0        0    15864 2024-04-07 11:17:39.809084 langchain_zhipu-4.1.0/langchain_zhipu/chat.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:05.270126 langchain_zhipu-4.1.0/langchain_zhipu/core/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-12 15:34:05.270458 langchain_zhipu-4.1.0/langchain_zhipu/core/_base_api.py
+-rw-r--r--   0        0        0     3392 2024-04-12 15:34:05.272267 langchain_zhipu-4.1.0/langchain_zhipu/core/_base_type.py
+-rw-r--r--   0        0        0     2038 2024-04-12 15:34:05.272714 langchain_zhipu-4.1.0/langchain_zhipu/core/_errors.py
+-rw-r--r--   0        0        0     1384 2024-04-12 15:34:05.275395 langchain_zhipu-4.1.0/langchain_zhipu/core/_files.py
+-rw-r--r--   0        0        0    12233 2024-04-12 15:34:05.278500 langchain_zhipu-4.1.0/langchain_zhipu/core/_http_client.py
+-rw-r--r--   0        0        0      713 2024-04-12 15:34:05.278835 langchain_zhipu-4.1.0/langchain_zhipu/core/_jwt_token.py
+-rw-r--r--   0        0        0     1694 2024-04-12 15:34:05.280017 langchain_zhipu-4.1.0/langchain_zhipu/core/_request_opt.py
+-rw-r--r--   0        0        0     3394 2024-04-12 15:34:05.281411 langchain_zhipu-4.1.0/langchain_zhipu/core/_response.py
+-rw-r--r--   0        0        0     4085 2024-04-12 15:34:05.282603 langchain_zhipu-4.1.0/langchain_zhipu/core/_sse_client.py
+-rw-r--r--   0        0        0      443 2024-04-12 15:34:05.283079 langchain_zhipu-4.1.0/langchain_zhipu/core/_utils.py
+-rw-r--r--   0        0        0     1499 2024-04-12 15:33:28.452985 langchain_zhipu-4.1.0/langchain_zhipu/embeddings.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.0/langchain_zhipu/http/__init__.py
+-rw-r--r--   0        0        0     6408 2024-04-09 11:14:03.743373 langchain_zhipu-4.1.0/langchain_zhipu/http/api.py
+-rw-r--r--   0        0        0    13988 2024-04-12 15:30:45.341675 langchain_zhipu-4.1.0/langchain_zhipu/http/base.py
+-rw-r--r--   0        0        0     7711 2024-04-10 11:31:06.455774 langchain_zhipu-4.1.0/langchain_zhipu/http/chat.py
+-rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.0/langchain_zhipu/http/enum.py
+-rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.0/langchain_zhipu/http/env.py
+-rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.0/langchain_zhipu/http/manager.py
+-rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.0/langchain_zhipu/http/types.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:05.283423 langchain_zhipu-4.1.0/langchain_zhipu/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:05.283788 langchain_zhipu-4.1.0/langchain_zhipu/types/chat/__init__.py
+-rw-r--r--   0        0        0      568 2024-04-12 15:34:05.285073 langchain_zhipu-4.1.0/langchain_zhipu/types/chat/async_chat_completion.py
+-rw-r--r--   0        0        0      879 2024-04-12 15:34:05.286840 langchain_zhipu-4.1.0/langchain_zhipu/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1226 2024-04-12 15:34:05.288657 langchain_zhipu-4.1.0/langchain_zhipu/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      171 2024-04-12 15:34:05.288987 langchain_zhipu-4.1.0/langchain_zhipu/types/chat/chat_completions_create_param.py
+-rw-r--r--   0        0        0      446 2024-04-12 15:34:05.290012 langchain_zhipu-4.1.0/langchain_zhipu/types/embeddings.py
+-rw-r--r--   0        0        0      550 2024-04-12 15:34:05.291312 langchain_zhipu-4.1.0/langchain_zhipu/types/file_object.py
+-rw-r--r--   0        0        0      244 2024-04-12 15:34:05.291828 langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     1051 2024-04-12 15:34:05.292643 langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0     1121 2024-04-12 15:34:05.293310 langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      339 2024-04-12 15:34:05.293603 langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      394 2024-04-12 15:34:05.294518 langchain_zhipu-4.1.0/langchain_zhipu/types/image.py
+-rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.0/langchain_zhipu/utils.py
+-rw-r--r--   0        0        0      750 2024-04-12 15:32:18.972368 langchain_zhipu-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.0/PKG-INFO
```

### Comparing `langchain_zhipu-4.0.9/README.md` & `langchain_zhipu-4.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,49 +2,82 @@
 [![PyPI version](https://img.shields.io/pypi/v/langchain_zhipu.svg)](https://pypi.org/project/langchain_zhipu/)
 
 为了方便在 langchain 中使用，在官方SDK基础上做了如下额外工作：
 
 - 问题1: 智谱AI的官方SDK使用了 pydantic v2，这与 langchain（尤其是langserve）不兼容
 - 问题2: langchain.community 的国内包更新不及时，无法在 langchain 的 LCEL 语法中使用
 
-## 已支持全部 langchain 接口
+# 已支持全部 langchain 接口
 
 1. invoke
 2. ainvoke
 3. batch
 4. abatch
 5. stream
 6. astream
 7. astream_events
 8. asteram_log
 
-## 已支持模型能力
+# 已支持模型能力
 
-- 模型名称："glm-3-turbo", "glm-4", "glm-4v"
+- 已支持生成模型："glm-3-turbo", "glm-4", "glm-4v"
+- 已支持向量模型："embedding-2"
 - 逻辑推理和对话生成
 - 支持工具回调
+- 支持智能体
+- 支持RAG
+
+# 使用
 
 ## 简单的例子
 
 ```python
-from zhipuai_pydantic_v1 import ChatZhipuAI
+from langchain_zhipu import ChatZhipuAI
 llm = ChatZhipuAI()
 
 # invoke
 llm.invoke("hi")
 
 # stream
 for s in llm.stream("hi"):
   print(s)
 
 # astream
 async for s in llm.astream("hi"):
   print(s)
 ```
 
+## retrieval 工具
+
+```python
+from langchain_zhipu import convert_to_retrieval_tool
+llm.bind(tools=[convert_to_retrieval_tool(knowledge_id="1772979648448397312")]).invoke("你知道马冬梅住哪里吗？")
+```
+
+## web_search 工具
+
+```python
+from langchain_zhipu import convert_to_web_search_tool
+llm.bind(tools=[convert_to_web_search_tool(search_query="周星驰电影")]).invoke("哪部电影好看？")
+```
+
+## function 工具
+
+```python
+from langchain_core.utils.function_calling import convert_to_openai_tool
+from langchain.tools import tool
+
+@tool
+def search(query: str) -> str:
+    """查询 langchan 资料; args: query 类型为字符串，描述用户的问题."""
+    return "langchain_chinese 是一个为中国大模型优化的langchain模块"
+
+llm.bind(tools=[convert_to_openai_tool(search)]).invoke("langchain_chinese是啥？请查询本地资料回答。")
+```
+
 ## 使用glm-4v
 
 ```python
 from langchain_zhipu import ChatZhipuAI
 from langchain_core.prompts import ChatPromptTemplate
 
 llm4v = ChatZhipuAI(model="glm-4v")
@@ -63,19 +96,20 @@
           }
         ]),
 ])
 
 (prompt|llm4v).invoke({})
 ```
 
-------------------------------------------
+## 智能体
 
-**接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)大模型接口 Python SDK（Big Model API SDK in Python），让开发者更便捷的调用智谱开放API
+请查看 [agent.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/agent.ipynb)
 
-**官方SDK** [![PyPI version](https://img.shields.io/pypi/v/zhipuai.svg)](https://pypi.org/project/zhipuai/)
+# 更多用法
 
-**官方SDK能力简介**
-- 对所有接口进行了类型封装。
-- 初始化client并调用成员函数，无需关注http调用过程的各种细节，所见即所得。
-- 默认缓存token。
+请参考 [langchain_chinese](https://github.com/arcstep/langchain_chinese)
 
+------------------------------------------
 
+**官方接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)大模型接口 Python SDK（Big Model API SDK in Python），让开发者更便捷的调用智谱开放API
+
+**官方SDK** [![PyPI version](https://img.shields.io/pypi/v/zhipuai.svg)](https://pypi.org/project/zhipuai/)
```

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/_client.py` & `langchain_zhipu-4.1.0/langchain_zhipu/_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from . import api_resource
 import os
 import httpx
 from httpx import Timeout
 
 
 class ZhipuAI(HttpClient):
-    chat: api_resource.chat
+    chat: api_resource.chat.Chat
+    embeddings: api_resource.embeddings.Embeddings
+    knowledge_embeddings: api_resource.knowledge.base.Embeddings
     api_key: str
 
     def __init__(
             self,
             *,
             api_key: str | None = None,
             base_url: str | httpx.URL | None = None,
@@ -45,14 +47,15 @@
             timeout=timeout,
             custom_httpx_client=http_client,
             custom_headers=custom_headers,
         )
         self.chat = api_resource.chat.Chat(self)
         self.images = api_resource.images.Images(self)
         self.embeddings = api_resource.embeddings.Embeddings(self)
+        self.knowledge_embeddings = api_resource.knowledge.base.Embeddings(self)
         self.files = api_resource.files.Files(self)
         self.fine_tuning = api_resource.fine_tuning.FineTuning(self)
 
     @property
     @override
     def _auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
```

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/_langchain.py` & `langchain_zhipu-4.1.0/langchain_zhipu/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
+
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
     generate_from_stream,
 )
 
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 
 # common types
-from typing import Type, Any, Mapping, Dict, Iterator, List, Optional, cast
+from typing import (
+    Type, Any, Mapping, Dict, Iterator, List, Optional, cast,
+    AsyncIterator, Union, Literal, AbstractSet, Collection
+)
 
 # async
 import asyncio
-from typing import AsyncIterator
+
+import tiktoken
 
 # all message types
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     BaseMessageChunk,
     HumanMessage,
     HumanMessageChunk,
     ToolMessage,
     ToolMessageChunk,
+    FunctionMessage,
+    FunctionMessageChunk,
     SystemMessage,
     SystemMessageChunk,
     ChatMessage,
     ChatMessageChunk,
 )
 
 from ._client import ZhipuAI
@@ -41,35 +48,46 @@
     Args:
         _dict: The dictionary.
 
     Returns:
         The LangChain message.
     """
     role = _dict.get("role")
+    id_ = _dict.get("id")
     if role == "user":
-        return HumanMessage(content=_dict.get("content", ""))
+        return HumanMessage(content=_dict.get("content", ""), id=id_)
     elif role == "assistant":
         # Fix for azure
         # Also OpenAI returns None for tool invocations
         content = _dict.get("content", "") or ""
         additional_kwargs: Dict = {}
+        if function_call := _dict.get("function_call"):
+            additional_kwargs["function_call"] = dict(function_call)
         if tool_calls := _dict.get("tool_calls"):
             additional_kwargs["tool_calls"] = tool_calls
-        return AIMessage(content=content, additional_kwargs=additional_kwargs)
+        return AIMessage(content=content, additional_kwargs=additional_kwargs, id=id_)
     elif role == "system":
-        return SystemMessage(content=_dict.get("content", ""))
+        return SystemMessage(content=_dict.get("content", ""), id=id_)
+    elif role == "function":
+        return FunctionMessage(
+            content=_dict.get("content", ""), name=_dict.get("name"), id=id_
+        )
     elif role == "tool":
         additional_kwargs = {}
+        if "name" in _dict:
+            additional_kwargs["name"] = _dict["name"]
         return ToolMessage(
             content=_dict.get("content", ""),
             tool_call_id=_dict.get("tool_call_id"),
             additional_kwargs=additional_kwargs,
+            id=id_,
         )
     else:
-        return ChatMessage(content=_dict.get("content", ""), role=role)
+        return ChatMessage(content=_dict.get("content", ""), role=role, id=id_)
+
 
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
 
@@ -79,54 +97,79 @@
     message_dict: Dict[str, Any]
     if isinstance(message, ChatMessage):
         message_dict = {"role": message.role, "content": message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {"role": "user", "content": message.content}
     elif isinstance(message, AIMessage):
         message_dict = {"role": "assistant", "content": message.content}
+        if "function_call" in message.additional_kwargs:
+            message_dict["function_call"] = message.additional_kwargs["function_call"]
+            # If function call only, content is None not empty string
+            if message_dict["content"] == "":
+                message_dict["content"] = None
         if "tool_calls" in message.additional_kwargs:
             message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
             # If tool calls only, content is None not empty string
             if message_dict["content"] == "":
                 message_dict["content"] = None
     elif isinstance(message, SystemMessage):
         message_dict = {"role": "system", "content": message.content}
+    elif isinstance(message, FunctionMessage):
+        message_dict = {
+            "role": "function",
+            "content": message.content,
+            "name": message.name,
+        }
     elif isinstance(message, ToolMessage):
         message_dict = {
             "role": "tool",
             "content": message.content,
             "tool_call_id": message.tool_call_id,
         }
     else:
         raise TypeError(f"Got unknown type {message}")
     if "name" in message.additional_kwargs:
         message_dict["name"] = message.additional_kwargs["name"]
     return message_dict
 
+
 def _convert_delta_to_message_chunk(
     _dict: Mapping[str, Any], default_class: Type[BaseMessageChunk]
 ) -> BaseMessageChunk:
+    id_ = _dict.get("id")
     role = cast(str, _dict.get("role"))
     content = cast(str, _dict.get("content") or "")
     additional_kwargs: Dict = {}
+    if _dict.get("function_call"):
+        function_call = dict(_dict["function_call"])
+        if "name" in function_call and function_call["name"] is None:
+            function_call["name"] = ""
+        additional_kwargs["function_call"] = function_call
     if _dict.get("tool_calls"):
         additional_kwargs["tool_calls"] = _dict["tool_calls"]
 
     if role == "user" or default_class == HumanMessageChunk:
-        return HumanMessageChunk(content=content)
+        return HumanMessageChunk(content=content, id=id_)
     elif role == "assistant" or default_class == AIMessageChunk:
-        return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
+        return AIMessageChunk(
+            content=content, additional_kwargs=additional_kwargs, id=id_
+        )
     elif role == "system" or default_class == SystemMessageChunk:
-        return SystemMessageChunk(content=content)
+        return SystemMessageChunk(content=content, id=id_)
+    elif role == "function" or default_class == FunctionMessageChunk:
+        return FunctionMessageChunk(content=content, name=_dict["name"], id=id_)
     elif role == "tool" or default_class == ToolMessageChunk:
-        return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
+        return ToolMessageChunk(
+            content=content, tool_call_id=_dict["tool_call_id"], id=id_
+        )
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)
+        return ChatMessageChunk(content=content, role=role, id=id_)
     else:
-        return default_class(content=content)  # type: ignore
+        return default_class(content=content, id=id_)  # type: ignore
+
 
 class ChatZhipuAI(BaseChatModel):
     """支持最新的智谱API"""
 
     @property
     def lc_secrets(self) -> Dict[str, str]:
         return {"zhipuai_api_key": "ZHIPUAI_API_KEY"}
@@ -157,15 +200,15 @@
         return ["langchain", "chat_models", "ZhipuAI"]
     
     client: Any = None
     """访问智谱AI的客户端"""
     
     api_key: str = None
 
-    model: str = Field(default="glm-3-turbo")
+    model: str = Field(default="glm-4")
     """所要调用的模型编码"""
 
     request_id: Optional[str] = None
     """
     由用户端传参，需保证唯一性；用于区分每次请求的唯一标识，用户端不传时平台会默认生成。
     """
     
@@ -208,53 +251,57 @@
     可供模型调用的工具列表,tools字段会计算 tokens ，同样受到tokens长度的限制。
     """
 
     tool_choice: Optional[str] = "auto"
     """
     用于控制模型是如何选择要调用的函数，仅当工具类型为function时补充。默认为auto，当前仅支持auto。
     """
+    
+    streaming: Optional[bool] = False
+    """
+    流式输出。
+    """
+
+    allowed_special: Union[Literal["all"], AbstractSet[str]] = set()
+    """Set of special tokens that are allowed。"""
 
+    disallowed_special: Union[Literal["all"], Collection[str]] = "all"
+    """Set of special tokens that are not allowed。"""
+    
     @classmethod
-    def valid_params(cls):
+    def filter_model_kwargs(cls):
         """
-        ZhipuAI只接受这些参数。另外，stream参数根据使用invoke方法还是stream方法来设定，而不是在对象构建时提供。
+        ZhipuAI在调用时只接受这些参数。
         """
         return [
             "model",
             "request_id",
             "do_sample",
-            "api_key",
             "temperature",
             "top_p",
             "max_tokens",
             "stop",
             "tools",
             "tool_choice",
         ]
         
     # 获得模型调用参数
     def get_model_kwargs(self):
         params = {}
         for attr, value in self.__dict__.items():
-            if attr in self.__class__.valid_params() and value is not None:
+            if attr in self.__class__.filter_model_kwargs() and value is not None:
                 params[attr] = value
         return params
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
-        try:
-            if values["api_key"] is not None:
-                values["client"] =  ZhipuAI(api_key=values["api_key"])
-            else:
-                values["client"] =  ZhipuAI()
-        except ImportError:
-            raise RuntimeError(
-                "Could not import zhipuai package. "
-                "Please install it via 'pip install -U zhipuai'"
-            )
+        if values["api_key"] is not None:
+            values["client"] =  ZhipuAI(api_key=values["api_key"])
+        else:
+            values["client"] =  ZhipuAI()
         return values
 
     # 实现 invoke 调用方法
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
@@ -268,14 +315,23 @@
         # 构造参数序列
         params = self.get_model_kwargs()
         params.update(kwargs)
         params.update({"stream": False})
         if stop is not None:
             params.update({"stop": stop})
     
+        # 支持根据 stream 或 streaming 生成流
+        should_stream = stream if stream is not None else self.streaming
+        if should_stream:
+            stream_iter = self._stream(
+                messages, stop=stop, run_manager=run_manager, **kwargs
+            )
+            return generate_from_stream(stream_iter)
+    
+        # 调用模型
         response = self.client.chat.completions.create(
             messages=prompt,
             **params
         )
 
         generations = []
         if not isinstance(response, dict):
@@ -312,26 +368,26 @@
         # 构造参数序列
         params = self.get_model_kwargs()
         params.update(kwargs)
         params.update({"stream": True})
         if stop is not None:
             params.update({"stop": stop})
     
-        response = self.client.chat.completions.create(
+        responses = self.client.chat.completions.create(
             messages=prompt,
             **params
         )
 
         default_chunk_class = AIMessageChunk
-        for chunk in response:
-            if not isinstance(chunk, dict):
-                chunk = chunk.dict()
-            if len(chunk["choices"]) == 0:
+        for response in responses:                
+            if not isinstance(response, dict):
+                response = response.dict()
+            if len(response["choices"]) == 0:
                 continue
-            choice = chunk["choices"][0]
+            choice = response["choices"][0]
             chunk = _convert_delta_to_message_chunk(
                 choice["delta"], default_chunk_class
             )
             generation_info = {}
             if finish_reason := choice.get("finish_reason"):
                 generation_info["finish_reason"] = finish_reason
             default_chunk_class = chunk.__class__
@@ -356,39 +412,48 @@
         # 构造参数序列
         params = self.get_model_kwargs()
         params.update(kwargs)
         params.update({"stream": True})
         if stop is not None:
             params.update({"stop": stop})
 
-
         # 创建一个新的函数来调用 self.client.chat.completions.create
         def create_completions():
             return self.client.chat.completions.create(
                 messages=prompt,
                 **params
             )
 
         # 由于ZhipuAI没有基于流的异步返回，因此使用asyncio构建
         loop = asyncio.get_running_loop()
-        response = await loop.run_in_executor(None, create_completions)
+        responses = await loop.run_in_executor(None, create_completions)
 
         default_chunk_class = AIMessageChunk
-        for chunk in response:
-            if not isinstance(chunk, dict):
-                chunk = chunk.dict()
-            if len(chunk["choices"]) == 0:
+        for response in responses:
+            if not isinstance(response, dict):
+                response = response.dict()
+            if len(response["choices"]) == 0:
                 continue
-            choice = chunk["choices"][0]
+            choice = response["choices"][0]
             chunk = _convert_delta_to_message_chunk(
                 choice["delta"], default_chunk_class
             )
             generation_info = {}
             if finish_reason := choice.get("finish_reason"):
                 generation_info["finish_reason"] = finish_reason
             default_chunk_class = chunk.__class__
             chunk = ChatGenerationChunk(
                 message=chunk, generation_info=generation_info or None
             )
             if run_manager:
                 await run_manager.on_llm_new_token(chunk.text, chunk=chunk)
-            yield chunk
+            yield chunk
+
+    def get_token_ids(self, text: str) -> List[int]:
+        """Get the token IDs using the tiktoken package."""
+
+        encoding_model = tiktoken.get_encoding("cl100k_base")
+        return encoding_model.encode(
+            text,
+            allowed_special=self.allowed_special,
+            disallowed_special=self.disallowed_special,
+        )
```

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/async_completions.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/async_completions.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/chat/completions.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/chat/completions.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/embeddings.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/files.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/files.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/fine_tuning/jobs.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/fine_tuning/jobs.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/api_resource/images.py` & `langchain_zhipu-4.1.0/langchain_zhipu/api_resource/images.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_base_type.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_base_type.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_errors.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_errors.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_files.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_files.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_http_client.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_http_client.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_jwt_token.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_jwt_token.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_request_opt.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_request_opt.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_response.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_response.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/core/_sse_client.py` & `langchain_zhipu-4.1.0/langchain_zhipu/core/_sse_client.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/chat/async_chat_completion.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/chat/async_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/chat/chat_completion.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/chat/chat_completion_chunk.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/file_object.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/file_object.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/fine_tuning_job.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/langchain_zhipu/types/fine_tuning/fine_tuning_job_event.py` & `langchain_zhipu-4.1.0/langchain_zhipu/types/fine_tuning/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.0.9/pyproject.toml` & `langchain_zhipu-4.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain_zhipu"
-version = "4.0.9"
+version = "4.1.0"
 description = "将智谱AI集成到LangChain"
 license = "MIT"
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/langchain_zhipuai"
 repository = "https://github.com/arcstep/langchain_zhipuai.git"
 readme = "README.md"
 
@@ -20,11 +20,12 @@
 pytest = "^8.0.1"
 ipykernel = "^6.29.2"
 python-dotenv = "^1.0.1"
 langchain-experimental = "^0.0.52"
 pandas = "^2.2.0"
 tabulate = "^0.9.0"
 langchain-openai = "^0.0.6"
+dashscope = "^1.14.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langchain_zhipu-4.0.9/PKG-INFO` & `langchain_zhipu-4.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_zhipu
-Version: 4.0.9
+Version: 4.1.0
 Summary: 将智谱AI集成到LangChain
 Home-page: https://github.com/arcstep/langchain_zhipuai
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,49 +25,82 @@
 [![PyPI version](https://img.shields.io/pypi/v/langchain_zhipu.svg)](https://pypi.org/project/langchain_zhipu/)
 
 为了方便在 langchain 中使用，在官方SDK基础上做了如下额外工作：
 
 - 问题1: 智谱AI的官方SDK使用了 pydantic v2，这与 langchain（尤其是langserve）不兼容
 - 问题2: langchain.community 的国内包更新不及时，无法在 langchain 的 LCEL 语法中使用
 
-## 已支持全部 langchain 接口
+# 已支持全部 langchain 接口
 
 1. invoke
 2. ainvoke
 3. batch
 4. abatch
 5. stream
 6. astream
 7. astream_events
 8. asteram_log
 
-## 已支持模型能力
+# 已支持模型能力
 
-- 模型名称："glm-3-turbo", "glm-4", "glm-4v"
+- 已支持生成模型："glm-3-turbo", "glm-4", "glm-4v"
+- 已支持向量模型："embedding-2"
 - 逻辑推理和对话生成
 - 支持工具回调
+- 支持智能体
+- 支持RAG
+
+# 使用
 
 ## 简单的例子
 
 ```python
-from zhipuai_pydantic_v1 import ChatZhipuAI
+from langchain_zhipu import ChatZhipuAI
 llm = ChatZhipuAI()
 
 # invoke
 llm.invoke("hi")
 
 # stream
 for s in llm.stream("hi"):
   print(s)
 
 # astream
 async for s in llm.astream("hi"):
   print(s)
 ```
 
+## retrieval 工具
+
+```python
+from langchain_zhipu import convert_to_retrieval_tool
+llm.bind(tools=[convert_to_retrieval_tool(knowledge_id="1772979648448397312")]).invoke("你知道马冬梅住哪里吗？")
+```
+
+## web_search 工具
+
+```python
+from langchain_zhipu import convert_to_web_search_tool
+llm.bind(tools=[convert_to_web_search_tool(search_query="周星驰电影")]).invoke("哪部电影好看？")
+```
+
+## function 工具
+
+```python
+from langchain_core.utils.function_calling import convert_to_openai_tool
+from langchain.tools import tool
+
+@tool
+def search(query: str) -> str:
+    """查询 langchan 资料; args: query 类型为字符串，描述用户的问题."""
+    return "langchain_chinese 是一个为中国大模型优化的langchain模块"
+
+llm.bind(tools=[convert_to_openai_tool(search)]).invoke("langchain_chinese是啥？请查询本地资料回答。")
+```
+
 ## 使用glm-4v
 
 ```python
 from langchain_zhipu import ChatZhipuAI
 from langchain_core.prompts import ChatPromptTemplate
 
 llm4v = ChatZhipuAI(model="glm-4v")
@@ -86,20 +119,21 @@
           }
         ]),
 ])
 
 (prompt|llm4v).invoke({})
 ```
 
-------------------------------------------
+## 智能体
 
-**接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)大模型接口 Python SDK（Big Model API SDK in Python），让开发者更便捷的调用智谱开放API
+请查看 [agent.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/agent.ipynb)
 
-**官方SDK** [![PyPI version](https://img.shields.io/pypi/v/zhipuai.svg)](https://pypi.org/project/zhipuai/)
+# 更多用法
 
-**官方SDK能力简介**
-- 对所有接口进行了类型封装。
-- 初始化client并调用成员函数，无需关注http调用过程的各种细节，所见即所得。
-- 默认缓存token。
+请参考 [langchain_chinese](https://github.com/arcstep/langchain_chinese)
 
+------------------------------------------
 
+**官方接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)大模型接口 Python SDK（Big Model API SDK in Python），让开发者更便捷的调用智谱开放API
+
+**官方SDK** [![PyPI version](https://img.shields.io/pypi/v/zhipuai.svg)](https://pypi.org/project/zhipuai/)
```

