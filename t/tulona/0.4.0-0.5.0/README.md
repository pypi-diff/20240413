# Comparing `tmp/tulona-0.4.0.tar.gz` & `tmp/tulona-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.4.0.tar", last modified: Fri Apr 12 06:52:13 2024, max compression
+gzip compressed data, was "tulona-0.5.0.tar", last modified: Sat Apr 13 15:02:06 2024, max compression
```

## Comparing `tulona-0.4.0.tar` & `tulona-0.5.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-12 06:52:03.000000 tulona-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-12 06:52:13.308987 tulona-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-12 06:52:03.000000 tulona-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.300987 tulona-0.4.0/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.300987 tulona-0.4.0/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-12 06:52:03.000000 tulona-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:52:13.308987 tulona-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.711878 tulona-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-13 15:02:01.000000 tulona-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-13 15:02:06.711878 tulona-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-13 15:02:01.000000 tulona-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.703878 tulona-0.5.0/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.707877 tulona-0.5.0/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.707877 tulona-0.5.0/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.707877 tulona-0.5.0/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.707877 tulona-0.5.0/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.711878 tulona-0.5.0/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.711878 tulona-0.5.0/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.711878 tulona-0.5.0/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-13 15:02:01.000000 tulona-0.5.0/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:02:06.711878 tulona-0.5.0/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 15:02:06.000000 tulona-0.5.0/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-13 15:02:01.000000 tulona-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:02:06.711878 tulona-0.5.0/setup.cfg
```

### Comparing `tulona-0.4.0/LICENSE` & `tulona-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/PKG-INFO` & `tulona-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.4.0/README.rst` & `tulona-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/adapter/connection.py` & `tulona-0.5.0/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/adapter/mssql.py` & `tulona-0.5.0/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/adapter/mysql.py` & `tulona-0.5.0/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/adapter/postgres.py` & `tulona-0.5.0/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/adapter/snowflake.py` & `tulona-0.5.0/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/cli/base.py` & `tulona-0.5.0/core/tulona/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 # command: tulona compare-column
 @cli.command("compare-column")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
+@p.composite
 def compare_column(ctx, **kwargs):
     """
     Column name must be specified for task: compare-column
     by specifying 'compare_column' property in
     all the datasource[project] configs
     (check sample tulona-project.yml file for example)
     """
@@ -234,26 +235,28 @@
 
         task = CompareColumnTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
+            composite=kwargs["composite"],
         )
         task.execute()
 
 
 # command: tulona compare
 @cli.command("compare")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 @p.sample_count
+@p.composite
 def compare(ctx, **kwargs):
     """
     Compare everything(profiles, rows and columns) for the given datasoures
     """
 
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
@@ -293,13 +296,14 @@
         task = CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
             runtime=ctx.obj["runtime"],
             datasources=datasource_list,
             outfile_fqn=outfile_fqn,
             sample_count=kwargs["sample_count"],
+            composite=kwargs["composite"],
         )
         task.execute()
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `tulona-0.4.0/core/tulona/cli/params.py` & `tulona-0.5.0/core/tulona/cli/params.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,7 +22,14 @@
 )
 
 compare = click.option(
     "--compare",
     is_flag=True,
     help="Can be used with profile task to compare profiles of different data sources",
 )
+
+composite = click.option(
+    "--composite",
+    is_flag=True,
+    help="Used with compare-column task to indicate if all columns are to be combined"
+    "for comparison. For example, ds1:column1-column2 vs ds2:column1-column2",
+)
```

### Comparing `tulona-0.4.0/core/tulona/config/profile.py` & `tulona-0.5.0/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/config/project.py` & `tulona-0.5.0/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/exceptions.py` & `tulona-0.5.0/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/task/base.py` & `tulona-0.5.0/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/task/compare.py` & `tulona-0.5.0/core/tulona/task/compare.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     get_table_fqn,
 )
 
 log = logging.getLogger(__name__)
 
 DEFAULT_VALUES = {
     "sample_count": 20,
+    "compare_column_composite": False,
 }
 
 
 @dataclass
 class CompareDataTask(BaseTask):
     profile: Dict
     project: Dict
@@ -55,15 +56,14 @@
         start_time = time.time()
 
         if len(self.datasources) != 2:
             raise ValueError("Data comparison needs two data sources.")
 
         log.info(f"Comparing {self.datasources}")
 
-        # TODO: Add support of composite primary key
         # TODO: Add support for different names of primary keys in different tables
         # Check if primary key[s] is[are] specified for row comparison
         primary_keys = set()
         ds_names = []
         ds_name_compressed_list = []
         ds_configs = []
         dbtypes = []
@@ -111,40 +111,39 @@
                 ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
             )
             if isinstance(exclude_columns, str):
                 exclude_columns = [exclude_columns]
             exclude_columns_lol.append(exclude_columns)
 
             if "primary_key" in ds_config:
-                if (
-                    isinstance(ds_config["primary_key"], list)
-                    and len(ds_config["primary_key"]) > 1
-                ):
-                    raise ValueError("Composite primary key is not supported yet")
-                primary_keys = primary_keys.union({ds_config["primary_key"]})
+                primary_keys.add(
+                    (ds_config["primary_key"],)
+                    if isinstance(ds_config["primary_key"], str)
+                    else tuple(sorted(ds_config["primary_key"]))
+                )
 
         if len(primary_keys) == 0:
             raise TulonaMissingPrimaryKeyError(
-                "Primary key must be provided with at least one of the data source config"
+                "Primary key must be provided for comparison"
             )
 
         if len(primary_keys) > 1:
             raise ValueError(
-                "Primary key column name has to be same in all candidate tables for comparison"
+                "Primary key must be same in all candidate tables for comparison"
             )
         primary_key = primary_keys.pop()
 
         # Config extraction
         dbtype1, dbtype2 = dbtypes
         table_fqn1, table_fqn2 = table_fqns
         conman1, conman2 = connection_managers
         exclude_columns1, exclude_columns2 = exclude_columns_lol
 
         # TODO: push column exclusion down to the database/query
-        primary_key = primary_key.lower()
+        primary_key = tuple([k.lower() for k in primary_key])
         query_expr = None
 
         i = 0
         while i < 5:
             log.debug(f"Extraction iteration: {i + 1}/5")
 
             query1 = get_table_data_query(
@@ -153,16 +152,17 @@
             if self.sample_count < 51:
                 log.debug(f"Executing query: {query1}")
             df1 = get_query_output_as_df(connection_manager=conman1, query_text=query1)
             if df1.shape[0] == 0:
                 raise ValueError(f"Table {table_fqn1} doesn't have any data")
 
             df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
-            if primary_key not in df1.columns.tolist():
-                raise ValueError(f"Primary key {primary_key} not present in {table_fqn2}")
+            for k in primary_key:
+                if k not in df1.columns.tolist():
+                    raise ValueError(f"Primary key {k} not present in {table_fqn1}")
 
             # Exclude columns
             log.debug(f"Excluding columns from {table_fqn1}")
             if len(exclude_columns1):
                 df1 = apply_column_exclusion(
                     df1, primary_key, exclude_columns1, table_fqn1
                 )
@@ -171,29 +171,32 @@
                 dbtype2,
                 table_fqn2,
                 self.sample_count,
                 query_expr=build_filter_query_expression(df1, primary_key),
             )
             if self.sample_count < 51:
                 log.debug(f"Executing query: {query2}")
+
             df2 = get_query_output_as_df(connection_manager=conman2, query_text=query2)
             df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
 
-            if primary_key not in df2.columns.tolist():
-                raise ValueError(f"Primary key {primary_key} not present in {table_fqn2}")
+            for k in primary_key:
+                if k not in df2.columns.tolist():
+                    raise ValueError(f"Primary key {k} not present in {table_fqn2}")
 
             # Exclude columns
             log.debug(f"Excluding columns from {table_fqn2}")
             if len(exclude_columns2):
                 df2 = apply_column_exclusion(
                     df2, primary_key, exclude_columns2, table_fqn2
                 )
 
             if df2.shape[0] > 0:
-                df1 = df1[df1[primary_key].isin(df2[primary_key].tolist())]
+                for k in primary_key:
+                    df1 = df1[df1[k].isin(df2[k].tolist())]
                 row_data_list = [df1, df2]
                 break
             else:
                 query_expr = build_filter_query_expression(
                     df1, primary_key, positive=False
                 )
 
@@ -202,19 +205,27 @@
         if df2.shape[0] == 0:
             raise ValueError(
                 f"Could not find common data between {table_fqn1} and {table_fqn2}"
             )
 
         log.debug("Preparing row comparison")
         df_row_comp = perform_comparison(
-            ds_name_compressed_list, row_data_list, primary_key
+            ds_compressed_names=ds_name_compressed_list,
+            dataframes=row_data_list,
+            on=primary_key,
         )
         log.debug(f"Prepared comparison for {df_row_comp.shape[0]} rows")
 
         log.debug(f"Writing comparison result into: {self.outfile_fqn}")
+        # Moving key columns to the beginning
+        new_columns = list(primary_key) + [
+            col for col in df_row_comp if col not in primary_key
+        ]
+        df_row_comp = df_row_comp[new_columns]
+
         _ = create_dir_if_not_exist(self.project["outdir"])
         with pd.ExcelWriter(
             self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
         ) as writer:
             df_row_comp.to_excel(writer, sheet_name="Row Comparison", index=False)
 
         log.debug("Highlighting mismtach cells")
@@ -233,31 +244,15 @@
 @dataclass
 class CompareColumnTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
-
-    def get_column_data(self, datasource, table, column):
-        connection_profile = get_connection_profile(
-            self.profile, self.project, datasource
-        )
-        conman = self.get_connection_manager(conn_profile=connection_profile)
-
-        query = get_column_query(table, column)
-        try:
-            log.debug(f"Trying unquoted column name: {column}")
-            df = get_query_output_as_df(connection_manager=conman, query_text=query)
-        except Exception as exp:
-            log.debug(f"Failed with error: {exp}")
-            log.debug(f'Trying quoted column name: "{column}"')
-            query = get_column_query(table, column, quoted=True)
-            df = get_query_output_as_df(connection_manager=conman, query_text=query)
-        return df
+    composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     def execute(self):
         log.info("------------------------ Starting task: compare-column")
         start_time = time.time()
 
         if len(self.datasources) != 2:
             raise ValueError("Comparison works between two entities, not more, not less.")
@@ -267,21 +262,22 @@
         column_df_list = []
         for ds_name in self.datasources:
             log.info(f"Processing data source {ds_name}")
             ds_compressed_names.append(ds_name.replace("_", ""))
             ds_config = self.project["datasources"][ds_name]
 
             if "compare_column" in ds_config:
-                column = ds_config["compare_column"]
-                compare_columns.append(column)
+                columns = ds_config["compare_column"]
+                columns = [columns] if isinstance(columns, str) else columns
+                compare_columns.append(columns)
             else:
                 raise TulonaMissingPropertyError(
-                    "Property 'compare_column' must be specified for column comparison"
+                    "Property 'compare_column' must be specified"
+                    "in tulona-project.yml for column comparison"
                 )
-            log.debug(f"Extracting data for column {column}")
 
             dbtype = self.profile["profiles"][
                 extract_profile_name(self.project, ds_name)
             ]["type"]
             log.debug(f"Database type: {dbtype}")
 
             # MySQL doesn't have logical database
@@ -290,82 +286,122 @@
             else:
                 database = None
             schema = ds_config["schema"]
             table = ds_config["table"]
             table_fqn = get_table_fqn(database, schema, table)
             log.debug(f"Table FQN: {table_fqn}")
 
+            log.debug(f"Extracting data for column {columns}")
             log.debug(f"Acquiring connection to the database of: {ds_name}")
             connection_profile = get_connection_profile(
                 self.profile, self.project, ds_name
             )
             conman = self.get_connection_manager(conn_profile=connection_profile)
 
-            query = get_column_query(table_fqn, column)
+            query = get_column_query(table_fqn, columns)
             try:
-                log.debug(f"Trying unquoted column name: {column}")
+                log.debug(f"Trying unquoted column names: {columns}")
                 log.debug(f"Executing query: {query}")
                 df = get_query_output_as_df(connection_manager=conman, query_text=query)
             except Exception as exp:
                 log.warning(f"Failed with error: {exp}")
-                log.debug(f'Trying quoted column name: "{column}"')
-                query = get_column_query(table_fqn, column, quoted=True)
+                log.debug(f'Trying quoted column names: "{columns}"')
+                query = get_column_query(table_fqn, columns, quoted=True)
                 log.debug(f"Executing query: {query}")
                 df = get_query_output_as_df(connection_manager=conman, query_text=query)
 
             if df.shape[0] == 0:
                 raise ValueError(f"Table {table_fqn} doesn't have any data")
 
             log.debug(f"Found {df.shape[0]} records in {table_fqn}")
 
             df = df.rename(columns={c: c.lower() for c in df.columns})
             column_df_list.append(df)
 
-        compare_columns = {c.lower() for c in compare_columns}
+        compare_columns = {
+            tuple(map(lambda c: c.lower(), clist)) for clist in compare_columns
+        }
         if len(compare_columns) > 1:
             raise ValueError(
-                "Column comparison works only when the column name is same for both data source"
+                "Column comparison works only when the column name is same for all data sources"
                 "(not case sensitive)"
+                "and they have to be specified in the same order"
+                "in the config file for all data sources"
             )
+        compare_columns = compare_columns.pop()
+        log.debug(f"Final list of columns for comparison: {compare_columns}")
 
-        log.debug("Perform comparison")
-        df_comp = perform_comparison(
-            ds_compressed_names=ds_compressed_names,
-            dataframes=column_df_list,
-            on=compare_columns.pop(),
-            how="outer",
-            indicator="presence",
-            validate="one_to_one",
-        )
-        df_comp = df_comp[df_comp["presence"] != "both"]
-        df_comp["presence"] = df_comp["presence"].map(
-            {"left_only": ds_compressed_names[0], "right_only": ds_compressed_names[1]}
-        )
-        log.debug(f"Found {df_comp.shape[0]} mismatches both side combined")
+        output_dataframes = dict()
+        if self.composite:
+            log.debug(f"Performing composite comparison for: {compare_columns}")
+            df_comp = perform_comparison(
+                ds_compressed_names=ds_compressed_names,
+                dataframes=column_df_list,
+                on=compare_columns,
+                how="outer",
+                indicator="presence",
+                validate="one_to_one",
+            )
+            df_comp = df_comp[df_comp["presence"] != "both"]
+            df_comp["presence"] = df_comp["presence"].map(
+                {
+                    "left_only": ds_compressed_names[0],
+                    "right_only": ds_compressed_names[1],
+                }
+            )
+            log.debug(f"Found {df_comp.shape[0]} mismatches all sides combined")
+            output_dataframes["-".join(compare_columns)] = df_comp
+        else:
+            for c in compare_columns:
+                log.debug(f"Performing comparison for: {c}")
+                column_df_list_unique = [
+                    pd.DataFrame(df[c].drop_duplicates()) for df in column_df_list
+                ]
+                df_comp = perform_comparison(
+                    ds_compressed_names=ds_compressed_names,
+                    dataframes=column_df_list_unique,
+                    on=c,
+                    how="outer",
+                    indicator="presence",
+                    validate="one_to_one",
+                )
+                df_comp = df_comp[df_comp["presence"] != "both"]
+                df_comp["presence"] = df_comp["presence"].map(
+                    {
+                        "left_only": ds_compressed_names[0],
+                        "right_only": ds_compressed_names[1],
+                    }
+                )
+                log.debug(f"Found {df_comp.shape[0]} mismatches all sides combined")
+                output_dataframes[c] = df_comp
 
         log.debug(f"Writing output into: {self.outfile_fqn}")
         _ = create_dir_if_not_exist(self.project["outdir"])
-        with pd.ExcelWriter(
-            self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
-        ) as writer:
-            df_comp.to_excel(writer, sheet_name="Column Comparison", index=False)
+        for sheet, df in output_dataframes.items():
+            with pd.ExcelWriter(
+                self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
+            ) as writer:
+                df.to_excel(
+                    writer, sheet_name=f"Column Comparison-> {sheet}", index=False
+                )
 
         end_time = time.time()
         log.info("------------------------ Finished task: compare-column")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
 
 
 @dataclass
 class CompareTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     sample_count: int = DEFAULT_VALUES["sample_count"]
+    composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     # Support for default values
     def __post_init__(self):
         for field in fields(self):
             # If there is a default and the value of the field is none we can assign a value
             if (
                 not isinstance(field.default, _MISSING_TYPE)
@@ -407,14 +443,15 @@
         try:
             CompareColumnTask(
                 profile=self.profile,
                 project=self.project,
                 runtime=self.runtime,
                 datasources=self.datasources,
                 outfile_fqn=self.outfile_fqn,
+                composite=self.composite,
             ).execute()
         except Exception as exc:
             log.error(f"Column comparison failed with error: {exc}")
 
         end_time = time.time()
         log.info("------------------------ Finished task: compare")
         log.info(
```

### Comparing `tulona-0.4.0/core/tulona/task/helper.py` & `tulona-0.5.0/core/tulona/task/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,38 +73,40 @@
     return df
 
 
 # TODO: common param to toggle comparison result for common vs all columns
 def perform_comparison(
     ds_compressed_names: List[str],
     dataframes: List[pd.DataFrame],
-    on: str,
+    on: Union[str, List],
     how: str = "inner",
     suffixes: Tuple[str] = ("_x", "_y"),
     indicator: Union[bool, str] = False,
     validate: Optional[str] = None,
 ) -> pd.DataFrame:
-    primary_key = on.lower()
+    on = [on] if isinstance(on, str) else on
+    primary_key = [k.lower() for k in on]
     common_columns = {c.lower() for c in dataframes[0].columns.tolist()}
 
     dataframes_final = []
     for df in dataframes[1:]:
         colset = {c.lower() for c in df.columns.tolist()}
         common_columns = common_columns.intersection(colset)
 
     for ds_name, df in zip(ds_compressed_names, dataframes):
         df = df[list(common_columns)]
         df = df.rename(
             columns={
-                c: f"{c}_{ds_name}" if c.lower() != primary_key else c.lower()
+                c: f"{c}_{ds_name}" if c.lower() not in primary_key else c
                 for c in df.columns
             }
         )
-        if pd.api.types.is_string_dtype(df[primary_key]):
-            df[primary_key] = df[primary_key].str.lower()
+        for k in primary_key:
+            if pd.api.types.is_string_dtype(df[k]):
+                df[k] = df[k].str.lower()
         dataframes_final.append(df)
 
     df_merge = dataframes_final.pop()
     for df in dataframes_final:
         df_merge = pd.merge(
             left=df_merge,
             right=df,
```

### Comparing `tulona-0.4.0/core/tulona/task/ping.py` & `tulona-0.5.0/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/task/profile.py` & `tulona-0.5.0/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/task/scan.py` & `tulona-0.5.0/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/util/database.py` & `tulona-0.5.0/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/util/dataframe.py` & `tulona-0.5.0/core/tulona/util/dataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from typing import Union
+from typing import List, Tuple, Union
 
 import pandas as pd
 
 from tulona.exceptions import TulonaFundamentalError
 
 
 def apply_column_exclusion(
-    df: pd.DataFrame, primary_key: str, exclude_columns: list, table: str
+    df: pd.DataFrame,
+    primary_key: Union[List, Tuple, str],
+    exclude_columns: list,
+    table: str,
 ) -> Union[pd.DataFrame, None]:
-    if primary_key in exclude_columns:
-        raise TulonaFundamentalError(
-            "Cannot exclude primary key/join key from data comparison"
-        )
+    for k in primary_key:
+        if k in exclude_columns:
+            raise TulonaFundamentalError(
+                f"Cannot exclude primary key/join key {k} from comparison"
+            )
 
     missing_cols = []
     for col in exclude_columns:
         if col not in df.columns.tolist():
             missing_cols.append(col)
 
     if len(missing_cols) > 0:
```

### Comparing `tulona-0.4.0/core/tulona/util/excel.py` & `tulona-0.5.0/core/tulona/util/excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Tuple, Union
 
 from openpyxl import load_workbook, styles
 from openpyxl.styles import Border, Side
 from openpyxl.worksheet.worksheet import Worksheet
 
 
 def get_column_index(sheet: Worksheet, column: str):
@@ -12,15 +12,18 @@
                 return idx
     raise ValueError(f"Column {column} could not be found in the Excel sheet.")
 
 
 # TODO: Testable function - it should take WorkBook as input instead of excel_file and return WorkBook
 # instead of saving the file
 def highlight_mismatch_cells(  # pargma: no cover
-    excel_file, sheet: str, num_ds: int, skip_columns: Union[str, List[str]] = None
+    excel_file,
+    sheet: str,
+    num_ds: int,
+    skip_columns: Union[str, Tuple[str], List[str]] = None,
 ):
     wb = load_workbook(excel_file)
     ws = wb[sheet]
 
     yellow_fill = styles.PatternFill(
         start_color="FFFFFF00", end_color="FFFFFF00", fill_type="solid"
     )
@@ -43,15 +46,19 @@
         left=Side(border_style="dotted"),
         right=Side(border_style="thin"),
         top=Side(border_style="thin"),
         bottom=Side(border_style="thin"),
     )
 
     if skip_columns:
-        skip_columns = skip_columns if isinstance(skip_columns, list) else [skip_columns]
+        skip_columns = (
+            skip_columns
+            if isinstance(skip_columns, list) or isinstance(skip_columns, tuple)
+            else [skip_columns]
+        )
         skip_idxs = [get_column_index(ws, c.lower()) - 1 for c in skip_columns]
         compareable_col_idxs = list(set(range(ws.max_column)) - set(skip_idxs))
     else:
         compareable_col_idxs = list(range(ws.max_column))
 
     for row in ws.iter_rows(
         min_row=2, min_col=0, max_row=ws.max_row, max_col=ws.max_column
```

### Comparing `tulona-0.4.0/core/tulona/util/filesystem.py` & `tulona-0.5.0/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/util/profiles.py` & `tulona-0.5.0/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/core/tulona/util/sql.py` & `tulona-0.5.0/core/tulona/util/sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union
+from typing import Dict, List, Tuple, Union
 
 import pandas as pd
 
 from tulona.exceptions import TulonaNotImplementedError
 
 
 def get_table_fqn(database: Union[str, None], schema: str, table: str) -> str:
@@ -26,41 +26,46 @@
         raise TulonaNotImplementedError(
             f"Extracting sample rows from source type {dbtype} is not implemented."
         )
 
     return query
 
 
-def get_column_query(table_fqn: str, column: str, quoted=False):
-    if quoted:
-        query = f"""select "{column}" from {table_fqn}"""
-    else:
-        query = f"""select {column} from {table_fqn}"""
+def get_column_query(table_fqn: str, columns: List[str], quoted=False):
+    column_expr = ", ".join([f'"{c}"' if quoted else c for c in columns])
+    query = f"""select {column_expr} from {table_fqn}"""
 
     return query
 
 
 def get_query_output_as_df(connection_manager, query_text: str):  # pragma: no cover
     with connection_manager.engine.connect() as conn:
         df = pd.read_sql_query(query_text, conn)
     return df
 
 
 def build_filter_query_expression(
-    df: pd.DataFrame, primary_key: str, positive: bool = True
+    df: pd.DataFrame, primary_key: Union[List, Tuple, str], positive: bool = True
 ):
-    primary_keys = df[primary_key].tolist()
+    expr_list = []
+    primary_key = [primary_key] if isinstance(primary_key, str) else primary_key
+    for k in primary_key:
+        primary_key_values = df[k].tolist()
+
+        if pd.api.types.is_numeric_dtype(df[k]):
+            primary_key_values = [str(k) for k in primary_key_values]
+            query_expr = f"""{k}{'' if positive else ' not'} in ({", ".join(primary_key_values)})"""
+        else:
+            query_expr = f"""{k}{'' if positive else ' not'} in ('{"', '".join(primary_key_values)}')"""
 
-    if "int" in str(df[primary_key].dtype):
-        primary_keys = [str(k) for k in primary_keys]
-        query_expr = f"""{primary_key}{'' if positive else ' not'} in ({", ".join(primary_keys)})"""
-    else:
-        query_expr = f"""{primary_key}{'' if positive else ' not'} in ('{"', '".join(primary_keys)}')"""
+        expr_list.append(query_expr)
+
+    final_expr = f" {'and' if positive else 'or'} ".join(expr_list)
 
-    return query_expr
+    return final_expr
 
 
 def get_metadata_query(database, schema, table):
     if database:
         query = f"""
         select * from information_schema.columns
         where upper(table_catalog) = '{database.upper()}'
```

### Comparing `tulona-0.4.0/core/tulona.egg-info/PKG-INFO` & `tulona-0.5.0/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.4.0/core/tulona.egg-info/SOURCES.txt` & `tulona-0.5.0/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.4.0/pyproject.toml` & `tulona-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.4.0"
+version = "0.5.0"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -110,22 +110,22 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.5.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
-tag = true
+tag = false
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 commit = false
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
```

