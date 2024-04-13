# Comparing `tmp/fb_tools-2.5.0.tar.gz` & `tmp/fb_tools-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_tools-2.5.0.tar", last modified: Wed Mar 13 16:36:47 2024, max compression
+gzip compressed data, was "fb_tools-2.5.1.tar", last modified: Sat Apr 13 05:57:57 2024, max compression
```

## Comparing `fb_tools-2.5.0.tar` & `fb_tools-2.5.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.621666 fb_tools-2.5.0/
--rw-r--r--   0 root         (0) root         (0)     7652 2024-03-13 16:36:27.000000 fb_tools-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2024-03-13 16:36:27.000000 fb_tools-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1887 2024-03-13 16:36:47.621666 fb_tools-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2024-03-13 16:36:27.000000 fb_tools-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.609666 fb_tools-2.5.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2298 2024-03-13 16:36:27.000000 fb_tools-2.5.0/bin/get-file-to-remove
--rwxr-xr-x   0 root         (0) root         (0)     2286 2024-03-13 16:36:27.000000 fb_tools-2.5.0/bin/myip
--rwxr-xr-x   0 root         (0) root         (0)     2293 2024-03-13 16:36:27.000000 fb_tools-2.5.0/bin/update-ddns
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.605666 fb_tools-2.5.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.613666 fb_tools-2.5.0/lib/fb_tools/
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29242 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/app.py
--rw-r--r--   0 root         (0) root         (0)     8423 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/argparse_actions.py
--rw-r--r--   0 root         (0) root         (0)     9465 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/cfg_app.py
--rw-r--r--   0 root         (0) root         (0)    36990 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/collections.py
--rw-r--r--   0 root         (0) root         (0)    30170 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/common.py
--rw-r--r--   0 root         (0) root         (0)     7978 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/lib/fb_tools/ddns/
--rw-r--r--   0 root         (0) root         (0)    20366 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/ddns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12479 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/ddns/config.py
--rw-r--r--   0 root         (0) root         (0)     4516 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/ddns/errors.py
--rw-r--r--   0 root         (0) root         (0)     5594 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/ddns/myip_app.py
--rw-r--r--   0 root         (0) root         (0)    27714 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/ddns/update_app.py
--rw-r--r--   0 root         (0) root         (0)    19921 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/errors.py
--rw-r--r--   0 root         (0) root         (0)    24586 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/get_file_rm_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/lib/fb_tools/handler/
--rw-r--r--   0 root         (0) root         (0)    13864 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42608 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/handler/lock.py
--rw-r--r--   0 root         (0) root         (0)    43592 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/handling_obj.py
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    34973 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/mailaddress.py
--rw-r--r--   0 root         (0) root         (0)     2391 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/lib/fb_tools/multi_config/
--rw-r--r--   0 root         (0) root         (0)    20431 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/multi_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12240 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/multi_config/files.py
--rw-r--r--   0 root         (0) root         (0)     7783 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/multi_config/inits.py
--rw-r--r--   0 root         (0) root         (0)    11922 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/multi_config/read.py
--rw-r--r--   0 root         (0) root         (0)    11761 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/obj.py
--rw-r--r--   0 root         (0) root         (0)    17133 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/pidfile.py
--rw-r--r--   0 root         (0) root         (0)     3390 2024-03-13 16:36:27.000000 fb_tools-2.5.0/lib/fb_tools/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.621666 fb_tools-2.5.0/lib/fb_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1887 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1582 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-13 16:36:47.000000 fb_tools-2.5.0/lib/fb_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.609666 fb_tools-2.5.0/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    47617 2024-03-13 16:36:47.000000 fb_tools-2.5.0/locale/de/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    69131 2024-03-13 16:36:27.000000 fb_tools-2.5.0/locale/de/LC_MESSAGES/fb_tools.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.609666 fb_tools-2.5.0/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.617666 fb_tools-2.5.0/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     6156 2024-03-13 16:36:47.000000 fb_tools-2.5.0/locale/en/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    49500 2024-03-13 16:36:27.000000 fb_tools-2.5.0/locale/en/LC_MESSAGES/fb_tools.po
--rw-r--r--   0 root         (0) root         (0)    47320 2024-03-13 16:36:27.000000 fb_tools-2.5.0/locale/fb_tools.pot
--rw-r--r--   0 root         (0) root         (0)     1795 2024-03-13 16:36:47.625666 fb_tools-2.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8889 2024-03-13 16:36:27.000000 fb_tools-2.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:36:47.621666 fb_tools-2.5.0/test/
--rwxr-xr-x   0 root         (0) root         (0)      270 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/call_script.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/call_sleep.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/do_sleep
--rw-r--r--   0 root         (0) root         (0)     4756 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     5221 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    26677 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_05_common.py
--rwxr-xr-x   0 root         (0) root         (0)     6873 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_10_base_object.py
--rwxr-xr-x   0 root         (0) root         (0)    61659 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_13_collections.py
--rwxr-xr-x   0 root         (0) root         (0)    52551 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_15_mailaddress.py
--rwxr-xr-x   0 root         (0) root         (0)    23387 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_17_multicfg.py
--rwxr-xr-x   0 root         (0) root         (0)     6078 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_18_pidfile.py
--rwxr-xr-x   0 root         (0) root         (0)    23666 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_20_handling_object.py
--rwxr-xr-x   0 root         (0) root         (0)     7698 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_25_ddns_update_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8159 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_30_base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)    15313 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_33_lock.py
--rwxr-xr-x   0 root         (0) root         (0)    10128 2024-03-13 16:36:27.000000 fb_tools-2.5.0/test/test_40_app_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.512420 fb_tools-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)     7652 2024-04-13 05:57:36.000000 fb_tools-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2024-04-13 05:57:36.000000 fb_tools-2.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-04-13 05:57:57.512420 fb_tools-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2024-04-13 05:57:36.000000 fb_tools-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.500420 fb_tools-2.5.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2298 2024-04-13 05:57:36.000000 fb_tools-2.5.1/bin/get-file-to-remove
+-rwxr-xr-x   0 root         (0) root         (0)     2286 2024-04-13 05:57:36.000000 fb_tools-2.5.1/bin/myip
+-rwxr-xr-x   0 root         (0) root         (0)     2293 2024-04-13 05:57:36.000000 fb_tools-2.5.1/bin/update-ddns
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.496420 fb_tools-2.5.1/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.504420 fb_tools-2.5.1/lib/fb_tools/
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29242 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/argparse_actions.py
+-rw-r--r--   0 root         (0) root         (0)     9465 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/cfg_app.py
+-rw-r--r--   0 root         (0) root         (0)    36990 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/collections.py
+-rw-r--r--   0 root         (0) root         (0)    30170 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/common.py
+-rw-r--r--   0 root         (0) root         (0)     7978 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.504420 fb_tools-2.5.1/lib/fb_tools/ddns/
+-rw-r--r--   0 root         (0) root         (0)    20366 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/ddns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12479 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/ddns/config.py
+-rw-r--r--   0 root         (0) root         (0)     4516 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/ddns/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5594 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/ddns/myip_app.py
+-rw-r--r--   0 root         (0) root         (0)    27714 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/ddns/update_app.py
+-rw-r--r--   0 root         (0) root         (0)    19921 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/errors.py
+-rw-r--r--   0 root         (0) root         (0)    24586 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/get_file_rm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.504420 fb_tools-2.5.1/lib/fb_tools/handler/
+-rw-r--r--   0 root         (0) root         (0)    13864 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42608 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/handler/lock.py
+-rw-r--r--   0 root         (0) root         (0)    43592 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/handling_obj.py
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    34985 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/mailaddress.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.508420 fb_tools-2.5.1/lib/fb_tools/multi_config/
+-rw-r--r--   0 root         (0) root         (0)    20431 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/multi_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/multi_config/files.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/multi_config/inits.py
+-rw-r--r--   0 root         (0) root         (0)    11922 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/multi_config/read.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/obj.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/pidfile.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-04-13 05:57:36.000000 fb_tools-2.5.1/lib/fb_tools/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.512420 fb_tools-2.5.1/lib/fb_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 05:57:57.000000 fb_tools-2.5.1/lib/fb_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.508420 fb_tools-2.5.1/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.496420 fb_tools-2.5.1/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.508420 fb_tools-2.5.1/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    47617 2024-04-13 05:57:57.000000 fb_tools-2.5.1/locale/de/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    69131 2024-04-13 05:57:36.000000 fb_tools-2.5.1/locale/de/LC_MESSAGES/fb_tools.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.496420 fb_tools-2.5.1/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.508420 fb_tools-2.5.1/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     6156 2024-04-13 05:57:57.000000 fb_tools-2.5.1/locale/en/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    49500 2024-04-13 05:57:36.000000 fb_tools-2.5.1/locale/en/LC_MESSAGES/fb_tools.po
+-rw-r--r--   0 root         (0) root         (0)    47320 2024-04-13 05:57:36.000000 fb_tools-2.5.1/locale/fb_tools.pot
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-13 05:57:57.512420 fb_tools-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8889 2024-04-13 05:57:36.000000 fb_tools-2.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:57:57.512420 fb_tools-2.5.1/test/
+-rwxr-xr-x   0 root         (0) root         (0)      270 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/call_script.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/call_sleep.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/do_sleep
+-rw-r--r--   0 root         (0) root         (0)     4756 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     5221 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    26677 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     6873 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_10_base_object.py
+-rwxr-xr-x   0 root         (0) root         (0)    61659 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_13_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)    52551 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_15_mailaddress.py
+-rwxr-xr-x   0 root         (0) root         (0)    23387 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_17_multicfg.py
+-rwxr-xr-x   0 root         (0) root         (0)     6078 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_18_pidfile.py
+-rwxr-xr-x   0 root         (0) root         (0)    23666 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_20_handling_object.py
+-rwxr-xr-x   0 root         (0) root         (0)     7698 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_25_ddns_update_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8159 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_30_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    15313 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_33_lock.py
+-rwxr-xr-x   0 root         (0) root         (0)    10128 2024-04-13 05:57:36.000000 fb_tools-2.5.1/test/test_40_app_modules.py
```

### Comparing `fb_tools-2.5.0/LICENSE` & `fb_tools-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/PKG-INFO` & `fb_tools-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.5.0
+Version: 2.5.1
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.5.0/bin/get-file-to-remove` & `fb_tools-2.5.1/bin/get-file-to-remove`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/bin/myip` & `fb_tools-2.5.1/bin/myip`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/bin/update-ddns` & `fb_tools-2.5.1/bin/update-ddns`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/__init__.py` & `fb_tools-2.5.1/lib/fb_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 DDNS_CFG_BASENAME = 'ddns.ini'
 MAX_TIMEOUT = 3600
 UTF8_ENCODING = 'utf-8'
 DEFAULT_ENCODING = UTF8_ENCODING
 DEFAULT_TERMINAL_WIDTH = 99
 DEFAULT_TERMINAL_HEIGHT = 40
 
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 
 from .mailaddress import MailAddress, QualifiedMailAddress, MailAddressList     # noqa
 from .multi_config import BaseMultiConfig                                       # noqa
 
 # vim: ts=4 et list
```

### Comparing `fb_tools-2.5.0/lib/fb_tools/app.py` & `fb_tools-2.5.1/lib/fb_tools/app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/argparse_actions.py` & `fb_tools-2.5.1/lib/fb_tools/argparse_actions.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/cfg_app.py` & `fb_tools-2.5.1/lib/fb_tools/cfg_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/collections.py` & `fb_tools-2.5.1/lib/fb_tools/collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/common.py` & `fb_tools-2.5.1/lib/fb_tools/common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/config.py` & `fb_tools-2.5.1/lib/fb_tools/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/ddns/__init__.py` & `fb_tools-2.5.1/lib/fb_tools/ddns/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/ddns/config.py` & `fb_tools-2.5.1/lib/fb_tools/ddns/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/ddns/errors.py` & `fb_tools-2.5.1/lib/fb_tools/ddns/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/ddns/myip_app.py` & `fb_tools-2.5.1/lib/fb_tools/ddns/myip_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/ddns/update_app.py` & `fb_tools-2.5.1/lib/fb_tools/ddns/update_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/errors.py` & `fb_tools-2.5.1/lib/fb_tools/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/get_file_rm_app.py` & `fb_tools-2.5.1/lib/fb_tools/get_file_rm_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/handler/__init__.py` & `fb_tools-2.5.1/lib/fb_tools/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/handler/lock.py` & `fb_tools-2.5.1/lib/fb_tools/handler/lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/handling_obj.py` & `fb_tools-2.5.1/lib/fb_tools/handling_obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/mailaddress.py` & `fb_tools-2.5.1/lib/fb_tools/mailaddress.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Own modules
 from .common import is_sequence, pp, to_bool, to_str
 from .errors import EmptyMailAddressError
 from .errors import InvalidMailAddressError
 from .obj import FbBaseObject, FbGenericBaseObject
 from .xlate import XLATOR, format_list
 
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 def convert_attr(value):
@@ -44,16 +44,16 @@
 
 # =============================================================================
 class MailAddress(FbGenericBaseObject):
     """Class for encapsulating a mail simple address."""
 
     pat_valid_domain = r'@((?:[a-z0-9](?:[a-z0-9\-]*[a-z0-9])?\.)+[a-z][a-z]+)'
 
-    pat_valid_user = r'([a-z0-9](?:[a-z0-9_\-\.\+]*[a-z0-9])?'
-    pat_valid_user += r'(?:\+[a-z0-9][a-z0-9_\-\.]*[a-z0-9])*)'
+    pat_valid_user = r'([a-z0-9](?:[a-z0-9_\-\.\+=/]*[a-z0-9=\-_])?'
+    pat_valid_user += r'(?:\+[a-z0-9][a-z0-9_\-\.=/]*[a-z0-9=\-_])*)'
 
     pat_valid_address = pat_valid_user + pat_valid_domain
 
     re_valid_user = re.compile(r'^' + pat_valid_user + r'$', re.IGNORECASE)
     re_valid_domain = re.compile(r'^' + pat_valid_domain + r'$', re.IGNORECASE)
     re_valid_address = re.compile(r'^' + pat_valid_address + r'$', re.IGNORECASE)
```

### Comparing `fb_tools-2.5.0/lib/fb_tools/merge.py` & `fb_tools-2.5.1/lib/fb_tools/merge.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/multi_config/__init__.py` & `fb_tools-2.5.1/lib/fb_tools/multi_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/multi_config/files.py` & `fb_tools-2.5.1/lib/fb_tools/multi_config/files.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/multi_config/inits.py` & `fb_tools-2.5.1/lib/fb_tools/multi_config/inits.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/multi_config/read.py` & `fb_tools-2.5.1/lib/fb_tools/multi_config/read.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/obj.py` & `fb_tools-2.5.1/lib/fb_tools/obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/pidfile.py` & `fb_tools-2.5.1/lib/fb_tools/pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools/xlate.py` & `fb_tools-2.5.1/lib/fb_tools/xlate.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/lib/fb_tools.egg-info/PKG-INFO` & `fb_tools-2.5.1/lib/fb_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.5.0
+Version: 2.5.1
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.5.0/lib/fb_tools.egg-info/SOURCES.txt` & `fb_tools-2.5.1/lib/fb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/locale/de/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.5.1/locale/de/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/locale/de/LC_MESSAGES/fb_tools.po` & `fb_tools-2.5.1/locale/de/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/locale/en/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.5.1/locale/en/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/locale/en/LC_MESSAGES/fb_tools.po` & `fb_tools-2.5.1/locale/en/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/locale/fb_tools.pot` & `fb_tools-2.5.1/locale/fb_tools.pot`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/setup.cfg` & `fb_tools-2.5.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
-ignore = E226,E302,E41,E402,W503,B902
+ignore = A005,E226,E302,E41,E402,W503,B902
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fb_tools-2.5.0/setup.py` & `fb_tools-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/general.py` & `fb_tools-2.5.1/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_00_errors.py` & `fb_tools-2.5.1/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_05_common.py` & `fb_tools-2.5.1/test/test_05_common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_10_base_object.py` & `fb_tools-2.5.1/test/test_10_base_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_13_collections.py` & `fb_tools-2.5.1/test/test_13_collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_15_mailaddress.py` & `fb_tools-2.5.1/test/test_15_mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_17_multicfg.py` & `fb_tools-2.5.1/test/test_17_multicfg.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_18_pidfile.py` & `fb_tools-2.5.1/test/test_18_pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_20_handling_object.py` & `fb_tools-2.5.1/test/test_20_handling_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_25_ddns_update_status.py` & `fb_tools-2.5.1/test/test_25_ddns_update_status.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_30_base_handler.py` & `fb_tools-2.5.1/test/test_30_base_handler.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_33_lock.py` & `fb_tools-2.5.1/test/test_33_lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.0/test/test_40_app_modules.py` & `fb_tools-2.5.1/test/test_40_app_modules.py`

 * *Files identical despite different names*

