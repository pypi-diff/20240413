# Comparing `tmp/segmentation_skeleton_metrics-4.1.3.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.3.tar", last modified: Wed Apr 10 18:00:15 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.4.tar", last modified: Sat Apr 13 19:29:21 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.3.tar` & `segmentation_skeleton_metrics-4.1.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.671061 segmentation_skeleton_metrics-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.639061 segmentation_skeleton_metrics-4.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.643061 segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.643061 segmentation_skeleton_metrics-4.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-10 18:00:15.671061 segmentation_skeleton_metrics-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.643061 segmentation_skeleton_metrics-4.1.3/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.643061 segmentation_skeleton_metrics-4.1.3/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.643061 segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.655061 segmentation_skeleton_metrics-4.1.3/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.667061 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:00:15.671061 segmentation_skeleton_metrics-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.639061 segmentation_skeleton_metrics-4.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.667061 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 18:00:05.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/merge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.671061 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-10 18:00:15.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-10 18:00:15.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:00:15.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 18:00:15.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 18:00:15.000000 segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:00:15.671061 segmentation_skeleton_metrics-4.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 18:00:04.000000 segmentation_skeleton_metrics-4.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.013685 segmentation_skeleton_metrics-4.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.029685 segmentation_skeleton_metrics-4.1.4/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.041685 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.013685 segmentation_skeleton_metrics-4.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.041685 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 19:29:10.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-13 19:29:21.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.4/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.4/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/.gitignore` & `segmentation_skeleton_metrics-4.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/LICENSE` & `segmentation_skeleton_metrics-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/PKG-INFO` & `segmentation_skeleton_metrics-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.3
+Version: 4.1.4
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.3/README.md` & `segmentation_skeleton_metrics-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.4/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.4/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.4/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/pyproject.toml` & `segmentation_skeleton_metrics-4.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.4/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.4/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/merge_detection.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/merge_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     -------
     list
         List such that each entry is a line from the swc file.
 
     """
     contents = read_from_cloud(zip_file, path)
     if len(contents) > min_size:
-        swc_id = int(utils.get_swc_id(path))
+        swc_id = int(utils.get_id(path))
         return {swc_id: get_coords(contents, anisotropy)}
     else:
         return dict()
 
 
 def read_from_local(path):
     """
```

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.3
+Version: 4.1.4
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.3/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

