# Comparing `tmp/telegram_wallet_pay-0.2.0.tar.gz` & `tmp/telegram_wallet_pay-0.2.1.tar.gz`

## Comparing `telegram_wallet_pay-0.2.0.tar` & `telegram_wallet_pay-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.editorconfig
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/codecov.yaml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/examples/00_get_started.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_schemas.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.gitignore
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/README.md
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/.editorconfig
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/codecov.yaml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/examples/00_get_started.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/tests/test_client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/tests/test_schemas.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/README.md
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.1/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.2.0/.pre-commit-config.yaml` & `telegram_wallet_pay-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/examples/00_get_started.py` & `telegram_wallet_pay-0.2.1/examples/00_get_started.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Mapping,
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
+import certifi
 from aiohttp import ClientResponse, ClientSession, TCPConnector
 from pydantic import BaseModel
 
 from telegram_wallet_pay.errors import (
     InvalidAPIKeyError,
     InvalidRequestError,
     NotFountError,
@@ -149,17 +150,16 @@
         # Wait 250 ms for the underlying SSL connections to close
         # https://docs.aiohttp.org/en/stable/client_advanced.html#graceful-shutdown
         await asyncio.sleep(0.25)
 
     async def _get_session(self) -> ClientSession:
         """Get aiohttp session with cache."""
         if self._session is None or self._session.closed:
-            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-            ssl_context.load_default_certs()
-            connector = TCPConnector(ssl_context=ssl_context)
+            ssl_context = ssl.create_default_context(cafile=certifi.where())
+            connector = TCPConnector(ssl=ssl_context)
             self._session = ClientSession(
                 base_url=self._base_url,
                 connector=connector,
                 headers=self._headers,
             )
 
         return self._session
```

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.2.1/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/tests/test_client.py` & `telegram_wallet_pay-0.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/tests/test_schemas.py` & `telegram_wallet_pay-0.2.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/tests/test_signature.py` & `telegram_wallet_pay-0.2.1/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/.gitignore` & `telegram_wallet_pay-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/README.md` & `telegram_wallet_pay-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.2.0/pyproject.toml` & `telegram_wallet_pay-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "aiohttp>=3.8.5,<3.10",
     "pydantic>=2.4,<3",
+    "certifi>=2023",
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff>=0",
     "mypy>=1",
     "pre-commit>=3",
```

### Comparing `telegram_wallet_pay-0.2.0/PKG-INFO` & `telegram_wallet_pay-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.2.0
+Version: 0.2.1
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: aiohttp<3.10,>=3.8.5
+Requires-Dist: certifi>=2023
 Requires-Dist: pydantic<3,>=2.4
 Provides-Extra: dev
 Requires-Dist: mypy>=1; extra == 'dev'
 Requires-Dist: pre-commit>=3; extra == 'dev'
 Requires-Dist: ruff>=0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: aresponses==3.0.0; extra == 'test'
```

