# Comparing `tmp/brplotviz-0.2.2.tar.gz` & `tmp/brplotviz-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brplotviz-0.2.2.tar", last modified: Sat Mar 30 13:44:51 2024, max compression
+gzip compressed data, was "brplotviz-0.2.3.tar", last modified: Sat Apr 13 11:40:54 2024, max compression
```

## Comparing `brplotviz-0.2.2.tar` & `brplotviz-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-03-30 13:44:51.104656 brplotviz-0.2.2/
--rwxr-xr-x   0 bertram   (1000) bertram   (1000)    35081 2022-08-05 18:57:03.000000 brplotviz-0.2.2/LICENSE
--rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-03-30 13:44:51.104656 brplotviz-0.2.2/PKG-INFO
--rwxr-xr-x   0 bertram   (1000) bertram   (1000)     3345 2024-03-30 13:05:24.000000 brplotviz-0.2.2/README.md
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1194 2024-03-30 13:26:54.000000 brplotviz-0.2.2/pyproject.toml
--rw-r--r--   0 bertram   (1000) bertram   (1000)       38 2024-03-30 13:44:51.104656 brplotviz-0.2.2/setup.cfg
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-03-30 13:44:51.104656 brplotviz-0.2.2/src/
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-03-30 13:44:51.104656 brplotviz-0.2.2/src/brplotviz/
--rw-r--r--   0 bertram   (1000) bertram   (1000)      182 2024-03-17 19:47:01.000000 brplotviz-0.2.2/src/brplotviz/__init__.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)    20923 2024-03-17 19:47:01.000000 brplotviz-0.2.2/src/brplotviz/plot.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1578 2024-03-17 19:47:01.000000 brplotviz-0.2.2/src/brplotviz/styleselect.py
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-03-30 13:44:51.104656 brplotviz-0.2.2/src/brplotviz/table/
--rw-r--r--   0 bertram   (1000) bertram   (1000)    22135 2024-03-30 11:51:53.000000 brplotviz-0.2.2/src/brplotviz/table/__init__.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     7410 2024-03-17 19:47:01.000000 brplotviz-0.2.2/src/brplotviz/table/engines.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1233 2024-03-17 19:47:01.000000 brplotviz-0.2.2/src/brplotviz/table/rules.py
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-03-30 13:44:51.104656 brplotviz-0.2.2/src/brplotviz.egg-info/
--rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-03-30 13:44:51.000000 brplotviz-0.2.2/src/brplotviz.egg-info/PKG-INFO
--rw-r--r--   0 bertram   (1000) bertram   (1000)      385 2024-03-30 13:44:51.000000 brplotviz-0.2.2/src/brplotviz.egg-info/SOURCES.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)        1 2024-03-30 13:44:51.000000 brplotviz-0.2.2/src/brplotviz.egg-info/dependency_links.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)       24 2024-03-30 13:44:51.000000 brplotviz-0.2.2/src/brplotviz.egg-info/requires.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)       10 2024-03-30 13:44:51.000000 brplotviz-0.2.2/src/brplotviz.egg-info/top_level.txt
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/
+-rwxr-xr-x   0 bertram   (1000) bertram   (1000)    35081 2022-08-05 18:57:03.000000 brplotviz-0.2.3/LICENSE
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-04-13 11:40:54.279367 brplotviz-0.2.3/PKG-INFO
+-rwxr-xr-x   0 bertram   (1000) bertram   (1000)     3345 2024-03-30 13:05:24.000000 brplotviz-0.2.3/README.md
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1194 2024-04-13 11:36:40.000000 brplotviz-0.2.3/pyproject.toml
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       38 2024-04-13 11:40:54.279367 brplotviz-0.2.3/setup.cfg
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)      182 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/__init__.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    20923 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/plot.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1578 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/styleselect.py
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz/table/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    22137 2024-04-10 18:41:11.000000 brplotviz-0.2.3/src/brplotviz/table/__init__.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     7410 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/table/engines.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1233 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/table/rules.py
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz.egg-info/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/PKG-INFO
+-rw-r--r--   0 bertram   (1000) bertram   (1000)      385 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/SOURCES.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)        1 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/dependency_links.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       24 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/requires.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       10 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/top_level.txt
```

### Comparing `brplotviz-0.2.2/LICENSE` & `brplotviz-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/PKG-INFO` & `brplotviz-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brplotviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: Plot utilities for outputting plots and tables nicely formatted
 Author-email: Bertram Richter <bertram.richter@tu-dresden.de>
 Maintainer-email: Bertram Richter <bertram.richter@tu-dresden.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `brplotviz-0.2.2/README.md` & `brplotviz-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/pyproject.toml` & `brplotviz-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "brplotviz"
 
-version = "0.2.2"
+version = "0.2.3"
 
 description = "Plot utilities for outputting plots and tables nicely formatted"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
```

### Comparing `brplotviz-0.2.2/src/brplotviz/plot.py` & `brplotviz-0.2.3/src/brplotviz/plot.py`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/src/brplotviz/styleselect.py` & `brplotviz-0.2.3/src/brplotviz/styleselect.py`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/src/brplotviz/table/__init__.py` & `brplotviz-0.2.3/src/brplotviz/table/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,19 +115,14 @@
 	|				|		|		|
 	| :---			| :---:	| :---:	|
 	| `head_col 0`	| `0,0`	| `0,1`	|
 	| `head_col 1`	| `1,0`	| `1,1`	|
 	"""
 	engine_kwargs = engine_kwargs if engine_kwargs is not None else {}
 	engine = get_engine(engine, **engine_kwargs)
-	# Convert the entries of the top_left, head column and head row to str.
-	# This will result in a new list, so the original data is not modified.
-	head_col = _apply_format([head_col], formatter=None)[0]
-	head_row = _apply_format([head_row], formatter=None)[0]
-	top_left = "{}".format(top_left)
 	# Convert the table to a list of lists (e.g., from numpy arrays) and
 	# extract extra rules
 	clean_table = []
 	rule_dict = {}
 	for i, row in enumerate(copy.deepcopy(table)):
 		if isinstance(row, Rule):
 			rule_dict[i] = row
@@ -140,17 +135,22 @@
 				raise ValueError("Cannot convert {}th entry to list: {}".format(i, row))
 	table = clean_table
 	# Transpose the body data, if requested
 	if transpose_data:
 		table = _transpose(table)
 	# Convert to table of str
 	table = _apply_format(table, formatter)
+	# Convert the entries of the top_left, head column and head row to str.
+	# This will result in a new list, so the original data is not modified.
+	top_left = "{}".format(top_left)
 	if head_row is not None:
+		head_row = _apply_format([head_row], formatter=None)[0]
 		table.insert(0, head_row)
 	if head_row is not None and head_col is not None:
+		head_col = _apply_format([head_col], formatter=None)[0]
 		head_col.insert(0, top_left)
 	# Transpose and operate column wise
 	table = _transpose(table)
 	# Add header column
 	if head_col is not None:
 		table.insert(0, head_col)
 	if replacement is not None:
```

### Comparing `brplotviz-0.2.2/src/brplotviz/table/engines.py` & `brplotviz-0.2.3/src/brplotviz/table/engines.py`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/src/brplotviz/table/rules.py` & `brplotviz-0.2.3/src/brplotviz/table/rules.py`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.2/src/brplotviz.egg-info/PKG-INFO` & `brplotviz-0.2.3/src/brplotviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brplotviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: Plot utilities for outputting plots and tables nicely formatted
 Author-email: Bertram Richter <bertram.richter@tu-dresden.de>
 Maintainer-email: Bertram Richter <bertram.richter@tu-dresden.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

