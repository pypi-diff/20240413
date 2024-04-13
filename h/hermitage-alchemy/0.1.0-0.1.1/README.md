# Comparing `tmp/hermitage_alchemy-0.1.0.tar.gz` & `tmp/hermitage_alchemy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.1.0.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.1.1.tar", max compression
```

## Comparing `hermitage_alchemy-0.1.0.tar` & `hermitage_alchemy-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage_alchemy-0.1.0/README.md
--rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.0/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10318 2024-04-02 15:23:42.890253 hermitage_alchemy-0.1.0/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      824 2024-04-02 15:23:42.890336 hermitage_alchemy-0.1.0/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.0/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.0/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0     2766 2024-04-11 07:57:07.718686 hermitage_alchemy-0.1.0/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.0/hermitage_alchemy/definition/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.0/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6220 2024-04-02 15:23:42.891182 hermitage_alchemy-0.1.0/hermitage_alchemy/execution/fetching.py
--rw-r--r--   0        0        0     3933 2024-04-02 15:23:42.891290 hermitage_alchemy-0.1.0/hermitage_alchemy/execution/storing.py
--rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/__init__.py
--rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/generic.py
--rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/total.py
--rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/upsert.py
--rw-r--r--   0        0        0      279 2024-04-12 12:57:30.290154 hermitage_alchemy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage_alchemy-0.1.1/README.md
+-rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.1/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.1/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.1/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.1/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/fetching.py
+-rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/storing.py
+-rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/generic.py
+-rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/total.py
+-rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/upsert.py
+-rw-r--r--   0        0        0      416 2024-04-13 14:00:48.255293 hermitage_alchemy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.1/PKG-INFO
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/__init__.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/assembling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import abc
 import collections.abc
 import operator
 import functools
 from collections import deque
 
 import sqlalchemy
-from ext.zodchy import codex
+import hermitage
+
 from .definition import contracts
 from .configuration import Schema
 
 
 class ClauseCompiler(abc.ABC):
     def __init__(
         self,
@@ -26,25 +27,25 @@
     def _compile(self, clause: contracts.Clause) -> sqlalchemy.ClauseElement: ...
 
 
 class FilterCompiler(ClauseCompiler):
     @property
     def _operations(self):
         return {
-            codex.query.EQ: self._simple_clause(operator.eq),
-            codex.query.NE: self._simple_clause(operator.ne),
-            codex.query.LE: self._simple_clause(operator.le),
-            codex.query.LT: self._simple_clause(operator.lt),
-            codex.query.GE: self._simple_clause(operator.ge),
-            codex.query.GT: self._simple_clause(operator.gt),
-            codex.query.IS: lambda v: self._get_column(v).is_(v.operation.value),
-            codex.query.LIKE: self._like_clause,
-            codex.query.NOT: self._not_clause,
-            codex.query.SET: self._set_clause,
-            codex.query.RANGE: self._range_clause,
+            hermitage.query.EQ: self._simple_clause(operator.eq),
+            hermitage.query.NE: self._simple_clause(operator.ne),
+            hermitage.query.LE: self._simple_clause(operator.le),
+            hermitage.query.LT: self._simple_clause(operator.lt),
+            hermitage.query.GE: self._simple_clause(operator.ge),
+            hermitage.query.GT: self._simple_clause(operator.gt),
+            hermitage.query.IS: lambda v: self._get_column(v).is_(v.operation.value),
+            hermitage.query.LIKE: self._like_clause,
+            hermitage.query.NOT: self._not_clause,
+            hermitage.query.SET: self._set_clause,
+            hermitage.query.RANGE: self._range_clause,
         }
 
     def _compile(self, clause: contracts.Clause) -> sqlalchemy.ClauseElement:
         if clause.address:
             return self._operations[type(clause.operation)](clause)
 
         stack = deque()
@@ -60,24 +61,24 @@
 
         return stack.pop()
 
     def _get_column(self, clause: contracts.Clause) -> sqlalchemy.Column:
         return self._schema.get_column(clause)
 
     def _not_clause(self, clause: contracts.Clause):
-        if isinstance(clause.operation, codex.query.IS):
+        if isinstance(clause.operation, hermitage.query.IS):
             return self._get_column(clause).isnot(clause.operation.value)
-        elif isinstance(clause.operation, codex.query.EQ):
+        elif isinstance(clause.operation, hermitage.query.EQ):
             return operator.ne(self._get_column(clause), clause.operation.value)
-        elif isinstance(clause.operation, codex.query.LIKE):
+        elif isinstance(clause.operation, hermitage.query.LIKE):
             return self._like_clause(
                 contracts.Clause(clause.address, clause.operation),
                 inversion=True
             )
-        elif isinstance(clause.operation, codex.query.SET):
+        elif isinstance(clause.operation, hermitage.query.SET):
             return self._set_clause(
                 contracts.Clause(clause.address, clause.operation),
                 inversion=True
             )
         else:
             return sqlalchemy.not_(self._compile(clause)),
 
@@ -119,16 +120,16 @@
     def __call__(self, condition: contracts.Clause) -> list[sqlalchemy.ClauseElement]:
         result = self._compile(condition)
         return result
 
     @property
     def _operations(self):
         return {
-            codex.query.ASC: sqlalchemy.asc,
-            codex.query.DESC: sqlalchemy.desc
+            hermitage.query.ASC: sqlalchemy.asc,
+            hermitage.query.DESC: sqlalchemy.desc
         }
 
     def _compile(self, clause: contracts.Clause) -> list[sqlalchemy.ClauseElement]:
         stack = deque()
         result = []
         for element in clause or ():
             if element is contracts.LogicalOperator.AND:
@@ -226,15 +227,15 @@
                 self._parse_invoice(
                     invoice=contracts.Invoice(nested_namespace, *nested_invoice),
                     prefix=nested_item.name
                 )
                 _joins_index.add(str(link))
 
         for clause in filter(
-            lambda x: codex.query.FilterBit in x.kind.__mro__ and len(x.namespace) > 1,
+            lambda x: hermitage.query.FilterBit in x.kind.__mro__ and len(x.namespace) > 1,
             invoice.clauses
         ):
             if link := self._schema.get_m2o(clause.namespace):
                 if str(link) not in _joins_index:
                     self._joins.append((
                         link.source_table(),
                         link.target_table(),
@@ -251,31 +252,31 @@
                     self._order,
                     self._limit,
                     self._offset
                 )
 
     @functools.cached_property
     def _filter_clause(self) -> contracts.Clause | None:
-        clauses = filter(lambda x: codex.query.FilterBit in x.kind.__mro__, self._clauses)
+        clauses = filter(lambda x: hermitage.query.FilterBit in x.kind.__mro__, self._clauses)
         try:
             result = functools.reduce(operator.and_, clauses)
             return result
         except TypeError:
             return
 
     @functools.cached_property
     def _limit_clause(self) -> contracts.Clause | None:
-        for clause in filter(lambda x: isinstance(x.operation, codex.query.Limit), self._clauses):
+        for clause in filter(lambda x: isinstance(x.operation, hermitage.query.Limit), self._clauses):
             return clause
 
     @functools.cached_property
     def _offset_clause(self) -> contracts.Clause | None:
-        for clause in filter(lambda x: isinstance(x.operation, codex.query.Offset), self._clauses):
+        for clause in filter(lambda x: isinstance(x.operation, hermitage.query.Offset), self._clauses):
             return clause
 
     @functools.cached_property
     def _order_clause(self) -> contracts.Clause | None:
-        clauses = filter(lambda x: codex.query.OrderBit in x.kind.__mro__, self._clauses)
+        clauses = filter(lambda x: hermitage.query.OrderBit in x.kind.__mro__, self._clauses)
         try:
             return functools.reduce(operator.and_, clauses)
         except TypeError:
             return
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/bootstraping.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import typing
+
 from sqlalchemy.ext.asyncio import create_async_engine
+
 from .definition import contracts
 
 
 def get_engine(dsn: str) -> contracts.AsyncEngineContract:
     return typing.cast(
         contracts.AsyncEngineContract,
         create_async_engine(
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/definition/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 import functools
 import dataclasses
 
 import sqlalchemy.ext.asyncio
 import collections.abc
 
-from ext.hermitage.definition import contracts as hermitage_contracts
+from hermitage.definition import contracts as hermitage_contracts
 
 AsyncEngineContract = sqlalchemy.ext.asyncio.AsyncEngine
 AsyncConnectionContract = sqlalchemy.ext.asyncio.AsyncConnection
 StorageBucketCollectionContract = collections.abc.Iterable[sqlalchemy.Table]
 
 Namespace = hermitage_contracts.Namespace
 Address = hermitage_contracts.Address
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/definition/exceptions.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/execution/fetching.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/execution/fetching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections.abc
 import functools
 import typing
 
-from ext.zodchy import codex
+import hermitage
+
 from ..configuration import Schema
 from ..assembling import QueryBuilder
 from ..definition import contracts
 
 ResultDataType = collections.abc.Iterable[collections.abc.Mapping]
 
 
@@ -97,15 +98,15 @@
                     self._schema.get_fk_table_alias(link.interim_target_column),
                     *item.invoice
                 )
             )
         )
         nested_invoice += contracts.Clause(
             link.interim_source_column,
-            codex.query.SET(*(r.get(str(link.source_column)) for r in data))
+            hermitage.query.SET(*(r.get(str(link.source_column)) for r in data))
         )
         nested_result = await self._launch_invoice(nested_invoice)
         index = collections.defaultdict(list)
         for row in nested_result[0]:
             index[row[str(link.interim_source_column)]].append(
                 {k.replace(f'{item.name}__', ''): v for k, v in row.items() if k.startswith(item.name)}
             )
@@ -127,15 +128,15 @@
         nested_invoice = item.invoice
         nested_invoice += contracts.Item(
             str(link.target_column),
             link.target_column
         )
         nested_invoice += contracts.Clause(
             link.target_column,
-            codex.query.SET(*(r.get(str(link.source_column)) for r in data))
+            hermitage.query.SET(*(r.get(str(link.source_column)) for r in data))
         )
         nested_result = await self._launch_invoice(nested_invoice)
         index = collections.defaultdict(list)
         for row in nested_result[0]:
             index[row[str(link.target_column)]].append(
                 {k: v for k, v in row.items() if k in original_items}
             )
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/execution/storing.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/execution/storing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections.abc
 
 import sqlalchemy
 
-from ext.hermitage.definition import contracts
+from hermitage.definition import contracts
 from ..configuration import Schema
 from ..assembling import FilterCompiler
 from ..definition import contracts
 
 SaverDataContract = contracts.Row | contracts.Clause
```

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/total.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/total.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.0/hermitage_alchemy/plugins/upsert.py` & `hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/upsert.py`

 * *Files identical despite different names*

