# Comparing `tmp/apache_airflow_providers_odbc-4.5.0.tar.gz` & `tmp/apache_airflow_providers_odbc-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_odbc-4.5.0.tar", last modified: Tue Apr  9 12:36:44 2024, max compression
+gzip compressed data, was "apache_airflow_providers_odbc-4.5.0rc1.tar", last modified: Tue Apr  9 12:36:44 2024, max compression
```

## Comparing `apache_airflow_providers_odbc-4.5.0.tar` & `apache_airflow_providers_odbc-4.5.0rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4221 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/LICENSE
--rw-r--r--   0        0        0     1579 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/__init__.py
--rw-r--r--   0        0        0     2449 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/hooks/__init__.py
--rw-r--r--   0        0        0     9984 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/hooks/odbc.py
--rw-r--r--   0        0        0     3079 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4225 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/odbc.py
+-rw-r--r--   0        0        0     3089 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.5.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_odbc-4.5.0/README.rst` & `apache_airflow_providers_odbc-4.5.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.5.0``
+Release: ``4.5.0.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/LICENSE` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/__init__.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/get_provider_info.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/hooks/__init__.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.5.0/airflow/providers/odbc/hooks/odbc.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/odbc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.5.0/pyproject.toml` & `apache_airflow_providers_odbc-4.5.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-odbc"
-version = "4.5.0"
+version = "4.5.0.rc1"
 description = "Provider package apache-airflow-providers-odbc for Apache Airflow"
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
-    "apache-airflow-providers-common-sql>=1.10.0",
-    "apache-airflow>=2.6.0",
+    "apache-airflow-providers-common-sql>=1.10.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "pyodbc",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_odbc-4.5.0/PKG-INFO` & `apache_airflow_providers_odbc-4.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 4.5.0
+Version: 4.5.0rc1
 Summary: Provider package apache-airflow-providers-odbc for Apache Airflow
 Keywords: airflow-provider,odbc,airflow,integration
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
-Requires-Dist: apache-airflow-providers-common-sql>=1.10.0
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.10.0rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: pyodbc
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -74,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.5.0``
+Release: ``4.5.0.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
```

