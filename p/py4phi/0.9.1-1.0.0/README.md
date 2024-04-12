# Comparing `tmp/py4phi-0.9.1.tar.gz` & `tmp/py4phi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4phi-0.9.1.tar", last modified: Sun Apr  7 20:48:09 2024, max compression
+gzip compressed data, was "py4phi-1.0.0.tar", last modified: Fri Apr 12 23:06:10 2024, max compression
```

## Comparing `py4phi-0.9.1.tar` & `py4phi-1.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    11357 2024-04-07 09:44:34.000000 py4phi-0.9.1/LICENSE
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1873 2024-04-07 10:07:22.000000 py4phi-0.9.1/NOTICE
--rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21919 2024-04-07 20:48:09.236741 py4phi-0.9.1/PKG-INFO
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7409 2024-04-07 20:28:28.000000 py4phi-0.9.1/README.md
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.1/cli/__init__.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/analytics/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/analytics/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3764 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/analytics/feature_selection.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3725 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/analytics/principal_component_analysis.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      497 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/cli_main.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4512 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/descriptions.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/encryption/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.1/cli/encryption/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8938 2024-04-07 09:05:07.000000 py4phi-0.9.1/cli/encryption/encryption.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1807 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/encryption/model_encryption.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/utils.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/py4phi/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       78 2024-04-04 21:26:02.000000 py4phi-0.9.1/py4phi/__init__.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/_encryption/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 08:44:07.000000 py4phi-0.9.1/py4phi/_encryption/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4530 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3248 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_model_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1903 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/_encryption/_pandas_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2154 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_polars_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2385 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_pyspark_encryptor.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/analytics/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/analytics/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      386 2024-03-30 16:13:27.000000 py4phi-0.9.1/py4phi/analytics/base_analytics.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7134 2024-04-03 20:50:33.000000 py4phi-0.9.1/py4phi/analytics/feature_selection.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8868 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/analytics/principal_component_analysis.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4619 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/config_processor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      680 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/consts.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    16943 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/controller.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4470 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/core.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/dataset_handlers/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-04 14:14:53.000000 py4phi-0.9.1/py4phi/dataset_handlers/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     6097 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/dataset_handlers/base_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3117 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/pandas_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3084 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/polars_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4235 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/pyspark_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3636 2024-04-02 21:42:25.000000 py4phi-0.9.1/py4phi/dataset_handlers/pyspark_write_utils.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      553 2024-02-24 17:29:06.000000 py4phi-0.9.1/py4phi/log4j.properties
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      371 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/logger_setup.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      648 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/utils.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi.egg-info/
--rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21919 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/PKG-INFO
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1303 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/SOURCES.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        1 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/dependency_links.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       45 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/entry_points.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/requires.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       11 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/top_level.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1573 2024-04-07 20:47:52.000000 py4phi-0.9.1/pyproject.toml
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       38 2024-04-07 20:48:09.236741 py4phi-0.9.1/setup.cfg
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.358260 py4phi-1.0.0/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    11357 2024-04-07 09:44:34.000000 py4phi-1.0.0/LICENSE
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1873 2024-04-07 10:07:22.000000 py4phi-1.0.0/NOTICE
+-rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    24334 2024-04-12 23:06:10.358260 py4phi-1.0.0/PKG-INFO
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     9652 2024-04-11 20:55:33.000000 py4phi-1.0.0/README.md
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.350260 py4phi-1.0.0/cli/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-1.0.0/cli/__init__.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.354260 py4phi-1.0.0/cli/analytics/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-30 22:00:06.000000 py4phi-1.0.0/cli/analytics/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3764 2024-03-31 13:04:23.000000 py4phi-1.0.0/cli/analytics/feature_selection.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3725 2024-03-31 13:04:23.000000 py4phi-1.0.0/cli/analytics/principal_component_analysis.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      497 2024-03-31 13:04:23.000000 py4phi-1.0.0/cli/cli_main.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4512 2024-03-31 13:04:23.000000 py4phi-1.0.0/cli/descriptions.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.354260 py4phi-1.0.0/cli/encryption/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-1.0.0/cli/encryption/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8938 2024-04-07 09:05:07.000000 py4phi-1.0.0/cli/encryption/encryption.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1807 2024-03-30 22:00:06.000000 py4phi-1.0.0/cli/encryption/model_encryption.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-03-30 22:00:06.000000 py4phi-1.0.0/cli/utils.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.354260 py4phi-1.0.0/py4phi/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       78 2024-04-04 21:26:02.000000 py4phi-1.0.0/py4phi/__init__.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.354260 py4phi-1.0.0/py4phi/_encryption/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 08:44:07.000000 py4phi-1.0.0/py4phi/_encryption/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4632 2024-04-11 20:28:07.000000 py4phi-1.0.0/py4phi/_encryption/_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3248 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/_encryption/_model_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1903 2024-04-04 20:31:34.000000 py4phi-1.0.0/py4phi/_encryption/_pandas_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2154 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/_encryption/_polars_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2385 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/_encryption/_pyspark_encryptor.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.358260 py4phi-1.0.0/py4phi/analytics/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-27 20:27:56.000000 py4phi-1.0.0/py4phi/analytics/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      386 2024-03-30 16:13:27.000000 py4phi-1.0.0/py4phi/analytics/base_analytics.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7134 2024-04-03 20:50:33.000000 py4phi-1.0.0/py4phi/analytics/feature_selection.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8868 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/analytics/principal_component_analysis.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4619 2024-04-04 20:31:34.000000 py4phi-1.0.0/py4phi/config_processor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      680 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/consts.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    18008 2024-04-11 20:32:35.000000 py4phi-1.0.0/py4phi/controller.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4478 2024-04-09 21:20:29.000000 py4phi-1.0.0/py4phi/core.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.358260 py4phi-1.0.0/py4phi/dataset_handlers/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-04 14:14:53.000000 py4phi-1.0.0/py4phi/dataset_handlers/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     6097 2024-03-27 20:27:56.000000 py4phi-1.0.0/py4phi/dataset_handlers/base_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3117 2024-04-04 20:31:34.000000 py4phi-1.0.0/py4phi/dataset_handlers/pandas_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3084 2024-04-04 20:31:34.000000 py4phi-1.0.0/py4phi/dataset_handlers/polars_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4365 2024-04-12 15:14:38.000000 py4phi-1.0.0/py4phi/dataset_handlers/pyspark_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3636 2024-04-02 21:42:25.000000 py4phi-1.0.0/py4phi/dataset_handlers/pyspark_write_utils.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      553 2024-02-24 17:29:06.000000 py4phi-1.0.0/py4phi/log4j.properties
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      371 2024-04-07 09:05:07.000000 py4phi-1.0.0/py4phi/logger_setup.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      648 2024-03-27 20:27:56.000000 py4phi-1.0.0/py4phi/utils.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-12 23:06:10.358260 py4phi-1.0.0/py4phi.egg-info/
+-rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    24334 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/PKG-INFO
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1303 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/SOURCES.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        1 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/dependency_links.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       45 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/entry_points.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/requires.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       11 2024-04-12 23:06:10.000000 py4phi-1.0.0/py4phi.egg-info/top_level.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1731 2024-04-12 18:25:12.000000 py4phi-1.0.0/pyproject.toml
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       38 2024-04-12 23:06:10.358260 py4phi-1.0.0/setup.cfg
```

### Comparing `py4phi-0.9.1/LICENSE` & `py4phi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/NOTICE` & `py4phi-1.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/PKG-INFO` & `py4phi-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4phi
-Version: 0.9.1
+Version: 1.0.0
 Summary: A library for encryption/decryption and analysis of sensitive data.
 Author-email: Volodymyr Kiriushyn <zalorderon3331@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,24 +202,27 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/volodymyrkir/py4phi
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: iniconfig>=2.0.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: pluggy>=1.3.0
@@ -247,39 +250,83 @@
 In the modern IT world, sharing a dataset with sensitive data is common, especially if a team working on it is wide. It can be used for various purposes, including building a ML/DL model, simple business analysis, etc. Of course, in most companies, different restrictions are applied on the data, including row-level security, column hashing, or encrypting, but this requires at least some knowledge of data engineering libraries and can be  a challenging and time-consuming task. At the same time, employees with access to sensitive parts of the data may not have such expertise, which is where **py4phi** can be helpful.
 
 [![Coverage Status](https://coveralls.io/repos/github/volodymyrkir/py4phi/badge.svg?branch=ci_update)](https://coveralls.io/github/volodymyrkir/py4phi?branch=ci_update)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/py4phi)
 [![image](https://img.shields.io/pypi/v/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/l/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/pyversions/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
+[![image](https://img.shields.io/pypi/format/py4phi)](https://img.shields.io/pypi/format/py4phi)
+[![image](https://img.shields.io/pypi/status/py4phi)](https://img.shields.io/pypi/status/py4phi)
+
 # Functionality
 **py4phi** offers the following functionality to solve the problem mentioned above and more:
 **Encrypt a dataset column-wise.**
 **Decrypt a dataset column-wise.**
 **Encrypt any folder or machine learning model**
 **Decrypt any folder or machine learning model**
 **Perform principal component analysis on a dataset**
 **Perform correlation analysis for feature selection on a dataset**
 You can use **py4phi** both in Python code and through your terminal via the convenient CLI interface.
-#Setup and prerequisites
-In order to install the library [from PyPi](), just run
+# Setup and prerequisites
+
+In order to install the library [from PyPi](https://pypi.org/project/py4phi/), just run
 ```shell
 pip install py4phi
 ```
 
 ### **py4phi** is compatible with the following engines for data processing and encryption:
-* [Pandas](https://github.com/pandas-dev/pandas)
-* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)
-* [Polars](https://pola.rs/) 
-
-NOTE: Default engine for CLI is Pandas, whereas for library - PySpark.
-
-Nevertheless, you'll need a JDK installed and a JAVA_HOME environment variable set in order 
-to work with the PySpark engine. 
-However, you can still work with Pandas or Polars without JDK, if you wish.
+* [Pandas](https://github.com/pandas-dev/pandas)(v. 2.2.0+)
+* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)(v. 3.5.0+)
+* [Polars](https://pola.rs/)(v. 0.20.9)
+
+Default engine for CLI is Pandas, whereas for the library - PySpark.
+
+**NOTE: You can avoid steps below and still be able to use pandas or polars engines if that suits your needs.**
+## Pyspark installation
+
+You'll need a JDK installed and a JAVA_HOME environment variable set in order 
+to work with the PySpark engine on UNIX-like systems. 
+### Windows pyspark installation
+Apart from the JDK and JAVA_HOME variable, in order to work with pyspark engine, you will have to:
+1. Download and extract Spark 3.5.0+.
+2. Download winutils.exe and hadoop.dll.
+3. Add these files to /hadoop/bin folder.
+4. Set HADOOP_HOME environment variable pointing to $absolute_path/hadoop/bin.
+5. You may need to also set SPARK_HOME and PYSPARK_PYTHON environment variables.
+
+For more detailed info, please go through [this guide](https://saumyagoyal.medium.com/how-to-install-pyspark-on-windows-faf7ac293ecf).
+# API help
+**py4phi** documentation is still TBD, however API is pretty simple
+and most parameters are covered in the Usage section below and in the /examples folder.
+
+## Library API
+**py4phi.core** currently exposes 4 main functions.
+* from_path - allows you to initialize py4phi Controller(read below) from a file. 
+* from_dataframe - initialize with a dataframe (Pandas/Polars/PySpark).
+* encrypt_model - encrypt any folder or ML model INPLACE 
+* decrypt_model - decrypt any folder or ML model.
+
+The Controller itself has a lot of functionality,
+including encryption/decryption of a dataframes,
+feature selection and principal component analysis.
+
+## Terminal API
+As previously mentioned, you can perform all the same actions from your terminal.
+to get list of available commands, enter
+
+```shell
+py4phi --help
+```
+
+to get options/parameters of a specific command (e.g. encrypt), enter
+
+```shell
+py4phi encrypt --help
+```
+
 # Usage
 You can integrate **py4phi** in your existing pandas/pyspark/polars data pipeline by 
 initializing from a DataFrame or loading from a file. Currently, CSV and Parquet 
 file types are supported. 
 
 Encryption and decryption of the datasets are facilitated by the use of configs.
 Each column gets its own encryption key and a nonce, which are saved in the configs. These resulting files can be further encrypted for even more safety.
@@ -290,20 +337,20 @@
 and don't need to write long scripts to encrypt data and save the keys. 
 
 The following example showcases the encryption process of a dataset.csv file. \
 (you can find it in the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder) \
 The output dataset, along with the decryption configs, is then saved to the "test_folder" directory under CWD,
 
 ```python
-from py4phi.core import from_path
+from py4phi.core import from_path, PYSPARK
 
 controller = from_path(
     './dataset.csv',
     'csv',
-    engine='pyspark',
+    engine=PYSPARK,
     log_level='DEBUG',
     header=True  # pyspark read option
 )
 controller.print_current_df()
 controller.encrypt(columns_to_encrypt=['Staff involved', 'ACF'])
 controller.print_current_df()
 controller.save_encrypted(
@@ -372,39 +419,46 @@
 # Analytics usage
 Apart from the main encrypt/decrypt functionality, one may be interested in reducing
 the dimensionality of a dataset or performing correlation analysis of the feature (feature selection).
 In a typical scenario, this requires a lot of effort from the data analyst.
 Instead, a person with access to the sensitive data 
 can perform a lightweight **PCA/feature selection** in a couple of code lines or terminal commands.
 
-**NOTE**: This functionality is a quick top-level analysis, diving deeper into a dataset's feature analysis will always bring more profit.
+**NOTE**: _This functionality is a quick top-level analysis,
+diving deeper into a dataset's feature analysis will always bring more profit._
 
 To perform principal component analysis with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='pyspark')
+from py4phi.core import from_path, PYSPARK
+controller = from_path('Titanic.parquet', file_type='parquet', engine=PYSPARK)
 controller.perform_pca(
     target_feature='Survived',
     ignore_columns=['Name', 'Sex', 'Ticket', 'Cabin', 'Embarked'],
     save_reduced=False
 )
 ```
 
 Via terminal:
 
 ```shell
 py4phi perform-pca -i ./dataset.csv  --target 'Staff involved' -c ACF
 ```
 
+**NOTE** _In order to suggest feature - candidates for dropping,
+correlation analysis is leveraged. As for categorical features, Cramers V measure is used to calculate correlation. 
+It is heavily impacted by dataset's size, so please consider ignoring string columns
+for feature selection unless your data is bigger than at least 100-200 rows. In general, keep in mind that this
+analysis is kind of top-level._
+
 To perform feature selection with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='polars')
+from py4phi.core import from_path, POLARS
+controller = from_path('Titanic.parquet', file_type='parquet', engine=POLARS)
 controller.perform_feature_selection(
     target_feature='Survived',
     target_correlation_threshold=0.2,
     features_correlation_threshold=0.2,
     drop_recommended=False
 )
 ```
@@ -412,8 +466,8 @@
 Via terminal:
 
 ```shell
 py4phi feature-selection -i ./Titanic.parquet --target Survived --target_corr_threshold 0.3 --feature_corr_threshold 0.55
 ```
 
 Please look into the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder for more examples.
-It also contains training datasets.
+It also contains respective demo datasets.
```

### Comparing `py4phi-0.9.1/README.md` & `py4phi-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,39 +4,83 @@
 In the modern IT world, sharing a dataset with sensitive data is common, especially if a team working on it is wide. It can be used for various purposes, including building a ML/DL model, simple business analysis, etc. Of course, in most companies, different restrictions are applied on the data, including row-level security, column hashing, or encrypting, but this requires at least some knowledge of data engineering libraries and can be  a challenging and time-consuming task. At the same time, employees with access to sensitive parts of the data may not have such expertise, which is where **py4phi** can be helpful.
 
 [![Coverage Status](https://coveralls.io/repos/github/volodymyrkir/py4phi/badge.svg?branch=ci_update)](https://coveralls.io/github/volodymyrkir/py4phi?branch=ci_update)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/py4phi)
 [![image](https://img.shields.io/pypi/v/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/l/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/pyversions/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
+[![image](https://img.shields.io/pypi/format/py4phi)](https://img.shields.io/pypi/format/py4phi)
+[![image](https://img.shields.io/pypi/status/py4phi)](https://img.shields.io/pypi/status/py4phi)
+
 # Functionality
 **py4phi** offers the following functionality to solve the problem mentioned above and more:
 **Encrypt a dataset column-wise.**
 **Decrypt a dataset column-wise.**
 **Encrypt any folder or machine learning model**
 **Decrypt any folder or machine learning model**
 **Perform principal component analysis on a dataset**
 **Perform correlation analysis for feature selection on a dataset**
 You can use **py4phi** both in Python code and through your terminal via the convenient CLI interface.
-#Setup and prerequisites
-In order to install the library [from PyPi](), just run
+# Setup and prerequisites
+
+In order to install the library [from PyPi](https://pypi.org/project/py4phi/), just run
 ```shell
 pip install py4phi
 ```
 
 ### **py4phi** is compatible with the following engines for data processing and encryption:
-* [Pandas](https://github.com/pandas-dev/pandas)
-* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)
-* [Polars](https://pola.rs/) 
-
-NOTE: Default engine for CLI is Pandas, whereas for library - PySpark.
-
-Nevertheless, you'll need a JDK installed and a JAVA_HOME environment variable set in order 
-to work with the PySpark engine. 
-However, you can still work with Pandas or Polars without JDK, if you wish.
+* [Pandas](https://github.com/pandas-dev/pandas)(v. 2.2.0+)
+* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)(v. 3.5.0+)
+* [Polars](https://pola.rs/)(v. 0.20.9)
+
+Default engine for CLI is Pandas, whereas for the library - PySpark.
+
+**NOTE: You can avoid steps below and still be able to use pandas or polars engines if that suits your needs.**
+## Pyspark installation
+
+You'll need a JDK installed and a JAVA_HOME environment variable set in order 
+to work with the PySpark engine on UNIX-like systems. 
+### Windows pyspark installation
+Apart from the JDK and JAVA_HOME variable, in order to work with pyspark engine, you will have to:
+1. Download and extract Spark 3.5.0+.
+2. Download winutils.exe and hadoop.dll.
+3. Add these files to /hadoop/bin folder.
+4. Set HADOOP_HOME environment variable pointing to $absolute_path/hadoop/bin.
+5. You may need to also set SPARK_HOME and PYSPARK_PYTHON environment variables.
+
+For more detailed info, please go through [this guide](https://saumyagoyal.medium.com/how-to-install-pyspark-on-windows-faf7ac293ecf).
+# API help
+**py4phi** documentation is still TBD, however API is pretty simple
+and most parameters are covered in the Usage section below and in the /examples folder.
+
+## Library API
+**py4phi.core** currently exposes 4 main functions.
+* from_path - allows you to initialize py4phi Controller(read below) from a file. 
+* from_dataframe - initialize with a dataframe (Pandas/Polars/PySpark).
+* encrypt_model - encrypt any folder or ML model INPLACE 
+* decrypt_model - decrypt any folder or ML model.
+
+The Controller itself has a lot of functionality,
+including encryption/decryption of a dataframes,
+feature selection and principal component analysis.
+
+## Terminal API
+As previously mentioned, you can perform all the same actions from your terminal.
+to get list of available commands, enter
+
+```shell
+py4phi --help
+```
+
+to get options/parameters of a specific command (e.g. encrypt), enter
+
+```shell
+py4phi encrypt --help
+```
+
 # Usage
 You can integrate **py4phi** in your existing pandas/pyspark/polars data pipeline by 
 initializing from a DataFrame or loading from a file. Currently, CSV and Parquet 
 file types are supported. 
 
 Encryption and decryption of the datasets are facilitated by the use of configs.
 Each column gets its own encryption key and a nonce, which are saved in the configs. These resulting files can be further encrypted for even more safety.
@@ -47,20 +91,20 @@
 and don't need to write long scripts to encrypt data and save the keys. 
 
 The following example showcases the encryption process of a dataset.csv file. \
 (you can find it in the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder) \
 The output dataset, along with the decryption configs, is then saved to the "test_folder" directory under CWD,
 
 ```python
-from py4phi.core import from_path
+from py4phi.core import from_path, PYSPARK
 
 controller = from_path(
     './dataset.csv',
     'csv',
-    engine='pyspark',
+    engine=PYSPARK,
     log_level='DEBUG',
     header=True  # pyspark read option
 )
 controller.print_current_df()
 controller.encrypt(columns_to_encrypt=['Staff involved', 'ACF'])
 controller.print_current_df()
 controller.save_encrypted(
@@ -129,39 +173,46 @@
 # Analytics usage
 Apart from the main encrypt/decrypt functionality, one may be interested in reducing
 the dimensionality of a dataset or performing correlation analysis of the feature (feature selection).
 In a typical scenario, this requires a lot of effort from the data analyst.
 Instead, a person with access to the sensitive data 
 can perform a lightweight **PCA/feature selection** in a couple of code lines or terminal commands.
 
-**NOTE**: This functionality is a quick top-level analysis, diving deeper into a dataset's feature analysis will always bring more profit.
+**NOTE**: _This functionality is a quick top-level analysis,
+diving deeper into a dataset's feature analysis will always bring more profit._
 
 To perform principal component analysis with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='pyspark')
+from py4phi.core import from_path, PYSPARK
+controller = from_path('Titanic.parquet', file_type='parquet', engine=PYSPARK)
 controller.perform_pca(
     target_feature='Survived',
     ignore_columns=['Name', 'Sex', 'Ticket', 'Cabin', 'Embarked'],
     save_reduced=False
 )
 ```
 
 Via terminal:
 
 ```shell
 py4phi perform-pca -i ./dataset.csv  --target 'Staff involved' -c ACF
 ```
 
+**NOTE** _In order to suggest feature - candidates for dropping,
+correlation analysis is leveraged. As for categorical features, Cramers V measure is used to calculate correlation. 
+It is heavily impacted by dataset's size, so please consider ignoring string columns
+for feature selection unless your data is bigger than at least 100-200 rows. In general, keep in mind that this
+analysis is kind of top-level._
+
 To perform feature selection with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='polars')
+from py4phi.core import from_path, POLARS
+controller = from_path('Titanic.parquet', file_type='parquet', engine=POLARS)
 controller.perform_feature_selection(
     target_feature='Survived',
     target_correlation_threshold=0.2,
     features_correlation_threshold=0.2,
     drop_recommended=False
 )
 ```
@@ -169,8 +220,8 @@
 Via terminal:
 
 ```shell
 py4phi feature-selection -i ./Titanic.parquet --target Survived --target_corr_threshold 0.3 --feature_corr_threshold 0.55
 ```
 
 Please look into the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder for more examples.
-It also contains training datasets.
+It also contains respective demo datasets.
```

### Comparing `py4phi-0.9.1/cli/analytics/feature_selection.py` & `py4phi-1.0.0/cli/analytics/feature_selection.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/cli/analytics/principal_component_analysis.py` & `py4phi-1.0.0/cli/analytics/principal_component_analysis.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/cli/descriptions.py` & `py4phi-1.0.0/cli/descriptions.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/cli/encryption/encryption.py` & `py4phi-1.0.0/cli/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/cli/encryption/model_encryption.py` & `py4phi-1.0.0/cli/encryption/model_encryption.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/_encryption/_encryptor.py` & `py4phi-1.0.0/py4phi/_encryption/_encryptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         ----
         decryption_dict (dict[str, dict]): Dictionary containing
                                             decryption details for each column.
 
         Returns: Decrypted dataframe.
 
         """
+        logger.info(f"Decrypting columns: {decryption_dict}")
+        logger.info(f'{self._columns}')
         for column in self._columns:
             logger.info(f"Decrypting column: {column}.")
             if column in decryption_dict:
                 self._df = self._decrypt_column(column, decryption_dict[column])
             else:
                 logger.error(f"Column {column} is not in decryption config,"
                              f" cannot decrypt it.")
```

### Comparing `py4phi-0.9.1/py4phi/_encryption/_model_encryptor.py` & `py4phi-1.0.0/py4phi/_encryption/_model_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/_encryption/_pandas_encryptor.py` & `py4phi-1.0.0/py4phi/_encryption/_pandas_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/_encryption/_polars_encryptor.py` & `py4phi-1.0.0/py4phi/_encryption/_polars_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/_encryption/_pyspark_encryptor.py` & `py4phi-1.0.0/py4phi/_encryption/_pyspark_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/analytics/feature_selection.py` & `py4phi-1.0.0/py4phi/analytics/feature_selection.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/analytics/principal_component_analysis.py` & `py4phi-1.0.0/py4phi/analytics/principal_component_analysis.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/config_processor.py` & `py4phi-1.0.0/py4phi/config_processor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/consts.py` & `py4phi-1.0.0/py4phi/consts.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/controller.py` & `py4phi-1.0.0/py4phi/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,19 +184,20 @@
             save_format=save_format,
             **kwargs
         )
         logger.info(f'Saved outputs to: {save_location}.')
 
     def decrypt(
             self,
-            columns_to_decrypt: list[str],
+            columns_to_decrypt: list[str] = None,
             configs_path: str = CWD,
             config_file_name: str = DEFAULT_CONFIG_NAME,
             config_encrypted: bool = True,
-            key_file_name: str = DEFAULT_SECRET_NAME
+            key_file_name: str = DEFAULT_SECRET_NAME,
+            columns_mapping: dict[str, str] = None
     ) -> BaseDF:
         """
         Decrypt specified columns in dataset.
 
         Args:
         ----
         columns_to_decrypt (list[str]): List of columns to be decrypted.
@@ -205,47 +206,63 @@
                                         Defaults to current working directory.
         config_encrypted (bool): Whether config is encrypted.
                                     Defaults to True.
         config_file_name (str): Name of config to be saved.
                                     Defaults to DEFAULT_CONFIG_NAME.
         key_file_name (str): Name of config to be saved.
                                 Defaults to DEFAULT_SECRET_NAME.
+        columns_mapping (dict[str,str]): Mapping of columns, that were
+                                            originally in the config to new names.
+                                            key - old name, value - new name,
+                                            Defaults to None.
 
         Returns: Decrypted dataframe.
 
         """
         self.__encryptor = (
-            self._encryption_cls(self._current_df, columns_to_decrypt)
+            self._encryption_cls(self._current_df, columns_to_decrypt or [])
             if not self.__encryptor
             else self.__encryptor
         )
         if self.__columns_data:
             logger.debug(self.__columns_data)
             decryption_dict = {key: val for key, val in self.__columns_data.items()
                                if key in columns_to_decrypt}
             logger.debug("Decrypting previously encrypted dataframe, "
                          f"for columns {list(decryption_dict.keys())} "
                          "ignoring provided configs paths...")
         else:
-            logger.info(f'Kicking off decryption on current dataframe on columns: '
-                        f'{columns_to_decrypt}. ')
+            if columns_to_decrypt:
+                logger.info(f'Kicking off decryption on current dataframe for columns: '
+                            f'{columns_to_decrypt}. ')
             try:
                 logger.info(f'Config path is {configs_path}. '
                             f"{'Config is encrypted' if config_encrypted else ''}")
                 decryption_dict = self._config_processor.read_config(
                     configs_path,
                     conf_file_name=config_file_name,
                     config_encrypted=config_encrypted,
                     key_file_name=key_file_name
                 )
+                if not columns_to_decrypt:
+                    logger.info('No columns to decrypt provided, '
+                                'will decrypt all columns from the config:\n'
+                                f'{list(decryption_dict.keys())}')
+                    self.__encryptor._columns = list(decryption_dict.keys())
             except FileNotFoundError:
                 raise FileNotFoundError(
                     f"Decryption config files not found under {configs_path}. "
                 )
-
+        if columns_mapping:
+            for key, val in columns_mapping.items():
+                if key in decryption_dict:
+                    decryption_dict[val] = decryption_dict.pop(key)
+            self.__encryptor._columns = [
+                columns_mapping.get(key, key) for key in self.__encryptor._columns
+            ]
         self._current_df = self.__encryptor.decrypt(decryption_dict)
         self._decrypted = True
         logger.info('Successfully decrypted current df.')
         return self._current_df
 
     def perform_pca(
             self,
```

### Comparing `py4phi-0.9.1/py4phi/core.py` & `py4phi-1.0.0/py4phi/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     reader_cls = ENGINE_NAME_MAPPING.get(engine)
     if not reader_cls:
         raise ValueError(f"No such engine: {engine}, "
                          f"can be one of {tuple(ENGINE_NAME_MAPPING)}")
     reader = reader_cls()
     logger.debug(f"Reading dataframe using {type(reader)} "
                  f"from file: {path}, of type {file_type}.")
-    if not path.endswith(file_type):
+    if not path.endswith(file_type.lower()):
         logger.warning(f"Pay attention, path {path} "
                        f"does not end with file type {file_type}")
 
     reader.read_file(path=path, file_type=file_type, **kwargs)
 
     return Controller(reader)
```

### Comparing `py4phi-0.9.1/py4phi/dataset_handlers/base_dataset_handler.py` & `py4phi-1.0.0/py4phi/dataset_handlers/base_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/dataset_handlers/pandas_dataset_handler.py` & `py4phi-1.0.0/py4phi/dataset_handlers/pandas_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/dataset_handlers/polars_dataset_handler.py` & `py4phi-1.0.0/py4phi/dataset_handlers/polars_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/dataset_handlers/pyspark_dataset_handler.py` & `py4phi-1.0.0/py4phi/dataset_handlers/pyspark_dataset_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 
 
 class PySparkDatasetHandler(BaseDatasetHandler):
     """Class for reading in file or PySpark dataframe."""
 
     def __init__(self):
         super().__init__()
-        log4j_props_path = files(py4phi) / "log4j.properties"
+        log4j_props_path = os.path.normpath(
+            os.path.abspath(files(py4phi) / "log4j.properties")
+        )
+        log4j_props_path = log4j_props_path.replace(os.sep, os.sep + os.sep)
         self._spark = (
             SparkSession.builder.appName('py4phi')
             .config("spark.driver.extraJavaOptions",
-                    f"-Dlog4j.configuration=file:{log4j_props_path}")
+                    f"-Dlog4j2.configuration={log4j_props_path}")
             .getOrCreate()
         )
 
     @staticmethod
     def print_df(df: DataFrame) -> None:
         """
         Print PySpark dataframe.
```

### Comparing `py4phi-0.9.1/py4phi/dataset_handlers/pyspark_write_utils.py` & `py4phi-1.0.0/py4phi/dataset_handlers/pyspark_write_utils.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/log4j.properties` & `py4phi-1.0.0/py4phi/log4j.properties`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi/utils.py` & `py4phi-1.0.0/py4phi/utils.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/py4phi.egg-info/PKG-INFO` & `py4phi-1.0.0/py4phi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4phi
-Version: 0.9.1
+Version: 1.0.0
 Summary: A library for encryption/decryption and analysis of sensitive data.
 Author-email: Volodymyr Kiriushyn <zalorderon3331@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,24 +202,27 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/volodymyrkir/py4phi
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Security
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: iniconfig>=2.0.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: pluggy>=1.3.0
@@ -247,39 +250,83 @@
 In the modern IT world, sharing a dataset with sensitive data is common, especially if a team working on it is wide. It can be used for various purposes, including building a ML/DL model, simple business analysis, etc. Of course, in most companies, different restrictions are applied on the data, including row-level security, column hashing, or encrypting, but this requires at least some knowledge of data engineering libraries and can be  a challenging and time-consuming task. At the same time, employees with access to sensitive parts of the data may not have such expertise, which is where **py4phi** can be helpful.
 
 [![Coverage Status](https://coveralls.io/repos/github/volodymyrkir/py4phi/badge.svg?branch=ci_update)](https://coveralls.io/github/volodymyrkir/py4phi?branch=ci_update)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/py4phi)
 [![image](https://img.shields.io/pypi/v/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/l/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
 [![image](https://img.shields.io/pypi/pyversions/py4phi.svg)](https://pypi.python.org/pypi/py4phi)
+[![image](https://img.shields.io/pypi/format/py4phi)](https://img.shields.io/pypi/format/py4phi)
+[![image](https://img.shields.io/pypi/status/py4phi)](https://img.shields.io/pypi/status/py4phi)
+
 # Functionality
 **py4phi** offers the following functionality to solve the problem mentioned above and more:
 **Encrypt a dataset column-wise.**
 **Decrypt a dataset column-wise.**
 **Encrypt any folder or machine learning model**
 **Decrypt any folder or machine learning model**
 **Perform principal component analysis on a dataset**
 **Perform correlation analysis for feature selection on a dataset**
 You can use **py4phi** both in Python code and through your terminal via the convenient CLI interface.
-#Setup and prerequisites
-In order to install the library [from PyPi](), just run
+# Setup and prerequisites
+
+In order to install the library [from PyPi](https://pypi.org/project/py4phi/), just run
 ```shell
 pip install py4phi
 ```
 
 ### **py4phi** is compatible with the following engines for data processing and encryption:
-* [Pandas](https://github.com/pandas-dev/pandas)
-* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)
-* [Polars](https://pola.rs/) 
-
-NOTE: Default engine for CLI is Pandas, whereas for library - PySpark.
-
-Nevertheless, you'll need a JDK installed and a JAVA_HOME environment variable set in order 
-to work with the PySpark engine. 
-However, you can still work with Pandas or Polars without JDK, if you wish.
+* [Pandas](https://github.com/pandas-dev/pandas)(v. 2.2.0+)
+* [PySpark](https://spark.apache.org/docs/latest/api/python/index.html)(v. 3.5.0+)
+* [Polars](https://pola.rs/)(v. 0.20.9)
+
+Default engine for CLI is Pandas, whereas for the library - PySpark.
+
+**NOTE: You can avoid steps below and still be able to use pandas or polars engines if that suits your needs.**
+## Pyspark installation
+
+You'll need a JDK installed and a JAVA_HOME environment variable set in order 
+to work with the PySpark engine on UNIX-like systems. 
+### Windows pyspark installation
+Apart from the JDK and JAVA_HOME variable, in order to work with pyspark engine, you will have to:
+1. Download and extract Spark 3.5.0+.
+2. Download winutils.exe and hadoop.dll.
+3. Add these files to /hadoop/bin folder.
+4. Set HADOOP_HOME environment variable pointing to $absolute_path/hadoop/bin.
+5. You may need to also set SPARK_HOME and PYSPARK_PYTHON environment variables.
+
+For more detailed info, please go through [this guide](https://saumyagoyal.medium.com/how-to-install-pyspark-on-windows-faf7ac293ecf).
+# API help
+**py4phi** documentation is still TBD, however API is pretty simple
+and most parameters are covered in the Usage section below and in the /examples folder.
+
+## Library API
+**py4phi.core** currently exposes 4 main functions.
+* from_path - allows you to initialize py4phi Controller(read below) from a file. 
+* from_dataframe - initialize with a dataframe (Pandas/Polars/PySpark).
+* encrypt_model - encrypt any folder or ML model INPLACE 
+* decrypt_model - decrypt any folder or ML model.
+
+The Controller itself has a lot of functionality,
+including encryption/decryption of a dataframes,
+feature selection and principal component analysis.
+
+## Terminal API
+As previously mentioned, you can perform all the same actions from your terminal.
+to get list of available commands, enter
+
+```shell
+py4phi --help
+```
+
+to get options/parameters of a specific command (e.g. encrypt), enter
+
+```shell
+py4phi encrypt --help
+```
+
 # Usage
 You can integrate **py4phi** in your existing pandas/pyspark/polars data pipeline by 
 initializing from a DataFrame or loading from a file. Currently, CSV and Parquet 
 file types are supported. 
 
 Encryption and decryption of the datasets are facilitated by the use of configs.
 Each column gets its own encryption key and a nonce, which are saved in the configs. These resulting files can be further encrypted for even more safety.
@@ -290,20 +337,20 @@
 and don't need to write long scripts to encrypt data and save the keys. 
 
 The following example showcases the encryption process of a dataset.csv file. \
 (you can find it in the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder) \
 The output dataset, along with the decryption configs, is then saved to the "test_folder" directory under CWD,
 
 ```python
-from py4phi.core import from_path
+from py4phi.core import from_path, PYSPARK
 
 controller = from_path(
     './dataset.csv',
     'csv',
-    engine='pyspark',
+    engine=PYSPARK,
     log_level='DEBUG',
     header=True  # pyspark read option
 )
 controller.print_current_df()
 controller.encrypt(columns_to_encrypt=['Staff involved', 'ACF'])
 controller.print_current_df()
 controller.save_encrypted(
@@ -372,39 +419,46 @@
 # Analytics usage
 Apart from the main encrypt/decrypt functionality, one may be interested in reducing
 the dimensionality of a dataset or performing correlation analysis of the feature (feature selection).
 In a typical scenario, this requires a lot of effort from the data analyst.
 Instead, a person with access to the sensitive data 
 can perform a lightweight **PCA/feature selection** in a couple of code lines or terminal commands.
 
-**NOTE**: This functionality is a quick top-level analysis, diving deeper into a dataset's feature analysis will always bring more profit.
+**NOTE**: _This functionality is a quick top-level analysis,
+diving deeper into a dataset's feature analysis will always bring more profit._
 
 To perform principal component analysis with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='pyspark')
+from py4phi.core import from_path, PYSPARK
+controller = from_path('Titanic.parquet', file_type='parquet', engine=PYSPARK)
 controller.perform_pca(
     target_feature='Survived',
     ignore_columns=['Name', 'Sex', 'Ticket', 'Cabin', 'Embarked'],
     save_reduced=False
 )
 ```
 
 Via terminal:
 
 ```shell
 py4phi perform-pca -i ./dataset.csv  --target 'Staff involved' -c ACF
 ```
 
+**NOTE** _In order to suggest feature - candidates for dropping,
+correlation analysis is leveraged. As for categorical features, Cramers V measure is used to calculate correlation. 
+It is heavily impacted by dataset's size, so please consider ignoring string columns
+for feature selection unless your data is bigger than at least 100-200 rows. In general, keep in mind that this
+analysis is kind of top-level._
+
 To perform feature selection with Python, use: 
 
 ```python
-from py4phi.core import from_path
-controller = from_path('Titanic.parquet', file_type='parquet', engine='polars')
+from py4phi.core import from_path, POLARS
+controller = from_path('Titanic.parquet', file_type='parquet', engine=POLARS)
 controller.perform_feature_selection(
     target_feature='Survived',
     target_correlation_threshold=0.2,
     features_correlation_threshold=0.2,
     drop_recommended=False
 )
 ```
@@ -412,8 +466,8 @@
 Via terminal:
 
 ```shell
 py4phi feature-selection -i ./Titanic.parquet --target Survived --target_corr_threshold 0.3 --feature_corr_threshold 0.55
 ```
 
 Please look into the [/examples](https://github.com/volodymyrkir/py4phi/tree/main/examples) folder for more examples.
-It also contains training datasets.
+It also contains respective demo datasets.
```

### Comparing `py4phi-0.9.1/py4phi.egg-info/SOURCES.txt` & `py4phi-1.0.0/py4phi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.1/pyproject.toml` & `py4phi-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 [tool.setuptools.packages.find]
 include = ["py4phi*", "cli*"]
 
 [project]
 name="py4phi"
 requires-python = ">=3.10"
 license={file="LICENSE"}
-version = "0.9.1"
+version = "1.0.0"
 description="A library for encryption/decryption and analysis of sensitive data."
 readme = "README.md"
 classifiers=[
-    "Development Status :: 4 - Beta",
-    "License :: OSI Approved :: MIT License",
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Topic :: Security",
-    "Topic :: Scientific/Engineering"
+    "Topic :: Scientific/Engineering",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+
+    "Environment :: Console"
 ]
 
 authors = [
   {name = "Volodymyr Kiriushyn", email = "zalorderon3331@gmail.com" }
 ]
 dependencies = [
     "iniconfig>=2.0.0",
```

