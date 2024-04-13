# Comparing `tmp/wikidot-3.0.0a11.tar.gz` & `tmp/wikidot-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidot-3.0.0a11.tar", last modified: Sat Mar 16 20:22:57 2024, max compression
+gzip compressed data, was "wikidot-3.0.0a2.tar", last modified: Sat Apr 13 12:07:04 2024, max compression
```

## Comparing `wikidot-3.0.0a11.tar` & `wikidot-3.0.0a2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.634066 wikidot-3.0.0a11/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-03-16 19:56:22.000000 wikidot-3.0.0a11/LICENSE
--rw-r--r--   0 ukwhatn    (501) staff       (20)      917 2024-03-16 20:22:57.633864 wikidot-3.0.0a11/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)      133 2024-03-16 20:19:09.000000 wikidot-3.0.0a11/README.md
--rw-r--r--   0 ukwhatn    (501) staff       (20)      735 2024-03-16 20:21:42.000000 wikidot-3.0.0a11/pyproject.toml
--rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-03-16 20:22:57.634106 wikidot-3.0.0a11/setup.cfg
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.629577 wikidot-3.0.0a11/wikidot/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-03-16 20:20:13.000000 wikidot-3.0.0a11/wikidot/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.630646 wikidot-3.0.0a11/wikidot/common/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/common/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1140 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/common/decorators.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/common/exceptions.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/common/logger.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.631121 wikidot-3.0.0a11/wikidot/connector/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/connector/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    11105 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/connector/ajax.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/connector/api.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.632240 wikidot-3.0.0a11/wikidot/module/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/auth.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6174 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/client.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     8521 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/private_message.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     4845 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/site.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/site_application.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7728 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/module/user.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.632765 wikidot-3.0.0a11/wikidot/util/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.633080 wikidot-3.0.0a11/wikidot/util/parser/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/parser/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/parser/odate.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/parser/user.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/quick_module.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/requestutil.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/stringutil.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.633286 wikidot-3.0.0a11/wikidot/util/table/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/table/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-03-16 19:52:51.000000 wikidot-3.0.0a11/wikidot/util/table/char_table.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-03-16 20:22:57.633546 wikidot-3.0.0a11/wikidot.egg-info/
--rw-r--r--   0 ukwhatn    (501) staff       (20)      917 2024-03-16 20:22:57.000000 wikidot-3.0.0a11/wikidot.egg-info/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)      849 2024-03-16 20:22:57.000000 wikidot-3.0.0a11/wikidot.egg-info/SOURCES.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-03-16 20:22:57.000000 wikidot-3.0.0a11/wikidot.egg-info/dependency_links.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-03-16 20:22:57.000000 wikidot-3.0.0a11/wikidot.egg-info/requires.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-03-16 20:22:57.000000 wikidot-3.0.0a11/wikidot.egg-info/top_level.txt
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.657706 wikidot-3.0.0a2/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/LICENSE
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2684 2024-04-13 12:07:04.657492 wikidot-3.0.0a2/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1900 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/README.md
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      734 2024-04-13 12:01:44.000000 wikidot-3.0.0a2/pyproject.toml
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-13 12:07:04.657746 wikidot-3.0.0a2/setup.cfg
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.652650 wikidot-3.0.0a2/wikidot/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.653693 wikidot-3.0.0a2/wikidot/common/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/common/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-13 11:47:29.000000 wikidot-3.0.0a2/wikidot/common/decorators.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/common/exceptions.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/common/logger.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.654120 wikidot-3.0.0a2/wikidot/connector/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/connector/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    13291 2024-04-13 11:01:08.000000 wikidot-3.0.0a2/wikidot/connector/ajax.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/connector/api.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.655543 wikidot-3.0.0a2/wikidot/module/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/module/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/module/auth.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-13 11:47:18.000000 wikidot-3.0.0a2/wikidot/module/client.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    10770 2024-04-13 11:51:58.000000 wikidot-3.0.0a2/wikidot/module/page.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     8521 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/module/private_message.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-13 11:36:34.000000 wikidot-3.0.0a2/wikidot/module/site.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/module/site_application.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7728 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/module/user.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.656220 wikidot-3.0.0a2/wikidot/util/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.656644 wikidot-3.0.0a2/wikidot/util/parser/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/parser/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/parser/odate.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/parser/user.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/quick_module.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/requestutil.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/stringutil.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.656895 wikidot-3.0.0a2/wikidot/util/table/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/table/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-13 10:37:49.000000 wikidot-3.0.0a2/wikidot/util/table/char_table.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-13 12:07:04.657144 wikidot-3.0.0a2/wikidot.egg-info/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2684 2024-04-13 12:07:04.000000 wikidot-3.0.0a2/wikidot.egg-info/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      872 2024-04-13 12:07:04.000000 wikidot-3.0.0a2/wikidot.egg-info/SOURCES.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-13 12:07:04.000000 wikidot-3.0.0a2/wikidot.egg-info/dependency_links.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-13 12:07:04.000000 wikidot-3.0.0a2/wikidot.egg-info/requires.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-13 12:07:04.000000 wikidot-3.0.0a2/wikidot.egg-info/top_level.txt
```

### Comparing `wikidot-3.0.0a11/LICENSE` & `wikidot-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/pyproject.toml` & `wikidot-3.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wikidot"
-version = "3.0.0a11"
+version = "3.0.0a2"
 authors = [{ name = "ukwhatn", email = "ukwhatn@gmail.com" }]
 description = "Wikidot Utility Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wikidot-3.0.0a11/wikidot/common/decorators.py` & `wikidot-3.0.0a2/wikidot/common/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from functools import wraps
 
-from .exceptions import LoginRequiredException
-
 
 def login_required(func):
     """ログインが必要な関数につけるデコレータ
 
     関数のパラメータに存在するclientを取得し、ログインしていない場合は例外を送出する
     clientはパラメータ、もしくはself.clientで取得できる
     """
@@ -26,13 +24,12 @@
             if client is None:
                 if hasattr(args[0], 'client'):
                     client = args[0].client
 
         if client is None:
             raise ValueError('Client is not found')
 
-        if not client.is_logged_in:
-            raise LoginRequiredException('Login is required to execute this function')
+        client.login_check()
 
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `wikidot-3.0.0a11/wikidot/common/exceptions.py` & `wikidot-3.0.0a2/wikidot/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/connector/ajax.py` & `wikidot-3.0.0a2/wikidot/connector/ajax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import json.decoder
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Any, Tuple
 
 import httpx
 
 from ..common import wd_logger
 from ..common.exceptions import NotFoundException, AMCHttpStatusCodeException, ResponseDataException, \
     WikidotStatusCodeException
 
@@ -112,14 +113,21 @@
     """
     request_timeout: int = 20
     attempt_limit: int = 3
     retry_interval: int = 5
     semaphore_limit: int = 10
 
 
+@dataclass
+class HTTPRequestData:
+    url: str
+    headers: dict[str, any] = field(default_factory=dict)
+    data: dict[str, any] = field(default_factory=dict)
+
+
 class AjaxModuleConnectorClient:
     """ajax-module-connector.phpへのリクエストを行うクライアント"""
 
     def __init__(
             self,
             site_name: str | None = None,
             config: AjaxModuleConnectorConfig | None = None
@@ -160,15 +168,15 @@
 
     def request(
             self,
             bodies: list[dict[str, any]],
             return_exceptions: bool = False,
             site_name: str | None = None,
             site_ssl_supported: bool | None = None
-    ) -> list[httpx.Response | Exception]:
+    ) -> tuple[BaseException | Any]:
         """ajax-module-connector.phpへのリクエストを行う
 
         Parameters
         ----------
         bodies: list[dict]
             リクエストボディのリスト
         return_exceptions: bool
@@ -283,7 +291,50 @@
                 return response
 
         async def _execute_requests():
             return await asyncio.gather(*[_request(body) for body in bodies], return_exceptions=return_exceptions)
 
         # 処理を実行
         return asyncio.run(_execute_requests())
+
+    def get(self, datas: list[HTTPRequestData | dict[str, Any]]) -> tuple[Any]:
+        semaphore_instance = asyncio.Semaphore(self.config.semaphore_limit)
+
+        # datasの中身をHTTPRequestDataに変換
+        datas = [data if isinstance(data, HTTPRequestData) else HTTPRequestData(**data) for data in datas]
+
+        async def _get(_data: HTTPRequestData) -> httpx.Response:
+            retry_count = 0
+
+            while True:
+                try:
+                    async with semaphore_instance:
+                        async with httpx.AsyncClient() as client:
+                            wd_logger.debug(f'GET Request: {_data.url} -> {_data.data}')
+                            response = await client.get(
+                                _data.url,
+                                headers=_data.headers,
+                                params=_data.data,
+                                timeout=self.config.request_timeout
+                            )
+                            response.raise_for_status()
+                except (httpx.HTTPStatusError, httpx.TimeoutException) as e:
+                    retry_count += 1
+
+                    if retry_count >= self.config.attempt_limit:
+                        wd_logger.error(f'HTTP GET is respond HTTP error code: {response.status_code} -> {_data.url}')
+                        raise AMCHttpStatusCodeException(
+                            f'HTTP GET is respond HTTP error code: {response.status_code}',
+                            response.status_code
+                        ) from e
+
+                    wd_logger.info(
+                        f'HTTP GET is respond status: {response.status_code} (retry: {retry_count}) -> {_data.url}')
+                    await asyncio.sleep(self.config.retry_interval)
+                    continue
+
+                return response
+
+        async def _execute_gets():
+            return await asyncio.gather(*[_get(data) for data in datas])
+
+        return asyncio.run(_execute_gets())
```

### Comparing `wikidot-3.0.0a11/wikidot/module/auth.py` & `wikidot-3.0.0a2/wikidot/module/auth.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/module/client.py` & `wikidot-3.0.0a2/wikidot/module/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from wikidot.common import wd_logger
+from wikidot.common.exceptions import LoginRequiredException
 from wikidot.connector.ajax import AjaxModuleConnectorClient, AjaxModuleConnectorConfig
 from wikidot.module.auth import HTTPAuthentication
 from wikidot.module.private_message import PrivateMessage, PrivateMessageInbox, \
     PrivateMessageSentBox, PrivateMessageCollection
 from wikidot.module.site import Site
 from wikidot.module.user import User, UserCollection
 
@@ -218,7 +219,12 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.__del__()
         return
 
     def __str__(self):
         return f"Client(username={self.username}, is_logged_in={self.is_logged_in})"
+
+    def login_check(self) -> None:
+        if not self.is_logged_in:
+            raise LoginRequiredException('Login is required to execute this function')
+        return
```

### Comparing `wikidot-3.0.0a11/wikidot/module/private_message.py` & `wikidot-3.0.0a2/wikidot/module/private_message.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/module/site.py` & `wikidot-3.0.0a2/wikidot/module/site.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,83 @@
 import re
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 import httpx
 
 from wikidot.common import exceptions
 from wikidot.common.decorators import login_required
+from wikidot.module.page import SearchPagesQuery, PageCollection
 from wikidot.module.site_application import SiteApplication
 
 if TYPE_CHECKING:
     from wikidot.module.client import Client
     from wikidot.module.user import User
+    from wikidot.module.page import Page
+
+
+class SitePagesMethods:
+    def __init__(self, site: 'Site'):
+        self.site = site
+
+    def search(
+            self,
+            **kwargs
+    ) -> 'PageCollection':
+        """ページを検索する
+
+        Parameters
+        ----------
+        site: Site
+            サイト
+        query: SearchPagesQuery
+            検索クエリ
+
+        Returns
+        -------
+        PageCollection
+            ページのコレクション
+        """
+
+        query = SearchPagesQuery(**kwargs)
+        return PageCollection.search_pages(self.site, query)
+
+
+class SitePageMethods:
+    def __init__(self, site: 'Site'):
+        self.site = site
+
+    def get(
+            self,
+            fullname: str,
+            raise_when_not_found: bool = True
+    ) -> Optional['Page']:
+        """フルネームからページを取得する
+
+        Parameters
+        ----------
+        fullname: str
+            ページのフルネーム
+        raise_when_not_found: bool
+            ページが見つからなかった場合に例外を発生させるかどうか させない場合はNoneを返す
+
+        Returns
+        -------
+        Page
+            ページオブジェクト
+        """
+        res = PageCollection.search_pages(
+            self.site,
+            SearchPagesQuery(fullname=fullname)
+        )
+        if len(res) == 0:
+            if raise_when_not_found:
+                raise exceptions.NotFoundException(f'Page is not found: {fullname}')
+            return None
+        return res[0]
 
 
 @dataclass
 class Site:
     """サイトオブジェクト
 
     Attributes
@@ -41,14 +104,18 @@
 
     id: int
     title: str
     unix_name: str
     domain: str
     ssl_supported: bool
 
+    def __post_init__(self):
+        self.pages = SitePagesMethods(self)
+        self.page = SitePageMethods(self)
+
     def __str__(self):
         return f'Site(id={self.id}, title={self.title}, unix_name={self.unix_name})'
 
     @staticmethod
     def from_unix_name(
             client: 'Client',
             unix_name: str
@@ -143,7 +210,11 @@
                 raise exceptions.TargetErrorException(
                     f'User is already invited to {self.unix_name}: {user.name}') from e
             elif e.status_code == 'already_member':
                 raise exceptions.TargetErrorException(
                     f'User is already a member of {self.unix_name}: {user.name}') from e
             else:
                 raise e
+
+    def get_url(self):
+        """サイトのURLを取得する"""
+        return f'http{"s" if self.ssl_supported else ""}://{self.domain}'
```

### Comparing `wikidot-3.0.0a11/wikidot/module/site_application.py` & `wikidot-3.0.0a2/wikidot/module/site_application.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/module/user.py` & `wikidot-3.0.0a2/wikidot/module/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/parser/odate.py` & `wikidot-3.0.0a2/wikidot/util/parser/odate.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/parser/user.py` & `wikidot-3.0.0a2/wikidot/util/parser/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/quick_module.py` & `wikidot-3.0.0a2/wikidot/util/quick_module.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/requestutil.py` & `wikidot-3.0.0a2/wikidot/util/requestutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/stringutil.py` & `wikidot-3.0.0a2/wikidot/util/stringutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot/util/table/char_table.py` & `wikidot-3.0.0a2/wikidot/util/table/char_table.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.0a11/wikidot.egg-info/SOURCES.txt` & `wikidot-3.0.0a2/wikidot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 wikidot/common/logger.py
 wikidot/connector/__init__.py
 wikidot/connector/ajax.py
 wikidot/connector/api.py
 wikidot/module/__init__.py
 wikidot/module/auth.py
 wikidot/module/client.py
+wikidot/module/page.py
 wikidot/module/private_message.py
 wikidot/module/site.py
 wikidot/module/site_application.py
 wikidot/module/user.py
 wikidot/util/__init__.py
 wikidot/util/quick_module.py
 wikidot/util/requestutil.py
```

