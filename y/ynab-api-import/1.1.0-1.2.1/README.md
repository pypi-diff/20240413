# Comparing `tmp/ynab_api_import-1.1.0.tar.gz` & `tmp/ynab_api_import-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_api_import-1.1.0.tar", max compression
+gzip compressed data, was "ynab_api_import-1.2.1.tar", max compression
```

## Comparing `ynab_api_import-1.1.0.tar` & `ynab_api_import-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    35148 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/LICENSE
--rw-r--r--   0        0        0     6516 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/README.md
--rw-r--r--   0        0        0      832 2024-04-12 06:16:30.322406 ynab_api_import-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/__init__.py
--rw-r--r--   0        0        0     1373 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/accountclient.py
--rw-r--r--   0        0        0     1465 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/accountfetcher.py
--rw-r--r--   0        0        0       48 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/exceptions.py
--rw-r--r--   0        0        0      340 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/memocleaner.py
--rw-r--r--   0        0        0      757 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/config.py
--rw-r--r--   0        0        0      223 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/exceptions.py
--rw-r--r--   0        0        0     1466 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/transaction.py
--rw-r--r--   0        0        0     2913 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/requisitionhandler.py
--rw-r--r--   0        0        0     5817 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/ynabapiimport.py
--rw-r--r--   0        0        0     1036 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/ynabclient.py
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 ynab_api_import-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/LICENSE
+-rw-r--r--   0        0        0     6515 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/README.md
+-rw-r--r--   0        0        0      832 2024-04-13 06:36:19.342345 ynab_api_import-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/__init__.py
+-rw-r--r--   0        0        0     1373 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/accountclient.py
+-rw-r--r--   0        0        0     1465 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/accountfetcher.py
+-rw-r--r--   0        0        0      340 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/memocleaner.py
+-rw-r--r--   0        0        0      757 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/config.py
+-rw-r--r--   0        0        0      272 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/exceptions.py
+-rw-r--r--   0        0        0     1466 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/transaction.py
+-rw-r--r--   0        0        0     2913 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/requisitionhandler.py
+-rw-r--r--   0        0        0     6957 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/ynabapiimport.py
+-rw-r--r--   0        0        0     1036 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/ynabclient.py
+-rw-r--r--   0        0        0     7324 1970-01-01 00:00:00.000000 ynab_api_import-1.2.1/PKG-INFO
```

### Comparing `ynab_api_import-1.1.0/LICENSE` & `ynab_api_import-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/README.md` & `ynab_api_import-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 ### Compare balances
 This method will fetch the available [balance variants](https://developer.gocardless.com/bank-account-data/balance) for your account from the API and compare them to the balance in YNAB. It compares the plain balance values as well as the balances minus the sum of still pending transactions. If none of them match it raises a `BalancesDontMatchError`
 ```py
 ynab_api_import.compare_balances()
 ```
 ### Delete current bank authorization
 By default you can create only one bank authorization per reference. If you need to replace the authorization under 
-your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
+your current reference you can explicitly do that by setting the `delete_current_auth` option when creating an auth 
 link.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
 ### Show Logs
 The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs 
 import the logging module and set it to the level `INFO`. You can also access the logger for advanced configuration
```

### Comparing `ynab_api_import-1.1.0/pyproject.toml` & `ynab_api_import-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-api-import"
-version = "1.1.0"
+version = "1.2.1"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to import bank transactions via API into You Need A Budget (YNAB)"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabapiimport'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_api_import-1.1.0/ynabapiimport/accountclient.py` & `ynab_api_import-1.2.1/ynabapiimport/accountclient.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/ynabapiimport/accountfetcher.py` & `ynab_api_import-1.2.1/ynabapiimport/accountfetcher.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/ynabapiimport/models/config.py` & `ynab_api_import-1.2.1/ynabapiimport/models/config.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/ynabapiimport/models/transaction.py` & `ynab_api_import-1.2.1/ynabapiimport/models/transaction.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/ynabapiimport/requisitionhandler.py` & `ynab_api_import-1.2.1/ynabapiimport/requisitionhandler.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/ynabapiimport/ynabapiimport.py` & `ynab_api_import-1.2.1/ynabapiimport/ynabapiimport.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,36 +2,51 @@
 from datetime import date, timedelta
 from pathlib import Path
 from typing import List
 
 import yaml
 from nordigen import NordigenClient
 
-from ynabapiimport.exceptions import BalancesDontMatchError
+from ynabapiimport.models.exceptions import BalancesDontMatchError
 from ynabapiimport.requisitionhandler import RequisitionHandler
 from ynabapiimport.accountclient import AccountClient
 from ynabapiimport.memocleaner import MemoCleaner
 from ynabapiimport.ynabclient import YnabClient
 
 
 class YnabApiImport:
 	"""
 	Class which allows to connect to bank accounts via GoCardless API and import transactions into YNAB
+	:ivar reference: self chosen reference string to identify connection in GoCardless
+	:ivar resource_id: GoCardless resource id to specify accounts in case multiple are available
+	:ivar logger: Logger object which receives info messages from methods
 	"""
 
 	def __init__(self, secret_id: str, secret_key: str, token: str,
 				 reference: str, budget_id: str, account_id: str, resource_id: str = None) -> None:
+		"""
+		:param secret_id: Secret id from GoCardless
+		:param secret_key: Secret Key from GoCardless
+		:param token: YNAB token
+		:param reference: self chosen reference string to identify connection in GoCardless
+		:param budget_id: YNAB budget id
+		:param account_id: YNAB account id
+		:param resource_id: GoCardless resource id to specify accounts in case multiple are available
+		:raises NoRequisitionError: if GoCardless connection is not valid
+		:raises NoAccountError: if no account is available in authorized GoCardless connection
+		:raises MultipleAccountsError: if multiple accounts are available in authorized GoCardless connection
+		"""
 		self.logger = self._set_up_logger()
-		self._reference = reference
-		self._resource_id = resource_id
+		self.reference = reference
+		self.resource_id = resource_id
 		self._ynab_client = YnabClient(token=token, account_id=account_id, budget_id=budget_id)
 		self._api_client = NordigenClient(secret_id=secret_id, secret_key=secret_key)
 		self._api_client.generate_token()
-		self._account_client = AccountClient.from_api_client(client=self._api_client, reference=self._reference,
-										  resource_id=resource_id)
+		self._account_client = AccountClient.from_api_client(client=self._api_client, reference=self.reference,
+										  resource_id=self.resource_id)
 
 	@classmethod
 	def from_yaml(cls, path: str):
 		"""
 		Creates instance from provided yaml file
 		:param path: path to yaml configuration file
 		:return: instance of YnabApiImport
@@ -64,68 +79,70 @@
 		transactions = self._account_client.fetch_transactions(startdate=startdate)
 
 		if memo_regex:
 			mc = MemoCleaner(memo_regex=memo_regex)
 			transactions = [mc.clean(t) for t in transactions]
 
 		i = self._ynab_client.insert(transactions)
-		self.logger.info(f"inserted {i} transactions for {self._reference}")
+		self.logger.info(f"inserted {i} transactions for {self.reference}")
 		return i
 
 	def compare_balances(self):
 		"""
 		Compares balance variants for the account (e.g. expected, closingBooked) from API and from YNAB. The method
 		compares the plain balance values as well as the balances minus the sum of still pending transactions.
 		:raises BalancesDontMatchError: if none of the API returned balances for the account match with the one in YNAB
 		"""
 		ab, ap = self._account_client.fetch_balances()
 		yb = self._ynab_client.fetch_balance()
 		if yb not in ab.values() and yb not in [b - ap for b in ab.values()]:
 			raise BalancesDontMatchError({'api': ab, 'ynab': yb, 'pending': ap})
-		self.logger.info(f'balances match for {self._reference}')
+		self.logger.info(f'balances match for {self.reference}')
 
 	def create_auth_link(self, institution_id: str, use_max_historical_days: bool = False,
 						 delete_current_auth: bool = False) -> str:
 		"""
 		Creates a link to authenticate access to specified bank through GoCardless. Link needs to be used in browser
 		:param institution_id: Gocardless id for your bank
-		:param use_max_historical_days: If set to True will create an auth link for the max_days specified in history for the bank
+		:param use_max_historical_days: If set to True will create an auth link for the max_days specified in history for the bank (might cause a 500 error with API if bank doesn't support for any reason)
 		:param delete_current_auth: if set to True will delete currently active auth
 		:return: Link to authenticate access to bank through Gocardless
+		:raises ReferenceNotValidError: if reference string contains illegal characters
+		:raises ReferenceNotUniqueError: if existing connection already uses the reference
 		"""
-		rh = RequisitionHandler(client=self._api_client, reference=self._reference)
+		rh = RequisitionHandler(client=self._api_client, reference=self.reference)
 		if delete_current_auth:
 			rh.delete_current_requisition()
-			self.logger.info(f'deleted auth for reference {self._reference}')
+			self.logger.info(f'deleted auth for reference {self.reference}')
 		auth_link = rh.create_requisition_auth_link(institution_id=institution_id,
 													use_max_historical_days=use_max_historical_days)
-		self.logger.info(f'created auth link for {institution_id} under reference {self._reference}')
+		self.logger.info(f'created auth link for {institution_id} under reference {self.reference}')
 		return auth_link
 
 	def fetch_institutions(self, countrycode: str) -> List[dict]:
 		"""
 		Fetches institutions for specified country from GoCardless
 		:param countrycode: ISO2 country code
 		:return: List of available institutions in country with as with name, institution_id and max_history_days
 		"""
-		rh = RequisitionHandler(client=self._api_client, reference=self._reference)
+		rh = RequisitionHandler(client=self._api_client, reference=self.reference)
 		institutions = rh.get_institutions(countrycode=countrycode)
 		self.logger.info(f'fetched list with {len(institutions)} institutions for countrycode {countrycode}')
 		return institutions
 
 	def test_memo_regex(self, memo_regex: str) -> List[dict]:
 		"""
 		Tests cleaning memos in transactions from bank with provided regex. Will test on bank transactions from last 90 days
 		:param memo_regex: Regex expression to use for cleaning memos
 		:return: list with `dict` which has original memo as key and cleaned memo as value
 		"""
 		transactions = self._account_client.fetch_transactions(date.today() - timedelta(days=90))
 		mc = MemoCleaner(memo_regex=memo_regex)
 		r = [{t.memo: mc.clean(t).memo} for t in transactions]
-		self.logger.info(f'tested memo regex on {len(r)} transactions from {self._reference}')
+		self.logger.info(f'tested memo regex on {len(r)} transactions from {self.reference}')
 		return r
 
 	@staticmethod
 	def _set_up_logger() -> logging.Logger:
 		parent_name = '.'.join(__name__.split('.')[:-1])
 		logger = logging.getLogger(parent_name)
 		logger.setLevel(20)
```

### Comparing `ynab_api_import-1.1.0/ynabapiimport/ynabclient.py` & `ynab_api_import-1.2.1/ynabapiimport/ynabclient.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.1.0/PKG-INFO` & `ynab_api_import-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-api-import
-Version: 1.1.0
+Version: 1.2.1
 Summary: Library to import bank transactions via API into You Need A Budget (YNAB)
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -121,15 +121,15 @@
 ### Compare balances
 This method will fetch the available [balance variants](https://developer.gocardless.com/bank-account-data/balance) for your account from the API and compare them to the balance in YNAB. It compares the plain balance values as well as the balances minus the sum of still pending transactions. If none of them match it raises a `BalancesDontMatchError`
 ```py
 ynab_api_import.compare_balances()
 ```
 ### Delete current bank authorization
 By default you can create only one bank authorization per reference. If you need to replace the authorization under 
-your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
+your current reference you can explicitly do that by setting the `delete_current_auth` option when creating an auth 
 link.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
 ### Show Logs
 The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs 
 import the logging module and set it to the level `INFO`. You can also access the logger for advanced configuration
```

