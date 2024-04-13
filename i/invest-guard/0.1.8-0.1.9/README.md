# Comparing `tmp/invest-guard-0.1.8.tar.gz` & `tmp/invest-guard-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest-guard-0.1.8.tar", last modified: Sat Apr 13 21:01:31 2024, max compression
+gzip compressed data, was "invest-guard-0.1.9.tar", last modified: Sat Apr 13 21:22:42 2024, max compression
```

## Comparing `invest-guard-0.1.8.tar` & `invest-guard-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:01:31.329910 invest-guard-0.1.8/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 21:01:31.329517 invest-guard-0.1.8/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.8/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:01:31.329033 invest-guard-0.1.8/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       40 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 21:01:31.329980 invest-guard-0.1.8/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1189 2024-04-13 21:01:23.000000 invest-guard-0.1.8/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:22:42.238897 invest-guard-0.1.9/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2595 2024-04-13 21:22:42.238501 invest-guard-0.1.9/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1774 2024-04-13 21:21:28.000000 invest-guard-0.1.9/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:22:42.238014 invest-guard-0.1.9/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2595 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       35 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:22:42.000000 invest-guard-0.1.9/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 21:22:42.238985 invest-guard-0.1.9/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1184 2024-04-13 21:19:46.000000 invest-guard-0.1.9/setup.py
```

### Comparing `invest-guard-0.1.8/PKG-INFO` & `invest-guard-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.8
+Version: 0.1.9
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 ```
 
 ## Usage
 
 To fetch stock data, simply use the `guard fetch` command followed by the appropriate options. For example:
 
 ```bash
-guard fetch --ticker AAPL --start-date 2022-01-01 --end-date 2022-12-31
+guard fetch --asset-type stock --t AAPL --start-date 2022-01-01 --end-date 2022-12-31
 ```
 
 For more information on available commands and options, refer to the [documentation](https://github.com/Work-With-Phoenix/invest-guard).
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Work-With-Phoenix/invest-guard).
```

### Comparing `invest-guard-0.1.8/README.md` & `invest-guard-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 
 ## Usage
 
 To fetch stock data, simply use the `guard fetch` command followed by the appropriate options. For example:
 
 ```bash
-guard fetch --ticker AAPL --start-date 2022-01-01 --end-date 2022-12-31
+guard fetch --asset-type stock --t AAPL --start-date 2022-01-01 --end-date 2022-12-31
 ```
 
 For more information on available commands and options, refer to the [documentation](https://github.com/Work-With-Phoenix/invest-guard).
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Work-With-Phoenix/invest-guard).
```

### Comparing `invest-guard-0.1.8/invest_guard.egg-info/PKG-INFO` & `invest-guard-0.1.9/invest_guard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.8
+Version: 0.1.9
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 ```
 
 ## Usage
 
 To fetch stock data, simply use the `guard fetch` command followed by the appropriate options. For example:
 
 ```bash
-guard fetch --ticker AAPL --start-date 2022-01-01 --end-date 2022-12-31
+guard fetch --asset-type stock --t AAPL --start-date 2022-01-01 --end-date 2022-12-31
 ```
 
 For more information on available commands and options, refer to the [documentation](https://github.com/Work-With-Phoenix/invest-guard).
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Work-With-Phoenix/invest-guard).
```

### Comparing `invest-guard-0.1.8/setup.py` & `invest-guard-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 setup(
     name='invest-guard',
     version=VERSION,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'guard = main:main_run'
+            'guard = main:run'
         ]
     },
     install_requires=[
         'rich',
         'tabulate',
         'yfinance',
         'pandas',
```

