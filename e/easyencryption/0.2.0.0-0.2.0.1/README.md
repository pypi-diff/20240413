# Comparing `tmp/easyencryption-0.2.tar.gz` & `tmp/easyencryption-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.2.tar", last modified: Fri Apr 12 16:52:17 2024, max compression
+gzip compressed data, was "easyencryption-0.2.0.1.tar", last modified: Sat Apr 13 12:25:32 2024, max compression
```

## Comparing `easyencryption-0.2.tar` & `easyencryption-0.2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.187365 easyencryption-0.2/
--rw-rw-rw-   0        0        0     4099 2024-04-12 16:52:17.187365 easyencryption-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.2/README.md
--rw-rw-rw-   0        0        0      723 2024-04-12 16:52:17.191956 easyencryption-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-04-12 16:51:51.000000 easyencryption-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.156297 easyencryption-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.169547 easyencryption-0.2/src/easyencryption/
--rw-rw-rw-   0        0        0      556 2024-04-12 15:42:25.000000 easyencryption-0.2/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.2/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.2/src/easyencryption/ascii.py
--rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.2/src/easyencryption/blake.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.2/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.2/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.2/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.2/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.2/src/easyencryption/shake.py
--rw-rw-rw-   0        0        0     4437 2024-04-12 16:50:14.000000 easyencryption-0.2/src/easyencryption/test_all.py
--rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.2/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:52:17.186342 easyencryption-0.2/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     4099 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 16:52:17.000000 easyencryption-0.2/src/easyencryption.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.737778 easyencryption-0.2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.737778 easyencryption-0.2.0.1/src/easyencryption/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/blake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/fernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/shake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/src/easyencryption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.2/PKG-INFO` & `easyencryption-0.2.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: easyencryption
-Version: 0.2.0.0
-Summary: A very easy way to encrypt data.
-Home-page: https://github.com/BlazenBoi/easyencryption/issues
-Author: Blazen
-Author-email: contact@fireballbot.com
-License: MIT
-Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
-Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
-Project-URL: Source, https://github.com/BlazenBoi/easyencryption
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools>=42
-Requires-Dist: cryptography
-Requires-Dist: pycryptodomex
-Requires-Dist: pycryptodome
-Requires-Dist: wheel
-Requires-Dist: eciespy
-
-In Progress...
-
-
-We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
+Metadata-Version: 2.1
+Name: easyencryption
+Version: 0.2.0.1
+Summary: A very easy way to encrypt data.
+Home-page: https://github.com/BlazenBoi/easyencryption/issues
+Author: Blazen
+Author-email: contact@fireballbot.com
+License: MIT
+Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
+Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
+Project-URL: Source, https://github.com/BlazenBoi/easyencryption
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
+
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-0.2/README.md` & `easyencryption-0.2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-In Progress...
-
-
-We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
 [![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-0.2/setup.cfg` & `easyencryption-0.2.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2065 6173 7965 6e63 7279 7074 696f   = easyencryptio
-00000020: 6e0d 0a76 6572 7369 6f6e 203d 2030 2e31  n..version = 0.1
-00000030: 2e36 0d0a 6175 7468 6f72 203d 2062 6c61  .6..author = bla
-00000040: 7a65 6e0d 0a61 7574 686f 725f 656d 6169  zen..author_emai
-00000050: 6c20 3d20 636f 6e74 6163 7440 6669 7265  l = contact@fire
-00000060: 6261 6c6c 626f 742e 636f 6d0d 0a64 6573  ballbot.com..des
-00000070: 6372 6970 7469 6f6e 203d 2041 2076 6572  cription = A ver
-00000080: 7920 6561 7379 2077 6179 2074 6f20 656e  y easy way to en
-00000090: 6372 7970 7420 6461 7461 0d0a 6c6f 6e67  crypt data..long
-000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000b0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000d0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-000000f0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000100: 6875 622e 636f 6d2f 426c 617a 656e 426f  hub.com/BlazenBo
-00000110: 692f 6361 6e76 6163 6f72 642e 7079 0d0a  i/canvacord.py..
-00000120: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-00000130: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-00000140: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000150: 6f6d 2f42 6c61 7a65 6e42 6f69 2f63 616e  om/BlazenBoi/can
-00000160: 7661 636f 7264 2e70 792f 6973 7375 6573  vacord.py/issues
-00000170: 0d0a 0944 6973 636f 7264 2053 6572 7665  ...Discord Serve
-00000180: 7220 3d20 6874 7470 733a 2f2f 6469 7363  r = https://disc
-00000190: 6f72 642e 636f 6d2f 696e 7669 7465 2f6d  ord.com/invite/m
-000001a0: 5055 3348 7962 4273 390d 0a63 6c61 7373  PU3HybBs9..class
-000001b0: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-000001c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001d0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001e0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001f0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000200: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000210: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000220: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-00000230: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000240: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000250: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000260: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000270: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
-00000280: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000290: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000002a0: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-000002b0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002c0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002d0: 0a0d 0a                                  ...
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6561 7379 656e 6372 7970 7469 6f6e  = easyencryption
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e36  .version = 0.1.6
+00000030: 0a61 7574 686f 7220 3d20 626c 617a 656e  .author = blazen
+00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000050: 636f 6e74 6163 7440 6669 7265 6261 6c6c  contact@fireball
+00000060: 626f 742e 636f 6d0a 6465 7363 7269 7074  bot.com.descript
+00000070: 696f 6e20 3d20 4120 7665 7279 2065 6173  ion = A very eas
+00000080: 7920 7761 7920 746f 2065 6e63 7279 7074  y way to encrypt
+00000090: 2064 6174 610a 6c6f 6e67 5f64 6573 6372   data.long_descr
+000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000b0: 4541 444d 452e 6d64 0a6c 6f6e 675f 6465  EADME.md.long_de
+000000c0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+000000d0: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+000000e0: 726b 646f 776e 0a75 726c 203d 2068 7474  rkdown.url = htt
+000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000100: 426c 617a 656e 426f 692f 6361 6e76 6163  BlazenBoi/canvac
+00000110: 6f72 642e 7079 0a70 726f 6a65 6374 5f75  ord.py.project_u
+00000120: 726c 7320 3d20 0a09 4275 6720 5472 6163  rls = ..Bug Trac
+00000130: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000140: 7468 7562 2e63 6f6d 2f42 6c61 7a65 6e42  thub.com/BlazenB
+00000150: 6f69 2f63 616e 7661 636f 7264 2e70 792f  oi/canvacord.py/
+00000160: 6973 7375 6573 0a09 4469 7363 6f72 6420  issues..Discord 
+00000170: 5365 7276 6572 203d 2068 7474 7073 3a2f  Server = https:/
+00000180: 2f64 6973 636f 7264 2e63 6f6d 2f69 6e76  /discord.com/inv
+00000190: 6974 652f 6d50 5533 4879 6242 7339 0a63  ite/mPU3HybBs9.c
+000001a0: 6c61 7373 6966 6965 7273 203d 200a 0950  lassifiers = ..P
+000001b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001d0: 2033 0a09 4c69 6365 6e73 6520 3a3a 204f   3..License :: O
+000001e0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+000001f0: 4954 204c 6963 656e 7365 0a09 4f70 6572  IT License..Oper
+00000200: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000210: 4f53 2049 6e64 6570 656e 6465 6e74 0a0a  OS Independent..
+00000220: 5b6f 7074 696f 6e73 5d0a 7061 636b 6167  [options].packag
+00000230: 655f 6469 7220 3d20 0a09 3d20 7372 630a  e_dir = ..= src.
+00000240: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000250: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000260: 203d 203e 3d33 2e36 0a0a 5b6f 7074 696f   = >=3.6..[optio
+00000270: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000280: 5d0a 7768 6572 6520 3d20 7372 630a 0a5b  ].where = src..[
+00000290: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
+000002a0: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
+000002b0: 3d20 300a 0a                             = 0..
```

### Comparing `easyencryption-0.2/setup.py` & `easyencryption-0.2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_desc = open("README.md", "r")
-long_description = long_desc.read()
-version = "0.2.0.0"
-
-setup(
-    name='easyencryption',
-    version=version,
-    description='A very easy way to encrypt data.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    license='MIT',
-    url='https://github.com/BlazenBoi/easyencryption/issues',
-    author='Blazen',
-    author_email='contact@fireballbot.com',
-    keywords='',
-    packages=find_packages(include=['easyencryption']),
-    python_requires='>=3.6',
-    install_requires=[
-    "setuptools>=42",
-    "cryptography",
-    "pycryptodomex",
-    "pycryptodome",
-    "wheel",
-    "eciespy",
-    ],
-    project_urls={
-        'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
-        'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
-        'Source': 'https://github.com/BlazenBoi/easyencryption',
-    },
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Internet',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-      ]
-)
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_desc = open("README.md", "r")
+long_description = long_desc.read()
+version = "0.2.0.1"
+
+setup(
+    name='easyencryption',
+    version=version,
+    description='A very easy way to encrypt data.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    license='MIT',
+    url='https://github.com/BlazenBoi/easyencryption/issues',
+    author='Blazen',
+    author_email='contact@fireballbot.com',
+    keywords='',
+    packages=find_packages(include=['easyencryption']),
+    python_requires='>=3.6',
+    install_requires=[
+    "setuptools>=42",
+    "cryptography",
+    "pycryptodomex",
+    "pycryptodome",
+    "wheel",
+    "eciespy",
+    ],
+    project_urls={
+        'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
+        'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
+        'Source': 'https://github.com/BlazenBoi/easyencryption',
+    },
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Internet',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+      ]
+)
 #© 2021 GitHub, Inc.
```

### Comparing `easyencryption-0.2/src/easyencryption/__init__.py` & `easyencryption-0.2.0.1/src/easyencryption/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .fernet import fernetencrypt, fernetdecrypt, multifernetencrypt, multifernetdecrypt
-from .rsa import rsaencrypt, rsadecrypt
-from .aes import aesencrypt, aesdecrypt
-from .sha import sha224encrypt, sha224check, sha256encrypt, sha256check, sha384encrypt, sha384check, sha512encrypt, sha512check
-from .ascii import asciiencrypt, asciidecrypt
-from .ecc import eccencrypt, eccdecrypt
-from .xor import xorencrypt, xordecrypt
-from .blake import blakeencrypt, blakecheck
+from .fernet import fernetencrypt, fernetdecrypt, multifernetencrypt, multifernetdecrypt
+from .rsa import rsaencrypt, rsadecrypt
+from .aes import aesencrypt, aesdecrypt
+from .sha import sha224encrypt, sha224check, sha256encrypt, sha256check, sha384encrypt, sha384check, sha512encrypt, sha512check
+from .ascii import asciiencrypt, asciidecrypt
+from .ecc import eccencrypt, eccdecrypt
+from .xor import xorencrypt, xordecrypt
+from .blake import blakeencrypt, blakecheck
 from .shake import shake128encrypt, shake128check, shake256encrypt, shake256check
```

### Comparing `easyencryption-0.2/src/easyencryption/aes.py` & `easyencryption-0.2.0.1/src/easyencryption/aes.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import base64, hashlib, Crypto
-from Cryptodome.Cipher import AES
-
-async def genkey():
-    generated_key = Crypto.Random.new().read(AES.block_size)
-    key = hashlib.sha256(generated_key).digest()
-    with open("aeseasyencryption.key", "wb") as key_file:
-        key_file.write(key)
-    return key
-
-async def callkey():
-  try:
-    key = open("aeseasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await genkey()
-      key = open("aeseasyencryption.key", "rb").read()
-    return key
-  except:
-    await genkey()
-    key = open("aeseasyencryption.key", "rb").read()
-    return key
-
-async def aesencrypt(slogan:str):
-    key = await callkey()
-    BS = AES.block_size
-    pad = lambda s: s + (BS - len(s) % BS) * chr(BS - len(s) % BS)
-
-    slogan = base64.b64encode(pad(slogan).encode('utf8'))
-    iv = Crypto.Random.get_random_bytes(AES.block_size)
-    cipher = AES.new(key=key, mode= AES.MODE_CFB,iv= iv)
-    return base64.b64encode(iv + cipher.encrypt(slogan))
-
-async def aesdecrypt(coded_slogan:bytes):
-    key = await callkey()
-    unpad = lambda s: s[:-ord(s[-1:])]
-
-    coded_slogan = base64.b64decode(coded_slogan)
-    iv = coded_slogan[:AES.block_size]
-    cipher = AES.new(key, AES.MODE_CFB, iv)
+import base64, hashlib, Crypto
+from Cryptodome.Cipher import AES
+
+async def genkey():
+    generated_key = Crypto.Random.new().read(AES.block_size)
+    key = hashlib.sha256(generated_key).digest()
+    with open("aeseasyencryption.key", "wb") as key_file:
+        key_file.write(key)
+    return key
+
+async def callkey():
+  try:
+    key = open("aeseasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await genkey()
+      key = open("aeseasyencryption.key", "rb").read()
+    return key
+  except:
+    await genkey()
+    key = open("aeseasyencryption.key", "rb").read()
+    return key
+
+async def aesencrypt(slogan:str):
+    key = await callkey()
+    BS = AES.block_size
+    pad = lambda s: s + (BS - len(s) % BS) * chr(BS - len(s) % BS)
+
+    slogan = base64.b64encode(pad(slogan).encode('utf8'))
+    iv = Crypto.Random.get_random_bytes(AES.block_size)
+    cipher = AES.new(key=key, mode= AES.MODE_CFB,iv= iv)
+    return base64.b64encode(iv + cipher.encrypt(slogan))
+
+async def aesdecrypt(coded_slogan:bytes):
+    key = await callkey()
+    unpad = lambda s: s[:-ord(s[-1:])]
+
+    coded_slogan = base64.b64decode(coded_slogan)
+    iv = coded_slogan[:AES.block_size]
+    cipher = AES.new(key, AES.MODE_CFB, iv)
     return unpad(base64.b64decode(cipher.decrypt(coded_slogan[AES.block_size:])).decode('utf8'))
```

### Comparing `easyencryption-0.2/src/easyencryption/ascii.py` & `easyencryption-0.2.0.1/src/easyencryption/ascii.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import random, math
-
-async def asciiencrypt(string:str):
-    asciis = []
-    biggest = 0
-    for char in enumerate(string):
-        charascii = ord(char[1])
-        rand = math.floor(random.random() * (126-charascii))
-        if (charascii + rand) > biggest:
-            biggest = charascii + rand
-        asciis.append({"Ascii":charascii, "Rand":rand, "Total":charascii + rand})
-    randadd = math.floor(random.random() * (126-biggest))
-    firststring = ""
-    secondstring = ""
-    for charascii in asciis:
-        firststring += chr(charascii["Total"] + randadd)
-        secondstring += chr(charascii["Rand"] + 65 + randadd)
-    middle = chr(randadd + 65)
-    finalstring = firststring + middle + secondstring
-    return finalstring
-
-async def asciidecrypt(string:str):
-    middle = string[(len(string)-1)//2:(len(string)+2)//2]
-    randadd = ord(middle) - 65
-    h = len(string)//2
-    mod = (len(string) + 1) % 2
-    string = string[:h - mod] + string[h + 1:]
-    encoded, added = string[:len(string)//2], string[len(string)//2:]
-    finalstring = ""
-    iternum = 0
-    for ascii in enumerate(added):
-        add = ord(ascii[1]) - 65 - randadd
-        finalstring += chr(ord(encoded[iternum]) - add - randadd)
-        iternum += 1
+import random, math
+
+async def asciiencrypt(string:str):
+    asciis = []
+    biggest = 0
+    for char in enumerate(string):
+        charascii = ord(char[1])
+        rand = math.floor(random.random() * (126-charascii))
+        if (charascii + rand) > biggest:
+            biggest = charascii + rand
+        asciis.append({"Ascii":charascii, "Rand":rand, "Total":charascii + rand})
+    randadd = math.floor(random.random() * (126-biggest))
+    firststring = ""
+    secondstring = ""
+    for charascii in asciis:
+        firststring += chr(charascii["Total"] + randadd)
+        secondstring += chr(charascii["Rand"] + 65 + randadd)
+    middle = chr(randadd + 65)
+    finalstring = firststring + middle + secondstring
+    return finalstring
+
+async def asciidecrypt(string:str):
+    middle = string[(len(string)-1)//2:(len(string)+2)//2]
+    randadd = ord(middle) - 65
+    h = len(string)//2
+    mod = (len(string) + 1) % 2
+    string = string[:h - mod] + string[h + 1:]
+    encoded, added = string[:len(string)//2], string[len(string)//2:]
+    finalstring = ""
+    iternum = 0
+    for ascii in enumerate(added):
+        add = ord(ascii[1]) - 65 - randadd
+        finalstring += chr(ord(encoded[iternum]) - add - randadd)
+        iternum += 1
     return finalstring
```

### Comparing `easyencryption-0.2/src/easyencryption/fernet.py` & `easyencryption-0.2.0.1/src/easyencryption/fernet.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import os, codecs
-from cryptography.fernet import Fernet, MultiFernet
-
-async def genkey():
-  key = Fernet.generate_key()
-  with open("symeasyencryption.key", "wb") as key_file:
-    key_file.write(key)
-  return key
-
-async def regenkey():
-  if os.path.exists("symeasyencryption.key"):
-    os.remove("symeasyencryption.key")
-  await genkey()
-  
-async def callkey():
-  try:
-    key = open("symeasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await genkey()
-      key = open("symeasyencryption.key", "rb").read()
-    return key
-  except:
-    await genkey()
-    key = open("symeasyencryption.key", "rb").read()
-    return key
-  
-async def genkeys():
-  key1 = Fernet.generate_key()
-  with open("sym1easyencryption.key", "wb") as key_file:
-    key_file.write(key1)
-  key2 = Fernet.generate_key()
-  with open("sym2easyencryption.key", "wb") as key_file:
-    key_file.write(key1)
-  key3 = Fernet.generate_key()
-  with open("sym3easyencryption.key", "wb") as key_file:
-    key_file.write(key1)
-  return [key1, key2, key3]
-
-async def callkeys():
-  try:
-    key1 = open("sym1easyencryption.key", "rb").read()
-    if str(key1) == "b''":
-      await genkeys()
-      key1 = open("sym1easyencryption.key", "rb").read()
-  except:
-    await genkeys()
-    key1 = open("sym1easyencryption.key", "rb").read()
-  try:
-    key2 = open("sym2easyencryption.key", "rb").read()
-    if str(key2) == "b''":
-      await genkeys()
-      key2 = open("sym2easyencryption.key", "rb").read()
-  except:
-    await genkeys()
-    key2 = open("sym2easyencryption.key", "rb").read()
-  try:
-    key3 = open("sym3easyencryption.key", "rb").read()
-    if str(key3) == "b''":
-      await genkeys()
-      key3 = open("sym3easyencryption.key", "rb").read()
-  except:
-    await genkeys()
-    key3 = open("sym3easyencryption.key", "rb").read()
-  return [key1, key2, key3]
-  
-async def fernetencrypt(slogan:str):
-  key = await callkey()
-  slogan = slogan.encode()
-  a = Fernet(key)
-  coded_slogan = a.encrypt(slogan)
-  return coded_slogan
-
-async def fernetdecrypt(coded_slogan:bytes):
-  key = await callkey()
-  b = Fernet(key)
-  decoded_slogan = codecs.decode(b.decrypt(coded_slogan))
-  return decoded_slogan
-
-async def multifernetencrypt(slogan:str):
-  keys = await callkeys()
-  slogan = slogan.encode()
-  a = Fernet(keys[0])
-  b = Fernet(keys[1])
-  c = Fernet(keys[2])
-  f = MultiFernet([a, b, c])
-  coded_slogan = f.encrypt(slogan)
-  return coded_slogan
-
-async def multifernetdecrypt(coded_slogan:bytes):
-  keys = await callkeys()
-  a = Fernet(keys[0])
-  b = Fernet(keys[1])
-  c = Fernet(keys[2])
-  f = MultiFernet([c, b, a])
-  rotated = f.rotate(coded_slogan)
-  decoded_slogan = codecs.decode(b.decrypt(coded_slogan))
-  return decoded_slogan
-
+import os, codecs
+from cryptography.fernet import Fernet, MultiFernet
+
+async def genkey():
+  key = Fernet.generate_key()
+  with open("symeasyencryption.key", "wb") as key_file:
+    key_file.write(key)
+  return key
+
+async def regenkey():
+  if os.path.exists("symeasyencryption.key"):
+    os.remove("symeasyencryption.key")
+  await genkey()
+  
+async def callkey():
+  try:
+    key = open("symeasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await genkey()
+      key = open("symeasyencryption.key", "rb").read()
+    return key
+  except:
+    await genkey()
+    key = open("symeasyencryption.key", "rb").read()
+    return key
+  
+async def genkeys():
+  key1 = Fernet.generate_key()
+  with open("sym1easyencryption.key", "wb") as key_file:
+    key_file.write(key1)
+  key2 = Fernet.generate_key()
+  with open("sym2easyencryption.key", "wb") as key_file:
+    key_file.write(key1)
+  key3 = Fernet.generate_key()
+  with open("sym3easyencryption.key", "wb") as key_file:
+    key_file.write(key1)
+  return [key1, key2, key3]
+
+async def callkeys():
+  try:
+    key1 = open("sym1easyencryption.key", "rb").read()
+    if str(key1) == "b''":
+      await genkeys()
+      key1 = open("sym1easyencryption.key", "rb").read()
+  except:
+    await genkeys()
+    key1 = open("sym1easyencryption.key", "rb").read()
+  try:
+    key2 = open("sym2easyencryption.key", "rb").read()
+    if str(key2) == "b''":
+      await genkeys()
+      key2 = open("sym2easyencryption.key", "rb").read()
+  except:
+    await genkeys()
+    key2 = open("sym2easyencryption.key", "rb").read()
+  try:
+    key3 = open("sym3easyencryption.key", "rb").read()
+    if str(key3) == "b''":
+      await genkeys()
+      key3 = open("sym3easyencryption.key", "rb").read()
+  except:
+    await genkeys()
+    key3 = open("sym3easyencryption.key", "rb").read()
+  return [key1, key2, key3]
+  
+async def fernetencrypt(slogan:str):
+  key = await callkey()
+  slogan = slogan.encode()
+  a = Fernet(key)
+  coded_slogan = a.encrypt(slogan)
+  return coded_slogan
+
+async def fernetdecrypt(coded_slogan:bytes):
+  key = await callkey()
+  b = Fernet(key)
+  decoded_slogan = codecs.decode(b.decrypt(coded_slogan))
+  return decoded_slogan
+
+async def multifernetencrypt(slogan:str):
+  keys = await callkeys()
+  slogan = slogan.encode()
+  a = Fernet(keys[0])
+  b = Fernet(keys[1])
+  c = Fernet(keys[2])
+  f = MultiFernet([a, b, c])
+  coded_slogan = f.encrypt(slogan)
+  return coded_slogan
+
+async def multifernetdecrypt(coded_slogan:bytes):
+  keys = await callkeys()
+  a = Fernet(keys[0])
+  b = Fernet(keys[1])
+  c = Fernet(keys[2])
+  f = MultiFernet([c, b, a])
+  rotated = f.rotate(coded_slogan)
+  decoded_slogan = codecs.decode(b.decrypt(coded_slogan))
+  return decoded_slogan
+
```

### Comparing `easyencryption-0.2/src/easyencryption/rsa.py` & `easyencryption-0.2.0.1/src/easyencryption/rsa.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import os
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_OAEP
-
-async def genkeys():
-    key = RSA.generate(2048)
-    publickey = key.publickey().export_key()
-    privatekey = key.export_key()
-    with open("pubeasyencryption.key", "wb") as pub_key_file:
-        pub_key_file.write(publickey)
-    with open("priveasyencryption.key", "wb") as priv_key_file:
-        priv_key_file.write(privatekey)
-    keys = [publickey, privatekey]
-    return keys
-
-async def regenkeys():
-    if os.path.exists("pubeasyencryption.key"):
-        os.remove("pubeasyencryption.key")
-    if os.path.exists("priveasyencryption.key"):
-        os.remove("priveasyencryption.key")
-    await genkeys()
-
-async def callpubkey():
-  try:
-    key = open("pubeasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await genkeys()
-      key = open("pubeasyencryption.key", "rb").read()
-    key = RSA.import_key(key)
-    return key
-  except:
-    await genkeys()
-    key = open("pubeasyencryption.key", "rb").read()
-    key = RSA.import_key(key)
-    return key
-
-async def callprivkey():
-  try:
-    key = open("priveasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await genkeys()
-      key = open("priveasyencryption.key", "rb").read()
-    key = RSA.import_key(key)
-    return key
-  except:
-    await genkeys()
-    key = open("priveasyencryption.key", "rb").read()
-    key = RSA.import_key(key)
-    return key
-
-async def rsaencrypt(slogan:str):
-    key = await callpubkey()
-    encryptor = PKCS1_OAEP.new(key)
-    coded_slogan = encryptor.encrypt(slogan.encode("utf-8"))
-    return coded_slogan
-
-async def rsadecrypt(coded_slogan:bytes):
-    key = await callprivkey()
-    decryptor = PKCS1_OAEP.new(key)
-    decoded_slogan = decryptor.decrypt(coded_slogan)
-    decoded_slogan = str(decoded_slogan)
-    decoded_slogan = decoded_slogan[2:]
-    decoded_slogan = decoded_slogan[:-1]
-    return decoded_slogan
-
+import os
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_OAEP
+
+async def genkeys():
+    key = RSA.generate(2048)
+    publickey = key.publickey().export_key()
+    privatekey = key.export_key()
+    with open("pubeasyencryption.key", "wb") as pub_key_file:
+        pub_key_file.write(publickey)
+    with open("priveasyencryption.key", "wb") as priv_key_file:
+        priv_key_file.write(privatekey)
+    keys = [publickey, privatekey]
+    return keys
+
+async def regenkeys():
+    if os.path.exists("pubeasyencryption.key"):
+        os.remove("pubeasyencryption.key")
+    if os.path.exists("priveasyencryption.key"):
+        os.remove("priveasyencryption.key")
+    await genkeys()
+
+async def callpubkey():
+  try:
+    key = open("pubeasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await genkeys()
+      key = open("pubeasyencryption.key", "rb").read()
+    key = RSA.import_key(key)
+    return key
+  except:
+    await genkeys()
+    key = open("pubeasyencryption.key", "rb").read()
+    key = RSA.import_key(key)
+    return key
+
+async def callprivkey():
+  try:
+    key = open("priveasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await genkeys()
+      key = open("priveasyencryption.key", "rb").read()
+    key = RSA.import_key(key)
+    return key
+  except:
+    await genkeys()
+    key = open("priveasyencryption.key", "rb").read()
+    key = RSA.import_key(key)
+    return key
+
+async def rsaencrypt(slogan:str):
+    key = await callpubkey()
+    encryptor = PKCS1_OAEP.new(key)
+    coded_slogan = encryptor.encrypt(slogan.encode("utf-8"))
+    return coded_slogan
+
+async def rsadecrypt(coded_slogan:bytes):
+    key = await callprivkey()
+    decryptor = PKCS1_OAEP.new(key)
+    decoded_slogan = decryptor.decrypt(coded_slogan)
+    decoded_slogan = str(decoded_slogan)
+    decoded_slogan = decoded_slogan[2:]
+    decoded_slogan = decoded_slogan[:-1]
+    return decoded_slogan
+
```

### Comparing `easyencryption-0.2/src/easyencryption/sha.py` & `easyencryption-0.2.0.1/src/easyencryption/sha.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import hashlib, codecs, secrets
-
-async def gensalt():
-    generated_salt = secrets.token_hex(32)
-    with open("shasalteasyencryption.key", "wb") as key_file:
-        key_file.write(codecs.encode(generated_salt))
-    return generated_salt
-
-async def callsalt():
-  try:
-    key = open("shasalteasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await gensalt()
-      key = open("shasalteasyencryption.key", "rb").read()
-    return key
-  except:
-    await gensalt()
-    key = open("shasalteasyencryption.key", "rb").read()
-    return key
-
-async def sha224encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.sha3_224(codecs.encode(salt + string))
-    return hashing.hexdigest()
-
-async def sha224check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.sha3_224(codecs.encode(salt + string))
-    return strhashing.hexdigest() == bytes
-
-async def sha256encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.sha3_256(codecs.encode(salt + string))
-    return hashing.hexdigest()
-
-async def sha256check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.sha3_256(codecs.encode(salt + string))
-    return strhashing.hexdigest() == bytes
-
-async def sha384encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.sha3_384(codecs.encode(salt + string))
-    return hashing.hexdigest()
-
-async def sha384check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.sha3_384(codecs.encode(salt + string))
-    return strhashing.hexdigest() == bytes
-
-async def sha512encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.sha3_512(codecs.encode(salt + string))
-    return hashing.hexdigest()
-
-async def sha512check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.sha3_512(codecs.encode(salt + string))
+import hashlib, codecs, secrets
+
+async def gensalt():
+    generated_salt = secrets.token_hex(32)
+    with open("shasalteasyencryption.key", "wb") as key_file:
+        key_file.write(codecs.encode(generated_salt))
+    return generated_salt
+
+async def callsalt():
+  try:
+    key = open("shasalteasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await gensalt()
+      key = open("shasalteasyencryption.key", "rb").read()
+    return key
+  except:
+    await gensalt()
+    key = open("shasalteasyencryption.key", "rb").read()
+    return key
+
+async def sha224encrypt(string:str):
+    salt = codecs.decode(await callsalt())
+    hashing = hashlib.sha3_224(codecs.encode(salt + string))
+    return hashing.hexdigest()
+
+async def sha224check(string:str, bytes:bytes):
+    salt = codecs.decode(await callsalt())
+    strhashing = hashlib.sha3_224(codecs.encode(salt + string))
+    return strhashing.hexdigest() == bytes
+
+async def sha256encrypt(string:str):
+    salt = codecs.decode(await callsalt())
+    hashing = hashlib.sha3_256(codecs.encode(salt + string))
+    return hashing.hexdigest()
+
+async def sha256check(string:str, bytes:bytes):
+    salt = codecs.decode(await callsalt())
+    strhashing = hashlib.sha3_256(codecs.encode(salt + string))
+    return strhashing.hexdigest() == bytes
+
+async def sha384encrypt(string:str):
+    salt = codecs.decode(await callsalt())
+    hashing = hashlib.sha3_384(codecs.encode(salt + string))
+    return hashing.hexdigest()
+
+async def sha384check(string:str, bytes:bytes):
+    salt = codecs.decode(await callsalt())
+    strhashing = hashlib.sha3_384(codecs.encode(salt + string))
+    return strhashing.hexdigest() == bytes
+
+async def sha512encrypt(string:str):
+    salt = codecs.decode(await callsalt())
+    hashing = hashlib.sha3_512(codecs.encode(salt + string))
+    return hashing.hexdigest()
+
+async def sha512check(string:str, bytes:bytes):
+    salt = codecs.decode(await callsalt())
+    strhashing = hashlib.sha3_512(codecs.encode(salt + string))
     return strhashing.hexdigest() == bytes
```

### Comparing `easyencryption-0.2/src/easyencryption/shake.py` & `easyencryption-0.2.0.1/src/easyencryption/blake.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-import hashlib, codecs, secrets
-
-async def gensalt():
-    generated_salt = secrets.token_hex(32)
-    with open("shakesalteasyencryption.key", "wb") as key_file:
-        key_file.write(codecs.encode(generated_salt))
-    return generated_salt
-
-async def callsalt():
-  try:
-    key = open("shakesalteasyencryption.key", "rb").read()
-    if str(key) == "b''":
-      await gensalt()
-      key = open("shakesalteasyencryption.key", "rb").read()
-    return key
-  except:
-    await gensalt()
-    key = open("shakesalteasyencryption.key", "rb").read()
-    return key
-
-async def shake128encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.shake_128(codecs.encode(salt + string))
-    return hashing.hexdigest(16)
-
-async def shake128check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.shake_128(codecs.encode(salt + string))
-    return strhashing.hexdigest(16) == bytes
-
-async def shake256encrypt(string:str):
-    salt = codecs.decode(await callsalt())
-    hashing = hashlib.shake_256(codecs.encode(salt + string))
-    return hashing.hexdigest(32)
-
-async def shake256check(string:str, bytes:bytes):
-    salt = codecs.decode(await callsalt())
-    strhashing = hashlib.shake_256(codecs.encode(salt + string))
-    return strhashing.hexdigest(32) == bytes
+import hashlib, codecs, secrets
+
+async def gensalt():
+    generated_salt = secrets.token_hex(32)
+    with open("blakesalteasyencryption.key", "wb") as key_file:
+        key_file.write(codecs.encode(generated_salt))
+    return generated_salt
+
+async def callsalt():
+  try:
+    key = open("blakesalteasyencryption.key", "rb").read()
+    if str(key) == "b''":
+      await gensalt()
+      key = open("blakesalteasyencryption.key", "rb").read()
+    return key
+  except:
+    await gensalt()
+    key = open("blakesalteasyencryption.key", "rb").read()
+    return key
+
+async def blakeencrypt(string:str):
+    salt = codecs.decode(await callsalt())
+    hashing = hashlib.blake2b(codecs.encode(salt + string))
+    return hashing.hexdigest()
+
+async def blakecheck(string:str, bytes:bytes):
+    salt = codecs.decode(await callsalt())
+    strhashing = hashlib.blake2b(codecs.encode(salt + string))
+    return strhashing.hexdigest() == bytes
```

### Comparing `easyencryption-0.2/src/easyencryption/test_all.py` & `easyencryption-0.2.0.1/src/easyencryption/test_all.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import asyncio
-import pytest
-pytest_plugins = ('pytest_asyncio',)
-
-from .aes import aesencrypt, aesdecrypt
-
-teststr = "TestString"
-
-@pytest.mark.asyncio
-async def test_aes():
-      estr = await aesencrypt(teststr)
-      dstr = await aesdecrypt(estr)
-      if dstr != teststr:
-            raise Exception("AES check failed")
-      else:
-            return dstr == teststr
-
-from .ascii import asciiencrypt, asciidecrypt
-
-@pytest.mark.asyncio
-async def test_ascii():
-      estr = await asciiencrypt(teststr)
-      dstr = await asciidecrypt(estr)
-      if dstr != teststr:
-            raise Exception("ASCII check failed")
-      else:
-            return dstr == teststr
-
-from .blake import blakeencrypt, blakecheck
-
-@pytest.mark.asyncio
-async def test_blake():
-      estr = await blakeencrypt(teststr)
-      dstr = await blakecheck(teststr, estr)
-      if not dstr:
-            raise Exception("Blake check failed")
-      else:
-            return dstr == teststr
-
-from .ecc import eccencrypt, eccdecrypt
-
-@pytest.mark.asyncio
-async def test_ecc():
-      estr = await eccencrypt(teststr)
-      dstr = await eccdecrypt(estr)
-      if dstr != teststr:
-            raise Exception("ECC check failed")
-      else:
-            return dstr == teststr
-      
-from .fernet import fernetencrypt, fernetdecrypt
-
-@pytest.mark.asyncio
-async def test_fernet():
-      estr = await fernetencrypt(teststr)
-      dstr = await fernetdecrypt(estr)
-      if dstr != teststr:
-            raise Exception("Fernet check failed")
-      else:
-            return dstr == teststr
-      
-from .fernet import multifernetencrypt, multifernetdecrypt
-
-@pytest.mark.asyncio
-async def test_multifernet():
-      estr = await multifernetencrypt(teststr)
-      dstr = await multifernetdecrypt(estr)
-      if dstr != teststr:
-            raise Exception("MultiFernet check failed")
-      else:
-            return dstr == teststr
-      
-from .rsa import rsaencrypt, rsadecrypt
-
-@pytest.mark.asyncio
-async def test_rsa():
-      estr = await rsaencrypt(teststr)
-      dstr = await rsadecrypt(estr)
-      if dstr != teststr:
-            raise Exception("RSA check failed")
-      else:
-            return dstr == teststr
-      
-from .sha import sha224encrypt, sha224check
-
-@pytest.mark.asyncio
-async def test_sha224():
-      estr = await sha224encrypt(teststr)
-      dstr = await sha224check(teststr, estr)
-      if not dstr:
-            raise Exception("SHA224 check failed")
-      else:
-            return dstr == teststr
-
-from .sha import sha256encrypt, sha256check
-
-@pytest.mark.asyncio
-async def test_sha256():
-      estr = await sha256encrypt(teststr)
-      dstr = await sha256check(teststr, estr)
-      if not dstr:
-            raise Exception("SHA256 check failed")
-      else:
-            return dstr == teststr
-
-from .sha import sha384encrypt, sha384check
-
-@pytest.mark.asyncio
-async def test_sha384():
-      estr = await sha384encrypt(teststr)
-      dstr = await sha384check(teststr, estr)
-      if not dstr:
-            raise Exception("SHA384 check failed")
-      else:
-            return dstr == teststr
-
-from .sha import sha512encrypt, sha512check
-
-@pytest.mark.asyncio
-async def test_sha512():
-      estr = await sha512encrypt(teststr)
-      dstr = await sha512check(teststr, estr)
-      if not dstr:
-            raise Exception("SHA512 check failed")
-      else:
-            return dstr == teststr
-
-from .shake import shake128encrypt, shake128check
-
-@pytest.mark.asyncio
-async def test_shake128():
-      estr = await shake128encrypt(teststr)
-      dstr = await shake128check(teststr, estr)
-      if not dstr:
-            raise Exception("SHAKE128 check failed")
-      else:
-            return dstr == teststr
-
-from .shake import shake256encrypt, shake256check
-
-@pytest.mark.asyncio
-async def test_shake256():
-      estr = await shake256encrypt(teststr)
-      dstr = await shake256check(teststr, estr)
-      if not dstr:
-            raise Exception("SHAKE256 check failed")
-      else:
-            return dstr == teststr
-      
-from .xor import xorencrypt, xordecrypt
-
-@pytest.mark.asyncio
-async def test_xor():
-      estr = await xorencrypt(teststr)
-      dstr = await xordecrypt(estr)
-      if dstr != teststr:
-            raise Exception("XOR check failed")
-      else:
-            return dstr == teststr
-
+import asyncio
+import pytest
+pytest_plugins = ('pytest_asyncio',)
+
+from .aes import aesencrypt, aesdecrypt
+
+teststr = "TestString"
+
+@pytest.mark.asyncio
+async def test_aes():
+      estr = await aesencrypt(teststr)
+      dstr = await aesdecrypt(estr)
+      if dstr != teststr:
+            raise Exception("AES check failed")
+      else:
+            return dstr == teststr
+
+from .ascii import asciiencrypt, asciidecrypt
+
+@pytest.mark.asyncio
+async def test_ascii():
+      estr = await asciiencrypt(teststr)
+      dstr = await asciidecrypt(estr)
+      if dstr != teststr:
+            raise Exception("ASCII check failed")
+      else:
+            return dstr == teststr
+
+from .blake import blakeencrypt, blakecheck
+
+@pytest.mark.asyncio
+async def test_blake():
+      estr = await blakeencrypt(teststr)
+      dstr = await blakecheck(teststr, estr)
+      if not dstr:
+            raise Exception("Blake check failed")
+      else:
+            return dstr == teststr
+
+from .ecc import eccencrypt, eccdecrypt
+
+@pytest.mark.asyncio
+async def test_ecc():
+      estr = await eccencrypt(teststr)
+      dstr = await eccdecrypt(estr)
+      if dstr != teststr:
+            raise Exception("ECC check failed")
+      else:
+            return dstr == teststr
+      
+from .fernet import fernetencrypt, fernetdecrypt
+
+@pytest.mark.asyncio
+async def test_fernet():
+      estr = await fernetencrypt(teststr)
+      dstr = await fernetdecrypt(estr)
+      if dstr != teststr:
+            raise Exception("Fernet check failed")
+      else:
+            return dstr == teststr
+      
+from .fernet import multifernetencrypt, multifernetdecrypt
+
+@pytest.mark.asyncio
+async def test_multifernet():
+      estr = await multifernetencrypt(teststr)
+      dstr = await multifernetdecrypt(estr)
+      if dstr != teststr:
+            raise Exception("MultiFernet check failed")
+      else:
+            return dstr == teststr
+      
+from .rsa import rsaencrypt, rsadecrypt
+
+@pytest.mark.asyncio
+async def test_rsa():
+      estr = await rsaencrypt(teststr)
+      dstr = await rsadecrypt(estr)
+      if dstr != teststr:
+            raise Exception("RSA check failed")
+      else:
+            return dstr == teststr
+      
+from .sha import sha224encrypt, sha224check
+
+@pytest.mark.asyncio
+async def test_sha224():
+      estr = await sha224encrypt(teststr)
+      dstr = await sha224check(teststr, estr)
+      if not dstr:
+            raise Exception("SHA224 check failed")
+      else:
+            return dstr == teststr
+
+from .sha import sha256encrypt, sha256check
+
+@pytest.mark.asyncio
+async def test_sha256():
+      estr = await sha256encrypt(teststr)
+      dstr = await sha256check(teststr, estr)
+      if not dstr:
+            raise Exception("SHA256 check failed")
+      else:
+            return dstr == teststr
+
+from .sha import sha384encrypt, sha384check
+
+@pytest.mark.asyncio
+async def test_sha384():
+      estr = await sha384encrypt(teststr)
+      dstr = await sha384check(teststr, estr)
+      if not dstr:
+            raise Exception("SHA384 check failed")
+      else:
+            return dstr == teststr
+
+from .sha import sha512encrypt, sha512check
+
+@pytest.mark.asyncio
+async def test_sha512():
+      estr = await sha512encrypt(teststr)
+      dstr = await sha512check(teststr, estr)
+      if not dstr:
+            raise Exception("SHA512 check failed")
+      else:
+            return dstr == teststr
+
+from .shake import shake128encrypt, shake128check
+
+@pytest.mark.asyncio
+async def test_shake128():
+      estr = await shake128encrypt(teststr)
+      dstr = await shake128check(teststr, estr)
+      if not dstr:
+            raise Exception("SHAKE128 check failed")
+      else:
+            return dstr == teststr
+
+from .shake import shake256encrypt, shake256check
+
+@pytest.mark.asyncio
+async def test_shake256():
+      estr = await shake256encrypt(teststr)
+      dstr = await shake256check(teststr, estr)
+      if not dstr:
+            raise Exception("SHAKE256 check failed")
+      else:
+            return dstr == teststr
+      
+from .xor import xorencrypt, xordecrypt
+
+@pytest.mark.asyncio
+async def test_xor():
+      estr = await xorencrypt(teststr)
+      dstr = await xordecrypt(estr)
+      if dstr != teststr:
+            raise Exception("XOR check failed")
+      else:
+            return dstr == teststr
+
```

### Comparing `easyencryption-0.2/src/easyencryption/xor.py` & `easyencryption-0.2.0.1/src/easyencryption/xor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import base64, random, string, codecs, itertools
-
-async def genkey():
-  key = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(64))
-  with open("xoreasyencryption.key", "wb") as key_file:
-    key_file.write(codecs.encode(key))
-  return key
-  
-async def callkey():
-  try:
-    key = codecs.decode(open("xoreasyencryption.key", "rb").read())
-    if str(key) == "b''":
-      await genkey()
-      key = codecs.decode(open("xoreasyencryption.key", "rb").read())
-    return key
-  except:
-    await genkey()
-    key = codecs.decode(open("xoreasyencryption.key", "rb").read())
-    return key
-
-async def crypt(data:str, key=None, encode = False, decode = False):
-   if key == None:
-     key = await callkey()
-   if decode:
-      data = base64.b64decode(data)
-      data = data.decode('ascii')
-   xored = ''.join(chr(ord(x) ^ ord(y)) for (x,y) in zip(data, itertools.cycle(key)))
-   
-   if encode:
-      xored = xored.encode('ascii')
-      return base64.b64encode(xored).strip()
-   return xored
-
-async def xorencrypt(slogan:str):
-      key = await callkey()
-      return await crypt(slogan, key=key, encode = True)
-
-async def xordecrypt(coded_slogan:bytes):
-      key = await callkey()
+import base64, random, string, codecs, itertools
+
+async def genkey():
+  key = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(64))
+  with open("xoreasyencryption.key", "wb") as key_file:
+    key_file.write(codecs.encode(key))
+  return key
+  
+async def callkey():
+  try:
+    key = codecs.decode(open("xoreasyencryption.key", "rb").read())
+    if str(key) == "b''":
+      await genkey()
+      key = codecs.decode(open("xoreasyencryption.key", "rb").read())
+    return key
+  except:
+    await genkey()
+    key = codecs.decode(open("xoreasyencryption.key", "rb").read())
+    return key
+
+async def crypt(data:str, key=None, encode = False, decode = False):
+   if key == None:
+     key = await callkey()
+   if decode:
+      data = base64.b64decode(data)
+      data = data.decode('ascii')
+   xored = ''.join(chr(ord(x) ^ ord(y)) for (x,y) in zip(data, itertools.cycle(key)))
+   
+   if encode:
+      xored = xored.encode('ascii')
+      return base64.b64encode(xored).strip()
+   return xored
+
+async def xorencrypt(slogan:str):
+      key = await callkey()
+      return await crypt(slogan, key=key, encode = True)
+
+async def xordecrypt(coded_slogan:bytes):
+      key = await callkey()
       return await crypt(coded_slogan, key=key, decode = True)
```

### Comparing `easyencryption-0.2/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.2.0.1/src/easyencryption.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: easyencryption
-Version: 0.2.0.0
-Summary: A very easy way to encrypt data.
-Home-page: https://github.com/BlazenBoi/easyencryption/issues
-Author: Blazen
-Author-email: contact@fireballbot.com
-License: MIT
-Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
-Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
-Project-URL: Source, https://github.com/BlazenBoi/easyencryption
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools>=42
-Requires-Dist: cryptography
-Requires-Dist: pycryptodomex
-Requires-Dist: pycryptodome
-Requires-Dist: wheel
-Requires-Dist: eciespy
-
-In Progress...
-
-
-We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
+Metadata-Version: 2.1
+Name: easyencryption
+Version: 0.2.0.1
+Summary: A very easy way to encrypt data.
+Home-page: https://github.com/BlazenBoi/easyencryption/issues
+Author: Blazen
+Author-email: contact@fireballbot.com
+License: MIT
+Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
+Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
+Project-URL: Source, https://github.com/BlazenBoi/easyencryption
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
+
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-0.2/src/easyencryption.egg-info/SOURCES.txt` & `easyencryption-0.2.0.1/src/easyencryption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

