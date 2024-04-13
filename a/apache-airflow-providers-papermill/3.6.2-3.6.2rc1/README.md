# Comparing `tmp/apache_airflow_providers_papermill-3.6.2.tar.gz` & `tmp/apache_airflow_providers_papermill-3.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_papermill-3.6.2.tar", last modified: Tue Apr  9 12:38:44 2024, max compression
+gzip compressed data, was "apache_airflow_providers_papermill-3.6.2rc1.tar", last modified: Tue Apr  9 12:38:44 2024, max compression
```

## Comparing `apache_airflow_providers_papermill-3.6.2.tar` & `apache_airflow_providers_papermill-3.6.2rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3110 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/__init__.py
--rw-r--r--   0        0        0     2881 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/hooks/__init__.py
--rw-r--r--   0        0        0     5937 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/hooks/kernel.py
--rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/operators/__init__.py
--rw-r--r--   0        0        0     4689 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/operators/papermill.py
--rw-r--r--   0        0        0     2977 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0     3114 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/__init__.py
+-rw-r--r--   0        0        0     2881 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/__init__.py
+-rw-r--r--   0        0        0     5937 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/kernel.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/__init__.py
+-rw-r--r--   0        0        0     4689 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/papermill.py
+-rw-r--r--   0        0        0     2984 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.6.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_papermill-3.6.2/README.rst` & `apache_airflow_providers_papermill-3.6.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.6.2``
+Release: ``3.6.2.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/LICENSE` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/get_provider_info.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/hooks/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/hooks/kernel.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/kernel.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/operators/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/airflow/providers/papermill/operators/papermill.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/papermill.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.2/pyproject.toml` & `apache_airflow_providers_papermill-3.6.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-papermill"
-version = "3.6.2"
+version = "3.6.2.rc1"
 description = "Provider package apache-airflow-providers-papermill for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -51,15 +51,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0rc0",
     "ipykernel",
     "papermill[all]>=2.4.0",
     "scrapbook[all]",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2"
```

### Comparing `apache_airflow_providers_papermill-3.6.2/PKG-INFO` & `apache_airflow_providers_papermill-3.6.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-papermill
-Version: 3.6.2
+Version: 3.6.2rc1
 Summary: Provider package apache-airflow-providers-papermill for Apache Airflow
 Keywords: airflow-provider,papermill,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: ipykernel
 Requires-Dist: papermill[all]>=2.4.0
 Requires-Dist: scrapbook[all]
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -72,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.6.2``
+Release: ``3.6.2.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
```

