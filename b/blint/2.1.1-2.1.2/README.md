# Comparing `tmp/blint-2.1.1.tar.gz` & `tmp/blint-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.1.tar", max compression
+gzip compressed data, was "blint-2.1.2.tar", max compression
```

## Comparing `blint-2.1.1.tar` & `blint-2.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-04-08 15:54:29.791994 blint-2.1.1/LICENSE
--rw-r--r--   0        0        0     6240 2024-04-08 15:54:29.791994 blint-2.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-08 15:54:29.791994 blint-2.1.1/blint/__init__.py
--rw-r--r--   0        0        0    24122 2024-04-08 15:54:29.791994 blint-2.1.1/blint/analysis.py
--rw-r--r--   0        0        0    13955 2024-04-08 15:54:29.795994 blint-2.1.1/blint/android.py
--rw-r--r--   0        0        0    56201 2024-04-08 15:54:29.795994 blint-2.1.1/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-04-08 15:54:29.795994 blint-2.1.1/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-04-08 15:54:29.795994 blint-2.1.1/blint/cli.py
--rw-r--r--   0        0        0    20365 2024-04-08 15:54:29.795994 blint-2.1.1/blint/config.py
--rw-r--r--   0        0        0      324 2024-04-08 15:54:29.795994 blint-2.1.1/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-04-08 15:54:29.795994 blint-2.1.1/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-04-08 15:54:29.795994 blint-2.1.1/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-04-08 15:54:29.795994 blint-2.1.1/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-04-08 15:54:29.795994 blint-2.1.1/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-04-08 15:54:29.799994 blint-2.1.1/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-04-08 15:54:29.799994 blint-2.1.1/blint/logger.py
--rw-r--r--   0        0        0    23279 2024-04-08 15:54:29.799994 blint-2.1.1/blint/sbom.py
--rw-r--r--   0        0        0    14323 2024-04-08 15:54:29.799994 blint-2.1.1/blint/utils.py
--rw-r--r--   0        0        0     1812 2024-04-08 15:54:29.799994 blint-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 blint-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-13 14:33:01.619021 blint-2.1.2/LICENSE
+-rw-r--r--   0        0        0     6240 2024-04-13 14:33:01.619021 blint-2.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/__init__.py
+-rw-r--r--   0        0        0    24122 2024-04-13 14:33:01.623021 blint-2.1.2/blint/analysis.py
+-rw-r--r--   0        0        0    13955 2024-04-13 14:33:01.623021 blint-2.1.2/blint/android.py
+-rw-r--r--   0        0        0    56201 2024-04-13 14:33:01.623021 blint-2.1.2/blint/binary.py
+-rw-r--r--   0        0        0     2794 2024-04-13 14:33:01.623021 blint-2.1.2/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cli.py
+-rw-r--r--   0        0        0    20365 2024-04-13 14:33:01.623021 blint-2.1.2/blint/config.py
+-rw-r--r--   0        0        0      324 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-04-13 14:33:01.627021 blint-2.1.2/blint/logger.py
+-rw-r--r--   0        0        0    23315 2024-04-13 14:33:01.627021 blint-2.1.2/blint/sbom.py
+-rw-r--r--   0        0        0    14323 2024-04-13 14:33:01.627021 blint-2.1.2/blint/utils.py
+-rw-r--r--   0        0        0     1812 2024-04-13 14:33:01.627021 blint-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 blint-2.1.2/PKG-INFO
```

### Comparing `blint-2.1.1/LICENSE` & `blint-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/README.md` & `blint-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/analysis.py` & `blint-2.1.2/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/android.py` & `blint-2.1.2/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/binary.py` & `blint-2.1.2/blint/binary.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/checks.py` & `blint-2.1.2/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/cli.py` & `blint-2.1.2/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/config.py` & `blint-2.1.2/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/cyclonedx/spdx.py` & `blint-2.1.2/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/cyclonedx/spec.py` & `blint-2.1.2/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.2/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.2/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_exe_go.yml` & `blint-2.1.2/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.2/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.2/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.2/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.2/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_monero_go.yml` & `blint-2.1.2/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_monero_rust` & `blint-2.1.2/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.2/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.2/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.2/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.2/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.2/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.2/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.2/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/data/rules.yml` & `blint-2.1.2/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/logger.py` & `blint-2.1.2/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/blint/sbom.py` & `blint-2.1.2/blint/sbom.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     Args:
         src_dirs (list): A list of source directories.
 
     Returns:
         Metadata: A Metadata object for SBOM generation.
     """
     metadata = Metadata()
-    metadata.timestamp = datetime.now()
+    metadata.timestamp = f'{datetime.now().isoformat(timespec="seconds")}Z'
     metadata.component = default_parent(src_dirs)
     metadata.tools = (
         Tools(
             components=[
                 Component(
                     type=Type.application,
                     author="OWASP Foundation",
```

### Comparing `blint-2.1.1/blint/utils.py` & `blint-2.1.2/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.1/pyproject.toml` & `blint-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.1"
+version = "2.1.2"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
```

### Comparing `blint-2.1.1/PKG-INFO` & `blint-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.1
+Version: 2.1.2
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
```

