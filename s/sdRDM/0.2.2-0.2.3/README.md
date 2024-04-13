# Comparing `tmp/sdrdm-0.2.2.tar.gz` & `tmp/sdrdm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdrdm-0.2.2.tar", max compression
+gzip compressed data, was "sdrdm-0.2.3.tar", max compression
```

## Comparing `sdrdm-0.2.2.tar` & `sdrdm-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1755 2024-02-01 11:42:00.714666 sdrdm-0.2.2/README.md
--rw-r--r--   0        0        0     1136 2024-02-01 11:42:00.714666 sdrdm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       91 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/__init__.py
--rw-r--r--   0        0        0       60 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/__init__.py
--rw-r--r--   0        0        0    34076 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/datamodel.py
--rw-r--r--   0        0        0       23 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/datatypes/__init__.py
--rw-r--r--   0        0        0     4543 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/datatypes/unit.py
--rw-r--r--   0        0        0     2808 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/importedmodules.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/ioutils/__init__.py
--rw-r--r--   0        0        0     4721 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/ioutils/hdf5.py
--rw-r--r--   0        0        0     7933 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/linker.py
--rw-r--r--   0        0        0     3318 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/listplus.py
--rw-r--r--   0        0        0     2790 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/referencecheck.py
--rw-r--r--   0        0        0     3795 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/tree.py
--rw-r--r--   0        0        0     3248 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/base/utils.py
--rw-r--r--   0        0        0     4966 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/cli.py
--rw-r--r--   0        0        0       41 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/__init__.py
--rw-r--r--   0        0        0    17914 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/classrender.py
--rw-r--r--   0        0        0     5387 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/codegen.py
--rw-r--r--   0        0        0     7122 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/datatypes.py
--rw-r--r--   0        0        0      519 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/enumrender.py
--rw-r--r--   0        0        0     1251 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/initrender.py
--rw-r--r--   0        0        0     1511 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/schemagen.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/__init__.py
--rw-r--r--   0        0        0      936 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/add_method_template.jinja2
--rw-r--r--   0        0        0      363 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/add_unit_template.jinja2
--rw-r--r--   0        0        0      777 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/attribute_template.jinja2
--rw-r--r--   0        0        0      786 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/class_template.jinja2
--rw-r--r--   0        0        0      137 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/enum_template.jinja2
--rw-r--r--   0        0        0      137 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/function_docstring.jinja2
--rw-r--r--   0        0        0      442 2024-02-01 11:42:00.714666 sdrdm-0.2.2/sdRDM/generator/templates/import_template.jinja2
--rw-r--r--   0        0        0      146 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/templates/init_file_library.jinja2
--rw-r--r--   0        0        0      240 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/templates/init_file_template.jinja2
--rw-r--r--   0        0        0      877 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/templates/mermaid_class.jinja2
--rw-r--r--   0        0        0      701 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/templates/reference_template.jinja2
--rw-r--r--   0        0        0     6398 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/updater.py
--rw-r--r--   0        0        0      893 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/generator/utils.py
--rw-r--r--   0        0        0       43 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/__init__.py
--rw-r--r--   0        0        0     1390 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/enumutils.py
--rw-r--r--   0        0        0     5284 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/markdownparser.py
--rw-r--r--   0        0        0    11637 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/objectutils.py
--rw-r--r--   0        0        0     2493 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/smalltypes.py
--rw-r--r--   0        0        0      477 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/markdown/tokens.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/tools/__init__.py
--rw-r--r--   0        0        0     5596 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/tools/gitutils.py
--rw-r--r--   0        0        0     1301 2024-02-01 11:42:00.718666 sdrdm-0.2.2/sdRDM/tools/utils.py
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 sdrdm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1759 2024-04-13 06:32:20.173393 sdrdm-0.2.3/README.md
+-rw-r--r--   0        0        0     1167 2024-04-13 06:32:20.173393 sdrdm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/__init__.py
+-rw-r--r--   0        0        0    33906 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/datamodel.py
+-rw-r--r--   0        0        0       23 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/datatypes/__init__.py
+-rw-r--r--   0        0        0     5083 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/datatypes/unit.py
+-rw-r--r--   0        0        0     2808 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/importedmodules.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/ioutils/__init__.py
+-rw-r--r--   0        0        0     4665 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/ioutils/hdf5.py
+-rw-r--r--   0        0        0     3318 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/listplus.py
+-rw-r--r--   0        0        0     2790 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/referencecheck.py
+-rw-r--r--   0        0        0     3795 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/tree.py
+-rw-r--r--   0        0        0     3248 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/base/utils.py
+-rw-r--r--   0        0        0     5167 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/cli.py
+-rw-r--r--   0        0        0       41 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/__init__.py
+-rw-r--r--   0        0        0    19699 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/classrender.py
+-rw-r--r--   0        0        0     5822 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/codegen.py
+-rw-r--r--   0        0        0     7185 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/datatypes.py
+-rw-r--r--   0        0        0      519 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/enumrender.py
+-rw-r--r--   0        0        0     1251 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/initrender.py
+-rw-r--r--   0        0        0     1511 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/schemagen.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/__init__.py
+-rw-r--r--   0        0        0     1019 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/add_method_template.jinja2
+-rw-r--r--   0        0        0      363 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/add_unit_template.jinja2
+-rw-r--r--   0        0        0      668 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/attribute_leaf_template.jinja2
+-rw-r--r--   0        0        0      777 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/attribute_template.jinja2
+-rw-r--r--   0        0        0     1547 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/class_template.jinja2
+-rw-r--r--   0        0        0      137 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/enum_template.jinja2
+-rw-r--r--   0        0        0      137 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/function_docstring.jinja2
+-rw-r--r--   0        0        0      584 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/import_template.jinja2
+-rw-r--r--   0        0        0      146 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/init_file_library.jinja2
+-rw-r--r--   0        0        0      240 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/init_file_template.jinja2
+-rw-r--r--   0        0        0      877 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/mermaid_class.jinja2
+-rw-r--r--   0        0        0      701 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/templates/reference_template.jinja2
+-rw-r--r--   0        0        0     6514 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/updater.py
+-rw-r--r--   0        0        0      893 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/generator/utils.py
+-rw-r--r--   0        0        0       43 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/enumutils.py
+-rw-r--r--   0        0        0     6112 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/markdownparser.py
+-rw-r--r--   0        0        0    11771 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/objectutils.py
+-rw-r--r--   0        0        0     2493 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/smalltypes.py
+-rw-r--r--   0        0        0      477 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/markdown/tokens.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/tools/__init__.py
+-rw-r--r--   0        0        0     5596 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/tools/gitutils.py
+-rw-r--r--   0        0        0     7933 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/tools/linker.py
+-rw-r--r--   0        0        0     1883 2024-04-13 06:32:20.173393 sdrdm-0.2.3/sdRDM/tools/utils.py
+-rw-r--r--   0        0        0     3282 1970-01-01 00:00:00.000000 sdrdm-0.2.3/PKG-INFO
```

### Comparing `sdrdm-0.2.2/README.md` & `sdrdm-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">
   Software-Driven RDM</br>
   <a href="https://badge.fury.io/py/sdRDM"><img src="https://badge.fury.io/py/sdRDM.svg" alt="PyPI version" height="18"></a>
-  <img src="https://img.shields.io/badge/python-3.9|3.10|3.11-blue.svg" alt="Build Badge">
+  <img src="https://img.shields.io/badge/python-3.9 | 3.10 | 3.11-blue.svg" alt="Build Badge">
   <img src="https://github.com/JR-1991/software-driven-rdm/actions/workflows/tests.yml/badge.svg" alt="Build Badge">
 </h1>
 <p align="center">
 With Software-driven Research Data Management (sdRDM), you can confidently specify data models using verbose Markdown documents and effortlessly convert them into powerful Python objects that can be serialized into any data exchange format.
 </p>
 
 ### 🏎 Features
```

### Comparing `sdrdm-0.2.2/sdRDM/base/datamodel.py` & `sdrdm-0.2.3/sdRDM/base/datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from nob import Nob
 from nob.path import Path
 from dotted_dict import DottedDict
 from enum import Enum
 from anytree import Node, LevelOrderIter
 from bigtree import print_tree, levelorder_iter, yield_tree
 from functools import lru_cache
+from lxml.etree import _Element
 from pydantic import ConfigDict, PrivateAttr, field_validator
 from typing import (
     Any,
     List,
     Dict,
     Optional,
     IO,
@@ -41,27 +42,27 @@
 )
 from sdRDM.base.utils import generate_model
 from sdRDM.base.tree import _digit_free_path, build_guide_tree, ClassNode
 from sdRDM.generator.codegen import generate_python_api
 from sdRDM.generator.utils import extract_modules
 from sdRDM.tools.utils import YAMLDumper
 from sdRDM.tools.gitutils import (
-    ObjectNode,
     build_library_from_git_specs,
     _import_library,
 )
 
 
 class DataModel(pydantic_xml.BaseXmlModel):
     # * Config
     model_config = ConfigDict(
         validate_assignment=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         populate_by_name=True,
+        from_attributes=True,
     )
 
     # * Private attributes
     _node: Optional[Node] = PrivateAttr(default=None)
     _types: DottedDict = PrivateAttr(default=dict)
     _parent: Optional["DataModel"] = PrivateAttr(default=None)
     _references: DottedDict = PrivateAttr(default_factory=DottedDict)
@@ -175,15 +176,15 @@
         for path in matching_paths:  # type: ignore
             reference = self._check_query(
                 self._traverse_model_by_path(self, path),
                 attribute,
                 query,
             )
 
-            if reference:
+            if reference is not None:
                 references.append(reference)
 
         return references
 
     @staticmethod
     def _setup_query(
         target: Union[str, float, int, None, "DataModel", Callable]
@@ -261,15 +262,15 @@
 
         return current
 
     def paths(self, leaves: bool = False):
         """Returns all possible paths of an instantiated data model. Can also be reduced to just leaves."""
 
         # Get JSON representation
-        model = Nob(self.to_dict(warn=False))
+        model = Nob(self.to_dict(warn=False, mode="python"))
 
         if leaves:
             return model.leaves
         else:
             return model.paths
 
     @classmethod
@@ -325,14 +326,15 @@
         self,
         exclude_none=True,
         warn=True,
         convert_h5ds=True,
         mode="json",
         **kwargs,
     ):
+
         data = super().model_dump(
             exclude_none=exclude_none,
             by_alias=True,
             mode=mode,
             **kwargs,
         )
 
@@ -617,31 +619,29 @@
         except HDF5ExtError as e:
             return False
 
         return True
 
     @classmethod
     def from_markdown(cls, path: str) -> ImportedModules:
-        """Fetches a Markdown specification from a git repository and builds the library accordingly.
-
-        This function will clone the repository into a temporary directory and
-        builds the correpsonding API and loads it into the memory. After that
-        the cloned repository is deleted and the root object(s) detected.
+        """Converts a markdown file into a in-memory Python API.
 
         Args:
-            url (str): Link to the git repository. Use the URL ending with ".git".
-            commit (Optional[str], optional): Hash of the commit to fetch from. Defaults to None.
+            path (str): Path to the markdown file.
         """
 
         with tempfile.TemporaryDirectory() as tmpdirname:
             # Generate API to parse the file
             lib_name = f"sdRDM-Library-{str(random.randint(0,30))}"
             api_loc = os.path.join(tmpdirname, lib_name)
             generate_python_api(
-                path=path, dirpath=tmpdirname, libname=lib_name, use_formatter=False
+                path=path,
+                dirpath=tmpdirname,
+                libname=lib_name,
+                use_formatter=False,
             )
 
             lib = _import_library(api_loc, lib_name)
 
         return extract_modules(lib=lib, links={})
 
     @classmethod
@@ -659,14 +659,15 @@
         builds the correpsonding API and loads it into the memory. After that
         the cloned repository is deleted and the root object(s) detected.
 
         Args:
             url (str): Link to the git repository. Use the URL ending with ".git".
             commit (Optional[str], optional): Hash of the commit to fetch from. Defaults to None.
             tag (Optional[str], optional): Tag of the release or branch to fetch from. Defaults to None.
+            only_classes (bool, optional): If True, only the classes will be returned. Defaults to False.
         """
 
         if not validators.url(url):
             raise ValueError(f"Given URL '{url}' is not a valid URL.")
 
         # Build and import the library
         tmpdirname = tempfile.mkdtemp()
```

### Comparing `sdrdm-0.2.2/sdRDM/base/datatypes/unit.py` & `sdrdm-0.2.3/sdRDM/base/datatypes/unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from uuid import uuid4
 from pydantic_xml import attr, element, wrapped
+from pydantic import model_validator
 import sdRDM
 
 from typing import List, Union
-from astropy.units import UnitBase, Unit as AstroUnit
+from astropy.units import UnitBase, Unit as AstroUnit, dimensionless_unscaled
 from pydantic import field_serializer, PrivateAttr
 
 
 class BaseUnit(
     sdRDM.DataModel,
     tag="BaseUnit",
 ):
@@ -21,15 +22,14 @@
             return self.kind
         else:
             return str(self.kind)
 
 
 class Unit(
     sdRDM.DataModel,
-    nsmap={"": "https://www.github.com/software-driven-rdm"},
     tag="Unit",
 ):
     """
     Represents a unit type.
 
     Attributes:
         scale (float): The scale of the unit.
@@ -42,17 +42,30 @@
         from_string: Creates a Unit object from a string representation.
         from_astropy_unit: Creates an instance of the class from an Astropy unit.
         to_unit_string: Returns a string representation of the unit.
     """
 
     id: str = attr(name="id", default_factory=lambda: str(uuid4()))
     name: str = attr(name="name")
-    bases: List[BaseUnit] = element()
-    _unit: UnitBase = PrivateAttr()
-    _hash: int = PrivateAttr()
+    bases: List[BaseUnit] = wrapped(
+        "listOfUnits",
+        element(tag="unit"),
+    )
+
+    _unit: UnitBase = PrivateAttr(default=None)
+    _hash: int = PrivateAttr(default=None)
+
+    @model_validator(mode="after")
+    def create_astropy_unit(self):
+        if self._unit is None and self.name != "dimensionless":
+            self._unit = AstroUnit(self.name)
+        elif self.name == "dimensionless":
+            self._unit = AstroUnit(dimensionless_unscaled)
+
+        return self
 
     @classmethod
     def from_string(cls, unit_string: str):
         """
         Creates a Unit object from a string representation.
 
         Args:
@@ -60,14 +73,21 @@
 
         Returns:
             Unit: The created Unit object.
 
         Raises:
             AssertionError: If the unit is not a UnitBase or Unit.
         """
+
+        if unit_string.lower() == "dimensionless":
+            return cls(
+                name="dimensionless",
+                bases=[],
+            )
+
         unit = AstroUnit(unit_string)
 
         assert isinstance(
             unit, (UnitBase, AstroUnit)
         ), "Unit must be a UnitBase or Unit."
 
         return cls.from_astropy_unit(unit)
```

### Comparing `sdrdm-0.2.2/sdRDM/base/importedmodules.py` & `sdrdm-0.2.3/sdRDM/base/importedmodules.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/base/ioutils/hdf5.py` & `sdrdm-0.2.3/sdRDM/base/ioutils/hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
         # Fetch or create a group
         group = _get_group(file, prefix)
 
         if is_array and not is_multiple_numeric:
             _write_array(attribute, data, group)
         elif not is_array and is_multiple_numeric:
-            print(np.array(data), np.array(data).shape)
             _write_array(attribute, np.array(data), group)
         else:
             _write_attr(attribute, data, group)  # type: ignore
 
     if auto_close:
         file.close()
```

### Comparing `sdrdm-0.2.2/sdRDM/base/linker.py` & `sdrdm-0.2.3/sdRDM/tools/linker.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/base/listplus.py` & `sdrdm-0.2.3/sdRDM/base/listplus.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/base/referencecheck.py` & `sdrdm-0.2.3/sdRDM/base/referencecheck.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/base/tree.py` & `sdrdm-0.2.3/sdRDM/base/tree.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/base/utils.py` & `sdrdm-0.2.3/sdRDM/base/utils.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/cli.py` & `sdrdm-0.2.3/sdRDM/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         None,
         help="URL to the templates GitHub repository",
     ),
     commit: Optional[str] = typer.Option(
         None,
         help="Commit hash from which this API was generated",
     ),
+    json_schemes: bool = typer.Option(
+        default=False,
+        help="Generate JSON schemes for the API",
+    ),
 ):
     """Generates a Python API based on the Markdown fiels found in the path.
 
     Args:
         path (str, optional): Path to the data model specifications.
         out (str, optional): Destination where the Software will be written.
         name (str, optional): Name of the resulting software model.
@@ -56,15 +60,22 @@
     if not all([url, commit]):
         url, commit = None, None
 
     if url and url.startswith("git://"):
         # Convert into valid URL
         url = url.replace("git://", "https://", 1)
 
-    generate_python_api(path=path, dirpath=out, libname=name, commit=commit, url=url)
+    generate_python_api(
+        path=path,
+        dirpath=out,
+        libname=name,
+        commit=commit,
+        url=url,
+        json_schemes=json_schemes,
+    )
 
 
 @app.command()
 def schema(
     path: str = typer.Option(..., help="Path to the schema definition"),
     out: str = typer.Option(".", help="Directory where the file will be written to."),
     name: str = typer.Option(..., help="Name of the schema"),
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/classrender.py` & `sdrdm-0.2.3/sdRDM/generator/classrender.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 
 
 def render_object(
     object: Dict,
     objects: List[Dict],
     enums: List[Dict],
     inherits: List[Dict],
+    namespaces: Dict,
     repo: Optional[str] = None,
     commit: Optional[str] = None,
     small_types: Dict = {},
+    add_id_field: bool = True,
 ) -> str:
     """Renders a class of type object coming from a parsed Markdown model"""
 
     all_objects = objects + enums
 
     if small_types:
         small_type_part = "\n".join(
             [
                 render_class(
                     object=subtype,
                     inherits=[],
                     objects=all_objects,
                     repo=repo,
                     commit=commit,
+                    namespaces=namespaces,
+                    add_id_field=add_id_field,
                 )
                 for subtype in small_types.values()
                 if subtype["origin"] == object["name"]
             ]
         )
     else:
         small_type_part = ""
@@ -42,20 +46,23 @@
     # Get the class body
     class_part = render_class(
         object=object,
         inherits=inherits,
         objects=all_objects,
         repo=repo,
         commit=commit,
+        namespaces=namespaces,
+        add_id_field=add_id_field,
     )
 
     methods_part = render_add_methods(
         object=object,
         objects=all_objects,
         small_types=small_types,
+        add_id_field=add_id_field,
     )
 
     validator_part = render_reference_validator(
         object=object,
         objects=all_objects,
     )
 
@@ -80,14 +87,16 @@
     return f"{imports}\n\n{class_body}"
 
 
 def render_class(
     object: Dict,
     inherits: List[Dict],
     objects: List[Dict],
+    namespaces: Dict,
+    add_id_field: bool,
     repo: Optional[str] = None,
     commit: Optional[str] = None,
 ) -> str:
     """Takes an object definition and returns a rendered string"""
 
     object = deepcopy(object)
     template = Template(
@@ -111,70 +120,94 @@
                 objects,
                 name,
             )
             for attr in object["attributes"]
         ],
         repo=repo,
         commit=commit,
+        namespaces=namespaces,
+        add_id_field=add_id_field,
     )
 
 
 def render_attribute(
     attribute: Dict,
     objects: List[Dict],
     obj_name: str,
 ) -> str:
     """Renders an attributeibute to code using a Jinja2 template"""
 
     attribute = deepcopy(attribute)
-    template = Template(
+    attr_template = Template(
         pkg_resources.read_text(
             jinja_templates,
             "attribute_template.jinja2",
         )
     )
 
+    leaf_template = Template(
+        pkg_resources.read_text(
+            jinja_templates,
+            "attribute_leaf_template.jinja2",
+        )
+    )
+
     is_multiple = "multiple" in attribute
     is_required = attribute["required"]
     is_all_optional = _is_optional_single_dtype(attribute, objects, obj_name)
     has_reference = "reference" in attribute
 
     tag = _extract_xml_alias(attribute)
     attribute["type"] = [
         f'"{dtype}"' if dtype == obj_name else dtype for dtype in attribute["type"]
     ]
 
     if is_multiple:
         attribute["default_factory"] = "ListPlus"
     elif not is_multiple and is_all_optional:
         attribute["default_factory"] = f"{attribute['type'][0]}"
-        del attribute["default"]
+
+        if "default" in attribute:
+            del attribute["default"]
 
     if has_reference:
         reference_types = get_reference_type(attribute["reference"], objects)
         attribute["type"] += reference_types
 
-    if is_multiple and tag != "None":
-        xml_alias = tag
-        tag = attribute["type"][0]
+    if tag and len(tag.split("/")) > 1:
+        xml_alias = "/".join(tag.split("/")[:-1])
+        tag = _transform(attribute["type"][0], tag.split("/")[-1])
         wrapped = True
     else:
         xml_alias = None
         wrapped = False
 
-    return template.render(
-        name=attribute.pop("name"),
-        required=attribute.pop("required"),
-        dtype=combine_types(attribute.pop("type"), is_multiple, is_required),
-        metadata=stringize_option_values(attribute),
-        field_type=_get_field_type(attribute),
-        wrapped=wrapped,
-        tag=tag,
-        xml_alias=xml_alias,
-    )
+    if xml_alias == obj_name or tag == obj_name:
+        return leaf_template.render(
+            name=attribute.pop("name"),
+            required=attribute.pop("required"),
+            dtype=combine_types(attribute.pop("type"), is_multiple, is_required),
+            metadata=stringize_option_values(attribute),
+            field_type=_get_field_type(attribute),
+            wrapped=wrapped,
+            tag=tag,
+            xml_alias=xml_alias,
+        )
+
+    else:
+        return attr_template.render(
+            name=attribute.pop("name"),
+            required=attribute.pop("required"),
+            dtype=combine_types(attribute.pop("type"), is_multiple, is_required),
+            metadata=stringize_option_values(attribute),
+            field_type=_get_field_type(attribute),
+            wrapped=wrapped,
+            tag=tag,
+            xml_alias=xml_alias,
+        )
 
 
 def _get_field_type(attribute: Dict) -> str:
     if "xml" not in attribute:
         return "element"
 
     if attribute["xml"].lstrip('"').startswith("@"):
@@ -260,14 +293,15 @@
         elif "()" in option:
             continue
         elif is_reference(key, option):
             continue
         elif key == "default_factory":
             continue
 
+        option = option.replace('"', "'")
         attribute[key] = f'"{option}"'
 
     return attribute
 
 
 def is_pure_string_type(value: str) -> Union[bool, str]:
     """Checks whether the given option value could be bool"""
@@ -297,15 +331,20 @@
     if len(option.split(".")) > 1 and option.count(" ") == 0:
         # Typically references to classes will follow pattern 'Something.something'
         return True
 
     return False
 
 
-def render_add_methods(object: Dict, objects: List[Dict], small_types: Dict) -> str:
+def render_add_methods(
+    object: Dict,
+    objects: List[Dict],
+    small_types: Dict,
+    add_id_field: bool,
+) -> str:
     """Renders add methods fro each non-native type of an attribute"""
 
     add_methods = []
 
     for attribute in object["attributes"]:
         complex_types = get_complex_types(attribute, objects)
         is_single_type = len(complex_types) == 1
@@ -313,20 +352,21 @@
         if "Unit" in attribute["type"] and "multiple" in attribute:
             add_methods.append(render_unit_add_method(attribute["name"]))
             continue
 
         for type in complex_types:
             add_methods.append(
                 render_single_add_method(
-                    attribute,
-                    type,
-                    objects,
-                    is_single_type,
-                    object["name"],
-                    small_types,
+                    attribute=attribute,
+                    type=type,
+                    objects=objects,
+                    is_single_type=is_single_type,
+                    obj_name=object["name"],
+                    small_types=small_types,
+                    add_id_field=add_id_field,
                 )
             )
 
     return "\n\n".join(add_methods)
 
 
 def get_complex_types(attribute: Dict, objects: List[Dict]) -> List[str]:
@@ -391,14 +431,15 @@
 def render_single_add_method(
     attribute: Dict,
     type: str,
     objects: List[Dict],
     is_single_type: bool,
     obj_name: str,
     small_types: Dict,
+    add_id_field: bool,
 ) -> str:
     """Renders an add method for an attribute that occurs multiple times"""
 
     attribute = deepcopy(attribute)
     objects = deepcopy(objects)
 
     template = Template(
@@ -416,14 +457,15 @@
 
     return template.render(
         attribute=attribute["name"],
         destination=destination,
         cls=type,
         signature=assemble_signature(type, objects, obj_name, small_types),
         summary=f"This method adds an object of type '{type}' to attribute {attribute['name']}",
+        add_id_field=add_id_field,
     )
 
 
 def render_unit_add_method(name: str):
     """
     Renders the template for adding a method to a unit.
 
@@ -449,14 +491,16 @@
     """Takes a non-native sdRDM type defined within the model and extracts all attributes"""
 
     try:
         sub_object = next(filter(lambda object: object["name"] == type, objects))
     except StopIteration:
         if type in small_types:
             sub_object = small_types[type]
+        elif type in DataTypes.__members__:
+            return []
         else:
             raise ValueError(f"Sub object '{type}' has no attributes.")
 
     sub_object_parent = sub_object.get("parent")
     sub_object_attrs = [
         convert_type(attribute, obj_name) for attribute in sub_object["attributes"]
     ]
@@ -549,14 +593,18 @@
     )
 
     for inherit in inherits:
         if inherit["child"] != object["name"]:
             continue
 
         parent_type = inherit["parent"]
+
+        if parent_type in DataTypes.__members__:
+            continue
+
         all_types += gather_all_types(
             get_object(parent_type, objects)["attributes"],
             objects,
             small_types,
         ) + [parent_type]
 
     # Sort types into local and from imports
@@ -648,16 +696,29 @@
     if object["type"] == "enum":
         return []
 
     attributes = object["attributes"]
     subtypes = gather_all_types(attributes, objects, small_types, object["name"])
 
     if object.get("parent"):
-        parent_obj = get_object(object["parent"], objects)
-        subtypes += gather_all_types(
-            parent_obj["attributes"], objects, small_types, parent_obj["name"]
-        )
+
+        if object["parent"] in DataTypes.__members__:
+            pass
+        else:
+            parent_obj = get_object(object["parent"], objects)
+            subtypes += gather_all_types(
+                parent_obj["attributes"], objects, small_types, parent_obj["name"]
+            )
 
     for subtype in subtypes:
         types.append(subtype)
 
     return types
+
+
+def _transform(dtype: str, tag: str) -> str:
+    """Transforms a dtype into a tag for special cases"""
+
+    if dtype == "MathML":
+        return "math"
+
+    return tag
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/codegen.py` & `sdrdm-0.2.3/sdRDM/generator/codegen.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     path: str,
     dirpath: str,
     libname: str,
     url: Optional[str] = None,
     commit: Optional[str] = None,
     only_classes: bool = False,
     use_formatter: bool = True,
+    json_schemes: bool = False,
 ) -> Optional[MarkdownParser]:
     """Generates a Python API based on a markdown model, which is parsed
     and code generated based on the specifications.
 
     Args:
         path (str): Path to the markdown model.
         dirpath (str): Directory to which the library will be written
@@ -48,37 +49,41 @@
     generate_api_from_parser(
         parser=parser,
         dirpath=dirpath,
         libname=libname,
         url=url,
         commit=commit,
         use_formatter=use_formatter,
+        json_schemes=json_schemes,
     )
 
 
 def generate_api_from_parser(
     parser: MarkdownParser,
     dirpath: str,
     libname: str,
+    json_schemes: bool,
     url: Optional[str] = None,
     commit: Optional[str] = None,
     use_formatter: bool = True,
 ):
     # Create directory structure
     libpath = create_directory_structure(dirpath, libname)
 
     # Write classes to the directory
     write_classes(
-        libpath,
-        parser.objects,
-        parser.enums,
-        parser.inherits,
-        use_formatter,
-        url,
-        commit,
+        libpath=libpath,
+        objects=parser.objects,
+        enums=parser.enums,
+        inherits=parser.inherits,
+        use_formatter=use_formatter,
+        repo=url,
+        commit=commit,
+        namespaces=parser.namespaces,
+        add_id_field=parser.add_id_field,
     )
 
     # Write init files
     core_init = render_core_init_file(parser.objects, parser.enums)
     save_rendered_to_file(
         core_init,
         os.path.join(libpath, "core", "__init__.py"),
@@ -90,44 +95,50 @@
         lib_init,
         os.path.join(libpath, "__init__.py"),
         use_formatter,
     )
 
     # Write schema to library
     generate_mermaid_schema(os.path.join(libpath, "schemes"), libname, parser)
-    _write_json_schemes(libpath, libname)
+
+    if json_schemes:
+        _write_json_schemes(libpath, libname)
 
 
 def write_classes(
     libpath: str,
     objects: List[Dict],
     enums: List[Dict],
     inherits: List[Dict],
     use_formatter: bool,
+    namespaces: Dict,
     repo: Optional[str] = None,
     commit: Optional[str] = None,
+    add_id_field: bool = True,
 ) -> None:
     """Renders classes that were parsed from a markdown model and creates a library."""
 
     # Keep track of small types
     small_types = {
         small_type["name"]: small_type
         for object in objects
         for small_type in object["subtypes"]
     }
 
     for object in objects:
         rendered = render_object(
-            object,
-            objects,
-            enums,
-            inherits,
-            repo,
-            commit,
-            small_types,
+            object=object,
+            objects=objects,
+            enums=enums,
+            inherits=inherits,
+            repo=repo,
+            commit=commit,
+            small_types=small_types,
+            namespaces=namespaces,
+            add_id_field=add_id_field,
         )
         path = os.path.join(libpath, "core", f"{object['name'].lower()}.py")
         save_rendered_to_file(rendered, path, use_formatter)
 
     for enum in enums:
         rendered = render_enum(enum)
         path = os.path.join(libpath, "core", f"{enum['name'].lower()}.py")
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/datatypes.py` & `sdrdm-0.2.3/sdRDM/generator/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,11 +137,12 @@
             "from numpy.typing import NDArray",
             "from h5py._hl.dataset import Dataset as H5Dataset",
             "from typing import Union",
         ],
     )
     H5Dataset = ("H5Dataset", ["from h5py._hl.dataset import Dataset as H5Dataset"])
     h5dataset = ("H5Dataset", ["from h5py._hl.dataset import Dataset as H5Dataset"])
+    RawXML = ("_Element", ["from lxml.etree import _Element"])
 
     @classmethod
     def get_value_list(cls):
         return [member.value[0] for member in cls]
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/enumrender.py` & `sdrdm-0.2.3/sdRDM/generator/enumrender.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/initrender.py` & `sdrdm-0.2.3/sdRDM/generator/initrender.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/schemagen.py` & `sdrdm-0.2.3/sdRDM/generator/schemagen.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/templates/add_method_template.jinja2` & `sdrdm-0.2.3/sdRDM/generator/templates/add_method_template.jinja2`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
     def add_{{ destination }}(
         self,
         {%- for attr in signature %}
         {{attr.name}}: {{attr.type}} {% if 'default' in attr%}= {{attr.default}} {% elif attr.multiple is true %}= ListPlus(){% endif %},
         {%- endfor %}
-        id: Optional[str] = None,
+        {% if add_id_field %}id: Optional[str] = None,{% endif %}
+        **kwargs,
     ) -> {{ cls }}:
         """
         {{summary}}
 
         Args:
-            id (str): Unique identifier of the '{{ cls }}' object. Defaults to 'None'.
+            {% if add_id_field %}id (str): Unique identifier of the '{{ cls }}' object. Defaults to 'None'.{% endif %}
             {%- for attr in signature %}
             {{attr.name}} ({{ attr.dtype }}): {{ attr.description }}.{% if 'default' in attr %} Defaults to {{attr.default}}{% endif %}
             {%- endfor %}
         """
 
         params = {
             {%- for attr in signature %}
@@ -22,8 +23,8 @@
         }
 
         if id is not None:
             params["id"] = id
 
         self.{{attribute}}.append({{cls}}(**params))
 
-        return self.{{attribute}}[-1]
+        return self.{{attribute}}[-1]
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/templates/attribute_template.jinja2` & `sdrdm-0.2.3/sdRDM/generator/templates/attribute_template.jinja2`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/templates/mermaid_class.jinja2` & `sdrdm-0.2.3/sdRDM/generator/templates/mermaid_class.jinja2`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/templates/reference_template.jinja2` & `sdrdm-0.2.3/sdRDM/generator/templates/reference_template.jinja2`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/generator/updater.py` & `sdrdm-0.2.3/sdRDM/generator/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Constants
 REFERENCE_PATTERN = r"get_[A-Za-z0-9\_]*_reference"
 ADDER_PATTERN = r"add_to_[A-Za-z0-9\_]*"
 INHERITANCE_PATTERN = r"class [A-Za-z0-9\_\.]*\(([A-Za-z0-9\_\.]*)\)\:"
 ATTRIBURE_PATTERN = r"description=(\"|\')[A-Za-z0-9\_\.]*"
 FUNCTION_PATTERN = r"def ([a-zA-Z0-9_]+)\("
 FUNCTION_NAME_PATTERN = r"def ([a-zA-Z0-9_]+)\("
+XML_PARSER_PATTERN = r"_parse_raw_xml_data"
 
 
 class ModuleOrder(Enum):
     IMPORT_SDRDM = auto()
     IMPORT_MISC = auto()
 
     FROM_TYPING = auto()
@@ -70,14 +71,16 @@
     for line_count, line in enumerate(previous_class):
         if not re.findall(FUNCTION_PATTERN, line):
             continue
 
         # Ignore adder functions
         if re.findall(ADDER_PATTERN, line):
             continue
+        elif re.findall(XML_PARSER_PATTERN, line):
+            continue
 
         # Account for decorators
         if previous_class[line_count - 1].strip().startswith("@"):
             method_starts.append(line_count - 1)
         else:
             method_starts.append(line_count)
```

### Comparing `sdrdm-0.2.2/sdRDM/generator/utils.py` & `sdrdm-0.2.3/sdRDM/generator/utils.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/markdown/enumutils.py` & `sdrdm-0.2.3/sdRDM/markdown/enumutils.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/markdown/markdownparser.py` & `sdrdm-0.2.3/sdRDM/markdown/markdownparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from io import StringIO
 import re
 
+import frontmatter
 from typing import List, Tuple, Dict, IO
 from markdown_it import MarkdownIt
 from markdown_it.token import Token
 from pydantic import BaseModel
 
 from sdRDM.generator.utils import camel_to_snake
 
@@ -13,22 +15,31 @@
 
 class MarkdownParser(BaseModel):
     objects: List = []
     enums: List = []
     inherits: List = []
     compositions: List = []
     external_objects: Dict = {}
+    namespaces: Dict = {}
+    add_id_field: bool = True
 
     @classmethod
     def parse(cls, handle: IO):
         """Parses a given markdown file to a mermaid schema from which code is generated."""
 
         parser = cls()
 
-        doc = MarkdownIt().parse(cls.clean_html_tags(handle.readlines()))
+        content = parser.clean_html_tags(handle.readlines())
+
+        # Extract frontmatter and markdown
+        metadata = frontmatter.load(StringIO(content))
+        parser.namespaces = metadata.get("xmlns", {})  # type: ignore
+        parser.add_id_field = metadata.get("id-field", True)  # type: ignore
+
+        doc = MarkdownIt().parse(parser._remove_header(content))
         modules, enumerations = parser.get_objects_and_enumerations(doc)
 
         for module, model in modules.items():
             parser.objects += [
                 obj
                 for obj in parse_markdown_module(module, model, parser.external_objects)
             ]
@@ -58,14 +69,30 @@
 
         self.objects += parser.objects
         self.enums += parser.enums
         self.inherits += parser.inherits
         self.compositions += parser.compositions
         self.external_objects.update(parser.external_objects)
 
+    @staticmethod
+    def _remove_header(text: str):
+        """
+        Removes the header from the given text.
+
+        Args:
+            text (str): The text containing the header.
+
+        Returns:
+            str: The text with the header removed.
+        """
+        header = re.search(r"^---\n.*?\n---\n", text, re.DOTALL)
+        if header:
+            text = text.replace(header.group(), "")
+        return text.strip()
+
     def _has_duplicate_object_names(self, parser):
         """Checks whether there are redundancies within the model"""
 
         assert isinstance(
             parser, self.__class__
         ), f"Expected parser of type 'MarkdownParser' got '{type(parser)}' instead."
```

### Comparing `sdrdm-0.2.2/sdRDM/markdown/objectutils.py` & `sdrdm-0.2.3/sdRDM/markdown/objectutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,17 @@
     assert match is not None, f"Option '{element.content}' is not valid."
 
     option, value = match.groups()
 
     if option.lower().strip() == "type":
         value = process_type_option(value, object_stack, external_types)
     elif option.lower().strip() == "multiple" and attribute_has_default(object_stack):
-        del object_stack[-1]["attributes"][-1]["default"]
+
+        if "default" in object_stack[-1]["attributes"][-1]:
+            del object_stack[-1]["attributes"][-1]["default"]
         object_stack[-1]["attributes"][-1]["default_factory"] = "ListPlus()"
 
     object_stack[-1]["attributes"][-1][option.strip().lower()] = value
 
 
 def attribute_has_default(object_stack: List[Dict]) -> bool:
     """Checks whether the current attribute has a default value or not"""
@@ -255,15 +257,17 @@
         _validate_dtype(dtype, object_stack)
 
         dtype = dtype.strip()
 
         if dtype.endswith("[]"):
             dtype = dtype.rstrip("[]")
             object_stack[-1]["attributes"][-1]["multiple"] = "True"
-            del object_stack[-1]["attributes"][-1]["default"]
+
+            if "default" in object_stack[-1]["attributes"][-1]:
+                del object_stack[-1]["attributes"][-1]["default"]
 
         if not dtype:
             continue
 
         if is_remote_type(dtype):
             dtype, cls_defs, url = process_remote_type(dtype)
             external_types[url] = cls_defs
```

### Comparing `sdrdm-0.2.2/sdRDM/markdown/smalltypes.py` & `sdrdm-0.2.3/sdRDM/markdown/smalltypes.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/sdRDM/tools/gitutils.py` & `sdrdm-0.2.3/sdRDM/tools/gitutils.py`

 * *Files identical despite different names*

### Comparing `sdrdm-0.2.2/PKG-INFO` & `sdrdm-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdRDM
-Version: 0.2.2
+Version: 0.2.3
 Summary: Software-driven RDM converts markdown data models into powerful objects that can be serialized to JSON, XML, YAML and HDF5
 License: MIT
 Author: Jan Range
 Author-email: range.jan@web.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,27 +22,28 @@
 Requires-Dist: gitpython (>=3.1.41,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: markdown-it-py (>=3.0.0,<4.0.0)
 Requires-Dist: nob (>=0.8.2,<0.9.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
-Requires-Dist: pydantic (==2.5.3)
-Requires-Dist: pydantic-xml (>=2.7.0,<3.0.0)
+Requires-Dist: pydantic (>=2.6.0,<3.0.0)
+Requires-Dist: pydantic-xml (>=2.9.0,<3.0.0)
+Requires-Dist: python-frontmatter (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: validators (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   Software-Driven RDM</br>
   <a href="https://badge.fury.io/py/sdRDM"><img src="https://badge.fury.io/py/sdRDM.svg" alt="PyPI version" height="18"></a>
-  <img src="https://img.shields.io/badge/python-3.9|3.10|3.11-blue.svg" alt="Build Badge">
+  <img src="https://img.shields.io/badge/python-3.9 | 3.10 | 3.11-blue.svg" alt="Build Badge">
   <img src="https://github.com/JR-1991/software-driven-rdm/actions/workflows/tests.yml/badge.svg" alt="Build Badge">
 </h1>
 <p align="center">
 With Software-driven Research Data Management (sdRDM), you can confidently specify data models using verbose Markdown documents and effortlessly convert them into powerful Python objects that can be serialized into any data exchange format.
 </p>
 
 ### 🏎 Features
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: sdRDM Version: 0.2.2 Summary: Software-driven RDM
+Metadata-Version: 2.1 Name: sdRDM Version: 0.2.3 Summary: Software-driven RDM
 converts markdown data models into powerful objects that can be serialized to
 JSON, XML, YAML and HDF5 License: MIT Author: Jan Range Author-email:
 range.jan@web.de Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: anytree
 (>=2.12.1,<3.0.0) Requires-Dist: astropy (>=6.0.0,<7.0.0) Requires-Dist:
 autoflake (==2.0.0) Requires-Dist: bigtree (>=0.15.4,<0.16.0) Requires-Dist:
 black (>=23.12.1,<24.0.0) Requires-Dist: dotted-dict (==1.1.3) Requires-Dist:
 email-validator (>=2.1.0.post1,<3.0.0) Requires-Dist: gitpython
 (>=3.1.41,<4.0.0) Requires-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-Dist: lxml
 (>=5.1.0,<6.0.0) Requires-Dist: markdown-it-py (>=3.0.0,<4.0.0) Requires-Dist:
 nob (>=0.8.2,<0.9.0) Requires-Dist: numpy (>=1.26.3,<2.0.0) Requires-Dist:
-pandas (>=2.1.4,<3.0.0) Requires-Dist: pydantic (==2.5.3) Requires-Dist:
-pydantic-xml (>=2.7.0,<3.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
-Dist: rich (>=13.7.0,<14.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-
-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: validators (>=0.22.0,<0.23.0)
-Description-Content-Type: text/markdown
+pandas (>=2.1.4,<3.0.0) Requires-Dist: pydantic (>=2.6.0,<3.0.0) Requires-Dist:
+pydantic-xml (>=2.9.0,<3.0.0) Requires-Dist: python-frontmatter
+(>=1.1.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich
+(>=13.7.0,<14.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: typer
+(>=0.9.0,<0.10.0) Requires-Dist: validators (>=0.22.0,<0.23.0) Description-
+Content-Type: text/markdown
    ************ SSooffttwwaarree--DDrriivveenn RRDDMM_[[_PP_yy_PP_II_ _vv_ee_rr_ss_ii_oo_nn_]][[BBuuiilldd BBaaddggee]][[BBuuiilldd BBaaddggee]] ************
   With Software-driven Research Data Management (sdRDM), you can confidently
  specify data models using verbose Markdown documents and effortlessly convert
 them into powerful Python objects that can be serialized into any data exchange
                                     format.
 ### ð Features - Generate and maintain RDM APIs via readable specifications
 in __Markdown__ - Data Models defined in sdRDM can be exported to __any
```

