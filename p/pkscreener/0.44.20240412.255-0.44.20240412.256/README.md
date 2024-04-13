# Comparing `tmp/pkscreener-0.44.20240412.255.tar.gz` & `tmp/pkscreener-0.44.20240412.256.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240412.255.tar", last modified: Fri Apr 12 10:16:27 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240412.256.tar", last modified: Fri Apr 12 23:32:24 2024, max compression
```

## Comparing `pkscreener-0.44.20240412.255.tar` & `pkscreener-0.44.20240412.256.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/
--rw-rw-rw-   0        0        0     1086 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.351607 pkscreener-0.44.20240412.255/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27550 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    17278 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   108935 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44525 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77670 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-12 10:16:19.000000 pkscreener-0.44.20240412.255/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   111236 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18397 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:32:24.686976 pkscreener-0.44.20240412.256/
+-rw-rw-rw-   0        0        0     1086 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-12 23:32:24.686976 pkscreener-0.44.20240412.256/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 23:32:24.671351 pkscreener-0.44.20240412.256/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:32:24.686976 pkscreener-0.44.20240412.256/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27550 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20761 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   110553 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77670 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-12 23:32:16.000000 pkscreener-0.44.20240412.256/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   111295 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18495 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:32:24.671351 pkscreener-0.44.20240412.256/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-12 23:32:24.000000 pkscreener-0.44.20240412.256/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-12 23:32:24.686976 pkscreener-0.44.20240412.256/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-12 23:28:25.000000 pkscreener-0.44.20240412.256/setup.py
```

### Comparing `pkscreener-0.44.20240412.255/LICENSE` & `pkscreener-0.44.20240412.256/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/LICENSE-Others` & `pkscreener-0.44.20240412.256/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/PKG-INFO` & `pkscreener-0.44.20240412.256/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240412.255
+Version: 0.44.20240412.256
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.255.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.256.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.255/README.md` & `pkscreener-0.44.20240412.256/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener/__init__.py` & `pkscreener-0.44.20240412.256/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import datetime
 import sys
 import os
 import numpy as np
 import pandas as pd
 import pkscreener.classes.Utility as Utility
 from pkscreener.classes.ConfigManager import parser, tools
+from pkscreener.classes.ScreeningStatistics import ScreeningStatistics
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.PKPickler import PKPicklerDB
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
 STD_ENCODING=sys.stdout.encoding if sys.stdout is not None else 'utf-8'
@@ -63,14 +64,15 @@
 
 
 class PKMarketOpenCloseAnalyser:
     configManager = tools()
     configManager.getConfig(parser)
     updatedCandleData = None
     allDailyCandles = None
+    allIntradayCandles = None
     def getStockDataForSimulation():
         int_exists, int_cache_file = PKMarketOpenCloseAnalyser.ensureIntradayStockDataExists()
         daily_exists, daily_cache_file = PKMarketOpenCloseAnalyser.ensureDailyStockDataExists()
         updatedCandleData = PKMarketOpenCloseAnalyser.updatedCandleData
         allDailyCandles = PKMarketOpenCloseAnalyser.allDailyCandles
         if  (int_exists and daily_exists) and (updatedCandleData is None or allDailyCandles is None):
             allDailyCandles = PKMarketOpenCloseAnalyser.getLatestDailyCandleData(daily_cache_file)
@@ -81,15 +83,15 @@
             Utility.tools.saveStockData(updatedCandleData,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
         return updatedCandleData, allDailyCandles
 
     def runOpenCloseAnalysis(updatedCandleData,allDailyCandles,screen_df,save_df,runOptionName=None):
         # stockListFromMorningTrade,morningIntraday_df = PKMarketOpenCloseAnalyser.simulateMorningTrade(updatedCandleData)
         # latest_daily_df = PKMarketOpenCloseAnalyser.runScanForStocksFromMorningTrade(stockListFromMorningTrade,allDailyCandles)
         try:
-            PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, allDailyCandles,runOptionName=runOptionName)
+            PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=runOptionName)
         except:
             pass
         Utility.tools.saveStockData(allDailyCandles,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
 
     def ensureIntradayStockDataExists():
         # Ensure that the intraday_stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
@@ -156,14 +158,15 @@
         #         continue
         return allDailyCandles
     
     def getIntradayCandleFromMorning(int_cache_file):
         morningIntradayCandle = None
         intradayDB = PKIntradayStockDataDB(fileName=int_cache_file)
         allDailyIntradayCandles = intradayDB.pickler.pickler.unpickle(fileName=intradayDB.pickler.fileName)
+        PKMarketOpenCloseAnalyser.allIntradayCandles = allDailyIntradayCandles
         morningIntradayCandle = {}
         stocks = list(allDailyIntradayCandles.keys())
         numOfCandles = PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber
         duration = PKMarketOpenCloseAnalyser.configManager.morninganalysiscandleduration
         numOfCandles = numOfCandles * int(duration.replace("m",""))
         for stock in stocks:
             try:
@@ -173,21 +176,25 @@
                 # We'd then combine the data from 9:15 to 9:57 as a single candle of 
                 # OHLCV and replace the last daily candle with this one candle to
                 # simulate the scan outcome from morning.
                 df = pd.DataFrame(data=allDailyIntradayCandles[stock]["data"],
                                 columns=allDailyIntradayCandles[stock]["columns"],
                                 index=allDailyIntradayCandles[stock]["index"])
                 df = df.head(numOfCandles)
-                df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+                try:
+                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+                except:
+                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
+                    pass
                 if df is not None and len(df) > 0:
                     combinedCandle = {"Open":PKMarketOpenCloseAnalyser.getMorningOpen(df), "High":max(df["High"]), 
                                     "Low":min(df["Low"]),"Close":PKMarketOpenCloseAnalyser.getMorningClose(df),
                                     "Adj Close":df["Adj Close"][-1],"Volume":sum(df["Volume"])}
-                    tradingDate = PKDateUtilities.tradingDate()
-                    timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d hh:mm:ss"),"%Y-%m-%d hh:mm:ss")
+                    tradingDate = df.index[-1] #PKDateUtilities.tradingDate()
+                    timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d %H:%M:%S"),"%Y-%m-%d %H:%M:%S")
                     df = pd.DataFrame([combinedCandle], columns=df.columns, index=[timestamp])
                     morningIntradayCandle[stock] = df.to_dict("split")
             except Exception as e:
                 print(f"{stock}:    {e}")
                 continue
         return morningIntradayCandle
 
@@ -246,52 +253,92 @@
                 continue
         return mutableAllDailyCandles
 
     def runScanForStocksFromMorningTrade(stockListFromMorningTrade,dailyCandleData):
         latest_daily_df = None
         return latest_daily_df
 
-    def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, allDailyCandles,runOptionName=None):
+    def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, updatedCandleData, allDailyCandles,runOptionName=None):
         save_df.reset_index(inplace=True)
         screen_df.reset_index(inplace=True)
+        save_df.drop(f"index", axis=1, inplace=True, errors="ignore")
+        screen_df.drop(f"index", axis=1, inplace=True, errors="ignore")
         stocks = save_df["Stock"]
         eodLTPs = []
-        diff = []
+        morningTimestamps = []
+        sellTimestamps = []
+        sellLTPs = []
+        eodDiffs = []
+        sqrOffDiffs = []
         index = 0
+        scrStats = ScreeningStatistics(PKMarketOpenCloseAnalyser.configManager, default_logger())
         for stock in stocks:
             try:
                 # Open, High, Low, Close, Adj Close, Volume. We need the 3rd index item: Close.
                 endOfDayLTP = allDailyCandles[stock]["data"][-1][3]
-                morningLTP = round(save_df["LTP"][index],2)
+                morningLTP = updatedCandleData[stock]["data"][-1][3] #round(save_df["LTP"][index],2)
+                morningTime = updatedCandleData[stock]["index"][-1].strftime("%H:%M")
+                morningTimestamps.append(morningTime)
+                morningCandles = PKMarketOpenCloseAnalyser.allIntradayCandles
+                df = pd.DataFrame(data=morningCandles[stock]["data"],
+                                columns=morningCandles[stock]["columns"],
+                                index=morningCandles[stock]["index"])
+                # try:
+                #     # Let's only consider those candles that are after the alert issue-time in the mornings
+                #     df = df[df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+                # except:
+                #     df = df[df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
+                #     pass
+                ts, row = scrStats.findMACDCrossover(df=df,
+                                           afterTimestamp=updatedCandleData[stock]["index"][-1],
+                                           nthCrossover=1,
+                                           upDirection=True)
+                sellTimestamps.append(ts.strftime("%H:%M"))
+                sellLTPs.append(row["High"][-1])
                 eodLTPs.append(round(endOfDayLTP,2))
-                diff.append(round(endOfDayLTP - morningLTP,2))
+                eodDiffs.append(round(endOfDayLTP - morningLTP,2))
+                sqrOffDiffs.append(round(row["High"][-1] - morningLTP,2))
                 index += 1
             except:
                 eodLTPs.append("0")
-                diff.append("0")
+                eodDiffs.append("0")
                 continue
+        save_df["AlertTime"] = morningTimestamps
+        screen_df["AlertTime"] = morningTimestamps
+        save_df["SqrOffLTP"] = sellLTPs
+        screen_df["SqrOffLTP"] = sellLTPs
+        save_df["SqrOff"] = sellTimestamps
+        screen_df["SqrOff"] = sellTimestamps
+        screen_df["SqrOffDiff"] = sqrOffDiffs
+        save_df["SqrOffDiff"] = sqrOffDiffs
         save_df["EoDLTP"] = eodLTPs
         screen_df["EoDLTP"] = eodLTPs
-        save_df["Diff"] = diff
-        screen_df["Diff"] = diff
+        save_df["EoDDiff"] = eodDiffs
+        screen_df["EoDDiff"] = eodDiffs
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
-            if col in ["Stock", "Pattern", "LTP", "EoDLTP", "Diff", "%Chng"]:
+            if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
                 if col == "Stock":
                     save_df.loc[lastIndex,col] = "PORTFOLIO"
                 elif col == "Pattern":
                     save_df.loc[lastIndex,col] = runOptionName if runOptionName is not None else ""
-                elif col in ["LTP","EoDLTP", "Diff"]:
+                elif col in ["LTP", "SqrOffLTP","SqrOffDiff", "EoDLTP", "EoDDiff"]:
                     save_df.loc[lastIndex,col] = round(sum(save_df[col].dropna(inplace=False).astype(float)),2)
                 elif col == "%Chng":
-                    change_pct = sum(save_df["Diff"].dropna(inplace=False).astype(float))*100/sum(save_df["LTP"].dropna(inplace=False).astype(float))
-                    save_df.loc[lastIndex,col] = round(2*change_pct,2) # when summing above for LTP, the total of LTP gets summed up too. Hence *2 here.
+                    ltpSum = sum(save_df["LTP"].dropna(inplace=False).astype(float))
+                    change_pct = sum(save_df["EoDDiff"].dropna(inplace=False).astype(float))*100/ltpSum
+                    save_df.loc[lastIndex,col] = f"{round(2*change_pct,2)}%" # when summing above for LTP, the total of LTP gets summed up too. Hence *2 here.
             else:
                 save_df.loc[lastIndex,col] = ""
             screen_df.loc[lastIndex,col] = save_df.loc[lastIndex,col]
+        save_df.loc[lastIndex,"EoDDiff"] = str(save_df.loc[lastIndex,"EoDDiff"]) + f'({round(100*2*save_df.loc[lastIndex,"EoDDiff"]/ltpSum,2)}%)'
+        save_df.loc[lastIndex,"SqrOffDiff"] = str(save_df.loc[lastIndex,"SqrOffDiff"]) + f'({round(100*2*save_df.loc[lastIndex,"SqrOffDiff"]/ltpSum,2)}%)'
+        screen_df.loc[lastIndex,"EoDDiff"] = save_df.loc[lastIndex,"EoDDiff"]
+        screen_df.loc[lastIndex,"SqrOffDiff"] = save_df.loc[lastIndex,"SqrOffDiff"]
         save_df.set_index("Stock", inplace=True)
         screen_df.set_index("Stock", inplace=True)
+        PKMarketOpenCloseAnalyser.allIntradayCandles = None
         if 'index' in save_df.columns:
             save_df.drop('index', axis=1, inplace=True, errors="ignore")
         if 'index' in screen_df.columns:
             screen_df.drop('index', axis=1, inplace=True, errors="ignore")
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Pktalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         except Exception:  # pragma: no cover
             # default_logger().debug(e, exc_info=True)
             return talib.MA(close, timeperiod)
 
     @classmethod
     def MACD(self, close, fast, slow, signal):
         try:
+            # import pandas_ta as talib
             return talib.macd(close, fast, slow, signal, talib=Imports["talib"])
         except Exception:  # pragma: no cover
             # default_logger().debug(e, exc_info=True)
             return talib.MACD(close, fast, slow, signal)
 
     @classmethod
     def RSI(self, close, timeperiod):
@@ -152,14 +153,24 @@
             data = {
                 aroon_down.name: aroon_down,
                 aroon_up.name: aroon_up,
             }
             return pd.DataFrame(data)
 
     @classmethod
+    def STOCHF(self, high, low, close, fastk_period, fastd_period, fastd_matype):
+        fastk, fastd = talib.STOCHF(high,
+                            low,
+                            close,
+                            fastk_period, 
+                            fastd_period,
+                            fastd_matype)
+        return fastk, fastd
+    
+    @classmethod
     def STOCHRSI(self, close, timeperiod, fastk_period, fastd_period, fastd_matype):
         try:
             _name = "STOCHRSI"
             _props = f"_{timeperiod}_{timeperiod}_{fastk_period}_{fastd_period}"
             stochrsi_kname = f"{_name}k{_props}"
             stochrsi_dname = f"{_name}d{_props}"
             df = talib.stochrsi(
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,14 +651,42 @@
             if filter not in [2,4]: # SqZ/All
                 return False
             screenDict["Pattern"] = f'{saved[0]}{colorText.BOLD}{colorText.WARN}TTM-SQZ{colorText.END}'
             saveDict["Pattern"] = f'{saved[1]}TTM-SQZ'
             return True
         return False
 
+    def findMACDCrossover(self, df, afterTimestamp=None, nthCrossover=1, upDirection=True):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        data = data[::-1]  # Reverse the dataframe so that its the oldest date first
+        macdLine, macdSignal, macdHist = pktalib.MACD(data["Close"], 12, 26, 9)
+        line_df = pd.DataFrame(macdLine)
+        signal_df = pd.DataFrame(macdSignal)
+        diff_df = pd.concat([line_df, signal_df, signal_df-line_df], axis=1)
+        diff_df.columns = ["line","signal","diff"]
+        try:
+            # Let's only consider those candles that are after the alert issue-time in the mornings
+            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+        except:
+            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
+            pass
+        index = len(diff_df)
+        if diff_df["diff"][-1] < 0:
+            while(diff_df["diff"][index-1] < 0 and index >=0):
+                index -= 1
+        else:
+            while(diff_df["diff"][index-1] >= 0 and index >=0):
+                index -= 1
+        ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
+        return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
+    
     # Find stocks with rising RSI from lower levels
     def findRisingRSI(self, df):
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
         dayMinus2RSI = data["RSI"].iloc[0]
         dayMinus1RSI = data["RSI"].iloc[1]
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/classes/keys.py` & `pkscreener-0.44.20240412.256/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/courbd.ttf` & `pkscreener-0.44.20240412.256/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/globals.py` & `pkscreener-0.44.20240412.256/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1701,15 +1701,15 @@
                 if saveResultsTrimmed is not None and len(saveResultsTrimmed) > 0:
                     markdown_results = colorText.miniTabulator().tabulate(
                         saveResultsTrimmed,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=Utility.tools.getMaxColumnWidths(saveResultsTrimmed)
                     ).encode("utf-8").decode(STD_ENCODING)
-                if not testing:
+                if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
                         pngName,
@@ -1812,22 +1812,22 @@
 def removedUnusedColumns(screenResults, saveResults, dropAdditionalColumns=[], userArgs=None):
     periods = configManager.periodsRange
     if userArgs is not None and userArgs.backtestdaysago is not None and int(userArgs.backtestdaysago) < 22:
         dropAdditionalColumns.append("22-Pd %")
     summaryReturns = ("w.r.t. " + saveResults["Date"].iloc[0]) if "Date" in saveResults.columns else ""
     for period in periods:
         if saveResults is not None:
-            if f"LTP{period}" in saveResults.columns and "MCapWt%" in saveResults.columns:
-                pdLTP = saveResults[f"LTP{period}"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
-                mktWeight = saveResults["MCapWt%"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
-                ltp = saveResults[f"LTP"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
-                pdReturn = round(100*(sum(pdLTP * mktWeight)-sum(ltp * mktWeight))/sum(ltp * mktWeight),1)
-                          #round((sum(saveResults[f"LTP{period}"]) - sum(saveResults['LTP']))*100/sum(saveResults['LTP']),1)
-                if pdReturn > -500:
-                    summaryReturns = f"{period}-Pd({pdReturn} %), {summaryReturns}"
+            # if f"LTP{period}" in saveResults.columns and "MCapWt%" in saveResults.columns:
+            #     pdLTP = saveResults[f"LTP{period}"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            #     mktWeight = saveResults["MCapWt%"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            #     ltp = saveResults[f"LTP"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            #     pdReturn = round(100*(sum(pdLTP * mktWeight)-sum(ltp * mktWeight))/sum(ltp * mktWeight),1)
+            #               #round((sum(saveResults[f"LTP{period}"]) - sum(saveResults['LTP']))*100/sum(saveResults['LTP']),1)
+            #     if pdReturn > -500:
+            #         summaryReturns = f"{period}-Pd({pdReturn} %), {summaryReturns}"
             saveResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             saveResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
             saveResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
             screenResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
             if len(dropAdditionalColumns) > 0:
                 for col in dropAdditionalColumns:
                     if col in saveResults.columns:
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240412.256/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240412.256/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240412.256/pkscreener/pkscreenercli.py`

 * *Files 3% similar despite different names*

```diff
@@ -299,17 +299,17 @@
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
                     if final_df is None:
-                        final_df = df_group[["Pattern","LTP","EoDLTP","Diff","%Chng"]]
+                        final_df = df_group[["Pattern","LTP","AlertTime","SqrOffLTP","SqrOff","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]
                     else:
-                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","EoDLTP","Diff","%Chng"]]], axis=0)
+                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","AlertTime","SqrOffLTP","SqrOff","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]], axis=0)
             mark_down = colorText.miniTabulator().tabulate(
                                 final_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 showindex = False
                             ).encode("utf-8").decode(Utility.STD_ENCODING)
             print(mark_down)
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240412.256/pkscreener.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240412.255
+Version: 0.44.20240412.256
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.255.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.256.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.255/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.255/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240412.256/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.255/setup.py` & `pkscreener-0.44.20240412.256/setup.py`

 * *Files identical despite different names*

