# Comparing `tmp/pycep_parser-0.5.1a3.tar.gz` & `tmp/pycep_parser-0.5.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycep_parser-0.5.1a3.tar", max compression
+gzip compressed data, was "pycep_parser-0.5.1a4.tar", max compression
```

## Comparing `pycep_parser-0.5.1a3.tar` & `pycep_parser-0.5.1a4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10834 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/LICENSE
--rw-r--r--   0        0        0     1400 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/README.md
--rw-r--r--   0        0        0       57 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/__init__.py
--rw-r--r--   0        0        0    13737 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/bicep.lark
--rw-r--r--   0        0        0     1833 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/main.py
--rw-r--r--   0        0        0        0 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/py.typed
--rw-r--r--   0        0        0    59445 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/transformer.py
--rw-r--r--   0        0        0    26006 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/typing.py
--rw-r--r--   0        0        0      274 2024-04-09 13:28:06.282433 pycep_parser-0.5.1a3/pycep/validator.py
--rw-r--r--   0        0        0     1921 2024-04-09 13:28:18.746487 pycep_parser-0.5.1a3/pyproject.toml
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pycep_parser-0.5.1a3/PKG-INFO
+-rw-r--r--   0        0        0    10834 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/README.md
+-rw-r--r--   0        0        0       57 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/__init__.py
+-rw-r--r--   0        0        0    13943 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/bicep.lark
+-rw-r--r--   0        0        0     1833 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/main.py
+-rw-r--r--   0        0        0        0 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/py.typed
+-rw-r--r--   0        0        0    60366 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/transformer.py
+-rw-r--r--   0        0        0    25993 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/typing.py
+-rw-r--r--   0        0        0      274 2024-04-13 00:27:57.411697 pycep_parser-0.5.1a4/pycep/validator.py
+-rw-r--r--   0        0        0     1921 2024-04-13 00:28:07.271760 pycep_parser-0.5.1a4/pyproject.toml
+-rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 pycep_parser-0.5.1a4/PKG-INFO
```

### Comparing `pycep_parser-0.5.1a3/LICENSE` & `pycep_parser-0.5.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a3/README.md` & `pycep_parser-0.5.1a4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 ## Current capabilities
 
 [Supported capabilities](docs/capabilities.md)
 
 ## Next milestones
 
+### Custom data types
+Initial support was added with following parts still missing
+- Array type
+- Decorators in object type
+- Union type in object type
+
 ### Functions
 - [ ] Array (in progress)
 - [ ] CIDR (in progress)
 - [ ] Lambda (in progress)
 
 ### Operators
 - [ ] Safe-dereference
```

### Comparing `pycep_parser-0.5.1a3/pycep/bicep.lark` & `pycep_parser-0.5.1a4/pycep/bicep.lark`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 element: "targetScope" "=" QUOTED_INTERPOLATION                                         -> scope
        | "metadata" STRING "=" metadata_value                                           -> metadata
        | [decorator] "param" STRING data_type ["=" value_brackets]                      -> param
        | [decorator] "var" STRING "=" var_value                                         -> var
        | [decorator] "output" STRING data_type "=" output_value                         -> output
        | [decorator] "resource" STRING type_api_pair [EXISTING] "=" resource_value      -> resource
        | [decorator] "module" STRING module_path "=" module_value                       -> module
+       | [decorator] "type" STRING "=" type_value                                       -> custom_type
 
 ?value: _NEWLINE? "null"                      -> null
       | _NEWLINE? "true"                      -> true
       | _NEWLINE? "false"                     -> false
       | _NEWLINE? INT                         -> int
       | _NEWLINE? STRING                      -> string
       | _NEWLINE? QUOTED_INTERPOLATION        -> string
@@ -32,14 +33,16 @@
 
 ?resource_value: object | loop | deploy_condition
 
 ?module_value: object | loop | deploy_condition
 
 child_resource: "resource" STRING QUOTED_INTERPOLATION [EXISTING] "=" object _CPP_COMMENT_NL+
 
+?type_value: value_brackets ("|" value_brackets)*
+
 // element type extras
 
 data_type: STRING
 
 type_api_pair: QUOTED_INTERPOLATION
 
 module_path: QUOTED_INTERPOLATION
@@ -64,15 +67,15 @@
 
 ?quoted_string: STRING | QUOTED_STRING | QUOTED_INTERPOLATION
 
 array: "[" _CPP_COMMENT_NL~0..10 (value_brackets ("," value_brackets)* _CPP_COMMENT_NL~0..5)* "]"
 
 object: "{" _CPP_COMMENT_NL~0..10 ((pair ("," pair)* | child_resource) _CPP_COMMENT_NL~0..5)* "}"
 
-pair: key ":" (value_brackets | loop)
+pair: key ":" (value_brackets | loop) "?"?
 
 !key: "resource" | quoted_string
 
 // decorators
 
 decorator: ("@" "sys."? (deco_allowed | deco_batch | deco_description | deco_min_len | deco_max_len | deco_min_val | deco_max_val | deco_metadata | deco_secure) _CPP_COMMENT_NL~0..5)+
 
@@ -182,21 +185,23 @@
 
 filter: ("filter" | "sys.filter") "(" value_brackets "," STRING "=>" value_brackets ")"
 
 // functions - logical
 
 ?function_logical: bool_func
 
-bool_func: ("bool" | "sys.bool") "(" value_brackets ")"
+_BOOL.1: ("bool" | "sys.bool") "("
+bool_func: _BOOL value_brackets ")"
 
 // functions - numeric
 
 ?function_numeric: int_func
 
-int_func: ("int" | "sys.int") "(" value_brackets ")"
+_INT.1: ("int" | "sys.int") "("
+int_func: _INT value_brackets ")"
 
 // functions - object
 
 ?function_object: json_func
 
 _JSON.1: ("json" | "sys.json") "("
 json_func: _JSON value_brackets ")" [["[" STRING "]"] "." (STRING | INDEXED)]
@@ -277,15 +282,16 @@
 
 split: ("split" | "sys.split") "(" value_brackets "," value_brackets ")" ["[" INT "]"]
 
 join: ("join" | "sys.join") "(" value_brackets "," value_brackets ")"
 
 starts_with: ("startsWith" | "sys.startsWith") "(" value_brackets "," value_brackets ")"
 
-string_func: ("string" | "sys.string") "(" value_brackets ")"
+_STRING.1: ("string" | "sys.string") "("
+string_func: _STRING value_brackets ")"
 
 substring: ("substring" | "sys.substring") "(" value_brackets "," value_brackets ["," value_brackets] ")"
 
 to_lower: ("toLower" | "sys.toLower") "(" value_brackets ")"
 
 to_upper: ("toUpper" | "sys.toUpper") "(" value_brackets ")"
```

### Comparing `pycep_parser-0.5.1a3/pycep/main.py` & `pycep_parser-0.5.1a4/pycep/main.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a3/pycep/transformer.py` & `pycep_parser-0.5.1a4/pycep/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import itertools
 import re
-from typing import Any, cast
+from typing import Any, Literal, cast
 
 from lark import Token, Transformer, v_args
 from lark.tree import Meta
-from typing_extensions import Literal
 
 from pycep import typing as pycep_typing
 
 BICEP_REGISTRY_ALIAS_PATTERN = re.compile(r"br/(?P<alias>[\w]+):(?P<path>[\w/\-.]+):(?P<tag>[\w.\-]+)")
 PUBLIC_BICEP_REGISTRY_PATTERN = re.compile(r"br:mcr\.microsoft\.com/(?P<path>[\w/\-]+):(?P<tag>[\w.\-]+)")
 PRIVATE_BICEP_REGISTRY_PATTERN = re.compile(
     r"br:(?P<registry_name>\w+)\.azurecr\.io/(?P<path>[\w/\-.]+):(?P<tag>[\w.\-]+)"
@@ -251,14 +250,36 @@
 
         if self.add_line_numbers:
             result["modules"]["__attrs__"]["__start_line__"] = meta.line
             result["modules"]["__attrs__"]["__end_line__"] = meta.end_line
 
         return result
 
+    @v_args(meta=True)
+    def custom_type(
+        self, meta: Meta, args: tuple[list[pycep_typing.Decorator] | None, Token, pycep_typing.PossibleValue]
+    ) -> pycep_typing.TypeResponse:
+        decorators, name, value = args
+
+        result: pycep_typing.TypeResponse = {
+            "types": {
+                "__name__": str(name),
+                "__attrs__": {
+                    "decorators": decorators if decorators else [],
+                    "value": value,
+                },
+            }
+        }
+
+        if self.add_line_numbers:
+            result["types"]["__attrs__"]["__start_line__"] = meta.line
+            result["types"]["__attrs__"]["__end_line__"] = meta.end_line
+
+        return result
+
     ####################
     #
     # element type extras
     #
     ####################
 
     def data_type(self, arg: tuple[Token]) -> str:
@@ -360,14 +381,18 @@
             "detail": {
                 "full": file_path,
                 "path": file_path,
             },
         }
         return local_result
 
+    def type_value(self, args: tuple[pycep_typing.PossibleNoneValue, ...]) -> str:
+        # this is only triggered, when a union type was found, ex. "'bicep' | 'arm' | 'azure'"
+        return " | ".join(str(arg) for arg in args)
+
     ####################
     #
     # loops
     #
     ####################
 
     def loop(self, args: tuple[pycep_typing.LoopType, str | None, dict[str, Any]]) -> pycep_typing.Loop:
```

### Comparing `pycep_parser-0.5.1a3/pycep/typing.py` & `pycep_parser-0.5.1a4/pycep/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Literal, TypedDict
 
-from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict
+from typing_extensions import NotRequired, TypeAlias
 
-# dict[str, Any] -> dict[str, PossibleValue] not supported https://github.com/python/mypy/issues/731
-PossibleValue: TypeAlias = "bool | int | str | list[bool | int | str] | dict[str, Any]"
+PossibleValue: TypeAlias = "bool | int | str | list[bool | int | str] | dict[str, PossibleValue]"
 PossibleNoneValue: TypeAlias = "PossibleValue | None"
 
 ModulePath: TypeAlias = "LocalModulePath | BicepRegistryModulePath | BicepRegistryAliasModulePath | TemplateSpecModulePath | TemplateSpecAliasModulePath"
 ModuleDetail: TypeAlias = "_LocalModulePathDetail | _BicepRegistryModulePathDetail | _BicepRegistryAliasModulePathDetail | _TemplateSpecModulePathDetail | _TemplateSpecAliasModulePathDetail"
 LoopType: TypeAlias = "LoopArray | LoopArrayIndex | LoopObject | LoopRange"
-ElementResponse: TypeAlias = "ParamResponse | VarResponse | ResourceResponse | ModuleResponse | OutputResponse"
+ElementResponse: TypeAlias = (
+    "ParamResponse | VarResponse | ResourceResponse | ModuleResponse | OutputResponse | TypeResponse"
+)
 Decorator: TypeAlias = "DecoratorAllowed | DecoratorBatchSize | DecoratorDescription | DecoratorMinLength | DecoratorMaxLength | DecoratorMinValue | DecoratorMaxValue | DecoratorMetadata | DecoratorSecure"
 
 ComparisonOperators: TypeAlias = "GreaterThanOrEquals | GreaterThan | LessThanOrEquals | LessThan | Equals | NotEquals | EqualsCaseInsensitive | NotEqualsCaseInsensitive"
 LogicalOperators: TypeAlias = "And | Or | Not | Coalesce | Conditional"
 NumericOperators: TypeAlias = "Add | Divide | Minus | Modulo | Multiply | Substract"
 AccessorOperators: TypeAlias = "IndexAccessor | FunctionAccessor | NestedResourceAccessor | PropertyAccessor"
 Operators: TypeAlias = "ComparisonOperators | LogicalOperators | NumericOperators | AccessorOperators"
@@ -168,14 +169,18 @@
 
 
 class ApiTypeVersion(TypedDict):
     type: str
     api_version: str
 
 
+class TypeResponse(TypedDict):
+    types: _Variables
+
+
 ####################
 #
 # Module Paths
 #
 ####################
```

### Comparing `pycep_parser-0.5.1a3/pyproject.toml` & `pycep_parser-0.5.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycep-parser"
-version = "0.5.1a3"
+version = "0.5.1a4"
 description = "A Python based Bicep parser"
 authors = ["Anton Grübel <anton.gruebel@gmail.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 
 packages = [
```

### Comparing `pycep_parser-0.5.1a3/PKG-INFO` & `pycep_parser-0.5.1a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycep-parser
-Version: 0.5.1a3
+Version: 0.5.1a4
 Summary: A Python based Bicep parser
 Home-page: https://github.com/gruebel/pycep
 License: Apache-2.0
 Keywords: bicep,parser,lark
 Author: Anton Grübel
 Author-email: anton.gruebel@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -50,14 +50,20 @@
 
 ## Current capabilities
 
 [Supported capabilities](docs/capabilities.md)
 
 ## Next milestones
 
+### Custom data types
+Initial support was added with following parts still missing
+- Array type
+- Decorators in object type
+- Union type in object type
+
 ### Functions
 - [ ] Array (in progress)
 - [ ] CIDR (in progress)
 - [ ] Lambda (in progress)
 
 ### Operators
 - [ ] Safe-dereference
```

