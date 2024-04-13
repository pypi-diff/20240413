# Comparing `tmp/msfinance-0.2.1.tar.gz` & `tmp/msfinance-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfinance-0.2.1.tar", last modified: Thu Nov 16 14:10:16 2023, max compression
+gzip compressed data, was "msfinance-0.2.2.tar", last modified: Sat Apr 13 03:51:38 2024, max compression
```

## Comparing `msfinance-0.2.1.tar` & `msfinance-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 14:10:16.478173 msfinance-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-16 14:10:06.000000 msfinance-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2023-11-16 14:10:16.478173 msfinance-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-11-16 14:10:06.000000 msfinance-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 14:10:16.478173 msfinance-0.2.1/msfinance/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 14:10:06.000000 msfinance-0.2.1/msfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18189 2023-11-16 14:10:06.000000 msfinance-0.2.1/msfinance/stocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 14:10:16.478173 msfinance-0.2.1/msfinance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2023-11-16 14:10:16.000000 msfinance-0.2.1/msfinance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-16 14:10:16.000000 msfinance-0.2.1/msfinance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 14:10:16.000000 msfinance-0.2.1/msfinance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-16 14:10:16.000000 msfinance-0.2.1/msfinance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-16 14:10:16.000000 msfinance-0.2.1/msfinance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-16 14:10:06.000000 msfinance-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 14:10:16.478173 msfinance-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 14:10:16.478173 msfinance-0.2.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2088 2023-11-16 14:10:06.000000 msfinance-0.2.1/tests/test_stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 03:51:38.393850 msfinance-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 03:51:34.000000 msfinance-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-13 03:51:38.393850 msfinance-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-13 03:51:34.000000 msfinance-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 03:51:38.389850 msfinance-0.2.2/msfinance/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-13 03:51:34.000000 msfinance-0.2.2/msfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-13 03:51:34.000000 msfinance-0.2.2/msfinance/stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 03:51:38.393850 msfinance-0.2.2/msfinance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-13 03:51:38.000000 msfinance-0.2.2/msfinance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-13 03:51:38.000000 msfinance-0.2.2/msfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 03:51:38.000000 msfinance-0.2.2/msfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 03:51:38.000000 msfinance-0.2.2/msfinance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 03:51:38.000000 msfinance-0.2.2/msfinance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 03:51:34.000000 msfinance-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 03:51:38.393850 msfinance-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 03:51:38.393850 msfinance-0.2.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2168 2024-04-13 03:51:34.000000 msfinance-0.2.2/tests/test_stocks.py
```

### Comparing `msfinance-0.2.1/LICENSE` & `msfinance-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msfinance-0.2.1/PKG-INFO` & `msfinance-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfinance
-Version: 0.2.1
+Version: 0.2.2
 Summary: msfinance offers Pythonic way to download stocks financial data from morningstar.com
 Author-email: Jimmy Situ <web@jimmystone.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,39 +237,39 @@
 
 ## Quick Start
 ```python
 #!/usr/bin/python3 -u
 import msfinance as msf
 
 stock = msf.Stock(
-    session='msf_database.sql3',
+    session='msf_database.db3',
 )
 
 
 print(stock.get_income_statement('aapl', 'xnas'))
 print(stock.get_balance_sheet_statement('aapl', 'xnas'))
 print(stock.get_cash_flow_statement('aapl', 'xnas'))
 
 print(stock.get_growth('aapl', 'xnas'))
 print(stock.get_operating_and_efficiency('aapl', 'xnas'))
 print(stock.get_financial_health('aapl', 'xnas'))
 print(stock.get_cash_flow('aapl', 'xnas'))
 ```
-- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory
+- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory. Add msfinance path to environment variable: PYTHONPATH, and run examples directly 
 
 
 ## US Tickers and Exchanges
 - Get all tickers symbol of each exchange [here](https://www.nasdaq.com/market-activity/stocks/screener)
 
 
 ## HK Tickers and Exchanges
-- TBD
+- Get all tickers numbers of Heng Seng Index [here](https://en.wikipedia.org/wiki/Hang_Seng_Index#Components)
 
 
 ## TODO
 - [x] Add 'Last Updated' to database record
-- [ ] Add docs in docs directory for readthedoc.io
 - [x] Add support for pip package
+- [x] Add tickers from HK exchanges
+- [ ] Add docs in docs directory for readthedoc.io
 - [ ] Add multiprocessing for speed up
 - [ ] More robust error handling
-- [ ] Add tickers from HK exchanges
 - [ ] Add more statistics valuations
```

### Comparing `msfinance-0.2.1/README.md` & `msfinance-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,39 +14,39 @@
 
 ## Quick Start
 ```python
 #!/usr/bin/python3 -u
 import msfinance as msf
 
 stock = msf.Stock(
-    session='msf_database.sql3',
+    session='msf_database.db3',
 )
 
 
 print(stock.get_income_statement('aapl', 'xnas'))
 print(stock.get_balance_sheet_statement('aapl', 'xnas'))
 print(stock.get_cash_flow_statement('aapl', 'xnas'))
 
 print(stock.get_growth('aapl', 'xnas'))
 print(stock.get_operating_and_efficiency('aapl', 'xnas'))
 print(stock.get_financial_health('aapl', 'xnas'))
 print(stock.get_cash_flow('aapl', 'xnas'))
 ```
-- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory
+- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory. Add msfinance path to environment variable: PYTHONPATH, and run examples directly 
 
 
 ## US Tickers and Exchanges
 - Get all tickers symbol of each exchange [here](https://www.nasdaq.com/market-activity/stocks/screener)
 
 
 ## HK Tickers and Exchanges
-- TBD
+- Get all tickers numbers of Heng Seng Index [here](https://en.wikipedia.org/wiki/Hang_Seng_Index#Components)
 
 
 ## TODO
 - [x] Add 'Last Updated' to database record
-- [ ] Add docs in docs directory for readthedoc.io
 - [x] Add support for pip package
+- [x] Add tickers from HK exchanges
+- [ ] Add docs in docs directory for readthedoc.io
 - [ ] Add multiprocessing for speed up
 - [ ] More robust error handling
-- [ ] Add tickers from HK exchanges
 - [ ] Add more statistics valuations
```

### Comparing `msfinance-0.2.1/msfinance/stocks.py` & `msfinance-0.2.2/msfinance/stocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.proxy import Proxy, ProxyType
 
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import ElementClickInterceptedException
+from selenium.common.exceptions import ElementNotInteractableException
 from selenium.common.exceptions import TimeoutException
 
 
 # For Chrome driver
 from webdriver_manager.chrome import ChromeDriverManager
 
 # Form Firefox driver
@@ -224,17 +225,17 @@
             if df is not None:
                 return df
 
         # Fetch data from website starts here
         url = f"https://www.morningstar.com/stocks/{exchange}/{ticker}/financials"
         self.driver.get(url)
 
-        # Select income statement
-        income_button = self.driver.find_element(By.XPATH, f"//button[contains(., '{statement}')]")
-        income_button.click()
+        # Select statement type
+        type_button = self.driver.find_element(By.XPATH, f"//button[contains(., '{statement}')]")
+        type_button.click()
 
         # Select statement period
         period_list_button = self.driver.find_element(By.XPATH, "//button[contains(., 'Annual') and @aria-haspopup='true']")
         try:
             period_list_button.click()
             time.sleep(1)
         except ElementClickInterceptedException:
@@ -247,32 +248,36 @@
         
         try:
             period_button.click()
             time.sleep(1)
         except ElementClickInterceptedException:
             pass
 
-        # Select statement type
-        type_list_button = self.driver.find_element(By.XPATH, "//button[contains(., 'As Originally Reported') and @aria-haspopup='true']")
+        # Select statement stage
+        stage_list_button = self.driver.find_element(By.XPATH, "//button[contains(., 'As Originally Reported') and @aria-haspopup='true']")
         try: 
-            type_list_button.click()
+            stage_list_button.click()
             time.sleep(1)
         except ElementClickInterceptedException:
             pass
+        except ElementNotInteractableException:
+            pass
 
         if 'As Originally Reported' == stage:
-            type_button = self.driver.find_element(By.XPATH, "//span[contains(., 'As Originally Reported') and @class='mds-list-group__item-text__sal']")
+            stage_button = self.driver.find_element(By.XPATH, "//span[contains(., 'As Originally Reported') and @class='mds-list-group__item-text__sal']")
         else:
-            type_button = self.driver.find_element(By.XPATH, "//span[contains(., 'Restated') and @class='mds-list-group__item-text__sal']")
+            stage_button = self.driver.find_element(By.XPATH, "//span[contains(., 'Restated') and @class='mds-list-group__item-text__sal']")
 
         try: 
-            type_button.click()
+            stage_button.click()
             time.sleep(1)
         except ElementClickInterceptedException:
             pass
+        except ElementNotInteractableException:
+            pass
 
         # Expand the detail page
         expand_detail_view = WebDriverWait(self.driver, 30).until(
             EC.visibility_of_element_located((By.XPATH, "//span[contains(., 'Expand Detail View')]"))
         )
         expand_detail_view.click()
 
@@ -345,152 +350,168 @@
             ticker: Stock symbol
             exchange: Exchange name
             update: Force update data from website
         Returns:
             DataFrame of statistics
         '''
         statistics = 'Growth'
-        return self._get_valuation(ticker, exchange, statistics)
+        return self._get_valuation(ticker, exchange, statistics, update)
     
-    def get_operating_and_efficiency(self, ticker, exchange):
+    def get_operating_and_efficiency(self, ticker, exchange, update=False):
         '''
         Get operating and efficiency statistics of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
         Returns:
             DataFrame of statistics
         '''
         statistics = 'Operating and Efficiency'
-        return self._get_valuation(ticker, exchange, statistics)
+        return self._get_valuation(ticker, exchange, statistics, update)
     
-    def get_financial_health(self, ticker, exchange):
+    def get_financial_health(self, ticker, exchange, update=False):
         '''
         Get financial health statistics of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
         Returns:
             DataFrame of statistics
         '''
         statistics = 'Financial Health'
-        return self._get_valuation(ticker, exchange, statistics)
+        return self._get_valuation(ticker, exchange, statistics, update)
     
-    def get_cash_flow(self, ticker, exchange):
+    def get_cash_flow(self, ticker, exchange, update=False):
         '''
         Get cash flow statistics of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
         Returns:
             DataFrame of statistics
         '''
         statistics = 'Cash Flow'
-        return self._get_valuation(ticker, exchange, statistics)
+        return self._get_valuation(ticker, exchange, statistics, update)
 
-    def get_valuations(self, ticker, exchange):
+    def get_valuations(self, ticker, exchange, update=False):
         '''
         Get all valuations of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
         Returns:
             DataFrame list of statistics
         '''
 
         self.valuations = []
         for statistics in ['Growth', 'Operating and Efficiency', 'Financial Health','Cash Flow']:
-            df = self._get_valuation(ticker, exchange, statistics)
+            df = self._get_valuation(ticker, exchange, statistics, update)
             self.valuations.append(df)
         
         return self.valuations
 
-    def get_income_statement(self, ticker, exchange, period='Annual', stage='Restated'):
+    def get_income_statement(self, ticker, exchange, period='Annual', stage='Restated', update=False):
         '''
         Get income statement of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
             period: Period of statement, which can be 'Annual'(default), 'Quarterly'
             stage: Stage of statement, which can be 'As Originally Reported', 'Restated'(default)
         Returns:
             DataFrame of income statement
         '''
         statement = 'Income Statement'
-        return self._get_financials(ticker, exchange, statement, period, stage)
+        return self._get_financials(ticker, exchange, statement, period, stage, update)
 
-    def get_balance_sheet_statement(self, ticker, exchange, period='Annual', stage='Restated'):
+    def get_balance_sheet_statement(self, ticker, exchange, period='Annual', stage='Restated', update=False):
         '''
         Get balance sheet statement of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
             period: Period of statement, which can be 'Annual'(default), 'Quarterly'
             stage: Stage of statement, which can be 'As Originally Reported', 'Restated'(default)
         Returns:
             DataFrame of balance sheet statement
         '''
         statement = 'Balance Sheet'
-        return self._get_financials(ticker, exchange, statement, period, stage)
+        return self._get_financials(ticker, exchange, statement, period, stage, update)
 
-    def get_cash_flow_statement(self, ticker, exchange, period='Annual', stage='Restated'):
+    def get_cash_flow_statement(self, ticker, exchange, period='Annual', stage='Restated', update=False):
         '''
         Get cash flow statement of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
             period: Period of statement, which can be 'Annual'(default), 'Quarterly'
             stage: Stage of statement, which can be 'As Originally Reported', 'Restated'(default)
         Returns:
             DataFrame of cash flow statement
         '''
         statement = 'Cash Flow'
-        return self._get_financials(ticker, exchange, statement, period, stage)
+        return self._get_financials(ticker, exchange, statement, period, stage, update)
 
-    def get_financials(self, ticker, exchange, period='Annual', stage='As Originally Reported'):
+    def get_financials(self, ticker, exchange, period='Annual', stage='As Originally Reported', update=False):
         '''
         Get all financials statements of stock
         
         Args:
             ticker: Stock symbol
             exchange: Exchange name
             period: Period of statement, which can be 'Annual'(default), 'Quarterly'
             stage: Stage of statement, which can be 'As Originally Reported'(default), 'Restated'
         Returns:
             DataFrame list of financials statements
         '''
 
         self.financials = []
         for statement in ['Income Statement', 'Balance Sheet', 'Cash Flow']:
-            df = self._get_financials(ticker, exchange, statement, period, stage)
+            df = self._get_financials(ticker, exchange, statement, period, stage, update)
             self.financials.append(df)
 
         return self.financials
 
+    def get_hsi_tickers(self):
+        '''
+        Get ticker of Hang Seng Index
+
+        Returns:
+            List of ticker with 5-digital number string
+        ''' 
+        url = "https://en.wikipedia.org/wiki/Hang_Seng_Index"
+        response = requests.get(url, proxies=self.proxies)
+        tables = pd.read_html(response.text)
+        symbols = tables[6]['Ticker'].tolist()
+        pfx_len = len('SEHK:\xa0')
+        symbols = [s[pfx_len:].zfill(5) for s in symbols]
+        return symbols
+
+
     def get_sp500_tickers(self):
         '''
-        Get tickers of sp500
+        Get tickers of SP500
 
         Returns:
             List of ticker names
         '''
         url = "https://en.wikipedia.org/wiki/List_of_S%26P_500_companies"
         response = requests.get(url, proxies=self.proxies)
         tables = pd.read_html(response.text)
         symbols = tables[0]['Symbol'].tolist()
         return symbols
     
-
+    
     def get_xnas_tickers(self):
         '''
         Get tickers of NASDAQ
 
         Returns:
             List of ticker names in NASDAQ
         '''
```

### Comparing `msfinance-0.2.1/msfinance.egg-info/PKG-INFO` & `msfinance-0.2.2/msfinance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfinance
-Version: 0.2.1
+Version: 0.2.2
 Summary: msfinance offers Pythonic way to download stocks financial data from morningstar.com
 Author-email: Jimmy Situ <web@jimmystone.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,39 +237,39 @@
 
 ## Quick Start
 ```python
 #!/usr/bin/python3 -u
 import msfinance as msf
 
 stock = msf.Stock(
-    session='msf_database.sql3',
+    session='msf_database.db3',
 )
 
 
 print(stock.get_income_statement('aapl', 'xnas'))
 print(stock.get_balance_sheet_statement('aapl', 'xnas'))
 print(stock.get_cash_flow_statement('aapl', 'xnas'))
 
 print(stock.get_growth('aapl', 'xnas'))
 print(stock.get_operating_and_efficiency('aapl', 'xnas'))
 print(stock.get_financial_health('aapl', 'xnas'))
 print(stock.get_cash_flow('aapl', 'xnas'))
 ```
-- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory
+- More example is placed in [example](https://github.com/jimmysitu/msfinance/tree/main/example) directory. Add msfinance path to environment variable: PYTHONPATH, and run examples directly 
 
 
 ## US Tickers and Exchanges
 - Get all tickers symbol of each exchange [here](https://www.nasdaq.com/market-activity/stocks/screener)
 
 
 ## HK Tickers and Exchanges
-- TBD
+- Get all tickers numbers of Heng Seng Index [here](https://en.wikipedia.org/wiki/Hang_Seng_Index#Components)
 
 
 ## TODO
 - [x] Add 'Last Updated' to database record
-- [ ] Add docs in docs directory for readthedoc.io
 - [x] Add support for pip package
+- [x] Add tickers from HK exchanges
+- [ ] Add docs in docs directory for readthedoc.io
 - [ ] Add multiprocessing for speed up
 - [ ] More robust error handling
-- [ ] Add tickers from HK exchanges
 - [ ] Add more statistics valuations
```

### Comparing `msfinance-0.2.1/pyproject.toml` & `msfinance-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "msfinance"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "Jimmy Situ", email = "web@jimmystone.com"}
 ]
 description = "msfinance offers Pythonic way to download stocks financial data from morningstar.com"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `msfinance-0.2.1/tests/test_stocks.py` & `msfinance-0.2.2/tests/test_stocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
     tickers_list = {}
     tickers_list['xnas'] = stock.get_xnas_tickers()
     tickers_list['xnys'] = stock.get_xnys_tickers()
     tickers_list['xase'] = stock.get_xase_tickers()
 
     sp500_tickers = stock.get_sp500_tickers()
+    assert 'AAPL' in sp500_tickers
+    
+    hsi_tickers = stock.get_hsi_tickers()
+    assert '00700' in hsi_tickers
 
     # Test method in class Stock
     stage = 'As Originally Reported'
     stock.get_income_statement('aapl', 'xnas', stage=stage)
     stock.get_balance_sheet_statement('aapl', 'xnas', stage=stage)
     stock.get_cash_flow_statement('aapl', 'xnas', stage=stage)
 
@@ -52,16 +56,14 @@
     db = sqlite3.connect(session)
 
     for exchange in ['nasdaq', 'nyse', 'amex']:
         query = f"SELECT * FROM us_exchange_{exchange}_tickers"
         df = pd.read_sql_query(query, db)
         assert df is not None, f"{query} is not found in database"
 
-    assert 'AAPL' in sp500_tickers
-
     stage = 'As Originally Reported'.replace(' ', '_').lower()
     for statement in ['income_statement', 'balance_sheet', 'cash_flow']:
         query = f"SELECT * FROM aapl_xnas_{statement}_annual_{stage}"
         df = pd.read_sql_query(query, db)
         assert df is not None, f"{query} is not found in database"
 
     for statistics in ['growth', 'operating_and_efficiency', 'financial_health','cash_flow']:
```

