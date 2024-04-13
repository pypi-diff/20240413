# Comparing `tmp/aiotgm-0.3.6.tar.gz` & `tmp/aiotgm-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.3.6.tar", last modified: Sun Apr  7 09:37:35 2024, max compression
+gzip compressed data, was "aiotgm-0.3.7.tar", last modified: Sat Apr 13 17:37:13 2024, max compression
```

## Comparing `aiotgm-0.3.6.tar` & `aiotgm-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.6/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-07 09:37:35.026950 aiotgm-0.3.6/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1235 2024-04-04 07:17:27.000000 aiotgm-0.3.6/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.022949 aiotgm-0.3.6/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-07 09:37:23.000000 aiotgm-0.3.6/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)    28031 2024-04-04 07:02:24.000000 aiotgm-0.3.6/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   283164 2024-04-04 07:07:39.000000 aiotgm-0.3.6/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.6/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.6/aiotgm/logging.py
--rw-r--r--   0 kali      (1000) root         (0)   381827 2024-04-07 09:35:26.000000 aiotgm-0.3.6/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.6/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.6/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-07 09:37:35.000000 aiotgm-0.3.6/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-07 09:37:21.000000 aiotgm-0.3.6/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-07 09:37:35.026950 aiotgm-0.3.6/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 09:37:35.026950 aiotgm-0.3.6/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.6/tests/test_func_ok.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-13 17:37:13.766619 aiotgm-0.3.7/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.7/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-13 17:37:13.766619 aiotgm-0.3.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1235 2024-04-04 07:17:27.000000 aiotgm-0.3.7/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-13 17:37:13.762619 aiotgm-0.3.7/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-13 17:36:44.000000 aiotgm-0.3.7/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    28031 2024-04-04 07:02:24.000000 aiotgm-0.3.7/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   283165 2024-04-13 17:36:27.000000 aiotgm-0.3.7/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.7/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.7/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   381827 2024-04-07 09:35:26.000000 aiotgm-0.3.7/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.7/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.7/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-13 17:37:13.766619 aiotgm-0.3.7/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-13 17:37:13.000000 aiotgm-0.3.7/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-13 17:37:13.000000 aiotgm-0.3.7/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-13 17:37:13.000000 aiotgm-0.3.7/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-13 17:37:13.000000 aiotgm-0.3.7/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-13 17:37:13.000000 aiotgm-0.3.7/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-13 17:36:42.000000 aiotgm-0.3.7/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-13 17:37:13.766619 aiotgm-0.3.7/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-13 17:37:13.766619 aiotgm-0.3.7/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.7/tests/test_func_ok.py
```

### Comparing `aiotgm-0.3.6/LICENSE` & `aiotgm-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/PKG-INFO` & `aiotgm-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.6
+Version: 0.3.7
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.6/README.md` & `aiotgm-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/api.py` & `aiotgm-0.3.7/aiotgm/api.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/client.py` & `aiotgm-0.3.7/aiotgm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,15 +883,15 @@
                     max_retries=float('inf'),
                     keep_alive=True
                 )
                 updates = [Update._dese(update) for update in result]
 
             except TelegramError as exc:
                 if bad_gateway.search(exc.description):
-                    logger.info('{!r} occurred in long polling.'.format(exc))
+                    logger.error('{!r} occurred in long polling.'.format(exc))
                     await asyncio.sleep(2)
                 else:
                     await self.session.close()
                     logger.info('long polling was interrupted.')
                     raise exc from None
 
             except BaseException as exc:
```

### Comparing `aiotgm-0.3.6/aiotgm/constants.py` & `aiotgm-0.3.7/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/logging.py` & `aiotgm-0.3.7/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/types.py` & `aiotgm-0.3.7/aiotgm/types.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/update_manager.py` & `aiotgm-0.3.7/aiotgm/update_manager.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm/utils.py` & `aiotgm-0.3.7/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.6/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.3.7/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.6
+Version: 0.3.7
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.6/tests/test_func_ok.py` & `aiotgm-0.3.7/tests/test_func_ok.py`

 * *Files identical despite different names*

