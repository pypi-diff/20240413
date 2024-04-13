# Comparing `tmp/bdchecker-0.0.2a1.tar.gz` & `tmp/bdchecker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdchecker-0.0.2a1.tar", last modified: Tue Jan  9 15:45:16 2024, max compression
+gzip compressed data, was "bdchecker-0.0.3.tar", last modified: Sat Apr 13 06:30:22 2024, max compression
```

## Comparing `bdchecker-0.0.2a1.tar` & `bdchecker-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:45:16.880121 bdchecker-0.0.2a1/
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1077 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/LICENSE
--rw-r--r--   0 mugglewei  (1001) mugglewei  (1001)     1783 2024-01-09 15:45:16.880121 bdchecker-0.0.2a1/PKG-INFO
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/README.md
-drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:45:16.876121 bdchecker-0.0.2a1/bdchecker/
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/__init__.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       30 2024-01-09 15:44:19.000000 bdchecker-0.0.2a1/bdchecker/__version__.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     8483 2024-01-09 15:22:23.000000 bdchecker-0.0.2a1/bdchecker/checker.py
-drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:45:16.876121 bdchecker-0.0.2a1/bdchecker/command/
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1541 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/command/check.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1555 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/command/clean.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1539 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/command/gen.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1543 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/main.py
-drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:45:16.876121 bdchecker-0.0.2a1/bdchecker/utils/
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/utils/__init__.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       23 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/utils/const_var.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     4616 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/utils/log_handle.py
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      230 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/bdchecker/utils/singleton.py
-drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:45:16.880121 bdchecker-0.0.2a1/bdchecker.egg-info/
--rw-r--r--   0 mugglewei  (1001) mugglewei  (1001)     1783 2024-01-09 15:45:16.000000 bdchecker-0.0.2a1/bdchecker.egg-info/PKG-INFO
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      498 2024-01-09 15:45:16.000000 bdchecker-0.0.2a1/bdchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        1 2024-01-09 15:45:16.000000 bdchecker-0.0.2a1/bdchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       50 2024-01-09 15:45:16.000000 bdchecker-0.0.2a1/bdchecker.egg-info/entry_points.txt
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       10 2024-01-09 15:45:16.000000 bdchecker-0.0.2a1/bdchecker.egg-info/top_level.txt
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      958 2024-01-09 15:42:55.000000 bdchecker-0.0.2a1/pyproject.toml
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.2a1/requirements.txt
--rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       38 2024-01-09 15:45:16.880121 bdchecker-0.0.2a1/setup.cfg
+drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-04-13 06:30:22.203328 bdchecker-0.0.3/
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1077 2024-01-09 15:21:58.000000 bdchecker-0.0.3/LICENSE
+-rw-r--r--   0 mugglewei  (1001) mugglewei  (1001)     5967 2024-04-13 06:30:22.203328 bdchecker-0.0.3/PKG-INFO
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     4185 2024-04-13 06:17:51.000000 bdchecker-0.0.3/README.md
+drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-04-13 06:30:22.199328 bdchecker-0.0.3/bdchecker/
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/__init__.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       22 2024-04-13 06:24:30.000000 bdchecker-0.0.3/bdchecker/__version__.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     8694 2024-01-10 06:14:45.000000 bdchecker-0.0.3/bdchecker/checker.py
+drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-04-13 06:30:22.199328 bdchecker-0.0.3/bdchecker/command/
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1541 2024-04-13 06:24:30.000000 bdchecker-0.0.3/bdchecker/command/check.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1555 2024-04-13 06:24:30.000000 bdchecker-0.0.3/bdchecker/command/clean.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1539 2024-04-13 06:24:30.000000 bdchecker-0.0.3/bdchecker/command/gen.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     1543 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/main.py
+drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-04-13 06:30:22.199328 bdchecker-0.0.3/bdchecker/utils/
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/utils/__init__.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       23 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/utils/const_var.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)     4616 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/utils/log_handle.py
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      230 2024-01-09 15:21:58.000000 bdchecker-0.0.3/bdchecker/utils/singleton.py
+drwxrwxr-x   0 mugglewei  (1001) mugglewei  (1001)        0 2024-04-13 06:30:22.199328 bdchecker-0.0.3/bdchecker.egg-info/
+-rw-r--r--   0 mugglewei  (1001) mugglewei  (1001)     5967 2024-04-13 06:30:22.000000 bdchecker-0.0.3/bdchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      498 2024-04-13 06:30:22.000000 bdchecker-0.0.3/bdchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        1 2024-04-13 06:30:22.000000 bdchecker-0.0.3/bdchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       50 2024-04-13 06:30:22.000000 bdchecker-0.0.3/bdchecker.egg-info/entry_points.txt
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       10 2024-04-13 06:30:22.000000 bdchecker-0.0.3/bdchecker.egg-info/top_level.txt
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)      958 2024-01-10 06:14:45.000000 bdchecker-0.0.3/pyproject.toml
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)        0 2024-01-09 15:21:58.000000 bdchecker-0.0.3/requirements.txt
+-rw-rw-r--   0 mugglewei  (1001) mugglewei  (1001)       38 2024-04-13 06:30:22.203328 bdchecker-0.0.3/setup.cfg
```

### Comparing `bdchecker-0.0.2a1/LICENSE` & `bdchecker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bdchecker-0.0.2a1/bdchecker/checker.py` & `bdchecker-0.0.3/bdchecker/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,27 +158,34 @@
         for k, v in meta_dict.items():
             filepath = os.path.join(dst_dir, k)
             hash_val_hex = self._gen_hash(filepath)
             meta_dict[k] = hash_val_hex
             logging.debug(
                 "calculate hash value: {}, {}".format(k, hash_val_hex))
 
+        is_all_pass = True
         for k, v in old_meta_dict.items():
             if k not in meta_dict:
                 logging.warning("missing file: {}".format(k))
+                is_all_pass = False
 
         for k, v in meta_dict.items():
             if k not in old_meta_dict:
                 logging.warning("new file: {}".format(k))
+                is_all_pass = False
 
             old_v = old_meta_dict[k]
             if v != old_v:
                 logging.error(
                     "check failed: {}, old hash: {}, cur hash: {}".format(
                         k, old_v, v))
+                is_all_pass = False
+
+        if is_all_pass is True:
+            logging.info("all check pass")
 
     def _dump_meta(self, meta_filepath, meta_dict):
         """
         dump meta infos
         """
         backup_filepath = "{}.backup".format(meta_filepath)
         tmp_meta_filepath = "{}.tmp".format(meta_filepath)
```

### Comparing `bdchecker-0.0.2a1/bdchecker/command/check.py` & `bdchecker-0.0.3/bdchecker/command/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "Options: \n" \
             "  -d, --dir        [REQUIRED] target directory\n" \
             "  -v, --verbose    [OPTIONAL] set verbose level; [0|1]\n" \
             "    , --hash       [OPTIONAL] hash algo; [md5|sha256|sha512]\n" \
             "".format(APP_NAME)
 
         self._dir = ""
-        self._verbose = 0
+        self._verbose = 1
         self._hash_algo = "sha256"
 
     def run(self, args):
         """
         run command gen
         """
         self._parse_args(args)
```

### Comparing `bdchecker-0.0.2a1/bdchecker/command/clean.py` & `bdchecker-0.0.3/bdchecker/command/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             "Options: \n" \
             "  -d, --dir        [REQUIRED] target directory\n" \
             "  -v, --verbose    [OPTIONAL] set verbose level; [0|1]\n" \
             "    , --hash       [OPTIONAL] hash algo; [md5|sha256|sha512]\n" \
             "".format(APP_NAME)
 
         self._dir = ""
-        self._verbose = 0
+        self._verbose = 1
         self._hash_algo = "sha256"
 
     def run(self, args):
         """
         run command gen
         """
         self._parse_args(args)
```

### Comparing `bdchecker-0.0.2a1/bdchecker/command/gen.py` & `bdchecker-0.0.3/bdchecker/command/gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "Options: \n" \
             "  -d, --dir        [REQUIRED] target directory\n" \
             "  -v, --verbose    [OPTIONAL] set verbose level; [0|1]\n" \
             "    , --hash       [OPTIONAL] hash algo; [md5|sha256|sha512]\n" \
             "".format(APP_NAME)
 
         self._dir = ""
-        self._verbose = 0
+        self._verbose = 1
         self._hash_algo = "sha256"
 
     def run(self, args):
         """
         run command gen
         """
         self._parse_args(args)
```

### Comparing `bdchecker-0.0.2a1/bdchecker/main.py` & `bdchecker-0.0.3/bdchecker/main.py`

 * *Files identical despite different names*

### Comparing `bdchecker-0.0.2a1/bdchecker/utils/log_handle.py` & `bdchecker-0.0.3/bdchecker/utils/log_handle.py`

 * *Files identical despite different names*

### Comparing `bdchecker-0.0.2a1/pyproject.toml` & `bdchecker-0.0.3/pyproject.toml`

 * *Files identical despite different names*

