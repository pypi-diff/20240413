# Comparing `tmp/apache_airflow_providers_snowflake-5.4.0.tar.gz` & `tmp/apache_airflow_providers_snowflake-5.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_snowflake-5.4.0.tar", last modified: Tue Apr  9 12:41:54 2024, max compression
+gzip compressed data, was "apache_airflow_providers_snowflake-5.4.0rc1.tar", last modified: Tue Apr  9 12:41:54 2024, max compression
```

## Comparing `apache_airflow_providers_snowflake-5.4.0.tar` & `apache_airflow_providers_snowflake-5.4.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4481 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/__init__.py
--rw-r--r--   0        0        0     4721 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0        0        0    21418 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0        0        0    14773 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0        0        0    26383 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/operators/snowflake.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0        0        0    12631 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0        0        0     4223 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/triggers/snowflake_trigger.py
--rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0        0        0     1644 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0        0        0     6762 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
--rw-r--r--   0        0        0     3240 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0/pyproject.toml
--rw-r--r--   0        0        0     6508 1970-01-01 00:00:00.000000 apache_airflow_providers_snowflake-5.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4485 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0        0        0     4721 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0        0        0    21418 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0        0        0    14773 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0        0        0    26383 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/snowflake.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0        0        0    12631 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0        0        0     4223 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0        0        0     1644 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0        0        0     6762 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+-rw-r--r--   0        0        0     3250 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6521 1970-01-01 00:00:00.000000 apache_airflow_providers_snowflake-5.4.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_snowflake-5.4.0/README.rst` & `apache_airflow_providers_snowflake-5.4.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``5.4.0``
+Release: ``5.4.0.rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/LICENSE` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/get_provider_info.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/operators/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/operators/snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/transfers/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/triggers/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/common.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.4.0/pyproject.toml` & `apache_airflow_providers_snowflake-5.4.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-snowflake"
-version = "5.4.0"
+version = "5.4.0.rc1"
 description = "Provider package apache-airflow-providers-snowflake for Apache Airflow"
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
     "snowflake-connector-python>=2.7.8",
     "snowflake-sqlalchemy>=1.1.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html"
```

### Comparing `apache_airflow_providers_snowflake-5.4.0/PKG-INFO` & `apache_airflow_providers_snowflake-5.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 5.4.0
+Version: 5.4.0rc1
 Summary: Provider package apache-airflow-providers-snowflake for Apache Airflow
 Keywords: airflow-provider,snowflake,airflow,integration
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
 Requires-Dist: snowflake-connector-python>=2.7.8
 Requires-Dist: snowflake-sqlalchemy>=1.1.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0
@@ -77,15 +77,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``5.4.0``
+Release: ``5.4.0.rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

