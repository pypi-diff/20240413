# Comparing `tmp/grutils-0.1.8.2.tar.gz` & `tmp/grutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grutils-0.1.8.2.tar", last modified: Wed Dec 22 04:41:10 2021, max compression
+gzip compressed data, was "dist/grutils-0.1.9.tar", last modified: Thu Dec 23 09:53:11 2021, max compression
```

## Comparing `grutils-0.1.8.2.tar` & `grutils-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-22 04:41:10.000000 grutils-0.1.8.2/
--rw-r--r--   0 liuleidong   (501) staff       (20)    11357 2021-09-14 13:30:32.000000 grutils-0.1.8.2/LICENSE
--rw-r--r--   0 liuleidong   (501) staff       (20)      156 2021-11-19 04:44:07.000000 grutils-0.1.8.2/MANIFEST.in
--rw-r--r--   0 liuleidong   (501) staff       (20)      603 2021-12-22 04:41:10.000000 grutils-0.1.8.2/PKG-INFO
--rw-r--r--   0 liuleidong   (501) staff       (20)       75 2021-11-19 05:35:56.000000 grutils-0.1.8.2/README.md
-drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils/
--rw-r--r--   0 liuleidong   (501) staff       (20)      135 2021-12-22 04:40:17.000000 grutils-0.1.8.2/grutils/__init__.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     1439 2021-11-20 12:15:47.000000 grutils-0.1.8.2/grutils/configs.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     2281 2021-12-13 02:28:08.000000 grutils-0.1.8.2/grutils/csv.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     1231 2021-05-24 09:13:28.000000 grutils-0.1.8.2/grutils/error.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     8854 2021-12-16 06:09:47.000000 grutils-0.1.8.2/grutils/excel.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     1402 2021-11-20 03:23:01.000000 grutils-0.1.8.2/grutils/file.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     7284 2021-12-13 04:23:22.000000 grutils-0.1.8.2/grutils/form.py
--rw-r--r--   0 liuleidong   (501) staff       (20)      607 2021-05-09 03:09:37.000000 grutils-0.1.8.2/grutils/iterable.py
--rw-r--r--   0 liuleidong   (501) staff       (20)      682 2021-11-20 03:22:49.000000 grutils-0.1.8.2/grutils/printer.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     4676 2021-12-22 04:39:55.000000 grutils-0.1.8.2/grutils/progress.py
--rw-r--r--   0 liuleidong   (501) staff       (20)     3738 2021-12-13 13:17:37.000000 grutils-0.1.8.2/grutils/utils.py
-drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/
--rw-r--r--   0 liuleidong   (501) staff       (20)      603 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/PKG-INFO
--rw-r--r--   0 liuleidong   (501) staff       (20)      418 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/SOURCES.txt
--rw-r--r--   0 liuleidong   (501) staff       (20)        1 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/dependency_links.txt
--rw-r--r--   0 liuleidong   (501) staff       (20)       31 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/requires.txt
--rw-r--r--   0 liuleidong   (501) staff       (20)        8 2021-12-22 04:41:10.000000 grutils-0.1.8.2/grutils.egg-info/top_level.txt
--rw-r--r--   0 liuleidong   (501) staff       (20)       31 2021-12-13 02:28:48.000000 grutils-0.1.8.2/requirements.txt
--rw-r--r--   0 liuleidong   (501) staff       (20)       38 2021-12-22 04:41:10.000000 grutils-0.1.8.2/setup.cfg
--rw-r--r--   0 liuleidong   (501) staff       (20)     1142 2021-11-19 04:57:39.000000 grutils-0.1.8.2/setup.py
-drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-22 04:41:10.000000 grutils-0.1.8.2/test/
--rw-r--r--   0 liuleidong   (501) staff       (20)     1956 2021-12-22 04:37:56.000000 grutils-0.1.8.2/test/test.py
+drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-23 09:53:11.000000 grutils-0.1.9/
+-rw-r--r--   0 liuleidong   (501) staff       (20)    11357 2021-09-14 13:30:32.000000 grutils-0.1.9/LICENSE
+-rw-r--r--   0 liuleidong   (501) staff       (20)      156 2021-11-19 04:44:07.000000 grutils-0.1.9/MANIFEST.in
+-rw-r--r--   0 liuleidong   (501) staff       (20)      601 2021-12-23 09:53:11.000000 grutils-0.1.9/PKG-INFO
+-rw-r--r--   0 liuleidong   (501) staff       (20)       75 2021-11-19 05:35:56.000000 grutils-0.1.9/README.md
+drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils/
+-rw-r--r--   0 liuleidong   (501) staff       (20)      132 2021-12-23 09:51:04.000000 grutils-0.1.9/grutils/__init__.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1439 2021-11-20 12:15:47.000000 grutils-0.1.9/grutils/configs.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     2281 2021-12-13 02:28:08.000000 grutils-0.1.9/grutils/csv.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     6517 2021-12-23 09:48:00.000000 grutils-0.1.9/grutils/easyform.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1231 2021-05-24 09:13:28.000000 grutils-0.1.9/grutils/error.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     8898 2021-12-23 09:47:47.000000 grutils-0.1.9/grutils/excel.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1402 2021-11-20 03:23:01.000000 grutils-0.1.9/grutils/file.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     7284 2021-12-13 04:23:22.000000 grutils-0.1.9/grutils/form.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1629 2021-12-23 09:47:37.000000 grutils-0.1.9/grutils/form_utils.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)      607 2021-05-09 03:09:37.000000 grutils-0.1.9/grutils/iterable.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)      682 2021-11-20 03:22:49.000000 grutils-0.1.9/grutils/printer.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     4676 2021-12-22 04:39:55.000000 grutils-0.1.9/grutils/progress.py
+-rw-r--r--   0 liuleidong   (501) staff       (20)     5639 2021-12-23 09:48:23.000000 grutils-0.1.9/grutils/utils.py
+drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/
+-rw-r--r--   0 liuleidong   (501) staff       (20)      601 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/PKG-INFO
+-rw-r--r--   0 liuleidong   (501) staff       (20)      460 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/SOURCES.txt
+-rw-r--r--   0 liuleidong   (501) staff       (20)        1 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/dependency_links.txt
+-rw-r--r--   0 liuleidong   (501) staff       (20)       31 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/requires.txt
+-rw-r--r--   0 liuleidong   (501) staff       (20)        8 2021-12-23 09:53:11.000000 grutils-0.1.9/grutils.egg-info/top_level.txt
+-rw-r--r--   0 liuleidong   (501) staff       (20)       31 2021-12-13 02:28:48.000000 grutils-0.1.9/requirements.txt
+-rw-r--r--   0 liuleidong   (501) staff       (20)       38 2021-12-23 09:53:11.000000 grutils-0.1.9/setup.cfg
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1142 2021-11-19 04:57:39.000000 grutils-0.1.9/setup.py
+drwxr-xr-x   0 liuleidong   (501) staff       (20)        0 2021-12-23 09:53:11.000000 grutils-0.1.9/test/
+-rw-r--r--   0 liuleidong   (501) staff       (20)     1939 2021-12-23 09:50:47.000000 grutils-0.1.9/test/test.py
```

### Comparing `grutils-0.1.8.2/LICENSE` & `grutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/PKG-INFO` & `grutils-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grutils
-Version: 0.1.8.2
+Version: 0.1.9
 Summary: reusable grutils
 Home-page: UNKNOWN
 Author: leidong.liu
 Author-email: leidong.liu@gmail.com
 License: Apache2.0
 Project-URL: Source, https://github.com/lldld/gr.py3.utils
 Description: # gr.py3.utils
```

### Comparing `grutils-0.1.8.2/grutils/configs.py` & `grutils-0.1.9/grutils/configs.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/csv.py` & `grutils-0.1.9/grutils/csv.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/error.py` & `grutils-0.1.9/grutils/error.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/excel.py` & `grutils-0.1.9/grutils/excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,15 @@
     # uploading
     source_wb = app.books.open(source_file_path)
     target_wb = app.books.open(target_file_path)
 
     uploaded = append_sht_to_another(err, source_wb, target_wb,
                                      source_sheet,
                                      target_sheet,
+                                     False,
                                      empty_rows,
                                      source_ref_column,
                                      target_ref_column)
 
     if uploaded is not None and uploaded:
         target_wb.save()
```

### Comparing `grutils-0.1.8.2/grutils/file.py` & `grutils-0.1.9/grutils/file.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/form.py` & `grutils-0.1.9/grutils/form.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/iterable.py` & `grutils-0.1.9/grutils/iterable.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/printer.py` & `grutils-0.1.9/grutils/printer.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/progress.py` & `grutils-0.1.9/grutils/progress.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/grutils/utils.py` & `grutils-0.1.9/grutils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import os
 from datetime import datetime, date
 from typing import Dict, List, Optional, Tuple
 
+from .configs import Configuration
 from .error import Error
 
 
 def strip_if_str(s):
     if type(s) == str:
         return s.strip()
     else:
@@ -131,7 +133,89 @@
                                   formatter: str = "{}",
                                   linker: str = "-",
                                   joiner: str = ","
                                   ):
     items = list(map(lambda group: (formatter + linker + formatter).format(group[0], group[1]) if group[0] != group[
         1] else formatter.format(group[0]), groups))
     return joiner.join(items)
+
+
+def str_without_prefix(val: any, prefix='\''):
+    if type(val) == str and val.startswith(prefix):
+        return val[len(prefix):]
+    else:
+        return val
+
+
+def str_without_prefixes(val: any, prefixes: List[str]):
+    if type(val) != str:
+        return val
+    _val = val
+    for prefix in prefixes:
+        if _val.startswith(prefix):
+            _val = _val[len(prefix):]
+    return _val
+
+
+def str_with_prefix(val: any, formatter: str = '{}', prefix='\''):
+    if type(val) == str and val.startswith(prefix):
+        return val
+    else:
+        return (prefix + formatter).format(val)
+
+
+def simple_date_str(d: date):
+    return '{}/{}'.format(d.month, d.day)
+
+
+def compare_two_list(a: Optional[List], b: Optional[List]):
+    if a is None and b is None:
+        return True
+
+    if a is None or b is None:
+        return False
+
+    for k in a:
+        if k not in b:
+            return False
+
+    for k in b:
+        if k not in a:
+            return False
+
+    return True
+
+
+def get_os_user():
+    return os.getenv('username')
+
+
+def get_special_folder(err: Error, key: str, config: Configuration, test_os_user: str = 'liuleidong'):
+    if err.has_error():
+        return
+
+    folder = config.get(key=key, default='', save_if_no=False)
+    if os.path.exists(folder):
+        return folder
+
+    os_user = get_os_user()
+    if os_user == test_os_user:
+        folder = config.get(key='test_' + key, default='', save_if_no=False)
+        if len(folder) == 0:
+            return folder
+        if os.path.exists(folder):
+            return folder
+
+    err.append('folder "' + folder + '" is not exists')
+
+
+# noinspection PyBroadException
+def int_val_or_none(s: str):
+    try:
+        i = int(round(float(s)))
+        return i
+    except Exception as _:
+        return None
+
+
+def string_of(v: any):
+    return v if type(v) == str else '{}'.format(v)
```

### Comparing `grutils-0.1.8.2/grutils.egg-info/PKG-INFO` & `grutils-0.1.9/grutils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grutils
-Version: 0.1.8.2
+Version: 0.1.9
 Summary: reusable grutils
 Home-page: UNKNOWN
 Author: leidong.liu
 Author-email: leidong.liu@gmail.com
 License: Apache2.0
 Project-URL: Source, https://github.com/lldld/gr.py3.utils
 Description: # gr.py3.utils
```

### Comparing `grutils-0.1.8.2/setup.py` & `grutils-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `grutils-0.1.8.2/test/test.py` & `grutils-0.1.9/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # err = error.Error()
 # print(utils.int_value_of("101.12", err, 0))
 #
 # print(date_of(datetime.date(datetime.now())))
 
 from grutils.progress import shared_progress
+from grutils.form_utils import read_sht
 
 shared_progress.reset()
 
 shared_progress.register_step("step 1", 6)
 shared_progress.register_step("step 2", 4)
 shared_progress.register_step("step 2.1", 0.6, ["step 2"])
 shared_progress.register_step("step 2.2", 0.4, ["step 2"])
@@ -28,22 +29,18 @@
 
 shared_progress.re_assign_steps()
 
 shared_progress.finish_step(["step 3"])
 shared_progress.dump_steps()
 
 shared_progress.reset()
-shared_progress.finish_step(["step 2"])
+shared_progress.finish_step(["step 2", "step 2.2", "step 2.2.1"])
 shared_progress.dump_steps()
 
 
-shared_progress.reset(True)
-shared_progress.finish()
-shared_progress.dump_steps()
-
 # print('\n\n  ============== ')
 # shared_progress.finish_step(["step 1"])
 #
 # print('\n\n  ============== ')
 # shared_progress.finish_step(["step 2", "step 2.1"])
 #
 # print('\n\n  ============== ')
```

