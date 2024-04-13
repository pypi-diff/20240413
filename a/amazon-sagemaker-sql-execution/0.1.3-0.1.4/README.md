# Comparing `tmp/amazon-sagemaker-sql-execution-0.1.3.tar.gz` & `tmp/amazon_sagemaker_sql_execution-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-sagemaker-sql-execution-0.1.3.tar", last modified: Mon Mar 25 16:52:21 2024, max compression
+gzip compressed data, was "amazon_sagemaker_sql_execution-0.1.4.tar", last modified: Sat Apr 13 00:11:48 2024, max compression
```

## Comparing `amazon-sagemaker-sql-execution-0.1.3.tar` & `amazon_sagemaker_sql_execution-0.1.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.359685 amazon-sagemaker-sql-execution-0.1.3/
--rw-r--r--   0 shahvar    (504) staff       (20)    11386 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/LICENSE
--rw-r--r--   0 shahvar    (504) staff       (20)       21 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/MANIFEST.in
--rw-r--r--   0 shahvar    (504) staff       (20)    15242 2024-03-25 16:52:21.359436 amazon-sagemaker-sql-execution-0.1.3/PKG-INFO
--rw-r--r--   0 shahvar    (504) staff       (20)      233 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/README.md
--rw-r--r--   0 shahvar    (504) staff       (20)     1856 2024-03-23 01:52:56.000000 amazon-sagemaker-sql-execution-0.1.3/pyproject.toml
--rw-r--r--   0 shahvar    (504) staff       (20)       38 2024-03-25 16:52:21.359725 amazon-sagemaker-sql-execution-0.1.3/setup.cfg
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.348222 amazon-sagemaker-sql-execution-0.1.3/src/
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.350408 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/
--rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/__init__.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.351723 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/
--rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     3342 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/connection.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1031 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/connection_supplier.py
--rw-r--r--   0 shahvar    (504) staff       (20)     4246 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/models.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1330 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/connection.py
--rw-r--r--   0 shahvar    (504) staff       (20)     6973 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/connection_pool.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1014 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/exceptions.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.352167 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/models/
--rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/models/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     4567 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/models/sql_execution.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.352942 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/
--rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     5297 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/connection.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1053 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/connection_supplier.py
--rw-r--r--   0 shahvar    (504) staff       (20)     6035 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/models.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.353689 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/
--rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     4078 2024-03-23 01:50:53.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/connection.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1064 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/connection_supplier.py
--rw-r--r--   0 shahvar    (504) staff       (20)     4169 2024-03-23 01:50:53.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/models.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1219 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/sql_connection_supplier.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.355314 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/
--rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1348 2024-03-23 01:50:53.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/aws_secret_retriver.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1493 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/constants.py
--rw-r--r--   0 shahvar    (504) staff       (20)     3327 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/logging_utils.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.356211 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/
--rw-r--r--   0 shahvar    (504) staff       (20)     1508 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/BaseSQLFactory.py
--rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1273 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/connection_metadata_retriever.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1731 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/file_metadata_retriever.py
--rw-r--r--   0 shahvar    (504) staff       (20)     3644 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/glueconnection_metadata_retriever.py
--rw-r--r--   0 shahvar    (504) staff       (20)     1601 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/metadata_retriever_factory.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.357061 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/
--rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/__init__.py
--rw-r--r--   0 shahvar    (504) staff       (20)     2378 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/app_metadata.py
--rw-r--r--   0 shahvar    (504) staff       (20)      831 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/aws_config.py
--rw-r--r--   0 shahvar    (504) staff       (20)     9487 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/service_metrics.py
--rw-r--r--   0 shahvar    (504) staff       (20)      965 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/stack_trace_filter.py
--rw-r--r--   0 shahvar    (504) staff       (20)     2818 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/mixins.py
--rw-r--r--   0 shahvar    (504) staff       (20)     7739 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/sql_connection_factory.py
--rw-r--r--   0 shahvar    (504) staff       (20)      926 2024-03-22 17:24:08.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/sql_connection_supplier_factory.py
-drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-03-25 16:52:21.358109 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/
--rw-r--r--   0 shahvar    (504) staff       (20)    15242 2024-03-25 16:52:21.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/PKG-INFO
--rw-r--r--   0 shahvar    (504) staff       (20)     2676 2024-03-25 16:52:21.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/SOURCES.txt
--rw-r--r--   0 shahvar    (504) staff       (20)        1 2024-03-25 16:52:21.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/dependency_links.txt
--rw-r--r--   0 shahvar    (504) staff       (20)      545 2024-03-25 16:52:21.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/requires.txt
--rw-r--r--   0 shahvar    (504) staff       (20)       31 2024-03-25 16:52:21.000000 amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/top_level.txt
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.472214 amazon_sagemaker_sql_execution-0.1.4/
+-rw-r--r--   0 shahvar    (504) staff       (20)    11386 2024-03-26 23:24:59.000000 amazon_sagemaker_sql_execution-0.1.4/LICENSE
+-rw-r--r--   0 shahvar    (504) staff       (20)       21 2024-03-26 23:25:09.000000 amazon_sagemaker_sql_execution-0.1.4/MANIFEST.in
+-rw-r--r--   0 shahvar    (504) staff       (20)    15296 2024-04-13 00:11:48.472018 amazon_sagemaker_sql_execution-0.1.4/PKG-INFO
+-rw-r--r--   0 shahvar    (504) staff       (20)      233 2024-03-26 23:25:09.000000 amazon_sagemaker_sql_execution-0.1.4/README.md
+-rw-r--r--   0 shahvar    (504) staff       (20)     1902 2024-04-13 00:09:53.000000 amazon_sagemaker_sql_execution-0.1.4/pyproject.toml
+-rw-r--r--   0 shahvar    (504) staff       (20)       38 2024-04-13 00:11:48.472258 amazon_sagemaker_sql_execution-0.1.4/setup.cfg
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.461717 amazon_sagemaker_sql_execution-0.1.4/src/
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.463997 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/
+-rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/__init__.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.465727 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/
+-rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     3342 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/connection.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1031 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/connection_supplier.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     4246 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/models.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1330 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/connection.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     6973 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/connection_pool.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1014 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/exceptions.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.466163 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/models/
+-rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/models/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     4567 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/models/sql_execution.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.466889 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/
+-rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     5297 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/connection.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1053 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/connection_supplier.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     6035 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/models.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.467496 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/
+-rw-r--r--   0 shahvar    (504) staff       (20)      107 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     4078 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/connection.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1064 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/connection_supplier.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     4169 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/models.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1219 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/sql_connection_supplier.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.468755 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/
+-rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1348 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/aws_secret_retriver.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1493 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/constants.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     3327 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/logging_utils.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.469656 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/
+-rw-r--r--   0 shahvar    (504) staff       (20)     1508 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/BaseSQLFactory.py
+-rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1273 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/connection_metadata_retriever.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1731 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/file_metadata_retriever.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     3644 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/glueconnection_metadata_retriever.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     1601 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/metadata_retriever_factory.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.470488 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/
+-rw-r--r--   0 shahvar    (504) staff       (20)        0 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/__init__.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     2378 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/app_metadata.py
+-rw-r--r--   0 shahvar    (504) staff       (20)      831 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/aws_config.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     9487 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/service_metrics.py
+-rw-r--r--   0 shahvar    (504) staff       (20)      965 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/stack_trace_filter.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     2818 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/mixins.py
+-rw-r--r--   0 shahvar    (504) staff       (20)     7739 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/sql_connection_factory.py
+-rw-r--r--   0 shahvar    (504) staff       (20)      926 2024-03-26 23:25:12.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/sql_connection_supplier_factory.py
+drwxr-xr-x   0 shahvar    (504) staff       (20)        0 2024-04-13 00:11:48.470827 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/
+-rw-r--r--   0 shahvar    (504) staff       (20)    15296 2024-04-13 00:11:48.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/PKG-INFO
+-rw-r--r--   0 shahvar    (504) staff       (20)     2676 2024-04-13 00:11:48.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 shahvar    (504) staff       (20)        1 2024-04-13 00:11:48.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 shahvar    (504) staff       (20)      584 2024-04-13 00:11:48.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/requires.txt
+-rw-r--r--   0 shahvar    (504) staff       (20)       31 2024-04-13 00:11:48.000000 amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/top_level.txt
```

### Comparing `amazon-sagemaker-sql-execution-0.1.3/LICENSE` & `amazon_sagemaker_sql_execution-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/PKG-INFO` & `amazon_sagemaker_sql_execution-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-sql-execution
-Version: 0.1.3
+Version: 0.1.4
 Summary: SageMaker SQL Execution library
 Author: Amazon Web Services
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -217,14 +217,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.28.64
 Requires-Dist: pyathena<4,>=3.3.0
 Requires-Dist: redshift-connector<3,>=2.1.0
 Requires-Dist: aws_embedded_metrics<4,>=3.2.0
+Requires-Dist: snowflake-connector-python<4.0,>=3.8.1
 Requires-Dist: cryptography>=42.0.0
 Provides-Extra: all
 Requires-Dist: amazon-sagemaker-sql-execution[dev,flake8,pydocstyle,pylint,snowflake,test,twine]; extra == "all"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python<4.0,>=3.7.0; extra == "snowflake"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `amazon-sagemaker-sql-execution-0.1.3/pyproject.toml` & `amazon_sagemaker_sql_execution-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 61",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amazon-sagemaker-sql-execution"
-version = "0.1.3"
+version = "0.1.4"
 description = "SageMaker SQL Execution library"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 authors = [
     { name = "Amazon Web Services" },
 ]
@@ -27,14 +27,15 @@
 ]
 
 dependencies = [
     "boto3>=1.28.64",
     "pyathena>=3.3.0,<4",
     "redshift-connector>=2.1.0,<3",
     "aws_embedded_metrics>=3.2.0,<4",
+    "snowflake-connector-python>=3.8.1,<4.0",
     "cryptography>=42.0.0"
 ]
 
 [project.optional-dependencies]
 all = [
     "amazon-sagemaker-sql-execution[dev, test, flake8, pylint, pydocstyle, twine, snowflake]"
 ]
```

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/connection.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/connection.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/connection_supplier.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/connection_supplier.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/athena/models.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/athena/models.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/connection.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/connection.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/connection_pool.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/connection_pool.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/exceptions.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/models/sql_execution.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/models/sql_execution.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/connection.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/connection.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/connection_supplier.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/connection_supplier.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/redshift/models.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/redshift/models.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/connection.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/connection.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/connection_supplier.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/connection_supplier.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/snowflake/models.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/snowflake/models.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/sql_connection_supplier.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/sql_connection_supplier.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/aws_secret_retriver.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/aws_secret_retriver.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/constants.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/logging_utils.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/BaseSQLFactory.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/BaseSQLFactory.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/connection_metadata_retriever.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/connection_metadata_retriever.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/file_metadata_retriever.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/file_metadata_retriever.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/glueconnection_metadata_retriever.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/glueconnection_metadata_retriever.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/metadata_retriever_factory.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metadata_retriever/metadata_retriever_factory.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/app_metadata.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/aws_config.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/aws_config.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/service_metrics.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/service_metrics.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/metrics/stack_trace_filter.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/metrics/stack_trace_filter.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/mixins.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/sql_connection_factory.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/sql_connection_factory.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution/utils/sql_connection_supplier_factory.py` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution/utils/sql_connection_supplier_factory.py`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/PKG-INFO` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-sql-execution
-Version: 0.1.3
+Version: 0.1.4
 Summary: SageMaker SQL Execution library
 Author: Amazon Web Services
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -217,14 +217,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.28.64
 Requires-Dist: pyathena<4,>=3.3.0
 Requires-Dist: redshift-connector<3,>=2.1.0
 Requires-Dist: aws_embedded_metrics<4,>=3.2.0
+Requires-Dist: snowflake-connector-python<4.0,>=3.8.1
 Requires-Dist: cryptography>=42.0.0
 Provides-Extra: all
 Requires-Dist: amazon-sagemaker-sql-execution[dev,flake8,pydocstyle,pylint,snowflake,test,twine]; extra == "all"
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python<4.0,>=3.7.0; extra == "snowflake"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/SOURCES.txt` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-sagemaker-sql-execution-0.1.3/src/amazon_sagemaker_sql_execution.egg-info/requires.txt` & `amazon_sagemaker_sql_execution-0.1.4/src/amazon_sagemaker_sql_execution.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 boto3>=1.28.64
 pyathena<4,>=3.3.0
 redshift-connector<3,>=2.1.0
 aws_embedded_metrics<4,>=3.2.0
+snowflake-connector-python<4.0,>=3.8.1
 cryptography>=42.0.0
 
 [all]
 amazon-sagemaker-sql-execution[dev,flake8,pydocstyle,pylint,snowflake,test,twine]
 
 [dev]
 black
```

