# Comparing `tmp/acctf-0.2.1.tar.gz` & `tmp/acctf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acctf-0.2.1.tar", last modified: Tue Apr  9 13:00:35 2024, max compression
+gzip compressed data, was "acctf-0.3.0.tar", last modified: Sat Apr 13 14:10:13 2024, max compression
```

## Comparing `acctf-0.2.1.tar` & `acctf-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.2.1/LICENSE
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-04-09 13:00:35.975093 acctf-0.2.1/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3085 2024-04-06 13:38:11.000000 acctf-0.2.1/README.md
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      819 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      680 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/mizuho/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     5583 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/mizuho/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.2.1/acctf/bank/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     7948 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/sbi/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/other/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/other/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/other/wealthnavi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2180 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/other/wealthnavi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/other/wealthnavi/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/securities/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      799 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/securities/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/securities/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/securities/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3941 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/securities/sbi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/securities/sbi/utils.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/acctf/utils/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/utils/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.2.1/acctf/utils/format.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.2.1/acctf/utils/totp.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/acctf.egg-info/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/SOURCES.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/dependency_links.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/requires.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/top_level.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-09 13:00:35.975093 acctf-0.2.1/setup.cfg
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      940 2024-04-09 12:57:35.000000 acctf-0.2.1/setup.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.238694 acctf-0.3.0/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.3.0/LICENSE
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-13 14:10:13.238694 acctf-0.3.0/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4021 2024-04-13 14:09:09.000000 acctf-0.3.0/README.md
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.218694 acctf-0.3.0/acctf/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      471 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.228694 acctf-0.3.0/acctf/bank/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      691 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/bank/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.228694 acctf-0.3.0/acctf/bank/mizuho/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     5593 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/bank/mizuho/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.3.0/acctf/bank/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.228694 acctf-0.3.0/acctf/bank/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     7948 2024-04-09 12:55:27.000000 acctf-0.3.0/acctf/bank/sbi/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.228694 acctf-0.3.0/acctf/other/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.3.0/acctf/other/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.228694 acctf-0.3.0/acctf/other/wealthnavi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2190 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/other/wealthnavi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.3.0/acctf/other/wealthnavi/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.238694 acctf-0.3.0/acctf/securities/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      810 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/securities/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.3.0/acctf/securities/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.238694 acctf-0.3.0/acctf/securities/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3951 2024-04-13 14:09:09.000000 acctf-0.3.0/acctf/securities/sbi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.3.0/acctf/securities/sbi/utils.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.238694 acctf-0.3.0/acctf/utils/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.3.0/acctf/utils/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.3.0/acctf/utils/format.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.3.0/acctf/utils/totp.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 14:10:13.238694 acctf-0.3.0/acctf.egg-info/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-13 14:10:13.000000 acctf-0.3.0/acctf.egg-info/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-04-13 14:10:13.000000 acctf-0.3.0/acctf.egg-info/SOURCES.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-04-13 14:10:13.000000 acctf-0.3.0/acctf.egg-info/dependency_links.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       63 2024-04-13 14:10:13.000000 acctf-0.3.0/acctf.egg-info/requires.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-04-13 14:10:13.000000 acctf-0.3.0/acctf.egg-info/top_level.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-13 14:10:13.238694 acctf-0.3.0/setup.cfg
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      929 2024-04-13 14:09:09.000000 acctf-0.3.0/setup.py
```

### Comparing `acctf-0.2.1/LICENSE` & `acctf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acctf-0.2.1/PKG-INFO` & `acctf-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.2.1
+Version: 0.3.0
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: bs4
-Requires-Dist: chromedriver-binary
 Requires-Dist: selenium
 Requires-Dist: pandas
 Requires-Dist: lxml
 Requires-Dist: PySocks
 Requires-Dist: pyotp
+Requires-Dist: html5lib
 
 # acctf
 
 ### English | [日本語](https://github.com/hirano00o/acctf/blob/main/README.ja.md)
 
 This is a library that obtains deposit/withdrawal history, price and quantity of held stocks from bank and securities accounts.
 
@@ -62,16 +62,23 @@
 
 ## Example
 
 ### Securities
 
 ```python
 from acctf.securities.sbi import SBI
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
-sbi = SBI().login("<ユーザID>", "<パスワード>")
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
+
+sbi = SBI(driver=driver).login("<ユーザID>", "<パスワード>")
 stocks = sbi.get_stock_specific()
 print("銘柄, 数量, 取得単価, 現在値")
 for s in stocks:
   print(f"{s.name}, {s.amount}, {s.acquisition_value}, {s.current_value}")
 
 sbi.logout()
 sbi.close()
@@ -86,16 +93,23 @@
 
 ### Bank
 
 #### Balance
 
 ```python
 from acctf.bank.mizuho import Mizuho
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
 
-mizuho = Mizuho().login("<ユーザID>", "<パスワード>")
+mizuho = Mizuho(driver=driver).login("<ユーザID>", "<パスワード>")
 b = mizuho.get_balance("7654321")
 print(f"口座番号, 店舗, 残高, 口座タイプ")
 print(f"{b[0].account_number}, {b[0].branch_name}, {b[0].value}, {b[0].deposit_type}")
 
 mizuho.logout()
 mizuho.close()
 ```
@@ -105,16 +119,23 @@
 7654321, 本店, 1234567.0, DepositType.ordinary
 ```
 
 #### Transaction history
 
 ```python
 from acctf.bank.mizuho import Mizuho
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
-mizuho = Mizuho().login("<ユーザID>", "<パスワード>")
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
+
+mizuho = Mizuho(driver=driver).login("<ユーザID>", "<パスワード>")
 hist = mizuho.get_transaction_history("7654321")
 # You can also specify the start/end date.
 # hist = mizuho.get_transaction_history("7654321", date(2023, 12, 1), date(2023, 12, 31))
 print(f"日付, 取引内容, 金額")
 for h in hist:
   print(f"{h.date}, {h.content}, {h.value}")
 
@@ -130,16 +151,23 @@
 
 ### Other
 
 #### WealthNavi
 
 ```python
 from acctf.other.wealthnavi import WealthNavi
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
 
-w = WealthNavi().login("<ユーザID>", "<パスワード>", "<TOTP>")
+w = WealthNavi(driver=driver).login("<ユーザID>", "<パスワード>", "<TOTP>")
 # If you don't set the Time-based One Time Password
 # w = WealthNavi().login("<ユーザID>", "<パスワード>")
 print("資産クラス, 現在価格, 損益")
 for h in w.get_valuation():
   print(f"{h.name}, {h.value}, {h.pl_value}")
 
 w.logout()
```

### Comparing `acctf-0.2.1/acctf/bank/__init__.py` & `acctf-0.3.0/acctf/bank/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from datetime import date
 from abc import ABCMeta, abstractmethod
 
+from selenium import webdriver
+
 from acctf.bank.model import Transaction, Balance, CurrencyType
 from acctf import Base
 
 
 class Bank(Base, metaclass=ABCMeta):
-    def __init__(self, executable_path: str = None):
-        super().__init__(executable_path=executable_path)
+    def __init__(self, driver: webdriver = None):
+        super().__init__(driver=driver)
 
     @abstractmethod
     def get_balance(self, account_number: str) -> list[Balance]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_transaction_history(
```

### Comparing `acctf-0.2.1/acctf/bank/mizuho/__init__.py` & `acctf-0.3.0/acctf/bank/mizuho/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from abc import ABC
 from datetime import date, datetime
 from io import StringIO
 
 import pandas as pd
 from bs4 import BeautifulSoup
 from dateutil.relativedelta import relativedelta
+from selenium import webdriver
 from selenium.common import NoSuchElementException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.select import Select
 
 from acctf.bank import Bank, Balance, Transaction
 from acctf.bank.model import str_to_deposit_type, CurrencyType
 
 
 class Mizuho(Bank, ABC):
-    def __init__(self, executable_path: str = None):
-        super().__init__(executable_path=executable_path)
+    def __init__(self, driver: webdriver = None):
+        super().__init__(driver=driver)
         self.driver.get('https://web.ib.mizuhobank.co.jp/servlet/LOGBNK0000000B.do')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.NAME, 'txbCustNo')
         user_id_elem.send_keys(user_id)
         self.driver.find_element(By.NAME, 'N00000-next').click()
```

### Comparing `acctf-0.2.1/acctf/bank/model.py` & `acctf-0.3.0/acctf/bank/model.py`

 * *Files identical despite different names*

### Comparing `acctf-0.2.1/acctf/bank/sbi/__init__.py` & `acctf-0.3.0/acctf/bank/sbi/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.2.1/acctf/other/wealthnavi/__init__.py` & `acctf-0.3.0/acctf/other/wealthnavi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from io import StringIO
 
 import pandas as pd
 from bs4 import BeautifulSoup
+from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 from acctf import Base
 from acctf.other.wealthnavi.model import Asset
 from acctf.utils.format import format_displayed_money
 from acctf.utils.totp import get_code
 
 
 class WealthNavi(Base):
-    def __init__(self, executable_path: str = None):
-        super().__init__(executable_path=executable_path)
+    def __init__(self, driver: webdriver = None):
+        super().__init__(driver=driver)
         self.driver.get('https://invest.wealthnavi.com/login')
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.ID, 'username')
         user_id_elem.send_keys(user_id)
 
         user_pw_elem = self.driver.find_element(By.ID, 'password')
```

### Comparing `acctf-0.2.1/acctf/securities/__init__.py` & `acctf-0.3.0/acctf/securities/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from abc import ABCMeta, abstractmethod
 
+from selenium import webdriver
+
 from acctf import Base
 from acctf.securities.model import Value
 
 
 class Securities(Base, metaclass=ABCMeta):
-    def __init__(self, executable_path: str = None):
-        super().__init__(executable_path=executable_path)
+    def __init__(self, driver: webdriver = None):
+        super().__init__(driver=driver)
 
     @abstractmethod
     def get_stock_specific(self) -> list[Value]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_stock_specific_us(self) -> list[Value]:
```

### Comparing `acctf-0.2.1/acctf/securities/sbi/__init__.py` & `acctf-0.3.0/acctf/securities/sbi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from abc import ABC
 from io import StringIO
 
 import pandas as pd
 from bs4 import BeautifulSoup
+from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 from acctf.securities import Securities
 from acctf.securities.model import Value
 from acctf.securities.sbi.utils import get_formatted, AccountType
 
 
 class SBI(Securities, ABC):
     _df_fund_specific: pd.DataFrame = None
     _df_fund_nisa_accum: pd.DataFrame = None
     _df_fund_old_nisa_accum: pd.DataFrame = None
 
-    def __init__(self, executable_path: str = None):
-        super().__init__(executable_path=executable_path)
+    def __init__(self, driver: webdriver = None):
+        super().__init__(driver=driver)
         self.driver.get('https://www.sbisec.co.jp/ETGate')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.NAME, 'user_id')
         user_id_elem.send_keys(user_id)
         user_pw_elem = self.driver.find_element(By.NAME, 'user_password')
```

### Comparing `acctf-0.2.1/acctf/securities/sbi/utils.py` & `acctf-0.3.0/acctf/securities/sbi/utils.py`

 * *Files identical despite different names*

### Comparing `acctf-0.2.1/acctf.egg-info/PKG-INFO` & `acctf-0.3.0/acctf.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.2.1
+Version: 0.3.0
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: bs4
-Requires-Dist: chromedriver-binary
 Requires-Dist: selenium
 Requires-Dist: pandas
 Requires-Dist: lxml
 Requires-Dist: PySocks
 Requires-Dist: pyotp
+Requires-Dist: html5lib
 
 # acctf
 
 ### English | [日本語](https://github.com/hirano00o/acctf/blob/main/README.ja.md)
 
 This is a library that obtains deposit/withdrawal history, price and quantity of held stocks from bank and securities accounts.
 
@@ -62,16 +62,23 @@
 
 ## Example
 
 ### Securities
 
 ```python
 from acctf.securities.sbi import SBI
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
-sbi = SBI().login("<ユーザID>", "<パスワード>")
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
+
+sbi = SBI(driver=driver).login("<ユーザID>", "<パスワード>")
 stocks = sbi.get_stock_specific()
 print("銘柄, 数量, 取得単価, 現在値")
 for s in stocks:
   print(f"{s.name}, {s.amount}, {s.acquisition_value}, {s.current_value}")
 
 sbi.logout()
 sbi.close()
@@ -86,16 +93,23 @@
 
 ### Bank
 
 #### Balance
 
 ```python
 from acctf.bank.mizuho import Mizuho
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
 
-mizuho = Mizuho().login("<ユーザID>", "<パスワード>")
+mizuho = Mizuho(driver=driver).login("<ユーザID>", "<パスワード>")
 b = mizuho.get_balance("7654321")
 print(f"口座番号, 店舗, 残高, 口座タイプ")
 print(f"{b[0].account_number}, {b[0].branch_name}, {b[0].value}, {b[0].deposit_type}")
 
 mizuho.logout()
 mizuho.close()
 ```
@@ -105,16 +119,23 @@
 7654321, 本店, 1234567.0, DepositType.ordinary
 ```
 
 #### Transaction history
 
 ```python
 from acctf.bank.mizuho import Mizuho
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
-mizuho = Mizuho().login("<ユーザID>", "<パスワード>")
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
+
+mizuho = Mizuho(driver=driver).login("<ユーザID>", "<パスワード>")
 hist = mizuho.get_transaction_history("7654321")
 # You can also specify the start/end date.
 # hist = mizuho.get_transaction_history("7654321", date(2023, 12, 1), date(2023, 12, 31))
 print(f"日付, 取引内容, 金額")
 for h in hist:
   print(f"{h.date}, {h.content}, {h.value}")
 
@@ -130,16 +151,23 @@
 
 ### Other
 
 #### WealthNavi
 
 ```python
 from acctf.other.wealthnavi import WealthNavi
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+
+options = Options()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+driver = webdriver.Chrome(options=options)
 
-w = WealthNavi().login("<ユーザID>", "<パスワード>", "<TOTP>")
+w = WealthNavi(driver=driver).login("<ユーザID>", "<パスワード>", "<TOTP>")
 # If you don't set the Time-based One Time Password
 # w = WealthNavi().login("<ユーザID>", "<パスワード>")
 print("資産クラス, 現在価格, 損益")
 for h in w.get_valuation():
   print(f"{h.name}, {h.value}, {h.pl_value}")
 
 w.logout()
```

### Comparing `acctf-0.2.1/acctf.egg-info/SOURCES.txt` & `acctf-0.3.0/acctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acctf-0.2.1/setup.py` & `acctf-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="acctf",
-    version="0.2.1",
+    version="0.3.0",
     description="library that scrapes the data from an account such as securities, bank",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hirano00o/acctf",
     author="hirano00o",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -19,16 +19,16 @@
         "Operating System :: OS Independent",
     ],
     keywords="scrape, account, development",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4",
         "bs4",
-        "chromedriver-binary",
         "selenium",
         "pandas",
         "lxml",
         "PySocks",
         "pyotp",
+        "html5lib",
     ],
     python_requires='>=3.11',
 )
```

