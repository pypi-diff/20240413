# Comparing `tmp/avilla_red-1.0.0a7.tar.gz` & `tmp/avilla_red-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla_red-1.0.0a7.tar", last modified: Sat Sep  2 13:54:59 2023, max compression
+gzip compressed data, was "avilla_red-1.0.0a9.tar", last modified: Fri Oct 20 14:21:59 2023, max compression
```

## Comparing `avilla_red-1.0.0a7.tar` & `avilla_red-1.0.0a9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      510 2023-09-02 13:54:42.284647 avilla_red-1.0.0a7/.mina/red.toml
--rw-r--r--   0        0        0     1070 2023-09-02 13:54:42.284647 avilla_red-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     8360 2023-09-02 13:54:42.284647 avilla_red-1.0.0a7/README.md
--rw-r--r--   0        0        0       94 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/__init__.py
--rw-r--r--   0        0        0      657 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/account.py
--rw-r--r--   0        0        0        0 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/collector/__init__.py
--rw-r--r--   0        0        0      894 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/collector/connection.py
--rw-r--r--   0        0        0     1104 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/exception.py
--rw-r--r--   0        0        0        0 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/net/__init__.py
--rw-r--r--   0        0        0     5215 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/net/base.py
--rw-r--r--   0        0        0     6978 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/net/ws_client.py
--rw-r--r--   0        0        0        0 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/__init__.py
--rw-r--r--   0        0        0        0 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/action/__init__.py
--rw-r--r--   0        0        0     2097 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/action/friend.py
--rw-r--r--   0        0        0     3976 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/action/group.py
--rw-r--r--   0        0        0     3287 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/action/member.py
--rw-r--r--   0        0        0     4027 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/action/message.py
--rw-r--r--   0        0        0     1530 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/context.py
--rw-r--r--   0        0        0        0 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/__init__.py
--rw-r--r--   0        0        0     5074 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/group.py
--rw-r--r--   0        0        0     1593 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/lifespan.py
--rw-r--r--   0        0        0     6511 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/member.py
--rw-r--r--   0        0        0     3362 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/message.py
--rw-r--r--   0        0        0     2832 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/event/relationship.py
--rw-r--r--   0        0        0     4402 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/message/deserialize.py
--rw-r--r--   0        0        0     2779 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/message/serialize.py
--rw-r--r--   0        0        0     2960 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/query.py
--rw-r--r--   0        0        0     1930 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/perform/resource_fetch.py
--rw-r--r--   0        0        0     2643 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/protocol.py
--rw-r--r--   0        0        0     1728 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/resource.py
--rw-r--r--   0        0        0     1098 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/service.py
--rw-r--r--   0        0        0     3865 2023-09-02 13:54:42.292647 avilla_red-1.0.0a7/avilla/red/utils.py
--rw-r--r--   0        0        0      963 2023-09-02 13:54:59.680911 avilla_red-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0     8782 1970-01-01 00:00:00.000000 avilla_red-1.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0      492 2023-10-20 14:21:44.454844 avilla_red-1.0.0a9/.mina/red.toml
+-rw-r--r--   0        0        0     1070 2023-10-20 14:21:44.454844 avilla_red-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     8613 2023-10-20 14:21:44.454844 avilla_red-1.0.0a9/README.md
+-rw-r--r--   0        0        0       94 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/__init__.py
+-rw-r--r--   0        0        0      657 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/account.py
+-rw-r--r--   0        0        0     1985 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/capability.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/collector/__init__.py
+-rw-r--r--   0        0        0      905 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/collector/connection.py
+-rw-r--r--   0        0        0     1104 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/exception.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/net/__init__.py
+-rw-r--r--   0        0        0     5467 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/net/base.py
+-rw-r--r--   0        0        0     7325 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/net/ws_client.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/action/__init__.py
+-rw-r--r--   0        0        0     2168 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/action/friend.py
+-rw-r--r--   0        0        0     4076 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/action/group.py
+-rw-r--r--   0        0        0     4307 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/action/member.py
+-rw-r--r--   0        0        0     9010 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/action/message.py
+-rw-r--r--   0        0        0     1693 2023-10-20 14:21:44.462844 avilla_red-1.0.0a9/avilla/red/perform/context.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/__init__.py
+-rw-r--r--   0        0        0     5127 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/group.py
+-rw-r--r--   0        0        0     1832 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/lifespan.py
+-rw-r--r--   0        0        0     6639 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/member.py
+-rw-r--r--   0        0        0     3604 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/message.py
+-rw-r--r--   0        0        0     2843 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/event/relationship.py
+-rw-r--r--   0        0        0     5555 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/message/deserialize.py
+-rw-r--r--   0        0        0     6307 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/message/serialize.py
+-rw-r--r--   0        0        0     3026 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/query.py
+-rw-r--r--   0        0        0     2151 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/perform/resource_fetch.py
+-rw-r--r--   0        0        0     3182 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/protocol.py
+-rw-r--r--   0        0        0     2059 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/resource.py
+-rw-r--r--   0        0        0     1098 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/service.py
+-rw-r--r--   0        0        0     3852 2023-10-20 14:21:44.466845 avilla_red-1.0.0a9/avilla/red/utils.py
+-rw-r--r--   0        0        0      957 2023-10-20 14:21:59.434028 avilla_red-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     9035 1970-01-01 00:00:00.000000 avilla_red-1.0.0a9/PKG-INFO
```

### Comparing `avilla_red-1.0.0a7/LICENSE` & `avilla_red-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `avilla_red-1.0.0a7/README.md` & `avilla_red-1.0.0a9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 |:--------------------------------------------:|:----------------:|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------------------------:|:--------:|:------:|
 |             [Core](avilla/core)              |        -         |           -            |  **Alpha**  |            [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)            | Official |  MIT   |
 |          [Console](avilla/console)           |       终端环境       |       `Console`        |  **Alpha**  |         [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)         | Official |  MIT   |
 |        [Elizabeth](avilla/elizabeth)         |    Tencent QQ    |    `mirai-api-http`    |  **Alpha**  |       [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)       | Official | AGPLv3 |
 |        [Onebot 11](avilla/onebot/v11)        |     *多平台支持*      |      `OneBot v11`      |   **WIP**   |      [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11)      | Official |   -    |
 | [QQ Guild (Tencent)](avilla/qqguild/tencent) | Tencent QQ Guild | `QQGuild Official API` |   **WIP**   | [![image](https://img.shields.io/pypi/v/avilla-qqguild-tencent)](https://pypi.org/project/avilla-qqguild-tencent) | Official |  MIT   |
 |              [Red](avilla/red)               |   Tencent QQNT   |     `Red Protocol`     |   **WIP**   |             [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)             | Official |  MIT   |
+|           [Satori](avilla/satori)            |     *多平台支持*      | `Satori Protocol (v1)` |   **WIP**   |          [![image](https://img.shields.io/pypi/v/avilla-satori)](https://pypi.org/project/avilla-satori)          | Official |  MIT   |
 |         [Telegram](avilla/telegram)          |     Telegram     |       `Telegram`       |  **Draft**  |        [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)        |    -     |   -    |
 |        [Nightcord](avilla/nightcord)         |     Discord      |     `Discord Bots`     |  **Draft**  |       [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)       |    -     |   -    |
 |             [Kook](avilla/kook)              |       Kook       |         `Kook`         |  **Draft**  |            [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)            |    -     |   -    |
 |        [OneBot 12](avilla/onebot/v12)        |     *多平台支持*      |      `OneBot v12`      | **Planned** |                                                         -                                                         |    -     |   -    |
 
 ## 我们的愿景
```

### Comparing `avilla_red-1.0.0a7/avilla/red/account.py` & `avilla_red-1.0.0a9/avilla/red/account.py`

 * *Files identical despite different names*

### Comparing `avilla_red-1.0.0a7/avilla/red/collector/connection.py` & `avilla_red-1.0.0a9/avilla/red/collector/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar, TypeVar
 
-from avilla.core.ryanvk.collector.base import AvillaBaseCollector, BasePerform
-from graia.ryanvk import Access
+from avilla.core.ryanvk.collector.base import AvillaBaseCollector
+from graia.ryanvk import Access, BasePerform
 
 if TYPE_CHECKING:
     from avilla.red.net.ws_client import RedWsClientNetworking
     from avilla.red.protocol import RedProtocol
 
 
 T = TypeVar("T")
@@ -27,11 +27,12 @@
     @property
     def _(self):
         upper = super()._
 
         class PerformTemplate(
             ConnectionBasedPerformTemplate,
             upper,
+            native=True,
         ):
-            __native__ = True
+            ...
 
         return PerformTemplate
```

### Comparing `avilla_red-1.0.0a7/avilla/red/exception.py` & `avilla_red-1.0.0a9/avilla/red/exception.py`

 * *Files identical despite different names*

### Comparing `avilla_red-1.0.0a7/avilla/red/net/ws_client.py` & `avilla_red-1.0.0a9/avilla/red/net/ws_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 from launart import Service
 from launart.manager import Launart
 from launart.utilles import any_completed
 from loguru import logger
 
 from avilla.red.account import RedAccount
 from avilla.red.net.base import RedNetworking
-from avilla.standard.core.account import AccountUnregistered
+from avilla.standard.core.account import AccountUnregistered, AccountUnavailable
 
 if TYPE_CHECKING:
-    from avilla.red.protocol import RedProtocol, RedConfig
+    from avilla.red.protocol import RedConfig, RedProtocol
 
 
-class RedWsClientNetworking(RedNetworking["RedWsClientNetworking"], Service):
-    id = "red/connection/websocket/client"
-
+class RedWsClientNetworking(RedNetworking, Service):
     required: set[str] = set()
     stages: set[str] = {"preparing", "blocking", "cleanup"}
 
     config: RedConfig
     connection: aiohttp.ClientWebSocketResponse | None = None
     session: aiohttp.ClientSession
 
     def __init__(self, protocol: RedProtocol, config: RedConfig) -> None:
         super().__init__(protocol)
         self.config = config
 
+    @property
+    def id(self):
+        return f"satori/connection/websocket/client#{id(self)}"
+
     async def message_receive(self):
         if self.connection is None:
             raise RuntimeError("connection is not established")
 
         async for msg in self.connection:
             if msg.type in {aiohttp.WSMsgType.CLOSE, aiohttp.WSMsgType.ERROR, aiohttp.WSMsgType.CLOSED}:
                 self.close_signal.set()
@@ -101,63 +103,66 @@
 
     @property
     def alive(self):
         return self.connection is not None and not self.connection.closed
 
     async def connection_daemon(self, manager: Launart, session: aiohttp.ClientSession):
         while not manager.status.exiting:
-            async with session.ws_connect(self.config.endpoint) as self.connection:
-                logger.info(f"{self} Websocket client connected")
-                self.close_signal.clear()
-
-                close_task = asyncio.create_task(self.close_signal.wait())
-                receiver_task = asyncio.create_task(self.message_handle())
-                sigexit_task = asyncio.create_task(manager.status.wait_for_sigexit())
-                await self.send(
-                    {
-                        "type": "meta::connect",
-                        "payload": {
-                            "token": self.config.access_token,
-                        },
-                    }
-                )
-                done, pending = await any_completed(
-                    sigexit_task,
-                    close_task,
-                    receiver_task,
-                )
-                avilla = self.protocol.avilla
-                if sigexit_task in done:
-                    logger.info(f"{self} Websocket client exiting...")
-                    await self.connection.close()
-                    self.close_signal.set()
-                    self.connection = None
-                    for v in list(avilla.accounts.values()):
-                        if v.protocol is self.protocol:
-                            _account = v.route["account"]
-                            if _account == self.account.route["account"]:  # type: ignore
+            try:
+                async with session.ws_connect(
+                    self.config.endpoint,
+                    timeout=30
+                ) as self.connection:
+                    logger.info(f"{self} Websocket client connected")
+                    self.close_signal.clear()
+
+                    close_task = asyncio.create_task(self.close_signal.wait())
+                    receiver_task = asyncio.create_task(self.message_handle())
+                    sigexit_task = asyncio.create_task(manager.status.wait_for_sigexit())
+                    await self.send(
+                        {
+                            "type": "meta::connect",
+                            "payload": {
+                                "token": self.config.access_token,
+                            },
+                        }
+                    )
+                    done, pending = await any_completed(
+                        sigexit_task,
+                        close_task,
+                        receiver_task,
+                    )
+                    avilla = self.protocol.avilla
+                    if sigexit_task in done:
+                        logger.info(f"{self} Websocket client exiting...")
+                        await self.connection.close()
+                        self.close_signal.set()
+                        self.connection = None
+                        for v in list(avilla.accounts.values()):
+                            if v.protocol is self.protocol and self.account and v.route["account"] == self.account.route["account"]:  # type: ignore
                                 self.account = None
-                    return
-                if close_task in done:
-                    receiver_task.cancel()
-                    logger.warning(f"{self} Connection closed by server, will reconnect in 5 seconds...")
-                    for n in list(avilla.accounts.keys()):
-                        logger.debug(f"Unregistering red-protocol account {n}...")
-                        account = cast("RedAccount", avilla.accounts[n].account)
-                        account.status.enabled = False
-                        await avilla.broadcast.postEvent(AccountUnregistered(avilla, avilla.accounts[n].account))
-                        if (
-                            n.follows("land(qq).account")
-                            and n["account"] == self.account.route["account"]  # type: ignore
-                        ):
-                            del avilla.accounts[n]
-                    self.account = None
-                    await asyncio.sleep(5)
-                    logger.info(f"{self} Reconnecting...")
-                    continue
+                                del avilla.accounts[v.route]
+                                await avilla.broadcast.postEvent(AccountUnregistered(avilla, v.account))
+                                return
+                    if close_task in done:
+                        receiver_task.cancel()
+                        logger.warning(f"{self} Connection closed by server, will reconnect in 5 seconds...")
+                        for n in list(avilla.accounts.keys()):
+                            logger.debug(f"Unregistering red-protocol account {n}...")
+                            account = cast("RedAccount", avilla.accounts[n].account)
+                            account.status.enabled = False
+                            await avilla.broadcast.postEvent(AccountUnavailable(avilla, avilla.accounts[n].account))
+                        self.account = None
+                        await asyncio.sleep(5)
+                        logger.info(f"{self} Reconnecting...")
+                        continue
+            except Exception as e:
+                logger.error(f"{self} Error while connecting: {e}")
+                await asyncio.sleep(5)
+                logger.info(f"{self} Reconnecting...")
 
     async def launch(self, manager: Launart):
         async with self.stage("preparing"):
             self.session = aiohttp.ClientSession()
 
         async with self.stage("blocking"):
             await self.connection_daemon(manager, self.session)
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/action/friend.py` & `avilla_red-1.0.0a9/avilla/red/perform/action/friend.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 
 from typing import TYPE_CHECKING, cast
 
 from avilla.core.exceptions import UnknownTarget
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.core.selector import Selector
 from avilla.standard.core.profile import Nick, Summary
-from graia.amnesia.builtins.memcache import MemcacheService, Memcache
+from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 
 if TYPE_CHECKING:
     from avilla.red.account import RedAccount  # noqa
     from avilla.red.protocol import RedProtocol  # noqa
 
 
 class RedFriendActionPerform((m := AccountCollector["RedProtocol", "RedAccount"]())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::action"
+    m.identify = "friend"
 
     @m.pull("land.friend", Summary)
-    async def get_summary(self, target: Selector) -> Summary:
+    async def get_summary(self, target: Selector, route: ...) -> Summary:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         if raw := await cache.get(f"red/account({self.account.route['account']}).friend({target.pattern['friend']})"):
             return Summary(raw["nick"], "a friend contact assigned to this account")
         result = await self.account.websocket_client.call_http("get", "api/bot/friends", {})
         result = cast(list, result)
         for i in result:
             friend_id = str(i["uin"])
             if friend_id == target["friend"]:
                 return Summary(i["nick"], "name of friend")
         raise UnknownTarget("Friend not found")
 
     @m.pull("land.friend", Nick)
-    async def get_nick(self, target: Selector) -> Nick:
+    async def get_nick(self, target: Selector, route: ...) -> Nick:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         if raw := await cache.get(f"red/account({self.account.route['account']}).friend({target.pattern['friend']})"):
             return Nick(raw["nick"], raw["remark"] or raw["nick"], raw["longNick"])
         result = await self.account.websocket_client.call_http("get", "api/bot/friends", {})
         result = cast(list, result)
         for i in result:
             friend_id = str(i["uin"])
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/action/group.py` & `avilla_red-1.0.0a9/avilla/red/perform/action/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,76 +5,77 @@
 from avilla.core.exceptions import UnknownTarget
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.core.selector import Selector
 from avilla.standard.core.common import Count
 from avilla.standard.core.privilege import MuteAllCapability
 from avilla.standard.core.profile import Nick, Summary
 from avilla.standard.core.relation import SceneCapability
-from graia.amnesia.builtins.memcache import MemcacheService, Memcache
+from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 
 if TYPE_CHECKING:
     from avilla.red.account import RedAccount  # noqa
     from avilla.red.protocol import RedProtocol  # noqa
 
 
 class RedGroupActionPerform((m := AccountCollector["RedProtocol", "RedAccount"]())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::action"
+    m.identify = "group"
 
     @m.pull("land.group", Summary)
-    async def get_summary(self, target: Selector) -> Summary:
+    async def get_summary(self, target: Selector, route: ...) -> Summary:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']})"):
             return Summary(raw["name"], "a group contact assigned to this account")
         result = await self.account.websocket_client.call_http("get", "api/bot/groups", {})
         result = cast(list, result)
         for i in result:
             group_id = str(i["groupCode"])
             if group_id == target["group"]:
                 return Summary(i["groupName"], "name of group")
         raise UnknownTarget("Group not found")
 
     @m.pull("land.group", Nick)
-    async def get_nick(self, target: Selector) -> Nick:
+    async def get_nick(self, target: Selector, route: ...) -> Nick:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']})"):
             return Nick(raw["name"], raw["remark"] or raw["name"], None)
         result = await self.account.websocket_client.call_http("get", "api/bot/groups", {})
         result = cast(list, result)
         for i in result:
             group_id = str(i["groupCode"])
             if group_id == target["group"]:
                 return Nick(i["groupName"], i["remarkName"], None)
         raise UnknownTarget("Group not found")
 
     @m.pull("land.group", Count)
-    async def get_count(self, target: Selector) -> Count:
+    async def get_count(self, target: Selector, route: ...) -> Count:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']})"):
             return Count(raw["memberCount"], raw["maxMember"])
         result = await self.account.websocket_client.call_http("get", "api/bot/groups", {})
         result = cast(list, result)
         for i in result:
             group_id = str(i["groupCode"])
             if group_id == target["group"]:
                 return Count(i["memberCount"], i["maxMember"])
         raise UnknownTarget("Group not found")
 
-    @MuteAllCapability.mute_all.collect(m, "land.group")
+    @m.entity(MuteAllCapability.mute_all, target="land.group")
     async def mute_all(self, target: Selector):
         await self.account.websocket_client.call_http(
             "post", "api/group/muteEveryone", {"group": int(target["group"]), "enable": True}
         )
 
-    @MuteAllCapability.unmute_all.collect(m, "land.group")
+    @m.entity(MuteAllCapability.unmute_all, target="land.group")
     async def unmute_all(self, target: Selector):
         await self.account.websocket_client.call_http(
             "post", "api/group/muteEveryone", {"group": int(target["group"]), "enable": False}
         )
 
-    @SceneCapability.remove_member.collect(m, "land.group.member")
+    @m.entity(SceneCapability.remove_member, target="land.group.member")
     async def remove_member(self, target: Selector, reason: str | None = None):
         await self.account.websocket_client.call_http(
             "post",
             "api/group/kick",
             {
                 "group": int(target["group"]),
                 "uidList": [int(target["member"])],
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/action/member.py` & `avilla_red-1.0.0a9/avilla/red/perform/action/member.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,63 +2,93 @@
 
 from datetime import timedelta
 from typing import TYPE_CHECKING, cast
 
 from avilla.core.exceptions import UnknownTarget
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.core.selector import Selector
+from avilla.standard.core.privilege import MuteCapability, MuteInfo
 from avilla.standard.core.profile import Nick, Summary
-from avilla.standard.core.privilege import MuteInfo
-from graia.amnesia.builtins.memcache import MemcacheService, Memcache
+from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 
 if TYPE_CHECKING:
     from avilla.red.account import RedAccount  # noqa
     from avilla.red.protocol import RedProtocol  # noqa
 
 
 class RedMemberActionPerform((m := AccountCollector["RedProtocol", "RedAccount"]())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::action"
+    m.identify = "member"
 
     @m.pull("land.group.member", Summary)
-    async def get_summary(self, target: Selector) -> Summary:
+    async def get_summary(self, target: Selector, route: ...) -> Summary:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
-        if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"):
+        if raw := await cache.get(
+            f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"
+        ):
             return Summary(raw["nick"], "a member of this group")
-        result = await self.account.websocket_client.call_http("get", "api/group/getMemberList", {"group": target.pattern["group"]})
+        result = await self.account.websocket_client.call_http(
+            "get", "api/group/getMemberList", {"group": target.pattern["group"]}
+        )
         result = cast(list, result)
         for i in result:
             member_id = str(i["uin"])
             if member_id == target["member"]:
                 return Summary(i["nick"], "name of member")
         raise UnknownTarget("Member not found")
 
     @m.pull("land.group.member", Nick)
-    async def get_nick(self, target: Selector) -> Nick:
+    async def get_nick(self, target: Selector, route: ...) -> Nick:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
-        if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"):
+        if raw := await cache.get(
+            f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"
+        ):
             return Nick(raw["nick"], raw["remark"] or raw["nick"], raw["cardName"])
-        result = await self.account.websocket_client.call_http("get", "api/group/getMemberList", {"group": target.pattern["group"]})
+        result = await self.account.websocket_client.call_http(
+            "get", "api/group/getMemberList", {"group": target.pattern["group"]}
+        )
         result = cast(list, result)
         for i in result:
             member_id = str(i["uin"])
             if member_id == target["member"]:
                 return Nick(i["nick"], i["card"], i["cardName"])
         raise UnknownTarget("Member not found")
 
     @m.pull("land.group.member", MuteInfo)
-    async def get_mute_info(self, target: Selector) -> MuteInfo:
+    async def get_mute_info(self, target: Selector, route: ...) -> MuteInfo:
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
-        if raw := await cache.get(f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"):
+        if raw := await cache.get(
+            f"red/account({self.account.route['account']}).group({target.pattern['group']}).member({target.pattern['member']})"
+        ):
             return MuteInfo(
                 raw["shutUpTime"] > 0,
                 timedelta(seconds=raw["shutUpTime"]),
             )
-        result = await self.account.websocket_client.call_http("get", "api/group/getMemberList", {"group": target.pattern["group"]})
+        result = await self.account.websocket_client.call_http(
+            "get", "api/group/getMemberList", {"group": target.pattern["group"]}
+        )
         result = cast(list, result)
         for i in result:
             member_id = str(i["uin"])
             if member_id == target["member"]:
                 return MuteInfo(
                     i["shutUpTime"] > 0,
                     timedelta(seconds=i["shutUpTime"]),
                 )
         raise UnknownTarget("Member not found")
+
+    @m.entity(MuteCapability.mute, target="land.group.member")
+    async def group_member_mute(self, target: Selector, duration: timedelta):
+        time = max(60.0, min(duration.total_seconds(), 2592000))
+        await self.account.websocket_client.call_http(
+            "post",
+            "api/group/muteMember",
+            {"group": int(target["group"]), "memList": [{"uin": int(target["member"]), "timeStamp": time}]},
+        )
+
+    @m.entity(MuteCapability.unmute, target="land.group.member")
+    async def group_member_unmute(self, target: Selector):
+        await self.account.websocket_client.call_http(
+            "post",
+            "api/group/muteMember",
+            {"group": int(target["group"]), "memList": [{"uin": int(target["member"]), "timeStamp": 0}]},
+        )
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/context.py` & `avilla_red-1.0.0a9/avilla/red/perform/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from avilla.core.builtins.capability import CoreCapability
+from avilla.core.context import Context
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.core.selector import Selector
-from avilla.core.context import Context
-from avilla.core.builtins.capability import CoreCapability
 
 if TYPE_CHECKING:
     from avilla.red.account import RedAccount  # noqa
     from avilla.red.protocol import RedProtocol  # noqa
 
 
 class RedContextPerform((m := AccountCollector["RedProtocol", "RedAccount"]())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::context"
 
-    @CoreCapability.get_context.collect(m, "land.group")
+    @m.entity(CoreCapability.get_context, target="land.group")
     def get_context_from_group(self, target: Selector, *, via: Selector | None = None):
         return Context(
             self.account,
             target,
             target,
             target,
             target.member(self.account.route["account"]),
         )
 
-    @CoreCapability.get_context.collect(m, "land.friend")
+    @m.entity(CoreCapability.get_context, target="land.friend")
     def get_context_from_friend(self, target: Selector, *, via: Selector | None = None):
-        return Context(
-            self.account,
-            target,
-            self.account.route,
-            target,
-            self.account.route
-        )
+        if via:
+            return Context(
+                self.account,
+                via,
+                target,
+                target,
+                self.account.route,
+            )
+        return Context(self.account, target, self.account.route, target, self.account.route)
 
-    @CoreCapability.get_context.collect(m, "land.group.member")
+    @m.entity(CoreCapability.get_context, target="land.group.member")
     def get_context_from_member(self, target: Selector, *, via: Selector | None = None):
         return Context(
             self.account,
             target,
             target.into("::group"),
             target.into("::group"),
             target.into(f"~.member({self.account.route['account']})"),
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/event/group.py` & `avilla_red-1.0.0a9/avilla/red/perform/event/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
+from loguru import logger
+
 from avilla.core.context import Context
 from avilla.core.event import MetadataModified, ModifyDetail
 from avilla.core.selector import Selector
-from avilla.core.ryanvk.descriptor.event import EventParse
-from avilla.standard.core.profile import Summary
+from avilla.red.capability import RedCapability
 from avilla.red.collector.connection import ConnectionCollector
-from loguru import logger
+from avilla.standard.core.profile import Summary
 
 
 class RedEventGroupPerform((m := ConnectionCollector())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::event"
+    m.identify = "group"
+
 
-    @EventParse.collect(m, "group::name_update")
-    async def group_name_change(self, raw_event: dict):
+    @m.entity(RedCapability.event_callback, event_type="group::name_update")
+    async def group_name_change(self, event_type: ..., raw_event: dict):
         account = self.connection.account
         if account is None:
             logger.warning(f"Unknown account received message {raw_event}")
             return
         group = Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
         group_data = raw_event["elements"][0]["grayTipElement"]["groupElement"]
         operator = group.member(str(group_data["memberUin"]))
@@ -28,20 +31,20 @@
             group,
             group.member(account.route["account"]),
         )
         return MetadataModified(
             context,
             group,
             Summary,
-            {
-                Summary.inh(lambda x: x.name): ModifyDetail("update", group_data["groupName"], "")
-            },
+            {Summary.inh(lambda x: x.name): ModifyDetail("update", group_data["groupName"], "")},
             operator=operator,
             scene=group,
         )
+
+
 _ = {
     "msgId": "7273401197226772043",
     "msgRandom": "7198583817760031691",
     "msgSeq": "6288",
     "cntSeq": "0",
     "chatType": 2,
     "msgType": 5,
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/event/lifespan.py` & `avilla_red-1.0.0a9/avilla/red/perform/event/lifespan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 from loguru import logger
 
 from avilla.core.account import AccountInfo
 from avilla.core.platform import Abstract, Land, Platform, Version
-from avilla.core.ryanvk.descriptor.event import EventParse
 from avilla.core.selector import Selector
 from avilla.red.account import RedAccount
+from avilla.red.capability import RedCapability
 from avilla.red.collector.connection import ConnectionCollector
-from avilla.standard.core.account.event import AccountRegistered
-
-if TYPE_CHECKING:
-    ...
+from avilla.standard.core.account.event import AccountRegistered, AccountAvailable
 
 
 class RedEventLifespanPerform((m := ConnectionCollector())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::event"
+    m.identify = "lifespan"
 
-    @EventParse.collect(m, "meta::connect")
-    async def connect(self, raw_event: dict):
+    @m.entity(RedCapability.event_callback, event_type="meta::connect")
+    async def connect(self,  event_type: ..., raw_event: dict):
         self_id: int = raw_event["authData"]["account"]
         account = self.connection.account
+
         if account is None:
             # create account instance
             account = RedAccount(route=Selector().land("qq").account(str(self_id)), protocol=self.protocol)
+            version_info = raw_event["version"]
+            platform = Platform(
+                Land("qq"),
+                Abstract(f"red-protocol/{version_info}"),
+                Version({"app": version_info}),
+            )
+            self.connection.account = account
+            self.protocol.avilla.accounts[account.route] = AccountInfo(account.route, account, self.protocol, platform)
+            account.websocket_client = self.connection
+            logger.success(f"Account {self_id} connected and created with red-protocol version {version_info}")
+            return AccountRegistered(self.protocol.avilla, account)
         else:
+            self.connection.account = account
             account.route = Selector().land("qq").account(str(self_id))
-
-        version_info = raw_event["version"]
-        platform = Platform(
-            Land("qq"),
-            Abstract(f"red-protocol/{version_info}"),
-            Version({"app": version_info}),
-        )
-
-        self.connection.account = account
-        self.protocol.avilla.accounts[account.route] = AccountInfo(account.route, account, self.protocol, platform)
-        account.websocket_client = self.connection
-
-        logger.info(f"Account {self_id} connected and created")
-        return AccountRegistered(self.protocol.avilla, account)
+            return AccountAvailable(self.protocol.avilla, account)
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/event/member.py` & `avilla_red-1.0.0a9/avilla/red/perform/event/member.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 from datetime import timedelta
 
+from loguru import logger
+
 from avilla.core.context import Context
 from avilla.core.event import MetadataModified, ModifyDetail
 from avilla.core.selector import Selector
-from avilla.core.ryanvk.descriptor.event import EventParse
+from avilla.red.capability import RedCapability
 from avilla.red.collector.connection import ConnectionCollector
 from avilla.standard.core.privilege import MuteInfo
-from loguru import logger
 
 
 class RedEventGroupMemberPerform((m := ConnectionCollector())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::event"
+    m.identify = "member"
+
 
-    @EventParse.collect(m, "group::member::mute")
-    async def group_name_change(self, raw_event: dict):
+    @m.entity(RedCapability.event_callback, event_type="group::member::mute")
+    async def group_name_change(self,  event_type: ..., raw_event: dict):
         account = self.connection.account
         if account is None:
             logger.warning(f"Unknown account received message {raw_event}")
             return
         group = Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
         group_data = raw_event["elements"][0]["grayTipElement"]["groupElement"]
         target = group.member(str(group_data["shutUp"]["member"]["uin"]))
@@ -34,27 +37,29 @@
         if group_data["shutUp"]["duration"] == "0":
             return MetadataModified(
                 context,
                 target,
                 MuteInfo,
                 {
                     MuteInfo.inh(lambda x: x.muted): ModifyDetail("update", False, True),
-                    MuteInfo.inh(lambda x: x.duration): ModifyDetail("clear",  timedelta(seconds=0)),
+                    MuteInfo.inh(lambda x: x.duration): ModifyDetail("clear", timedelta(seconds=0)),
                 },
                 operator=operator,
                 scene=group,
             )
         else:
             return MetadataModified(
                 context,
                 target,
                 MuteInfo,
                 {
                     MuteInfo.inh(lambda x: x.muted): ModifyDetail("update", True, False),
-                    MuteInfo.inh(lambda x: x.duration): ModifyDetail("set", timedelta(seconds=int(group_data["shutUp"]["duration"]))),
+                    MuteInfo.inh(lambda x: x.duration): ModifyDetail(
+                        "set", timedelta(seconds=int(group_data["shutUp"]["duration"]))
+                    ),
                 },
                 operator=operator,
                 scene=group,
             )
 
 
 _ = {
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/event/message.py` & `avilla_red-1.0.0a9/avilla/red/perform/event/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,85 +2,90 @@
 
 from datetime import datetime, timedelta
 
 from loguru import logger
 
 from avilla.core.context import Context
 from avilla.core.message import Message
-from avilla.core.ryanvk.descriptor.event import EventParse
 from avilla.core.selector import Selector
+from avilla.red.capability import RedCapability
 from avilla.red.collector.connection import ConnectionCollector
 from avilla.red.utils import pre_deserialize
-from avilla.standard.core.message import MessageReceived
+from avilla.standard.core.message import MessageReceived, MessageSent
 from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 
 
 class RedEventMessagePerform((m := ConnectionCollector())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::event"
+    m.identify = "message"
 
-    @EventParse.collect(m, "message::recv")
-    async def message(self, raw_event: dict):
+    @m.entity(RedCapability.event_callback, event_type="message::recv")
+    async def message(self,  event_type: ..., raw_event: dict):
         account = self.connection.account
         if account is None:
             logger.warning(f"Unknown account received message {raw_event}")
             return
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
+        reply = None
         if raw_event["chatType"] == 2:
-            group = Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
+            group = (
+                Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
+            )
             member = group.member(str(raw_event.get("senderUin", raw_event.get("senderUid"))))
             context = Context(
                 account,
                 member,
                 group,
                 group,
                 group.member(account.route["account"]),
             )
             elements = pre_deserialize(raw_event["elements"])
-            reply = None
             if elements[0]["type"] == "reply":
                 reply = group.message(f"{elements[0]['sourceMsgIdInRecords']}")
                 elements = elements[1:]
-            message = await account.staff.ext({"context": context}).deserialize_message(elements)
+            message = await RedCapability(account.staff.ext({"context": context})).deserialize(
+                elements
+            )
             msg = Message(
                 id=f'{raw_event["msgId"]}',
                 scene=group,
                 sender=member,
                 content=message,
                 time=datetime.fromtimestamp(int(raw_event["msgTime"])),
                 reply=reply,
             )
         else:
             friend = (
-                Selector()
-                .land(account.route["land"])
-                .friend(f"{raw_event.get('peerUin', raw_event.get('senderUin'))}")
+                Selector().land(account.route["land"]).friend(f"{raw_event.get('peerUin', raw_event.get('senderUin'))}")
             )
             context = Context(
                 account,
                 friend,
                 account.route,
                 friend,
                 account.route,
             )
             elements = pre_deserialize(raw_event["elements"])
-            reply = None
             if elements[0]["type"] == "reply":
                 reply = friend.message(f"{elements[0]['sourceMsgIdInRecords']}")
                 elements = elements[1:]
-            message = await account.staff.ext({"context": context}).deserialize_message(elements)
+            message = await RedCapability(account.staff.ext({"context": context})).deserialize(
+                elements
+            )
             msg = Message(
                 id=f'{raw_event["msgId"]}',
                 scene=friend,
                 sender=friend,
                 content=message,
                 time=datetime.fromtimestamp(int(raw_event["msgTime"])),
                 reply=reply,
             )
         await cache.set(f"red/account({account.route['account']}).message({msg.id})", raw_event, timedelta(minutes=5))
-        context._collect_metadatas(
-            msg.to_selector(),
-            msg
-        )
-        return MessageReceived(
+        context._collect_metadatas(msg.to_selector(), msg)
+        return MessageSent(
             context,
             msg,
+            account
+        ) if msg.sender.last_value == account.route["account"] else MessageReceived(
+            context,
+            msg
         )
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/event/relationship.py` & `avilla_red-1.0.0a9/avilla/red/perform/event/relationship.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
+from loguru import logger
+from selectolax.parser import HTMLParser
+
 from avilla.core.context import Context
 from avilla.core.event import RelationshipCreated
 from avilla.core.selector import Selector
-from avilla.core.ryanvk.descriptor.event import EventParse
+from avilla.red.capability import RedCapability
 from avilla.red.collector.connection import ConnectionCollector
-from loguru import logger
-from selectolax.parser import HTMLParser
 
 # async function adaptGuildMemberAddedMessage(
 #   session: Session,
 #   data: Message,
 # ): Promise<Session | undefined> {
 #   const session2 = await adaptChatMessage(session, data)
 #   session2.type = 'guild-member-added'
@@ -23,50 +24,39 @@
 #     nickname: data.elements[0]!.grayTipElement!.groupElement!.memberNick!,
 #   }
 #   session2.userId = session2.author.userId
 #
 #   return session2
 # }
 
+
 class RedEventRelationshipPerform((m := ConnectionCollector())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::event"
+    m.identify = "relationship"
 
-    @EventParse.collect(m, "group::member::add")
-    async def member_join(self, raw_event: dict):
+    @m.entity(RedCapability.event_callback, event_type="group::member::add")
+    async def member_join(self,  event_type: ..., raw_event: dict):
         account = self.connection.account
         if account is None:
             logger.warning(f"Unknown account received message {raw_event}")
             return
         group = Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
         group_data = raw_event["elements"][0]["grayTipElement"]["groupElement"]
         member = group.member(str(group_data["memberUin"]))
         operator = group.member(str(group_data["adminUin"]))
-        context = Context(
-            account,
-            member,
-            group,
-            group,
-            group.member(account.route["account"]),
-            mediums=[operator]
-        )
+        context = Context(account, member, group, group, group.member(account.route["account"]), mediums=[operator])
         return RelationshipCreated(context)
 
-    @EventParse.collect(m, "group::member::legacy::add::invited")
-    async def member_join(self, raw_event: dict):
+
+    @m.entity(RedCapability.event_callback, event_type="group::member::legacy::add::invited")
+    async def member_join_invited(self, event_type: ..., raw_event: dict):
         account = self.connection.account
         if account is None:
             logger.warning(f"Unknown account received message {raw_event}")
             return
         group = Selector().land(account.route["land"]).group(str(raw_event.get("peerUin", raw_event.get("peerUid"))))
         group_data = raw_event["elements"][0]["grayTipElement"]["xmlElement"]
         root = HTMLParser(group_data["content"])
-        operator = group.member(root.tags("qq")[0].attributes["jp"])
-        member = group.member(root.tags("qq")[1].attributes["jp"])
-        context = Context(
-            account,
-            member,
-            group,
-            group,
-            group.member(account.route["account"]),
-            mediums=[operator]
-        )
+        operator = group.member(root.tags("qq")[0].attributes["jp"])  # type: ignore
+        member = group.member(root.tags("qq")[1].attributes["jp"])  # type: ignore
+        context = Context(account, member, group, group, group.member(account.route["account"]), mediums=[operator])
         return RelationshipCreated(context)
```

### Comparing `avilla_red-1.0.0a7/avilla/red/perform/query.py` & `avilla_red-1.0.0a9/avilla/red/perform/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 
 from datetime import timedelta
 from typing import TYPE_CHECKING, Callable, cast
 
 from avilla.core.builtins.capability import CoreCapability
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.core.selector import Selector
-from graia.amnesia.builtins.memcache import MemcacheService, Memcache
+from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 
 if TYPE_CHECKING:
     from ..account import RedAccount  # noqa
     from ..protocol import RedProtocol  # noqa
 
 
 class RedQueryPerform((m := AccountCollector["RedProtocol", "RedAccount"]())._):
-    m.post_applying = True
+    m.namespace = "avilla.protocol/red::query"
 
-    @CoreCapability.query.collect(m, "land.group")
+    @m.entity(CoreCapability.query, target="land.group")
     async def query_group(self, predicate: Callable[[str, str], bool] | str, previous: None):
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         result = await self.account.websocket_client.call_http("get", "api/bot/groups", {})
         result = cast(list, result)
         for i in result:
             group_id = str(i["groupCode"])
-            await cache.set(
-                f"red/account({self.account.route['account']}).group({group_id})", i, timedelta(minutes=5)
-            )
+            await cache.set(f"red/account({self.account.route['account']}).group({group_id})", i, timedelta(minutes=5))
             if callable(predicate) and predicate("group", group_id) or group_id == predicate:
                 yield Selector().land(self.account.route["land"]).group(group_id)
 
-    @CoreCapability.query.collect(m, "land.friend")
+    @m.entity(CoreCapability.query, target="land.friend")
     async def query_friend(self, predicate: Callable[[str, str], bool] | str, previous: None):
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         result = await self.account.websocket_client.call_http("get", "api/bot/friends", {})
         result = cast(list, result)
         for i in result:
             friend_id = str(i["uin"])
             await cache.set(
                 f"red/account({self.account.route['account']}).friend({friend_id})", i, timedelta(minutes=5)
             )
             if callable(predicate) and predicate("friend", friend_id) or friend_id == predicate:
                 yield Selector().land(self.account.route["land"]).friend(friend_id)
 
-    @CoreCapability.query.collect(m, "member", "land.group")
+    @m.entity(CoreCapability.query, target="member", previous="land.group")  # type: ignore
     async def query_group_members(self, predicate: Callable[[str, str], bool] | str, previous: Selector):
         cache: Memcache = self.protocol.avilla.launch_manager.get_component(MemcacheService).cache
         result = await self.account.websocket_client.call_http(
             "post", "api/group/getMemberList", {"group": int(previous["group"])}
         )
         result = cast(list, result)
         for i in result:
             member_id = str(i["uin"])
             await cache.set(
-                f"red/account({self.account.route['account']}).group({previous['group']}).member({member_id})", i, timedelta(minutes=5)
+                f"red/account({self.account.route['account']}).group({previous['group']}).member({member_id})",
+                i,
+                timedelta(minutes=5),
             )
             if callable(predicate) and predicate("member", member_id) or member_id == predicate:
                 yield previous.member(member_id)
```

### Comparing `avilla_red-1.0.0a7/avilla/red/resource.py` & `avilla_red-1.0.0a9/avilla/red/resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 from __future__ import annotations
 
 from pathlib import Path
 
+from avilla.core.context import Context
 from avilla.core.resource import Resource
 from avilla.core.selector import Selector
 
 
 class RedResource(Resource[bytes]):
     id: str
+    ctx: Context
     size: int
     name: str
     elem: str
     uuid: str
 
-    def __init__(self, selector: Selector, id: str, size: int, name: str, elem: str, uuid: str):
+    def __init__(self, ctx: Context, selector: Selector, id: str, size: int, name: str, elem: str, uuid: str):
         super().__init__(selector)
+        self.ctx = ctx
         self.id = id
         self.size = size
         self.name = name
         self.elem = elem
         self.uuid = uuid
 
 
 class RedFileResource(RedResource):
     pass
 
 
 class RedImageResource(RedResource):
     def __init__(
         self,
+        ctx: Context,
         selector: Selector,
         id: str,
         size: int,
         name: str,
         elem: str,
         uuid: str,
         path: str | Path,
         width: int,
         height: int,
     ):
-        super().__init__(selector, id, size, name, elem, uuid)
+        super().__init__(ctx, selector, id, size, name, elem, uuid)
         self.path = Path(path)
         self.width = width
         self.height = height
 
     @property
     def url(self) -> str:
+        if self.ctx.scene.last_key == "friend":
+            return f"https://c2cpicdw.qpic.cn/offpic_new//{self.ctx.scene.last_value}-0-{self.id.upper()}/0"
         return f"https://gchat.qpic.cn/gchatpic_new/0/0-0-{self.id.upper()}/0"
 
 
 class RedVoiceResource(RedResource):
     def __init__(
         self,
+        ctx: Context,
         selector: Selector,
         id: str,
         size: int,
         name: str,
         elem: str,
         uuid: str,
         path: str | Path,
     ):
-        super().__init__(selector, id, size, name, elem, uuid)
+        super().__init__(ctx, selector, id, size, name, elem, uuid)
         self.path = Path(path)
 
 
-
 class RedVideoResource(RedResource):
     def __init__(
         self,
+        ctx: Context,
         selector: Selector,
         id: str,
         size: int,
         name: str,
         elem: str,
         uuid: str,
         path: str | Path,
     ):
-        super().__init__(selector, id, size, name, elem, uuid)
+        super().__init__(ctx, selector, id, size, name, elem, uuid)
         self.path = Path(path)
```

### Comparing `avilla_red-1.0.0a7/avilla/red/service.py` & `avilla_red-1.0.0a9/avilla/red/service.py`

 * *Files identical despite different names*

### Comparing `avilla_red-1.0.0a7/avilla/red/utils.py` & `avilla_red-1.0.0a9/avilla/red/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-from enum import IntEnum
-from typing import TypedDict, Literal
 from dataclasses import dataclass
+from enum import IntEnum
+from typing import Literal, TypedDict
+
 
 class MsgType(IntEnum):
     normal = 2
     may_file = 3
     system = 5
     voice = 6
     video = 7
     value8 = 8
     reply = 9
     wallet = 10
     ark = 11
     may_market = 17
 
+
 class SubMsgTypes(TypedDict):
     text: bool
     image: bool
     face: bool
     link: bool
     forward: bool
     reply: bool
     market_face: bool
     file: bool
 
+
 @dataclass
 class MsgTypes:
     chat: Literal["friend", "group"]
     msg: MsgType
     sub: SubMsgTypes
     send: Literal["system", "normal"]
 
     @property
     def group(self):
         return self.chat == "group"
 
+
 def pre_deserialize(elements: list[dict]):
     res = []
     for elem in elements:
         slot = {}
         data = {k: v for k, v in elem.items() if v is not None}
         for k, v in data.items():
             if k.endswith("Element"):
                 slot["type"] = k[:-7]
                 slot.update(v)
             elif k != "elementType":
                 slot[k] = v
         res.append(slot)
     return res
 
+
 def get_msg_types(raw_event: dict) -> MsgTypes:
-    return MsgTypes(**{
-        "chat": "friend" if raw_event["chatType"] == 1 else "group",
-        "msg": MsgType(raw_event["msgType"]),
-        "sub": {
-            "text": bool(raw_event["subMsgType"] & (1 << 0)),
-            "image": bool(raw_event["subMsgType"] & (1 << 1)),
-            "face": bool(raw_event["subMsgType"] & (1 << 4)),
-            "link": bool(raw_event["subMsgType"] & (1 << 7)),
-            "forward": bool(raw_event["subMsgType"] & (1 << 3)),
-            "reply": (
-                raw_event["msgType"] == 9 and bool(raw_event["subMsgType"] & (1 << 5))
-            ),
-            "market_face": (
-                raw_event["msgType"] == 17 and bool(raw_event["subMsgType"] & (1 << 3))
-            ),
-            "file": (
-                raw_event["msgType"] == 3 and bool(raw_event["subMsgType"] & (1 << 9))
-            )
-        },
-        "send": "system" if raw_event["sendType"] == 3 else "normal",
-    })
+    return MsgTypes(
+        **{
+            "chat": "friend" if raw_event["chatType"] == 1 else "group",
+            "msg": MsgType(raw_event["msgType"]),
+            "sub": {
+                "text": bool(raw_event["subMsgType"] & (1 << 0)),
+                "image": bool(raw_event["subMsgType"] & (1 << 1)),
+                "face": bool(raw_event["subMsgType"] & (1 << 4)),
+                "link": bool(raw_event["subMsgType"] & (1 << 7)),
+                "forward": bool(raw_event["subMsgType"] & (1 << 3)),
+                "reply": (raw_event["msgType"] == 9 and bool(raw_event["subMsgType"] & (1 << 5))),
+                "market_face": (raw_event["msgType"] == 17 and bool(raw_event["subMsgType"] & (1 << 3))),
+                "file": (raw_event["msgType"] == 3 and bool(raw_event["subMsgType"] & (1 << 9))),
+            },
+            "send": "system" if raw_event["sendType"] == 3 else "normal",
+        }
+    )
+
 
 """\
 1 ===> text, at, ...
     content
     atType {0: not At, 1: everyone, 2: someone (atNtUid, atNtUin)}
 2 ===> image(pic)
     fileName
```

### Comparing `avilla_red-1.0.0a7/pyproject.toml` & `avilla_red-1.0.0a9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avilla-red"
-version = "1.0.0-alpha.7"
+version = "1.0.0a9"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.1",
     "selectolax>=0.3.16",
 ]
```

### Comparing `avilla_red-1.0.0a7/PKG-INFO` & `avilla_red-1.0.0a9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avilla-red
-Version: 1.0.0a7
+Version: 1.0.0a9
 Home-page: https://github.com/GraiaProject/Avilla
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/GraiaProject/Avilla
 Project-URL: Repository, https://github.com/GraiaProject/Avilla
 Requires-Python: >=3.9
 Requires-Dist: aiohttp>=3.8.1
@@ -72,14 +72,15 @@
 |:--------------------------------------------:|:----------------:|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------------------------:|:--------:|:------:|
 |             [Core](avilla/core)              |        -         |           -            |  **Alpha**  |            [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)            | Official |  MIT   |
 |          [Console](avilla/console)           |       终端环境       |       `Console`        |  **Alpha**  |         [![image](https://img.shields.io/pypi/v/avilla-console)](https://pypi.org/project/avilla-console)         | Official |  MIT   |
 |        [Elizabeth](avilla/elizabeth)         |    Tencent QQ    |    `mirai-api-http`    |  **Alpha**  |       [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)       | Official | AGPLv3 |
 |        [Onebot 11](avilla/onebot/v11)        |     *多平台支持*      |      `OneBot v11`      |   **WIP**   |      [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11)      | Official |   -    |
 | [QQ Guild (Tencent)](avilla/qqguild/tencent) | Tencent QQ Guild | `QQGuild Official API` |   **WIP**   | [![image](https://img.shields.io/pypi/v/avilla-qqguild-tencent)](https://pypi.org/project/avilla-qqguild-tencent) | Official |  MIT   |
 |              [Red](avilla/red)               |   Tencent QQNT   |     `Red Protocol`     |   **WIP**   |             [![image](https://img.shields.io/pypi/v/avilla-red)](https://pypi.org/project/avilla-red)             | Official |  MIT   |
+|           [Satori](avilla/satori)            |     *多平台支持*      | `Satori Protocol (v1)` |   **WIP**   |          [![image](https://img.shields.io/pypi/v/avilla-satori)](https://pypi.org/project/avilla-satori)          | Official |  MIT   |
 |         [Telegram](avilla/telegram)          |     Telegram     |       `Telegram`       |  **Draft**  |        [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)        |    -     |   -    |
 |        [Nightcord](avilla/nightcord)         |     Discord      |     `Discord Bots`     |  **Draft**  |       [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)       |    -     |   -    |
 |             [Kook](avilla/kook)              |       Kook       |         `Kook`         |  **Draft**  |            [![image](https://img.shields.io/pypi/v/avilla-kook)](https://pypi.org/project/avilla-kook)            |    -     |   -    |
 |        [OneBot 12](avilla/onebot/v12)        |     *多平台支持*      |      `OneBot v12`      | **Planned** |                                                         -                                                         |    -     |   -    |
 
 ## 我们的愿景
```

