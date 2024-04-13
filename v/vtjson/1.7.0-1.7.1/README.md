# Comparing `tmp/vtjson-1.7.0.tar.gz` & `tmp/vtjson-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.0.tar", last modified: Fri Apr 12 01:05:52 2024, max compression
+gzip compressed data, was "vtjson-1.7.1.tar", last modified: Fri Apr 12 03:50:59 2024, max compression
```

## Comparing `vtjson-1.7.0.tar` & `vtjson-1.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:05:52.900255 vtjson-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 01:05:46.000000 vtjson-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-12 01:05:52.900255 vtjson-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17660 2024-04-12 01:05:46.000000 vtjson-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 01:05:46.000000 vtjson-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:05:52.900255 vtjson-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:05:52.900255 vtjson-1.7.0/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-04-12 01:05:46.000000 vtjson-1.7.0/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:50:59.643749 vtjson-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 03:50:54.000000 vtjson-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-04-12 03:50:59.643749 vtjson-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-12 03:50:54.000000 vtjson-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 03:50:54.000000 vtjson-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:50:59.643749 vtjson-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:50:59.643749 vtjson-1.7.1/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-04-12 03:50:59.000000 vtjson-1.7.1/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 03:50:59.000000 vtjson-1.7.1/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:50:59.000000 vtjson-1.7.1/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 03:50:59.000000 vtjson-1.7.1/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 03:50:59.000000 vtjson-1.7.1/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28120 2024-04-12 03:50:54.000000 vtjson-1.7.1/vtjson.py
```

### Comparing `vtjson-1.7.0/LICENSE` & `vtjson-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.0/PKG-INFO` & `vtjson-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.0
+Version: 1.7.1
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -303,15 +303,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.pyq`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
@@ -332,14 +332,15 @@
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
 {"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
 ```
+Note that you can create an infinite recursion by validating a recursive object against a recursive schema.
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.7.0/README.md` & `vtjson-1.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.pyq`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
@@ -315,14 +315,15 @@
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
 {"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
 ```
+Note that you can create an infinite recursion by validating a recursive object against a recursive schema.
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.7.0/pyproject.toml` & `vtjson-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.0/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.1/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.0
+Version: 1.7.1
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -303,15 +303,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.pyq`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
@@ -332,14 +332,15 @@
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
 {"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
 ```
+Note that you can create an infinite recursion by validating a recursive object against a recursive schema.
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.7.0/vtjson.py` & `vtjson-1.7.1/vtjson.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -674,46 +674,77 @@
     def __validate__(self, object, name, strict):
         for k in self.args:
             if k not in object:
                 return f"{name}[{repr(k)}] is missing"
         return ""
 
 
-class ifthen:
-    def __init__(self, if_schema, then_schema, else_schema=None):
-        self.if_schema = compile(if_schema)
-        self.then_schema = compile(then_schema)
+class _ifthen:
+    def __init__(self, if_schema, then_schema, else_schema=None, _deferred_compiles={}):
+        self.if_schema = compile(if_schema, _deferred_compiles=_deferred_compiles)
+        self.then_schema = compile(then_schema, _deferred_compiles=_deferred_compiles)
         if else_schema is not None:
-            self.else_schema = compile(else_schema)
+            self.else_schema = compile(
+                else_schema, _deferred_compiles=_deferred_compiles
+            )
         else:
             self.else_schema = else_schema
 
     def __validate__(self, object, name, strict):
         if self.if_schema.__validate__(object, name, strict) == "":
             return self.then_schema.__validate__(object, name, strict)
         elif self.else_schema is not None:
             return self.else_schema.__validate__(object, name, strict)
         return ""
 
 
-class cond:
-    def __init__(self, *args):
+class ifthen:
+    def __init__(self, if_schema, then_schema, else_schema=None):
+        self.if_schema = if_schema
+        self.then_schema = then_schema
+        self.else_schema = else_schema
+
+    def __compile__(self, _deferred_compiles={}):
+        return _ifthen(
+            self.if_schema,
+            self.then_schema,
+            else_schema=self.else_schema,
+            _deferred_compiles=_deferred_compiles,
+        )
+
+
+class _cond:
+    def __init__(self, args, _deferred_compiles={}):
         self.conditions = []
         for c in args:
-            if not isinstance(c, tuple) or len(c) != 2:
-                raise SchemaError(f"{repr(c)} is not a tuple of length two")
-            self.conditions.append((compile(c[0]), compile(c[1])))
+            self.conditions.append(
+                (
+                    compile(c[0], _deferred_compiles=_deferred_compiles),
+                    compile(c[1], _deferred_compiles=_deferred_compiles),
+                )
+            )
 
     def __validate__(self, object, name, strict):
         for c in self.conditions:
             if c[0].__validate__(object, name, strict) == "":
                 return c[1].__validate__(object, name, strict)
         return ""
 
 
+class cond:
+    def __init__(self, *args):
+        for c in args:
+            if not isinstance(c, tuple) or len(c) != 2:
+                raise SchemaError(f"{repr(c)} is not a tuple of length two")
+        self.args = args
+
+    def __compile__(self, _deferred_compiles={}):
+        return _cond(self.args, _deferred_compiles=_deferred_compiles)
+
+
 class _dict:
     def __init__(self, schema, _deferred_compiles={}):
         self.schema = collections.OrderedDict()
         for k, v in schema.items():
             self.schema[k] = compile(v, _deferred_compiles=_deferred_compiles)
         self.keys = _keys(self.schema)
         self.keys2 = _keys2(self.schema)
```

