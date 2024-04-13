# Comparing `tmp/apache_airflow_providers_apache_spark-4.7.2rc1.tar.gz` & `tmp/apache_airflow_providers_apache_spark-4.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_spark-4.7.2rc1.tar", last modified: Tue Apr  9 12:14:59 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_spark-4.8.0rc1.tar", last modified: Mon Jan 22 08:25:41 2024, max compression
```

## Comparing `apache_airflow_providers_apache_spark-4.7.2rc1.tar` & `apache_airflow_providers_apache_spark-4.8.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4222 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/LICENSE
--rw-r--r--   0        0        0     1587 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0        0        0      787 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/decorators/__init__.py
--rw-r--r--   0        0        0     4546 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/decorators/pyspark.py
--rw-r--r--   0        0        0     4472 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0        0        0     3237 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_connect.py
--rw-r--r--   0        0        0    11730 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0        0        0     6753 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0        0        0     7917 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0        0        0    32598 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py
--rw-r--r--   0        0        0      787 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0        0        0     8899 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0        0        0     4909 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0        0        0     9657 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_submit.py
--rw-r--r--   0        0        0     3141 2024-04-09 12:14:59.000000 apache_airflow_providers_apache_spark-4.7.2rc1/pyproject.toml
--rw-r--r--   0        0        0     6099 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_spark-4.7.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     4217 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/LICENSE
+-rw-r--r--   0        0        0     1587 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/__init__.py
+-rw-r--r--   0        0        0     4546 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/pyspark.py
+-rw-r--r--   0        0        0     4451 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0        0        0     3192 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_connect.py
+-rw-r--r--   0        0        0    11730 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0        0        0     6753 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0        0        0     7906 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0        0        0    32569 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+-rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0        0        0    10223 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0        0        0     4508 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0        0        0     9702 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_submit.py
+-rw-r--r--   0        0        0     3094 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6042 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_spark-4.8.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/README.rst` & `apache_airflow_providers_apache_spark-4.8.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.7.2.rc1``
+Release: ``4.8.0.rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -93,8 +93,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/LICENSE` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.7.2"
+__version__ = "4.8.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/decorators/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/decorators/pyspark.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/pyspark.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/get_provider_info.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1712664899,
+        "source-date-epoch": 1705911941,
         "versions": [
-            "4.7.2",
-            "4.7.1",
+            "4.8.0",
             "4.7.0",
             "4.6.0",
             "4.5.0",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.5",
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_connect.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_connect_default"
     conn_type = "spark_connect"
     hook_name = "Spark Connect"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom UI field behaviour for Spark Connect connection."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": [
                 "schema",
             ],
             "relabeling": {"password": "Token", "login": "User ID"},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Return connection widgets to add to Spark Connect connection form."""
+        """Returns connection widgets to add to connection form."""
         from flask_babel import lazy_gettext
         from wtforms import BooleanField
 
         return {
             SparkConnectHook.PARAM_USE_SSL: BooleanField(lazy_gettext("Use SSL"), default=False),
         }
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,23 +52,23 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_sql_default"
     conn_type = "spark_sql"
     hook_name = "Spark SQL"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom UI field behaviour for Spark SQL connection."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["schema", "login", "password", "extra"],
             "relabeling": {},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Return connection widgets to add to Spark SQL connection form."""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
         from wtforms.validators import Optional
 
         return {
             "queue": StringField(
@@ -90,16 +90,17 @@
         keytab: str | None = None,
         principal: str | None = None,
         master: str | None = None,
         name: str = "default-name",
         num_executors: int | None = None,
         verbose: bool = True,
         yarn_queue: str | None = None,
+        **kwargs,
     ) -> None:
-        super().__init__()
+        super().__init__(**kwargs)
         options: dict = {}
         conn: Connection | None = None
 
         try:
             conn = self.get_connection(conn_id)
         except AirflowNotFoundException:
             conn = None
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,23 +93,23 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_default"
     conn_type = "spark"
     hook_name = "Spark"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom UI field behaviour for Spark connection."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["schema", "login", "password", "extra"],
             "relabeling": {},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Return connection widgets to add to Spark connection form."""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
         from wtforms.validators import Optional, any_of
 
         return {
             "queue": StringField(
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,23 +40,31 @@
     :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark-submit>`
         as configured in Airflow administration
     :param spark_conf: Any additional Spark configuration properties
     :param spark_py_files: Additional python files used (.zip, .egg, or .py)
     :param spark_files: Additional files to upload to the container running the job
     :param spark_jars: Additional jars to upload and add to the driver and
                        executor classpath
+    :param num_executors: number of executor to run. This should be set so as to manage
+                          the number of connections made with the JDBC database
+    :param executor_cores: Number of cores per executor
+    :param executor_memory: Memory per executor (e.g. 1000M, 2G)
+    :param driver_memory: Memory allocated to the driver (e.g. 1000M, 2G)
+    :param verbose: Whether to pass the verbose flag to spark-submit for debugging
+    :param keytab: Full path to the file that contains the keytab
+    :param principal: The name of the kerberos principal used for keytab
     :param cmd_type: Which way the data should flow. 2 possible values:
                      spark_to_jdbc: data written by spark from metastore to jdbc
                      jdbc_to_spark: data written by spark from jdbc to metastore
     :param jdbc_table: The name of the JDBC table
     :param jdbc_conn_id: Connection id used for connection to JDBC database
     :param jdbc_driver: Name of the JDBC driver to use for the JDBC connection. This
                         driver (usually a jar) should be passed in the 'jars' parameter
     :param metastore_table: The name of the metastore table,
-    :param jdbc_truncate: (spark_to_jdbc only) Whether Spark should truncate or
+    :param jdbc_truncate: (spark_to_jdbc only) Whether or not Spark should truncate or
                          drop and recreate the JDBC table. This only takes effect if
                          'save_mode' is set to Overwrite. Also, if the schema is
                          different, Spark cannot truncate, and will drop and recreate
     :param save_mode: The Spark save-mode to use (e.g. overwrite, append, etc.)
     :param save_format: (jdbc_to_spark-only) The Spark save-format to use (e.g. parquet)
     :param batch_size: (spark_to_jdbc only) The size of the batch to insert per round
                        trip to the JDBC database. Defaults to 1000
@@ -79,26 +87,35 @@
     :param create_table_column_types: (spark_to_jdbc-only) The database column data types
                                       to use instead of the defaults, when creating the
                                       table. Data type information should be specified in
                                       the same format as CREATE TABLE columns syntax
                                       (e.g: "name CHAR(64), comments VARCHAR(1024)").
                                       The specified types should be valid spark sql data
                                       types.
-    :param kwargs: kwargs passed to SparkSubmitOperator.
+    :param use_krb5ccache: if True, configure spark to use ticket cache instead of relying
+                           on keytab for Kerberos login
+
     """
 
     def __init__(
         self,
         *,
         spark_app_name: str = "airflow-spark-jdbc",
         spark_conn_id: str = "spark-default",
         spark_conf: dict[str, Any] | None = None,
         spark_py_files: str | None = None,
         spark_files: str | None = None,
         spark_jars: str | None = None,
+        num_executors: int | None = None,
+        executor_cores: int | None = None,
+        executor_memory: str | None = None,
+        driver_memory: str | None = None,
+        verbose: bool = False,
+        principal: str | None = None,
+        keytab: str | None = None,
         cmd_type: str = "spark_to_jdbc",
         jdbc_table: str | None = None,
         jdbc_conn_id: str = "jdbc-default",
         jdbc_driver: str | None = None,
         metastore_table: str | None = None,
         jdbc_truncate: bool = False,
         save_mode: str | None = None,
@@ -106,23 +123,31 @@
         batch_size: int | None = None,
         fetch_size: int | None = None,
         num_partitions: int | None = None,
         partition_column: str | None = None,
         lower_bound: str | None = None,
         upper_bound: str | None = None,
         create_table_column_types: str | None = None,
+        use_krb5ccache: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self._spark_app_name = spark_app_name
         self._spark_conn_id = spark_conn_id
         self._spark_conf = spark_conf
         self._spark_py_files = spark_py_files
         self._spark_files = spark_files
         self._spark_jars = spark_jars
+        self._num_executors = num_executors
+        self._executor_cores = executor_cores
+        self._executor_memory = executor_memory
+        self._driver_memory = driver_memory
+        self._verbose = verbose
+        self._keytab = keytab
+        self._principal = principal
         self._cmd_type = cmd_type
         self._jdbc_table = jdbc_table
         self._jdbc_conn_id = jdbc_conn_id
         self._jdbc_driver = jdbc_driver
         self._metastore_table = metastore_table
         self._jdbc_truncate = jdbc_truncate
         self._save_mode = save_mode
@@ -131,14 +156,15 @@
         self._fetch_size = fetch_size
         self._num_partitions = num_partitions
         self._partition_column = partition_column
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
         self._create_table_column_types = create_table_column_types
         self._hook: SparkJDBCHook | None = None
+        self._use_krb5ccache = use_krb5ccache
 
     def execute(self, context: Context) -> None:
         """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.submit_jdbc_job()
 
@@ -156,16 +182,16 @@
             spark_files=self._spark_files,
             spark_jars=self._spark_jars,
             num_executors=self._num_executors,
             executor_cores=self._executor_cores,
             executor_memory=self._executor_memory,
             driver_memory=self._driver_memory,
             verbose=self._verbose,
-            keytab=self.keytab,
-            principal=self.principal,
+            keytab=self._keytab,
+            principal=self._principal,
             cmd_type=self._cmd_type,
             jdbc_table=self._jdbc_table,
             jdbc_conn_id=self._jdbc_conn_id,
             jdbc_driver=self._jdbc_driver,
             metastore_table=self._metastore_table,
             jdbc_truncate=self._jdbc_truncate,
             save_mode=self._save_mode,
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Sequence
 
-from deprecated import deprecated
-
-from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.apache.spark.hooks.spark_sql import SparkSqlHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -51,17 +48,17 @@
     :param name: Name of the job
     :param num_executors: Number of executors to launch
     :param verbose: Whether to pass the verbose flag to spark-sql
     :param yarn_queue: The YARN queue to submit to
         (Default: The ``queue`` value set in the Connection, or ``"default"``)
     """
 
-    template_fields: Sequence[str] = ("sql",)
+    template_fields: Sequence[str] = ("_sql",)
     template_ext: Sequence[str] = (".sql", ".hql")
-    template_fields_renderers = {"sql": "sql"}
+    template_fields_renderers = {"_sql": "sql"}
 
     def __init__(
         self,
         *,
         sql: str,
         conf: str | None = None,
         conn_id: str = "spark_sql_default",
@@ -74,38 +71,29 @@
         name: str = "default-name",
         num_executors: int | None = None,
         verbose: bool = True,
         yarn_queue: str | None = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self.sql = sql
+        self._sql = sql
         self._conf = conf
         self._conn_id = conn_id
         self._total_executor_cores = total_executor_cores
         self._executor_cores = executor_cores
         self._executor_memory = executor_memory
         self._keytab = keytab
         self._principal = principal
         self._master = master
         self._name = name
         self._num_executors = num_executors
         self._verbose = verbose
         self._yarn_queue = yarn_queue
         self._hook: SparkSqlHook | None = None
 
-    @property
-    @deprecated(
-        reason="`_sql` is deprecated and will be removed in the future. Please use `sql` instead.",
-        category=AirflowProviderDeprecationWarning,
-    )
-    def _sql(self):
-        """Alias for ``sql``, used for compatibility (deprecated)."""
-        return self.sql
-
     def execute(self, context: Context) -> None:
         """Call the SparkSqlHook to run the provided sql query."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.run_query()
 
     def on_kill(self) -> None:
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,29 @@
     :param deploy_mode: Whether to deploy your driver on the worker nodes (cluster) or locally as a client.
                         (will overwrite any deployment mode defined in the connection's extra JSON)
     :param use_krb5ccache: if True, configure spark to use ticket cache instead of relying
                            on keytab for Kerberos login
     """
 
     template_fields: Sequence[str] = (
-        "application",
-        "conf",
-        "files",
-        "py_files",
-        "jars",
-        "driver_class_path",
-        "packages",
-        "exclude_packages",
-        "keytab",
-        "principal",
-        "proxy_user",
-        "name",
-        "application_args",
-        "env_vars",
-        "properties_file",
+        "_application",
+        "_conf",
+        "_files",
+        "_py_files",
+        "_jars",
+        "_driver_class_path",
+        "_packages",
+        "_exclude_packages",
+        "_keytab",
+        "_principal",
+        "_proxy_user",
+        "_name",
+        "_application_args",
+        "_env_vars",
+        "_properties_file",
     )
     ui_color = WEB_COLORS["LIGHTORANGE"]
 
     def __init__(
         self,
         *,
         application: str = "",
@@ -131,82 +131,82 @@
         properties_file: str | None = None,
         queue: str | None = None,
         deploy_mode: str | None = None,
         use_krb5ccache: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self.application = application
-        self.conf = conf
-        self.files = files
-        self.py_files = py_files
+        self._application = application
+        self._conf = conf
+        self._files = files
+        self._py_files = py_files
         self._archives = archives
-        self.driver_class_path = driver_class_path
-        self.jars = jars
+        self._driver_class_path = driver_class_path
+        self._jars = jars
         self._java_class = java_class
-        self.packages = packages
-        self.exclude_packages = exclude_packages
+        self._packages = packages
+        self._exclude_packages = exclude_packages
         self._repositories = repositories
         self._total_executor_cores = total_executor_cores
         self._executor_cores = executor_cores
         self._executor_memory = executor_memory
         self._driver_memory = driver_memory
-        self.keytab = keytab
-        self.principal = principal
-        self.proxy_user = proxy_user
-        self.name = name
+        self._keytab = keytab
+        self._principal = principal
+        self._proxy_user = proxy_user
+        self._name = name
         self._num_executors = num_executors
         self._status_poll_interval = status_poll_interval
-        self.application_args = application_args
-        self.env_vars = env_vars
+        self._application_args = application_args
+        self._env_vars = env_vars
         self._verbose = verbose
         self._spark_binary = spark_binary
-        self.properties_file = properties_file
+        self._properties_file = properties_file
         self._queue = queue
         self._deploy_mode = deploy_mode
         self._hook: SparkSubmitHook | None = None
         self._conn_id = conn_id
         self._use_krb5ccache = use_krb5ccache
 
     def execute(self, context: Context) -> None:
         """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
-        self._hook.submit(self.application)
+        self._hook.submit(self._application)
 
     def on_kill(self) -> None:
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.on_kill()
 
     def _get_hook(self) -> SparkSubmitHook:
         return SparkSubmitHook(
-            conf=self.conf,
+            conf=self._conf,
             conn_id=self._conn_id,
-            files=self.files,
-            py_files=self.py_files,
+            files=self._files,
+            py_files=self._py_files,
             archives=self._archives,
-            driver_class_path=self.driver_class_path,
-            jars=self.jars,
+            driver_class_path=self._driver_class_path,
+            jars=self._jars,
             java_class=self._java_class,
-            packages=self.packages,
-            exclude_packages=self.exclude_packages,
+            packages=self._packages,
+            exclude_packages=self._exclude_packages,
             repositories=self._repositories,
             total_executor_cores=self._total_executor_cores,
             executor_cores=self._executor_cores,
             executor_memory=self._executor_memory,
             driver_memory=self._driver_memory,
-            keytab=self.keytab,
-            principal=self.principal,
-            proxy_user=self.proxy_user,
-            name=self.name,
+            keytab=self._keytab,
+            principal=self._principal,
+            proxy_user=self._proxy_user,
+            name=self._name,
             num_executors=self._num_executors,
             status_poll_interval=self._status_poll_interval,
-            application_args=self.application_args,
-            env_vars=self.env_vars,
+            application_args=self._application_args,
+            env_vars=self._env_vars,
             verbose=self._verbose,
             spark_binary=self._spark_binary,
-            properties_file=self.properties_file,
+            properties_file=self._properties_file,
             queue=self._queue,
             deploy_mode=self._deploy_mode,
             use_krb5ccache=self._use_krb5ccache,
         )
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/pyproject.toml` & `apache_airflow_providers_apache_spark-4.8.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-spark"
-version = "4.7.2.rc1"
+version = "4.8.0.rc1"
 description = "Provider package apache-airflow-providers-apache-spark for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,35 +47,34 @@
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
+    "apache-airflow>=2.6.0.dev0",
     "grpcio-status>=1.59.0",
     "pyspark",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
 provider_info = "airflow.providers.apache.spark.get_provider_info:get_provider_info"
 [project.optional-dependencies]
 "cncf.kubernetes" = [
-    "apache-airflow-providers-cncf-kubernetes>=7.4.0rc0",
+    "apache-airflow-providers-cncf-kubernetes>=7.4.0",
 ]
 
 [tool.flit.module]
 name = "airflow.providers.apache.spark"
```

### Comparing `apache_airflow_providers_apache_spark-4.7.2rc1/PKG-INFO` & `apache_airflow_providers_apache_spark-4.8.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.7.2rc1
+Version: 4.8.0rc1
 Summary: Provider package apache-airflow-providers-apache-spark for Apache Airflow
 Keywords: airflow-provider,apache.spark,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,23 +15,22 @@
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
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: grpcio-status>=1.59.0
 Requires-Dist: pyspark
-Requires-Dist: apache-airflow-providers-cncf-kubernetes>=7.4.0rc0 ; extra == "cncf.kubernetes"
+Requires-Dist: apache-airflow-providers-cncf-kubernetes>=7.4.0 ; extra == "cncf.kubernetes"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: cncf.kubernetes
 
 
@@ -74,37 +73,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.7.2.rc1``
+Release: ``4.8.0.rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -129,8 +128,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.7.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html>`_.
```

