# Comparing `tmp/deribit_wrapper-0.3.0.tar.gz` & `tmp/deribit_wrapper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.3.0.tar", last modified: Fri Apr  5 18:05:37 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.3.1.tar", last modified: Sat Apr 13 10:35:02 2024, max compression
```

## Comparing `deribit_wrapper-0.3.0.tar` & `deribit_wrapper-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 18:05:37.000000 deribit_wrapper-0.3.0/deribit_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.653102 deribit_wrapper-0.3.0/dev_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/config_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/debug_account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/debug_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/dev_scripts/utilities_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:37.657101 deribit_wrapper-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-05 18:05:31.000000 deribit_wrapper-0.3.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:35:02.384095 deribit_wrapper-0.3.1/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-13 10:35:02.000000 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-13 10:35:02.000000 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:35:02.000000 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 10:35:02.000000 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 10:35:02.000000 deribit_wrapper-0.3.1/deribit_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/config_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/debug_account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/debug_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/debug_market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/dev_scripts/utilities_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:35:02.388095 deribit_wrapper-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 10:34:55.000000 deribit_wrapper-0.3.1/tests/test_base.py
```

### Comparing `deribit_wrapper-0.3.0/LICENSE` & `deribit_wrapper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/PKG-INFO` & `deribit_wrapper-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.3.0/README.md` & `deribit_wrapper-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/account_management.py` & `deribit_wrapper-0.3.1/deribit_wrapper/account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/authentication.py` & `deribit_wrapper-0.3.1/deribit_wrapper/authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/base.py` & `deribit_wrapper-0.3.1/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/core.py` & `deribit_wrapper-0.3.1/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/market_data.py` & `deribit_wrapper-0.3.1/deribit_wrapper/market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 def name_instrument(currency: str, expiry: DatetimeType, strike: StrikeType = None, opt_type: str = None) -> str:
     c = currency
     t = pd.to_datetime(expiry).strftime('%e%b%y').strip()
     if strike is None or opt_type is None:
         name = '{c}-{t}'
         name = name.format(c=c, t=t)
     else:
-        k = int(strike)
+        k = float(strike)
+        k = int(k) if k.is_integer() else k
         ot = 'c' if opt_type == 'call' else 'p'
         name = '{c}-{t}-{k:d}-{ot}'
         name = name.format(c=c, t=t, k=k, ot=ot)
     name = name.upper()
     return name
```

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/trading.py` & `deribit_wrapper-0.3.1/deribit_wrapper/trading.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper/utilities.py` & `deribit_wrapper-0.3.1/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.3.1/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.3.0/deribit_wrapper.egg-info/SOURCES.txt` & `deribit_wrapper-0.3.1/deribit_wrapper.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 deribit_wrapper.egg-info/dependency_links.txt
 deribit_wrapper.egg-info/requires.txt
 deribit_wrapper.egg-info/top_level.txt
 dev_scripts/__init__.py
 dev_scripts/config_dev.py
 dev_scripts/debug_account_management.py
 dev_scripts/debug_authentication.py
+dev_scripts/debug_market_data.py
 dev_scripts/utilities_dev.py
 tests/__init__.py
 tests/conftest.py
 tests/test_authentication.py
 tests/test_base.py
```

### Comparing `deribit_wrapper-0.3.0/dev_scripts/debug_account_management.py` & `deribit_wrapper-0.3.1/dev_scripts/debug_account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/dev_scripts/debug_authentication.py` & `deribit_wrapper-0.3.1/dev_scripts/debug_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/dev_scripts/utilities_dev.py` & `deribit_wrapper-0.3.1/dev_scripts/utilities_dev.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/setup.py` & `deribit_wrapper-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

### Comparing `deribit_wrapper-0.3.0/tests/test_authentication.py` & `deribit_wrapper-0.3.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.3.0/tests/test_base.py` & `deribit_wrapper-0.3.1/tests/test_base.py`

 * *Files identical despite different names*

