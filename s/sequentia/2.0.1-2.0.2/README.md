# Comparing `tmp/sequentia-2.0.1.tar.gz` & `tmp/sequentia-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentia-2.0.1.tar", max compression
+gzip compressed data, was "sequentia-2.0.2.tar", max compression
```

## Comparing `sequentia-2.0.1.tar` & `sequentia-2.0.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    23116 2024-04-02 09:24:35.135433 sequentia-2.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1096 2024-04-02 09:24:35.135433 sequentia-2.0.1/LICENSE
--rw-r--r--   0        0        0      473 2024-04-02 09:24:35.135433 sequentia-2.0.1/Makefile
--rw-r--r--   0        0        0    12403 2024-04-02 09:24:35.135433 sequentia-2.0.1/README.md
--rw-r--r--   0        0        0      326 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/__init__.py
--rw-r--r--   0        0        0      506 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/cov.py
--rw-r--r--   0        0        0      919 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/docs.py
--rw-r--r--   0        0        0     1056 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/lint.py
--rw-r--r--   0        0        0     1147 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/release.py
--rw-r--r--   0        0        0      758 2024-04-02 09:24:35.139433 sequentia-2.0.1/make/tests.py
--rw-r--r--   0        0        0     7547 2024-04-02 09:24:35.139433 sequentia-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      547 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/__init__.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/__init__.py
--rw-r--r--   0        0        0      663 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_data.py
--rw-r--r--   0        0        0      290 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_hmm/__init__.py
--rw-r--r--   0        0        0    11861 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_hmm/topologies.py
--rw-r--r--   0        0        0      539 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_multiprocessing.py
--rw-r--r--   0        0        0      434 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_typing.py
--rw-r--r--   0        0        0     6762 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/_internal/_validation.py
--rw-r--r--   0        0        0      594 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/datasets/__init__.py
--rw-r--r--   0        0        0    12315 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/datasets/base.py
--rw-r--r--   0        0        0      277 2024-04-02 09:24:35.139433 sequentia-2.0.1/sequentia/datasets/data/__init__.py
--rw-r--r--   0        0        0  2623137 2024-04-02 09:24:35.143433 sequentia-2.0.1/sequentia/datasets/data/digits.npz
--rw-r--r--   0        0        0  2106823 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/datasets/data/gene_families.npz
--rw-r--r--   0        0        0     1840 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/datasets/digits.py
--rw-r--r--   0        0        0     2574 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/datasets/gene_families.py
--rw-r--r--   0        0        0     2778 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/enums.py
--rw-r--r--   0        0        0      607 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/__init__.py
--rw-r--r--   0        0        0     6702 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/base.py
--rw-r--r--   0        0        0      508 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/__init__.py
--rw-r--r--   0        0        0    18497 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/classifier.py
--rw-r--r--   0        0        0      488 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/variants/__init__.py
--rw-r--r--   0        0        0    16915 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/variants/base.py
--rw-r--r--   0        0        0     6726 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/variants/categorical.py
--rw-r--r--   0        0        0     9787 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/hmm/variants/gaussian_mixture.py
--rw-r--r--   0        0        0      488 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/knn/__init__.py
--rw-r--r--   0        0        0    10632 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/knn/base.py
--rw-r--r--   0        0        0    13886 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/knn/classifier.py
--rw-r--r--   0        0        0     7172 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/models/knn/regressor.py
--rw-r--r--   0        0        0      475 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/preprocessing/__init__.py
--rw-r--r--   0        0        0    13569 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/preprocessing/transforms.py
--rw-r--r--   0        0        0     2965 2024-04-02 09:24:35.155434 sequentia-2.0.1/sequentia/version.py
--rw-r--r--   0        0        0     1878 2024-04-02 09:24:35.155434 sequentia-2.0.1/tasks.py
--rw-r--r--   0        0        0      260 2024-04-02 09:24:35.155434 sequentia-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-02 09:24:35.155434 sequentia-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.155434 sequentia-2.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.155434 sequentia-2.0.1/tests/unit/test_datasets/__init__.py
--rw-r--r--   0        0        0     6696 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_datasets/test_base.py
--rw-r--r--   0        0        0      729 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_datasets/test_digits.py
--rw-r--r--   0        0        0      855 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_datasets/test_gene_families.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_internal/__init__.py
--rw-r--r--   0        0        0      297 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_internal/test_data.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_internal/test_hmm/__init__.py
--rw-r--r--   0        0        0    16110 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_internal/test_hmm/test_topologies.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/__init__.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/hmm/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/hmm/test_classifier.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/hmm/variants/__init__.py
--rw-r--r--   0        0        0     7368 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/hmm/variants/test_categorical.py
--rw-r--r--   0        0        0     9601 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/hmm/variants/test_gaussian_mixture.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/knn/__init__.py
--rw-r--r--   0        0        0     9012 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/knn/test_classifier.py
--rw-r--r--   0        0        0     6020 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_models/knn/test_regressor.py
--rw-r--r--   0        0        0     8146 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_pipeline.py
--rw-r--r--   0        0        0      241 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_preprocessing/__init__.py
--rw-r--r--   0        0        0     3129 2024-04-02 09:24:35.159433 sequentia-2.0.1/tests/unit/test_preprocessing/test_transforms.py
--rw-r--r--   0        0        0      445 2024-04-02 09:24:35.159433 sequentia-2.0.1/tox.ini
--rw-r--r--   0        0        0    14369 1970-01-01 00:00:00.000000 sequentia-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    23317 2024-04-13 17:46:39.479964 sequentia-2.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1096 2024-04-13 17:46:39.479964 sequentia-2.0.2/LICENSE
+-rw-r--r--   0        0        0      473 2024-04-13 17:46:39.479964 sequentia-2.0.2/Makefile
+-rw-r--r--   0        0        0    12403 2024-04-13 17:46:39.479964 sequentia-2.0.2/README.md
+-rw-r--r--   0        0        0      326 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/cov.py
+-rw-r--r--   0        0        0      919 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/docs.py
+-rw-r--r--   0        0        0     1056 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/lint.py
+-rw-r--r--   0        0        0     1147 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/release.py
+-rw-r--r--   0        0        0      758 2024-04-13 17:46:39.483964 sequentia-2.0.2/make/tests.py
+-rw-r--r--   0        0        0     7547 2024-04-13 17:46:39.483964 sequentia-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      547 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_data.py
+-rw-r--r--   0        0        0      290 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_hmm/__init__.py
+-rw-r--r--   0        0        0    11861 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_hmm/topologies.py
+-rw-r--r--   0        0        0      539 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_multiprocessing.py
+-rw-r--r--   0        0        0      434 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_typing.py
+-rw-r--r--   0        0        0     6762 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/_internal/_validation.py
+-rw-r--r--   0        0        0      594 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/datasets/__init__.py
+-rw-r--r--   0        0        0    12315 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/datasets/base.py
+-rw-r--r--   0        0        0      277 2024-04-13 17:46:39.483964 sequentia-2.0.2/sequentia/datasets/data/__init__.py
+-rw-r--r--   0        0        0  2623137 2024-04-13 17:46:39.487964 sequentia-2.0.2/sequentia/datasets/data/digits.npz
+-rw-r--r--   0        0        0  2106823 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/datasets/data/gene_families.npz
+-rw-r--r--   0        0        0     1840 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/datasets/digits.py
+-rw-r--r--   0        0        0     2574 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/datasets/gene_families.py
+-rw-r--r--   0        0        0     2778 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/enums.py
+-rw-r--r--   0        0        0      607 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/__init__.py
+-rw-r--r--   0        0        0     6702 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/base.py
+-rw-r--r--   0        0        0      508 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/__init__.py
+-rw-r--r--   0        0        0    18497 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/classifier.py
+-rw-r--r--   0        0        0      488 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/variants/__init__.py
+-rw-r--r--   0        0        0    16915 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/variants/base.py
+-rw-r--r--   0        0        0     6726 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/variants/categorical.py
+-rw-r--r--   0        0        0     9787 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/hmm/variants/gaussian_mixture.py
+-rw-r--r--   0        0        0      488 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/knn/__init__.py
+-rw-r--r--   0        0        0    10634 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/knn/base.py
+-rw-r--r--   0        0        0    13886 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/knn/classifier.py
+-rw-r--r--   0        0        0     7172 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/models/knn/regressor.py
+-rw-r--r--   0        0        0      475 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/preprocessing/__init__.py
+-rw-r--r--   0        0        0    13569 2024-04-13 17:46:39.499964 sequentia-2.0.2/sequentia/preprocessing/transforms.py
+-rw-r--r--   0        0        0     2965 2024-04-13 17:46:39.503964 sequentia-2.0.2/sequentia/version.py
+-rw-r--r--   0        0        0     1878 2024-04-13 17:46:39.503964 sequentia-2.0.2/tasks.py
+-rw-r--r--   0        0        0      260 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_datasets/__init__.py
+-rw-r--r--   0        0        0     6696 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_datasets/test_base.py
+-rw-r--r--   0        0        0      729 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_datasets/test_digits.py
+-rw-r--r--   0        0        0      855 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_datasets/test_gene_families.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_internal/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_internal/test_data.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_internal/test_hmm/__init__.py
+-rw-r--r--   0        0        0    16110 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_internal/test_hmm/test_topologies.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/hmm/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/hmm/test_classifier.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/hmm/variants/__init__.py
+-rw-r--r--   0        0        0     7368 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/hmm/variants/test_categorical.py
+-rw-r--r--   0        0        0     9601 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/hmm/variants/test_gaussian_mixture.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/knn/__init__.py
+-rw-r--r--   0        0        0     9326 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/knn/test_classifier.py
+-rw-r--r--   0        0        0     6020 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_models/knn/test_regressor.py
+-rw-r--r--   0        0        0     8146 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_pipeline.py
+-rw-r--r--   0        0        0      241 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_preprocessing/__init__.py
+-rw-r--r--   0        0        0     3129 2024-04-13 17:46:39.503964 sequentia-2.0.2/tests/unit/test_preprocessing/test_transforms.py
+-rw-r--r--   0        0        0      445 2024-04-13 17:46:39.503964 sequentia-2.0.2/tox.ini
+-rw-r--r--   0        0        0    14369 1970-01-01 00:00:00.000000 sequentia-2.0.2/PKG-INFO
```

### Comparing `sequentia-2.0.1/CHANGELOG.md` & `sequentia-2.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,20 @@
 
 #### Major changes
 
 Nothing, initial release!
 
 </details>
 
+## [v2.0.2](https://github.com/eonu/sequentia/releases/tag/v2.0.2) - 2024-04-13
+
+### Bug Fixes
+
+- call `KNNMixin._dtw1d` when `independent=True` ([#251](https://github.com/eonu/sequentia/issues/251))
+
 ## [v2.0.1](https://github.com/eonu/sequentia/releases/tag/v2.0.1) - 2024-04-02
 
 ### Bug Fixes
 
 - use log probs for `KNNClassifier.predict_log_proba` ([#247](https://github.com/eonu/sequentia/issues/247))
 
 ## [v2.0.0](https://github.com/eonu/sequentia/releases/tag/v2.0.0) - 2024-04-01
```

### Comparing `sequentia-2.0.1/LICENSE` & `sequentia-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/README.md` & `sequentia-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/make/docs.py` & `sequentia-2.0.2/make/docs.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/make/lint.py` & `sequentia-2.0.2/make/lint.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/make/release.py` & `sequentia-2.0.2/make/release.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/make/tests.py` & `sequentia-2.0.2/make/tests.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/pyproject.toml` & `sequentia-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequentia"
-version = "2.0.1"
+version = "2.0.2"
 license = "MIT"
 authors = ["Edwin Onuonga <ed@eonu.net>"]
 maintainers = ["Edwin Onuonga <ed@eonu.net>"]
 description = "Scikit-Learn compatible HMM and DTW based sequence machine learning algorithms in Python."
 readme = "README.md"
 homepage = "https://github.com/eonu/sequentia"
 repository = "https://github.com/eonu/sequentia"
```

### Comparing `sequentia-2.0.1/sequentia/__init__.py` & `sequentia-2.0.2/sequentia/__init__.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/_internal/_data.py` & `sequentia-2.0.2/sequentia/_internal/_data.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/_internal/_hmm/topologies.py` & `sequentia-2.0.2/sequentia/_internal/_hmm/topologies.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/_internal/_multiprocessing.py` & `sequentia-2.0.2/sequentia/_internal/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/_internal/_validation.py` & `sequentia-2.0.2/sequentia/_internal/_validation.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/__init__.py` & `sequentia-2.0.2/sequentia/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/base.py` & `sequentia-2.0.2/sequentia/datasets/base.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/data/digits.npz` & `sequentia-2.0.2/sequentia/datasets/data/digits.npz`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/data/gene_families.npz` & `sequentia-2.0.2/sequentia/datasets/data/gene_families.npz`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/digits.py` & `sequentia-2.0.2/sequentia/datasets/digits.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/datasets/gene_families.py` & `sequentia-2.0.2/sequentia/datasets/gene_families.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/enums.py` & `sequentia-2.0.2/sequentia/enums.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/__init__.py` & `sequentia-2.0.2/sequentia/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/base.py` & `sequentia-2.0.2/sequentia/models/base.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/hmm/classifier.py` & `sequentia-2.0.2/sequentia/models/hmm/classifier.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/hmm/variants/base.py` & `sequentia-2.0.2/sequentia/models/hmm/variants/base.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/hmm/variants/categorical.py` & `sequentia-2.0.2/sequentia/models/hmm/variants/categorical.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/hmm/variants/gaussian_mixture.py` & `sequentia-2.0.2/sequentia/models/hmm/variants/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/knn/base.py` & `sequentia-2.0.2/sequentia/models/knn/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         per-feature DTW distances, allowing each feature to be warped
         independently.
         """
         window = self._window(A, B)
 
         def dtw(a: FloatArray, b: FloatArray) -> float:
             """Windowed DTW wrapper function."""
-            return self._dtw(a, b, window=window)
+            return self._dtw1d(a, b, window=window)
 
         return np.sum([dtw(A[:, i], B[:, i]) for i in range(A.shape[1])])
 
     def _dtwd(self: KNNMixin, A: FloatArray, B: FloatArray) -> float:
         """Compute the multivariate DTW distance so that the warping of the
         features depends on each other, by modifying the local distance
         measure.
```

### Comparing `sequentia-2.0.1/sequentia/models/knn/classifier.py` & `sequentia-2.0.2/sequentia/models/knn/classifier.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/models/knn/regressor.py` & `sequentia-2.0.2/sequentia/models/knn/regressor.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/preprocessing/transforms.py` & `sequentia-2.0.2/sequentia/preprocessing/transforms.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/sequentia/version.py` & `sequentia-2.0.2/sequentia/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
     FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
     DEALINGS IN THE SOFTWARE.
 """
 
 __all__ = ["VERSION", "version_info"]
 
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 
 
 def version_info() -> str:
     """Return complete version information for Sequentia and its
     dependencies.
     """
     import importlib.metadata
```

### Comparing `sequentia-2.0.1/tasks.py` & `sequentia-2.0.2/tasks.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/conftest.py` & `sequentia-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_datasets/test_base.py` & `sequentia-2.0.2/tests/unit/test_datasets/test_base.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_datasets/test_digits.py` & `sequentia-2.0.2/tests/unit/test_datasets/test_digits.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_datasets/test_gene_families.py` & `sequentia-2.0.2/tests/unit/test_datasets/test_gene_families.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_internal/test_hmm/test_topologies.py` & `sequentia-2.0.2/tests/unit/test_internal/test_hmm/test_topologies.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_models/hmm/test_classifier.py` & `sequentia-2.0.2/tests/unit/test_models/hmm/test_classifier.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_models/hmm/variants/test_categorical.py` & `sequentia-2.0.2/tests/unit/test_models/hmm/variants/test_categorical.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_models/hmm/variants/test_gaussian_mixture.py` & `sequentia-2.0.2/tests/unit/test_models/hmm/variants/test_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_models/knn/test_classifier.py` & `sequentia-2.0.2/tests/unit/test_models/knn/test_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,40 @@
     Helpers.assert_equal(clf.X_, data.X)
     Helpers.assert_equal(clf.y_, data.y)
     Helpers.assert_equal(clf.lengths_, data.lengths)
 
 
 @pytest.mark.parametrize("k", [1, 2, 5])
 @pytest.mark.parametrize("weighting", [None, lambda x: np.exp(-x)])
+@pytest.mark.parametrize("independent", [False, True])
 def test_classifier_e2e(
     helpers: t.Any,
     request: SubRequest,
-    k: int,
-    weighting: t.Callable | None,
     dataset: SequentialDataset,
     random_state: np.random.RandomState,
+    *,
+    k: int,
+    weighting: t.Callable | None,
+    independent: bool,
 ) -> None:
-    clf = KNNClassifier(k=k, weighting=weighting, random_state=random_state)
+    clf = KNNClassifier(
+        k=k,
+        weighting=weighting,
+        independent=independent,
+        random_state=random_state,
+    )
 
     assert clf.k == k
     assert clf.weighting == weighting
+    assert clf.independent == independent
+
+    if independent:
+        assert clf._dtw().__name__ == "_dtwi"
+    else:
+        assert clf._dtw().__name__ == "_dtwd"
 
     data = dataset.copy()
     data._X = data._X[:, :1]  # only use one feature
     subset, _ = data.split(
         test_size=0.98, random_state=random_state, stratify=True
     )
     train, test = subset.split(
```

### Comparing `sequentia-2.0.1/tests/unit/test_models/knn/test_regressor.py` & `sequentia-2.0.2/tests/unit/test_models/knn/test_regressor.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_pipeline.py` & `sequentia-2.0.2/tests/unit/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/tests/unit/test_preprocessing/test_transforms.py` & `sequentia-2.0.2/tests/unit/test_preprocessing/test_transforms.py`

 * *Files identical despite different names*

### Comparing `sequentia-2.0.1/PKG-INFO` & `sequentia-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentia
-Version: 2.0.1
+Version: 2.0.2
 Summary: Scikit-Learn compatible HMM and DTW based sequence machine learning algorithms in Python.
 Home-page: https://github.com/eonu/sequentia
 License: MIT
 Keywords: python,machine-learning,time-series,hmm,hidden-markov-models,dtw,dynamic-time-warping,knn,k-nearest-neighbors,sequence-classification,time-series-classification,multivariate-time-series,variable-length,classification-algorithms
 Author: Edwin Onuonga
 Author-email: ed@eonu.net
 Maintainer: Edwin Onuonga
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sequentia Version: 2.0.1 Summary: Scikit-Learn
+Metadata-Version: 2.1 Name: sequentia Version: 2.0.2 Summary: Scikit-Learn
 compatible HMM and DTW based sequence machine learning algorithms in Python.
 Home-page: https://github.com/eonu/sequentia License: MIT Keywords:
 python,machine-learning,time-series,hmm,hidden-markov-models,dtw,dynamic-time-
 warping,knn,k-nearest-neighbors,sequence-classification,time-series-
 classification,multivariate-time-series,variable-length,classification-
 algorithms Author: Edwin Onuonga Author-email: ed@eonu.net Maintainer: Edwin
 Onuonga Maintainer-email: ed@eonu.net Requires-Python: >=3.11,<4.0 Classifier:
```

