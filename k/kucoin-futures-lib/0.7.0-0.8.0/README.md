# Comparing `tmp/kucoin_futures_lib-0.7.0.tar.gz` & `tmp/kucoin_futures_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.7.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.8.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.7.0.tar` & `kucoin_futures_lib-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0     1760 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/README.md
--rw-r--r--   0        0        0      719 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      415 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     2695 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     1440 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/fill.py
--rw-r--r--   0        0        0     2769 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     3660 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/trailing.py
--rw-r--r--   0        0        0     1813 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    17231 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     3521 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      598 2024-04-11 02:46:38.347644 kucoin_futures_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1760 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      424 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     2695 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2044 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/message.py
+-rw-r--r--   0        0        0     2769 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     3611 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/trailing.py
+-rw-r--r--   0        0        0     1813 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    17231 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     3879 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      598 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.8.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.7.0/LICENSE` & `kucoin_futures_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/README.md` & `kucoin_futures_lib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/handlers/trailing.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/trailing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Trailing stop loss handler."""
 
 import asyncio
 import logging
 from typing import Dict, Callable, Any, Awaitable, Literal
 
-from kucoin_futures_lib.handlers import OcoHandler
 from kucoin_futures_lib.handlers.base import HandlerABC
 
 logger = logging.getLogger(__name__)
 
 
 class TrailingHandler(HandlerABC):
     """Handler that moves the stop loss price based on the trailing stop loss strategy."""
@@ -17,15 +16,15 @@
         self,
         instrument: str,
         direction: Literal["buy", "sell"],
         sl_order_id: str,
         sl_order_price: float,
         trailing_distance: float,
         trailing_step: float,
-        oco_handler: OcoHandler,
+        handler: HandlerABC,
         update_order: Callable[[Any], Awaitable[None]],
     ):
         """Initialize the handler.
         :param instrument: instrument symbol
         :param direction: buy or sell
         :param sl_order_id: Stop loss order ID
         :param sl_order_price: Stop loss order stop price
@@ -38,15 +37,15 @@
         self.instrument = instrument
         self.direction = direction
         self.sl_order_id = sl_order_id
         self.sl_order_price = sl_order_price
         self.trailing_distance = trailing_distance
         self.trailing_step = trailing_step
         self.update_order = update_order
-        self.oco_handler = oco_handler
+        self.external_handler = handler
         self._done = asyncio.Event()
         self._topic = "/contract/instrument"
 
     def __repr__(self):
         return f"TrailingHandler({self.instrument}, sl_order_id={self.sl_order_id}, trailing_distance={self.trailing_distance}, trailing_step={self.trailing_step})"
 
     @property
@@ -78,15 +77,15 @@
                 else self.sl_order_price - adjustment
             )
 
     async def handle(self, msg: Dict):
         if self._done.is_set():
             return
 
-        if self.oco_handler.done.is_set():
+        if self.external_handler.done.is_set():
             self._done.set()
             return
 
         if msg["subject"] == "mark.index.price":
             mark_price = msg["data"]["markPrice"]
             new_price = self.calculate_new_price(mark_price)
             if new_price:
```

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.7.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.8.0/kucoin_futures_lib/websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Kucoin Futures WebSocket module."""
 
 import asyncio
 import logging
-from typing import Union, Callable, Awaitable, Optional
+from typing import Union, Callable, Awaitable, Optional, Literal, List
 
 from kucoin_futures.client import WsToken
 from kucoin_futures.ws_client import KucoinFuturesWsClient
 
-from kucoin_futures_lib.handlers import OcoHandler, EntryRangeHandler, FillHandler, HandlerABC
+from kucoin_futures_lib.handlers import OcoHandler, EntryRangeHandler, MessageHandler, HandlerABC
 
 logger = logging.getLogger(__name__)
 
 
 class KucoinFuturesWebsocket:
     """Kucoin Futures user wrapper class."""
 
@@ -20,16 +20,15 @@
 
     async def subscribe(
         self, handler: HandlerABC, timeout: Optional[float] = 60 * 60 * 12
     ) -> None:
         """Subscribe to the WebSocket topic.
         :param handler: Handler object
         :param timeout: Timeout in seconds. Default is 12 hours
-        :raises asyncio.TimeoutError: If the timeout is reached
-        """
+        :raises asyncio.TimeoutError: If the timeout is reached"""
         ws_client = await KucoinFuturesWsClient.create(
             loop=None,
             client=self.token,
             callback=handler.handle,
             private=handler.private,
         )
         await ws_client.subscribe(handler.topic)
@@ -84,18 +83,25 @@
             market_order_id=sl_order_id,
             instrument=instrument,
             cancel_order=cancel_order,
         )
         await self.subscribe(handler, None)
 
 
-    async def listen_for_fill(
+    async def listen_for_message(
         self,
         order_id: str,
+        message_type: List[Literal["open", "match", "filled", "canceled", "update"]],
         timeout: float = 60 * 60 * 12,
-    ) -> None:
-        """Listen for the order to be filled.
+    ) -> Literal["open", "match", "filled", "canceled", "update"]:
+        """Listen for the order message.
         :param order_id: Order ID
-        :param timeout: timeout in seconds. Default is 12 hours
+        :param message_type: The message types to listen for.
+        :param timeout: timeout in seconds. Default is 12 hours.
+        :return: The message type received.
         """
-        handler = FillHandler(order_id=order_id)
-        await self.subscribe(handler, timeout)
+        handler = MessageHandler(
+            order_id=order_id,
+            message_type=message_type,
+        )
+        await self.subscribe(handler, timeout)
+        return handler.received_message
```

### Comparing `kucoin_futures_lib-0.7.0/pyproject.toml` & `kucoin_futures_lib-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kucoin-futures-lib"
-version = "0.7.0"
+version = "0.8.0"
 description = "Kucoin Futures wrapper library"
 authors = ["Evgeny Aleshin"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `kucoin_futures_lib-0.7.0/PKG-INFO` & `kucoin_futures_lib-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

