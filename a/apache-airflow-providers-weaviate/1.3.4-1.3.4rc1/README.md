# Comparing `tmp/apache_airflow_providers_weaviate-1.3.4.tar.gz` & `tmp/apache_airflow_providers_weaviate-1.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_weaviate-1.3.4.tar", last modified: Tue Apr  9 12:42:44 2024, max compression
+gzip compressed data, was "apache_airflow_providers_weaviate-1.3.4rc1.tar", last modified: Tue Apr  9 12:42:44 2024, max compression
```

## Comparing `apache_airflow_providers_weaviate-1.3.4.tar` & `apache_airflow_providers_weaviate-1.3.4rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3123 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/LICENSE
--rw-r--r--   0        0        0     1583 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/__init__.py
--rw-r--r--   0        0        0     2403 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/get_provider_info.py
--rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/hooks/__init__.py
--rw-r--r--   0        0        0    47541 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/hooks/weaviate.py
--rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/operators/__init__.py
--rw-r--r--   0        0        0     8500 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/operators/weaviate.py
--rw-r--r--   0        0        0     3005 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 apache_airflow_providers_weaviate-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3127 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/__init__.py
+-rw-r--r--   0        0        0     2403 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/get_provider_info.py
+-rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/__init__.py
+-rw-r--r--   0        0        0    47541 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/weaviate.py
+-rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/__init__.py
+-rw-r--r--   0        0        0     8500 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/weaviate.py
+-rw-r--r--   0        0        0     3012 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 apache_airflow_providers_weaviate-1.3.4rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_weaviate-1.3.4/README.rst` & `apache_airflow_providers_weaviate-1.3.4rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-weaviate``
 
-Release: ``1.3.4``
+Release: ``1.3.4.rc1``
 
 
 `Weaviate <https://weaviate.io/developers/weaviate>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/LICENSE` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/get_provider_info.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/hooks/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/hooks/weaviate.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/weaviate.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/operators/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/airflow/providers/weaviate/operators/weaviate.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/weaviate.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.4/pyproject.toml` & `apache_airflow_providers_weaviate-1.3.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-weaviate"
-version = "1.3.4"
+version = "1.3.4.rc1"
 description = "Provider package apache-airflow-providers-weaviate for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,15 +52,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0rc0",
     "pandas>=1.2.5,<2.2",
     "weaviate-client>=3.24.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html"
```

### Comparing `apache_airflow_providers_weaviate-1.3.4/PKG-INFO` & `apache_airflow_providers_weaviate-1.3.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-weaviate
-Version: 1.3.4
+Version: 1.3.4rc1
 Summary: Provider package apache-airflow-providers-weaviate for Apache Airflow
 Keywords: airflow-provider,weaviate,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: weaviate-client>=3.24.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -72,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-weaviate``
 
-Release: ``1.3.4``
+Release: ``1.3.4.rc1``
 
 
 `Weaviate <https://weaviate.io/developers/weaviate>`__
 
 
 Provider package
 ----------------
```

