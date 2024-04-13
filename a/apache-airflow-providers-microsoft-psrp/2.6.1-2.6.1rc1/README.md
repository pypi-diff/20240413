# Comparing `tmp/apache_airflow_providers_microsoft_psrp-2.6.1.tar.gz` & `tmp/apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_microsoft_psrp-2.6.1.tar", last modified: Tue Apr  9 12:36:19 2024, max compression
+gzip compressed data, was "apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar", last modified: Tue Apr  9 12:36:19 2024, max compression
```

## Comparing `apache_airflow_providers_microsoft_psrp-2.6.1.tar` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3226 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/LICENSE
--rw-r--r--   0        0        0     1589 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/__init__.py
--rw-r--r--   0        0        0     2873 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/hooks/__init__.py
--rw-r--r--   0        0        0    11157 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/hooks/psrp.py
--rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/operators/__init__.py
--rw-r--r--   0        0        0     7180 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/operators/psrp.py
--rw-r--r--   0        0        0     3011 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_psrp-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3230 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/LICENSE
+-rw-r--r--   0        0        0     1589 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/__init__.py
+-rw-r--r--   0        0        0     2873 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
+-rw-r--r--   0        0        0    11157 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py
+-rw-r--r--   0        0        0     7180 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py
+-rw-r--r--   0        0        0     3018 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4959 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/README.rst` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.6.1``
+Release: ``2.6.1.rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/openspecs/windows_protocols/ms-psrp/>`__.
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/LICENSE` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/get_provider_info.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/hooks/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/hooks/psrp.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/operators/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/airflow/providers/microsoft/psrp/operators/psrp.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/pyproject.toml` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-microsoft-psrp"
-version = "2.6.1"
+version = "2.6.1.rc1"
 description = "Provider package apache-airflow-providers-microsoft-psrp for Apache Airflow"
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
     "pypsrp>=0.8.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.1/PKG-INFO` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.6.1
+Version: 2.6.1rc1
 Summary: Provider package apache-airflow-providers-microsoft-psrp for Apache Airflow
 Keywords: airflow-provider,microsoft.psrp,airflow,integration
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
 Requires-Dist: pypsrp>=0.8.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.6.1``
+Release: ``2.6.1.rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/openspecs/windows_protocols/ms-psrp/>`__.
```

