# Comparing `tmp/apache_airflow_providers_cohere-1.1.3rc1.tar.gz` & `tmp/apache_airflow_providers_cohere-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cohere-1.1.3rc1.tar", last modified: Tue Apr  9 12:22:19 2024, max compression
+gzip compressed data, was "apache_airflow_providers_cohere-1.2.0rc1.tar", last modified: Mon Jan 22 08:26:32 2024, max compression
```

## Comparing `apache_airflow_providers_cohere-1.1.3rc1.tar` & `apache_airflow_providers_cohere-1.2.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3059 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/LICENSE
--rw-r--r--   0        0        0     1581 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/__init__.py
--rw-r--r--   0        0        0     2251 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/get_provider_info.py
--rw-r--r--   0        0        0     1053 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/hooks/__init__.py
--rw-r--r--   0        0        0     2725 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/hooks/cohere.py
--rw-r--r--   0        0        0      785 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/operators/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/operators/embedding.py
--rw-r--r--   0        0        0     2964 2024-04-09 12:22:19.000000 apache_airflow_providers_cohere-1.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0     4750 1970-01-01 00:00:00.000000 apache_airflow_providers_cohere-1.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     3051 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/LICENSE
+-rw-r--r--   0        0        0     1581 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/__init__.py
+-rw-r--r--   0        0        0     2239 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/get_provider_info.py
+-rw-r--r--   0        0        0     1053 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/hooks/__init__.py
+-rw-r--r--   0        0        0     2725 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/hooks/cohere.py
+-rw-r--r--   0        0        0      785 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/operators/__init__.py
+-rw-r--r--   0        0        0     2640 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/operators/embedding.py
+-rw-r--r--   0        0        0     2917 2024-01-22 08:26:32.000000 apache_airflow_providers_cohere-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 apache_airflow_providers_cohere-1.2.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/README.rst` & `apache_airflow_providers_cohere-1.2.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -38,43 +38,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cohere``
 
-Release: ``1.1.3.rc1``
+Release: ``1.2.0.rc1``
 
 
 `Cohere <https://docs.cohere.com/docs>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cohere`` provider. All classes for this provider package
 are in ``airflow.providers.cohere`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cohere``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.6.0``
-``cohere``          ``>=4.37,<5``
+``cohere``          ``>=4.37``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/LICENSE` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/__init__.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.3"
+__version__ = "1.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/get_provider_info.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cohere",
         "name": "Cohere",
         "description": "`Cohere <https://docs.cohere.com/docs>`__\n",
         "state": "ready",
-        "source-date-epoch": 1712665339,
-        "versions": ["1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "source-date-epoch": 1705911992,
+        "versions": ["1.2.0", "1.1.1", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Cohere",
                 "external-doc-url": "https://docs.cohere.com/docs",
                 "how-to-guide": ["/docs/apache-airflow-providers-cohere/operators/embedding.rst"],
                 "tags": ["software"],
             }
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "cohere>=4.37,<5"],
+        "dependencies": ["apache-airflow>=2.6.0", "cohere>=4.37"],
         "hooks": [
             {"integration-name": "Cohere", "python-modules": ["airflow.providers.cohere.hooks.cohere"]}
         ],
         "operators": [
             {"integration-name": "Cohere", "python-modules": ["airflow.providers.cohere.operators.embedding"]}
         ],
         "connection-types": [
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/hooks/__init__.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/hooks/cohere.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/hooks/cohere.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,23 @@
     hook_name = "Cohere"
 
     def __init__(
         self,
         conn_id: str = default_conn_name,
         timeout: int | None = None,
         max_retries: int | None = None,
+        **kwargs,
     ) -> None:
-        super().__init__()
+        super().__init__(**kwargs)
         self.conn_id = conn_id
         self.timeout = timeout
         self.max_retries = max_retries
 
     @cached_property
-    def get_conn(self) -> cohere.Client:  # type: ignore[override]
+    def get_conn(self) -> cohere.Client:
         conn = self.get_connection(self.conn_id)
         return cohere.Client(
             api_key=conn.password, timeout=self.timeout, max_retries=self.max_retries, api_url=conn.host
         )
 
     def create_embeddings(
         self, texts: list[str], model: str = "embed-multilingual-v2.0"
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/operators/__init__.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/airflow/providers/cohere/operators/embedding.py` & `apache_airflow_providers_cohere-1.2.0rc1/airflow/providers/cohere/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/pyproject.toml` & `apache_airflow_providers_cohere-1.2.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-cohere"
-version = "1.1.3.rc1"
+version = "1.2.0.rc1"
 description = "Provider package apache-airflow-providers-cohere for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,26 +47,25 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0rc0",
-    "cohere>=4.37,<5",
+    "apache-airflow>=2.6.0.dev0",
+    "cohere>=4.37",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_cohere-1.1.3rc1/PKG-INFO` & `apache_airflow_providers_cohere-1.2.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cohere
-Version: 1.1.3rc1
+Version: 1.2.0rc1
 Summary: Provider package apache-airflow-providers-cohere for Apache Airflow
 Keywords: airflow-provider,cohere,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,21 +15,20 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0rc0
-Requires-Dist: cohere>=4.37,<5
+Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: cohere>=4.37
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -71,43 +70,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cohere``
 
-Release: ``1.1.3.rc1``
+Release: ``1.2.0.rc1``
 
 
 `Cohere <https://docs.cohere.com/docs>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cohere`` provider. All classes for this provider package
 are in ``airflow.providers.cohere`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cohere``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.6.0``
-``cohere``          ``>=4.37,<5``
+``cohere``          ``>=4.37``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.1.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cohere/1.2.0/changelog.html>`_.
```

