# Comparing `tmp/cefi-4.4.9.tar.gz` & `tmp/cefi-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.4.9.tar", max compression
+gzip compressed data, was "cefi-4.5.0.tar", max compression
```

## Comparing `cefi-4.4.9.tar` & `cefi-4.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-07 14:56:21.924445 cefi-4.4.9/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-07 14:56:21.924445 cefi-4.4.9/README.md
--rw-r--r--   0        0        0       87 2024-04-07 14:56:56.448538 cefi-4.4.9/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/__init__.py
--rw-r--r--   0        0        0    10668 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     7383 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8055 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/main.py
--rw-r--r--   0        0        0     3734 2024-04-07 14:56:56.448538 cefi-4.4.9/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-12 09:41:58.953568 cefi-4.5.0/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-12 09:41:58.953568 cefi-4.5.0/README.md
+-rw-r--r--   0        0        0       87 2024-04-12 09:42:35.558231 cefi-4.5.0/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    10523 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-12 09:41:58.953568 cefi-4.5.0/cefi/main.py
+-rw-r--r--   0        0        0     3756 2024-04-12 09:42:35.558231 cefi-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.5.0/PKG-INFO
```

### Comparing `cefi-4.4.9/LICENSE` & `cefi-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/README.md` & `cefi-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/cefi/default_settings.toml` & `cefi-4.5.0/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/cefi/handler/capitalcom.py` & `cefi-4.5.0/cefi/handler/capitalcom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 
 Capital.com API client
 
 
 """
 
-from datetime import datetime, timedelta
+import asyncio
 
 from capitalcom.client import Client, DirectionType
 from capitalcom.client_demo import Client as DemoClient
 from loguru import logger
 
 from .client import CexClient
 
@@ -45,95 +45,110 @@
     ):
         """
         Initialize the capital.com client
 
         """
         super().__init__(**kwargs)
         try:
-            if self.testmode:
-                self.client = DemoClient(
-                    log=self.user_id,
-                    pas=self.password,
-                    api_key=self.api_key,
-                )
-            else:
-                self.client = Client(
-                    log=self.user_id,
-                    pas=self.password,
-                    api_key=self.api_key,
-                )
 
+            self._build_client()
             logger.debug("Client: {}", self.client)
             self.accounts_data = self.client.all_accounts()
             logger.debug("Account data: {}", self.accounts_data)
             self.account_number = self.accounts_data["accounts"][0]["accountId"]
             logger.debug("Account number: {}", self.account_number)
+            logger.debug("Session details: {}", self.client.get_sesion_details())
 
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
 
+    def _build_client(self):
+        """
+        Builds and sets the client based on the testmode flag.
+
+        Capital.com session last only 10 minutes
+
+        """
+
+        if self.testmode:
+            self.client = DemoClient(
+                log=self.user_id,
+                pas=self.password,
+                api_key=self.api_key,
+            )
+        else:
+            self.client = Client(
+                log=self.user_id,
+                pas=self.password,
+                api_key=self.api_key,
+            )
+
     async def get_quote(self, instrument):
         """
         Asynchronously fetches a ask/offer quote
         for the specified instrument.
 
         :param instrument: The instrument for which the quote is to be fetched.
         :return: The fetched quote.
         """
         try:
+            self._build_client()
             logger.debug("Instrument: {}", instrument)
             instrument = await self.replace_instrument(instrument)
             logger.debug("Changed Instrument: {}", instrument)
-            search_markets = self.client.searching_market(searchTerm=instrument)
-            logger.debug("Instrument verification: {}", search_markets)
+            # search_markets = self.client.searching_market(searchTerm=instrument)
+            await asyncio.sleep(1)  # Wait for 1 second
+            # logger.debug("Instrument verification: {}", search_markets)
 
             market = self.client.single_market(instrument)
-            logger.debug("Raw Quote: {}", market)
+            # logger.debug("Raw Quote: {}", market)
 
             quote = market["snapshot"]["offer"]
             logger.debug("Quote: {}", quote)
 
-            return quote
+            return float(quote)
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
             return e
 
+    # Alias for get_quote
+    get_offer = get_quote
+
     async def get_bid(self, instrument):
         """
         Asynchronously retrieves the bid
         for the specified instrument.
 
         Args:
             instrument: The instrument for which
             the bid is to be retrieved.
 
         Returns:
             The bid for the specified instrument.
         """
         try:
+            self._build_client()
             logger.debug("Instrument: {}", instrument)
             instrument = await self.replace_instrument(instrument)
             logger.debug("Changed Instrument: {}", instrument)
-            search_markets = self.client.searching_market(searchTerm=instrument)
-            logger.debug("Instrument verification: {}", search_markets)
+            # search_markets = self.client.searching_market(searchTerm=instrument)
+            await asyncio.sleep(1)  # Wait for 1 second
+            # logger.debug("Instrument verification: {}", search_markets)
 
             market = self.client.single_market(instrument)
-            logger.debug("Raw Quote: {}", market)
+            # logger.debug("market: {}", market)
 
             quote = market["snapshot"]["bid"]
             logger.debug("Quote: {}", quote)
 
-            return quote
+            return float(quote)
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
             return e
 
-    # Alias for get_quote
-    get_offer = get_quote
-
     async def get_account_balance(self):
         """
         return account balance of
         a given ccxt exchange
 
         Args:
             None
@@ -174,41 +189,32 @@
                     epic = market_details.get("epic", "")
                     upl = position_details.get("upl", 0)
                     extracted_positions.append(f"{epic}: {upl}")
                 return "\n".join(extracted_positions)
         except Exception as e:
             logger.error(f"{self.name} Error {e}")
 
-    async def get_account_pnl(self, period=None):
+    async def calculate_pnl(self, period=None):
         """
-        Return account pnl.
+        no pnl info available via openapi endpoint
 
         Args:
             None
 
         Returns:
             pnl
         """
-        today = datetime.now().date()
-        if period is None:
-            start_date = today
-        elif period == "W":
-            start_date = today - timedelta(days=today.weekday())
-        elif period == "M":
-            start_date = today.replace(day=1)
-        elif period == "Y":
-            start_date = today.replace(month=1, day=1)
-
-        end_date = datetime.now()
-        formatted_end_date = end_date.strftime("%Y-%m-%dT%H:%M:%S")
-        logger.debug("{} {}", start_date, formatted_end_date)
+        # end_date = datetime.now()
+        # formatted_end_date = end_date.strftime("%Y-%m-%dT%H:%M:%S")
+        # logger.debug("{} {}", start_date, formatted_end_date)
         # history = self.client.account_activity_history(
-        #     fr=start_date, to=formatted_end_date, detailed=True, type="TRADE"
+        #     fr=start_date, to=formatted_end_date, detailed=True
         # )
-        # no pnl info available via openapi endpoint
+        # logger.debug("History: {}", history)
+
         return 0
 
     async def pre_order_checks(self, order_params):
         """ """
         return True
 
     async def get_trading_asset_balance(self):
@@ -259,64 +265,59 @@
             instrument = await self.replace_instrument(order_params.get("instrument"))
             quantity = order_params.get("quantity", self.trading_risk_amount)
             amount = await self.get_order_amount(
                 quantity=quantity,
                 instrument=instrument,
                 is_percentage=self.trading_risk_percentage,
             )
+            await asyncio.sleep(1)  # Wait for 1 second
+
             if not (await self.pre_order_checks(order_params)):
                 return f"Error executing {self.name}"
 
             decimals = await self.get_instrument_decimals(instrument)
+            await asyncio.sleep(1)  # Wait for 1 second
+
+            offer = await self.get_offer(instrument)
+            await asyncio.sleep(1)  # Wait for 1 second
+
+            bid = await self.get_bid(instrument)
+            await asyncio.sleep(1)  # Wait for 1 second
 
+            logger.debug("bid {}", bid)
+            logger.debug("offer {}", offer)
             profit_price = (
-                (
-                    await self.get_offer(instrument)
-                    + (order_params.get("take_profit", 0) / (10**decimals))
-                )
+                (offer + (int(order_params.get("take_profit", 0)) / (10**decimals)))
                 if action_str == "BUY"
-                else (
-                    await self.get_bid(instrument)
-                    - (order_params.get("take_profit", 0) / (10**decimals))
-                )
+                else (bid - (int(order_params.get("take_profit", 0)) / (10**decimals)))
             )
             stop_price = (
-                (
-                    await self.get_bid(instrument)
-                    - (order_params.get("stop_loss", 0) / (10**decimals))
-                )
+                (bid - (int(order_params.get("stop_loss", 0)) / (10**decimals)))
                 if action_str == "BUY"
-                else (
-                    self.get_offer(instrument)
-                    + (order_params.get("stop_loss", 0) / (10**decimals))
-                )
+                else (offer + (int(order_params.get("stop_loss", 0)) / (10**decimals)))
             )
             logger.debug("stop price {}", stop_price)
             logger.debug("profit price {}", profit_price)
-            try:
-                order = self.client.place_the_position(
-                    direction=action,
-                    epic=instrument,
-                    size=amount,
-                    gsl=False,
-                    tsl=False,
-                    stop_level=stop_price,
-                    stop_distance=None,
-                    stop_amount=None,
-                    profit_level=profit_price,
-                    profit_distance=None,
-                    profit_amount=None,
-                )
-                # Check if the order response contains an errorCode
-                if "errorCode" in order:
-                    # Handle the error, e.g., log it or return a specific message
-                    logger.error(f"Error placing order: {order['errorCode']}")
-                    return f"Error placing order: {order['errorCode']}"
-            except Exception as e:
-                return str(e)
+            order = self.client.place_the_position(
+                direction=action,
+                epic=instrument,
+                size=amount,
+                gsl=False,
+                tsl=False,
+                stop_level=stop_price,
+                stop_distance=None,
+                stop_amount=None,
+                profit_level=profit_price,
+                profit_distance=None,
+                profit_amount=None,
+            )
+
+            if "errorCode" in order:
+                logger.error(f"Error placing order: {order['errorCode']}")
+                return str(order["errorCode"])
 
             logger.debug("Order: {}", order)
             deal_reference = order["dealReference"]
             order_check = self.client.position_order_confirmation(
                 deal_reference=deal_reference
             )
```

### Comparing `cefi-4.4.9/cefi/handler/ccxt.py` & `cefi-4.5.0/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/cefi/handler/client.py` & `cefi-4.5.0/cefi/handler/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 CEX client based
 class
 
 
 """
 
+from datetime import datetime, timedelta
+
 from loguru import logger
 
 
 class CexClient:
     """
     CEX Object to support CEFI
     exchange and trading
@@ -18,14 +20,31 @@
 
     Args:
         None
 
     Returns:
         None
 
+    Methods:
+        get_quote(self, instrument)
+        get_offer(self, instrument)
+        get_bid(self, instrument)
+        get_account_balance(self)
+        get_account_position(self)
+        calculate_pnl(self, period=None)
+        get_account_pnl(self, start_date)
+        execute_order(self, order_params)
+        get_trading_asset_balance(self)
+        get_order_amount(self, quantity, instrument, is_percentage)
+        pre_order_checks(self, order_params)
+        replace_instrument(self, instrument)
+        get_instrument_decimals(self, instrument)
+        get_trade_confirmation(self, order_params)
+
+
     """
 
     def __init__(self, **kwargs):
         """
         Initialize the Cex object
 
         """
@@ -57,14 +76,15 @@
             self.leverage_type = kwargs.get("leverage_type", None)
             self.leverage = kwargs.get("leverage", None)
             self.defaulttype = kwargs.get("defaulttype", None)
             self.ordertype = kwargs.get("ordertype", None)
             self.mapping = kwargs.get("mapping", None)
             self.balance_limit = kwargs.get("balance_limit", True)
             self.balance_limit_value = kwargs.get("balance_limit_value", 10)
+            self.is_pnl_active = kwargs.get("is_pnl_active", False)
 
         except Exception as error:
             logger.error("Client initialization error {}", error)
             return None
         if not self.enabled:
             logger.debug("{} Not enabled", self.name)
             return
@@ -126,14 +146,38 @@
 
         Args:
             None
 
         Returns:
             pnl
         """
+        today = datetime.now().date()
+        if period is None:
+            start_date = today
+        elif period == "W":
+            start_date = today - timedelta(days=today.weekday())
+        elif period == "M":
+            start_date = today.replace(day=1)
+        elif period == "Y":
+            start_date = today.replace(month=1, day=1)
+        else:
+            return 0
+        return self.calculate_pnl(start_date) if self.is_pnl_active else 0
+
+    async def calculate_pnl(self, period=None):
+        """
+        Calculate the PnL for a given period.
+
+        Parameters:
+            period (str): The period for which
+            to calculate PnL ('W', 'M', 'Y', or None).
+
+        Returns:
+            pnl: The calculated PnL value.
+        """
 
     async def execute_order(self, order_params):
         """
         Execute order
 
         Args:
             order_params (dict):
@@ -174,21 +218,23 @@
         """
         balance = await self.get_trading_asset_balance()
         logger.debug("Balance {}", balance)
         quote = await self.get_quote(instrument)
         logger.debug("Quote {}", quote)
 
         if not is_percentage and balance and quote:
+            logger.debug("Amount based on money {}", balance * quantity / quote)
             return quantity
 
         if balance and quote:
             risk_percentage = float(quantity) / 100
             amount = balance * risk_percentage / quote
-            logger.debug("Amount {}", amount)
+            logger.debug("Amount based on percentage {}", amount)
         if amount >= self.trading_amount_threshold:
+            logger.debug("Amount above threshold {}", amount)
             return amount
 
     async def pre_order_checks(self, order_params):
         """ """
 
     async def replace_instrument(self, instrument):
         """
@@ -246,10 +292,10 @@
             trade_confirmation += f"⚫ {round(0 or trade['amount'], 4)}\n"
             trade_confirmation += f"🔵 {round(0 or trade['price'], 4)}\n"
             trade_confirmation += f"🟢 {round(0 or trade['takeProfitPrice'], 4)}\n"
             trade_confirmation += f"🔴 {round(0 or trade['stopLossPrice'], 4)}\n"
             trade_confirmation += f"ℹ️ {trade['id']}\n"
             trade_confirmation += f"🗓️ {trade['datetime']}"
             if trade_confirmation:
-                return f"{self.name}:\n{trade_confirmation}"
+                return f"{trade_confirmation}"
         except Exception as e:
             logger.error("Error {}", e)
```

### Comparing `cefi-4.4.9/cefi/handler/ctrader.py` & `cefi-4.5.0/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/cefi/handler/ib_sync.py` & `cefi-4.5.0/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.9/cefi/main.py` & `cefi-4.5.0/cefi/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,27 +222,32 @@
 
         """
         _info = ["📊\n"]
         for client in self.clients:
             _info.append(f"{client.name}:\n{await client.get_account_position()}")
         return "\n".join(_info)
 
-    async def get_pnls(self):
+    async def get_pnls(self, **kwargs):
         """
         Return account pnl.
 
         Args:
             None
 
         Returns:
             pnl
         """
-        _info = ["📊\n"]
+        _info = ["🏆\n"]
         for client in self.clients:
-            _info.append(f"{client.name}:\n{await client.get_account_pnl()}")
+            client_name = f"{client.name}:\n"
+            account_pnl = await client.get_account_pnl(
+                period=kwargs.get("period", None)
+            )
+            client_info = f"{client_name}{account_pnl}"
+            _info.append(client_info)
         return "\n".join(_info)
 
     async def submit_order(self, order_params):
         """
         Execute order
 
         Args:
@@ -251,15 +256,13 @@
                 instrument(str)
                 quantity(int)
 
         Returns:
             trade_confirmation(dict)
 
         """
-        order = []
+        _order = ["🧾 Order\n"]
         for client in self.clients:
-            try:
-                trade = await client.execute_order(order_params)
-                order.append(trade)
-            except Exception as e:
-                logger.error("submit_order - client {} error {}", client.name, e)
-        return order
+            _order.append(
+                f"{client.name}:\n{await client.execute_order(order_params)}\n"
+            )
+        return "\n".join(_order)
```

### Comparing `cefi-4.4.9/pyproject.toml` & `cefi-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.4.9"
+version = "4.5.0"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -146,27 +146,49 @@
 
 
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `cefi-4.4.9/PKG-INFO` & `cefi-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.4.9
+Version: 4.5.0
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.4.9 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.5.0 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

