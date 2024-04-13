# Comparing `tmp/pytha-fuzz-0.1.tar.gz` & `tmp/pytha-fuzz-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytha-fuzz-0.1.tar", last modified: Sat Apr 13 04:22:17 2024, max compression
+gzip compressed data, was "pytha-fuzz-0.2.tar", last modified: Sat Apr 13 04:41:55 2024, max compression
```

## Comparing `pytha-fuzz-0.1.tar` & `pytha-fuzz-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:22:17.198290 pytha-fuzz-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 04:22:13.000000 pytha-fuzz-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-13 04:22:17.198290 pytha-fuzz-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-13 04:22:13.000000 pytha-fuzz-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:22:17.198290 pytha-fuzz-0.1/pytha/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 04:22:13.000000 pytha-fuzz-0.1/pytha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-13 04:22:13.000000 pytha-fuzz-0.1/pytha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:22:17.198290 pytha-fuzz-0.1/pytha_fuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 04:22:17.000000 pytha-fuzz-0.1/pytha_fuzz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:22:17.198290 pytha-fuzz-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 04:22:13.000000 pytha-fuzz-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:41:55.975094 pytha-fuzz-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 04:41:46.000000 pytha-fuzz-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-13 04:41:55.975094 pytha-fuzz-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-13 04:41:46.000000 pytha-fuzz-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:41:55.975094 pytha-fuzz-0.2/pytha/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 04:41:46.000000 pytha-fuzz-0.2/pytha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-13 04:41:46.000000 pytha-fuzz-0.2/pytha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:41:55.975094 pytha-fuzz-0.2/pytha_fuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 04:41:55.000000 pytha-fuzz-0.2/pytha_fuzz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:41:55.975094 pytha-fuzz-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 04:41:46.000000 pytha-fuzz-0.2/setup.py
```

### Comparing `pytha-fuzz-0.1/LICENSE` & `pytha-fuzz-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytha-fuzz-0.1/PKG-INFO` & `pytha-fuzz-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytha-fuzz
-Version: 0.1
+Version: 0.2
 Summary: PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.
 Home-page: https://github.com/shivangmauryaa/pytha-fuzz
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,16 @@
 Requires-Dist: aiofiles
 Requires-Dist: colorama
 Requires-Dist: httpx
 
 # Directory Search Tool (FUZZER)
 
 
-![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) ![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
+![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) 
+![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
 ![Static Badge](https://img.shields.io/badge/python-Strict-checking?style=plastic&logo=python&label=Type-Checking&labelColor=yellow)
 
 ![FUZZER Logo](https://static.thenounproject.com/png/2221438-200.png)
 
 
 
 > [!IMPORTANT]
```

### Comparing `pytha-fuzz-0.1/README.md` & `pytha-fuzz-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Directory Search Tool (FUZZER)
 
 
-![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) ![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
+![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) 
+![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
 ![Static Badge](https://img.shields.io/badge/python-Strict-checking?style=plastic&logo=python&label=Type-Checking&labelColor=yellow)
 
 ![FUZZER Logo](https://static.thenounproject.com/png/2221438-200.png)
 
 
 
 > [!IMPORTANT]
```

### Comparing `pytha-fuzz-0.1/pytha/__init__.py` & `pytha-fuzz-0.2/pytha/__init__.py`

 * *Files identical despite different names*

### Comparing `pytha-fuzz-0.1/pytha/main.py` & `pytha-fuzz-0.2/pytha/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,43 @@
 import aiofiles
 import pathlib
 from colorama import Fore, Style, init
 
 init(autoreset=True)
 
 
-def load_wordlist(wordlist_file: t.Union[pathlib.Path, str]) -> t.List[str]:
+WORDLIST_URL = "https://github.com/halfstackpgr/pytha-fuzz/blob/main/wordlist.txt"
+
+
+async def download_wordlist(url: str, save_path: str) -> bool:
+    try:
+        async with httpx.AsyncClient() as client:
+            response = await client.get(url)
+            if response.status_code == 200:
+                async with aiofiles.open(save_path, "wb") as file:
+                    await file.write(response.content)
+                return True
+            else:
+                print(Fore.RED + f"Failed to download wordlist. Status code: {response.status_code}")
+                return False
+    except Exception as e:
+        print(Fore.RED + f"An error occurred while downloading the wordlist: {e}")
+        return False
+
+def load_wordlist(wordlist_file: t.Optional[t.Union[pathlib.Path, str]]) -> t.List[str]:
+    if wordlist_file is None:
+        print(Fore.YELLOW + "No wordlist provided. Downloading default wordlist...")
+        download_path = "wordlist.txt"
+        if not asyncio.run(download_wordlist(WORDLIST_URL, download_path)):
+            print(Fore.RED + "Failed to download the default wordlist. Exiting...")
+            sys.exit(1)
+        else:
+            print(Fore.GREEN + "Default wordlist downloaded successfully.")
+            wordlist_file = download_path
+
     try:
         with open(wordlist_file, "r") as file:
             return [line.strip() for line in file.readlines()]
     except FileNotFoundError:
         print(Fore.RED + f"Wordlist file '{wordlist_file}' not found.")
         return []
     except Exception as e:
@@ -183,8 +211,7 @@
         )
     )
 
     print_farewell_message("Shivang | GitHub")
 
     if args.output:
         sys.exit(0)
-
```

### Comparing `pytha-fuzz-0.1/pytha_fuzz.egg-info/PKG-INFO` & `pytha-fuzz-0.2/pytha_fuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytha-fuzz
-Version: 0.1
+Version: 0.2
 Summary: PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.
 Home-page: https://github.com/shivangmauryaa/pytha-fuzz
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,16 @@
 Requires-Dist: aiofiles
 Requires-Dist: colorama
 Requires-Dist: httpx
 
 # Directory Search Tool (FUZZER)
 
 
-![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) ![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
+![Ruff](https://camo.githubusercontent.com/18c26428c337f9d641fa09b629a3a03b514e8ac84b57974a0ed7d1b38e14e060/68747470733a2f2f696d672e736869656c64732e696f2f656e64706f696e743f75726c3d68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f61737472616c2d73682f727566662f6d61696e2f6173736574732f62616467652f76322e6a736f6e) 
+![Passing Package](https://github.com/halfstackpgr/pytha-fuzz/actions/workflows/python-publish.yml/badge.svg)
 ![Static Badge](https://img.shields.io/badge/python-Strict-checking?style=plastic&logo=python&label=Type-Checking&labelColor=yellow)
 
 ![FUZZER Logo](https://static.thenounproject.com/png/2221438-200.png)
 
 
 
 > [!IMPORTANT]
```

### Comparing `pytha-fuzz-0.1/setup.py` & `pytha-fuzz-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pytha-fuzz",
-    version="0.1",
+    version="0.2",
     author="Parth Mishra",
     author_email="halfstackpgr@gmail.com",
     description="PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shivangmauryaa/pytha-fuzz",
     packages=["pytha"],
```

