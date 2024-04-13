# Comparing `tmp/qcop-0.5.3.tar.gz` & `tmp/qcop-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcop-0.5.3.tar", max compression
+gzip compressed data, was "qcop-0.5.4.tar", max compression
```

## Comparing `qcop-0.5.3.tar` & `qcop-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-04-11 22:35:46.722615 qcop-0.5.3/LICENSE
--rw-r--r--   0        0        0     7283 2024-04-11 22:35:46.722615 qcop-0.5.3/README.md
--rw-r--r--   0        0        0     1832 2024-04-11 22:35:46.726615 qcop-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      248 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/__init__.py
--rw-r--r--   0        0        0      360 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/__init__.py
--rw-r--r--   0        0        0    12380 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/base.py
--rw-r--r--   0        0        0     1487 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/file.py
--rw-r--r--   0        0        0    11141 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/geometric.py
--rw-r--r--   0        0        0     2111 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/qcengine.py
--rw-r--r--   0        0        0     4662 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/terachem.py
--rw-r--r--   0        0        0     8709 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/utils.py
--rw-r--r--   0        0        0     4419 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/xtb.py
--rw-r--r--   0        0        0     3639 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/exceptions.py
--rw-r--r--   0        0        0     3134 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/main.py
--rw-r--r--   0        0        0        0 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/py.typed
--rw-r--r--   0        0        0     3363 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/utils.py
--rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-13 02:25:25.190613 qcop-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7283 2024-04-13 02:25:25.190613 qcop-0.5.4/README.md
+-rw-r--r--   0        0        0     1832 2024-04-13 02:25:25.190613 qcop-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-04-13 02:25:25.190613 qcop-0.5.4/qcop/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-13 02:25:25.190613 qcop-0.5.4/qcop/adapters/__init__.py
+-rw-r--r--   0        0        0    12404 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/base.py
+-rw-r--r--   0        0        0     1487 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/file.py
+-rw-r--r--   0        0        0    11141 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/geometric.py
+-rw-r--r--   0        0        0     2111 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/qcengine.py
+-rw-r--r--   0        0        0     4602 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/terachem.py
+-rw-r--r--   0        0        0     8751 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/utils.py
+-rw-r--r--   0        0        0     4492 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/adapters/xtb.py
+-rw-r--r--   0        0        0     3639 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/exceptions.py
+-rw-r--r--   0        0        0     3134 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/main.py
+-rw-r--r--   0        0        0        0 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/py.typed
+-rw-r--r--   0        0        0     3363 2024-04-13 02:25:25.194613 qcop-0.5.4/qcop/utils.py
+-rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.4/PKG-INFO
```

### Comparing `qcop-0.5.3/LICENSE` & `qcop-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/README.md` & `qcop-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/pyproject.toml` & `qcop-0.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qcop"
-version = "0.5.3"
+version = "0.5.4"
 description = "A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcop-0.5.3/qcop/adapters/base.py` & `qcop-0.5.4/qcop/adapters/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self,
         inp_obj: InputBase,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
         **kwargs,
     ) -> Tuple[ResultsBase, str]:
         """Subclasses should implement this method with custom compute logic."""
+        raise NotImplementedError
 
     def compute(
         self,
         inp_obj: InputBase,
         *,
         scratch_dir: Optional[StrOrPath] = None,
         rm_scratch_dir: bool = True,
@@ -90,16 +91,15 @@
                 accept the in-process stdout/stderr output as a string for its first
                 argument.
             update_interval: The minimum time in seconds between calls to the
                 update_func.
             print_stdout: Whether to print stdout/stderr to the terminal in real time as
                 the program executes. Will be ignored if an update_func passed.
             raise_exc: If False, qcop will return a ProgramFailure object when the QC
-                program fails rather than raise an exception. qcop exceptions not
-                related to the external program failure will always be raised.
+                program fails rather than raise an exception.
             propagate_wfn: For any adapter performing a sequential task, such
                 as a geometry optimization, propagate the wavefunction from the previous
                 step to the next step. This is useful for accelerating convergence by
                 using a previously computed wavefunction as a starting guess. If an
                 adapter does not support wavefunction propagation, an AdapterInputError
                 will be raised.
             **kwargs: Additional keyword arguments to pass to the adapter or
@@ -119,108 +119,111 @@
                 on the system.
             AdapterInputError: If the input is invalid for the adapter.
             ExternalProgramExecutionError: If the program fails during execution and
                 raise_exc=True.
             QCEngineError: If QCEngine performed the computation, fails and
                 raise_exc=True.
         """
-        self.validate_input(inp_obj)
-        # Set update_func if print_stdout is True and update_func is None
+        # Print stdout to terminal in real time as program executes
         if print_stdout and update_func is None:
             update_func, update_interval = (
                 lambda _, stdout_new: print(stdout_new),
                 0.1,
             )
 
-        # Change cwd to a temporary directory to run the program.
+        # cd to a temporary directory to run the program.
         with tmpdir(scratch_dir, rm_scratch_dir) as final_scratch_dir:
             if self.write_files:  # Write non structured input files to disk.
                 inp_obj.save_files()
 
+            # Define outputs
             output_dict: Dict[str, Optional[Union[str, QCIOModelBase]]] = {}
-            stdout: Optional[str]
+            stdout: Optional[str] = None
+            # TODO: Update when qcio updates to allow None results
+            results: Optional[ResultsBase] = None
+            exc: Optional[QCOPBaseError] = None
+            program_version: Optional[str] = None
 
             start = time()
-            qcop_exception = None
-            results: Optional[ResultsBase]
             try:
-                # Execute the program; return results and stdout
+                # Validate input object
+                self.validate_input(inp_obj)
+
+                # Execute the program. results will be None if FileInput
                 results, stdout = self.compute_results(
                     inp_obj,
                     update_func,
                     update_interval,
                     propagate_wfn=propagate_wfn,
                     **kwargs,
                 )
                 # None value covers FileInput case
+                # TODO: Update this to ProgramOutput[type(inp_obj), type(results)]
                 output_cls = calctype_to_output(getattr(inp_obj, "calctype", None))
+                program_version = self.program_version(stdout)
+
+                # Optionally collect wavefunction file
+                if collect_wfn and not collect_files:
+                    output_dict["files"] = self.collect_wfn()
+
             except QCOPBaseError as e:
-                qcop_exception = e
                 # Set variables to construct a ProgramFailure object.
-                output_cls = ProgramFailure
-                results = getattr(e, "results", None)  # Any half-completed results
-                stdout = getattr(e, "stdout", None)
+                exc, output_cls = e, ProgramFailure
+                results = getattr(e, "results", results)  # Any half-completed results
+                stdout = getattr(e, "stdout", stdout)
                 # For mypy because e.stdout is not of a known type
                 stdout = str(stdout) if stdout is not None else None
                 output_dict["traceback"] = traceback.format_exc()
 
-            # Construct Provenance object
             wall_time = time() - start
+
+            # Construct Provenance object
             provenance = construct_provenance(
-                self.program, self.program_version(stdout), final_scratch_dir, wall_time
+                self.program,
+                program_version,
+                final_scratch_dir,
+                wall_time,
             )
 
-            # Construct output object
-            stdout = (  # Always collect for failures; otherwise obey collect_stdout
-                None if output_cls != ProgramFailure and not collect_stdout else stdout
-            )
+            # Always collect for failures; otherwise obey collect_stdout
+            stdout = stdout if collect_stdout or output_cls == ProgramFailure else None
 
-            # Ensure results is not None to maintain interface
+            # Construct output object
             results = results if results is not None else ResultsBase()
             output_dict.update(
                 {
                     "input_data": inp_obj,
                     "stdout": stdout,
                     "results": results,
                     "provenance": provenance,
                 }
             )
-
             output_obj = output_cls(**output_dict)
 
-            # Optionally collect output files
+            # Collect files generated by the program
             if collect_files or isinstance(inp_obj, FileInput):
-                # Collect output files from the calc_dir
                 output_obj.open_files(
                     final_scratch_dir, recursive=True, exclude=inp_obj.files.keys()
                 )
 
-            # Optionally collect wavefunction file
-            if collect_wfn and not collect_files:
-                # Collect wavefunction file from the calc_dir
-                self.collect_wfn(output_obj)
-
         # Append ProgramFailures to exception and raise if raise_exc=True
-        # Helpful for BigChem exception handling
-        if raise_exc and qcop_exception:
-            qcop_exception.program_failure = output_obj
+        # Helpful for BigChem and ChemCloud exception handling
+        if raise_exc and exc:
+            exc.program_failure = output_obj
             # Updating .args is necessary for Celery to properly serialize the exception
-            qcop_exception.args = (*qcop_exception.args, output_obj)
-            raise qcop_exception
+            exc.args = (*exc.args, output_obj)
+            raise exc
 
         return output_obj
 
-    def collect_wfn(self, output_obj: OutputBase) -> None:
+    def collect_wfn(self) -> Dict[str, Union[str, bytes]]:
         """Collect the wavefunction file(s) from the scratch_dir.
 
-        Args:
-            output_obj: The output object to add the wavefunction file(s) to.
-
         Returns:
-            None. The output_obj is modified in place.
+            Dictionary of filenames and file data. E.g. {"c0": b"filedata"}
 
         """
         # Collect wavefunction file from the calc_dir
         raise AdapterInputError(
             self.program,
             f"Adapter for {self.program} does not support wavefunction collection.",
         )
```

### Comparing `qcop-0.5.3/qcop/adapters/file.py` & `qcop-0.5.4/qcop/adapters/file.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/qcop/adapters/geometric.py` & `qcop-0.5.4/qcop/adapters/geometric.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/qcop/adapters/qcengine.py` & `qcop-0.5.4/qcop/adapters/qcengine.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/qcop/adapters/terachem.py` & `qcop-0.5.4/qcop/adapters/terachem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
-from typing import Callable, Optional, Tuple
+from typing import Callable, Dict, Optional, Tuple, Union
 
+import qcparse
 from qcio import CalcType, ProgramInput, SinglePointOutput, SinglePointResults
-from qcparse import encode, parse_results
 from qcparse.encoders.terachem import XYZ_FILENAME
 from qcparse.parsers.terachem import parse_version_string
 
-from qcop.exceptions import AdapterInputError
+from qcop.exceptions import AdapterError, AdapterInputError
 
 from .base import ProgramAdapter
 from .utils import execute_subprocess
 
 
 class TeraChemAdapter(ProgramAdapter):
     """Adapter for TeraChem."""
@@ -50,48 +50,44 @@
             update_interval: The minimum time in seconds between calls to the
                 update_func.
 
         Returns:
             A tuple of SinglePointComputedProps and the stdout str.
         """
         input_filename = "tc.in"
-        native_input = encode(inp_obj, self.program)
+        try:
+            native_input = qcparse.encode(inp_obj, self.program)
+        except qcparse.exceptions.EncoderError as e:
+            raise AdapterInputError(self.program, str(e))
         Path(input_filename).write_text(native_input.input_file)
         Path(native_input.geometry_filename).write_text(native_input.geometry_file)
 
         stdout = execute_subprocess(
             self.program, [input_filename], update_func, update_interval
         )
-        parsed_output = parse_results(stdout, self.program, "stdout")
+        parsed_output = qcparse.parse_results(stdout, self.program, "stdout")
         return parsed_output, stdout
 
-    def collect_wfn(self, output: SinglePointOutput) -> None:
-        """Append wavefunction data to the output.
-
-        Args:
-            output: SinglePointOutput object on which to append wavefunction data.
-
-        Returns:
-            None. Modifies the output object in place.
-        """
+    def collect_wfn(self) -> Dict[str, Union[str, bytes]]:
+        """Append wavefunction data to the output."""
 
         # Naming conventions from TeraChem uses xyz filename as scratch dir postfix
         scr_postfix = XYZ_FILENAME.split(".")[0]
 
         # Wavefunction filenames
         wfn_filenames = ("c0", "ca0", "cb0")
         wfn_paths = [Path(f"scr.{scr_postfix}/{fn}") for fn in wfn_filenames]
         if not any(wfn_path.exists() for wfn_path in wfn_paths):
-            raise AdapterInputError(
-                program=self.program,
-                message=f"No wavefunction files found in {Path.cwd()}",
-            )
+            raise AdapterError(f"No wavefunction files found in {Path.cwd()}")
+
+        wfns: Dict[str, Union[str, bytes]] = {}
         for wfn_path in wfn_paths:
             if wfn_path.exists():
-                output.files[str(wfn_path)] = wfn_path.read_bytes()
+                wfns[str(wfn_path)] = wfn_path.read_bytes()
+        return wfns
 
     def propagate_wfn(self, output: SinglePointOutput, prog_inp: ProgramInput) -> None:
         """Propagate the wavefunction from the previous calculation.
 
         Args:
             output: The output from a previous calculation containing wavefunction data.
             prog_inp: The ProgramInput object on which to place the wavefunction data.
```

### Comparing `qcop-0.5.3/qcop/adapters/utils.py` & `qcop-0.5.4/qcop/adapters/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,17 @@
     """Context manager for a temporary directory.
 
     Args:
         directory: Where to create the temporary directory. If None, a new directory is
             created in the system default temporary directory.
         rmdir: Whether to remove the temporary directory when the context manager exits.
     """
+    cwd = Path.cwd()  # Save current working directory
     temp_dir = Path(directory or tempfile.mkdtemp())  # Set path to directory
     temp_dir.mkdir(parents=True, exist_ok=True)  # Create directory
-    cwd = Path.cwd()  # Save current working directory
-    os.chdir(temp_dir)  # Change to temporary directory
-    yield temp_dir  # Execute code in context manager
-    if rmdir:  # After exiting context manager
-        shutil.rmtree(temp_dir)
-    os.chdir(cwd)
+    try:
+        os.chdir(temp_dir)  # Change to temporary directory
+        yield temp_dir  # Execute code in context manager
+    finally:
+        if rmdir:  # After exiting context manager
+            shutil.rmtree(temp_dir)
+        os.chdir(cwd)
```

### Comparing `qcop-0.5.3/qcop/adapters/xtb.py` & `qcop-0.5.4/qcop/adapters/xtb.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class XTBAdapter(ProgramAdapter):
     """Adapter for xtb-python."""
 
     supported_calctypes = [CalcType.energy, CalcType.gradient]
     program = "xtb"
+    write_files = False  # xtb-python does not use files written to disk
 
     def __init__(self):
         super().__init__()
         # Check that xtb-python is installed.
         self.xtb = self._ensure_xtb()
 
     def validate_input(self, inp_obj: ProgramInput) -> None:
```

### Comparing `qcop-0.5.3/qcop/exceptions.py` & `qcop-0.5.4/qcop/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/qcop/main.py` & `qcop-0.5.4/qcop/main.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/qcop/utils.py` & `qcop-0.5.4/qcop/utils.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.3/PKG-INFO` & `qcop-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcop
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

