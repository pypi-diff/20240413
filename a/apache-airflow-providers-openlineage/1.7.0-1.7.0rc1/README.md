# Comparing `tmp/apache_airflow_providers_openlineage-1.7.0.tar.gz` & `tmp/apache_airflow_providers_openlineage-1.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openlineage-1.7.0.tar", last modified: Tue Apr  9 12:37:27 2024, max compression
+gzip compressed data, was "apache_airflow_providers_openlineage-1.7.0rc1.tar", last modified: Tue Apr  9 12:37:27 2024, max compression
```

## Comparing `apache_airflow_providers_openlineage-1.7.0.tar` & `apache_airflow_providers_openlineage-1.7.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4406 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/LICENSE
--rw-r--r--   0        0        0     1586 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/__init__.py
--rw-r--r--   0        0        0     3398 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/conf.py
--rw-r--r--   0        0        0     1081 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0        0        0     5070 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0        0        0     2412 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0        0        0     9996 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0        0        0     2999 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0        0        0     6605 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0        0        0    14634 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0        0        0     2644 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0        0        0    11624 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0        0        0     3076 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0        0        0     1625 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0        0        0    13806 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/sqlparser.py
--rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/selective_enable.py
--rw-r--r--   0        0        0     9366 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0        0        0    13115 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/utils.py
--rw-r--r--   0        0        0     3345 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4410 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE
+-rw-r--r--   0        0        0     1586 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py
+-rw-r--r--   0        0        0     3398 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/conf.py
+-rw-r--r--   0        0        0     1081 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0        0        0     5070 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0        0        0     2412 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0        0        0     9996 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0        0        0     2999 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0        0        0     6605 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0        0        0    14634 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0        0        0     2644 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0        0        0    11624 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0        0        0     3076 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0        0        0     1625 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0        0        0    13806 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/selective_enable.py
+-rw-r--r--   0        0        0     9366 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0        0        0    13115 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py
+-rw-r--r--   0        0        0     3355 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openlineage-1.7.0/README.rst` & `apache_airflow_providers_openlineage-1.7.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.0``
+Release: ``1.7.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/LICENSE` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/conf.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/conf.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/base.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/bash.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/manager.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/extractors/python.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/get_provider_info.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/adapter.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/facets.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/listener.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/macros.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/plugins/openlineage.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/sqlparser.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/selective_enable.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/selective_enable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/sql.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/airflow/providers/openlineage/utils/utils.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0/pyproject.toml` & `apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openlineage"
-version = "1.7.0"
+version = "1.7.0.rc1"
 description = "Provider package apache-airflow-providers-openlineage for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,16 +52,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.6.0",
-    "apache-airflow>=2.7.0",
+    "apache-airflow-providers-common-sql>=1.6.0rc0",
+    "apache-airflow>=2.7.0rc0",
     "attrs>=22.2",
     "openlineage-integration-common>=0.28.0",
     "openlineage-python>=0.28.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0"
```

### Comparing `apache_airflow_providers_openlineage-1.7.0/PKG-INFO` & `apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.7.0
+Version: 1.7.0rc1
 Summary: Provider package apache-airflow-providers-openlineage for Apache Airflow
 Keywords: airflow-provider,openlineage,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.6.0
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.6.0rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: attrs>=22.2
 Requires-Dist: openlineage-integration-common>=0.28.0
 Requires-Dist: openlineage-python>=0.28.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0
@@ -76,15 +76,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.0``
+Release: ``1.7.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

