# Comparing `tmp/clfutils4r-0.0.3.tar.gz` & `tmp/clfutils4r-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clfutils4r-0.0.3.tar", last modified: Mon Jul 24 04:56:10 2023, max compression
+gzip compressed data, was "clfutils4r-1.0.0.tar", last modified: Sat Apr 13 05:59:46 2024, max compression
```

## Comparing `clfutils4r-0.0.3.tar` & `clfutils4r-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-0.0.3/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6114 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5470 2023-07-24 04:53:33.000000 clfutils4r-0.0.3/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2023-07-24 04:54:12.000000 clfutils4r-0.0.3/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-0.0.3/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.966357 clfutils4r-0.0.3/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/src/clfutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-0.0.3/src/clfutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    19989 2023-07-24 04:53:38.000000 clfutils4r-0.0.3/src/clfutils4r/eval_classification.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/src/clfutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6114 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      295 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       50 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-1.0.0/LICENSE
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     6798 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6154 2024-04-13 05:58:30.000000 clfutils4r-1.0.0/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2024-04-13 05:59:39.000000 clfutils4r-1.0.0/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-1.0.0/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/clfutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-1.0.0/src/clfutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    27602 2024-04-13 05:53:50.000000 clfutils4r-1.0.0/src/clfutils4r/eval_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    13221 2024-04-13 03:17:53.000000 clfutils4r-1.0.0/src/clfutils4r/gridsearch_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    10883 2024-04-13 04:18:23.000000 clfutils4r-1.0.0/src/clfutils4r/pretty_cm.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/clfutils4r.egg-info/
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     6798 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      330 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/top_level.txt
```

### Comparing `clfutils4r-0.0.3/LICENSE` & `clfutils4r-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clfutils4r-0.0.3/PKG-INFO` & `clfutils4r-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-Metadata-Version: 2.1
-Name: clfutils4r
-Version: 0.0.3
-Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
-Home-page: https://github.com/rutujagurav/clfutils4r
-Author: Rutuja Gurav
-Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
-Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
-Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Classification Utilities
 
-This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. The only function available is `eval_classification()`. 
+This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. 
+There are two modules available - `gridsearch_classification` and `eval_classification`.
+
+## Installation
+
+`pip install clfutils4r`
+
+## Module `gridsearch_classification`:
+Only function available is `gridsearch_classification()`
+
+### Available Parameters
+
+`X`: dataset.
+
+`gt_labels`: ground truth labels.
+
+`best_model_metric`: metric to use to choose the best model.
+
+**For plotting**
+
+`show`: whether to display the plots; this is used in a notebook.
+
+`save`: whether to save the plots.
+
+`save_dir`: if `save=True`, directory to save results in.
+                                                        
+
+## Module `eval_classification`: 
+Only function available is `eval_classification()`
 
 Metrics plotted - 
 1. Confusion Matrix
 2. Class-wise PR curve
 3. Class-wise ROC curve
 
 Additional metrics plotted if binary classification - 
 1. KS Statistic Plot
 2. Lift Curve
 3. Cumulative Gain Plot
 4. Cross-validated PR curve
 5. Cross-validated ROC curve
 
-
-## Installation
-
-`pip install clfutils4r`
-
-## Available Parameters
-
+### Available Parameters
 **For cross-validation on full dataset**
 
 `untrained_model`: classifier object (untrained); this is used for cross-validation
 
 `X`: Pandas DataFrame containing preprocessed, normalized, complete dataset
 
 `y`: Pandas Series containing encoded labels for `X`
@@ -71,91 +77,90 @@
 
 `save`: set `True` if you want to save all results in RESULTS_DIR; defaults to `False`
 
 `show`: display all results; useful in notebooks; defaults to `False`
 
 ## Example Usage
 ```python
+
+import collections
 import matplotlib.pyplot as plt
+%matplotlib inline
 import numpy as np
 import pandas as pd
 import os
 
 from sklearn import datasets
 from sklearn.preprocessing import StandardScaler
 scaler = StandardScaler()
 
 ## Load dataset: Example - breast cancer prediction
 data = datasets.load_breast_cancer()
-class_names = data.target_names
-feature_names = data.feature_names
-X = pd.DataFrame(data.data, columns=feature_names)
-y = pd.Series(data.target)
-for feat_name in feature_names:
-    X[feat_name] = scaler.fit_transform(X[[feat_name]]) 
+class_names = [str(x) for x in data.target_names]
+feature_names = [str(x) for x in data.feature_names]
+
+X, y = data.data, data.target
+X = scaler.fit_transform(X)
 
 ## Split into train and test sets
 from sklearn.model_selection import train_test_split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30, random_state=42)
 
-## Setup model
-from sklearn.tree import DecisionTreeClassifier
-model = DecisionTreeClassifier()
-model_params = {'criterion': 'gini', 'max_depth': 3, 'min_samples_leaf': 5}
-model.set_params(**model_params)
-
-## Train model
-model.fit(X_train, y_train)
-
-## Evaluate model
-from clfutils4r.eval_classification import eval_classification
-y_pred = model.predict(X_test)
-y_pred_proba = model.predict_proba(X_test)
-
-eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
-                    n_splits=5, class_names=class_names, 
-                    X=X, y=y, 
-                    make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
-                    y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
-                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
-                    show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
+## Grid search for best model
+from gridsearch_classification import gridsearch_classification
+save_dir = "gridsearch_results"
+os.makedirs(save_dir, exist_ok=True)
+best_model, grid_search_results = gridsearch_classification(X=X_train,                    # dataset
+                                                            gt_labels=y_train,            # ground truth labels
+                                                            best_model_metric="F1",       # metric to use to choose the best model
+                                                            show=True,                    # whether to display the plots; this is used in a notebook
+                                                            save=True, save_dir=save_dir  # whether to save the plots
+                                                        )
+
+## Predict on test set
+y_pred = best_model.predict(X_test)
+y_pred_proba = best_model.predict_proba(X_test)
+
+## Evaluate best model on test set
+from eval_classification import eval_classification
+## Make metrics plots
+eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
+                    class_names=class_names, feature_names=feature_names,
+                    titlestr="Breast Cancer Detection",
+                    show=True, save=True, 
+                    RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
+<!-- ### Grid Search -->
+![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
+
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/test_results/confusion_matrix.png)
 <!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/test_results/classwise_roc_curve.png)
 <!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/test_results/classwise_pr_curve.png)
 <!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/test_results/ks_stat.png)
 <!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/test_results/lift_curve.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-![lift](tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/test_results/cumul_gain.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
-<!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
-
-<!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
-
 <!-- ### Shapley Analysis Summary Plot -->
-![shap](tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
-This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.3/README.md` & `clfutils4r-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,68 @@
+Metadata-Version: 2.1
+Name: clfutils4r
+Version: 1.0.0
+Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
+Home-page: https://github.com/rutujagurav/clfutils4r
+Author: Rutuja Gurav
+Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
+Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
+Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Classification Utilities
 
-This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. The only function available is `eval_classification()`. 
+This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. 
+There are two modules available - `gridsearch_classification` and `eval_classification`.
+
+## Installation
+
+`pip install clfutils4r`
+
+## Module `gridsearch_classification`:
+Only function available is `gridsearch_classification()`
+
+### Available Parameters
+
+`X`: dataset.
+
+`gt_labels`: ground truth labels.
+
+`best_model_metric`: metric to use to choose the best model.
+
+**For plotting**
+
+`show`: whether to display the plots; this is used in a notebook.
+
+`save`: whether to save the plots.
+
+`save_dir`: if `save=True`, directory to save results in.
+                                                        
+
+## Module `eval_classification`: 
+Only function available is `eval_classification()`
 
 Metrics plotted - 
 1. Confusion Matrix
 2. Class-wise PR curve
 3. Class-wise ROC curve
 
 Additional metrics plotted if binary classification - 
 1. KS Statistic Plot
 2. Lift Curve
 3. Cumulative Gain Plot
 4. Cross-validated PR curve
 5. Cross-validated ROC curve
 
-
-## Installation
-
-`pip install clfutils4r`
-
-## Available Parameters
-
+### Available Parameters
 **For cross-validation on full dataset**
 
 `untrained_model`: classifier object (untrained); this is used for cross-validation
 
 `X`: Pandas DataFrame containing preprocessed, normalized, complete dataset
 
 `y`: Pandas Series containing encoded labels for `X`
@@ -55,91 +93,90 @@
 
 `save`: set `True` if you want to save all results in RESULTS_DIR; defaults to `False`
 
 `show`: display all results; useful in notebooks; defaults to `False`
 
 ## Example Usage
 ```python
+
+import collections
 import matplotlib.pyplot as plt
+%matplotlib inline
 import numpy as np
 import pandas as pd
 import os
 
 from sklearn import datasets
 from sklearn.preprocessing import StandardScaler
 scaler = StandardScaler()
 
 ## Load dataset: Example - breast cancer prediction
 data = datasets.load_breast_cancer()
-class_names = data.target_names
-feature_names = data.feature_names
-X = pd.DataFrame(data.data, columns=feature_names)
-y = pd.Series(data.target)
-for feat_name in feature_names:
-    X[feat_name] = scaler.fit_transform(X[[feat_name]]) 
+class_names = [str(x) for x in data.target_names]
+feature_names = [str(x) for x in data.feature_names]
+
+X, y = data.data, data.target
+X = scaler.fit_transform(X)
 
 ## Split into train and test sets
 from sklearn.model_selection import train_test_split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30, random_state=42)
 
-## Setup model
-from sklearn.tree import DecisionTreeClassifier
-model = DecisionTreeClassifier()
-model_params = {'criterion': 'gini', 'max_depth': 3, 'min_samples_leaf': 5}
-model.set_params(**model_params)
-
-## Train model
-model.fit(X_train, y_train)
-
-## Evaluate model
-from clfutils4r.eval_classification import eval_classification
-y_pred = model.predict(X_test)
-y_pred_proba = model.predict_proba(X_test)
-
-eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
-                    n_splits=5, class_names=class_names, 
-                    X=X, y=y, 
-                    make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
-                    y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
-                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
-                    show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
+## Grid search for best model
+from gridsearch_classification import gridsearch_classification
+save_dir = "gridsearch_results"
+os.makedirs(save_dir, exist_ok=True)
+best_model, grid_search_results = gridsearch_classification(X=X_train,                    # dataset
+                                                            gt_labels=y_train,            # ground truth labels
+                                                            best_model_metric="F1",       # metric to use to choose the best model
+                                                            show=True,                    # whether to display the plots; this is used in a notebook
+                                                            save=True, save_dir=save_dir  # whether to save the plots
+                                                        )
+
+## Predict on test set
+y_pred = best_model.predict(X_test)
+y_pred_proba = best_model.predict_proba(X_test)
+
+## Evaluate best model on test set
+from eval_classification import eval_classification
+## Make metrics plots
+eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
+                    class_names=class_names, feature_names=feature_names,
+                    titlestr="Breast Cancer Detection",
+                    show=True, save=True, 
+                    RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
+<!-- ### Grid Search -->
+![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
+
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/test_results/confusion_matrix.png)
 <!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/test_results/classwise_roc_curve.png)
 <!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/test_results/classwise_pr_curve.png)
 <!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/test_results/ks_stat.png)
 <!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/test_results/lift_curve.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-![lift](tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/test_results/cumul_gain.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
-<!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
-
-<!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
-
 <!-- ### Shapley Analysis Summary Plot -->
-![shap](tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
-This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.3/pyproject.toml` & `clfutils4r-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clfutils4r"
-version = "0.0.3"
+version = "1.0.0"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `clfutils4r-0.0.3/setup.py` & `clfutils4r-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-0.0.3/src/clfutils4r/eval_classification.py` & `clfutils4r-1.0.0/src/clfutils4r/eval_classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import matplotlib.pyplot as plt
 plt.rcParams['font.family'] = 'serif'
 plt.rcParams['font.serif'] = ['Times New Roman'] + plt.rcParams['font.serif']
 plt.rcParams['axes.facecolor'] = plt.rcParams['savefig.facecolor'] = 'white'
+plt.rcParams['axes.labelsize'] = \
+    plt.rcParams['axes.titlesize'] = \
+    plt.rcParams['xtick.labelsize'] = \
+    plt.rcParams['ytick.labelsize'] = \
+    'xx-large'
+
 # from mpl_toolkits.axes_grid1 import make_axes_locatable
 import seaborn as sns
 # sns.set()
 import pandas as pd
 import numpy as np
-import os
-
+import os, textwrap
 from deprecation import deprecated
 
-import scikitplot
+import sklearn
+print(f"sklearn version: {sklearn.__version__}")
 from sklearn.inspection import permutation_importance
-from sklearn.model_selection import KFold, train_test_split, RandomizedSearchCV, StratifiedKFold, cross_val_score
-from sklearn.metrics import confusion_matrix, accuracy_score, auc, average_precision_score, precision_score, recall_score, confusion_matrix, classification_report, roc_curve, precision_recall_curve, f1_score, roc_auc_score
+from sklearn.model_selection import StratifiedKFold
+from sklearn.metrics import accuracy_score, average_precision_score, precision_score, recall_score, f1_score, roc_auc_score
+from sklearn.metrics import confusion_matrix, auc, classification_report, roc_curve, precision_recall_curve
 from sklearn.manifold import TSNE
 
+import scikitplot
+print(f"scikitplot version: {scikitplot.__version__}")
+import pretty_cm # type: ignore
+
 import shap
 
 dpi=300
 
 @deprecated
 def print_metrics(y_test=None, y_pred=None, threshold = 0.5):
     print("Precision", precision_score(y_test, y_pred > threshold))
@@ -75,167 +86,224 @@
     
     if(save):
         plt.savefig(RESULTS_DIR+'/roc_curve.png', bbox_inches='tight',dpi=dpi)
     if(show):
         plt.show()
     plt.close()
 
-def plot_confusion_matrix(y_test=None, y_pred=None, labels=[], threshold = 0.5, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
+def plot_confusion_matrix(y_test=None, y_pred=None, labels=[], threshold = 0.5, RESULTS_DIR='', titlestr='', pretty=True, show=False, save=False, dpi=300):
     """
     Returns a matplotlib figure containing the plotted confusion matrix.
     
     Args:
        y_test: ground-truth labels
        y_pred: predicted labels
        labels: class_names since y_test, y_pred are encoded.
     """
-    ## Create confusion matrix using scikit-plot
-    # fig, ax = plt.subplots()
-    # ax = scikitplot.metrics.plot_confusion_matrix(y_test,y_pred, ax=ax)
-    # if(len(labels) != 0):
-    #     ax.set_xticklabels(labels)
-    #     ax.set_yticklabels(labels)
-    #     # Rotate the tick labels and set their alignment.
-    #     plt.setp(ax.get_xticklabels(), rotation=0, ha="right", rotation_mode="anchor")
-    #     plt.setp(ax.get_yticklabels(), rotation=90, ha="right", rotation_mode="anchor")
-    
-    ## Create confusion matrix using sklearn
-    cm = confusion_matrix(y_test, y_pred)
-    # Normalize the confusion matrix.
-    cm = np.around(cm.astype('float') / cm.sum(axis=1)[:, np.newaxis], decimals=2)
-    # print(cm.shape)
+    num_classes = len(set(y_test))
+    if num_classes <= 3: figsize=(5,5)
+    else: figsize=(num_classes, num_classes)
+
+    if not pretty:
+        ## Create confusion matrix using scikit-plot
+        fig, ax = plt.subplots()
+        ax = scikitplot.metrics.plot_confusion_matrix(y_test, y_pred, 
+                                                    normalize=True, 
+                                                    text_fontsize='x-large', 
+                                                    title_fontsize='xx-large',
+                                                    ax=ax)
+        if(len(labels) != 0):
+            ax.set_xticks(ax.get_xticks())
+            ax.set_xticklabels(labels, rotation=0, ha="center", rotation_mode="anchor")
+            ax.set_yticks(ax.get_yticks())
+            ax.set_yticklabels(labels, rotation=90, ha="center", rotation_mode="anchor")
+    else:
+        cm = confusion_matrix(y_test, y_pred)
+        pretty_cm.plot_from_confusion_matrix(cm, columns=labels, 
+                                                fz='x-large', 
+                                                figsize=figsize
+                                            )
+    # ## Create confusion matrix using sklearn
+    # cm = confusion_matrix(y_test, y_pred)
+    # # Normalize the confusion matrix.
+    # cm = np.around(cm.astype('float') / cm.sum(axis=1)[:, np.newaxis], decimals=2)
+    # # print(cm.shape)
 
     # vals = [["{}\n(True Positives)".format(str(cm[0,0])), "{}\n(False Positives)".format(str(cm[0,1]))],
     #         ["{}\n(False Negatives)".format(str(cm[1,0])), "{}\n(True Negatives)".format(str(cm[0,1]))]
     #     ]
     # print(vals)
     
-    fig, ax = plt.subplots()
-    s = sns.heatmap(cm, vmin=0, vmax=1, center=0.5, 
-                    xticklabels = labels, yticklabels = labels,
-                    cmap=plt.cm.Blues, cbar=False, 
-                    ax=ax, square=True, 
-                    annot=True) # , annot_kws={"fontsize":10}
+    # fig, ax = plt.subplots()
+    # s = sns.heatmap(cm, vmin=0, vmax=1, center=0.5, 
+    #                 xticklabels = labels, yticklabels = labels,
+    #                 cmap=plt.cm.Blues, cbar=False, 
+    #                 ax=ax, square=True, 
+    #                 annot=True) # , annot_kws={"fontsize":10}
+    # s.set_ylabel('True Label')
+    # s.set_xlabel('Predicted Label')
 
     # plt.imshow(cm, interpolation='nearest', cmap=plt.cm.Blues)
     # plt.title("Confusion matrix")
     # plt.colorbar()
     # tick_marks = np.arange(len(class_names))+0.5
     # ax.set_xticks(tick_marks, class_names, rotation=90)
     # ax.set_yticks(tick_marks, class_names)
-    
     ### Use white text if squares are dark; otherwise black.
     # threshold = cm.max() / 2.0
     # for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
     #     color = "white" if cm[i, j] > threshold else "black"
     #     ax.set_text(j, i, cm[i, j], horizontalalignment="center", color=color)
     # ax.set_ylabel('True Label', fontsize=15)
     # ax.set_xlabel('Predicted Label', fontsize=15)
+        
+    # plt.title(titlestr+"Confusion Matrix")
+
 
-    s.set_ylabel('True Label') #, fontsize=15
-    s.set_xlabel('Predicted Label')
-    
-    plt.title(titlestr+"Confusion Matrix")
     plt.tight_layout()
-    
     if save:
         plt.savefig(RESULTS_DIR+'/confusion_matrix.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
         
-def plot_ks_stat(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
-    fig, ax = plt.subplots()
-    ax = scikitplot.metrics.plot_ks_statistic(y_test, y_pred, ax=ax)
+def plot_ks_stat(y_test=None, y_pred=None, titlestr='', classes_titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
+    if len(classes_titlestr) > 50: classes_titlestr = '\n'.join(textwrap.wrap(classes_titlestr, 50))
+
+    fig, ax = plt.subplots(figsize=(10,5))
+    ax = scikitplot.metrics.plot_ks_statistic(y_test, y_pred, 
+                                            text_fontsize='xx-large', 
+                                            title_fontsize='xx-large',
+                                            ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title(titlestr+"KS Statistic Plot ")
+    plt.title(titlestr+"KS Statistic Plot")
     plt.grid()
-    plt.legend(loc='best')
+    legend = plt.legend(bbox_to_anchor=(1, 0.5), loc='center left', title=classes_titlestr, fontsize='large')
+    legend.get_title().set_fontsize('large')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/ks_stat.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
-def plot_lift_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
-    fig, ax = plt.subplots()
-    ax = scikitplot.metrics.plot_lift_curve(y_test, y_pred, ax=ax)
+def plot_lift_curve(y_test=None, y_pred=None, titlestr='', classes_titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
+    if len(classes_titlestr) > 50: classes_titlestr = '\n'.join(textwrap.wrap(classes_titlestr, 50))
+
+    fig, ax = plt.subplots(figsize=(10,5))
+    ax = scikitplot.metrics.plot_lift_curve(y_test, y_pred, 
+                                            text_fontsize='xx-large', 
+                                            title_fontsize='xx-large',
+                                            ax=ax)
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title(titlestr+"Lift Curve ")
+    plt.title(titlestr+"Lift Curve", 
+            #   fontsize=axes_label_fontsize
+            )
     # plt.grid()
-    plt.legend(loc='best')
+    legend = plt.legend(bbox_to_anchor=(1, 0.5), loc='center left', title=classes_titlestr, fontsize='large')
+    legend.get_title().set_fontsize('large')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/lift_curve.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
-def plot_cumul_gain(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
-    fig, ax = plt.subplots()
-    ax = scikitplot.metrics.plot_cumulative_gain(y_test, y_pred, ax=ax)
+def plot_cumul_gain(y_test=None, y_pred=None, titlestr='', classes_titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
+    if len(classes_titlestr) > 50: classes_titlestr = '\n'.join(textwrap.wrap(classes_titlestr, 50))
+
+    fig, ax = plt.subplots(figsize=(10,5))
+    ax = scikitplot.metrics.plot_cumulative_gain(y_test, y_pred, 
+                                                text_fontsize='xx-large', 
+                                                title_fontsize='xx-large',
+                                                ax=ax)
+    ax.set_xlim([-0.05, 1.05])
+    ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title(titlestr+"Cumulative Gains Curve ")
+    plt.title(titlestr+"Cumulative Gains Curve")
     # plt.grid()
-    plt.legend(loc='best')
+    legend = plt.legend(bbox_to_anchor=(1, 0.5), loc='center left', title=classes_titlestr, fontsize='large')
+    legend.get_title().set_fontsize('large')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/cumul_gain.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
-def plot_classwise_pr_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
-    fig, ax = plt.subplots()
-    ax = scikitplot.metrics.plot_precision_recall(y_test, y_pred, ax=ax)
+def plot_classwise_pr_curve(y_test=None, y_pred=None, titlestr='', classes_titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
+    if len(classes_titlestr) > 50: classes_titlestr = '\n'.join(textwrap.wrap(classes_titlestr, 50))
+    
+    fig, ax = plt.subplots(figsize=(10,5))
+    ax = scikitplot.metrics.plot_precision_recall(y_test, y_pred, 
+                                                # text_fontsize='xx-large', 
+                                                title_fontsize='xx-large',
+                                                ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title(titlestr+"Precision-Recall Curve ")
+    ax.set_xticklabels(ax.get_xticks().round(1), fontsize='x-large')
+    ax.set_yticklabels(ax.get_yticks().round(1), fontsize='x-large')
+    ax.set_xlabel(ax.get_xlabel(), fontsize='xx-large')
+    ax.set_ylabel(ax.get_ylabel(), fontsize='xx-large')
+    plt.title(titlestr+"Precision-Recall Curve")
     plt.grid()
+    legend = plt.legend(bbox_to_anchor=(1, 0.5), loc='center left', title=classes_titlestr, fontsize='large')
+    legend.get_title().set_fontsize('large')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_pr_curve.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
-def plot_classwise_roc_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
-    fig, ax = plt.subplots()
-    ax = scikitplot.metrics.plot_roc(y_test, y_pred, ax=ax)
+def plot_classwise_roc_curve(y_test=None, y_pred=None, titlestr='', classes_titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
+    if len(classes_titlestr) > 50: classes_titlestr = '\n'.join(textwrap.wrap(classes_titlestr, 50))
+
+    fig, ax = plt.subplots(figsize=(10,5))
+    ax = scikitplot.metrics.plot_roc(y_test, y_pred, 
+                                    # text_fontsize='xx-large', 
+                                    title_fontsize='xx-large',
+                                    ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
+    ax.set_xticklabels(ax.get_xticks().round(1), fontsize='x-large')
+    ax.set_yticklabels(ax.get_yticks().round(1), fontsize='x-large')
+    ax.set_xlabel(ax.get_xlabel(), fontsize='xx-large')
+    ax.set_ylabel(ax.get_ylabel(), fontsize='xx-large')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title(titlestr+"ROC Curves ")
+    plt.title(titlestr+"ROC Curves")
     plt.grid()
+    legend = plt.legend(bbox_to_anchor=(1, 0.5), loc='center left', title=classes_titlestr, fontsize='large')
+    legend.get_title().set_fontsize('large')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_roc_curve.png', bbox_inches='tight', dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
+
 def generate_classification_report(y_test=None, y_pred=None, labels=[], RESULTS_DIR='', show=False, save=False):
     if(len(labels) !=0):
         report = classification_report(y_test, 
                                         y_pred, 
                                         target_names=[cl+'(class '+str(i)+')' for i, cl in enumerate(labels)], 
                                         output_dict=True)
     else:
@@ -249,16 +317,16 @@
 
 def plot_cv_roc_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Draw a Cross Validated ROC Curve.
     Keyword Args:
         classifier: Classifier Object
         cv: StratifiedKFold Object: (https://stats.stackexchange.com/questions/49540/understanding-stratified-cross-validation)
-        X: Feature Pandas DataFrame
-        y: Response Pandas Series
+        X: Features Pandas DataFrame
+        y: Target Pandas Series
     Example largely taken from http://scikit-learn.org/stable/auto_examples/model_selection/plot_roc_crossval.html#sphx-glr-auto-examples-model-selection-plot-roc-crossval-py
     """
     # Creating ROC Curve with Cross Validation
     tprs = []
     aucs = []
     mean_fpr = np.linspace(0, 1, 100)
     cv = StratifiedKFold(n_splits=n_splits)
@@ -357,144 +425,205 @@
     
     if save:
         plt.savefig(RESULTS_DIR+'/crossvalidation_pr_curve.png', bbox_inches='tight',dpi=dpi)   
     if show:
         plt.show()
     plt.close()
 
-def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, titlestr='', show=False, save=False, RESULTS_DIR=None):
+def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, feature_names=None, titlestr='', show=False, save=False, RESULTS_DIR=None, dpi=300):
     print("No. of samples used to build explainer and generate shap values: ", nsamples)
     explainer = shap.KernelExplainer(model.predict, shap.sample(X_train, nsamples))
     shap_values = explainer.shap_values(X=X_test, nsamples=nsamples)
-    shap.summary_plot(shap_values=shap_values, features=X_test, show=False)
+    shap.summary_plot(shap_values=shap_values, features=X_test, feature_names=feature_names, show=False)
     # shap.plots.violin(shap_values=shap_values, features=X_test, plot_type="layered_violin", show=False)
     plt.title(titlestr+'Shapley Analysis')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
     if show:
         plt.show()
 
     plt.close()
+
+def plot_calibration_curve(classifiers_list=[], 
+                           classifiers_names=[],
+                           X_train=None, X_test=None, y_train=None, y_test=None,
+                           titlestr='', RESULTS_DIR='', show=False, save=False, 
+                           dpi=300):
+    print("Generating Calibration Curves...")
+    probas_list = []
+    for classifier, name in zip(classifiers_list, classifiers_names):
+        print("\tTraining classifier: ", name)
+        probas_list.append(classifier.fit(X_train, y_train).predict_proba(X_test))
+
+    fig, ax = plt.subplots(figsize=(10, 7))
+    ax = scikitplot.metrics.plot_calibration_curve(y_test, probas_list, 
+                                                    classifiers_names, 
+                                                    text_fontsize='xx-large', 
+                                                    ax=ax)
+    ax.set_xlim([-0.05, 1.05])
+    ax.set_ylim([-0.05, 1.05])
+    ax.set_facecolor('white')
+    for l in ax.lines:
+        l.set_lw(2)
+    plt.title(titlestr+"Calibration Curve")
+    plt.grid()
+    plt.legend(bbox_to_anchor=(1, 1))
+    plt.tight_layout()
     
-def eval_classification(untrained_model=None, n_splits=10,
-                        X=None, y=None, 
-                        make_shap_plot=False, trained_model=None, X_train=None, X_test=None, 
-                        y_train=None, y_test=None, y_pred=None, y_pred_proba=None, 
-                        class_names=None,
+    if save:
+        plt.savefig(RESULTS_DIR+'/calibration_curve.png', bbox_inches='tight',dpi=dpi)
+    if show:
+        plt.show()
+    plt.close()
+
+def eval_classification(make_metrics_plots=True, y_pred=None, y_pred_proba=None, 
+                        untrained_model=None, n_splits=10, X=None, y=None, 
+                        make_calibration_curves=False, untrained_models_list=[], untrained_models_names=[],
+                        make_shap_plot=False, trained_model=None, shap_nsamples=50,
+                        X_train=None, X_test=None, y_train=None, y_test=None,
+                        class_names=None, feature_names=None,
                         titlestr="",
                         save=False, RESULTS_DIR=None,
                         show=False, dpi=300):
 
     classes_titlestr = ', '.join(["class {}: {}".format(i, cls_nm) for i, cls_nm in enumerate(class_names)])
     if titlestr != "":
-        titlestr_cls = titlestr+"\n("+classes_titlestr+")\n\n"
-        titlestr_nocls = titlestr+"\n\n"
+        # titlestr_cls = titlestr+"\n("+classes_titlestr+")\n\n"
+        # titlestr_nocls = titlestr+"\n\n"
+        titlestr_cls = titlestr_nocls = titlestr+"\n"
     else:
-        titlestr_cls = "("+classes_titlestr+")\n\n"
-        titlestr_nocls = titlestr
+        # titlestr_cls = "("+classes_titlestr+")\n\n"
+        # titlestr_nocls = titlestr
+        titlestr_cls = titlestr_nocls = ""
 
     if save:
         if RESULTS_DIR is not None:
             if not os.path.exists(RESULTS_DIR):
                 os.makedirs(RESULTS_DIR)
             print("Saving results in {}".format(RESULTS_DIR))   
         else:
             print("Hey! You asked me to save results but did not provide a RESULTS_DIR !!!")
 
-    if y_test is not None and y_pred is not None:
-        assert len(y_test) == len(y_pred), "[Length Mismatch]: Number of test samples not equal to number of predictions"
-        generate_classification_report(y_test=y_test, 
-                                        y_pred=y_pred, 
-                                        RESULTS_DIR=RESULTS_DIR, 
-                                        labels=class_names,
-                                        show=show, 
-                                        save=save)
+    if make_metrics_plots:
+        if y_test is not None and y_pred is not None:
+            assert len(y_test) == len(y_pred), "[Length Mismatch]: Number of test samples not equal to number of predictions"
+            generate_classification_report(y_test=y_test, 
+                                            y_pred=y_pred, 
+                                            RESULTS_DIR=RESULTS_DIR, 
+                                            labels=class_names,
+                                            show=show, 
+                                            save=save)
 
-        plot_confusion_matrix(y_test=y_test, 
+            plot_confusion_matrix(y_test=y_test, 
                                 y_pred=y_pred, 
                                 RESULTS_DIR=RESULTS_DIR, 
                                 labels=class_names,
                                 titlestr=titlestr_nocls,
                                 dpi=dpi,
                                 show=show,  
                                 save=save)
 
-    if y_test is not None and y_pred_proba is not None:
-        assert len(y_test) == len(y_pred_proba), "[Length Mismatch]: Number of test samples not equal to number of predictions"
-        
-        if len(list(set(y_test))) == 2:
-            plot_ks_stat(y_test=y_test,
-                            y_pred=y_pred_proba, 
-                            RESULTS_DIR=RESULTS_DIR, 
-                            titlestr=titlestr_cls,
-                            dpi=dpi,
-                            show=show, 
-                            save=save)
+        if y_test is not None and y_pred_proba is not None:
+            assert len(y_test) == len(y_pred_proba), "[Length Mismatch]: Number of test samples not equal to number of predictions"
             
-            plot_lift_curve(y_test=y_test,
-                                y_pred=y_pred_proba, 
-                                RESULTS_DIR=RESULTS_DIR, 
-                                titlestr=titlestr_cls,
-                                dpi=dpi,
-                                show=show, 
-                                save=save)
-
-            plot_cumul_gain(y_test=y_test,
+            if len(list(set(y_test))) == 2:
+                plot_ks_stat(y_test=y_test,
                                 y_pred=y_pred_proba, 
                                 RESULTS_DIR=RESULTS_DIR, 
                                 titlestr=titlestr_cls,
+                                classes_titlestr = classes_titlestr,
                                 dpi=dpi,
                                 show=show, 
                                 save=save)
-        else:
-            print("Skipping KS, Lift and Cumulative Gain plots as number of classes is not 2")
-        
-        plot_classwise_pr_curve(y_test=y_test,
+                
+                plot_lift_curve(y_test=y_test,
                                     y_pred=y_pred_proba, 
                                     RESULTS_DIR=RESULTS_DIR, 
                                     titlestr=titlestr_cls,
+                                    classes_titlestr = classes_titlestr,
                                     dpi=dpi,
                                     show=show, 
                                     save=save)
-        
-        plot_classwise_roc_curve(y_test=y_test,
+
+                plot_cumul_gain(y_test=y_test,
                                     y_pred=y_pred_proba, 
                                     RESULTS_DIR=RESULTS_DIR, 
                                     titlestr=titlestr_cls,
+                                    classes_titlestr = classes_titlestr,
                                     dpi=dpi,
                                     show=show, 
                                     save=save)
-
-    if untrained_model is not None and X is not None and y is not None:
-        assert len(X) == len(y), "[Length Mismatch]: Number of samples not equal to number of class labels"    
-        if len(list(set(y_test))) == 2:
-            plot_cv_roc_curve(classifier=untrained_model, 
-                                X=X, 
-                                y=pd.Series(y), 
-                                n_splits=n_splits,
-                                RESULTS_DIR=RESULTS_DIR, 
-                                titlestr=titlestr_nocls, 
-                                dpi=dpi,
-                                show=show, 
-                                save=save)
+            else:
+                print("Skipping KS, Lift and Cumulative Gain plots as number of classes is not 2")
             
-            plot_cv_pr_curve(classifier=untrained_model,  
-                                X=X, 
-                                y=pd.Series(y), 
-                                n_splits=n_splits,
-                                RESULTS_DIR=RESULTS_DIR, 
-                                titlestr=titlestr_nocls,
-                                dpi=dpi,
-                                show=show, 
-                                save=save)
-        else:
-            print("Skipping Cross Validated ROC and PR curves as number of classes is not 2")
+            plot_classwise_pr_curve(y_test=y_test,
+                                        y_pred=y_pred_proba, 
+                                        RESULTS_DIR=RESULTS_DIR, 
+                                        titlestr=titlestr_cls,
+                                        classes_titlestr = classes_titlestr,
+                                        dpi=dpi,
+                                        show=show, 
+                                        save=save)
+            
+            plot_classwise_roc_curve(y_test=y_test,
+                                        y_pred=y_pred_proba, 
+                                        RESULTS_DIR=RESULTS_DIR, 
+                                        titlestr=titlestr_cls,
+                                        classes_titlestr = classes_titlestr,
+                                        dpi=dpi,
+                                        show=show, 
+                                        save=save)
+
+        if untrained_model is not None and X is not None and y is not None:
+            assert len(X) == len(y), "[Length Mismatch]: Number of samples not equal to number of class labels"    
+            if len(list(set(y_test))) == 2:
+                
+                plot_cv_roc_curve(classifier=untrained_model, 
+                                            X=X, 
+                                            y=y, 
+                                            n_splits=n_splits,
+                                            RESULTS_DIR=RESULTS_DIR, 
+                                            titlestr=titlestr_nocls, 
+                                            dpi=dpi,
+                                            show=show, 
+                                            save=save)
+                
+                plot_cv_pr_curve(classifier=untrained_model,  
+                                    X=X, 
+                                    y=y, 
+                                    n_splits=n_splits,
+                                    RESULTS_DIR=RESULTS_DIR, 
+                                    titlestr=titlestr_nocls,
+                                    dpi=dpi,
+                                    show=show, 
+                                    save=save)
+            else:
+                print("Skipping Cross Validated ROC and PR curves as number of classes is not 2")
     
     if make_shap_plot:
         if X_train is not None and X_test is not None and trained_model is not None:
             plot_shap_summary(model=trained_model, X_train=X_train, X_test=X_test,
+                                nsamples=shap_nsamples, feature_names=feature_names,
                                 titlestr=titlestr_nocls, show=show, RESULTS_DIR=RESULTS_DIR, save=save)
         else:
             print("Hey! You asked me to make a shap plot but did not provide a trained model, X_train and X_test !!!")
+    
+    if make_calibration_curves:
+        if len(list(set(y_test))) == 2:
+            if untrained_models_list is not None and \
+                untrained_models_names is not None and \
+                    X_train is not None and y_train is not None and \
+                        X_test is not None and y_train is not None:
+                assert len(untrained_models_list) == len(untrained_models_names), "[Length Mismatch]: Number of models not equal to number of model names"
+                assert len(X_train) == len(y_train), "[Length Mismatch]: Number of samples not equal to number of class labels"
+                assert len(X_test) == len(y_test), "[Length Mismatch]: Number of samples not equal to number of class labels"
+
+                plot_calibration_curve(classifiers_list=untrained_models_list,
+                                        classifiers_names=untrained_models_names,
+                                        X_train=X_train, X_test=X_test, y_train=y_train, y_test=y_test,
+                                        titlestr=titlestr_nocls, RESULTS_DIR=RESULTS_DIR, show=show, save=save, dpi=dpi)
+            else:
+                print("Skipping Calibration Curves as number of classes is not >=2 ")
+
```

### Comparing `clfutils4r-0.0.3/src/clfutils4r.egg-info/PKG-INFO` & `clfutils4r-1.0.0/src/clfutils4r.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 0.0.3
+Version: 1.0.0
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -12,35 +12,57 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Classification Utilities
 
-This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. The only function available is `eval_classification()`. 
+This packages provides a simple convenience wrapper around some basic sklearn and scikit-plot utilities for classification. 
+There are two modules available - `gridsearch_classification` and `eval_classification`.
+
+## Installation
+
+`pip install clfutils4r`
+
+## Module `gridsearch_classification`:
+Only function available is `gridsearch_classification()`
+
+### Available Parameters
+
+`X`: dataset.
+
+`gt_labels`: ground truth labels.
+
+`best_model_metric`: metric to use to choose the best model.
+
+**For plotting**
+
+`show`: whether to display the plots; this is used in a notebook.
+
+`save`: whether to save the plots.
+
+`save_dir`: if `save=True`, directory to save results in.
+                                                        
+
+## Module `eval_classification`: 
+Only function available is `eval_classification()`
 
 Metrics plotted - 
 1. Confusion Matrix
 2. Class-wise PR curve
 3. Class-wise ROC curve
 
 Additional metrics plotted if binary classification - 
 1. KS Statistic Plot
 2. Lift Curve
 3. Cumulative Gain Plot
 4. Cross-validated PR curve
 5. Cross-validated ROC curve
 
-
-## Installation
-
-`pip install clfutils4r`
-
-## Available Parameters
-
+### Available Parameters
 **For cross-validation on full dataset**
 
 `untrained_model`: classifier object (untrained); this is used for cross-validation
 
 `X`: Pandas DataFrame containing preprocessed, normalized, complete dataset
 
 `y`: Pandas Series containing encoded labels for `X`
@@ -71,91 +93,90 @@
 
 `save`: set `True` if you want to save all results in RESULTS_DIR; defaults to `False`
 
 `show`: display all results; useful in notebooks; defaults to `False`
 
 ## Example Usage
 ```python
+
+import collections
 import matplotlib.pyplot as plt
+%matplotlib inline
 import numpy as np
 import pandas as pd
 import os
 
 from sklearn import datasets
 from sklearn.preprocessing import StandardScaler
 scaler = StandardScaler()
 
 ## Load dataset: Example - breast cancer prediction
 data = datasets.load_breast_cancer()
-class_names = data.target_names
-feature_names = data.feature_names
-X = pd.DataFrame(data.data, columns=feature_names)
-y = pd.Series(data.target)
-for feat_name in feature_names:
-    X[feat_name] = scaler.fit_transform(X[[feat_name]]) 
+class_names = [str(x) for x in data.target_names]
+feature_names = [str(x) for x in data.feature_names]
+
+X, y = data.data, data.target
+X = scaler.fit_transform(X)
 
 ## Split into train and test sets
 from sklearn.model_selection import train_test_split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30, random_state=42)
 
-## Setup model
-from sklearn.tree import DecisionTreeClassifier
-model = DecisionTreeClassifier()
-model_params = {'criterion': 'gini', 'max_depth': 3, 'min_samples_leaf': 5}
-model.set_params(**model_params)
-
-## Train model
-model.fit(X_train, y_train)
-
-## Evaluate model
-from clfutils4r.eval_classification import eval_classification
-y_pred = model.predict(X_test)
-y_pred_proba = model.predict_proba(X_test)
-
-eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
-                    n_splits=5, class_names=class_names, 
-                    X=X, y=y, 
-                    make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
-                    y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
-                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
-                    show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
+## Grid search for best model
+from gridsearch_classification import gridsearch_classification
+save_dir = "gridsearch_results"
+os.makedirs(save_dir, exist_ok=True)
+best_model, grid_search_results = gridsearch_classification(X=X_train,                    # dataset
+                                                            gt_labels=y_train,            # ground truth labels
+                                                            best_model_metric="F1",       # metric to use to choose the best model
+                                                            show=True,                    # whether to display the plots; this is used in a notebook
+                                                            save=True, save_dir=save_dir  # whether to save the plots
+                                                        )
+
+## Predict on test set
+y_pred = best_model.predict(X_test)
+y_pred_proba = best_model.predict_proba(X_test)
+
+## Evaluate best model on test set
+from eval_classification import eval_classification
+## Make metrics plots
+eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
+                    class_names=class_names, feature_names=feature_names,
+                    titlestr="Breast Cancer Detection",
+                    show=True, save=True, 
+                    RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
+<!-- ### Grid Search -->
+![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
+
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/test_results/confusion_matrix.png)
 <!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/test_results/classwise_roc_curve.png)
 <!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/test_results/classwise_pr_curve.png)
 <!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/test_results/ks_stat.png)
 <!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/test_results/lift_curve.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-![lift](tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/test_results/cumul_gain.png)
 <!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
-<!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
-
-<!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
-
 <!-- ### Shapley Analysis Summary Plot -->
-![shap](tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

