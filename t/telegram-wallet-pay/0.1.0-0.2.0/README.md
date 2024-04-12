# Comparing `tmp/telegram_wallet_pay-0.1.0.tar.gz` & `tmp/telegram_wallet_pay-0.2.0.tar.gz`

## Comparing `telegram_wallet_pay-0.1.0.tar` & `telegram_wallet_pay-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/.editorconfig
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/codecov.yaml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/examples/00_get_started.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_amount_result.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_new.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_reconciliation_result.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_result.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/update.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/tests/test_client.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/tests/test_schemas.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/.gitignore
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/README.md
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/codecov.yaml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/examples/00_get_started.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/README.md
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.2.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.1.0/.pre-commit-config.yaml` & `telegram_wallet_pay-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,83 @@
 import asyncio
-import logging
 import ssl
 from contextlib import asynccontextmanager
 from decimal import Decimal
-from typing import Any, AsyncIterator, Dict, Literal, Mapping, Optional, Union
+from http import HTTPStatus
+from typing import (
+    Any,
+    AsyncIterator,
+    Dict,
+    Literal,
+    Mapping,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from aiohttp import ClientResponse, ClientSession, TCPConnector
+from pydantic import BaseModel
 
-from telegram_wallet_pay import schemas
+from telegram_wallet_pay.errors import (
+    InvalidAPIKeyError,
+    InvalidRequestError,
+    NotFountError,
+    RequestLimitReachedError,
+    TelegramWalletPayError,
+    UnexpectedError,
+)
+from telegram_wallet_pay.schemas import (
+    CreateOrderRequest,
+    CreateOrderResponse,
+    GetOrderPreviewResponse,
+    GetOrderReconciliationListResponse,
+    MoneyAmount,
+    OrderAmountResponse,
+)
+
+T = TypeVar("T", bound=BaseModel)
 
 AUTH_HEADER = "Wpay-Store-Api-Key"
 DEFAULT_API_HOST = "https://pay.wallet.tg"
 
+EXCEPTIONS_MAPPING: Dict[Union[HTTPStatus, int], Type[TelegramWalletPayError]] = {
+    HTTPStatus.BAD_REQUEST: InvalidRequestError,
+    HTTPStatus.UNAUTHORIZED: InvalidAPIKeyError,
+    HTTPStatus.NOT_FOUND: NotFountError,
+    HTTPStatus.TOO_MANY_REQUESTS: RequestLimitReachedError,
+    HTTPStatus.INTERNAL_SERVER_ERROR: UnexpectedError,
+}
+
 
 class TelegramWalletPay:
     """Telegram Wallet API client."""
 
+    def __init__(self, token: str, api_host: str = DEFAULT_API_HOST) -> None:
+        self._base_url = api_host
+        self._session: Optional[ClientSession] = None
+        self._headers = {AUTH_HEADER: token}
+
     async def create_order(  # noqa: PLR0913
         self,
+        *,
         amount: Union[str, Decimal, float],
         currency_code: Literal["TON", "BTC", "USDT", "EUR", "USD", "RUB"],
         description: str,
         external_id: str,
         timeout_seconds: int,
         customer_telegram_user_id: int,
         auto_conversion_currency: Optional[Literal["TON", "BTC", "USDT"]] = None,
         return_url: Optional[str] = None,
         fail_return_url: Optional[str] = None,
         custom_data: Optional[str] = None,
-    ) -> schemas.OrderResult:
+    ) -> CreateOrderResponse:
         """Create an order."""
-        order_new = schemas.OrderNew(
-            amount=schemas.MoneyAmount(
+        create_order_request = CreateOrderRequest(
+            amount=MoneyAmount(
                 amount=str(amount),
                 currency_code=currency_code,
             ),
             auto_conversion_currency=auto_conversion_currency,
             description=description,
             return_url=return_url,
             fail_return_url=fail_return_url,
@@ -44,75 +86,73 @@
             timeout_seconds=timeout_seconds,
             customer_telegram_user_id=customer_telegram_user_id,
         )
 
         async with self._make_request(
             method="POST",
             url="/wpay/store-api/v1/order",
-            json=order_new.model_dump(by_alias=True),
-        ) as response:  # type: ClientResponse
-            json_data = await response.text()
-            self.log.info("Received answer: %s", json_data)
-
-        return schemas.OrderResult.model_validate_json(json_data)
+            json=create_order_request.model_dump(by_alias=True),
+        ) as response:
+            return await self._prepare_result(response, CreateOrderResponse)
 
-    async def get_preview(self, order_id: str) -> schemas.OrderResult:
+    async def get_preview(self, order_id: str) -> GetOrderPreviewResponse:
         """Retrieve the order information."""
         async with self._make_request(
             method="GET",
             url="/wpay/store-api/v1/order/preview",
             params={"id": order_id},
-        ) as response:  # type: ClientResponse
-            json_data = await response.text()
-
-        return schemas.OrderResult.model_validate_json(json_data)
+        ) as response:
+            return await self._prepare_result(response, GetOrderPreviewResponse)
 
     async def get_order_list(
         self,
         *,
         offset: int,
         count: int,
-    ) -> schemas.OrderReconciliationResult:
+    ) -> GetOrderReconciliationListResponse:
         """Get list of store orders.
 
         Items sorted by creation time in ascending order.
         """
         query_params: Dict[str, Any] = {
             "offset": offset,
             "count": count,
         }
 
         async with self._make_request(
             method="GET",
             url="/wpay/store-api/v1/reconciliation/order-list",
             params=query_params,
-        ) as response:  # type: ClientResponse
-            json_data = await response.text()
-
-        return schemas.OrderReconciliationResult.model_validate_json(json_data)
+        ) as response:
+            return await self._prepare_result(
+                response,
+                GetOrderReconciliationListResponse,
+            )
 
-    async def get_order_amount(self) -> schemas.OrderAmountResult:
+    async def get_order_amount(self) -> OrderAmountResponse:
         """Get total count of all created orders in the Store.
 
         Including all - paid and unpaid.
         """
         async with self._make_request(
             method="GET",
             url="/wpay/store-api/v1/reconciliation/order-amount",
-        ) as response:  # type: ClientResponse
-            json_data = await response.text()
+        ) as response:
+            return await self._prepare_result(response, OrderAmountResponse)
 
-        return schemas.OrderAmountResult.model_validate_json(json_data)
+    async def close(self) -> None:
+        """Graceful session close."""
+        if not self._session:
+            return
 
-    def __init__(self, token: str, api_host: str = DEFAULT_API_HOST) -> None:
-        self.log = logging.getLogger(self.__class__.__name__)
+        await self._session.close()
 
-        self._base_url = api_host
-        self._session: Optional[ClientSession] = None
-        self._headers = {AUTH_HEADER: token}
+        # Wait 250 ms for the underlying SSL connections to close
+        # https://docs.aiohttp.org/en/stable/client_advanced.html#graceful-shutdown
+        await asyncio.sleep(0.25)
 
     async def _get_session(self) -> ClientSession:
         """Get aiohttp session with cache."""
         if self._session is None or self._session.closed:
             ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
             ssl_context.load_default_certs()
             connector = TCPConnector(ssl_context=ssl_context)
@@ -130,30 +170,21 @@
         method: str,
         url: str,
         params: Optional[Mapping[str, str]] = None,
         json: Optional[Mapping[str, str]] = None,
     ) -> AsyncIterator[ClientResponse]:
         """Make request and return decoded json response."""
         session = await self._get_session()
-
-        self.log.debug(
-            "Making request %r %r with json %r and params %r",
-            method,
-            url,
-            json,
-            params,
-        )
         async with session.request(method, url, params=params, json=json) as response:
             yield response
 
-    async def close(self) -> None:
-        """Graceful session close."""
-        if not self._session:
-            self.log.debug("There's not session to close.")
-            return
+    @staticmethod
+    async def _prepare_result(response: ClientResponse, schema: Type[T]) -> T:
+        """Process error response."""
+        status = response.status
+        body = await response.text()
 
-        await self._session.close()
-        self.log.debug("Session successfully closed.")
+        if status == HTTPStatus.OK:
+            return schema.model_validate_json(body)
 
-        # Wait 250 ms for the underlying SSL connections to close
-        # https://docs.aiohttp.org/en/stable/client_advanced.html#graceful-shutdown
-        await asyncio.sleep(0.25)
+        exc_type = EXCEPTIONS_MAPPING.get(status, TelegramWalletPayError)
+        raise exc_type(body)
```

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_new.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pydantic import Field
 
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
 
 
-class OrderNew(DefaultModel):
+class CreateOrderRequest(DefaultModel):
     amount: MoneyAmount
     auto_conversion_currency: Optional[Literal["TON", "BTC", "USDT"]] = None
     description: str = Field(min_length=5, max_length=100)
     return_url: Optional[str] = Field(None, max_length=255)
     fail_return_url: Optional[str] = Field(None, max_length=255)
     custom_data: Optional[str] = Field(None, max_length=255)
     external_id: str = Field(max_length=255)
```

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/update.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from pydantic import Field
 
 from ._default import DefaultModel, DefaultRootModel
 from .webhook_payload import WebhookPayload
 
 
-class Update(DefaultModel):
+class WebhookMessage(DefaultModel):
     event_datetime: datetime = Field(alias="eventDateTime")
     event_id: int
     type: Literal["ORDER_FAILED", "ORDER_PAID"]
     payload: WebhookPayload
 
 
-class Updates(DefaultRootModel):
-    root: List[Update]
+class WebhookMessages(DefaultRootModel):
+    root: List[WebhookMessage]
 
-    def __iter__(self) -> Iterator[Update]:  # type: ignore[override]
+    def __iter__(self) -> Iterator[WebhookMessage]:  # type: ignore[override]
         """Iterate over root model."""
         return iter(self.root)
```

### Comparing `telegram_wallet_pay-0.1.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.2.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/tests/test_client.py` & `telegram_wallet_pay-0.2.0/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,66 @@
+import json
 from datetime import datetime
 from typing import AsyncIterator
 
 import pytest
 from aresponses import ResponsesMockServer
 from telegram_wallet_pay import TelegramWalletPay
+from telegram_wallet_pay.errors import InvalidAPIKeyError
 from telegram_wallet_pay.schemas import (
+    CreateOrderResponse,
+    GetOrderPreviewResponse,
+    GetOrderReconciliationListResponse,
     MoneyAmount,
     OrderAmount,
-    OrderAmountResult,
+    OrderAmountResponse,
     OrderPreview,
     OrderReconciliationItem,
     OrderReconciliationList,
-    OrderReconciliationResult,
-    OrderResult,
 )
 
-SUCCESS_ORDER_PREVIEW = OrderPreview(
+ORDER_PREVIEW = OrderPreview(
     id="",
     status="ACTIVE",
     number="",
     amount=MoneyAmount(currency_code="RUB", amount="42.0"),
     created_datetime=datetime.now(),
     expiration_datetime=datetime.now(),
     pay_link="",
     direct_pay_link="",
 )
 
-SUCCESS_RESPONSE = OrderResult(
+CREATE_ORDER_RESPONSE = CreateOrderResponse(
     status="SUCCESS",
     message="",
-    data=SUCCESS_ORDER_PREVIEW,
+    data=ORDER_PREVIEW,
+)
+
+GET_ORDER_PREVIEW_RESPONSE = GetOrderPreviewResponse(
+    status="SUCCESS",
+    message="",
+    data=ORDER_PREVIEW,
 )
 
 ORDER_RECONCILIATION_ITEM = OrderReconciliationItem(
     id=42,
     status="EXPIRED",
     amount=MoneyAmount(currency_code="RUB", amount="42.0"),
     external_id="",
     created_datetime=datetime.now(),
     expiration_datetime=datetime.now(),
 )
 
-SUCCESS_GET_ORDERS_LIST_REQUEST = OrderReconciliationResult(
+GET_ORDERS_LIST_RESPONSE = GetOrderReconciliationListResponse(
     status="SUCCESS",
     message=None,
     data=OrderReconciliationList(items=[]),
 )
 
-SUCCESS_ORDER_AMOUNT_RESULT = OrderAmountResult(
+ORDER_AMOUNT_RESPONSE = OrderAmountResponse(
     status="SUCCESS",
     message="",
     data=OrderAmount(total_amount=42),
 )
 
 
 @pytest.fixture()
@@ -72,28 +81,28 @@
         aresponses: ResponsesMockServer,
     ) -> None:
         """Test successful Order creation."""
         aresponses.add(
             path_pattern=self.URI,
             method_pattern=self.METHOD,
             response=aresponses.Response(
-                text=SUCCESS_RESPONSE.model_dump_json(by_alias=True),
+                text=CREATE_ORDER_RESPONSE.model_dump_json(by_alias=True),
                 content_type="application/json",
                 status=200,
             ),
         )
-        result = await wallet.create_order(
-            amount=SUCCESS_ORDER_PREVIEW.amount.amount,
-            currency_code=SUCCESS_ORDER_PREVIEW.amount.currency_code,
+        response = await wallet.create_order(
+            amount=ORDER_PREVIEW.amount.amount,
+            currency_code=ORDER_PREVIEW.amount.currency_code,
             description="description",
             external_id="",
             timeout_seconds=30,
             customer_telegram_user_id=42,
         )
-        assert result == SUCCESS_RESPONSE
+        assert response == CREATE_ORDER_RESPONSE
         aresponses.assert_plan_strictly_followed()
 
 
 class TestGetPreview:
     METHOD = "GET"
     URI = "/wpay/store-api/v1/order/preview"
 
@@ -103,21 +112,41 @@
         aresponses: ResponsesMockServer,
     ) -> None:
         """Test successful getting Order preview."""
         aresponses.add(
             path_pattern=self.URI,
             method_pattern=self.METHOD,
             response=aresponses.Response(
-                text=SUCCESS_RESPONSE.model_dump_json(by_alias=True),
+                text=GET_ORDER_PREVIEW_RESPONSE.model_dump_json(by_alias=True),
                 content_type="application/json",
                 status=200,
             ),
         )
-        result = await wallet.get_preview(SUCCESS_ORDER_PREVIEW.id)
-        assert result == SUCCESS_RESPONSE
+        response = await wallet.get_preview(ORDER_PREVIEW.id)
+        assert response == GET_ORDER_PREVIEW_RESPONSE
+        aresponses.assert_plan_strictly_followed()
+
+    async def test_invalid_token(
+        self,
+        wallet: TelegramWalletPay,
+        aresponses: ResponsesMockServer,
+    ) -> None:
+        """Test successful getting Order preview."""
+        aresponses.add(
+            path_pattern=self.URI,
+            method_pattern=self.METHOD,
+            response=aresponses.Response(
+                text=json.dumps({"success": False, "error": "Invalid token"}),
+                content_type="application/json",
+                status=401,
+            ),
+        )
+        with pytest.raises(InvalidAPIKeyError):
+            await wallet.get_preview(ORDER_PREVIEW.id)
+
         aresponses.assert_plan_strictly_followed()
 
 
 class TestGetOrderList:
     METHOD = "GET"
     URI = "/wpay/store-api/v1/reconciliation/order-list"
 
@@ -127,21 +156,21 @@
         aresponses: ResponsesMockServer,
     ) -> None:
         """Test successful getting Order preview."""
         aresponses.add(
             path_pattern=self.URI,
             method_pattern=self.METHOD,
             response=aresponses.Response(
-                text=SUCCESS_GET_ORDERS_LIST_REQUEST.model_dump_json(by_alias=True),
+                text=GET_ORDERS_LIST_RESPONSE.model_dump_json(by_alias=True),
                 content_type="application/json",
                 status=200,
             ),
         )
-        result = await wallet.get_order_list(offset=0, count=10)
-        assert result == SUCCESS_GET_ORDERS_LIST_REQUEST
+        response = await wallet.get_order_list(offset=0, count=10)
+        assert response == GET_ORDERS_LIST_RESPONSE
         aresponses.assert_plan_strictly_followed()
 
 
 class TestGetOrderAmount:
     METHOD = "GET"
     URI = "/wpay/store-api/v1/reconciliation/order-amount"
 
@@ -151,20 +180,20 @@
         aresponses: ResponsesMockServer,
     ) -> None:
         """Test successful getting Order preview."""
         aresponses.add(
             path_pattern=self.URI,
             method_pattern=self.METHOD,
             response=aresponses.Response(
-                text=SUCCESS_ORDER_AMOUNT_RESULT.model_dump_json(by_alias=True),
+                text=ORDER_AMOUNT_RESPONSE.model_dump_json(by_alias=True),
                 content_type="application/json",
                 status=200,
             ),
         )
-        result = await wallet.get_order_amount()
-        assert result == SUCCESS_ORDER_AMOUNT_RESULT
+        response = await wallet.get_order_amount()
+        assert response == ORDER_AMOUNT_RESPONSE
         aresponses.assert_plan_strictly_followed()
 
 
 class TestSession:
     async def test_close_without_session(self, wallet: TelegramWalletPay) -> None:
         """Test session close without any request."""
```

### Comparing `telegram_wallet_pay-0.1.0/tests/test_schemas.py` & `telegram_wallet_pay-0.2.0/tests/test_schemas.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 from typing import Any, Dict, List
 
 import pytest
 from pydantic import BaseModel, RootModel
 from telegram_wallet_pay.schemas import (
     MoneyAmount,
     PaymentOption,
-    Update,
-    Updates,
+    WebhookMessage,
+    WebhookMessages,
     WebhookPayload,
 )
 
 money_amount = MoneyAmount(currency_code="RUB", amount="42")
 payment_option = PaymentOption(
     amount=money_amount,
     amount_fee=money_amount,
     amount_net=money_amount,
     exchange_rate="",
 )
-payload = WebhookPayload(
+webhook_payload = WebhookPayload(
     id=1,
     number="",
     external_id="",
     status="PAID",
     order_amount=money_amount,
     selected_payment_option=payment_option,
     order_completed_datetime=datetime.now(),
 )
-update = Update(
+webhook_message = WebhookMessage(
     event_datetime=datetime.now(),
     event_id=1,
     type="ORDER_PAID",
-    payload=payload,
+    payload=webhook_payload,
 )
 
 
 @pytest.mark.parametrize(
     ("schema", "data"),
     [
-        (Updates, [update.model_dump(by_alias=True)]),
+        (WebhookMessages, [webhook_message.model_dump(by_alias=True)]),
     ],
 )
 def test_iteration(schema: RootModel, data: List[Dict[str, Any]]) -> None:
     """Test object is iterable."""
     iterable_object = schema.model_validate(data)
     for child in iterable_object:
         assert isinstance(child, (RootModel, BaseModel))
```

### Comparing `telegram_wallet_pay-0.1.0/tests/test_signature.py` & `telegram_wallet_pay-0.2.0/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/.gitignore` & `telegram_wallet_pay-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/README.md` & `telegram_wallet_pay-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 
 
 async def main():
     # create API-client instance
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
-    result = await wallet.create_order(
+    response = await wallet.create_order(
         amount=40,
         currency_code="RUB",
         description="Test Payment",
         external_id=str(uuid4()),
         timeout_seconds=5 * 60,
         customer_telegram_user_id=66812456,
     )
 
-    # let's print creation result
-    print("Result:", result)
-    print("Order:", result.data)
+    # let's print creation response
+    print("Response:", response)
+    print("Order:", response.data)
 
     # also you can update order status via `get_preview` method
-    result = await wallet.get_preview(result.data.id)
-    print("Updated Order Preview:", result.data)
+    response = await wallet.get_preview(response.data.id)
+    print("Updated Order Preview:", response.data)
 
     # don't forget close API-client instance on your app shutdown
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `telegram_wallet_pay-0.1.0/pyproject.toml` & `telegram_wallet_pay-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.1.0/PKG-INFO` & `telegram_wallet_pay-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.1.0
+Version: 0.2.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
@@ -72,30 +72,30 @@
 
 
 async def main():
     # create API-client instance
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
-    result = await wallet.create_order(
+    response = await wallet.create_order(
         amount=40,
         currency_code="RUB",
         description="Test Payment",
         external_id=str(uuid4()),
         timeout_seconds=5 * 60,
         customer_telegram_user_id=66812456,
     )
 
-    # let's print creation result
-    print("Result:", result)
-    print("Order:", result.data)
+    # let's print creation response
+    print("Response:", response)
+    print("Order:", response.data)
 
     # also you can update order status via `get_preview` method
-    result = await wallet.get_preview(result.data.id)
-    print("Updated Order Preview:", result.data)
+    response = await wallet.get_preview(response.data.id)
+    print("Updated Order Preview:", response.data)
 
     # don't forget close API-client instance on your app shutdown
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

