# Comparing `tmp/macnotesapp-0.5.3.tar.gz` & `tmp/macnotesapp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macnotesapp-0.5.3.tar", max compression
+gzip compressed data, was "macnotesapp-0.6.0.tar", max compression
```

## Comparing `macnotesapp-0.5.3.tar` & `macnotesapp-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2023-08-21 03:41:17.620013 macnotesapp-0.5.3/LICENSE
--rw-r--r--   0        0        0     6282 2023-08-21 03:41:17.620282 macnotesapp-0.5.3/README.md
--rw-r--r--   0        0        0      235 2023-08-21 03:41:17.622887 macnotesapp-0.5.3/macnotesapp/__init__.py
--rw-r--r--   0        0        0      108 2023-08-21 03:41:17.623129 macnotesapp-0.5.3/macnotesapp/__main__.py
--rw-r--r--   0        0        0       43 2023-08-22 14:28:05.536604 macnotesapp-0.5.3/macnotesapp/_version.py
--rw-r--r--   0        0        0       53 2023-08-21 03:41:17.623603 macnotesapp-0.5.3/macnotesapp/cli/__init__.py
--rw-r--r--   0        0        0    15167 2023-08-22 13:47:29.871421 macnotesapp-0.5.3/macnotesapp/cli/cli.py
--rw-r--r--   0        0        0     2848 2023-08-22 14:26:32.748205 macnotesapp-0.5.3/macnotesapp/cli/cli_config.py
--rw-r--r--   0        0        0     8287 2023-08-21 03:41:17.624527 macnotesapp-0.5.3/macnotesapp/cli/cli_help.py
--rw-r--r--   0        0        0      305 2023-08-21 03:41:17.624760 macnotesapp-0.5.3/macnotesapp/cli/cli_param_types.py
--rw-r--r--   0        0        0     8588 2023-08-21 03:41:17.625096 macnotesapp-0.5.3/macnotesapp/cli/click_rich_echo.py
--rw-r--r--   0        0        0      754 2023-08-21 03:41:17.625426 macnotesapp-0.5.3/macnotesapp/cli/readable.py
--rw-r--r--   0        0        0      509 2023-08-22 14:17:02.413122 macnotesapp-0.5.3/macnotesapp/logging.py
--rw-r--r--   0        0        0    13597 2023-08-21 03:41:17.625813 macnotesapp-0.5.3/macnotesapp/macnotesapp.applescript
--rw-r--r--   0        0        0    13931 2023-08-21 03:41:17.626047 macnotesapp-0.5.3/macnotesapp/macnotesapp_applescript.py
--rw-r--r--   0        0        0    28440 2023-08-22 14:17:02.414155 macnotesapp-0.5.3/macnotesapp/notesapp.py
--rw-r--r--   0        0        0      453 2023-08-22 14:17:02.415119 macnotesapp-0.5.3/macnotesapp/script_loader.py
--rw-r--r--   0        0        0      893 2023-08-22 14:17:02.415924 macnotesapp-0.5.3/macnotesapp/utils.py
--rw-r--r--   0        0        0     1369 2023-08-22 14:28:05.537204 macnotesapp-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7590 1970-01-01 00:00:00.000000 macnotesapp-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-21 03:41:17.620013 macnotesapp-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7750 2024-04-13 21:24:04.058980 macnotesapp-0.6.0/README.md
+-rw-r--r--   0        0        0      235 2023-08-21 03:41:17.622887 macnotesapp-0.6.0/macnotesapp/__init__.py
+-rw-r--r--   0        0        0      108 2023-08-21 03:41:17.623129 macnotesapp-0.6.0/macnotesapp/__main__.py
+-rw-r--r--   0        0        0       43 2024-04-13 21:28:01.028684 macnotesapp-0.6.0/macnotesapp/_version.py
+-rw-r--r--   0        0        0       53 2023-08-21 03:41:17.623603 macnotesapp-0.6.0/macnotesapp/cli/__init__.py
+-rw-r--r--   0        0        0    15167 2023-08-22 13:47:29.871421 macnotesapp-0.6.0/macnotesapp/cli/cli.py
+-rw-r--r--   0        0        0     2848 2023-08-22 14:26:32.748205 macnotesapp-0.6.0/macnotesapp/cli/cli_config.py
+-rw-r--r--   0        0        0     8287 2023-08-21 03:41:17.624527 macnotesapp-0.6.0/macnotesapp/cli/cli_help.py
+-rw-r--r--   0        0        0      305 2023-08-21 03:41:17.624760 macnotesapp-0.6.0/macnotesapp/cli/cli_param_types.py
+-rw-r--r--   0        0        0     8588 2023-08-21 03:41:17.625096 macnotesapp-0.6.0/macnotesapp/cli/click_rich_echo.py
+-rw-r--r--   0        0        0      754 2023-08-21 03:41:17.625426 macnotesapp-0.6.0/macnotesapp/cli/readable.py
+-rw-r--r--   0        0        0      509 2023-08-22 14:17:02.413122 macnotesapp-0.6.0/macnotesapp/logging.py
+-rw-r--r--   0        0        0    13597 2023-08-21 03:41:17.625813 macnotesapp-0.6.0/macnotesapp/macnotesapp.applescript
+-rw-r--r--   0        0        0    13931 2023-08-21 03:41:17.626047 macnotesapp-0.6.0/macnotesapp/macnotesapp_applescript.py
+-rw-r--r--   0        0        0    28440 2023-08-22 14:17:02.414155 macnotesapp-0.6.0/macnotesapp/notesapp.py
+-rw-r--r--   0        0        0      453 2023-08-22 14:17:02.415119 macnotesapp-0.6.0/macnotesapp/script_loader.py
+-rw-r--r--   0        0        0      893 2023-08-22 14:17:02.415924 macnotesapp-0.6.0/macnotesapp/utils.py
+-rw-r--r--   0        0        0     1396 2024-04-13 21:28:01.029850 macnotesapp-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9106 1970-01-01 00:00:00.000000 macnotesapp-0.6.0/PKG-INFO
```

### Comparing `macnotesapp-0.5.3/LICENSE` & `macnotesapp-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/README.md` & `macnotesapp-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # MacNotesApp
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code.
 
 ## Installation
 
 If you just want to use the command line tool, the easiest option is to install via [pipx](https://pypa.github.io/pipx/).
 
@@ -199,7 +202,30 @@
 
 * Password protected notes are not supported; unlocked password-protected notes can be accessed but locked notes cannot
 * Notes containing tags (#tagname) can be read but the tags will be stripped from the body of the note
 * Tags cannot be added to notes and will show up as plaintext if added manually with macnotesapp
 * Currently, only notes in top-level folders are accessible to `macnotesapp` (#4)
 * Attachments are not currently handled and will be ignored (#15)
 * The title style is not correctly set (#13)
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chadmando"><img src="https://avatars.githubusercontent.com/u/20407042?v=4?s=100" width="100px;" alt="chadmando"/><br /><sub><b>chadmando</b></sub></a><br /><a href="#userTesting-chadmando" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JonathanDoughty"><img src="https://avatars.githubusercontent.com/u/1918593?v=4?s=100" width="100px;" alt="JonathanDoughty"/><br /><sub><b>JonathanDoughty</b></sub></a><br /><a href="https://github.com/RhetTbull/macnotesapp/issues?q=author%3AJonathanDoughty" title="Bug reports">🐛</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `macnotesapp-0.5.3/macnotesapp/cli/cli.py` & `macnotesapp-0.6.0/macnotesapp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/cli/cli_config.py` & `macnotesapp-0.6.0/macnotesapp/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/cli/cli_help.py` & `macnotesapp-0.6.0/macnotesapp/cli/cli_help.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/cli/click_rich_echo.py` & `macnotesapp-0.6.0/macnotesapp/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/cli/readable.py` & `macnotesapp-0.6.0/macnotesapp/cli/readable.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/macnotesapp.applescript` & `macnotesapp-0.6.0/macnotesapp/macnotesapp.applescript`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/macnotesapp_applescript.py` & `macnotesapp-0.6.0/macnotesapp/macnotesapp_applescript.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/notesapp.py` & `macnotesapp-0.6.0/macnotesapp/notesapp.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/macnotesapp/utils.py` & `macnotesapp-0.6.0/macnotesapp/utils.py`

 * *Files identical despite different names*

### Comparing `macnotesapp-0.5.3/pyproject.toml` & `macnotesapp-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "macnotesapp"
-version = "0.5.3"
+version = "0.6.0"
 description = "Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code."
 authors = ["Rhet Turnbull <rturnbull@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/RhetTbull/macnotesapp"
 repository = "https://github.com/RhetTbull/macnotesapp"
 keywords = ["cli", "mac", "macos"]
@@ -20,14 +20,15 @@
 wheel = "^0.37.1"
 readability-lxml = "^0.8.1"
 requests = "^2.28.1"
 validators = "^0.20.0"
 markdownify = "^0.11.6"
 pyobjc-framework-ScriptingBridge = "^9.0.1"
 xdg = "^6.0.0"
+lxml-html-clean = "^0.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 cogapp = "^3.3.0"
 wheel = "^0.37.1"
 build = "^0.8.0"
 pyinstaller = "^5.7"
```

### Comparing `macnotesapp-0.5.3/PKG-INFO` & `macnotesapp-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: macnotesapp
-Version: 0.5.3
+Version: 0.6.0
 Summary: Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code.
 Home-page: https://github.com/RhetTbull/macnotesapp
 License: MIT
 Keywords: cli,mac,macos
 Author: Rhet Turnbull
 Author-email: rturnbull@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: lxml-html-clean (>=0.1.1,<0.2.0)
 Requires-Dist: markdown2 (>=2.4.3,<3.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: py-applescript (>=1.0.3,<2.0.0)
 Requires-Dist: pyobjc-framework-ScriptingBridge (>=9.0.1,<10.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: readability-lxml (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
@@ -26,14 +27,17 @@
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: wheel (>=0.37.1,<0.38.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Project-URL: Repository, https://github.com/RhetTbull/macnotesapp
 Description-Content-Type: text/markdown
 
 # MacNotesApp
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Work with Apple MacOS Notes.app from the command line. Also includes python interface for scripting Notes.app from your own python code.
 
 ## Installation
 
 If you just want to use the command line tool, the easiest option is to install via [pipx](https://pypa.github.io/pipx/).
 
@@ -231,7 +235,29 @@
 * Password protected notes are not supported; unlocked password-protected notes can be accessed but locked notes cannot
 * Notes containing tags (#tagname) can be read but the tags will be stripped from the body of the note
 * Tags cannot be added to notes and will show up as plaintext if added manually with macnotesapp
 * Currently, only notes in top-level folders are accessible to `macnotesapp` (#4)
 * Attachments are not currently handled and will be ignored (#15)
 * The title style is not correctly set (#13)
 
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chadmando"><img src="https://avatars.githubusercontent.com/u/20407042?v=4?s=100" width="100px;" alt="chadmando"/><br /><sub><b>chadmando</b></sub></a><br /><a href="#userTesting-chadmando" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JonathanDoughty"><img src="https://avatars.githubusercontent.com/u/1918593?v=4?s=100" width="100px;" alt="JonathanDoughty"/><br /><sub><b>JonathanDoughty</b></sub></a><br /><a href="https://github.com/RhetTbull/macnotesapp/issues?q=author%3AJonathanDoughty" title="Bug reports">🐛</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

