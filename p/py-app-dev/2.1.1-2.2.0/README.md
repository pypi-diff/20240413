# Comparing `tmp/py_app_dev-2.1.1.tar.gz` & `tmp/py_app_dev-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_app_dev-2.1.1.tar", max compression
+gzip compressed data, was "py_app_dev-2.2.0.tar", max compression
```

## Comparing `py_app_dev-2.1.1.tar` & `py_app_dev-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-04-12 08:18:41.738261 py_app_dev-2.1.1/LICENSE
--rw-r--r--   0        0        0     4773 2024-04-12 08:18:41.738261 py_app_dev-2.1.1/README.md
--rw-r--r--   0        0        0     2606 2024-04-12 08:18:42.418264 py_app_dev-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-12 08:18:42.390264 py_app_dev-2.1.1/src/py_app_dev/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/__init__.py
--rw-r--r--   0        0        0     6223 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/docs_utils.py
--rw-r--r--   0        0        0      278 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/exceptions.py
--rw-r--r--   0        0        0     2237 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/logging.py
--rw-r--r--   0        0        0     4608 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/pipeline.py
--rw-r--r--   0        0        0     4917 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/runnable.py
--rw-r--r--   0        0        0    10609 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/scoop_wrapper.py
--rw-r--r--   0        0        0     2328 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/subprocess.py
--rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/__init__.py
--rw-r--r--   0        0        0     1862 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/event_manager.py
--rw-r--r--   0        0        0      258 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/presenter.py
--rw-r--r--   0        0        0      174 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/view.py
--rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/py.typed
--rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 py_app_dev-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-13 19:30:55.142812 py_app_dev-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4583 2024-04-13 19:30:55.142812 py_app_dev-2.2.0/README.md
+-rw-r--r--   0        0        0     3787 2024-04-13 19:30:55.958811 py_app_dev-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-13 19:30:55.958811 py_app_dev-2.2.0/src/py_app_dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/__init__.py
+-rw-r--r--   0        0        0     6103 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/docs_utils.py
+-rw-r--r--   0        0        0      279 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/exceptions.py
+-rw-r--r--   0        0        0     2235 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/logging.py
+-rw-r--r--   0        0        0     4450 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/pipeline.py
+-rw-r--r--   0        0        0     4906 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/runnable.py
+-rw-r--r--   0        0        0     9967 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     2258 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/subprocess.py
+-rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/__init__.py
+-rw-r--r--   0        0        0     1837 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/event_manager.py
+-rw-r--r--   0        0        0      258 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/presenter.py
+-rw-r--r--   0        0        0      174 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/view.py
+-rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/py.typed
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 py_app_dev-2.2.0/PKG-INFO
```

### Comparing `py_app_dev-2.1.1/LICENSE` & `py_app_dev-2.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 MIT License
 
-Copyright (c) 2023 cuinixam
+Copyright (c) 2024 cuinixam
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `py_app_dev-2.1.1/README.md` & `py_app_dev-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     <img src="https://img.shields.io/codecov/c/github/cuinixam/python-app-dev.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
     <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
   </a>
-  <a href="https://github.com/ambv/black">
-    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  <a href="https://github.com/astral-sh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="ruff">
   </a>
   <a href="https://github.com/pre-commit/pre-commit">
     <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
   </a>
 </p>
 <p align="center">
   <a href="https://pypi.org/project/py-app-dev/">
@@ -37,39 +37,34 @@
 Install this via pip (or your favourite package manager):
 
 `pip install py_app_dev`
 
 ## Start developing
 
 The project uses Poetry for dependencies management and packaging.
-If you do not have Poetry installed, you can run the `boostrap.ps1` script.
-This will install Python and Poetry as configured in `scoopfile.json`.
+Run the `bootstrap.ps1` script to install Python and create the virtual environment.
 
 ```powershell
-Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force
 .\bootstrap.ps1
 ```
 
-To install the development dependencies in a virtual environment, type:
+This will also generate a `poetry.lock` file, you should track this file in version control.
 
-```shell
-poetry install
-```
-
-This will also generate a `poetry.lock` file, you should track this file in version control. To execute the test suite, call pytest inside Poetry's virtual environment via `poetry run`:
+To execute the test suite, call pytest inside Poetry's virtual environment via `poetry run`:
 
 ```shell
-poetry run pytest
+.venv/Scripts/poetry run pytest
 ```
 
 Check out the Poetry documentation for more information on the available commands.
 
 For those using [VS Code](https://code.visualstudio.com/) there are tasks defined for the most common commands:
 
-- install development dependencies
+- bootstrap
+- install dependencies
 - run tests
 - run all checks configured for pre-commit
 - generate documentation
 
 See the `.vscode/tasks.json` for more details.
 
 ## Committing changes
@@ -89,9 +84,9 @@
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## Credits
 
 This package was created with
 [Copier](https://copier.readthedocs.io/) and the
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+[cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template)
 project template.
```

#### html2text {}

```diff
@@ -1,29 +1,26 @@
 # Python App Development
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
-                          _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
+                          _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 My application development modules. ## Installation Install this via pip (or
 your favourite package manager): `pip install py_app_dev` ## Start developing
-The project uses Poetry for dependencies management and packaging. If you do
-not have Poetry installed, you can run the `boostrap.ps1` script. This will
-install Python and Poetry as configured in `scoopfile.json`. ```powershell Set-
-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force
-.\bootstrap.ps1 ``` To install the development dependencies in a virtual
-environment, type: ```shell poetry install ``` This will also generate a
-`poetry.lock` file, you should track this file in version control. To execute
-the test suite, call pytest inside Poetry's virtual environment via `poetry
-run`: ```shell poetry run pytest ``` Check out the Poetry documentation for
-more information on the available commands. For those using [VS Code](https://
+The project uses Poetry for dependencies management and packaging. Run the
+`bootstrap.ps1` script to install Python and create the virtual environment.
+```powershell .\bootstrap.ps1 ``` This will also generate a `poetry.lock` file,
+you should track this file in version control. To execute the test suite, call
+pytest inside Poetry's virtual environment via `poetry run`: ```shell .venv/
+Scripts/poetry run pytest ``` Check out the Poetry documentation for more
+information on the available commands. For those using [VS Code](https://
 code.visualstudio.com/) there are tasks defined for the most common commands: -
-install development dependencies - run tests - run all checks configured for
+bootstrap - install dependencies - run tests - run all checks configured for
 pre-commit - generate documentation See the `.vscode/tasks.json` for more
 details. ## Committing changes This repository uses [commitlint](https://
 github.com/conventional-changelog/commitlint) for checking if the commit
 message meets the [conventional commit format](https://
 www.conventionalcommits.org/en). ## Contributors â¨ Thanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template.
+copier.readthedocs.io/) and the [cuinixam/pypackage-template](https://
+github.com/cuinixam/pypackage-template) project template.
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/cmd_line.py` & `py_app_dev-2.2.0/src/py_app_dev/core/cmd_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,20 @@
         self.parser: ArgumentParser
 
     @abstractmethod
     def run(self, args: Namespace) -> int:
         """Run the command with the provided arguments."""
 
     def register_parser(self, parser_adder) -> None:  # type: ignore
-        """Register the command parser.
+        """
+        Register the command parser.
 
         :param parser_adder: The return value of ``ArgumentParser.add_subparsers()``
         """
-        self.parser = parser_adder.add_parser(
-            self.name, help=self.description, exit_on_error=False
-        )
+        self.parser = parser_adder.add_parser(self.name, help=self.description, exit_on_error=False)
         self._register_arguments(self.parser)
 
     @abstractmethod
     def _register_arguments(self, parser: ArgumentParser) -> None:
         """Register arguments for the command."""
 
 
@@ -84,19 +83,15 @@
             raise ValueError(f"Command {command.name} already exists")
         self.commands[command.name] = command
         command.register_parser(self.subparsers)
         return self
 
 
 def is_type_optional(some_type: Any) -> bool:
-    return (
-        hasattr(some_type, "__origin__")
-        and some_type.__origin__ is Union
-        and type(None) in some_type.__args__
-    )
+    return hasattr(some_type, "__origin__") and some_type.__origin__ is Union and type(None) in some_type.__args__
 
 
 def is_type_list(some_type: Any) -> bool:
     return hasattr(some_type, "__origin__") and some_type.__origin__ is list
 
 
 def get_actual_type(some_type: Any) -> Any:
@@ -108,37 +103,35 @@
     elif is_type_list(some_type):
         # Return the element type of the list
         return get_args(some_type)[0]
     return some_type
 
 
 def register_arguments_for_config_dataclass(
-    parser: ArgumentParser, config_dataclass: Type  # type: ignore
+    parser: ArgumentParser,
+    config_dataclass: Type,  # type: ignore
 ) -> None:
-    """Helper function to register arguments for a dataclass.
-    This avoid having to manually register arguments for each field of the dataclass."""
+    """
+    Helper function to register arguments for a dataclass.
+
+    This avoid having to manually register arguments for each field of the dataclass.
+    """
     if not dataclasses.is_dataclass(config_dataclass):
         raise TypeError(f"{config_dataclass.__name__} is not a dataclass.")
 
     for field_name, field in config_dataclass.__dataclass_fields__.items():
-        parameter_default = (
-            field.default if not field.default == dataclasses.MISSING else None
-        )
+        parameter_default = field.default if not field.default == dataclasses.MISSING else None
         # Handle fields with optional list arguments
         if field.default_factory is list:
             parameter_default = []
-        parameter_help = field.metadata.get(
-            "help", f"Value for {field_name}. Default: {parameter_default}"
-        )
+        parameter_help = field.metadata.get("help", f"Value for {field_name}. Default: {parameter_default}")
         parameter_name = field_name.replace("_", "-")
         parameter_action = field.metadata.get("action", None)
         parameter_type = field.type
-        parameter_required = not (
-            is_type_optional(parameter_type) or parameter_default is not None
-        )
+        parameter_required = not (is_type_optional(parameter_type) or parameter_default is not None)
         parameter_nargs = "+" if is_type_list(parameter_type) else None
 
         # In case there is a custom deserialize method, override the type
         # to force the conversion using the deserialize method
         deserialize_method = field.metadata.get("deserialize", None)
         if deserialize_method:
             parameter_type = deserialize_method
@@ -154,10 +147,10 @@
             )
         else:
             parser.add_argument(
                 f"--{parameter_name}",
                 required=parameter_required,
                 type=get_actual_type(parameter_type),
                 default=parameter_default,
-                nargs=parameter_nargs,  # type: ignore
+                nargs=parameter_nargs,
                 help=parameter_help,
             )
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/docs_utils.py` & `py_app_dev-2.2.0/src/py_app_dev/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/logging.py` & `py_app_dev-2.2.0/src/py_app_dev/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Logging utilities. """
+"""Logging utilities."""
 
 import sys
 import time
 from contextlib import contextmanager
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, Generator, Optional, TypeVar
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/pipeline.py` & `py_app_dev-2.2.0/src/py_app_dev/core/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import importlib
-from abc import ABC
 from dataclasses import dataclass
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import Generic, List, Optional, OrderedDict, Type, TypeAlias, TypeVar
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    OrderedDict,
+    Type,
+    TypeAlias,
+    TypeVar,
+)
 
 from mashumaro import DataClassDictMixin
 
 from py_app_dev.core.exceptions import UserNotificationException
 
 
 @dataclass
@@ -20,104 +29,85 @@
     module: Optional[str] = None
     #: Step class name
     class_name: Optional[str] = None
     #: Step description
     description: Optional[str] = None
     #: Step timeout in seconds
     timeout_sec: Optional[int] = None
+    #: Custom step configuration
+    config: Optional[Dict[str, Any]] = None
 
 
 PipelineConfig: TypeAlias = OrderedDict[str, List[PipelineStepConfig]]
 
 TPipelineStep = TypeVar("TPipelineStep")
 
 
-class PipelineStep(ABC):
+class PipelineStep:
     """Base class for pipelines with no custom user steps."""
 
     pass
 
 
 @dataclass
 class PipelineStepReference(Generic[TPipelineStep]):
     """Once a Step is found, keep the Step class reference to be able to instantiate it later."""
 
     group_name: str
     _class: Type[TPipelineStep]
+    config: Optional[Dict[str, Any]] = None
 
 
 class PipelineLoader(Generic[TPipelineStep]):
     def __init__(self, pipeline_config: PipelineConfig, project_root_dir: Path) -> None:
         self.pipeline_config = pipeline_config
         self.project_root_dir = project_root_dir
 
     def load_steps(self) -> List[PipelineStepReference[TPipelineStep]]:
         result = []
         for group_name, steps_config in self.pipeline_config.items():
-            result.extend(
-                self._load_steps(group_name, steps_config, self.project_root_dir)
-            )
+            result.extend(self._load_steps(group_name, steps_config, self.project_root_dir))
         return result
 
     @staticmethod
     def _load_steps(
         group_name: str,
         steps_config: List[PipelineStepConfig],
         project_root_dir: Path,
     ) -> List[PipelineStepReference[TPipelineStep]]:
         result = []
         for step_config in steps_config:
             step_class_name = step_config.class_name or step_config.step
             if step_config.module:
-                step_class = PipelineLoader[TPipelineStep]._load_module_step(
-                    step_config.module, step_class_name
-                )
+                step_class = PipelineLoader[TPipelineStep]._load_module_step(step_config.module, step_class_name)
             elif step_config.file:
-                step_class = PipelineLoader[TPipelineStep]._load_user_step(
-                    project_root_dir.joinpath(step_config.file), step_class_name
-                )
+                step_class = PipelineLoader[TPipelineStep]._load_user_step(project_root_dir.joinpath(step_config.file), step_class_name)
             else:
-                raise UserNotificationException(
-                    f"Step '{step_class_name}' has no 'module' nor 'file' defined."
-                    " Please check your pipeline configuration."
-                )
-            result.append(PipelineStepReference(group_name, step_class))
+                raise UserNotificationException(f"Step '{step_class_name}' has no 'module' nor 'file' defined." " Please check your pipeline configuration.")
+            result.append(PipelineStepReference(group_name, step_class, step_config.config))
         return result
 
     @staticmethod
     def _load_user_step(python_file: Path, step_class_name: str) -> Type[TPipelineStep]:
         # Create a module specification from the file path
         spec = spec_from_file_location(f"user__{step_class_name}", python_file)
         if spec and spec.loader:
             step_module = module_from_spec(spec)
             # Import the module
             spec.loader.exec_module(step_module)
             try:
                 step_class = getattr(step_module, step_class_name)
             except AttributeError:
-                raise UserNotificationException(
-                    f"Could not load class '{step_class_name}' from file '{python_file}'."
-                    " Please check your pipeline configuration."
-                )
+                raise UserNotificationException(f"Could not load class '{step_class_name}' from file '{python_file}'." " Please check your pipeline configuration.") from None
             return step_class
-        raise UserNotificationException(
-            f"Could not load file '{python_file}'."
-            " Please check the file for any errors."
-        )
+        raise UserNotificationException(f"Could not load file '{python_file}'." " Please check the file for any errors.")
 
     @staticmethod
-    def _load_module_step(
-        module_name: str, step_class_name: str
-    ) -> Type[TPipelineStep]:
+    def _load_module_step(module_name: str, step_class_name: str) -> Type[TPipelineStep]:
         try:
             module = importlib.import_module(module_name)
             step_class = getattr(module, step_class_name)
         except ImportError:
-            raise UserNotificationException(
-                f"Could not load module '{module_name}'. Please check your pipeline configuration."
-            )
+            raise UserNotificationException(f"Could not load module '{module_name}'. Please check your pipeline configuration.") from None
         except AttributeError:
-            raise UserNotificationException(
-                f"Could not load class '{step_class_name}' from module '{module_name}'."
-                " Please check your pipeline configuration."
-            )
+            raise UserNotificationException(f"Could not load class '{step_class_name}' from module '{module_name}'." " Please check your pipeline configuration.") from None
         return step_class
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/runnable.py` & `py_app_dev-2.2.0/src/py_app_dev/core/runnable.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 from .logging import logger
 
 
 class Runnable(ABC):
     @abstractmethod
     def run(self) -> int:
-        """Run stage"""
+        """Run and return exit code."""
 
     @abstractmethod
     def get_name(self) -> str:
-        """Get stage name"""
+        """Get runnable name."""
 
     @abstractmethod
     def get_inputs(self) -> List[Path]:
-        """Get stage dependencies"""
+        """Get runnable dependencies."""
 
     @abstractmethod
     def get_outputs(self) -> List[Path]:
-        """Get stage outputs"""
+        """Get runnable outputs."""
 
 
 class RunInfoStatus(Enum):
     MATCH = (False, "Nothing changed. Previous execution info matches.")
     NO_INFO = (True, "No previous execution info found.")
     FILE_NOT_FOUND = (True, "File not found.")
     FILE_CHANGED = (True, "File has changed.")
@@ -37,25 +37,27 @@
 
     def __init__(self, should_run: bool, message: str) -> None:
         self.should_run = should_run
         self.message = message
 
 
 class Executor:
-    """Accepts Runnable objects and executes them.
-    It create a file with the same name as the runnable's name
-    and stores the inputs and outputs with their hashes.
-    If the file exists, it checks the hashes of the inputs and outputs
-    and if they match, it skips the execution."""
+    """
+    Accepts Runnable objects and executes them.
+
+    It create a file with the same name as the runnable's name and stores the inputs and outputs with their hashes.
+    If the file exists, it checks the hashes of the inputs and outputs and if they match, it skips the execution.
+    """
 
     RUN_INFO_FILE_EXTENSION = ".deps.json"
 
-    def __init__(self, cache_dir: Path, force_run: bool = False) -> None:
+    def __init__(self, cache_dir: Path, force_run: bool = False, dry_run: bool = False) -> None:
         self.cache_dir = cache_dir
         self.force_run = force_run
+        self.dry_run = dry_run
 
     @staticmethod
     def get_file_hash(path: Path) -> Optional[str]:
         if path.is_file():
             with open(path, "rb") as file:
                 bytes = file.read()
                 readable_hash = hashlib.sha256(bytes).hexdigest()
@@ -71,22 +73,16 @@
         def file_hash_to_str(file_hash: Optional[str]) -> str:
             if file_hash is None:
                 return "NOT_FOUND"
             else:
                 return file_hash
 
         file_info = {
-            "inputs": {
-                str(path): file_hash_to_str(self.get_file_hash(path))
-                for path in runnable.get_inputs()
-            },
-            "outputs": {
-                str(path): file_hash_to_str(self.get_file_hash(path))
-                for path in runnable.get_outputs()
-            },
+            "inputs": {str(path): file_hash_to_str(self.get_file_hash(path)) for path in runnable.get_inputs()},
+            "outputs": {str(path): file_hash_to_str(self.get_file_hash(path)) for path in runnable.get_outputs()},
         }
 
         run_info_path = self.get_runnable_run_info_file(runnable)
         run_info_path.parent.mkdir(parents=True, exist_ok=True)
         with run_info_path.open("w") as f:
             # pretty print the json file
             json.dump(file_info, f, indent=4)
@@ -117,18 +113,16 @@
         else:
             return RunInfoStatus.NOTHING_TO_CHECK
         return RunInfoStatus.MATCH
 
     def execute(self, runnable: Runnable) -> int:
         run_info_status = self.previous_run_info_matches(runnable)
         if run_info_status.should_run:
-            logger.info(
-                f"Runnable '{runnable.get_name()}' must run. {run_info_status.message}"
-            )
+            logger.info(f"Runnable '{runnable.get_name()}' must run. {run_info_status.message}")
+            if self.dry_run:
+                return 0
             exit_code = runnable.run()
             self.store_run_info(runnable)
             return exit_code
-        logger.info(
-            f"Runnable '{runnable.get_name()}' execution skipped. {run_info_status.message}"
-        )
+        logger.info(f"Runnable '{runnable.get_name()}' execution skipped. {run_info_status.message}")
 
         return 0
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/scoop_wrapper.py` & `py_app_dev-2.2.0/src/py_app_dev/core/scoop_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def get_env_add_path(self) -> List[Path]:
         """Return the list of env_add_path paths."""
         return [self.path.joinpath(env_add_path) for env_add_path in self.env_add_path]
 
     def get_all_required_paths(self) -> List[Path]:
         """Return the list of all required paths, maintaining order and removing duplicates."""
-        all_paths = [self.path] + self.get_bin_paths() + self.get_env_add_path()
+        all_paths = [self.path, *self.get_bin_paths(), *self.get_env_add_path()]
         unique_paths = list(dict.fromkeys(all_paths))
         return unique_paths
 
 
 @dataclass
 class InstalledScoopApp(InstalledApp):
     #: App scoop manifest file
@@ -90,187 +90,142 @@
         self.logger = logger.bind()
 
     @property
     def apps_directory(self) -> Path:
         return self.scoop_root_dir.joinpath("apps")
 
     def install(self, scoop_file: Path) -> List[InstalledScoopApp]:
-        """Install scoop apps from a scoop file.
-        It returns a list with all apps required to be installed as installed apps."""
-        return self.do_install(
-            ScoopInstallConfigFile.from_file(scoop_file), self.get_installed_apps()
-        )
+        """
+        Install scoop apps from a scoop file.
+
+        It returns a list with all apps required to be installed as installed apps.
+        """
+        return self.do_install(ScoopInstallConfigFile.from_file(scoop_file), self.get_installed_apps())
 
     def _find_scoop_executable(self) -> Path:
         scoop_path = which("scoop")
         if not scoop_path:
             scoop_path = Path().home().joinpath("scoop", "shims", "scoop.cmd")
             if not scoop_path.is_file():
-                raise UserNotificationException(
-                    "Scoop not found in PATH or user home directory."
-                    " Please install Scoop and run the build script again."
-                )
+                raise UserNotificationException("Scoop not found in PATH or user home directory." " Please install Scoop and run the build script again.")
         return scoop_path
 
     def _find_scoop_root_dir(self, scoop_executable_path: Path) -> Path:
         pattern = r"^(.*?/scoop/)"
         match = re.match(pattern, scoop_executable_path.absolute().as_posix())
 
         if match:
             return Path(match.group(1))
         else:
-            raise UserNotificationException(
-                f"Could not determine scoop directory for {scoop_executable_path}."
-            )
+            raise UserNotificationException(f"Could not determine scoop directory for {scoop_executable_path}.")
 
-    def parse_bin_dirs(
-        self, bin_data: Union[str, List[Union[str, List[str]]]]
-    ) -> List[Path]:
+    def parse_bin_dirs(self, bin_data: Union[str, List[Union[str, List[str]]]]) -> List[Path]:
         """Parse the bin directory from the manifest file."""
 
         def get_parent_dir(bin_entry: Union[str, List[str]]) -> Optional[Path]:
-            bin_path = (
-                Path(bin_entry[0]) if isinstance(bin_entry, list) else Path(bin_entry)
-            )
+            bin_path = Path(bin_entry[0]) if isinstance(bin_entry, list) else Path(bin_entry)
             return bin_path.parent if len(bin_path.parts) > 1 else None
 
         result = []
         if isinstance(bin_data, str):
             result = [parent for parent in [get_parent_dir(bin_data)] if parent]
         elif isinstance(bin_data, list):
-            result = [
-                parent
-                for parent in [get_parent_dir(bin_entry) for bin_entry in bin_data]
-                if parent
-            ]
+            result = [parent for parent in [get_parent_dir(bin_entry) for bin_entry in bin_data] if parent]
         # Remove duplicates and maintain order
         return list(dict.fromkeys(result))
 
     def parse_env_path_dirs(self, env_paths: Union[str, List[str]]) -> List[Path]:
         """Parse the env_add_path directories from the manifest file."""
-
         if isinstance(env_paths, str):
             return [Path(env_paths)]
         elif isinstance(env_paths, list):
             return [Path(env_path) for env_path in env_paths]
 
     def parse_manifest_file(self, manifest_file: Path) -> InstalledScoopApp:
         app_directory: Path = manifest_file.parent
         tool_name: str = app_directory.parent.name
         with open(manifest_file) as f:
             manifest_data: Dict[str, Any] = json.load(f)
             tool_version: str = manifest_data.get("version", None)
             bin_dirs: List[Path] = self.parse_bin_dirs(manifest_data.get("bin", []))
-            env_add_path: List[Path] = self.parse_env_path_dirs(
-                manifest_data.get("env_add_path", [])
-            )
+            env_add_path: List[Path] = self.parse_env_path_dirs(manifest_data.get("env_add_path", []))
             return InstalledScoopApp(
                 name=tool_name,
                 version=tool_version,
                 path=app_directory,
                 manifest_file=manifest_file,
                 bin_dirs=bin_dirs,
                 env_add_path=env_add_path,
             )
 
     def get_installed_apps(self) -> List[InstalledScoopApp]:
         installed_tools: List[InstalledScoopApp] = []
         self.logger.info(f"Looking for installed apps in {self.apps_directory}")
-        manifest_files = [
-            file
-            for file in self.apps_directory.glob("*/*/manifest.json")
-            if "current" != file.parent.name
-        ]
+        manifest_files = [file for file in self.apps_directory.glob("*/*/manifest.json") if "current" != file.parent.name]
 
         with ThreadPoolExecutor() as executor:
-            future_to_file = {
-                executor.submit(self.parse_manifest_file, manifest_file): manifest_file
-                for manifest_file in manifest_files
-            }
+            future_to_file = {executor.submit(self.parse_manifest_file, manifest_file): manifest_file for manifest_file in manifest_files}
             for future in as_completed(future_to_file):
                 installed_tools.append(future.result())
 
         return installed_tools
 
     def do_install(
         self,
         scoop_install_config: ScoopInstallConfigFile,
         installed_apps: List[InstalledScoopApp],
     ) -> List[InstalledScoopApp]:
         """Install scoop apps from a scoop file."""
-
-        newly_installed_apps = self.do_install_missing(
-            scoop_install_config, installed_apps
-        )
+        newly_installed_apps = self.do_install_missing(scoop_install_config, installed_apps)
         # If some apps where just installed we need to update the list of installed apps
         if newly_installed_apps:
-            self.logger.info(
-                "New apps were installed, update the list of installed apps."
-            )
+            self.logger.info("New apps were installed, update the list of installed apps.")
             updated_installed_apps = self.get_installed_apps()
         else:
             updated_installed_apps = installed_apps
-        apps = self.map_required_apps_to_installed_apps(
-            scoop_install_config.app_names, updated_installed_apps
-        )
+        apps = self.map_required_apps_to_installed_apps(scoop_install_config.app_names, updated_installed_apps)
         return apps
 
     def do_install_missing(
         self,
         scoop_install_config: ScoopInstallConfigFile,
         installed_apps: List[InstalledScoopApp],
     ) -> List[ScoopFileElement]:
         """Check which apps are installed and install the missing ones."""
-        apps_to_install = self.get_tools_to_be_installed(
-            scoop_install_config, installed_apps
-        )
+        apps_to_install = self.get_tools_to_be_installed(scoop_install_config, installed_apps)
         if not apps_to_install:
             self.logger.info("All Scoop apps already installed. Skip installation.")
             return []
         already_installed_apps = set(scoop_install_config.apps) - set(apps_to_install)
         if already_installed_apps:
-            self.logger.info(
-                f"Scoop apps already installed: {','.join(str(app) for app in already_installed_apps)}"
-            )
-        self.logger.info(
-            f"Start installing missing apps: {','.join(str(app) for app in apps_to_install)}"
-        )
+            self.logger.info(f"Scoop apps already installed: {','.join(str(app) for app in already_installed_apps)}")
+        self.logger.info(f"Start installing missing apps: {','.join(str(app) for app in apps_to_install)}")
 
         # Create a temporary scoopfile with the remaining apps to install and install them
         with TemporaryDirectory() as tmp_dir:
             tmp_scoop_file = Path(tmp_dir).joinpath("scoopfile.json")
-            ScoopInstallConfigFile(
-                scoop_install_config.buckets, apps_to_install
-            ).to_file(tmp_scoop_file)
-            SubprocessExecutor(
-                [self.scoop_executable, "import", tmp_scoop_file]
-            ).execute()
+            ScoopInstallConfigFile(scoop_install_config.buckets, apps_to_install).to_file(tmp_scoop_file)
+            SubprocessExecutor([self.scoop_executable, "import", tmp_scoop_file]).execute()
         return apps_to_install
 
     @staticmethod
     def map_required_apps_to_installed_apps(
         app_names: List[str],
         installed_apps: List[InstalledScoopApp],
     ) -> List[InstalledScoopApp]:
         """Map the required apps to the installed apps."""
         # convert the list of installed apps into a dictionary for faster lookup
         installed_apps_dict = {app.name: app for app in installed_apps}
         try:
             apps = [installed_apps_dict[app_name] for app_name in app_names]
         except KeyError as e:
-            raise UserNotificationException(
-                f"Could not find {e} in the installed apps. Something went wrong during the scoop installation."
-            )
+            raise UserNotificationException(f"Could not find {e} in the installed apps. Something went wrong during the scoop installation.") from None
         return apps
 
     @staticmethod
     def get_tools_to_be_installed(
         scoop_install_config: ScoopInstallConfigFile,
         installed_tools: List[InstalledScoopApp],
     ) -> List[ScoopFileElement]:
         """Check which apps are installed and install the missing ones."""
         installed_tools_names = {tool.name for tool in installed_tools}
-        return [
-            app
-            for app in scoop_install_config.apps
-            if app.name not in installed_tools_names
-        ]
+        return [app for app in scoop_install_config.apps if app.name not in installed_tools_names]
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/core/subprocess.py` & `py_app_dev-2.2.0/src/py_app_dev/core/subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,30 +33,24 @@
         try:
             self.logger.info(f"Running command: {self.command}")
             cwd_path = (self.current_working_directory or Path.cwd()).as_posix()
             with subprocess.Popen(
                 self.command.split(),
                 cwd=cwd_path,
                 stdout=(subprocess.PIPE if self.capture_output else subprocess.DEVNULL),
-                stderr=(
-                    subprocess.STDOUT if self.capture_output else subprocess.DEVNULL
-                ),
+                stderr=(subprocess.STDOUT if self.capture_output else subprocess.DEVNULL),
                 text=True,
                 env=self.env,
-                shell=self.shell,
+                shell=self.shell,  # noqa: S603
             ) as process:  # nosec
                 if self.capture_output and process.stdout is not None:
                     for line in iter(process.stdout.readline, ""):
                         self.logger.info(line.strip())
                 process.wait()
 
             # Check return code
             if process.returncode != 0:
                 raise subprocess.CalledProcessError(process.returncode, self.command)
         except subprocess.CalledProcessError as e:
-            raise UserNotificationException(
-                f"Command '{self.command}' failed with return code {e.returncode}"
-            )
+            raise UserNotificationException(f"Command '{self.command}' failed with return code {e.returncode}") from None
         except FileNotFoundError as e:
-            raise UserNotificationException(
-                f"Command '{self.command}' failed with error {e}"
-            )
+            raise UserNotificationException(f"Command '{self.command}' failed with error {e}") from None
```

### Comparing `py_app_dev-2.1.1/src/py_app_dev/mvp/event_manager.py` & `py_app_dev-2.2.0/src/py_app_dev/mvp/event_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 class EventID(Enum):
     pass
 
 
 class EventManager:
     """
-    Manages events and their subscribers. One can register callbacks to specific events
-    with any number of arguments. When an event is triggered, all subscribers are called
+    Manages events and their subscribers.
+
+    One can register callbacks to specific events with any number of arguments.
+    When an event is triggered, all subscribers are called
     TODO: There is no check if the callback has the correct number of arguments.
     """
 
     def __init__(self) -> None:
         self._events: Dict[EventID, List[EventCallback]] = {}
 
     def create_event_trigger(self, event_id: EventID) -> EventTrigger:
@@ -27,17 +29,15 @@
         """Triggers an event and calls all subscribers."""
         for callback in self._events.get(event_id, []):
             callback(*args, **kwargs)
 
     def subscribe(self, event_id: EventID, callback: EventCallback) -> None:
         """Subscribes a callback to an event."""
         if self.is_already_subscribed(event_id, callback):
-            raise ValueError(
-                f"Callback {callback} is already subscribed to event {event_id}"
-            )
+            raise ValueError(f"Callback {callback} is already subscribed to event {event_id}")
         self._events.setdefault(event_id, []).append(callback)
 
     def unsubscribe(self, event_id: EventID, callback: EventCallback) -> None:
         """Unsubscribes a callback from an event."""
         self._events[event_id].remove(callback)
 
     def is_already_subscribed(self, event_id: EventID, callback: EventCallback) -> bool:
```

### Comparing `py_app_dev-2.1.1/PKG-INFO` & `py_app_dev-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-app-dev
-Version: 2.1.1
+Version: 2.2.0
 Summary: My application development modules.
 Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,16 +38,16 @@
     <img src="https://img.shields.io/codecov/c/github/cuinixam/python-app-dev.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
     <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
   </a>
-  <a href="https://github.com/ambv/black">
-    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  <a href="https://github.com/astral-sh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="ruff">
   </a>
   <a href="https://github.com/pre-commit/pre-commit">
     <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
   </a>
 </p>
 <p align="center">
   <a href="https://pypi.org/project/py-app-dev/">
@@ -64,39 +64,34 @@
 Install this via pip (or your favourite package manager):
 
 `pip install py_app_dev`
 
 ## Start developing
 
 The project uses Poetry for dependencies management and packaging.
-If you do not have Poetry installed, you can run the `boostrap.ps1` script.
-This will install Python and Poetry as configured in `scoopfile.json`.
+Run the `bootstrap.ps1` script to install Python and create the virtual environment.
 
 ```powershell
-Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force
 .\bootstrap.ps1
 ```
 
-To install the development dependencies in a virtual environment, type:
+This will also generate a `poetry.lock` file, you should track this file in version control.
 
-```shell
-poetry install
-```
-
-This will also generate a `poetry.lock` file, you should track this file in version control. To execute the test suite, call pytest inside Poetry's virtual environment via `poetry run`:
+To execute the test suite, call pytest inside Poetry's virtual environment via `poetry run`:
 
 ```shell
-poetry run pytest
+.venv/Scripts/poetry run pytest
 ```
 
 Check out the Poetry documentation for more information on the available commands.
 
 For those using [VS Code](https://code.visualstudio.com/) there are tasks defined for the most common commands:
 
-- install development dependencies
+- bootstrap
+- install dependencies
 - run tests
 - run all checks configured for pre-commit
 - generate documentation
 
 See the `.vscode/tasks.json` for more details.
 
 ## Committing changes
@@ -116,10 +111,10 @@
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## Credits
 
 This package was created with
 [Copier](https://copier.readthedocs.io/) and the
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+[cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template)
 project template.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-app-dev Version: 2.1.1 Summary: My application
+Metadata-Version: 2.1 Name: py-app-dev Version: 2.2.0 Summary: My application
 development modules. Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -11,34 +11,31 @@
 (>=0.7.1,<0.8.0) Requires-Dist: mashumaro (>=3.9.1,<4.0.0) Project-URL: Bug
 Tracker, https://github.com/cuinixam/python-app-dev/issues Project-URL:
 Changelog, https://github.com/cuinixam/python-app-dev/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://python-app-dev.readthedocs.io Project-URL:
 Repository, https://github.com/cuinixam/python-app-dev Description-Content-
 Type: text/markdown # Python App Development
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
-                          _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
+                          _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 My application development modules. ## Installation Install this via pip (or
 your favourite package manager): `pip install py_app_dev` ## Start developing
-The project uses Poetry for dependencies management and packaging. If you do
-not have Poetry installed, you can run the `boostrap.ps1` script. This will
-install Python and Poetry as configured in `scoopfile.json`. ```powershell Set-
-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force
-.\bootstrap.ps1 ``` To install the development dependencies in a virtual
-environment, type: ```shell poetry install ``` This will also generate a
-`poetry.lock` file, you should track this file in version control. To execute
-the test suite, call pytest inside Poetry's virtual environment via `poetry
-run`: ```shell poetry run pytest ``` Check out the Poetry documentation for
-more information on the available commands. For those using [VS Code](https://
+The project uses Poetry for dependencies management and packaging. Run the
+`bootstrap.ps1` script to install Python and create the virtual environment.
+```powershell .\bootstrap.ps1 ``` This will also generate a `poetry.lock` file,
+you should track this file in version control. To execute the test suite, call
+pytest inside Poetry's virtual environment via `poetry run`: ```shell .venv/
+Scripts/poetry run pytest ``` Check out the Poetry documentation for more
+information on the available commands. For those using [VS Code](https://
 code.visualstudio.com/) there are tasks defined for the most common commands: -
-install development dependencies - run tests - run all checks configured for
+bootstrap - install dependencies - run tests - run all checks configured for
 pre-commit - generate documentation See the `.vscode/tasks.json` for more
 details. ## Committing changes This repository uses [commitlint](https://
 github.com/conventional-changelog/commitlint) for checking if the commit
 message meets the [conventional commit format](https://
 www.conventionalcommits.org/en). ## Contributors â¨ Thanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template.
+copier.readthedocs.io/) and the [cuinixam/pypackage-template](https://
+github.com/cuinixam/pypackage-template) project template.
```

