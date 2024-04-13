# Comparing `tmp/llama_index_storage_chat_store_redis-0.1.2.tar.gz` & `tmp/llama_index_storage_chat_store_redis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_chat_store_redis-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_storage_chat_store_redis-0.1.3.tar", max compression
```

## Comparing `llama_index_storage_chat_store_redis-0.1.2.tar` & `llama_index_storage_chat_store_redis-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-02-13 13:53:01.908484 llama_index_storage_chat_store_redis-0.1.2/README.md
--rw-r--r--   0        0        0       99 2024-02-13 13:53:01.908764 llama_index_storage_chat_store_redis-0.1.2/llama_index/storage/chat_store/redis/__init__.py
--rw-r--r--   0        0        0     9734 2024-02-13 13:53:01.908865 llama_index_storage_chat_store_redis-0.1.2/llama_index/storage/chat_store/redis/base.py
--rw-r--r--   0        0        0     1493 2024-02-21 21:46:33.540797 llama_index_storage_chat_store_redis-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 llama_index_storage_chat_store_redis-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-13 04:09:40.078510 llama_index_storage_chat_store_redis-0.1.3/README.md
+-rw-r--r--   0        0        0       99 2024-04-13 04:09:40.078510 llama_index_storage_chat_store_redis-0.1.3/llama_index/storage/chat_store/redis/__init__.py
+-rw-r--r--   0        0        0     9673 2024-04-13 04:09:40.078510 llama_index_storage_chat_store_redis-0.1.3/llama_index/storage/chat_store/redis/base.py
+-rw-r--r--   0        0        0     1493 2024-04-13 04:09:40.078510 llama_index_storage_chat_store_redis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 llama_index_storage_chat_store_redis-0.1.3/PKG-INFO
```

### Comparing `llama_index_storage_chat_store_redis-0.1.2/llama_index/storage/chat_store/redis/base.py` & `llama_index_storage_chat_store_redis-0.1.3/llama_index/storage/chat_store/redis/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 import redis
 from redis import Redis
 from redis.cluster import RedisCluster
 
 
 # Convert a ChatMessage to a json object for Redis
 def _message_to_dict(message: ChatMessage) -> dict:
-    return {"type": message.role, "content": message.content}
+    return message.dict()
 
 
 # Convert the json object in Redis to a ChatMessage
 def _dict_to_message(d: dict) -> ChatMessage:
-    return ChatMessage(role=d["type"], content=d["content"])
+    return ChatMessage.parse_obj(d)
 
 
 class RedisChatStore(BaseChatStore):
     """Redis chat store."""
 
     redis_client: Any = Field(description="Redis client.")
     ttl: Optional[int] = Field(default=None, description="Time to live in seconds.")
```

### Comparing `llama_index_storage_chat_store_redis-0.1.2/pyproject.toml` & `llama_index_storage_chat_store_redis-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index storage-chat-store redis integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-chat-store-redis"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 redis = ">=4.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_storage_chat_store_redis-0.1.2/PKG-INFO` & `llama_index_storage_chat_store_redis-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-chat-store-redis
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index storage-chat-store redis integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: redis (>=4.1.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Chat_Store Integration: Redis Chat Store
```

