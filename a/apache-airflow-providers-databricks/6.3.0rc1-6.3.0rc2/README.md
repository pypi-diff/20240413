# Comparing `tmp/apache_airflow_providers_databricks-6.3.0rc1.tar.gz` & `tmp/apache_airflow_providers_databricks-6.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_databricks-6.3.0rc1.tar", last modified: Tue Apr  9 12:25:57 2024, max compression
+gzip compressed data, was "apache_airflow_providers_databricks-6.3.0rc2.tar", last modified: Tue Apr  9 12:25:57 2024, max compression
```

## Comparing `apache_airflow_providers_databricks-6.3.0rc1.tar` & `apache_airflow_providers_databricks-6.3.0rc2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4448 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/LICENSE
--rw-r--r--   0        0        0     1585 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0        0        0     6221 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0        0        0    23378 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0        0        0    30592 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0        0        0    12564 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
--rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0        0        0    42438 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0        0        0    13093 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0        0        0    16800 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py
--rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0        0        0    10605 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0        0        0     5771 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
--rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0        0        0     4125 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/databricks.py
--rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/databricks.py
--rw-r--r--   0        0        0     3268 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6500 1970-01-01 00:00:00.000000 apache_airflow_providers_databricks-6.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4448 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/LICENSE
+-rw-r--r--   0        0        0     1585 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/__init__.py
+-rw-r--r--   0        0        0     6221 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0        0        0    23377 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0        0        0    30592 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0        0        0    12564 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks_sql.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0        0        0    42438 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0        0        0    13093 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0        0        0    16800 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks_sql.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0        0        0    10605 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0        0        0     5771 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/databricks_sql.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0        0        0     4125 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/triggers/databricks.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/utils/databricks.py
+-rw-r--r--   0        0        0     3268 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6500 1970-01-01 00:00:00.000000 apache_airflow_providers_databricks-6.3.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/README.rst` & `apache_airflow_providers_databricks-6.3.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``6.3.0.rc1``
+Release: ``6.3.0.rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/LICENSE` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/get_provider_info.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 SUBMIT_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/submit")
 GET_RUN_ENDPOINT = ("GET", "api/2.1/jobs/runs/get")
 CANCEL_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel")
 DELETE_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/delete")
 REPAIR_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/repair")
 OUTPUT_RUNS_JOB_ENDPOINT = ("GET", "api/2.1/jobs/runs/get-output")
 CANCEL_ALL_RUNS_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel-all")
-UPDATE_PERMISSION_ENDPOINT = ("PATCH", "/api/2.0/permissions/jobs")
+UPDATE_PERMISSION_ENDPOINT = ("PATCH", "api/2.0/permissions/jobs")
 
 INSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/install")
 UNINSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/uninstall")
 
 LIST_JOBS_ENDPOINT = ("GET", "api/2.1/jobs/list")
 LIST_PIPELINES_ENDPOINT = ("GET", "api/2.0/pipelines")
```

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc2/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/pyproject.toml` & `apache_airflow_providers_databricks-6.3.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-databricks"
-version = "6.3.0.rc1"
+version = "6.3.0.rc2"
 description = "Provider package apache-airflow-providers-databricks for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
```

### Comparing `apache_airflow_providers_databricks-6.3.0rc1/PKG-INFO` & `apache_airflow_providers_databricks-6.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 6.3.0rc1
+Version: 6.3.0rc2
 Summary: Provider package apache-airflow-providers-databricks for Apache Airflow
 Keywords: airflow-provider,databricks,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -78,15 +78,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``6.3.0.rc1``
+Release: ``6.3.0.rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

