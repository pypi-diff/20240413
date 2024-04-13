# Comparing `tmp/pytha-fuzz-1.0.tar.gz` & `tmp/pytha-fuzz-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytha-fuzz-1.0.tar", last modified: Sat Apr 13 05:15:06 2024, max compression
+gzip compressed data, was "pytha-fuzz-1.1.tar", last modified: Sat Apr 13 05:44:07 2024, max compression
```

## Comparing `pytha-fuzz-1.0.tar` & `pytha-fuzz-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:15:06.974071 pytha-fuzz-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 05:14:56.000000 pytha-fuzz-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-13 05:15:06.974071 pytha-fuzz-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-13 05:14:56.000000 pytha-fuzz-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:15:06.974071 pytha-fuzz-1.0/pytha/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 05:14:56.000000 pytha-fuzz-1.0/pytha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-13 05:14:56.000000 pytha-fuzz-1.0/pytha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:15:06.974071 pytha-fuzz-1.0/pytha_fuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 05:15:06.000000 pytha-fuzz-1.0/pytha_fuzz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:15:06.974071 pytha-fuzz-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 05:14:56.000000 pytha-fuzz-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:44:07.274039 pytha-fuzz-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 05:44:03.000000 pytha-fuzz-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-13 05:44:07.274039 pytha-fuzz-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-13 05:44:03.000000 pytha-fuzz-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:44:07.270039 pytha-fuzz-1.1/pytha/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 05:44:03.000000 pytha-fuzz-1.1/pytha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-13 05:44:03.000000 pytha-fuzz-1.1/pytha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:44:07.274039 pytha-fuzz-1.1/pytha_fuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 05:44:07.000000 pytha-fuzz-1.1/pytha_fuzz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:44:07.274039 pytha-fuzz-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 05:44:03.000000 pytha-fuzz-1.1/setup.py
```

### Comparing `pytha-fuzz-1.0/LICENSE` & `pytha-fuzz-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytha-fuzz-1.0/PKG-INFO` & `pytha-fuzz-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytha-fuzz
-Version: 1.0
+Version: 1.1
 Summary: PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.
 Home-page: https://github.com/shivangmauryaa/pytha-fuzz
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytha-fuzz-1.0/README.md` & `pytha-fuzz-1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytha-fuzz-1.0/pytha/__init__.py` & `pytha-fuzz-1.1/pytha/__init__.py`

 * *Files identical despite different names*

### Comparing `pytha-fuzz-1.0/pytha/main.py` & `pytha-fuzz-1.1/pytha/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 
 WORDLIST_URL = "https://github.com/halfstackpgr/pytha-fuzz/files/14965324/wordlist.txt"
 
 
 async def download_wordlist(url: str, save_path: str) -> bool:
     try:
         async with httpx.AsyncClient() as client:
+            client.allow_redirects = True
             response = await client.get(url)
             if response.status_code == 200:
                 async with aiofiles.open(save_path, "wb") as file:
                     await file.write(response.content)
                 return True
             else:
-                print(Fore.RED + f"Failed to download wordlist. Status code: {response.status_code}")
+                print(
+                    Fore.RED
+                    + f"Failed to download wordlist. Status code: {response.status_code}"
+                )
                 return False
     except Exception as e:
         print(Fore.RED + f"An error occurred while downloading the wordlist: {e}")
         return False
 
+
 def load_wordlist(wordlist_file: t.Optional[t.Union[pathlib.Path, str]]) -> t.List[str]:
     if isinstance(wordlist_file, str):
         wordlist_path = pathlib.Path(wordlist_file)
     if wordlist_path.exists() is False:
         print(Fore.YELLOW + "No wordlist provided. Downloading default wordlist...")
         download_path = "wordlist.txt"
         if not asyncio.run(download_wordlist(WORDLIST_URL, download_path)):
```

### Comparing `pytha-fuzz-1.0/pytha_fuzz.egg-info/PKG-INFO` & `pytha-fuzz-1.1/pytha_fuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytha-fuzz
-Version: 1.0
+Version: 1.1
 Summary: PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.
 Home-page: https://github.com/shivangmauryaa/pytha-fuzz
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytha-fuzz-1.0/setup.py` & `pytha-fuzz-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pytha-fuzz",
-    version="1.0",
+    version="1.1",
     author="Parth Mishra",
     author_email="halfstackpgr@gmail.com",
     description="PYTHA is a Python-based directory fuzzer tool designed to aid in the discovery of hidden or sensitive directories and files on web servers. Originally developed by Shivang. Packed and moduled by the author.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shivangmauryaa/pytha-fuzz",
     packages=["pytha"],
```

