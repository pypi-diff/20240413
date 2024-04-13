# Comparing `tmp/dbt-clickhouse-1.7.5.tar.gz` & `tmp/dbt-clickhouse-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.7.5.tar", last modified: Tue Apr  2 06:29:19 2024, max compression
+gzip compressed data, was "dbt-clickhouse-1.7.6.tar", last modified: Sat Apr 13 01:05:16 2024, max compression
```

## Comparing `dbt-clickhouse-1.7.5.tar` & `dbt-clickhouse-1.7.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22383 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/column_spec_ddl.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/dictionary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.228861 dbt-clickhouse-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.216861 dbt-clickhouse-1.7.6/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.220861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/column_spec_ddl.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/dictionary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/distributed_table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:05:16.224861 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-13 01:05:16.000000 dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:05:16.228861 dbt-clickhouse-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-13 01:05:11.000000 dbt-clickhouse-1.7.6/setup.py
```

### Comparing `dbt-clickhouse-1.7.5/LICENSE` & `dbt-clickhouse-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/PKG-INFO` & `dbt-clickhouse-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.5
+Version: 1.7.6
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -125,14 +125,15 @@
 | primary_key            | Like order_by, a ClickHouse primary key expression.  If not specified, ClickHouse will use the order by expression as the primary key                                                                                                                  |                |
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        |                |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way |                |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | `default`      |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |                |
 | settings               | A map/dictionary of "TABLE" settings to be used to DDL statements like 'CREATE TABLE' with this model                                                                                                                                                  |                |
 | query_settings         | A map/dictionary of ClickHouse user level settings to be used with `INSERT` or `DELETE` statements in conjunction with this model                                                                                                                      |                |
+| ttl                    | A TTL expression to be used with the table.  The TTL expression is a string that can be used to specify the TTL for the table.                                                                                                                         |                |
 
 ## ClickHouse Cluster 
 
 The `cluster` setting in profile enables dbt-clickhouse to run against a ClickHouse cluster.
 
 ### Effective Scope
 
@@ -202,14 +203,15 @@
 
 The following macros are included to facilitate creating ClickHouse specific tables and views:
 - `engine_clause` -- Uses the `engine` model configuration property to assign a ClickHouse table engine.  dbt-clickhouse uses the `MergeTree` engine by default.
 - `partition_cols` -- Uses the `partition_by` model configuration property to assign a ClickHouse partition key.  No partition key is assigned by default.
 - `order_cols` -- Uses the `order_by` model configuration to assign a ClickHouse order by/sorting key.  If not specified ClickHouse will use an empty tuple() and the table will be unsorted
 - `primary_key_clause` -- Uses the `primary_key` model configuration property to assign a ClickHouse primary key.  By default, primary key is set and ClickHouse will use the order by clause as the primary key. 
 - `on_cluster_clause` -- Uses the `cluster` profile property to add an `ON CLUSTER` clause to certain dbt-operations: distributed materializations, views creation, database creation.
+- `ttl_config` -- Uses the `ttl` model configuration property to assign a ClickHouse table TTL expression.  No TTL is assigned by default.
 
 ### s3Source Helper Macro
 
 The `s3source` macro simplifies the process of selecting ClickHouse data directly from S3 using the ClickHouse S3 table function.  It works by
 populating the S3 table function parameters from a named configuration dictionary (the name of the dictionary must end in `s3`).  The macro
 first looks for the dictionary in the profile `vars`, and then in the model configuration.  The dictionary can contain any of the following
 keys used to populate the parameters of the S3 table function:
```

### Comparing `dbt-clickhouse-1.7.5/README.md` & `dbt-clickhouse-1.7.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 | primary_key            | Like order_by, a ClickHouse primary key expression.  If not specified, ClickHouse will use the order by expression as the primary key                                                                                                                  |                |
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        |                |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way |                |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | `default`      |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |                |
 | settings               | A map/dictionary of "TABLE" settings to be used to DDL statements like 'CREATE TABLE' with this model                                                                                                                                                  |                |
 | query_settings         | A map/dictionary of ClickHouse user level settings to be used with `INSERT` or `DELETE` statements in conjunction with this model                                                                                                                      |                |
+| ttl                    | A TTL expression to be used with the table.  The TTL expression is a string that can be used to specify the TTL for the table.                                                                                                                         |                |
 
 ## ClickHouse Cluster 
 
 The `cluster` setting in profile enables dbt-clickhouse to run against a ClickHouse cluster.
 
 ### Effective Scope
 
@@ -175,14 +176,15 @@
 
 The following macros are included to facilitate creating ClickHouse specific tables and views:
 - `engine_clause` -- Uses the `engine` model configuration property to assign a ClickHouse table engine.  dbt-clickhouse uses the `MergeTree` engine by default.
 - `partition_cols` -- Uses the `partition_by` model configuration property to assign a ClickHouse partition key.  No partition key is assigned by default.
 - `order_cols` -- Uses the `order_by` model configuration to assign a ClickHouse order by/sorting key.  If not specified ClickHouse will use an empty tuple() and the table will be unsorted
 - `primary_key_clause` -- Uses the `primary_key` model configuration property to assign a ClickHouse primary key.  By default, primary key is set and ClickHouse will use the order by clause as the primary key. 
 - `on_cluster_clause` -- Uses the `cluster` profile property to add an `ON CLUSTER` clause to certain dbt-operations: distributed materializations, views creation, database creation.
+- `ttl_config` -- Uses the `ttl` model configuration property to assign a ClickHouse table TTL expression.  No TTL is assigned by default.
 
 ### s3Source Helper Macro
 
 The `s3source` macro simplifies the process of selecting ClickHouse data directly from S3 using the ClickHouse S3 table function.  It works by
 populating the S3 table function parameters from a named configuration dictionary (the name of the dictionary must end in `s3`).  The macro
 first looks for the dictionary in the profile `vars`, and then in the model configuration.  The dictionary can contain any of the following
 keys used to populate the parameters of the S3 table function:
```

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__init__.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/cache.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/column.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/connections.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import re
 import time
 from contextlib import contextmanager
-from typing import Any, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
 
-import agate
 import dbt.exceptions
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse, Connection
 
 from dbt.adapters.clickhouse.dbclient import ChRetryableException, get_db_client
 from dbt.adapters.clickhouse.logger import logger
 
+if TYPE_CHECKING:
+    import agate
+
 retryable_exceptions = [ChRetryableException]
 ddl_re = re.compile(r'^\s*(CREATE|DROP|ALTER)\s', re.IGNORECASE)
 
 
 class ClickHouseConnectionManager(SQLConnectionManager):
     """
     ClickHouse Connector connection manager.
@@ -56,29 +58,31 @@
         connection.handle.close()
         logger.debug('Cancel query \'{}\'', connection_name)
 
     def release(self):
         pass  # There is no "release" type functionality in the existing ClickHouse connectors
 
     @classmethod
-    def get_table_from_response(cls, response, column_names) -> agate.Table:
+    def get_table_from_response(cls, response, column_names) -> "agate.Table":
         """
         Build agate table from response.
         :param response: ClickHouse query result
         :param column_names: Table column names
         """
+        from dbt.clients.agate_helper import table_from_data_flat
+
         data = []
         for row in response:
             data.append(dict(zip(column_names, row)))
 
-        return dbt.clients.agate_helper.table_from_data_flat(data, column_names)
+        return table_from_data_flat(data, column_names)
 
     def execute(
         self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
         # Don't try to fetch result of clustered DDL responses, we don't know what to do with them
         if fetch and ddl_re.match(sql):
             fetch = False
 
         sql = self._add_query_comment(sql)
         conn = self.get_thread_connection()
         client = conn.handle
@@ -93,15 +97,17 @@
             status = self.get_status(client)
             logger.debug(f'SQL status: {status} in {(time.time() - pre):.2f} seconds')
             if fetch:
                 table = self.get_table_from_response(
                     query_result.result_set, query_result.column_names
                 )
             else:
-                table = dbt.clients.agate_helper.empty_table()
+                from dbt.clients.agate_helper import empty_table
+
+                table = empty_table()
             return AdapterResponse(_message=status), table
 
     def add_query(
         self,
         sql: str,
         auto_begin: bool = True,
         bindings: Optional[Any] = None,
```

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/credentials.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/dbclient.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/dbclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/errors.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/errors.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/httpclient.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/httpclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,18 @@
         try:
             return self._client.command(sql, **kwargs)
         except DatabaseError as ex:
             raise DbtDatabaseError(str(ex).strip()) from ex
 
     def columns_in_query(self, sql: str, **kwargs) -> List[ClickHouseColumn]:
         try:
-            query_result = self._client.query(f"SELECT * FROM ({sql}) LIMIT 0", **kwargs)
+            query_result = self._client.query(
+                f"SELECT * FROM ( \n" f"{sql} \n" f") LIMIT 0",
+                **kwargs,
+            )
             return [
                 ClickHouseColumn.create(name, ch_type.name)
                 for name, ch_type in zip(query_result.column_names, query_result.column_types)
             ]
         except DatabaseError as ex:
             raise DbtDatabaseError(str(ex).strip()) from ex
```

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/impl.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/impl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 import io
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-import agate
 from dbt.adapters.base import AdapterConfig, available
 from dbt.adapters.base.impl import BaseAdapter, ConstraintSupport
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.capability import Capability, CapabilityDict, CapabilitySupport, Support
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import ConstraintType, ModelLevelConstraint
@@ -27,24 +26,28 @@
     schema_change_missing_source_error,
 )
 from dbt.adapters.clickhouse.logger import logger
 from dbt.adapters.clickhouse.query import quote_identifier
 from dbt.adapters.clickhouse.relation import ClickHouseRelation, ClickHouseRelationType
 from dbt.adapters.clickhouse.util import NewColumnDataType, compare_versions
 
+if TYPE_CHECKING:
+    import agate
+
 GET_CATALOG_MACRO_NAME = 'get_catalog'
 LIST_SCHEMAS_MACRO_NAME = 'list_schemas'
 
 
 @dataclass
 class ClickHouseConfig(AdapterConfig):
     engine: str = 'MergeTree()'
     order_by: Optional[Union[List[str], str]] = 'tuple()'
     partition_by: Optional[Union[List[str], str]] = None
     sharding_key: Optional[Union[List[str], str]] = 'rand()'
+    ttl: Optional[Union[List[str], str]] = None
 
 
 class ClickHouseAdapter(SQLAdapter):
     Relation = ClickHouseRelation
     Column = ClickHouseColumn
     ConnectionManager = ClickHouseConnectionManager
     AdapterSpecificConfigs = ClickHouseConfig
@@ -69,37 +72,39 @@
         self.cache = ClickHouseRelationsCache()
 
     @classmethod
     def date_function(cls):
         return 'now()'
 
     @classmethod
-    def convert_text_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_text_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return 'String'
 
     @classmethod
-    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_number_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
+        import agate
+
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
         # We match these type to the Column.TYPE_LABELS for consistency
         return 'Float32' if decimals else 'Int32'
 
     @classmethod
-    def convert_boolean_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_boolean_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return 'Bool'
 
     @classmethod
-    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_datetime_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return 'DateTime'
 
     @classmethod
-    def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_date_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return 'Date'
 
     @classmethod
-    def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_time_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         raise NotImplementedError('`convert_time_type` is not implemented for this adapter!')
 
     @available.parse(lambda *a, **k: {})
     def get_clickhouse_cluster_name(self):
         conn = self.connections.get_if_exists()
         if conn.credentials.cluster:
             return f'"{conn.credentials.cluster}"'
@@ -304,31 +309,33 @@
             results = self.execute_macro('clickhouse__get_database', kwargs={'database': schema})
             if len(results.rows):
                 return ClickHouseDatabase(**results.rows[0])
             return None
         except DbtRuntimeError:
             return None
 
-    def get_catalog(self, manifest) -> Tuple[agate.Table, List[Exception]]:
+    def get_catalog(self, manifest) -> Tuple["agate.Table", List[Exception]]:
+        from dbt.clients.agate_helper import empty_table
+
         relations = self._get_catalog_relations(manifest)
         schemas = set(relation.schema for relation in relations)
         if schemas:
             catalog = self._get_one_catalog(InformationSchema(Path()), schemas, manifest)
         else:
-            catalog = dbt.clients.agate_helper.empty_table()
+            catalog = empty_table()
         return catalog, []
 
     def get_filtered_catalog(
         self, manifest: Manifest, relations: Optional[Set[BaseRelation]] = None
     ):
         catalog, exceptions = self.get_catalog(manifest)
         if relations and catalog:
             relation_map = {(r.schema, r.identifier) for r in relations}
 
-            def in_map(row: agate.Row):
+            def in_map(row: "agate.Row"):
                 s = _expect_row_value("table_schema", row)
                 i = _expect_row_value("table_name", row)
                 return (s, i) in relation_map
 
             catalog = catalog.where(in_map)
         return catalog, exceptions
 
@@ -447,25 +454,32 @@
         return conn.handle.columns_in_query(sql)
 
     @available.parse_none
     def format_columns(self, columns) -> List[Dict]:
         return [{'name': column.name, 'data_type': column.dtype} for column in columns]
 
     @available
-    def get_credentials(self) -> Dict:
+    def get_credentials(self, connection_overrides) -> Dict:
         conn = self.connections.get_if_exists()
         if conn is None or conn.credentials is None:
             return dict()
-        return {
+        credentials = {
             'user': conn.credentials.user,
             'password': conn.credentials.password,
             'database': conn.credentials.database,
             'host': conn.credentials.host,
             'port': conn.credentials.port,
         }
+        credentials.update(connection_overrides)
+
+        for key in connection_overrides.keys():
+            if not credentials[key]:
+                credentials.pop(key)
+
+        return credentials
 
     @classmethod
     def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
         rendered_columns = []
         for v in raw_columns.values():
             rendered_columns.append(f"{quote_identifier(v['name'])} {v['data_type']}")
             if v.get("constraints"):
@@ -484,25 +498,25 @@
 @dataclass
 class ClickHouseDatabase:
     name: str
     engine: str
     comment: str
 
 
-def _expect_row_value(key: str, row: agate.Row):
+def _expect_row_value(key: str, row: "agate.Row"):
     if key not in row.keys():
         raise DbtInternalError(f'Got a row without \'{key}\' column, columns: {row.keys()}')
 
     return row[key]
 
 
-def _catalog_filter_schemas(manifest: Manifest) -> Callable[[agate.Row], bool]:
+def _catalog_filter_schemas(manifest: Manifest) -> Callable[["agate.Row"], bool]:
     schemas = frozenset((None, s) for d, s in manifest.get_used_schemas())
 
-    def test(row: agate.Row) -> bool:
+    def test(row: "agate.Row") -> bool:
         table_database = _expect_row_value('table_database', row)
         table_schema = _expect_row_value('table_schema', row)
         if table_schema is None:
             return False
         return (table_database, table_schema) in schemas
 
     return test
```

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/nativeclient.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/nativeclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
                 return result[0][0]
         except clickhouse_driver.errors.Error as ex:
             raise DbtDatabaseError(str(ex).strip()) from ex
 
     def columns_in_query(self, sql: str, **kwargs) -> List[ClickHouseColumn]:
         try:
             _, columns = self._client.execute(
-                f"SELECT * FROM ({sql}) LIMIT 0", with_column_types=True
+                f"SELECT * FROM ( \n" f"{sql} \n" f") LIMIT 0",
+                with_column_types=True,
             )
             return [ClickHouseColumn.create(column[0], column[1]) for column in columns]
         except clickhouse_driver.errors.Error as ex:
             raise DbtDatabaseError(str(ex).strip()) from ex
 
     def get_ch_setting(self, setting_name):
         try:
```

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/relation.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/util.py` & `dbt-clickhouse-1.7.6/dbt/adapters/clickhouse/util.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/catalog.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/column_spec_ddl.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/column_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/dictionary.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/dictionary.sql`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 {% macro http_source() %}
   HTTP(URL '{{ config.get("url") }}' FORMAT '{{ config.get("format") }}')
 {% endmacro %}
 
 
 {% macro clickhouse_source(sql) %}
-  {%- set credentials = adapter.get_credentials() -%}
+  {%- set credentials = adapter.get_credentials(config.get("connection_overrides", {})) -%}
   {%- set table = config.get('table') -%}
   CLICKHOUSE(
       user '{{ credentials.get("user") }}'
       {% if credentials.get("password") != '' -%}
       password '{{ credentials.get("password") }}'
       {%- endif %}
       {% if credentials.get("database") != '' -%}
```

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/distributed_table.sql`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
       {{ create_empty_table_from_relation(backup_relation, view_relation) }}
     {%- endcall %}
     {% do exchange_tables_atomic(backup_relation, existing_relation_local) %}
   {% else %}
     {% do run_query(create_empty_table_from_relation(intermediate_relation, view_relation)) or '' %}
     {{ adapter.rename_relation(existing_relation_local, backup_relation) }}
     {{ adapter.rename_relation(intermediate_relation, target_relation_local) }}
-    {{ create_distributed_table(target_relation, target_relation_local) }}
-  {% endif %}
+  {% endif %}  
+    {% do run_query(create_distributed_table(target_relation, target_relation_local)) or '' %}
   {% do run_query(clickhouse__insert_into(target_relation, sql)) or '' %}
   {{ drop_relation_if_exists(view_relation) }}
   -- cleanup
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation_local, grant_config, should_revoke=should_revoke) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
@@ -81,39 +81,40 @@
    {% if cluster is none %}
         {% do exceptions.raise_compiler_error('Cluster name should be defined for using distributed materializations, current is None') %}
     {% endif %}
 
    {%- set cluster = cluster[1:-1] -%}
    {%- set sharding = config.get('sharding_key') -%}
 
-    create table {{ relation }} {{ on_cluster_clause(relation) }} as {{ local_relation }}
+    create or replace table {{ relation }} {{ on_cluster_clause(relation) }} as {{ local_relation }}
     ENGINE = Distributed('{{ cluster}}', '{{ relation.schema }}', '{{ local_relation.name }}'
     {%- if sharding is not none and sharding.strip() != '' -%}
         , {{ sharding }}
     {%- else %}
         , rand()
     {% endif -%}
     )
  {% endmacro %}
 
 {% macro create_empty_table_from_relation(relation, source_relation) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
   {%- set columns = adapter.get_columns_in_relation(source_relation) | list -%}
+   
 
   {%- set col_list = [] -%}
   {% for col in columns %}
     {{col_list.append(col.name + ' ' + col.data_type) or '' }}
   {% endfor %}
   {{ sql_header if sql_header is not none }}
 
   create table {{ relation.include(database=False) }}
   {{ on_cluster_clause(relation) }} (
       {{col_list | join(', ')}}
   )
-
+  
   {{ engine_clause() }}
   {{ order_cols(label="order by") }}
   {{ primary_key_clause(label="primary key") }}
   {{ partition_cols(label="partition by") }}
   {{ adapter.get_model_settings(model) }}
 {%- endmacro %}
```

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/materialized_view.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,20 @@
       )
     {%- else %}
       {{ label }} (tuple())
     {%- endif %}
   {%- endif %}
 {%- endmacro -%}
 
+{% macro ttl_config(label) %}
+  {%- if config.get("ttl")%}
+    {{ label }} {{ config.get("ttl") }}
+  {%- endif %}
+{%- endmacro -%}
+
 {% macro on_cluster_clause(relation, force_sync) %}
   {% set active_cluster = adapter.get_clickhouse_cluster_name() %}
   {%- if active_cluster is not none and relation.should_on_cluster %}
     {# Add trailing whitespace to avoid problems when this clause is not last #}
     ON CLUSTER {{ active_cluster + ' ' }}
     {%- if force_sync %}
     SYNC
@@ -166,14 +172,15 @@
           {{ get_assert_columns_equivalent(sql) }}
           {{ get_table_columns_and_constraints() }}
         {%- endif %}
         {{ engine_clause() }}
         {{ order_cols(label="order by") }}
         {{ primary_key_clause(label="primary key") }}
         {{ partition_cols(label="partition by") }}
+        {{ ttl_config(label="ttl")}}
         {{ adapter.get_model_settings(model) }}
 
         {%- if not has_contract %}
           {%- if not adapter.is_before_version('22.7.1.2484') %}
             empty
           {%- endif %}
           as (
```

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt-clickhouse-1.7.6/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/PKG-INFO` & `dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.5
+Version: 1.7.6
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -125,14 +125,15 @@
 | primary_key            | Like order_by, a ClickHouse primary key expression.  If not specified, ClickHouse will use the order by expression as the primary key                                                                                                                  |                |
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        |                |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way |                |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | `default`      |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |                |
 | settings               | A map/dictionary of "TABLE" settings to be used to DDL statements like 'CREATE TABLE' with this model                                                                                                                                                  |                |
 | query_settings         | A map/dictionary of ClickHouse user level settings to be used with `INSERT` or `DELETE` statements in conjunction with this model                                                                                                                      |                |
+| ttl                    | A TTL expression to be used with the table.  The TTL expression is a string that can be used to specify the TTL for the table.                                                                                                                         |                |
 
 ## ClickHouse Cluster 
 
 The `cluster` setting in profile enables dbt-clickhouse to run against a ClickHouse cluster.
 
 ### Effective Scope
 
@@ -202,14 +203,15 @@
 
 The following macros are included to facilitate creating ClickHouse specific tables and views:
 - `engine_clause` -- Uses the `engine` model configuration property to assign a ClickHouse table engine.  dbt-clickhouse uses the `MergeTree` engine by default.
 - `partition_cols` -- Uses the `partition_by` model configuration property to assign a ClickHouse partition key.  No partition key is assigned by default.
 - `order_cols` -- Uses the `order_by` model configuration to assign a ClickHouse order by/sorting key.  If not specified ClickHouse will use an empty tuple() and the table will be unsorted
 - `primary_key_clause` -- Uses the `primary_key` model configuration property to assign a ClickHouse primary key.  By default, primary key is set and ClickHouse will use the order by clause as the primary key. 
 - `on_cluster_clause` -- Uses the `cluster` profile property to add an `ON CLUSTER` clause to certain dbt-operations: distributed materializations, views creation, database creation.
+- `ttl_config` -- Uses the `ttl` model configuration property to assign a ClickHouse table TTL expression.  No TTL is assigned by default.
 
 ### s3Source Helper Macro
 
 The `s3source` macro simplifies the process of selecting ClickHouse data directly from S3 using the ClickHouse S3 table function.  It works by
 populating the S3 table function parameters from a named configuration dictionary (the name of the dictionary must end in `s3`).  The macro
 first looks for the dictionary in the profile `vars`, and then in the model configuration.  The dictionary can contain any of the following
 keys used to populate the parameters of the S3 table function:
```

### Comparing `dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt-clickhouse-1.7.6/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.5/setup.py` & `dbt-clickhouse-1.7.6/setup.py`

 * *Files identical despite different names*

