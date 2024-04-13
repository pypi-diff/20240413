# Comparing `tmp/zodipy-0.8.6.tar.gz` & `tmp/zodipy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodipy-0.8.6.tar", max compression
+gzip compressed data, was "zodipy-0.9.0.tar", max compression
```

## Comparing `zodipy-0.8.6.tar` & `zodipy-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35148 2022-05-27 12:19:51.135025 zodipy-0.8.6/LICENSE
--rw-r--r--   0        0        0     3517 2024-03-21 02:00:42.410729 zodipy-0.8.6/README.md
--rw-r--r--   0        0        0     2223 2024-03-21 01:21:42.453479 zodipy-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      276 2024-02-01 07:45:46.077609 zodipy-0.8.6/zodipy/__init__.py
--rw-r--r--   0        0        0     2826 2023-02-03 09:26:36.666633 zodipy-0.8.6/zodipy/_bandpass.py
--rw-r--r--   0        0        0      580 2023-02-07 12:46:42.398482 zodipy-0.8.6/zodipy/_constants.py
--rw-r--r--   0        0        0     1677 2023-02-03 09:26:36.669642 zodipy-0.8.6/zodipy/_contour.py
--rw-r--r--   0        0        0     2976 2024-02-27 10:49:30.300531 zodipy-0.8.6/zodipy/_emission.py
--rw-r--r--   0        0        0     4353 2023-11-06 14:02:48.589227 zodipy-0.8.6/zodipy/_interpolate_source.py
--rw-r--r--   0        0        0     4434 2023-02-07 12:46:42.402979 zodipy-0.8.6/zodipy/_ipd_comps.py
--rw-r--r--   0        0        0    15221 2023-11-06 14:03:13.055442 zodipy-0.8.6/zodipy/_ipd_dens_funcs.py
--rw-r--r--   0        0        0     2942 2023-11-06 14:03:30.573906 zodipy-0.8.6/zodipy/_ipd_model.py
--rw-r--r--   0        0        0     3248 2024-02-02 15:01:26.320632 zodipy-0.8.6/zodipy/_line_of_sight.py
--rw-r--r--   0        0        0     2297 2023-11-06 14:03:38.179596 zodipy-0.8.6/zodipy/_sky_coords.py
--rw-r--r--   0        0        0     2752 2023-11-06 13:50:29.556216 zodipy-0.8.6/zodipy/_source_funcs.py
--rw-r--r--   0        0        0      311 2023-02-03 09:26:36.686612 zodipy-0.8.6/zodipy/_types.py
--rw-r--r--   0        0        0      998 2023-02-03 09:26:36.688761 zodipy-0.8.6/zodipy/_unit_vectors.py
--rw-r--r--   0        0        0     3298 2024-02-27 23:23:29.332427 zodipy-0.8.6/zodipy/_validators.py
--rw-r--r--   0        0        0     4667 2023-09-15 08:50:24.694430 zodipy-0.8.6/zodipy/comps.py
--rw-r--r--   0        0        0     1997 2023-09-15 08:50:24.696767 zodipy-0.8.6/zodipy/model_registry.py
--rw-r--r--   0        0        0        0 2022-11-28 11:09:29.298004 zodipy-0.8.6/zodipy/py.typed
--rw-r--r--   0        0        0     6165 2023-09-15 08:50:24.701308 zodipy-0.8.6/zodipy/source_params.py
--rw-r--r--   0        0        0    24080 2024-03-21 01:14:53.123739 zodipy-0.8.6/zodipy/zodipy.py
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 zodipy-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-13 07:26:26.411863 zodipy-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5995 2024-04-13 09:11:02.454322 zodipy-0.9.0/README.md
+-rw-r--r--   0        0        0     2244 2024-04-13 08:16:49.155424 zodipy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-04-13 07:26:26.441718 zodipy-0.9.0/zodipy/__init__.py
+-rw-r--r--   0        0        0     2826 2024-04-13 07:26:26.441950 zodipy-0.9.0/zodipy/_bandpass.py
+-rw-r--r--   0        0        0      580 2024-04-13 07:26:26.442110 zodipy-0.9.0/zodipy/_constants.py
+-rw-r--r--   0        0        0     1677 2024-04-13 07:26:26.442325 zodipy-0.9.0/zodipy/_contour.py
+-rw-r--r--   0        0        0     2976 2024-04-13 07:26:26.442697 zodipy-0.9.0/zodipy/_emission.py
+-rw-r--r--   0        0        0     4353 2024-04-13 07:26:26.442914 zodipy-0.9.0/zodipy/_interpolate_source.py
+-rw-r--r--   0        0        0     4434 2024-04-13 07:26:26.443132 zodipy-0.9.0/zodipy/_ipd_comps.py
+-rw-r--r--   0        0        0    15213 2024-04-13 08:34:40.194963 zodipy-0.9.0/zodipy/_ipd_dens_funcs.py
+-rw-r--r--   0        0        0     2942 2024-04-13 07:26:26.443565 zodipy-0.9.0/zodipy/_ipd_model.py
+-rw-r--r--   0        0        0     3248 2024-04-13 07:26:26.443729 zodipy-0.9.0/zodipy/_line_of_sight.py
+-rw-r--r--   0        0        0     2297 2024-04-13 07:26:26.443909 zodipy-0.9.0/zodipy/_sky_coords.py
+-rw-r--r--   0        0        0     2752 2024-04-13 07:26:26.444084 zodipy-0.9.0/zodipy/_source_funcs.py
+-rw-r--r--   0        0        0      311 2024-04-13 07:26:26.444243 zodipy-0.9.0/zodipy/_types.py
+-rw-r--r--   0        0        0      998 2024-04-13 07:26:26.444431 zodipy-0.9.0/zodipy/_unit_vectors.py
+-rw-r--r--   0        0        0     3298 2024-04-13 07:26:26.444611 zodipy-0.9.0/zodipy/_validators.py
+-rw-r--r--   0        0        0     4667 2024-04-13 07:26:26.444779 zodipy-0.9.0/zodipy/comps.py
+-rw-r--r--   0        0        0     1997 2024-04-13 07:26:26.444939 zodipy-0.9.0/zodipy/model_registry.py
+-rw-r--r--   0        0        0        0 2024-04-13 07:26:26.445008 zodipy-0.9.0/zodipy/py.typed
+-rw-r--r--   0        0        0     6165 2024-04-13 07:26:26.445218 zodipy-0.9.0/zodipy/source_params.py
+-rw-r--r--   0        0        0    24080 2024-04-13 07:26:26.445448 zodipy-0.9.0/zodipy/zodipy.py
+-rw-r--r--   0        0        0     7061 1970-01-01 00:00:00.000000 zodipy-0.9.0/PKG-INFO
```

### Comparing `zodipy-0.8.6/LICENSE` & `zodipy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/pyproject.toml` & `zodipy-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "zodipy"
 homepage = "https://github.com/Cosmoglobe/zodipy"
-version = "0.8.6"
+version = "0.9.0"
 description = "Software for simulating zodiacal emission"
 authors = ["Metin San <metinisan@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 exclude = ["test.py"]
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -21,35 +21,36 @@
     "cosmology",
     "space",
     "science",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-numpy = "^1.22.3"
-healpy = "^1.15.0"
+python = ">=3.9"
+numpy = "^1.26.4"
+healpy = "^1.16.6"
 astropy = ">=5.0.1"
 jplephem = "^2.17"
+scipy = "^1.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0"
 mkdocs = "^1.5.3"
 pymdown-extensions = "^9.4"
 markdown-include = "^0.6.0"
 pre-commit = "^2.19.0"
-hypothesis = "^6.47.5"
 coverage = "^7.1.0"
 pytest-cov = "^4.0.0"
 mkdocs-material = "^9.0.1"
 mkdocstrings = "^0.23.0"
 mkdocstrings-python = "^1.7.3"
-ruff = "^0.1.4"
+ruff = "^0.3.7"
 markdown = "<3.4.0"
+hypothesis = "^6.99.11"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
@@ -65,15 +66,15 @@
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::UserWarning",
     "ignore:.*overflow encountered in expm1.*",
 ]
 
 [tool.ruff]
-select = [
+lint.select = [
     "F", 
     "D", 
     "F", 
     "E", 
     "W", 
     "C", 
     "B", 
@@ -96,21 +97,19 @@
     "SIM",
     "PLR",
     "PLW",
     "TRY",
     "RUF",
 ]
 line-length = 100
-ignore = [
+lint.ignore = [
     "B905",
     "D100",
     "D104",
     "D105",
     "D107",
     "ANN101",
     "PLR0913",
     "ISC001"
 ]
 exclude = ["tests/*", "docs/*"]
-
-[tool.ruff.pydocstyle]
-convention = "google"
+lint.pydocstyle.convention = "google"
```

### Comparing `zodipy-0.8.6/zodipy/_bandpass.py` & `zodipy-0.9.0/zodipy/_bandpass.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_constants.py` & `zodipy-0.9.0/zodipy/_constants.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_contour.py` & `zodipy-0.9.0/zodipy/_contour.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_emission.py` & `zodipy-0.9.0/zodipy/_emission.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_interpolate_source.py` & `zodipy-0.9.0/zodipy/_interpolate_source.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_ipd_comps.py` & `zodipy-0.9.0/zodipy/_ipd_comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_ipd_dens_funcs.py` & `zodipy-0.9.0/zodipy/_ipd_dens_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,16 +407,15 @@
     BroadBand: compute_broad_band_density,
     RingRRM: compute_ring_density_rmm,
     FeatureRRM: compute_feature_density_rmm,
 }
 
 
 class ComponentDensityFn(Protocol):
-    def __call__(self, X_helio: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
-        ...
+    def __call__(self, X_helio: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]: ...
 
 
 def construct_density_partials(
     comps: Sequence[Component],
     dynamic_params: dict[str, Any],
 ) -> tuple[ComponentDensityFn, ...]:
     """Return density partials for the components.
```

### Comparing `zodipy-0.8.6/zodipy/_ipd_model.py` & `zodipy-0.9.0/zodipy/_ipd_model.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_line_of_sight.py` & `zodipy-0.9.0/zodipy/_line_of_sight.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_sky_coords.py` & `zodipy-0.9.0/zodipy/_sky_coords.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_source_funcs.py` & `zodipy-0.9.0/zodipy/_source_funcs.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_unit_vectors.py` & `zodipy-0.9.0/zodipy/_unit_vectors.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/_validators.py` & `zodipy-0.9.0/zodipy/_validators.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/comps.py` & `zodipy-0.9.0/zodipy/comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/model_registry.py` & `zodipy-0.9.0/zodipy/model_registry.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/source_params.py` & `zodipy-0.9.0/zodipy/source_params.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.8.6/zodipy/zodipy.py` & `zodipy-0.9.0/zodipy/zodipy.py`

 * *Files identical despite different names*

