# Comparing `tmp/nn_wrapper-1.0.0.tar.gz` & `tmp/nn_wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_wrapper-1.0.0.tar", max compression
+gzip compressed data, was "nn_wrapper-1.0.1.tar", max compression
```

## Comparing `nn_wrapper-1.0.0.tar` & `nn_wrapper-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.0/LICENSE
--rw-r--r--   0        0        0       43 2024-04-13 19:55:50.828702 nn_wrapper-1.0.0/nn-wrapper/__init__.py
--rw-r--r--   0        0        0    33351 2024-04-13 19:57:25.924521 nn_wrapper-1.0.0/nn-wrapper/NetworkWrapper.py
--rw-r--r--   0        0        0      833 2024-04-13 20:54:14.252452 nn_wrapper-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10248 2024-04-13 20:22:08.364735 nn_wrapper-1.0.0/README.md
--rw-r--r--   0        0        0    10765 1970-01-01 00:00:00.000000 nn_wrapper-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.1/LICENSE
+-rw-r--r--   0        0        0       43 2024-04-13 19:55:50.828702 nn_wrapper-1.0.1/NetworkWrapper/__init__.py
+-rw-r--r--   0        0        0    33351 2024-04-13 19:57:25.924521 nn_wrapper-1.0.1/NetworkWrapper/NetworkWrapper.py
+-rw-r--r--   0        0        0      837 2024-04-13 21:37:53.914985 nn_wrapper-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10252 2024-04-13 21:37:21.523136 nn_wrapper-1.0.1/README.md
+-rw-r--r--   0        0        0    10769 1970-01-01 00:00:00.000000 nn_wrapper-1.0.1/PKG-INFO
```

### Comparing `nn_wrapper-1.0.0/LICENSE` & `nn_wrapper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.0/nn-wrapper/NetworkWrapper.py` & `nn_wrapper-1.0.1/NetworkWrapper/NetworkWrapper.py`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.0/pyproject.toml` & `nn_wrapper-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "nn-wrapper"
-version = "1.0.0"
+version = "1.0.1"
 description = "A wrapper class for neural networks that makes working with them easier."
 authors = ["JohnConnor123 <ivan.eudokimoff2014@gmail.com>"]
 readme = "README.md"
-packages = [{include = "nn-wrapper"}]
+packages = [{include = "NetworkWrapper"}]
 
 # poetry config pypi-token.testpypi <API-token>
 #[[tool.poetry.source]]
 #name = "torch-cuda"
 #url = "https://download.pytorch.org/whl/cu118/"
 #priority = "supplemental"
```

### Comparing `nn_wrapper-1.0.0/README.md` & `nn_wrapper-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 By default, without first command the library will install the non-CUDA version of torch.
 
 ### Importing
 P.s. Optional: we set the main parts of the path of paths in windows and colab, relative to which relative paths are specified.
 
 ```python
-from nn-wrapper import NetworkWrapper
+from NetworkWrapper import NetworkWrapper
 
 main_windows_path = "D:\\Python_Projects\\Jupyter\\DL MIPT Stepik\\"
 main_colab_path = r'/content/gdrive/MyDrive/Colab Notebooks/Deep Learning School/'
 NetworkWrapper.set_main_paths(main_windows_path, main_colab_path)
 ```
 
 ### Creating NetworkWrapper object
```

### Comparing `nn_wrapper-1.0.0/PKG-INFO` & `nn_wrapper-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper class for neural networks that makes working with them easier.
 Author: JohnConnor123
 Author-email: ivan.eudokimoff2014@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -54,15 +54,15 @@
 ```
 By default, without first command the library will install the non-CUDA version of torch.
 
 ### Importing
 P.s. Optional: we set the main parts of the path of paths in windows and colab, relative to which relative paths are specified.
 
 ```python
-from nn-wrapper import NetworkWrapper
+from NetworkWrapper import NetworkWrapper
 
 main_windows_path = "D:\\Python_Projects\\Jupyter\\DL MIPT Stepik\\"
 main_colab_path = r'/content/gdrive/MyDrive/Colab Notebooks/Deep Learning School/'
 NetworkWrapper.set_main_paths(main_windows_path, main_colab_path)
 ```
 
 ### Creating NetworkWrapper object
```

