# Comparing `tmp/pkscreener-0.44.20240412.254.tar.gz` & `tmp/pkscreener-0.44.20240412.255.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240412.254.tar", last modified: Fri Apr 12 00:44:40 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240412.255.tar", last modified: Fri Apr 12 10:16:27 2024, max compression
```

## Comparing `pkscreener-0.44.20240412.254.tar` & `pkscreener-0.44.20240412.255.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/
--rw-rw-rw-   0        0        0     1086 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.964645 pkscreener-0.44.20240412.254/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27550 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    17214 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   108935 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44525 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77670 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-12 00:44:31.000000 pkscreener-0.44.20240412.254/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   111068 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18397 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.964645 pkscreener-0.44.20240412.254/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/
+-rw-rw-rw-   0        0        0     1086 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.351607 pkscreener-0.44.20240412.255/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27550 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    17278 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    16886 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   108935 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77670 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-12 10:16:19.000000 pkscreener-0.44.20240412.255/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   111236 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18397 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-12 10:16:27.000000 pkscreener-0.44.20240412.255/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-12 10:16:27.367231 pkscreener-0.44.20240412.255/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-12 10:12:07.000000 pkscreener-0.44.20240412.255/setup.py
```

### Comparing `pkscreener-0.44.20240412.254/LICENSE` & `pkscreener-0.44.20240412.255/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/LICENSE-Others` & `pkscreener-0.44.20240412.255/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/PKG-INFO` & `pkscreener-0.44.20240412.255/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240412.254
+Version: 0.44.20240412.255
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.254.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.255.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.254/README.md` & `pkscreener-0.44.20240412.255/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.254/pkscreener/__init__.py` & `pkscreener-0.44.20240412.255/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                 # We'd then combine the data from 9:15 to 9:57 as a single candle of 
                 # OHLCV and replace the last daily candle with this one candle to
                 # simulate the scan outcome from morning.
                 df = pd.DataFrame(data=allDailyIntradayCandles[stock]["data"],
                                 columns=allDailyIntradayCandles[stock]["columns"],
                                 index=allDailyIntradayCandles[stock]["index"])
                 df = df.head(numOfCandles)
-                df = df[df.index <=  f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30']
+                df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
                 if df is not None and len(df) > 0:
                     combinedCandle = {"Open":PKMarketOpenCloseAnalyser.getMorningOpen(df), "High":max(df["High"]), 
                                     "Low":min(df["Low"]),"Close":PKMarketOpenCloseAnalyser.getMorningClose(df),
                                     "Adj Close":df["Adj Close"][-1],"Volume":sum(df["Volume"])}
                     tradingDate = PKDateUtilities.tradingDate()
                     timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d hh:mm:ss"),"%Y-%m-%d hh:mm:ss")
                     df = pd.DataFrame([combinedCandle], columns=df.columns, index=[timestamp])
@@ -231,23 +231,23 @@
                 else:
                     # We should ideally have all stocks from intraday and eod matching,
                     # but for whatever reason, if we don't have the stock, we should skip those
                     # stocks from analysis
                     del mutableAllDailyCandles[stock]
             except:
                 del mutableAllDailyCandles[stock]
+                if 'PKDevTools_Default_Log_Level' in os.environ.keys():
+                    intradayChange = colorText.miniTabulator().tabulate(
+                                        pd.DataFrame(listPriceDict),
+                                        headers="keys",
+                                        tablefmt=colorText.No_Pad_GridFormat,
+                                        showindex=False
+                                    ).encode("utf-8").decode(STD_ENCODING)
+                    default_logger().debug(intradayChange)
                 continue
-            if 'PKDevTools_Default_Log_Level' in os.environ.keys():
-                intradayChange = colorText.miniTabulator().tabulate(
-                                    pd.DataFrame(listPriceDict),
-                                    headers="keys",
-                                    tablefmt=colorText.No_Pad_GridFormat,
-                                    showindex=False
-                                ).encode("utf-8").decode(STD_ENCODING)
-                default_logger().debug(intradayChange)
         return mutableAllDailyCandles
 
     def runScanForStocksFromMorningTrade(stockListFromMorningTrade,dailyCandleData):
         latest_daily_df = None
         return latest_daily_df
 
     def diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, allDailyCandles,runOptionName=None):
```

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/classes/keys.py` & `pkscreener-0.44.20240412.255/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/courbd.ttf` & `pkscreener-0.44.20240412.255/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/globals.py` & `pkscreener-0.44.20240412.255/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,14 +273,19 @@
             )
             detaildf.rename(
                 columns={
                     "LTP": "LTP on Date",
                 },
                 inplace=True,
             )
+    except urllib.error.HTTPError as e:
+        if "HTTP Error 404" in str(e):
+            pass
+        else:
+            default_logger().debug(e, exc_info=True)
     except Exception as e:# pragma: no cover
         default_logger().debug(e, exc_info=True)
         pass
     return summarydf, detaildf
 
 
 def getTestBuildChoices(indexOption=None, executeOption=None, menuOption=None):
```

### Comparing `pkscreener-0.44.20240412.254/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240412.255/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240412.255/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240412.255/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240412.255/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240412.254
+Version: 0.44.20240412.255
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.254.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.255.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240412.254/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240412.254/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240412.255/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240412.254/setup.py` & `pkscreener-0.44.20240412.255/setup.py`

 * *Files identical despite different names*

