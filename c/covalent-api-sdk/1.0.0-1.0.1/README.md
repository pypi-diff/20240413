# Comparing `tmp/covalent-api-sdk-1.0.0.tar.gz` & `tmp/covalent-api-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-api-sdk-1.0.0.tar", last modified: Wed Apr 10 20:22:45 2024, max compression
+gzip compressed data, was "covalent-api-sdk-1.0.1.tar", last modified: Fri Apr 12 22:12:36 2024, max compression
```

## Comparing `covalent-api-sdk-1.0.0.tar` & `covalent-api-sdk-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.806939 covalent-api-sdk-1.0.0/
--rw-r--r--   0 davidwork   (501) staff       (20)    23449 2024-04-10 20:22:45.806599 covalent-api-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)    22810 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/README.md
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.795261 covalent-api-sdk-1.0.0/covalent/
--rw-r--r--   0 davidwork   (501) staff       (20)      543 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)     2866 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/covalent_client.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.799217 covalent-api-sdk-1.0.0/covalent/services/
--rw-r--r--   0 davidwork   (501) staff       (20)        0 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)    76092 2024-03-12 23:29:12.000000 covalent-api-sdk-1.0.0/covalent/services/balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    72293 2024-04-10 20:15:51.000000 covalent-api-sdk-1.0.0/covalent/services/base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    96396 2024-04-10 20:15:51.000000 covalent-api-sdk-1.0.0/covalent/services/nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10439 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    19147 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)   112305 2024-04-10 20:15:51.000000 covalent-api-sdk-1.0.0/covalent/services/transaction_service.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.802264 covalent-api-sdk-1.0.0/covalent/services/util/
--rw-r--r--   0 davidwork   (501) staff       (20)      205 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)     3891 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      488 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/api_key_validator.py
--rw-r--r--   0 davidwork   (501) staff       (20)     2035 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)      983 2024-03-18 18:58:43.000000 covalent-api-sdk-1.0.0/covalent/services/util/calculate_pretty_balance.py
--rw-r--r--   0 davidwork   (501) staff       (20)     9913 2024-03-11 21:37:17.000000 covalent-api-sdk-1.0.0/covalent/services/util/chains.py
--rw-r--r--   0 davidwork   (501) staff       (20)      480 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/debugger.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1939 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/covalent/services/util/prettify_currency.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6601 2024-04-10 20:22:15.000000 covalent-api-sdk-1.0.0/covalent/services/util/types.py
--rw-r--r--   0 davidwork   (501) staff       (20)   137261 2024-04-04 22:14:44.000000 covalent-api-sdk-1.0.0/covalent/services/xyk_service.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.803433 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/
--rw-r--r--   0 davidwork   (501) staff       (20)    23449 2024-04-10 20:22:45.000000 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)     1239 2024-04-10 20:22:45.000000 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        1 2024-04-10 20:22:45.000000 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       61 2024-04-10 20:22:45.000000 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/requires.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        9 2024-04-10 20:22:45.000000 covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       38 2024-04-10 20:22:45.806989 covalent-api-sdk-1.0.0/setup.cfg
--rw-r--r--   0 davidwork   (501) staff       (20)     1549 2024-04-10 20:22:15.000000 covalent-api-sdk-1.0.0/setup.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-10 20:22:45.806184 covalent-api-sdk-1.0.0/tests/
--rw-r--r--   0 davidwork   (501) staff       (20)     1547 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      926 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)     8003 2024-03-12 23:29:12.000000 covalent-api-sdk-1.0.0/tests/test_balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10245 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1586 2024-03-18 18:58:43.000000 covalent-api-sdk-1.0.0/tests/test_calculate_pretty_balance.py
--rw-r--r--   0 davidwork   (501) staff       (20)      488 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_client.py
--rw-r--r--   0 davidwork   (501) staff       (20)    11861 2024-03-11 21:51:51.000000 covalent-api-sdk-1.0.0/tests/test_nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     2021 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_prettify_currency.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1336 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1656 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     7436 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_transaction_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     9115 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.0/tests/test_xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.589641 covalent-api-sdk-1.0.1/
+-rw-r--r--   0 davidwork   (501) staff       (20)    23449 2024-04-12 22:12:36.589158 covalent-api-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)    22810 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/README.md
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.577417 covalent-api-sdk-1.0.1/covalent/
+-rw-r--r--   0 davidwork   (501) staff       (20)      543 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     2866 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/covalent_client.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.581763 covalent-api-sdk-1.0.1/covalent/services/
+-rw-r--r--   0 davidwork   (501) staff       (20)        0 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    76092 2024-03-12 23:29:12.000000 covalent-api-sdk-1.0.1/covalent/services/balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    73861 2024-04-12 22:04:19.000000 covalent-api-sdk-1.0.1/covalent/services/base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    96396 2024-04-10 20:15:51.000000 covalent-api-sdk-1.0.1/covalent/services/nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10439 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    19147 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)   112305 2024-04-10 20:15:51.000000 covalent-api-sdk-1.0.1/covalent/services/transaction_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.585012 covalent-api-sdk-1.0.1/covalent/services/util/
+-rw-r--r--   0 davidwork   (501) staff       (20)      205 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     3891 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      488 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/api_key_validator.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     2035 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      983 2024-03-18 18:58:43.000000 covalent-api-sdk-1.0.1/covalent/services/util/calculate_pretty_balance.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     9913 2024-03-11 21:37:17.000000 covalent-api-sdk-1.0.1/covalent/services/util/chains.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      480 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/debugger.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1939 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/covalent/services/util/prettify_currency.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6601 2024-04-12 22:12:08.000000 covalent-api-sdk-1.0.1/covalent/services/util/types.py
+-rw-r--r--   0 davidwork   (501) staff       (20)   137261 2024-04-04 22:14:44.000000 covalent-api-sdk-1.0.1/covalent/services/xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.585890 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/
+-rw-r--r--   0 davidwork   (501) staff       (20)    23449 2024-04-12 22:12:36.000000 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)     1239 2024-04-12 22:12:36.000000 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        1 2024-04-12 22:12:36.000000 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       61 2024-04-12 22:12:36.000000 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        9 2024-04-12 22:12:36.000000 covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       38 2024-04-12 22:12:36.589696 covalent-api-sdk-1.0.1/setup.cfg
+-rw-r--r--   0 davidwork   (501) staff       (20)     1549 2024-04-12 22:12:08.000000 covalent-api-sdk-1.0.1/setup.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2024-04-12 22:12:36.588772 covalent-api-sdk-1.0.1/tests/
+-rw-r--r--   0 davidwork   (501) staff       (20)     1547 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      926 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     8003 2024-03-12 23:29:12.000000 covalent-api-sdk-1.0.1/tests/test_balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10245 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1586 2024-03-18 18:58:43.000000 covalent-api-sdk-1.0.1/tests/test_calculate_pretty_balance.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      488 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_client.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    11861 2024-03-11 21:51:51.000000 covalent-api-sdk-1.0.1/tests/test_nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     2021 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_prettify_currency.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1336 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1656 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     7436 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_transaction_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     9115 2024-03-11 20:15:02.000000 covalent-api-sdk-1.0.1/tests/test_xyk_service.py
```

### Comparing `covalent-api-sdk-1.0.0/PKG-INFO` & `covalent-api-sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-1.0.0/README.md` & `covalent-api-sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/__init__.py` & `covalent-api-sdk-1.0.1/covalent/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/covalent_client.py` & `covalent-api-sdk-1.0.1/covalent/covalent_client.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/balance_service.py` & `covalent-api-sdk-1.0.1/covalent/services/balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/base_service.py` & `covalent-api-sdk-1.0.1/covalent/services/base_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,46 @@
         self.updated_at = datetime.fromisoformat(data["updated_at"])
         self.chain_id = int(data["chain_id"])
         self.chain_name = data["chain_name"]
         self.items = [BlockHeights(item_data) for item_data in data["items"]]
         self.pagination = Pagination(data["pagination"]) if "pagination" in data and data["pagination"] is not None else None
 
 class BlockHeights:
+    block_hash: Optional[str]
+    """ The hash of the block. """
     signed_at: Optional[datetime]
     """ The block signed timestamp in UTC. """
     height: Optional[int]
     """ The block height. """
+    block_parent_hash: Optional[str]
+    """ The parent block hash. """
+    extra_data: Optional[str]
+    """ Extra data written to the block. """
+    miner_address: Optional[str]
+    """ The address of the miner. """
+    mining_cost: Optional[int]
+    """ The associated mining cost. """
+    gas_used: Optional[int]
+    """ The associated gas used. """
+    gas_limit: Optional[int]
+    """ The associated gas limit. """
+    transactions_link: Optional[str]
+    """ The link to the related tx by block endpoint. """
 
     def __init__(self, data):
+        self.block_hash = data["block_hash"] if "block_hash" in data and data["block_hash"] is not None else None
         self.signed_at = datetime.fromisoformat(data["signed_at"]) if "signed_at" in data and data["signed_at"] is not None else None
         self.height = int(data["height"]) if "height" in data and data["height"] is not None else None
+        self.block_parent_hash = data["block_parent_hash"] if "block_parent_hash" in data and data["block_parent_hash"] is not None else None
+        self.extra_data = data["extra_data"] if "extra_data" in data and data["extra_data"] is not None else None
+        self.miner_address = data["miner_address"] if "miner_address" in data and data["miner_address"] is not None else None
+        self.mining_cost = int(data["mining_cost"]) if "mining_cost" in data and data["mining_cost"] is not None else None
+        self.gas_used = int(data["gas_used"]) if "gas_used" in data and data["gas_used"] is not None else None
+        self.gas_limit = int(data["gas_limit"]) if "gas_limit" in data and data["gas_limit"] is not None else None
+        self.transactions_link = data["transactions_link"] if "transactions_link" in data and data["transactions_link"] is not None else None
 
 class Pagination:
     has_more: Optional[bool]
     """ True is there is another page. """
     page_number: Optional[int]
     """ The requested page number. """
     page_size: Optional[int]
```

### Comparing `covalent-api-sdk-1.0.0/covalent/services/nft_service.py` & `covalent-api-sdk-1.0.1/covalent/services/nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/pricing_service.py` & `covalent-api-sdk-1.0.1/covalent/services/pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/security_service.py` & `covalent-api-sdk-1.0.1/covalent/services/security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/transaction_service.py` & `covalent-api-sdk-1.0.1/covalent/services/transaction_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/api_helper.py` & `covalent-api-sdk-1.0.1/covalent/services/util/api_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/back_off.py` & `covalent-api-sdk-1.0.1/covalent/services/util/back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/calculate_pretty_balance.py` & `covalent-api-sdk-1.0.1/covalent/services/util/calculate_pretty_balance.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/chains.py` & `covalent-api-sdk-1.0.1/covalent/services/util/chains.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/prettify_currency.py` & `covalent-api-sdk-1.0.1/covalent/services/util/prettify_currency.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent/services/util/types.py` & `covalent-api-sdk-1.0.1/covalent/services/util/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal
 
 chain = Literal["btc-mainnet", "eth-mainnet", "matic-mainnet", "bsc-mainnet", "avalanche-mainnet", "optimism-mainnet", "fantom-mainnet", "moonbeam-mainnet", "moonbeam-moonriver", "rsk-mainnet", "arbitrum-mainnet", "palm-mainnet", "klaytn-mainnet", "heco-mainnet", "nervos-godwoken-mainnet", "axie-mainnet", "evmos-mainnet", "astar-mainnet", "iotex-mainnet", "harmony-mainnet", "cronos-mainnet", "aurora-mainnet", "emerald-paratime-mainnet", "boba-mainnet", "eth-goerli", "matic-mumbai", "avalanche-testnet", "bsc-testnet", "moonbeam-moonbase-alpha", "rsk-testnet", "arbitrum-goerli", "fantom-testnet", "palm-testnet", "heco-testnet", "nervos-godwoken-testnet", "evmos-testnet", "iotex-testnet", "harmony-testnet", "aurora-testnet", "scroll-l2-testnet", "scroll-sepolia-testnet", "covalent-internal-network-v1", "defi-kingdoms-mainnet", "swimmer-mainnet", "boba-avalanche-mainnet", "boba-bobabeam-mainnet", "boba-bnb-mainnet", "boba-rinkeby-testnet", "boba-bobabase-testnet", "boba-bnb-testnet", "boba-avalanche-testnet", "klaytn-testnet", "gather-mainnet", "gather-testnet", "skale-calypso", "skale-mainnet", "skale-razor", "avalanche-dexalot-mainnet", "skale-omnus", "avalanche-dexalot-testnet", "astar-shibuya", "cronos-testnet", "defi-kingdoms-testnet", "metis-mainnet", "metis-stardust", "milkomeda-a1-mainnet", "milkomeda-a1-devnet", "milkomeda-c1-mainnet", "milkomeda-c1-devnet", "swimmer-testnet", "solana-mainnet", "skale-europa", "meter-mainnet", "meter-testnet", "skale-exorde", "boba-goerli", "neon-testnet", "skale-staging-uum", "skale-staging-lcc", "arbitrum-nova-mainnet", "canto-mainnet", "bittorrent-mainnet", "bittorrent-testnet", "flarenetworks-flare-mainnet", "flarenetworks-flare-testnet", "flarenetworks-canary-mainnet", "flarenetworks-canary-testnet", "kcc-mainnet", "kcc-testnet", "polygon-zkevm-testnet", "linea-testnet", "base-testnet", "mantle-testnet", "scroll-alpha-testnet", "oasys-mainnet", "oasys-testnet", "findora-mainnet", "findora-forge-testnet", "sx-mainnet", "oasis-sapphire-mainnet", "oasis-sapphire-testnet", "optimism-goerli", "polygon-zkevm-mainnet", "horizen-yuma-testnet", "clv-parachain", "energi-mainnet", "energi-testnet", "horizen-gobi-testnet", "eth-sepolia", "skale-nebula", "skale-battleground", "avalanche-meld-testnet", "gunzilla-testnet", "ultron-mainnet", "ultron-testnet", "zora-mainnet", "zora-goerli-testnet", "neon-mainnet", "avalanche-shrapnel-mainnet", "base-mainnet", "mantle-mainnet", "avalanche-loco-legends-mainnet", "linea-mainnet", "horizen-eon-mainnet", "avalanche-numbers", "avalanche-dos", "avalanche-step-network", "avalanche-xplus", "avalanche-xanachain", "avalanche-meld-mainnet", "opside-public-zkevm", "opside-law-chain", "avalanche-shrapnel-testnet", "avalanche-loco-legends-testnet", "opside-cb-zkevm", "opside-pre-alpha-testnet", "opside-era7", "opside-xthrill", "zksync-mainnet", "metis-testnet", "zksync-testnet", "avalanche-blitz-testnet", "avalanche-d-chain-testnet", "avalanche-green-dot-testnet", "avalanche-mintara-testnet", "avalanche-beam-testnet", "bnb-meta-apes-mainnet", "bnb-antimatter-mainnet", "bnb-antimatter-testnet", "bnb-opbnb-testnet", "opside-debox", "opside-jackbot", "opside-odx-zkevm-testnet", "opside-readon-content-testnet", "opside-relation", "opside-soquest-zkevm", "opside-vip3", "opside-zkmeta", "avalanche-pulsar-testnet", "avalanche-uptn", "bnb-fncy-mainnet", "zetachain-testnet", "kinto-testnet", "mode-testnet", "loot-mainnet", "bnb-fncy-testnet", "manta-testnet", "pgn-mainnet", "pgn-testnet", "gnosis-mainnet", "gnosis-testnet", "rollux-mainnet", "rollux-testnet", "taiko-jolnir-testnet", "optimism-sepolia", "bnb-opbnb-mainnet", "telos-mainnet", "telos-testnet", "avalanche-hubble-exchange-testnet", "avalanche-miho-testnet", "avalanche-bulletin-testnet", "avalanche-kiwi-testnet", "avalanche-hero-testnet", "avalanche-avacloud-testnet", "avalanche-thirdweb-testnet", "avalanche-mondrian-testnet", "avalanche-conduit-testnet", "avalanche-nmac-testnet", "avalanche-orderly-testnet", "avalanche-amplify-testnet", "avalanche-mirai-testnet", "avalanche-wagmi-testnet", "avalanche-playa3ull-testnet", "avalanche-beam-mainnet", "scroll-mainnet", "eth-holesky", "tomochain-mainnet", "tomochain-testnet", "avalanche-jono11-testnet", "base-sepolia-testnet", "xai-testnet", "arbitrum-sepolia", "lumoz-public-zksync-v2", "lumoz-decibling", "lumoz-stark-sport", "avalanche-lt0-testnet", "avalanche-lt1-testnet", "avalanche-lt2-testnet", "avalanche-lt3-testnet", "avalanche-lt4-testnet", "avalanche-lt5-testnet", "syndr-testnet", "crossfi-evm-testnet", "celo-mainnet", "taiko-katla-testnet", "movement-mevm-testnet", "zora-sepolia-testnet", "merlin-mainnet", "merlin-testnet", "avalanche-hubble-exchange-mainnet", "xai-mainnet"]
 chain_id = Literal[20090103, 1, 137, 56, 43114, 10, 250, 1284, 1285, 30, 42161, 11297108109, 8217, 128, 71402, 2020, 9001, 592, 4689, 1666600000, 25, 1313161554, 42262, 288, 5, 80001, 43113, 97, 1287, 31, 421613, 4002, 11297108099, 256, 71401, 9000, 4690, 1666700000, 1313161555, 534354, 534351, 1131378225, 53935, 73772, 43288, 1294, 56288, 28, 1297, 9728, 4328, 1001, 192837465, 356256156, 1564830818, 278611351, 432204, 1026062157, 432201, 81, 338, 335, 1088, 588, 2002, 200202, 2001, 200101, 73773, 1399811149, 2046399126, 82, 83, 2139927552, 2888, 245022926, 344106930, 476158412, 42170, 7700, 119, 1029, 14, 114, 19, 16, 321, 322, 1422, 59140, 84531, 5001, 534353, 248, 9372, 2152, 2154, 416, 23294, 23295, 420, 1101, 1662, 1024, 39797, 49797, 1663, 11155111, 1482601649, 644937893, 222000222, 49321, 1231, 1230, 7777777, 999, 245022934, 2044, 8453, 5000, 262018, 59144, 7332, 10507, 7979, 1234, 1228, 8888, 333000333, 12008, 12011, 2038, 1995, 12010, 51178, 12009, 12012, 324, 599, 280, 1343, 11115, 6765897100, 1079, 13337, 16350, 1990, 20221, 5611, 12018, 12013, 12020, 12015, 12016, 12014, 12017, 12019, 431234, 6119, 73, 7001, 42888, 919, 5151706, 923018, 3441005, 424, 58008, 100, 10200, 570, 57000, 167007, 11155420, 204, 40, 41, 321123, 360163, 78431, 2037, 17772, 152703, 894538, 179188, 78432, 7777, 986532, 78430, 2195, 11111, 3012, 4337, 534352, 17000, 88, 89, 20765, 84532, 47279324479, 421614, 12027, 12028, 12029, 31330, 31331, 31332, 31333, 31334, 31335, 412346, 8545, 42220, 167008, 336, 999999999, 4200, 686868, 1992, 660279]
 quote = Literal["USD", "CAD", "EUR", "SGD", "INR", "JPY", "VND", "CNY", "KRW", "RUB", "TRY", "NGN", "ARS", "AUD", "CHF", "GBP"]
-user_agent = "com.covalenthq.sdk.python/1.0.0"
+user_agent = "com.covalenthq.sdk.python/1.0.1"
 
 RED = '\033[91m'
 GREEN = '\033[92m'
 YELLOW = '\033[93m'
 CYAN = '\033[96m'
 RESET = '\033[0m'  # Reset color to default
```

### Comparing `covalent-api-sdk-1.0.0/covalent/services/xyk_service.py` & `covalent-api-sdk-1.0.1/covalent/services/xyk_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/PKG-INFO` & `covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-1.0.0/covalent_api_sdk.egg-info/SOURCES.txt` & `covalent-api-sdk-1.0.1/covalent_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/setup.py` & `covalent-api-sdk-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='covalent-api-sdk',   # Replace with the name of your package
-    version='1.0.0',             # Replace with the version of your package
+    version='1.0.1',             # Replace with the version of your package
     license="MIT",
     # Description and long_description should contain a concise and detailed description of your project.
     description='covalent-api-sdk-py',
     long_description=open('README.md').read() + "\n",
     long_description_content_type='text/markdown',
     author='Covalenthq',          # Replace with your name
     python_requires='>=3.7',
```

### Comparing `covalent-api-sdk-1.0.0/tests/test_api_helper.py` & `covalent-api-sdk-1.0.1/tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_back_off.py` & `covalent-api-sdk-1.0.1/tests/test_back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_balance_service.py` & `covalent-api-sdk-1.0.1/tests/test_balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_base_service.py` & `covalent-api-sdk-1.0.1/tests/test_base_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_calculate_pretty_balance.py` & `covalent-api-sdk-1.0.1/tests/test_calculate_pretty_balance.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_nft_service.py` & `covalent-api-sdk-1.0.1/tests/test_nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_prettify_currency.py` & `covalent-api-sdk-1.0.1/tests/test_prettify_currency.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_pricing_service.py` & `covalent-api-sdk-1.0.1/tests/test_pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_security_service.py` & `covalent-api-sdk-1.0.1/tests/test_security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_transaction_service.py` & `covalent-api-sdk-1.0.1/tests/test_transaction_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-1.0.0/tests/test_xyk_service.py` & `covalent-api-sdk-1.0.1/tests/test_xyk_service.py`

 * *Files identical despite different names*

