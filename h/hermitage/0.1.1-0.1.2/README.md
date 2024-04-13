# Comparing `tmp/hermitage-0.1.1.tar.gz` & `tmp/hermitage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.1.tar", max compression
+gzip compressed data, was "hermitage-0.1.2.tar", max compression
```

## Comparing `hermitage-0.1.1.tar` & `hermitage-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage-0.1.1/README.md
--rw-r--r--   0        0        0      261 2024-04-02 15:23:42.889428 hermitage-0.1.1/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.1/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11824 2024-04-02 15:23:42.889642 hermitage-0.1.1/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.1/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1035 2024-04-11 07:57:07.718429 hermitage-0.1.1/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.1/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-05 16:44:15.856958 hermitage-0.1.1/hermitage/parsers/query.py
--rw-r--r--   0        0        0      271 2024-04-12 12:56:03.500345 hermitage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 hermitage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage-0.1.2/README.md
+-rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.2/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.2/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.2/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.2/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1020 2024-04-13 13:50:37.613982 hermitage-0.1.2/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.2/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.2/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      356 2024-04-13 13:47:50.456971 hermitage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 hermitage-0.1.2/PKG-INFO
```

### Comparing `hermitage-0.1.1/hermitage/definition/contracts.py` & `hermitage-0.1.2/hermitage/definition/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import functools
 import typing
 import uuid
 import enum
 import itertools
 from collections import deque
 
-from ext.zodchy import codex
+from zodchy import codex
 
 
 class Address:
     def __init__(self, value: str):
         self.value = value
 
     def __str__(self):
```

### Comparing `hermitage-0.1.1/hermitage/mappers/invoice.py` & `hermitage-0.1.2/hermitage/mappers/invoice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ext.zodchy import codex
-from ext import zodchy_patterns as patterns
+import zodchy
+import zodchy_patterns
 from ..definition import contracts
 
 
 class ClauseInjector:
     def __init__(
         self,
-        reference: patterns.Reference,
+        reference: zodchy_patterns.Reference,
         search_key: str,
         injection_key: str | None = None
     ):
         super().__init__()
         self._search_key = search_key
         self._injection_key = injection_key
         self._reference = reference
 
     def __call__(self, clause: contracts.Clause):
         if str(clause.address) == self._search_key:
             operation = clause.operation
-            if isinstance(operation, codex.query.SET):
-                operation = codex.query.SET(
+            if isinstance(operation, zodchy.codex.query.SET):
+                operation = zodchy.codex.query.SET(
                     *[self._reference(v) for v in operation.value]
                 )
             else:
                 operation = type(operation)(self._reference(operation.value))
             clause = contracts.Clause(
                 contracts.Address(self._injection_key),
                 operation
```

### Comparing `hermitage-0.1.1/hermitage/parsers/query.py` & `hermitage-0.1.2/hermitage/parsers/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import collections.abc
 import inspect
 import typing
 
-from ext.zodchy import codex
+from zodchy import codex
 from ..definition import contracts
 
 
 class QueryParser:
     def __init__(self, query: codex.Query):
         self._query = query
         self._mappers = None
```

