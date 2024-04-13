# Comparing `tmp/nonebot_adapter_feishu-2.4.2.tar.gz` & `tmp/nonebot_adapter_feishu-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_feishu-2.4.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_feishu-2.5.0.tar", max compression
```

## Comparing `nonebot_adapter_feishu-2.4.2.tar` & `nonebot_adapter_feishu-2.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/LICENSE
--rw-r--r--   0        0        0     2459 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/README.md
--rw-r--r--   0        0        0      863 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/__init__.py
--rw-r--r--   0        0        0    11470 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/adapter.py
--rw-r--r--   0        0        0    10938 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/bot.py
--rw-r--r--   0        0        0     1327 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/config.py
--rw-r--r--   0        0        0    12019 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/event.py
--rw-r--r--   0        0        0     1348 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/exception.py
--rw-r--r--   0        0        0    16594 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/message.py
--rw-r--r--   0        0        0       69 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/models/__init__.py
--rw-r--r--   0        0        0      725 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/models/api.py
--rw-r--r--   0        0        0    12854 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/models/common.py
--rw-r--r--   0        0        0      911 2024-02-22 12:37:40.720833 nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/utils.py
--rw-r--r--   0        0        0     2386 2024-02-22 12:37:40.724833 nonebot_adapter_feishu-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2459 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/README.md
+-rw-r--r--   0        0        0      863 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/__init__.py
+-rw-r--r--   0        0        0    11552 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/adapter.py
+-rw-r--r--   0        0        0    10938 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/bot.py
+-rw-r--r--   0        0        0     1366 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/config.py
+-rw-r--r--   0        0        0    12019 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/event.py
+-rw-r--r--   0        0        0     1348 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/exception.py
+-rw-r--r--   0        0        0    16590 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/message.py
+-rw-r--r--   0        0        0       69 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/api.py
+-rw-r--r--   0        0        0    12854 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/common.py
+-rw-r--r--   0        0        0      911 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/utils.py
+-rw-r--r--   0        0        0     2386 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.5.0/PKG-INFO
```

### Comparing `nonebot_adapter_feishu-2.4.2/LICENSE` & `nonebot_adapter_feishu-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/README.md` & `nonebot_adapter_feishu-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/__init__.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/adapter.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,17 @@
                 "doesn't support http client requests!"
                 f"{self.get_name()} Adapter needs a HTTPClient Driver to work."
             )
 
         self.driver.on_startup(self.startup)
 
     def get_api_base(self, bot_config: BotConfig) -> URL:
+        if bot_config.api_base:
+            return URL(str(bot_config.api_base))
+
         if bot_config.is_lark:
             return URL(str(self.feishu_config.feishu_lark_api_base))
         else:
             return URL(str(self.feishu_config.feishu_api_base))
 
     def get_api_url(self, bot_config: BotConfig, path: str):
         return self.get_api_base(bot_config).joinpath("open-apis", path)
```

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/bot.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/config.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """
 
     app_id: str
     app_secret: str
     encrypt_key: Optional[str] = None
     verification_token: str
     is_lark: bool = False
+    api_base: Optional[HttpUrl] = None
 
 
 class Config(BaseModel):
     """
     飞书适配器全局配置类
 
     :配置项:
```

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/event.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/exception.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/message.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return Text("text", {"text": str(text)})
 
     @staticmethod
     def at(user_id: str):
         return At("at", {"user_id": user_id})
 
     @staticmethod
-    def post(title: str, content: List[List["PostMessageNode"]]) -> "Post":
+    def post(title: str, content: List[List[Dict[str, Any]]]) -> "Post":
         return Post("post", data={"title": title, "content": content})
 
     @staticmethod
     def image(image_key: str) -> "Image":
         return Image("image", {"image_key": image_key})
 
     @staticmethod
@@ -410,15 +410,15 @@
 
 class PostEmotion(PostMessageNode):
     emoji_type: str
 
 
 class _PostData(TypedDict):
     title: str
-    content: List[List[PostMessageNode]]
+    content: List[List[Dict[str, Any]]]
 
 
 @dataclass
 class Post(MessageSegment):
     if TYPE_CHECKING:
         data: _PostData
```

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/models/api.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/models/common.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/nonebot/adapters/feishu/utils.py` & `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.4.2/pyproject.toml` & `nonebot_adapter_feishu-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-feishu"
-version = "2.4.2"
+version = "2.5.0"
 description = "feishu(larksuite) adapter for nonebot2"
 authors = ["StarHeartHunt <starheart233@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://feishu.adapters.nonebot.dev/"
 repository = "https://github.com/nonebot/adapter-feishu"
 documentation = "https://feishu.adapters.nonebot.dev/"
@@ -21,15 +21,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.2.0"
 cashews = "^7.0.0"
 pycryptodome = ">=3.18.0, <4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.0"
+ruff = "^0.3.0"
 isort = "^5.10.1"
 black = "^24.0.0"
 nonemoji = "^0.1.2"
 pre-commit = "^3.2.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = [
   "fastapi",
   "httpx",
```

### Comparing `nonebot_adapter_feishu-2.4.2/PKG-INFO` & `nonebot_adapter_feishu-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-feishu
-Version: 2.4.2
+Version: 2.5.0
 Summary: feishu(larksuite) adapter for nonebot2
 Home-page: https://feishu.adapters.nonebot.dev/
 License: MIT
 Keywords: bot,feishu,larksuite
 Author: StarHeartHunt
 Author-email: starheart233@gmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.4.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.5.0 Summary:
 feishu(larksuite) adapter for nonebot2 Home-page: https://
 feishu.adapters.nonebot.dev/ License: MIT Keywords: bot,feishu,larksuite
 Author: StarHeartHunt Author-email: starheart233@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
 Library Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

