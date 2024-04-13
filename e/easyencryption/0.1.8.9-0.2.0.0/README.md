# Comparing `tmp/easyencryption-0.1.8.9.tar.gz` & `tmp/easyencryption-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.9.tar", last modified: Fri Apr 12 15:40:34 2024, max compression
+gzip compressed data, was "easyencryption-0.2.tar", last modified: Fri Apr 12 16:52:17 2024, max compression
```

## Comparing `easyencryption-0.1.8.9.tar` & `easyencryption-0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:40:34.247313 easyencryption-0.1.8.9/
--rw-rw-rw-   0        0        0     4099 2024-04-12 15:40:34.247313 easyencryption-0.1.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.1.8.9/README.md
--rw-rw-rw-   0        0        0      723 2024-04-12 15:40:34.248332 easyencryption-0.1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1829 2024-04-12 15:40:23.000000 easyencryption-0.1.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:40:34.221871 easyencryption-0.1.8.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 15:40:34.233066 easyencryption-0.1.8.9/src/easyencryption/
--rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.9/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.9/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.9/src/easyencryption/ascii.py
--rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.9/src/easyencryption/blake.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.9/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.9/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.9/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.9/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.9/src/easyencryption/shake.py
--rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.9/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:40:34.246289 easyencryption-0.1.8.9/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     4099 2024-04-12 15:40:34.000000 easyencryption-0.1.8.9/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-04-12 15:40:34.000000 easyencryption-0.1.8.9/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:40:34.000000 easyencryption-0.1.8.9/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-12 15:40:34.000000 easyencryption-0.1.8.9/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 15:40:34.000000 easyencryption-0.1.8.9/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.187365 easyencryption-0.2/
+-rw-rw-rw-   0        0        0     4099 2024-04-12 16:52:17.187365 easyencryption-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.2/README.md
+-rw-rw-rw-   0        0        0      723 2024-04-12 16:52:17.191956 easyencryption-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-12 16:51:51.000000 easyencryption-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.156297 easyencryption-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.169547 easyencryption-0.2/src/easyencryption/
+-rw-rw-rw-   0        0        0      556 2024-04-12 15:42:25.000000 easyencryption-0.2/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.2/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.2/src/easyencryption/ascii.py
+-rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.2/src/easyencryption/blake.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.2/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.2/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.2/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.2/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.2/src/easyencryption/shake.py
+-rw-rw-rw-   0        0        0     4437 2024-04-12 16:50:14.000000 easyencryption-0.2/src/easyencryption/test_all.py
+-rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.2/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.186342 easyencryption-0.2/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     4099 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.9/PKG-INFO` & `easyencryption-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.9
+Version: 0.2.0.0
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.8.9/README.md` & `easyencryption-0.2/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/setup.cfg` & `easyencryption-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/setup.py` & `easyencryption-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-version = "0.1.8.9"
+version = "0.2.0.0"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -21,15 +21,15 @@
     python_requires='>=3.6',
     install_requires=[
     "setuptools>=42",
     "cryptography",
     "pycryptodomex",
     "pycryptodome",
     "wheel",
-    "eciespy"
+    "eciespy",
     ],
     project_urls={
         'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
         'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
         'Source': 'https://github.com/BlazenBoi/easyencryption',
     },
     classifiers=[
```

### Comparing `easyencryption-0.1.8.9/src/easyencryption/__init__.py` & `easyencryption-0.2/src/easyencryption/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,9 +2,8 @@
 from .rsa import rsaencrypt, rsadecrypt
 from .aes import aesencrypt, aesdecrypt
 from .sha import sha224encrypt, sha224check, sha256encrypt, sha256check, sha384encrypt, sha384check, sha512encrypt, sha512check
 from .ascii import asciiencrypt, asciidecrypt
 from .ecc import eccencrypt, eccdecrypt
 from .xor import xorencrypt, xordecrypt
 from .blake import blakeencrypt, blakecheck
-from .shake import shake128encrypt, shake128check, shake256encrypt, shake256check
-from .xor import xorencrypt, xordecrypt
+from .shake import shake128encrypt, shake128check, shake256encrypt, shake256check
```

### Comparing `easyencryption-0.1.8.9/src/easyencryption/aes.py` & `easyencryption-0.2/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/ascii.py` & `easyencryption-0.2/src/easyencryption/ascii.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/blake.py` & `easyencryption-0.2/src/easyencryption/blake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/ecc.py` & `easyencryption-0.2/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/fernet.py` & `easyencryption-0.2/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/rsa.py` & `easyencryption-0.2/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/sha.py` & `easyencryption-0.2/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/shake.py` & `easyencryption-0.2/src/easyencryption/shake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption/xor.py` & `easyencryption-0.2/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.9/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.2/src/easyencryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.9
+Version: 0.2.0.0
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

