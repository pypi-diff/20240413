# Comparing `tmp/xian_contracting-0.1.1.tar.gz` & `tmp/xian_contracting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xian_contracting-0.1.1.tar", max compression
+gzip compressed data, was "xian_contracting-0.1.2.tar", max compression
```

## Comparing `xian_contracting-0.1.1.tar` & `xian_contracting-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    35149 2024-02-28 22:50:02.409938 xian_contracting-0.1.1/LICENSE
--rw-r--r--   0        0        0     1389 2024-03-25 17:29:18.195376 xian_contracting-0.1.1/README.md
--rw-r--r--   0        0        0      365 2024-03-25 17:54:37.140950 xian_contracting-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       85 2024-02-28 22:50:02.410206 xian_contracting-0.1.1/xian_contracting/.gitignore
--rw-r--r--   0        0        0        7 2024-02-28 22:50:02.410260 xian_contracting-0.1.1/xian_contracting/.version
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.410283 xian_contracting-0.1.1/xian_contracting/__init__.py
--rw-r--r--   0        0        0    11855 2024-03-25 17:49:21.962374 xian_contracting-0.1.1/xian_contracting/client.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.410481 xian_contracting-0.1.1/xian_contracting/compilation/__init__.py
--rw-r--r--   0        0        0     4046 2024-03-25 17:49:21.936801 xian_contracting-0.1.1/xian_contracting/compilation/compiler.py
--rw-r--r--   0        0        0    11681 2024-03-25 17:49:21.970424 xian_contracting-0.1.1/xian_contracting/compilation/linter.py
--rw-r--r--   0        0        0     1431 2024-02-28 22:50:02.410726 xian_contracting-0.1.1/xian_contracting/compilation/parser.py
--rw-r--r--   0        0        0     2726 2024-02-28 22:50:02.410794 xian_contracting-0.1.1/xian_contracting/compilation/whitelists.py
--rw-r--r--   0        0        0      670 2024-02-28 22:50:02.410863 xian_contracting-0.1.1/xian_contracting/config.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.410919 xian_contracting-0.1.1/xian_contracting/contracts/__init__.py
--rw-r--r--   0        0        0      931 2024-02-28 22:50:02.410991 xian_contracting-0.1.1/xian_contracting/contracts/submission.s.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.411045 xian_contracting-0.1.1/xian_contracting/db/__init__.py
--rw-r--r--   0        0        0     1389 2024-03-25 17:49:21.959370 xian_contracting-0.1.1/xian_contracting/db/contract.py
--rw-r--r--   0        0        0    27568 2024-03-25 17:49:21.925727 xian_contracting-0.1.1/xian_contracting/db/driver.py
--rw-r--r--   0        0        0     5541 2024-03-25 17:49:21.945668 xian_contracting-0.1.1/xian_contracting/db/encoder.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.411406 xian_contracting-0.1.1/xian_contracting/db/hdf5/__init__.py
--rw-r--r--   0        0        0     5984 2024-02-28 22:50:02.411515 xian_contracting-0.1.1/xian_contracting/db/hdf5/h5c.c
--rw-r--r--   0        0        0     4590 2024-03-25 17:49:21.941364 xian_contracting-0.1.1/xian_contracting/db/orm.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.411668 xian_contracting-0.1.1/xian_contracting/execution/__init__.py
--rw-r--r--   0        0        0     8623 2024-03-25 17:49:21.954694 xian_contracting-0.1.1/xian_contracting/execution/executor.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.411847 xian_contracting-0.1.1/xian_contracting/execution/metering/__init__.py
--rw-r--r--   0        0        0      887 2024-02-28 22:50:02.411935 xian_contracting-0.1.1/xian_contracting/execution/metering/cu_costs.const
--rw-r--r--   0        0        0     1540 2024-02-28 22:50:02.412017 xian_contracting-0.1.1/xian_contracting/execution/metering/datastack.h
--rw-r--r--   0        0        0      685 2024-02-28 22:50:02.412097 xian_contracting-0.1.1/xian_contracting/execution/metering/filedisp.h
--rw-r--r--   0        0        0      709 2024-02-28 22:50:02.412166 xian_contracting-0.1.1/xian_contracting/execution/metering/stats.h
--rw-r--r--   0        0        0    12772 2024-02-28 22:50:02.412305 xian_contracting-0.1.1/xian_contracting/execution/metering/tracer.c
--rw-r--r--   0        0        0     1985 2024-02-28 22:50:02.412366 xian_contracting-0.1.1/xian_contracting/execution/metering/tracer.h
--rw-r--r--   0        0        0     2994 2024-02-28 22:50:02.412425 xian_contracting-0.1.1/xian_contracting/execution/metering/util.h
--rw-r--r--   0        0        0     4153 2024-03-25 17:49:21.968220 xian_contracting-0.1.1/xian_contracting/execution/module.py
--rw-r--r--   0        0        0     3079 2024-03-25 17:49:21.949607 xian_contracting-0.1.1/xian_contracting/execution/runtime.py
--rw-r--r--   0        0        0     5027 2024-02-28 22:50:02.412698 xian_contracting-0.1.1/xian_contracting/hlcpy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.412762 xian_contracting-0.1.1/xian_contracting/stdlib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 22:50:02.412841 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/__init__.py
--rw-r--r--   0        0        0     1183 2024-03-25 17:49:21.928873 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/access.py
--rw-r--r--   0        0        0     4738 2024-02-28 22:50:02.413000 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/decimal.py
--rw-r--r--   0        0        0      809 2024-02-28 22:50:02.413065 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/hashing.py
--rw-r--r--   0        0        0     2667 2024-03-25 17:49:21.920704 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/imports.py
--rw-r--r--   0        0        0     1407 2024-03-25 17:49:21.918051 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/orm.py
--rw-r--r--   0        0        0     2984 2024-03-25 17:49:21.965499 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/random.py
--rw-r--r--   0        0        0     7345 2024-02-28 22:50:02.413344 xian_contracting-0.1.1/xian_contracting/stdlib/bridge/time.py
--rw-r--r--   0        0        0      936 2024-03-25 17:49:21.957363 xian_contracting-0.1.1/xian_contracting/stdlib/env.py
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 xian_contracting-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-28 22:50:02.409938 xian_contracting-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1389 2024-03-25 17:29:18.195376 xian_contracting-0.1.2/README.md
+-rw-r--r--   0        0        0      365 2024-04-12 23:59:51.452324 xian_contracting-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-12 23:41:42.187329 xian_contracting-0.1.2/xian_contracting/.gitignore
+-rw-r--r--   0        0        0        7 2024-04-12 23:41:42.187399 xian_contracting-0.1.2/xian_contracting/.version
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187438 xian_contracting-0.1.2/xian_contracting/__init__.py
+-rw-r--r--   0        0        0    11775 2024-04-12 23:59:29.649917 xian_contracting-0.1.2/xian_contracting/client.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187883 xian_contracting-0.1.2/xian_contracting/compilation/__init__.py
+-rw-r--r--   0        0        0     3993 2024-04-12 23:59:29.657942 xian_contracting-0.1.2/xian_contracting/compilation/compiler.py
+-rw-r--r--   0        0        0    11682 2024-04-12 23:59:29.642039 xian_contracting-0.1.2/xian_contracting/compilation/linter.py
+-rw-r--r--   0        0        0     1431 2024-04-12 23:41:42.188181 xian_contracting-0.1.2/xian_contracting/compilation/parser.py
+-rw-r--r--   0        0        0     2733 2024-04-12 23:59:29.659873 xian_contracting-0.1.2/xian_contracting/compilation/whitelists.py
+-rw-r--r--   0        0        0      670 2024-04-12 23:41:42.188466 xian_contracting-0.1.2/xian_contracting/config.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188542 xian_contracting-0.1.2/xian_contracting/contracts/__init__.py
+-rw-r--r--   0        0        0      931 2024-04-12 23:41:42.188620 xian_contracting-0.1.2/xian_contracting/contracts/submission.s.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188683 xian_contracting-0.1.2/xian_contracting/db/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-12 23:59:29.631958 xian_contracting-0.1.2/xian_contracting/db/contract.py
+-rw-r--r--   0        0        0    17845 2024-04-12 23:59:29.634728 xian_contracting-0.1.2/xian_contracting/db/driver.py
+-rw-r--r--   0        0        0     5541 2024-04-12 23:59:29.646654 xian_contracting-0.1.2/xian_contracting/db/encoder.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.189379 xian_contracting-0.1.2/xian_contracting/db/hdf5/__init__.py
+-rw-r--r--   0        0        0     7083 2024-04-12 23:41:42.189581 xian_contracting-0.1.2/xian_contracting/db/hdf5/h5c.c
+-rw-r--r--   0        0        0     1836 2024-04-12 23:59:29.622042 xian_contracting-0.1.2/xian_contracting/db/hdf5/hdf5.py
+-rw-r--r--   0        0        0     4679 2024-04-12 23:59:29.661491 xian_contracting-0.1.2/xian_contracting/db/orm.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190019 xian_contracting-0.1.2/xian_contracting/execution/__init__.py
+-rw-r--r--   0        0        0     6224 2024-04-12 23:59:29.627638 xian_contracting-0.1.2/xian_contracting/execution/executor.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190327 xian_contracting-0.1.2/xian_contracting/execution/metering/__init__.py
+-rw-r--r--   0        0        0      887 2024-04-12 23:41:42.190405 xian_contracting-0.1.2/xian_contracting/execution/metering/cu_costs.const
+-rw-r--r--   0        0        0     1540 2024-04-12 23:41:42.190472 xian_contracting-0.1.2/xian_contracting/execution/metering/datastack.h
+-rw-r--r--   0        0        0      685 2024-04-12 23:41:42.190540 xian_contracting-0.1.2/xian_contracting/execution/metering/filedisp.h
+-rw-r--r--   0        0        0      709 2024-04-12 23:41:42.190607 xian_contracting-0.1.2/xian_contracting/execution/metering/stats.h
+-rw-r--r--   0        0        0    13222 2024-04-12 23:41:42.190849 xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.c
+-rw-r--r--   0        0        0     1985 2024-04-12 23:41:42.190914 xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.h
+-rw-r--r--   0        0        0     2994 2024-04-12 23:41:42.190981 xian_contracting-0.1.2/xian_contracting/execution/metering/util.h
+-rw-r--r--   0        0        0     4125 2024-04-12 23:59:29.651520 xian_contracting-0.1.2/xian_contracting/execution/module.py
+-rw-r--r--   0        0        0     3080 2024-04-12 23:59:29.638246 xian_contracting-0.1.2/xian_contracting/execution/runtime.py
+-rw-r--r--   0        0        0     5027 2024-04-12 23:41:42.191312 xian_contracting-0.1.2/xian_contracting/hlcpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191372 xian_contracting-0.1.2/xian_contracting/stdlib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191439 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-12 23:59:29.648140 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/access.py
+-rw-r--r--   0        0        0     4726 2024-04-12 23:59:29.636816 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/decimal.py
+-rw-r--r--   0        0        0      809 2024-04-12 23:41:42.191676 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/hashing.py
+-rw-r--r--   0        0        0     2667 2024-04-12 23:59:29.655655 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/imports.py
+-rw-r--r--   0        0        0     1407 2024-04-12 23:59:29.652728 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/orm.py
+-rw-r--r--   0        0        0     2984 2024-04-12 23:59:29.639637 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/random.py
+-rw-r--r--   0        0        0     7298 2024-04-12 23:59:29.644900 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/time.py
+-rw-r--r--   0        0        0      936 2024-04-12 23:59:29.630041 xian_contracting-0.1.2/xian_contracting/stdlib/env.py
+-rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 xian_contracting-0.1.2/PKG-INFO
```

### Comparing `xian_contracting-0.1.1/LICENSE` & `xian_contracting-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/README.md` & `xian_contracting-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/client.py` & `xian_contracting-0.1.2/xian_contracting/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,17 +274,20 @@
             if raise_errors:
                 for v in violations:
                     raise Exception(v)
             else:
                 return violations
 
     def estimate_stamps(self, contract_name, function_name, kwargs):
-        return self.executor.simulate_execute_without_writing(contract_name=contract_name,
-                                                              function_name=function_name,
-                                                              kwargs=kwargs)['stamps_used']
+        simulated = self.executor.simulate(
+            contract_name=contract_name,
+            function_name=function_name,
+            kwargs=kwargs)
+
+        return simulated['stamps_used']
 
     def compile(self, f):
         if isinstance(f, FunctionType):
             f, _ = self.closure_to_code_string(f)
 
         code = self.compiler.parse_to_code(f)
         return code
```

### Comparing `xian_contracting-0.1.1/xian_contracting/compilation/compiler.py` & `xian_contracting-0.1.2/xian_contracting/compilation/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from xian_contracting import config
 from xian_contracting.compilation.linter import Linter
 
 
 class ContractingCompiler(ast.NodeTransformer):
     def __init__(self, module_name='__main__', linter=Linter()):
-        #self.log = get_logger('xian_contracting.Compiler')
         self.module_name = module_name
         self.linter = linter
         self.lint_alerts = None
         self.constructor_visited = False
         self.private_names = set()
         self.orm_names = set()
         self.visited_names = set()  # store the method visits
@@ -29,15 +28,15 @@
 
         if self.lint_alerts is not None:
             raise Exception(self.lint_alerts)
 
         # check all visited nodes and see if they are actually private
 
         # An Expr node can have a value func of compilation.Name, or compilation.Attribute which you much access the value of.
-        # This code branching is not ideal and should be investigated for simplicity.
+        # TODO: This code branching is not ideal and should be investigated for simplicity.
         for node in self.visited_names:
             if node.id in self.private_names or node.id in self.orm_names:
                 node.id = self.privatize(node.id)
 
         ast.fix_missing_locations(tree)
 
         # reset state
@@ -113,8 +112,8 @@
         self.generic_visit(node)
         return node
 
     def visit_Num(self, node):
         if isinstance(node.n, float):
             return ast.Call(func=ast.Name(id='decimal', ctx=ast.Load()),
                             args=[ast.Str(str(node.n))], keywords=[])
-        return node
+        return node
```

### Comparing `xian_contracting-0.1.1/xian_contracting/compilation/linter.py` & `xian_contracting-0.1.2/xian_contracting/compilation/linter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import sys
 
 from .. import config
 
-from ..compilation.whitelists import ALLOWED_AST_TYPES, ALLOWED_ANNOTAION_TYPES, VIOLATION_TRIGGERS, ILLEGAL_BUILTINS, ILLEGAL_AST_TYPES
+from ..compilation.whitelists import ALLOWED_AST_TYPES, ALLOWED_ANNOTATION_TYPES, VIOLATION_TRIGGERS, ILLEGAL_BUILTINS, ILLEGAL_AST_TYPES
 
 from xian_contracting.db.driver import ContractDriver
 
 
 class Linter(ast.NodeVisitor):
 
     def __init__(self, driver=ContractDriver()):
@@ -231,15 +231,15 @@
         return node
 
     def annotation_types(self, t, lnum):
         if t is None:
             str = "Line {}".format(lnum) + " : " + VIOLATION_TRIGGERS[16]
             self._violations.append(str)
             self._is_success = False
-        elif t not in ALLOWED_ANNOTAION_TYPES:
+        elif t not in ALLOWED_ANNOTATION_TYPES:
             str = "Line {}".format(lnum) + " : " + VIOLATION_TRIGGERS[15] + " : {}" .format(t)
             self._violations.append(str)
             self._is_success = False
 
     def check_return_types(self, t, lnum):
         if t is not None:
             str = "Line {}".format(lnum) + " : " + VIOLATION_TRIGGERS[17] + " : {}" .format(t)
@@ -271,15 +271,14 @@
 
         for t, lineno in self.arg_types:
             self.annotation_types(t,lineno)
 
         for t, lineno in self.return_annotation:
             self.check_return_types(t,lineno)
 
-
     def _collect_function_defs(self, root):
         for node in ast.walk(root):
             if isinstance(node, ast.FunctionDef):
                 self._functions.append(node.name)
             elif isinstance(node, ast.Import) or isinstance(node, ast.ImportFrom):
                 for n in node.names:
                     if n.asname:
```

### Comparing `xian_contracting-0.1.1/xian_contracting/compilation/parser.py` & `xian_contracting-0.1.2/xian_contracting/compilation/parser.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/compilation/whitelists.py` & `xian_contracting-0.1.2/xian_contracting/compilation/whitelists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import ast, builtins
+import ast
+import builtins
 
 ALLOWED_BUILTINS = {'Exception', 'False', 'None', 'True', 'abs', 'all', 'any', 'ascii', 'bin', 'bool', 'bytearray',
                     'bytes', 'chr', 'dict', 'divmod', 'filter', 'format', 'frozenset', 'hex', 'int', 'isinstance',
                     'issubclass', 'import', 'len', 'list', 'map', 'max', 'min', 'oct', 'ord', 'pow', 'range', 'reversed',
                     'round', 'set', 'sorted', 'str', 'sum', 'tuple', 'zip'}
 
 ILLEGAL_BUILTINS = set(dir(builtins)) - ALLOWED_BUILTINS
@@ -32,15 +33,15 @@
     ast.Suite,
     ast.Try,
     ast.With,
     ast.Yield,
     ast.YieldFrom,
 }
 
-ALLOWED_ANNOTAION_TYPES = {'dict', 'list', 'str', 'int', 'float', 'bool', 'datetime.timedelta', 'datetime.datetime', 'Any'}
+ALLOWED_ANNOTATION_TYPES = {'dict', 'list', 'str', 'int', 'float', 'bool', 'datetime.timedelta', 'datetime.datetime', 'Any'}
 
 VIOLATION_TRIGGERS = [
     "S1- Illegal contracting syntax type used",
     "S2- Illicit use of '_' before variable",
     "S3- Illicit use of Nested imports",
     "S4- ImportFrom compilation nodes not yet supported",
     "S5- Contract not found in lib",
```

### Comparing `xian_contracting-0.1.1/xian_contracting/config.py` & `xian_contracting-0.1.2/xian_contracting/config.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/contracts/submission.s.py` & `xian_contracting-0.1.2/xian_contracting/contracts/submission.s.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/db/contract.py` & `xian_contracting-0.1.2/xian_contracting/db/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from xian_contracting.compilation.compiler import ContractingCompiler
 from xian_contracting.db.driver import ContractDriver
 from xian_contracting.execution.runtime import rt
-from types import ModuleType
 from xian_contracting.stdlib import env
 from xian_contracting import config
 
 _driver = rt.env.get('__Driver') or ContractDriver()
 
 
 class Contract:
-    def __init__(self, driver: ContractDriver=_driver):
+    def __init__(self, driver: ContractDriver = _driver):
         self._driver = driver
 
     def submit(self, name, code, owner=None, constructor_args={}, developer=None):
         if self._driver.get_contract(name) is not None:
             raise Exception('Contract already exists.')
 
         c = ContractingCompiler(module_name=name)
@@ -29,10 +28,23 @@
         if scope.get(config.INIT_FUNC_NAME) is not None:
             if constructor_args is None:
                 constructor_args = {}
             scope[config.INIT_FUNC_NAME](**constructor_args)
 
         now = scope.get('now')
         if now is not None:
-            self._driver.set_contract(name=name, code=code_obj, owner=owner, overwrite=False, timestamp=now, developer=developer)
+            self._driver.set_contract(
+                name=name,
+                code=code_obj,
+                owner=owner,
+                overwrite=False,
+                timestamp=now,
+                developer=developer
+            )
         else:
-            self._driver.set_contract(name=name, code=code_obj, owner=owner, overwrite=False, developer=developer)
+            self._driver.set_contract(
+                name=name,
+                code=code_obj,
+                owner=owner,
+                overwrite=False,
+                developer=developer
+            )
```

### Comparing `xian_contracting-0.1.1/xian_contracting/db/encoder.py` & `xian_contracting-0.1.2/xian_contracting/db/encoder.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/db/hdf5/h5c.c` & `xian_contracting-0.1.2/xian_contracting/db/hdf5/h5c.c`

 * *Files 15% similar despite different names*

```diff
@@ -7,34 +7,58 @@
 
 // HDF5 Reference Manual: https://support.hdfgroup.org/HDF5/doc/RM/RM_H5Front.html
 
 #define ATTR_LEN_MAX 64000 // http://davis.lbl.gov/Manuals/HDF5-1.8.7/UG/13_Attributes.html#SpecIssues
 #define ATTR_VALUE "value"
 #define ATTR_BLOCK "block"
 #define LOCK_SUFFIX "-lock"
+#define LOCK_TIMEOUT 10 // Timeout in seconds
 
 static char dirname_buf[PATH_MAX + 1];
 
-static void
-lock_acquire(char *filepath)
-{
+static void lock_acquire(char *filepath) {
+    char dirname_buf[PATH_MAX] = {0}; // Ensure dirname_buf is defined locally or is reset before use
+
+    // Construct the lock directory path
     strcat(dirname_buf, filepath);
     strcat(dirname_buf, LOCK_SUFFIX);
-    while(mkdir(dirname_buf, S_IRWXU) != 0)
-        ;
-    memset(dirname_buf, 0, sizeof(dirname_buf));
+
+    // Try to acquire the lock normally first
+    if (mkdir(dirname_buf, S_IRWXU) == 0) {
+        return; // Lock acquired successfully
+    } else if (errno == EEXIST) {
+        // The lock is already held, attempt to break it
+        printf("Force acquiring lock, removing existing lock for %s\n", filepath);
+        if (rmdir(dirname_buf) == 0) {
+            // Successfully removed the existing lock, try to acquire again
+            if (mkdir(dirname_buf, S_IRWXU) == 0) {
+                printf("Lock force acquired for %s\n", filepath);
+                return; // Lock acquired successfully after force
+            } else {
+                perror("Error force acquiring lock: ");
+            }
+        } else {
+            perror("Error removing existing lock: ");
+        }
+    } else {
+        perror("Error acquiring lock: ");
+    }
 }
 
-static void
-lock_release(char *filepath)
-{
+static void lock_release(char *filepath) {
+    char dirname_buf[PATH_MAX] = {0}; // Reset dirname_buf before use
+
     strcat(dirname_buf, filepath);
     strcat(dirname_buf, LOCK_SUFFIX);
-    rmdir(dirname_buf);
-    memset(dirname_buf, 0, sizeof(dirname_buf));
+
+    if (rmdir(dirname_buf) != 0) {
+        perror("Error releasing lock: ");
+    }
+
+    // No need to memset dirname_buf here if it's defined locally or properly managed
 }
 
 static void
 write_attr(hid_t gid, char *name, char *value)
 {
     H5Adelete(gid, name);
     if(value)
```

### Comparing `xian_contracting-0.1.1/xian_contracting/db/orm.py` & `xian_contracting-0.1.2/xian_contracting/db/orm.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         key = self._validate_key(key)
         self._set(key, value)
 
     def __getitem__(self, key):
         key = self._validate_key(key)
         return self._get(key)
 
+    def __contains__(self, key):
+        raise Exception('Cannot use "in" with a Hash.')
 
 class ForeignVariable(Variable):
     def __init__(self, contract, name, foreign_contract, foreign_name, driver: ContractDriver=driver):
         super().__init__(contract, name, driver=driver)
         self._key = self._driver.make_key(foreign_contract, foreign_name)
 
     def set(self, value):
```

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/cu_costs.const` & `xian_contracting-0.1.2/xian_contracting/execution/metering/cu_costs.const`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/datastack.h` & `xian_contracting-0.1.2/xian_contracting/execution/metering/datastack.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/filedisp.h` & `xian_contracting-0.1.2/xian_contracting/execution/metering/filedisp.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/stats.h` & `xian_contracting-0.1.2/xian_contracting/execution/metering/stats.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/tracer.c` & `xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.c`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   /* Variables to keep track of metering */
   unsigned long long cost;
   unsigned long long stamp_supplied;
   long last_frame_mem_usage;
   long total_mem_usage;
   int started;
   char * cu_cost_fname;
-
+  unsigned long long call_count; // Add this line to track call counts
 }
 Tracer;
 
 static int
 Tracer_init(Tracer * self, PyObject * args, PyObject * kwds) {
   //char *fname = getenv("CU_COST_FNAME");
 
@@ -97,22 +97,33 @@
   //    printf("%ld\n", r_usage.ru_maxrss);
 
   return r_usage.ru_maxrss;
 }
 
 static int
 Tracer_trace(Tracer * self, PyFrameObject * frame, int what, PyObject * arg) {
+    self->call_count++;
+
+    if (self->call_count > 400000) {
+        PyErr_SetString(PyExc_AssertionError, "Call count exceeded threshold! Infinite Loop?");
+        PyEval_SetTrace(NULL, NULL); // Stop tracing
+        self->started = 0; // Mark tracer as stopped
+        return RET_ERROR; // Use an appropriate return code
+    }
+
+
     unsigned long long estimate = 0;
     unsigned long long factor = 1000;
     const char * str;
     // IF, Frame object globals contains __contract__ and it is true, continue
     PyObject * kv = PyUnicode_FromString("__contract__");
     PyObject * globals = PyFrame_GetGlobals(frame);
     int t = PyDict_Contains(globals, kv);
     Py_DECREF(globals);
+    Py_DECREF(kv);
 
     if (t != 1) {
       return RET_OK;
     }
 
     if (self -> last_frame_mem_usage == 0) {
       self -> last_frame_mem_usage = get_memory_usage();
@@ -172,15 +183,15 @@
     return RET_OK;
     }
 
     static PyObject *
       Tracer_start(Tracer * self, PyObject * args) {
         PyEval_SetTrace((Py_tracefunc) Tracer_trace, (PyObject * ) self);
         self -> cost = 0;
-
+        self->call_count = 0;
         self -> started = 1;
         return Py_BuildValue("");
       }
 
     static PyObject *
       Tracer_stop(Tracer * self, PyObject * args) {
         if (self -> started) {
```

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/tracer.h` & `xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/metering/util.h` & `xian_contracting-0.1.2/xian_contracting/execution/metering/util.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/module.py` & `xian_contracting-0.1.2/xian_contracting/execution/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import importlib.util
 from importlib.abc import Loader, MetaPathFinder, PathEntryFinder
 from importlib import invalidate_caches, __import__
 from importlib.machinery import ModuleSpec
 from xian_contracting.db.driver import ContractDriver
 from xian_contracting.stdlib import env
 from xian_contracting.execution.runtime import rt
-from types import ModuleType
 import marshal
 import builtins
 
 # This function overrides the __import__ function, which is the builtin function that is called whenever Python runs
 # an 'import' statement. If the globals dictionary contains {'__contract__': True}, then this function will make sure
 # that the module being imported comes from the database and not from builtins or site packages.
 #
 # For all exec statements, we add the {'__contract__': True} _key to the globals to protect against unwanted imports.
 #
 # Note: anything installed with pip or in site-packages will also not work, so contract package names *must* be unique.
 #
 
+
 def is_valid_import(name):
     spec = importlib.util.find_spec(name)
     if not isinstance(spec.loader, DatabaseLoader):
         raise ImportError("module {} cannot be imported in a smart contract.".format(name))
 
 
 def restricted_import(name, globals=None, locals=None, fromlist=(), level=0):
```

### Comparing `xian_contracting-0.1.1/xian_contracting/execution/runtime.py` & `xian_contracting-0.1.2/xian_contracting/execution/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         'signer': None,
         'entry': None,
         'submission_name': None
     })
 
 WRITE_MAX = 1024 * 128
 
+
 class Runtime:
     cu_path = xian_contracting.__path__[0]
     cu_path = os.path.join(cu_path, 'execution', 'metering', 'cu_costs.const')
 
     os.environ['CU_COST_FNAME'] = cu_path
 
     loaded_modules = []
```

### Comparing `xian_contracting-0.1.1/xian_contracting/hlcpy/__init__.py` & `xian_contracting-0.1.2/xian_contracting/hlcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/access.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/access.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from xian_contracting.execution.runtime import rt
 from contextlib import ContextDecorator
 from xian_contracting.db.driver import ContractDriver
 from typing import Any
 
+
 class __export(ContextDecorator):
     def __init__(self, contract):
         self.contract = contract
 
     def __enter__(self, *args, **kwargs):
         driver = rt.env.get('__Driver') or ContractDriver()
```

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/decimal.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from decimal import Decimal
 import decimal
-import math
 
 MAX_UPPER_PRECISION = 30
 MAX_LOWER_PRECISION = 30
 CONTEXT = decimal.Context(prec=MAX_UPPER_PRECISION + MAX_LOWER_PRECISION, rounding=decimal.ROUND_FLOOR, Emin=-100,
                           Emax=100)
 decimal.setcontext(CONTEXT)
```

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/hashing.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/hashing.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/imports.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/imports.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/orm.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/orm.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/random.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/random.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/bridge/time.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from datetime import datetime as dt
 from datetime import timedelta as td
 from types import ModuleType
 
-from contracting.execution.runtime import rt
-
-
 # Redefine a controlled datetime object that feels like a regular Python datetime object but is restricted so that we
 # can regulate the user interaction with it to prevent security attack vectors. It may seem redundant, but it guarantees
 # security.
+
 SECONDS_IN_MINUTE = 60
 SECONDS_IN_HOUR = 3600
 SECONDS_IN_DAY = 86400
 SECONDS_IN_WEEK = 604800
 
 
 def get_raw_seconds(weeks, days, hours, minutes, seconds):
@@ -103,15 +101,14 @@
                        minutes=0,
                        seconds=0):
 
         self._timedelta = td(
             weeks=int(weeks), days=int(days), hours=int(hours), minutes=int(minutes), seconds=int(seconds)
         )
 
-
         # For fast access to how many hours are in a timedelta.
         self.__raw_seconds = get_raw_seconds(
             weeks=int(weeks), days=int(days), hours=int(hours), minutes=int(minutes), seconds=int(seconds)
         )
 
     def __lt__(self, other):
         if type(other) != Timedelta:
```

### Comparing `xian_contracting-0.1.1/xian_contracting/stdlib/env.py` & `xian_contracting-0.1.2/xian_contracting/stdlib/env.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.1/PKG-INFO` & `xian_contracting-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xian-contracting
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: endogen
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astor (>=0.8.1,<0.9.0)
```

