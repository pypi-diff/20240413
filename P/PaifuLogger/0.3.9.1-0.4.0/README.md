# Comparing `tmp/PaifuLogger-0.3.9.1.tar.gz` & `tmp/PaifuLogger-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaifuLogger-0.3.9.1.tar", last modified: Wed Apr  3 05:20:26 2024, max compression
+gzip compressed data, was "PaifuLogger-0.4.0.tar", last modified: Sat Apr 13 09:00:02 2024, max compression
```

## Comparing `PaifuLogger-0.3.9.1.tar` & `PaifuLogger-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 05:20:26.000000 PaifuLogger-0.3.9.1/PaifuLogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.085144 PaifuLogger-0.3.9.1/paifulogger/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/localizations/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/localizations/zh_tw.json
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/paifu_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/Paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/get_paifu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/log_into_xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/paifulogger/src/url_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:26.089144 PaifuLogger-0.3.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-03 05:20:21.000000 PaifuLogger-0.3.9.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.817308 PaifuLogger-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-13 09:00:02.817308 PaifuLogger-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.817308 PaifuLogger-0.4.0/PaifuLogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 09:00:02.000000 PaifuLogger-0.4.0/PaifuLogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/paifulogger/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/paifulogger/localizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/localizations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/localizations/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/localizations/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/localizations/zh_tw.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/paifu_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/paifulogger/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/Paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/get_paifu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/log_into_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/log_into_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/log_into_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/paifulogger/src/mjlog2mjai/
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/mjlog2mjai/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/mjlog2mjai/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/src/url_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/paifulogger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/pub_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/pub_tools/pub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:00:02.817308 PaifuLogger-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:00:02.813308 PaifuLogger-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-13 08:59:56.000000 PaifuLogger-0.4.0/test/test.py
```

### Comparing `PaifuLogger-0.3.9.1/LICENSE` & `PaifuLogger-0.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Jim137
+Copyright (c) 2023-2024 Jim137
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `PaifuLogger-0.3.9.1/PKG-INFO` & `PaifuLogger-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.3.9.1
+Version: 0.4.0
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
-        Copyright (c) 2023 Jim137
+        Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -70,15 +70,15 @@
 >>
 >> ```
 >> git clone https://github.com/Jim137/Tenhou-Paifu-Logger.git
 >> ```
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard.
 >>
->> iii. Open `runlog-user.bat`.
+>> iii. Open `runlog-user.bat` or `runlog-user.sh`.
 >
 > b. Download from pypi.
 >
 >> i. Open command line and type
 >>
 >> ```
 >> pip install PaifuLogger
@@ -105,26 +105,32 @@
 * [x] Customized output directory (-o, --output)
 * [x] Support mjai format paifu output (--mjai). *You have to run `git pull --recurse-submodules` first*.
 * [x] Localization support (-l, --language)
   * [x] English: en
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
+* [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
+  * Windows: `%localappdata%\Jim137\paifulogger\config.json`
+  * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
+  * Linux: `~/.local/share/paifulogger/config.json`
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
+* The change of Rate: Note it assumes that the player has played more than 400 games.
+* Number of wins
+* Number of deal-ins
 
 ## Future features
 
 * [ ] Add match replay for every round in html file
-* [ ] The change of Rate
 * [ ] Agari analysis
 * [ ] Support Majsoul paifu
 * [ ] GUI
 
 ## Contribute
 We welcome all kinds of contributions, including but not limited to bug reports, pull requests, feature requests, documentation improvements, localizations...etc.
```

### Comparing `PaifuLogger-0.3.9.1/PaifuLogger.egg-info/PKG-INFO` & `PaifuLogger-0.4.0/PaifuLogger.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PaifuLogger
-Version: 0.3.9.1
+Version: 0.4.0
 Summary: Logging tenhou paifu into excel or html file with some key information.
 Author-email: Jim137 <jim@mail.jim137.eu.org>
 License: MIT License
         
-        Copyright (c) 2023 Jim137
+        Copyright (c) 2023-2024 Jim137
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -70,15 +70,15 @@
 >>
 >> ```
 >> git clone https://github.com/Jim137/Tenhou-Paifu-Logger.git
 >> ```
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard.
 >>
->> iii. Open `runlog-user.bat`.
+>> iii. Open `runlog-user.bat` or `runlog-user.sh`.
 >
 > b. Download from pypi.
 >
 >> i. Open command line and type
 >>
 >> ```
 >> pip install PaifuLogger
@@ -105,26 +105,32 @@
 * [x] Customized output directory (-o, --output)
 * [x] Support mjai format paifu output (--mjai). *You have to run `git pull --recurse-submodules` first*.
 * [x] Localization support (-l, --language)
   * [x] English: en
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
+* [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
+  * Windows: `%localappdata%\Jim137\paifulogger\config.json`
+  * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
+  * Linux: `~/.local/share/paifulogger/config.json`
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
+* The change of Rate: Note it assumes that the player has played more than 400 games.
+* Number of wins
+* Number of deal-ins
 
 ## Future features
 
 * [ ] Add match replay for every round in html file
-* [ ] The change of Rate
 * [ ] Agari analysis
 * [ ] Support Majsoul paifu
 * [ ] GUI
 
 ## Contribute
 We welcome all kinds of contributions, including but not limited to bug reports, pull requests, feature requests, documentation improvements, localizations...etc.
```

### Comparing `PaifuLogger-0.3.9.1/PaifuLogger.egg-info/SOURCES.txt` & `PaifuLogger-0.4.0/PaifuLogger.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 PaifuLogger.egg-info/entry_points.txt
 PaifuLogger.egg-info/requires.txt
 PaifuLogger.egg-info/top_level.txt
 paifulogger/__init__.py
 paifulogger/__main__.py
 paifulogger/log.py
 paifulogger/paifu_dl.py
+paifulogger/version.py
 paifulogger/localizations/en.json
 paifulogger/localizations/ja.json
 paifulogger/localizations/zh.json
 paifulogger/localizations/zh_tw.json
 paifulogger/src/Paifu.py
 paifulogger/src/__init__.py
+paifulogger/src/config.py
 paifulogger/src/get_paifu.py
 paifulogger/src/i18n.py
 paifulogger/src/log_into_csv.py
 paifulogger/src/log_into_html.py
 paifulogger/src/log_into_xlsx.py
 paifulogger/src/url_log.py
 paifulogger/src/mjlog2mjai/parse.py
 paifulogger/src/mjlog2mjai/test.py
+pub_tools/pub.py
 test/__init__.py
 test/test.py
```

### Comparing `PaifuLogger-0.3.9.1/README.md` & `PaifuLogger-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 >>
 >> ```
 >> git clone https://github.com/Jim137/Tenhou-Paifu-Logger.git
 >> ```
 >>
 >> ii. Copy the paifu URL from tenhou.net to clipboard.
 >>
->> iii. Open `runlog-user.bat`.
+>> iii. Open `runlog-user.bat` or `runlog-user.sh`.
 >
 > b. Download from pypi.
 >
 >> i. Open command line and type
 >>
 >> ```
 >> pip install PaifuLogger
@@ -75,26 +75,32 @@
 * [x] Customized output directory (-o, --output)
 * [x] Support mjai format paifu output (--mjai). *You have to run `git pull --recurse-submodules` first*.
 * [x] Localization support (-l, --language)
   * [x] English: en
   * [x] Traditional Chinese: zh_tw
   * [x] Simplified Chinese: zh
   * [x] Japanese (ChatGPT): ja
+* [x] Support config file. Placing `config.json` in the same directory as the execution enables local configuration. For global configuration, place it in the following directories:
+  * Windows: `%localappdata%\Jim137\paifulogger\config.json`
+  * macOS: `/Users/{UserName}/Library/Application Support/paifulogger/config.json`
+  * Linux: `~/.local/share/paifulogger/config.json`
 
 ## Information logged
 
 * Game time
 * Placing
 * URL (for future use)
 * Rate before the game
+* The change of Rate: Note it assumes that the player has played more than 400 games.
+* Number of wins
+* Number of deal-ins
 
 ## Future features
 
 * [ ] Add match replay for every round in html file
-* [ ] The change of Rate
 * [ ] Agari analysis
 * [ ] Support Majsoul paifu
 * [ ] GUI
 
 ## Contribute
 We welcome all kinds of contributions, including but not limited to bug reports, pull requests, feature requests, documentation improvements, localizations...etc.
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/localizations/en.json` & `PaifuLogger-0.4.0/paifulogger/localizations/en.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'deal_in'": "'Deal-in num'",*

 * * "'deal_in_rate'": "'Deal-in rate'",*

 * * "'log_num'": "'Total games logged'",*

 * * "'r_change'": "'Change of rate'",*

 * * "'round_num'": "'Round number'",*

 * * "'win'": "'Win num'",*

 * * "'win_rate'": "'Win rate'"}*

```diff
@@ -1,19 +1,26 @@
 {
     "avg_plc": "Average Placing",
     "date": "Date",
+    "deal_in": "Deal-in num",
+    "deal_in_rate": "Deal-in rate",
     "excelE": 17,
     "hint_duplicate": "The match is duplicated.",
     "hint_input": "Please enter the URL of match:",
     "hint_record1": "Match of ",
     "hint_record2": " has been recorded.\n",
     "hint_tw": "Please check the URL of match and whether &tw=(seat) is attached to the end of the URL.",
     "hint_url": "Please check the URL of match and the network.",
     "log2mjai_import_error": "The submodule \"mjlog2mjai\" not found. Please run `git pull --recurse-submodules` or `git submodule update --init --recursive` to update the submodule.",
+    "log_num": "Total games logged",
     "paifu": "Paifu",
     "plc": "Placing",
     "preR": "Rate before match",
+    "r_change": "Change of rate",
     "remark": "Remark",
+    "round_num": "Round number",
     "sanma": "Sanma",
     "sanma_mjai_error": "The Sanma match does not support Mjai format.",
+    "win": "Win num",
+    "win_rate": "Win rate",
     "yonma": ""
 }
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/localizations/ja.json` & `PaifuLogger-0.4.0/paifulogger/localizations/ja.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'deal_in'": "'放銃数'",*

 * * "'deal_in_rate'": "'放銃率'",*

 * * "'log_num'": "'対局数'",*

 * * "'r_change'": "'R変動'",*

 * * "'round_num'": "'局数'",*

 * * "'win'": "'和了数'",*

 * * "'win_rate'": "'和了率'"}*

```diff
@@ -1,19 +1,26 @@
 {
     "avg_plc": "\u5e73\u5747\u9806\u4f4d",
     "date": "\u65e5\u4ed8",
+    "deal_in": "\u653e\u9283\u6570",
+    "deal_in_rate": "\u653e\u9283\u7387",
     "excelE": 11,
     "hint_duplicate": "\u65e2\u306b\u3053\u306e\u724c\u8b5c\u306f\u8a18\u9332\u3055\u308c\u3066\u3044\u307e\u3059",
     "hint_input": "\u724c\u8b5c\u306eURL\u3092\u5165\u529b\u3057\u3066\u304f\u3060\u3055\u3044:",
     "hint_record1": "\u4ee5\u4e0b\u306e\u724c\u8b5c\u3092\u8a18\u9332\u3057\u307e\u3057\u305f\uff1a",
     "hint_record2": "\n",
     "hint_tw": "URL\u306e\u5f8c\u306b&tw:(\u5e2d\u6b21)\u304c\u542b\u307e\u308c\u3066\u3044\u308b\u304b\u78ba\u8a8d\u3057\u3066\u304f\u3060\u3055\u3044",
     "hint_url": "\u724c\u8b5c\u306eURL\u304c\u6b63\u3057\u3044\u304b\u3001\u30cd\u30c3\u30c8\u30ef\u30fc\u30af\u306e\u72b6\u614b\u3092\u78ba\u8a8d\u3057\u3066\u304f\u3060\u3055\u3044",
     "log2mjai_import_error": "\u30b5\u30d6\u30e2\u30b8\u30e5\u30fc\u30eb\u300cmjlog2mjai\u300d\u304c\u898b\u3064\u304b\u308a\u307e\u305b\u3093\u3002`git pull --recurse-submodules`\u307e\u305f\u306f`git submodule update --init --recursive`\u30b3\u30de\u30f3\u30c9\u3092\u5b9f\u884c\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
+    "log_num": "\u5bfe\u5c40\u6570",
     "paifu": "\u724c\u8b5c",
     "plc": "\u9806\u4f4d",
     "preR": "\u5bfe\u5c40\u524dR\u5024",
+    "r_change": "R\u5909\u52d5",
     "remark": "\u5099\u8003",
+    "round_num": "\u5c40\u6570",
     "sanma": "\u4e09\u9ebb",
     "sanma_mjai_error": "\u4e09\u9ebb\u306e\u5bfe\u5c40\u3067\u306f\u307e\u3060mjai\u724c\u8b5c\u5f62\u5f0f\u306f\u30b5\u30dd\u30fc\u30c8\u3055\u308c\u3066\u3044\u307e\u305b\u3093",
+    "win": "\u548c\u4e86\u6570",
+    "win_rate": "\u548c\u4e86\u7387",
     "yonma": "\u56db\u9ebb"
 }
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/localizations/zh.json` & `PaifuLogger-0.4.0/paifulogger/localizations/zh.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'deal_in'": "'放铳数'",*

 * * "'deal_in_rate'": "'放铳率'",*

 * * "'log_num'": "'总对局数'",*

 * * "'r_change'": "'R值变化'",*

 * * "'round_num'": "'局数'",*

 * * "'win'": "'和牌数'",*

 * * "'win_rate'": "'和牌率'"}*

```diff
@@ -1,19 +1,26 @@
 {
     "avg_plc": "\u5e73\u987a",
     "date": "\u65e5\u671f",
+    "deal_in": "\u653e\u94f3\u6570",
+    "deal_in_rate": "\u653e\u94f3\u7387",
     "excelE": 11,
     "hint_duplicate": "\u5df2\u8bb0\u5f55\u8fc7\u6b64\u724c\u8c31",
     "hint_input": "\u8bf7\u8f93\u5165\u724c\u8c31\u7f51\u5740:",
     "hint_record1": "\u5df2\u5c06",
     "hint_record2": "\u724c\u8c31\u8bb0\u5f55\n",
     "hint_tw": "\u8bf7\u68c0\u67e5\u7f51\u5740\u540e\u9762&tw:(\u5e2d\u6b21)\u662f\u5426\u9644\u4e0a",
     "hint_url": "\u8bf7\u68c0\u67e5\u724c\u8c31\u7f51\u5740\u662f\u5426\u6b63\u786e\u4ee5\u53ca\u7f51\u7edc\u72b6\u6001",
     "log2mjai_import_error": "\u627e\u4e0d\u5230\u5b50\u6a21\u5757 \"mjlog2mjai\"\u3002\u8bf7\u6267\u884c `git pull --recurse-submodules` \u6216 `git submodule update --init --recursive` \u6765\u66f4\u65b0\u5b50\u6a21\u5757\u3002",
+    "log_num": "\u603b\u5bf9\u5c40\u6570",
     "paifu": "\u724c\u8c31",
     "plc": "\u987a\u4f4d",
     "preR": "\u5bf9\u5c40\u524dR\u503c",
+    "r_change": "R\u503c\u53d8\u5316",
     "remark": "\u5907\u6ce8",
+    "round_num": "\u5c40\u6570",
     "sanma": "\u4e09\u9ebb",
     "sanma_mjai_error": "\u4e09\u9ebb\u5bf9\u5c40\u5c1a\u4e0d\u6301mjai\u724c\u8c31\u683c\u5f0f",
+    "win": "\u548c\u724c\u6570",
+    "win_rate": "\u548c\u724c\u7387",
     "yonma": "\u56db\u9ebb"
 }
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/localizations/zh_tw.json` & `PaifuLogger-0.4.0/paifulogger/localizations/zh_tw.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'deal_in'": "'放銃數'",*

 * * "'deal_in_rate'": "'放銃率'",*

 * * "'log_num'": "'總對局數'",*

 * * "'r_change'": "'R值變化'",*

 * * "'round_num'": "'局數'",*

 * * "'win'": "'和牌數'",*

 * * "'win_rate'": "'和牌率'"}*

```diff
@@ -1,19 +1,26 @@
 {
     "avg_plc": "\u5e73\u9806",
     "date": "\u65e5\u671f",
+    "deal_in": "\u653e\u9283\u6578",
+    "deal_in_rate": "\u653e\u9283\u7387",
     "excelE": 11,
     "hint_duplicate": "\u5df2\u8a18\u9304\u904e\u6b64\u724c\u8b5c",
     "hint_input": "\u8acb\u8f38\u5165\u724c\u8b5c\u7db2\u5740:",
     "hint_record1": "\u5df2\u5c07",
     "hint_record2": "\u724c\u8b5c\u8a18\u9304\n",
     "hint_tw": "\u8acb\u6aa2\u67e5\u7db2\u5740\u5f8c\u9762&tw:(\u5e2d\u6b21)\u662f\u5426\u9644\u4e0a",
     "hint_url": "\u8acb\u6aa2\u67e5\u724c\u8b5c\u7db2\u5740\u662f\u5426\u6b63\u78ba\u4ee5\u53ca\u7db2\u8def\u72c0\u614b",
     "log2mjai_import_error": "\u627e\u4e0d\u5230\u5b50\u6a21\u7d44 \"mjlog2mjai\"\u3002\u8acb\u57f7\u884c `git pull --recurse-submodules` \u6216 `git submodule update --init --recursive` \u4f86\u66f4\u65b0\u5b50\u6a21\u7d44\u3002",
+    "log_num": "\u7e3d\u5c0d\u5c40\u6578",
     "paifu": "\u724c\u8b5c",
     "plc": "\u9806\u4f4d",
     "preR": "\u5c0d\u5c40\u524dR\u503c",
+    "r_change": "R\u503c\u8b8a\u5316",
     "remark": "\u5099\u8a3b",
+    "round_num": "\u5c40\u6578",
     "sanma": "\u4e09\u9ebb",
     "sanma_mjai_error": "\u4e09\u9ebb\u5c0d\u5c40\u5c1a\u4e0d\u652f\u63f4mjai\u724c\u8b5c\u683c\u5f0f",
+    "win": "\u548c\u724c\u6578",
+    "win_rate": "\u548c\u724c\u7387",
     "yonma": "\u56db\u9ebb"
 }
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/log.py` & `PaifuLogger-0.4.0/paifulogger/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import argparse
 import json
 import urllib.request
-import re
 import os
+import re
 import sys
 import warnings
 from typing import Callable
 
 from pandas import HDFStore, DataFrame
-from platformdirs import user_data_dir
 
+from .src.config import config_path
 from .src.get_paifu import get_paifu
 from .src.i18n import localized_str, LocalStr
 from .src.log_into_csv import log_into_csv
 from .src.log_into_xlsx import log_into_xlsx
 from .src.log_into_html import log_into_html
 from .src.url_log import url_log, check_duplicate
 
@@ -265,18 +265,16 @@
 def log(args: argparse.Namespace) -> int:
     """
     Parse the arguments and log paifu files.
     """
 
     # get version and exit
     if args.version:
-        try:
-            from paifulogger import __version__
-        except ImportError:
-            from . import __version__
+        from .version import __version__
+
         print("Tenhou-Paifu-Logger", __version__)
         return 0
 
     local_lang = _get_lang(args.lang)
     output = _get_output(args.output)
     urls = _get_urls(args.url, local_lang, output, args.remake)
     formats = _get_formats(args.format)
@@ -293,15 +291,17 @@
         output=output,
         remake=args.remake,
         ignore_duplicated=args.ignore_duplicated,
         mjai=args.mjai,
     )
 
 
-def log_parser(config_path: str | None = None) -> argparse.Namespace:
+def log_parser(
+    config_path: str | None = None, parser: argparse.ArgumentParser | None = None
+) -> argparse.Namespace:
     """
     Parse the arguments from the command line.
 
     Args:
         config_path: str
             The path of the config file.
 
@@ -310,15 +310,16 @@
     """
 
     config = {}
     if config_path and os.path.exists(f"{config_path}/config.json"):
         with open(f"{config_path}/config.json", "r") as f:
             config = json.load(f)
 
-    parser = argparse.ArgumentParser()
+    if parser is None:
+        parser = argparse.ArgumentParser(description="Paifu Logger")
     parser.add_argument("url", nargs="*", help="URL of the match.")
     parser.add_argument(
         "-l",
         "--lang",
         type=str,
         help="""Language of the program and output files. Default is English. 
         Available languages: English(en), 繁體中文(zh_tw), 简体中文(zh), 日本語(ja).""",
@@ -371,33 +372,19 @@
     parser.add_argument(
         "--ignore-duplicated",
         action="store_true",
         help=argparse.SUPPRESS,
         default=config.get("ignore_duplicated", False),
     )
     args = parser.parse_args()
+    if "plog" in args.url:
+        args.url.remove("plog")
     return args
 
 
-def config_path() -> str | None:
-    """
-    Try to get the path of the config file from current directory or user_data_dir.
-    """
-
-    appname = "paifulogger"
-    appauthor = "Jim137"
-    user_data_dir(appname, appauthor)
-    if os.path.exists(f"./config.json"):
-        return "."
-    elif os.path.exists(f"{user_data_dir(appname, appauthor)}/config.json"):
-        return user_data_dir(appname, appauthor)
-    else:
-        return None
-
-
-def main():
-    args = log_parser(config_path())
+def main(plog_parser: argparse.ArgumentParser | None = None):
+    args = log_parser(config_path(), plog_parser)
     return log(args)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/get_paifu.py` & `PaifuLogger-0.4.0/paifulogger/src/get_paifu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gzip
 import os
 import urllib.request
 import xml.etree.ElementTree as ET
 
-from .i18n import LocalStr
+from .i18n import LocalStr, localized_str
 from .Paifu import Paifu
 
 
 HEADER = {
     "Host": "e.mjv.jp",
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:65.0) Gecko/20100101 Firefox/65.0",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
@@ -23,15 +23,22 @@
     req = urllib.request.Request(url=url, headers=HEADER)
     opener = urllib.request.build_opener()
     response = opener.open(req)
     response = gzip.decompress(response.read()).decode("utf-8")
     return response
 
 
-def get_paifu(url: str, local_lang: LocalStr, output: str, mjai: bool = False):
+def get_paifu(
+    url: str,
+    local_lang: LocalStr = localized_str(
+        "en", os.path.dirname(os.path.abspath(__file__)).split("src")[0]
+    ),
+    output: str = "./",
+    mjai: bool = False,
+) -> Paifu:
     response = url_request_handler(url)
     root = ET.fromstring(response)
     paifu = Paifu(url, root)
     path = f"{output}/{local_lang.paifu}/{paifu.go_str}/"
     if not os.path.isdir(path):
         os.makedirs(path)
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/i18n.py` & `PaifuLogger-0.4.0/paifulogger/src/i18n.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/log_into_csv.py` & `PaifuLogger-0.4.0/paifulogger/src/log_into_csv.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,39 +15,53 @@
     else:
         paifu_str = local_lang.yonma + local_lang.paifu
     path = f"{output}/{local_lang.paifu}/{paifu_str}.csv"
     if os.path.isfile(path):
         csvfile = open(path, "a+", encoding="utf-8")
         writer = csv.writer(csvfile)
     else:
+        # Create a new csv file
         csvfile = open(path, "w", encoding="utf-8")
         writer = csv.writer(csvfile)
         writer.writerow(
             [
                 "# id",
                 local_lang.date,
                 local_lang.plc,
                 local_lang.paifu,
                 local_lang.preR,
+                local_lang.r_change,
+                local_lang.round_num,
+                local_lang.win,
+                local_lang.deal_in,
             ]
         )
     try:
-        df = pd.read_csv(path, index_col=0, encoding="utf-8")
-    except pd.errors.EmptyDataError:
-        df = pd.DataFrame(columns=["id", "date", "plc", "paifu", "preR"])
-    writer.writerow(
-        [
-            df.shape[0],
-            datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
-            paifu.get_place(paifu.ban),
-            paifu.url,
-            float(paifu.r[paifu.ban]),
-        ]
-    )
-    print(
-        "csv: "
-        + local_lang.hint_record1
-        + re.findall(r"\d{10}gm-\w{4}-\w{4}-\w{8}&tw=\d", paifu.url)[0]
-        + local_lang.hint_record2
-    )
-    csvfile.close()
+        try:
+            # Read the csv file
+            df = pd.read_csv(path, index_col=0, encoding="utf-8")
+        except pd.errors.EmptyDataError:
+            # If the csv file is empty, create a new DataFrame
+            df = pd.DataFrame(columns=["id", "date", "plc", "paifu", "preR", "r_change", "round_num", "win", "deal_in"])
+        # Append new paifu data to the csv file
+        writer.writerow(
+            [
+                df.shape[0],
+                datetime.strptime(re.findall(r"\d{10}", paifu.url)[0], "%Y%m%d%H"),
+                paifu.get_place(paifu.ban),
+                paifu.url,
+                float(paifu.r[paifu.ban]),
+                paifu.rate_change,
+                paifu.get_round_num(),
+                paifu.get_win_num(paifu.ban),
+                paifu.get_deal_in_num(paifu.ban),
+            ]
+        )
+        print(
+            "csv: "
+            + local_lang.hint_record1
+            + re.findall(r"\d{10}gm-\w{4}-\w{4}-\w{8}&tw=\d", paifu.url)[0]
+            + local_lang.hint_record2
+        )
+    finally:
+        csvfile.close()
     return None
```

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/parse.py` & `PaifuLogger-0.4.0/paifulogger/src/mjlog2mjai/parse.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/mjlog2mjai/test.py` & `PaifuLogger-0.4.0/paifulogger/src/mjlog2mjai/test.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9.1/paifulogger/src/url_log.py` & `PaifuLogger-0.4.0/paifulogger/src/url_log.py`

 * *Files identical despite different names*

### Comparing `PaifuLogger-0.3.9.1/pyproject.toml` & `PaifuLogger-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PaifuLogger"
-version = "0.3.9.1"
+version = "0.4.0"
 description = "Logging tenhou paifu into excel or html file with some key information."
 readme = "README.md"
 authors = [{ name = "Jim137", email = "jim@mail.jim137.eu.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 keywords = ["mahjong", "review", "logger", "paifu", "tenhou", "haifu", "paipu", "riichi-mahjong"]
-dependencies = [
-    "openpyxl",
-    "lxml",
-    "tables",
-    "pandas",
-    "platformdirs",
-]
+dependencies = ["openpyxl", "lxml", "tables", "pandas", "platformdirs"]
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://github.com/Jim137/Tenhou-Paifu-Logger"
 
 [project.scripts]
 log = "paifulogger.__main__:main"
 plog = "paifulogger.__main__:main"
 pdl = "paifulogger.paifu_dl:paifu_dl"
 
 [tool.setuptools.packages.find]
 exclude = [
-	"Paifu",
-	"牌譜",
+    "Paifu",
+    "牌譜",
 ]
 
 [tool.setuptools.package-data]
 "paifulogger.localizations" = [
-	"*.json",
+    "*.json",
 ]
```

### Comparing `PaifuLogger-0.3.9.1/test/test.py` & `PaifuLogger-0.4.0/test/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.version = True
 
-        self.assertEqual(log.log(args), 0)
+        self.assertEqual(log(args), 0)
 
     def test_1(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
@@ -49,15 +49,15 @@
             "https://tenhou.net/0/?log=2023050200gm-0099-0000-50c65fbf&tw=2",
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
         args.all_formats = True
         args.ignore_duplicated = True
         args.output = "./test/"
 
-        self.assertEqual(log.log(args), 0)
+        self.assertEqual(log(args), 0)
 
     def test_2(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
@@ -72,38 +72,38 @@
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
         args.all_formats = True
         args.ignore_duplicated = True
         args.output = "./test/"
         args.lang = "zh_tw"
 
-        self.assertEqual(log.log(args), 0)
+        self.assertEqual(log(args), 0)
 
     def test_3(self):
         urls = [
             # yonma tests
             "https://tenhou.net/3/?log=2022052501gm-00c1-0000-f71e7910&tw=1",
             "https://tenhou.net/0/?log=2023051123gm-0001-0000-b3720f99&tw=2",
             "http://tenhou.net/0/?log=2023051216gm-0001-0000-5fd022cc&tw=1",
             # sanma tests
             "https://tenhou.net/0/?log=2023050200gm-0099-0000-50c65fbf&tw=2",
             "http://tenhou.net/0/?log=2023050419gm-0099-0000-b3111c7e&tw=0",
         ]
 
-        self.assertEqual(paifu_dl.paifu_dl(urls, output="./test/"), 0)
+        self.assertEqual(paifu_dl(urls, output="./test/"), 0)
 
     def test_4(self):
         parser = argparse.ArgumentParser()
         args = parser.parse_args()
 
         for attr in ATTR:
             setattr(args, attr.replace("-", "_"), None)
 
         args.all_formats = True
         args.output = "./test/"
         args.remake = True
 
-        self.assertEqual(log.log(args), 0)
+        self.assertEqual(log(args), 0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

