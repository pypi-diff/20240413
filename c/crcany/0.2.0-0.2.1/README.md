# Comparing `tmp/crcany-0.2.tar.gz` & `tmp/crcany-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crcany-0.2.tar", last modified: Fri Apr 12 21:32:25 2024, max compression
+gzip compressed data, was "crcany-0.2.1.tar", last modified: Fri Apr 12 22:33:40 2024, max compression
```

## Comparing `crcany-0.2.tar` & `crcany-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.335497 crcany-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 21:32:21.000000 crcany-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-12 21:32:25.335497 crcany-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-12 21:32:21.000000 crcany-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.331498 crcany-0.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.335497 crcany-0.2/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-12 21:32:21.000000 crcany-0.2/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)    18026 2024-04-12 21:32:21.000000 crcany-0.2/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 21:32:21.000000 crcany-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:32:25.335497 crcany-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 21:32:21.000000 crcany-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.335497 crcany-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.335497 crcany-0.2/src/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 21:32:21.000000 crcany-0.2/src/crcany/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 21:32:21.000000 crcany-0.2/src/crcany/crcany.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-04-12 21:32:21.000000 crcany-0.2/src/crcany/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:32:25.335497 crcany-0.2/src/crcany.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-12 21:32:25.000000 crcany-0.2/src/crcany.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 21:32:25.000000 crcany-0.2/src/crcany.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:32:25.000000 crcany-0.2/src/crcany.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 21:32:25.000000 crcany-0.2/src/crcany.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.655871 crcany-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 22:33:35.000000 crcany-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-12 22:33:40.655871 crcany-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 22:33:35.000000 crcany-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.651871 crcany-0.2.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.655871 crcany-0.2.1/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-12 22:33:35.000000 crcany-0.2.1/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18026 2024-04-12 22:33:35.000000 crcany-0.2.1/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 22:33:35.000000 crcany-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:33:40.655871 crcany-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 22:33:35.000000 crcany-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.651871 crcany-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.655871 crcany-0.2.1/src/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 22:33:35.000000 crcany-0.2.1/src/crcany/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-12 22:33:35.000000 crcany-0.2.1/src/crcany/crcany.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-12 22:33:35.000000 crcany-0.2.1/src/crcany/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:33:40.655871 crcany-0.2.1/src/crcany.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-12 22:33:40.000000 crcany-0.2.1/src/crcany.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 22:33:40.000000 crcany-0.2.1/src/crcany.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:33:40.000000 crcany-0.2.1/src/crcany.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:33:40.000000 crcany-0.2.1/src/crcany.egg-info/top_level.txt
```

### Comparing `crcany-0.2/LICENSE` & `crcany-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crcany-0.2/PKG-INFO` & `crcany-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,51 @@
-Metadata-Version: 2.1
-Name: crcany
-Version: 0.2.0
-Summary: Python CRC Computation Library
-Project-URL: Homepage, https://github.com/marzooqy/crcany
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## crcany
-
-The fastest Python CRC computation library available.
-
-This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
-
-## Installation
-
-`pip install crcany`
-
-## Usage
-
-Use an existing model:
-
-```python
->>> import crcany
->>> data = b'Hello World!'
->>> crc32 = crcany.Model('CRC32/ISO-HDLC')
->>> crc32.calc(data)
-472456355
-```
-
-Read the data in chunks:
-
-```python
->>> crc32.reset() #set to the initial value
->>> crc32.calc(b'Hello ')
-3928882368
->>> crc32.calc(b'World!')
-472456355
-```
-
-Specify your own CRC parameters:
-
-```python
->>> # width, poly, init, refin, refout, xorout
->>> my_crc = crcany.CRC(10, 0b0101010101, 0x3ff, True, False, 0)
->>> my_crc.calc('Hello World!')
-35
-```
-
-## Benchmarks
-
-Calculating the CRC32 for lorem ipsum 10 million times:
-
-```
-crcany
-Time Elapsed: 7.732s
-Average: 0.773 us/run
-Relative: 1.000
-
-binascii
-Time Elapsed: 7.612s
-Average: 0.761 us/run
-Relative: 0.984
-
-fastcrc
-Time Elapsed: 16.483s
-Average: 1.648 us/run
-Relative: 2.132
-
-crcmod-plus
-Time Elapsed: 18.259s
-Average: 1.826 us/run
-Relative: 2.361
-```
+The fastest Python CRC library available.
+
+This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
+
+## Installation
+
+`pip install crcany`
+
+## Usage
+
+Use an existing model:
+
+```python
+>>> import crcany
+>>> data = b'Hello World!'
+>>> crc32 = crcany.Model('CRC32/ISO-HDLC')
+>>> crc32.calc(data)
+472456355
+```
+
+Read the data in chunks:
+
+```python
+>>> crc32.reset() #set to the initial value
+>>> crc32.calc(b'Hello ')
+3928882368
+>>> crc32.calc(b'World!')
+472456355
+```
+
+Specify your own CRC parameters:
+
+```python
+>>> # width, poly, init, refin, refout, xorout
+>>> my_crc = crcany.CRC(10, 0b0101010101, 0x3ff, True, False, 0)
+>>> my_crc.calc('Hello World!')
+35
+```
+
+For a list of pre-built models, check [models.py](https://github.com/marzooqy/crcany/blob/main/src/crcany/models.py)
+
+## Benchmarks
+
+Calculating the CRC32 for lorem ipsum 10 million times:
+
+| Module | Time Elapsed | Average | Relative |
+|---|:-:|:-:|:-:|
+| crcany | 7.732s | 0.773 us/run | 1.000 |
+| binascii | 7.612s | 0.761 us/run | 0.984 |
+| fastcrc | 16.483s | 1.648 us/run | 2.132 |
+| crcmod-plus | 18.259s | 1.826 us/run | 2.361 |
```

### Comparing `crcany-0.2/lib/crcany/crc.c` & `crcany-0.2.1/lib/crcany/crc.c`

 * *Files identical despite different names*

### Comparing `crcany-0.2/lib/crcany/model.c` & `crcany-0.2.1/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `crcany-0.2/src/crcany/crcany.pyx` & `crcany-0.2.1/src/crcany/crcany.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2024 Hussain Al Marzooq
+# Copyright (c) 2024 Hussain Al Marzooq
 
 from libc.stdint cimport uintmax_t
 from .models import models
 import sys
 
 ctypedef uintmax_t word_t
 
@@ -33,19 +33,19 @@
     cdef void crc_table_wordwise(model_t *model, unsigned little, unsigned bits)
     cdef word_t crc_wordwise(model_t *model, word_t crc, const void* dat, size_t len)
 
 cdef class CRC:
     cdef model_t model
     cdef word_t register
     
-    def __init__(self, unsigned short width, word_t poly, word_t init, char ref_in, char ref_out, word_t xor_out, word_t check=0, word_t residue=0, name=''):
+    def __init__(self, unsigned short width, word_t poly, word_t init, char ref_in, char ref_out, word_t xor_out, word_t check=0, word_t residue=0):
         refin = 'true' if ref_in else 'false'
         refout = 'true' if ref_out else 'false'
         
-        string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name="{name}"'.encode('utf-8')
+        string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name=""'.encode('utf-8')
         cdef int error_code = read_model(&self.model, string, 0)
         
         if error_code != 0:
             raise ValueError('An error occurred while retrieving the model, check the arguments passed to the CRC class')
             
         process_model(&self.model)
         crc_table_bytewise(&self.model)
@@ -65,8 +65,8 @@
         self.register = crc
         return crc
         
     def reset(self):
         self.register = self.model.init
         
 def Model(name):
-    return CRC(*models[name])
+    return CRC(*models[name])
```

