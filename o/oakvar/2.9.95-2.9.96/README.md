# Comparing `tmp/oakvar-2.9.95.tar.gz` & `tmp/oakvar-2.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakvar-2.9.95.tar", last modified: Thu Apr 11 21:59:14 2024, max compression
+gzip compressed data, was "oakvar-2.9.96.tar", last modified: Sat Apr 13 13:14:04 2024, max compression
```

## Comparing `oakvar-2.9.95.tar` & `oakvar-2.9.96.tar`

### file list

```diff
@@ -1,553 +1,553 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.511283 oakvar-2.9.95/
--rw-r--r--   0 rick       (501) staff       (20)     1753 2023-12-05 15:09:56.000000 oakvar-2.9.95/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-11 21:59:14.511088 oakvar-2.9.95/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     2339 2024-04-10 11:35:38.000000 oakvar-2.9.95/README.rst
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.439739 oakvar-2.9.95/cravat/
--rw-r--r--   0 rick       (501) staff       (20)       21 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/__main__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.440418 oakvar-2.9.95/cravat/api/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/config.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.440756 oakvar-2.9.95/cravat/api/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/module/ls_logic.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/new.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.440866 oakvar-2.9.95/cravat/api/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.440978 oakvar-2.9.95/cravat/api/store/account/
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/system.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/test.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/api/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.442410 oakvar-2.9.95/cravat/cli/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/config.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/gui.py
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/issue.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/license.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.442828 oakvar-2.9.95/cravat/cli/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/module/info_fn.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/module/ls.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/new.py
--rw-r--r--   0 rick       (501) staff       (20)      110 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/report.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/run.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.442935 oakvar-2.9.95/cravat/cli/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.443050 oakvar-2.9.95/cravat/cli/store/account/
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/system.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/test.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/update.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/util.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cli/version.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/constants.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/cravat_report.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.444485 oakvar-2.9.95/cravat/gui/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/job_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/multiuser.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/server.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/serveradmindb.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/store_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/system_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/system_message_db.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/system_worker.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/userjob.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/util.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/web_submit.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.444927 oakvar-2.9.95/cravat/gui/webresult/
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/webresult/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       48 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/webresult/jsonreporter.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/webresult/webresult.py
--rw-r--r--   0 rick       (501) staff       (20)       44 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/gui/websocket_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/inout.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445264 oakvar-2.9.95/cravat/lib/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.432510 oakvar-2.9.95/cravat/lib/assets/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.432873 oakvar-2.9.95/cravat/lib/assets/module_templates/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445397 oakvar-2.9.95/cravat/lib/assets/module_templates/annotator/
--rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/annotator/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445514 oakvar-2.9.95/cravat/lib/assets/module_templates/converter/
--rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/converter/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445631 oakvar-2.9.95/cravat/lib/assets/module_templates/mapper/
--rw-r--r--   0 rick       (501) staff       (20)       65 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/mapper/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445746 oakvar-2.9.95/cravat/lib/assets/module_templates/postaggregator/
--rw-r--r--   0 rick       (501) staff       (20)       73 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/postaggregator/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445865 oakvar-2.9.95/cravat/lib/assets/module_templates/preparer/
--rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/preparer/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.445986 oakvar-2.9.95/cravat/lib/assets/module_templates/reporter/
--rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/assets/module_templates/reporter/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.447654 oakvar-2.9.95/cravat/lib/base/
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/aggregator.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/annotator.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/app.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/commonmodule.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/converter.py
--rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/mapper.py
--rw-r--r--   0 rick       (501) staff       (20)       47 2024-01-10 14:33:05.000000 oakvar-2.9.95/cravat/lib/base/master_converter.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2024-01-10 14:33:05.000000 oakvar-2.9.95/cravat/lib/base/mp_runners.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/postaggregator.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/preparer.py
--rw-r--r--   0 rick       (501) staff       (20)       44 2024-01-10 14:33:05.000000 oakvar-2.9.95/cravat/lib/base/report_filter.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/reporter.py
--rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/runner.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/base/vcf2vcf.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.448219 oakvar-2.9.95/cravat/lib/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/module/cache.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/module/data_cache.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/module/local.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/module/remote.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.448554 oakvar-2.9.95/cravat/lib/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/store/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/store/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/store/db.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.448666 oakvar-2.9.95/cravat/lib/store/ov/
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/store/ov/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.448778 oakvar-2.9.95/cravat/lib/store/ov/account/
--rw-r--r--   0 rick       (501) staff       (20)       42 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/store/ov/account/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.449003 oakvar-2.9.95/cravat/lib/system/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/system/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/system/consts.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.450391 oakvar-2.9.95/cravat/lib/util/
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/admin_util.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/asyn.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:35:34.000000 oakvar-2.9.95/cravat/lib/util/db.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/download.py
--rw-r--r--   0 rick       (501) staff       (20)       47 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/download_library.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/image.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/inout.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/run.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/seq.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.95/cravat/lib/util/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.450613 oakvar-2.9.95/oakvar/
--rw-r--r--   0 rick       (501) staff       (20)     6681 2024-03-03 15:20:39.000000 oakvar-2.9.95/oakvar/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     7901 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/__main__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.451997 oakvar-2.9.95/oakvar/api/
--rw-r--r--   0 rick       (501) staff       (20)    19785 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/api/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     3144 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/api/config.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.452368 oakvar-2.9.95/oakvar/api/module/
--rw-r--r--   0 rick       (501) staff       (20)    18616 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/api/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     5305 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/api/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)     5687 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/api/module/ls_logic.py
--rw-r--r--   0 rick       (501) staff       (20)     3379 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/api/new.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.452491 oakvar-2.9.95/oakvar/api/store/
--rw-r--r--   0 rick       (501) staff       (20)     7179 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/api/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.452606 oakvar-2.9.95/oakvar/api/store/account/
--rw-r--r--   0 rick       (501) staff       (20)     4130 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/api/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     4510 2023-12-23 13:35:34.000000 oakvar-2.9.95/oakvar/api/system.py
--rw-r--r--   0 rick       (501) staff       (20)    34086 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/api/test.py
--rw-r--r--   0 rick       (501) staff       (20)    18455 2024-02-23 14:56:17.000000 oakvar-2.9.95/oakvar/api/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.454181 oakvar-2.9.95/oakvar/cli/
--rw-r--r--   0 rick       (501) staff       (20)     4470 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     4949 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/config.py
--rw-r--r--   0 rick       (501) staff       (20)    10930 2023-12-23 13:35:34.000000 oakvar-2.9.95/oakvar/cli/gui.py
--rw-r--r--   0 rick       (501) staff       (20)     2297 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/issue.py
--rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/license.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.454854 oakvar-2.9.95/oakvar/cli/module/
--rw-r--r--   0 rick       (501) staff       (20)    15171 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/cli/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     6422 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/module/info_fn.py
--rw-r--r--   0 rick       (501) staff       (20)     2410 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)     7792 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/module/ls.py
--rw-r--r--   0 rick       (501) staff       (20)     4408 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/new.py
--rw-r--r--   0 rick       (501) staff       (20)     6925 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/cli/report.py
--rw-r--r--   0 rick       (501) staff       (20)    11084 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/cli/run.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.455002 oakvar-2.9.95/oakvar/cli/store/
--rw-r--r--   0 rick       (501) staff       (20)     9370 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/cli/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.455151 oakvar-2.9.95/oakvar/cli/store/account/
--rw-r--r--   0 rick       (501) staff       (20)     7883 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     6736 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/system.py
--rw-r--r--   0 rick       (501) staff       (20)     2886 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/test.py
--rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/update.py
--rw-r--r--   0 rick       (501) staff       (20)     9339 2024-02-23 14:57:11.000000 oakvar-2.9.95/oakvar/cli/util.py
--rw-r--r--   0 rick       (501) staff       (20)     2474 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/cli/version.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.457012 oakvar-2.9.95/oakvar/gui/
--rw-r--r--   0 rick       (501) staff       (20)     2958 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/consts.py
--rw-r--r--   0 rick       (501) staff       (20)    28494 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/job_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)    11215 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/multiuser.py
--rw-r--r--   0 rick       (501) staff       (20)    17290 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/server.py
--rw-r--r--   0 rick       (501) staff       (20)    25415 2024-02-23 14:55:01.000000 oakvar-2.9.95/oakvar/gui/serveradmindb.py
--rw-r--r--   0 rick       (501) staff       (20)    15866 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/store_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)     8553 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/system_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)     3968 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/system_message_db.py
--rw-r--r--   0 rick       (501) staff       (20)     8117 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/system_worker.py
--rw-r--r--   0 rick       (501) staff       (20)     6042 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/userjob.py
--rw-r--r--   0 rick       (501) staff       (20)     7210 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/util.py
--rw-r--r--   0 rick       (501) staff       (20)    17662 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/web_submit.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.457872 oakvar-2.9.95/oakvar/gui/webresult/
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.457993 oakvar-2.9.95/oakvar/gui/webresult/css/
--rw-r--r--   0 rick       (501) staff       (20)     2389 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/css/pqselect.min.css
--rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/email.png
--rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/favicon.ico
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.459071 oakvar-2.9.95/oakvar/gui/webresult/fonts/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.476409 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/
--rw-r--r--   0 rick       (501) staff       (20)   138764 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
--rw-r--r--   0 rick       (501) staff       (20)   102868 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
--rw-r--r--   0 rick       (501) staff       (20)   146824 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   108752 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   143208 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
--rw-r--r--   0 rick       (501) staff       (20)   106140 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   151052 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111808 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142920 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
--rw-r--r--   0 rick       (501) staff       (20)   106108 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150628 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111708 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   140724 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
--rw-r--r--   0 rick       (501) staff       (20)   104232 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
--rw-r--r--   0 rick       (501) staff       (20)   149996 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111392 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   144372 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
--rw-r--r--   0 rick       (501) staff       (20)   106876 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   140632 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
--rw-r--r--   0 rick       (501) staff       (20)   104332 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150092 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111332 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142552 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
--rw-r--r--   0 rick       (501) staff       (20)   105924 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150988 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   112184 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   133844 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
--rw-r--r--   0 rick       (501) staff       (20)    98868 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142932 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
--rw-r--r--   0 rick       (501) staff       (20)   105804 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   151180 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   112048 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   135920 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
--rw-r--r--   0 rick       (501) staff       (20)    99632 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
--rw-r--r--   0 rick       (501) staff       (20)   145480 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   106496 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   245036 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)   227180 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)   324864 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)     5303 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/inter.css
--rw-r--r--   0 rick       (501) staff       (20)    26456 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    19508 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    25692 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    18980 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    26312 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    19416 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    33072 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    25740 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.479097 oakvar-2.9.95/oakvar/gui/webresult/images/
--rw-r--r--   0 rick       (501) staff       (20)      326 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      379 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-down-right.svg
--rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-down.svg
--rw-r--r--   0 rick       (501) staff       (20)      311 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-left.svg
--rw-r--r--   0 rick       (501) staff       (20)      312 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-right.svg
--rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrow-up.svg
--rw-r--r--   0 rick       (501) staff       (20)      706 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/arrows-move.svg
--rw-r--r--   0 rick       (501) staff       (20)     2140 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/camera.svg
--rw-r--r--   0 rick       (501) staff       (20)      291 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/caret-down.svg
--rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/caret-right.svg
--rw-r--r--   0 rick       (501) staff       (20)     3125 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/close.png
--rw-r--r--   0 rick       (501) staff       (20)     2390 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/close.svg
--rw-r--r--   0 rick       (501) staff       (20)      722 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/download-material-black.png
--rw-r--r--   0 rick       (501) staff       (20)     2066 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/download.svg
--rw-r--r--   0 rick       (501) staff       (20)      485 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/grip-vertical.svg
--rw-r--r--   0 rick       (501) staff       (20)     2219 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/pin.svg
--rw-r--r--   0 rick       (501) staff       (20)     2243 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 rick       (501) staff       (20)      280 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)     4645 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/sorry.png
--rw-r--r--   0 rick       (501) staff       (20)    25333 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/spinner.gif
--rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/x-lg.svg
--rw-r--r--   0 rick       (501) staff       (20)      332 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/images/x.svg
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.481896 oakvar-2.9.95/oakvar/gui/webresult/js/
--rw-r--r--   0 rick       (501) staff       (20)   398184 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/Chart.js
--rw-r--r--   0 rick       (501) staff       (20)    26580 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/axios.min.js
--rw-r--r--   0 rick       (501) staff       (20)   137820 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/axios.min.js.map
--rw-r--r--   0 rick       (501) staff       (20)     9278 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/dom-to-image.min.js
--rw-r--r--   0 rick       (501) staff       (20)     5839 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/download.js
--rw-r--r--   0 rick       (501) staff       (20)    12091 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
--rw-r--r--   0 rick       (501) staff       (20)   954164 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/graphics.js
--rw-r--r--   0 rick       (501) staff       (20)    86659 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.485164 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 rick       (501) staff       (20)    12660 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 rick       (501) staff       (20)     1817 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.434606 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.485291 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 rick       (501) staff       (20)   293430 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.486178 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 rick       (501) staff       (20)     6992 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6988 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6999 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6299 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)    32588 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 rick       (501) staff       (20)    35997 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 rick       (501) staff       (20)   520714 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 rick       (501) staff       (20)    30747 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 rick       (501) staff       (20)   253668 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 rick       (501) staff       (20)    18705 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 rick       (501) staff       (20)    15548 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 rick       (501) staff       (20)    17342 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 rick       (501) staff       (20)    13847 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 rick       (501) staff       (20)     1340 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 rick       (501) staff       (20)    13171 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery.tools.min.js
--rw-r--r--   0 rick       (501) staff       (20)     5451 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/jquery.url.js
--rw-r--r--   0 rick       (501) staff       (20)    24103 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/masonry.pkgd.min.js
--rw-r--r--   0 rick       (501) staff       (20)    84772 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.488272 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/
--rw-r--r--   0 rick       (501) staff       (20)    11583 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)   103213 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.489394 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 rick       (501) staff       (20)      230 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      210 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      771 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 rick       (501) staff       (20)     1668 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 rick       (501) staff       (20)       76 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 rick       (501) staff       (20)      216 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      201 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.489637 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 rick       (501) staff       (20)     1148 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 rick       (501) staff       (20)    76985 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.491176 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 rick       (501) staff       (20)      755 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 rick       (501) staff       (20)      750 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 rick       (501) staff       (20)      769 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 rick       (501) staff       (20)      802 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 rick       (501) staff       (20)      813 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 rick       (501) staff       (20)      805 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 rick       (501) staff       (20)      636 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 rick       (501) staff       (20)      774 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 rick       (501) staff       (20)      782 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 rick       (501) staff       (20)      822 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 rick       (501) staff       (20)      773 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 rick       (501) staff       (20)      675 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.491979 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 rick       (501) staff       (20)     1105 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)      613 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 rick       (501) staff       (20)      541 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 rick       (501) staff       (20)     2973 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 rick       (501) staff       (20)    27759 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 rick       (501) staff       (20)     2383 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 rick       (501) staff       (20)    12577 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 rick       (501) staff       (20)     2408 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 rick       (501) staff       (20)     2026 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 rick       (501) staff       (20)    16145 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 rick       (501) staff       (20)   481365 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 rick       (501) staff       (20)    12757 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 rick       (501) staff       (20)   242931 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 rick       (501) staff       (20)     1646 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 rick       (501) staff       (20)     1278 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 rick       (501) staff       (20)      555 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.436072 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492107 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492229 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492338 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492458 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492576 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492694 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492814 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.492928 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493046 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493165 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493287 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493405 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493517 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493643 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.493769 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.494357 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 rick       (501) staff       (20)     1042 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)     1164 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 rick       (501) staff       (20)     2677 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 rick       (501) staff       (20)     3716 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 rick       (501) staff       (20)     1847 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 rick       (501) staff       (20)    12583 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/pqselect.min.js
--rw-r--r--   0 rick       (501) staff       (20)    92225 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/raphael-min.js
--rw-r--r--   0 rick       (501) staff       (20)   326538 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/js/tailwind.min.js
--rw-r--r--   0 rick       (501) staff       (20)     2732 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/webresult/jsonreporter.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.494586 oakvar-2.9.95/oakvar/gui/webresult/nocache/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.494964 oakvar-2.9.95/oakvar/gui/webresult/nocache/css/
--rw-r--r--   0 rick       (501) staff       (20)     1714 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 rick       (501) staff       (20)    22655 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/css/style.css
--rw-r--r--   0 rick       (501) staff       (20)     2658 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/css/widget.css
--rw-r--r--   0 rick       (501) staff       (20)    21597 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/index.html
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.496226 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/
--rw-r--r--   0 rick       (501) staff       (20)    24858 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/filter.js
--rw-r--r--   0 rick       (501) staff       (20)    13105 2023-12-09 16:39:48.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/infomgr.js
--rw-r--r--   0 rick       (501) staff       (20)    30870 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/main.js
--rw-r--r--   0 rick       (501) staff       (20)   103450 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/setup.js
--rw-r--r--   0 rick       (501) staff       (20)     4903 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/showvariant.js
--rw-r--r--   0 rick       (501) staff       (20)    35998 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 rick       (501) staff       (20)    28858 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/util.js
--rw-r--r--   0 rick       (501) staff       (20)     1696 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/variables.js
--rw-r--r--   0 rick       (501) staff       (20)    22262 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 rick       (501) staff       (20)     5440 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/nocache/variant.html
--rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/question.png
--rw-r--r--   0 rick       (501) staff       (20)    31615 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/webresult/webresult.py
--rw-r--r--   0 rick       (501) staff       (20)      163 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webresult/webviewer.yml
--rw-r--r--   0 rick       (501) staff       (20)     5907 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websocket_handlers.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.436528 oakvar-2.9.95/oakvar/gui/webstore/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.498068 oakvar-2.9.95/oakvar/gui/webstore/images/
--rw-r--r--   0 rick       (501) staff       (20)      446 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      740 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/chat-dots.svg
--rw-r--r--   0 rick       (501) staff       (20)      396 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      545 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/chat-left-text.svg
--rw-r--r--   0 rick       (501) staff       (20)    22268 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/done.png
--rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/email.png
--rw-r--r--   0 rick       (501) staff       (20)     2226 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/empty.png
--rw-r--r--   0 rick       (501) staff       (20)     1763 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/folder.png
--rw-r--r--   0 rick       (501) staff       (20)    38197 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/genericmodulelogo.png
--rw-r--r--   0 rick       (501) staff       (20)     4766 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/hamburger.png
--rw-r--r--   0 rick       (501) staff       (20)     1194 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/left_arrow.png
--rw-r--r--   0 rick       (501) staff       (20)     3524 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/new.png
--rw-r--r--   0 rick       (501) staff       (20)      474 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/no_logo_module.svg
--rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/question.png
--rw-r--r--   0 rick       (501) staff       (20)     1214 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/right_arrow.png
--rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/webstore/images/x-lg.svg
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.436797 oakvar-2.9.95/oakvar/gui/websubmit/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.499701 oakvar-2.9.95/oakvar/gui/websubmit/images/
--rw-r--r--   0 rick       (501) staff       (20)   372952 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/images/background.png
--rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/images/logo.png
--rw-r--r--   0 rick       (501) staff       (20)    22716 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/images/logo_only.png
--rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/images/logo_transparent.png
--rw-r--r--   0 rick       (501) staff       (20)    22247 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/images/logo_transparent_bw.png
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.499838 oakvar-2.9.95/oakvar/gui/websubmit/inputexamples/
--rw-r--r--   0 rick       (501) staff       (20)     9036 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/inputexamples/exampleinput
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.501851 oakvar-2.9.95/oakvar/gui/websubmit/nocache/
--rw-r--r--   0 rick       (501) staff       (20)      692 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/alerts.js
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/element_constructors.js
--rw-r--r--   0 rick       (501) staff       (20)     6756 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/element_getters.js
--rw-r--r--   0 rick       (501) staff       (20)    55822 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/index.html
--rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/input.js
--rw-r--r--   0 rick       (501) staff       (20)    14408 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/jobstable.js
--rw-r--r--   0 rick       (501) staff       (20)     8242 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/login.html
--rw-r--r--   0 rick       (501) staff       (20)     3796 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/multiuser.css
--rw-r--r--   0 rick       (501) staff       (20)    16797 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/multiuser.js
--rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/select_modules.js
--rw-r--r--   0 rick       (501) staff       (20)      228 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/showhide.js
--rw-r--r--   0 rick       (501) staff       (20)     6783 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/submit.js
--rw-r--r--   0 rick       (501) staff       (20)      484 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/util.js
--rw-r--r--   0 rick       (501) staff       (20)    11319 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/websubmit.css
--rw-r--r--   0 rick       (501) staff       (20)    39200 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/gui/websubmit/nocache/websubmit.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.502134 oakvar-2.9.95/oakvar/gui/www/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.502422 oakvar-2.9.95/oakvar/gui/www/assets/
--rw-r--r--   0 rick       (501) staff       (20)    63287 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/www/assets/index.3526e7ae.css
--rw-r--r--   0 rick       (501) staff       (20)   834933 2023-12-09 16:39:48.000000 oakvar-2.9.95/oakvar/gui/www/assets/index.5e1d7274.js
--rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/gui/www/favicon.ico
--rw-r--r--   0 rick       (501) staff       (20)     2074 2023-12-09 16:39:48.000000 oakvar-2.9.95/oakvar/gui/www/index.html
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.503182 oakvar-2.9.95/oakvar/lib/
--rw-r--r--   0 rick       (501) staff       (20)     1946 2024-03-03 16:46:38.000000 oakvar-2.9.95/oakvar/lib/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.503973 oakvar-2.9.95/oakvar/lib/assets/
--rw-r--r--   0 rick       (501) staff       (20)     9036 2024-04-10 11:35:01.000000 oakvar-2.9.95/oakvar/lib/assets/exampleinput
--rw-r--r--   0 rick       (501) staff       (20)    16880 2024-02-08 01:06:28.000000 oakvar-2.9.95/oakvar/lib/assets/hg19.chromAlias.txt
--rw-r--r--   0 rick       (501) staff       (20)    27240 2024-02-08 00:52:40.000000 oakvar-2.9.95/oakvar/lib/assets/hg38.chromAlias.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.504195 oakvar-2.9.95/oakvar/lib/assets/license/
--rw-r--r--   0 rick       (501) staff       (20)     1707 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/license/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)     1330 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/license/liftover.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.437661 oakvar-2.9.95/oakvar/lib/assets/module_templates/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.504513 oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2109 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1195 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.504874 oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.md
--rw-r--r--   0 rick       (501) staff       (20)     4366 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1249 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.505219 oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.md
--rw-r--r--   0 rick       (501) staff       (20)     3078 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1120 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.505550 oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2563 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1335 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.505891 oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2033 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1327 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.506216 oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.md
--rw-r--r--   0 rick       (501) staff       (20)     3574 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1246 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.yml
--rw-r--r--   0 rick       (501) staff       (20)      135 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/oakvar.yml
--rw-r--r--   0 rick       (501) staff       (20)    10314 2024-04-10 12:11:07.000000 oakvar-2.9.95/oakvar/lib/assets/oakvar_example.vcf
--rw-r--r--   0 rick       (501) staff       (20)     3060 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/assets/output_columns.yml
--rw-r--r--   0 rick       (501) staff       (20)      768 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/assets/system.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.508127 oakvar-2.9.95/oakvar/lib/base/
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/base/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)    22714 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/aggregator.py
--rw-r--r--   0 rick       (501) staff       (20)    36762 2024-03-03 18:25:36.000000 oakvar-2.9.95/oakvar/lib/base/annotator.py
--rw-r--r--   0 rick       (501) staff       (20)     2588 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/base/app.py
--rw-r--r--   0 rick       (501) staff       (20)     4546 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/base/commonmodule.py
--rw-r--r--   0 rick       (501) staff       (20)     5216 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/converter.py
--rw-r--r--   0 rick       (501) staff       (20)    13627 2024-03-03 16:41:12.000000 oakvar-2.9.95/oakvar/lib/base/mapper.py
--rw-r--r--   0 rick       (501) staff       (20)    43499 2024-02-19 19:29:51.000000 oakvar-2.9.95/oakvar/lib/base/master_converter.py
--rw-r--r--   0 rick       (501) staff       (20)     4982 2024-03-03 18:25:36.000000 oakvar-2.9.95/oakvar/lib/base/mp_runners.py
--rw-r--r--   0 rick       (501) staff       (20)    27573 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/postaggregator.py
--rw-r--r--   0 rick       (501) staff       (20)     8852 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/preparer.py
--rw-r--r--   0 rick       (501) staff       (20)    44997 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/report_filter.py
--rw-r--r--   0 rick       (501) staff       (20)    44831 2024-03-07 14:37:13.000000 oakvar-2.9.95/oakvar/lib/base/reporter.py
--rw-r--r--   0 rick       (501) staff       (20)    84125 2024-03-07 14:36:39.000000 oakvar-2.9.95/oakvar/lib/base/runner.py
--rw-r--r--   0 rick       (501) staff       (20)    17018 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/base/vcf2vcf.py
--rw-r--r--   0 rick       (501) staff       (20)     4452 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/consts.py
--rw-r--r--   0 rick       (501) staff       (20)     9623 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.508767 oakvar-2.9.95/oakvar/lib/module/
--rw-r--r--   0 rick       (501) staff       (20)    32253 2024-04-11 21:57:44.000000 oakvar-2.9.95/oakvar/lib/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     5975 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/module/cache.py
--rw-r--r--   0 rick       (501) staff       (20)     5355 2023-12-05 15:09:56.000000 oakvar-2.9.95/oakvar/lib/module/data_cache.py
--rw-r--r--   0 rick       (501) staff       (20)    31979 2024-03-12 01:32:28.000000 oakvar-2.9.95/oakvar/lib/module/local.py
--rw-r--r--   0 rick       (501) staff       (20)    13243 2023-12-09 16:39:48.000000 oakvar-2.9.95/oakvar/lib/module/remote.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.509149 oakvar-2.9.95/oakvar/lib/store/
--rw-r--r--   0 rick       (501) staff       (20)     6162 2023-12-05 15:09:57.000000 oakvar-2.9.95/oakvar/lib/store/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     2483 2023-12-05 15:09:57.000000 oakvar-2.9.95/oakvar/lib/store/consts.py
--rw-r--r--   0 rick       (501) staff       (20)    28024 2024-04-11 14:27:45.000000 oakvar-2.9.95/oakvar/lib/store/db.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.509276 oakvar-2.9.95/oakvar/lib/store/ov/
--rw-r--r--   0 rick       (501) staff       (20)     9948 2024-04-11 04:57:50.000000 oakvar-2.9.95/oakvar/lib/store/ov/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.509394 oakvar-2.9.95/oakvar/lib/store/ov/account/
--rw-r--r--   0 rick       (501) staff       (20)    21588 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/store/ov/account/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.509644 oakvar-2.9.95/oakvar/lib/system/
--rw-r--r--   0 rick       (501) staff       (20)    43831 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/system/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     3126 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/system/consts.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.510858 oakvar-2.9.95/oakvar/lib/util/
--rw-r--r--   0 rick       (501) staff       (20)     2214 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/util/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     7408 2024-04-10 23:40:21.000000 oakvar-2.9.95/oakvar/lib/util/admin_util.py
--rw-r--r--   0 rick       (501) staff       (20)     2576 2023-12-05 15:09:57.000000 oakvar-2.9.95/oakvar/lib/util/asyn.py
--rw-r--r--   0 rick       (501) staff       (20)     8251 2024-02-23 15:11:11.000000 oakvar-2.9.95/oakvar/lib/util/db.py
--rw-r--r--   0 rick       (501) staff       (20)     6939 2023-12-09 16:39:48.000000 oakvar-2.9.95/oakvar/lib/util/download.py
--rw-r--r--   0 rick       (501) staff       (20)    20964 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/util/download_library.py
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:57.000000 oakvar-2.9.95/oakvar/lib/util/image.py
--rw-r--r--   0 rick       (501) staff       (20)    23939 2024-02-08 00:22:22.000000 oakvar-2.9.95/oakvar/lib/util/inout.py
--rw-r--r--   0 rick       (501) staff       (20)    10460 2024-03-07 14:36:39.000000 oakvar-2.9.95/oakvar/lib/util/run.py
--rw-r--r--   0 rick       (501) staff       (20)    14974 2024-03-22 00:57:28.000000 oakvar-2.9.95/oakvar/lib/util/seq.py
--rw-r--r--   0 rick       (501) staff       (20)    22030 2024-01-10 14:33:05.000000 oakvar-2.9.95/oakvar/lib/util/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-11 21:59:14.451271 oakvar-2.9.95/oakvar.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)    18985 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)       44 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/entry_points.txt
--rw-r--r--   0 rick       (501) staff       (20)      291 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       14 2024-04-11 21:59:14.000000 oakvar-2.9.95/oakvar.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)      625 2023-12-05 15:09:57.000000 oakvar-2.9.95/pyproject.toml
--rw-r--r--   0 rick       (501) staff       (20)       38 2024-04-11 21:59:14.511337 oakvar-2.9.95/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)     2443 2024-04-11 21:58:06.000000 oakvar-2.9.95/setup.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.291881 oakvar-2.9.96/
+-rw-r--r--   0 rick       (501) staff       (20)     1753 2023-12-05 15:09:56.000000 oakvar-2.9.96/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-13 13:14:04.291695 oakvar-2.9.96/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     2339 2024-04-10 11:35:38.000000 oakvar-2.9.96/README.rst
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.210358 oakvar-2.9.96/cravat/
+-rw-r--r--   0 rick       (501) staff       (20)       21 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/__main__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.211267 oakvar-2.9.96/cravat/api/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/config.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.211699 oakvar-2.9.96/cravat/api/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/module/ls_logic.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/new.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.211828 oakvar-2.9.96/cravat/api/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.211973 oakvar-2.9.96/cravat/api/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/system.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/test.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/api/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.213711 oakvar-2.9.96/cravat/cli/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/config.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/gui.py
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/issue.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/license.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.214217 oakvar-2.9.96/cravat/cli/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/module/info_fn.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/module/ls.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/new.py
+-rw-r--r--   0 rick       (501) staff       (20)      110 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/report.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/run.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.214538 oakvar-2.9.96/cravat/cli/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.214674 oakvar-2.9.96/cravat/cli/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/system.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/test.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/update.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/util.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cli/version.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/constants.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/cravat_report.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.216327 oakvar-2.9.96/cravat/gui/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/job_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/multiuser.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/server.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/serveradmindb.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/store_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/system_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/system_message_db.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/system_worker.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/userjob.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/util.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/web_submit.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.216702 oakvar-2.9.96/cravat/gui/webresult/
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/webresult/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       48 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/webresult/jsonreporter.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/webresult/webresult.py
+-rw-r--r--   0 rick       (501) staff       (20)       44 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/gui/websocket_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/inout.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217071 oakvar-2.9.96/cravat/lib/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.203206 oakvar-2.9.96/cravat/lib/assets/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.203545 oakvar-2.9.96/cravat/lib/assets/module_templates/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217201 oakvar-2.9.96/cravat/lib/assets/module_templates/annotator/
+-rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/annotator/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217341 oakvar-2.9.96/cravat/lib/assets/module_templates/converter/
+-rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/converter/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217483 oakvar-2.9.96/cravat/lib/assets/module_templates/mapper/
+-rw-r--r--   0 rick       (501) staff       (20)       65 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/mapper/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217615 oakvar-2.9.96/cravat/lib/assets/module_templates/postaggregator/
+-rw-r--r--   0 rick       (501) staff       (20)       73 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/postaggregator/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217740 oakvar-2.9.96/cravat/lib/assets/module_templates/preparer/
+-rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/preparer/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.217876 oakvar-2.9.96/cravat/lib/assets/module_templates/reporter/
+-rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/assets/module_templates/reporter/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.219763 oakvar-2.9.96/cravat/lib/base/
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/aggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/annotator.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/app.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/commonmodule.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/converter.py
+-rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/mapper.py
+-rw-r--r--   0 rick       (501) staff       (20)       47 2024-01-10 14:33:05.000000 oakvar-2.9.96/cravat/lib/base/master_converter.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2024-01-10 14:33:05.000000 oakvar-2.9.96/cravat/lib/base/mp_runners.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/postaggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/preparer.py
+-rw-r--r--   0 rick       (501) staff       (20)       44 2024-01-10 14:33:05.000000 oakvar-2.9.96/cravat/lib/base/report_filter.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/reporter.py
+-rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/runner.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/base/vcf2vcf.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.220403 oakvar-2.9.96/cravat/lib/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/module/cache.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/module/data_cache.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/module/local.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/module/remote.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.220764 oakvar-2.9.96/cravat/lib/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/store/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/store/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/store/db.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.220903 oakvar-2.9.96/cravat/lib/store/ov/
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/store/ov/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.221033 oakvar-2.9.96/cravat/lib/store/ov/account/
+-rw-r--r--   0 rick       (501) staff       (20)       42 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/store/ov/account/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.221294 oakvar-2.9.96/cravat/lib/system/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/system/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/system/consts.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.222662 oakvar-2.9.96/cravat/lib/util/
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/admin_util.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/asyn.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:35:34.000000 oakvar-2.9.96/cravat/lib/util/db.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/download.py
+-rw-r--r--   0 rick       (501) staff       (20)       47 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/download_library.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/image.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/inout.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/run.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/seq.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.96/cravat/lib/util/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.222911 oakvar-2.9.96/oakvar/
+-rw-r--r--   0 rick       (501) staff       (20)     6681 2024-03-03 15:20:39.000000 oakvar-2.9.96/oakvar/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     7901 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/__main__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.224268 oakvar-2.9.96/oakvar/api/
+-rw-r--r--   0 rick       (501) staff       (20)    19785 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/api/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     3144 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/api/config.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.224760 oakvar-2.9.96/oakvar/api/module/
+-rw-r--r--   0 rick       (501) staff       (20)    19114 2024-04-13 11:21:21.000000 oakvar-2.9.96/oakvar/api/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     5305 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/api/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)     5687 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/api/module/ls_logic.py
+-rw-r--r--   0 rick       (501) staff       (20)     3379 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/api/new.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.224963 oakvar-2.9.96/oakvar/api/store/
+-rw-r--r--   0 rick       (501) staff       (20)     7179 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/api/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.225072 oakvar-2.9.96/oakvar/api/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)     4130 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/api/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     4510 2023-12-23 13:35:34.000000 oakvar-2.9.96/oakvar/api/system.py
+-rw-r--r--   0 rick       (501) staff       (20)    34086 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/api/test.py
+-rw-r--r--   0 rick       (501) staff       (20)    18455 2024-02-23 14:56:17.000000 oakvar-2.9.96/oakvar/api/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.226711 oakvar-2.9.96/oakvar/cli/
+-rw-r--r--   0 rick       (501) staff       (20)     4470 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     4949 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/config.py
+-rw-r--r--   0 rick       (501) staff       (20)    10930 2023-12-23 13:35:34.000000 oakvar-2.9.96/oakvar/cli/gui.py
+-rw-r--r--   0 rick       (501) staff       (20)     2297 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/issue.py
+-rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/license.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.227270 oakvar-2.9.96/oakvar/cli/module/
+-rw-r--r--   0 rick       (501) staff       (20)    15171 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/cli/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     6422 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/module/info_fn.py
+-rw-r--r--   0 rick       (501) staff       (20)     2410 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)     7792 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/module/ls.py
+-rw-r--r--   0 rick       (501) staff       (20)     4408 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/new.py
+-rw-r--r--   0 rick       (501) staff       (20)     6925 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/cli/report.py
+-rw-r--r--   0 rick       (501) staff       (20)    11084 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/cli/run.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.227427 oakvar-2.9.96/oakvar/cli/store/
+-rw-r--r--   0 rick       (501) staff       (20)     9370 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/cli/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.227562 oakvar-2.9.96/oakvar/cli/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)     7883 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     6736 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/system.py
+-rw-r--r--   0 rick       (501) staff       (20)     2886 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/test.py
+-rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/update.py
+-rw-r--r--   0 rick       (501) staff       (20)     9339 2024-02-23 14:57:11.000000 oakvar-2.9.96/oakvar/cli/util.py
+-rw-r--r--   0 rick       (501) staff       (20)     2474 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/cli/version.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.229424 oakvar-2.9.96/oakvar/gui/
+-rw-r--r--   0 rick       (501) staff       (20)     2958 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)    28494 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/job_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)    11215 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/multiuser.py
+-rw-r--r--   0 rick       (501) staff       (20)    17290 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/server.py
+-rw-r--r--   0 rick       (501) staff       (20)    25415 2024-02-23 14:55:01.000000 oakvar-2.9.96/oakvar/gui/serveradmindb.py
+-rw-r--r--   0 rick       (501) staff       (20)    15866 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/store_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)     8553 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/system_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)     3968 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/system_message_db.py
+-rw-r--r--   0 rick       (501) staff       (20)     8117 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/system_worker.py
+-rw-r--r--   0 rick       (501) staff       (20)     6042 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/userjob.py
+-rw-r--r--   0 rick       (501) staff       (20)     7210 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/util.py
+-rw-r--r--   0 rick       (501) staff       (20)    17662 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/web_submit.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.230376 oakvar-2.9.96/oakvar/gui/webresult/
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.230479 oakvar-2.9.96/oakvar/gui/webresult/css/
+-rw-r--r--   0 rick       (501) staff       (20)     2389 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/css/pqselect.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/email.png
+-rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/favicon.ico
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.231494 oakvar-2.9.96/oakvar/gui/webresult/fonts/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.253674 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/
+-rw-r--r--   0 rick       (501) staff       (20)   138764 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
+-rw-r--r--   0 rick       (501) staff       (20)   102868 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   146824 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   108752 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   143208 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106140 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   151052 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111808 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142920 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106108 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150628 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111708 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   140724 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
+-rw-r--r--   0 rick       (501) staff       (20)   104232 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   149996 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111392 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   144372 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106876 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   140632 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
+-rw-r--r--   0 rick       (501) staff       (20)   104332 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150092 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111332 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142552 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
+-rw-r--r--   0 rick       (501) staff       (20)   105924 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150988 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   112184 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   133844 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
+-rw-r--r--   0 rick       (501) staff       (20)    98868 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142932 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   105804 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   151180 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   112048 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   135920 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
+-rw-r--r--   0 rick       (501) staff       (20)    99632 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   145480 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106496 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   245036 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   227180 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   324864 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)     5303 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/inter.css
+-rw-r--r--   0 rick       (501) staff       (20)    26456 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    19508 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    25692 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    18980 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    26312 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    19416 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    33072 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    25740 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.256675 oakvar-2.9.96/oakvar/gui/webresult/images/
+-rw-r--r--   0 rick       (501) staff       (20)      326 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      379 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-down.svg
+-rw-r--r--   0 rick       (501) staff       (20)      311 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-left.svg
+-rw-r--r--   0 rick       (501) staff       (20)      312 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrow-up.svg
+-rw-r--r--   0 rick       (501) staff       (20)      706 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/arrows-move.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2140 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/camera.svg
+-rw-r--r--   0 rick       (501) staff       (20)      291 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/caret-down.svg
+-rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/caret-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)     3125 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/close.png
+-rw-r--r--   0 rick       (501) staff       (20)     2390 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/close.svg
+-rw-r--r--   0 rick       (501) staff       (20)      722 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/download-material-black.png
+-rw-r--r--   0 rick       (501) staff       (20)     2066 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/download.svg
+-rw-r--r--   0 rick       (501) staff       (20)      485 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/grip-vertical.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2219 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/pin.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2243 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 rick       (501) staff       (20)      280 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)     4645 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/sorry.png
+-rw-r--r--   0 rick       (501) staff       (20)    25333 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/spinner.gif
+-rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/x-lg.svg
+-rw-r--r--   0 rick       (501) staff       (20)      332 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/images/x.svg
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.259764 oakvar-2.9.96/oakvar/gui/webresult/js/
+-rw-r--r--   0 rick       (501) staff       (20)   398184 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/Chart.js
+-rw-r--r--   0 rick       (501) staff       (20)    26580 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/axios.min.js
+-rw-r--r--   0 rick       (501) staff       (20)   137820 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/axios.min.js.map
+-rw-r--r--   0 rick       (501) staff       (20)     9278 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     5839 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/download.js
+-rw-r--r--   0 rick       (501) staff       (20)    12091 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
+-rw-r--r--   0 rick       (501) staff       (20)   954164 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/graphics.js
+-rw-r--r--   0 rick       (501) staff       (20)    86659 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.261921 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 rick       (501) staff       (20)    12660 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 rick       (501) staff       (20)     1817 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.205169 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.262032 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 rick       (501) staff       (20)   293430 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.263083 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 rick       (501) staff       (20)     6992 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6988 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6999 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6299 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)    32588 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 rick       (501) staff       (20)    35997 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 rick       (501) staff       (20)   520714 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 rick       (501) staff       (20)    30747 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 rick       (501) staff       (20)   253668 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    18705 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 rick       (501) staff       (20)    15548 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    17342 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 rick       (501) staff       (20)    13847 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     1340 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 rick       (501) staff       (20)    13171 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     5451 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/jquery.url.js
+-rw-r--r--   0 rick       (501) staff       (20)    24103 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/masonry.pkgd.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    84772 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.267025 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 rick       (501) staff       (20)    11583 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)   103213 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.268963 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 rick       (501) staff       (20)      230 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      210 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      771 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 rick       (501) staff       (20)     1668 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 rick       (501) staff       (20)       76 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 rick       (501) staff       (20)      216 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      201 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.269182 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 rick       (501) staff       (20)     1148 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 rick       (501) staff       (20)    76985 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.270536 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 rick       (501) staff       (20)      755 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 rick       (501) staff       (20)      750 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 rick       (501) staff       (20)      769 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 rick       (501) staff       (20)      802 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 rick       (501) staff       (20)      813 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 rick       (501) staff       (20)      805 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 rick       (501) staff       (20)      636 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 rick       (501) staff       (20)      774 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 rick       (501) staff       (20)      782 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 rick       (501) staff       (20)      822 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 rick       (501) staff       (20)      773 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 rick       (501) staff       (20)      675 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271352 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 rick       (501) staff       (20)     1105 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)      613 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)      541 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     2973 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)    27759 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)     2383 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    12577 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     2408 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)     2026 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    16145 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)   481365 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)    12757 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 rick       (501) staff       (20)   242931 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     1646 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)     1278 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 rick       (501) staff       (20)      555 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.206553 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271484 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271600 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271710 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271824 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.271936 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272053 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272166 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272277 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272387 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272499 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272611 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272722 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272836 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.272947 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.273073 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.273629 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 rick       (501) staff       (20)     1042 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)     1164 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 rick       (501) staff       (20)     2677 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 rick       (501) staff       (20)     3716 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)     1847 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    12583 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/pqselect.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    92225 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/raphael-min.js
+-rw-r--r--   0 rick       (501) staff       (20)   326538 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/js/tailwind.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     2732 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/webresult/jsonreporter.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.273871 oakvar-2.9.96/oakvar/gui/webresult/nocache/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.274382 oakvar-2.9.96/oakvar/gui/webresult/nocache/css/
+-rw-r--r--   0 rick       (501) staff       (20)     1714 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 rick       (501) staff       (20)    22655 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/css/style.css
+-rw-r--r--   0 rick       (501) staff       (20)     2658 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/css/widget.css
+-rw-r--r--   0 rick       (501) staff       (20)    21597 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/index.html
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.275667 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/
+-rw-r--r--   0 rick       (501) staff       (20)    24858 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/filter.js
+-rw-r--r--   0 rick       (501) staff       (20)    13105 2023-12-09 16:39:48.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 rick       (501) staff       (20)    30870 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/main.js
+-rw-r--r--   0 rick       (501) staff       (20)   103450 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/setup.js
+-rw-r--r--   0 rick       (501) staff       (20)     4903 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 rick       (501) staff       (20)    35998 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 rick       (501) staff       (20)    28858 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/util.js
+-rw-r--r--   0 rick       (501) staff       (20)     1696 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/variables.js
+-rw-r--r--   0 rick       (501) staff       (20)    22262 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 rick       (501) staff       (20)     5440 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/nocache/variant.html
+-rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/question.png
+-rw-r--r--   0 rick       (501) staff       (20)    31615 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/webresult/webresult.py
+-rw-r--r--   0 rick       (501) staff       (20)      163 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webresult/webviewer.yml
+-rw-r--r--   0 rick       (501) staff       (20)     5907 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websocket_handlers.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.206910 oakvar-2.9.96/oakvar/gui/webstore/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.277468 oakvar-2.9.96/oakvar/gui/webstore/images/
+-rw-r--r--   0 rick       (501) staff       (20)      446 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      740 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/chat-dots.svg
+-rw-r--r--   0 rick       (501) staff       (20)      396 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      545 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/chat-left-text.svg
+-rw-r--r--   0 rick       (501) staff       (20)    22268 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/done.png
+-rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/email.png
+-rw-r--r--   0 rick       (501) staff       (20)     2226 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/empty.png
+-rw-r--r--   0 rick       (501) staff       (20)     1763 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/folder.png
+-rw-r--r--   0 rick       (501) staff       (20)    38197 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 rick       (501) staff       (20)     4766 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/hamburger.png
+-rw-r--r--   0 rick       (501) staff       (20)     1194 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/left_arrow.png
+-rw-r--r--   0 rick       (501) staff       (20)     3524 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/new.png
+-rw-r--r--   0 rick       (501) staff       (20)      474 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/no_logo_module.svg
+-rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/question.png
+-rw-r--r--   0 rick       (501) staff       (20)     1214 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/right_arrow.png
+-rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/webstore/images/x-lg.svg
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.207130 oakvar-2.9.96/oakvar/gui/websubmit/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.279605 oakvar-2.9.96/oakvar/gui/websubmit/images/
+-rw-r--r--   0 rick       (501) staff       (20)   372952 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/images/background.png
+-rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/images/logo.png
+-rw-r--r--   0 rick       (501) staff       (20)    22716 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/images/logo_only.png
+-rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/images/logo_transparent.png
+-rw-r--r--   0 rick       (501) staff       (20)    22247 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/images/logo_transparent_bw.png
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.279726 oakvar-2.9.96/oakvar/gui/websubmit/inputexamples/
+-rw-r--r--   0 rick       (501) staff       (20)     9036 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/inputexamples/exampleinput
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.281531 oakvar-2.9.96/oakvar/gui/websubmit/nocache/
+-rw-r--r--   0 rick       (501) staff       (20)      692 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/alerts.js
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/element_constructors.js
+-rw-r--r--   0 rick       (501) staff       (20)     6756 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/element_getters.js
+-rw-r--r--   0 rick       (501) staff       (20)    55822 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/index.html
+-rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/input.js
+-rw-r--r--   0 rick       (501) staff       (20)    14408 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/jobstable.js
+-rw-r--r--   0 rick       (501) staff       (20)     8242 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/login.html
+-rw-r--r--   0 rick       (501) staff       (20)     3796 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/multiuser.css
+-rw-r--r--   0 rick       (501) staff       (20)    16797 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/multiuser.js
+-rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/select_modules.js
+-rw-r--r--   0 rick       (501) staff       (20)      228 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/showhide.js
+-rw-r--r--   0 rick       (501) staff       (20)     6783 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/submit.js
+-rw-r--r--   0 rick       (501) staff       (20)      484 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/util.js
+-rw-r--r--   0 rick       (501) staff       (20)    11319 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/websubmit.css
+-rw-r--r--   0 rick       (501) staff       (20)    39200 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/gui/websubmit/nocache/websubmit.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.281765 oakvar-2.9.96/oakvar/gui/www/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.282017 oakvar-2.9.96/oakvar/gui/www/assets/
+-rw-r--r--   0 rick       (501) staff       (20)    63287 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/www/assets/index.3526e7ae.css
+-rw-r--r--   0 rick       (501) staff       (20)   834933 2023-12-09 16:39:48.000000 oakvar-2.9.96/oakvar/gui/www/assets/index.5e1d7274.js
+-rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/gui/www/favicon.ico
+-rw-r--r--   0 rick       (501) staff       (20)     2074 2023-12-09 16:39:48.000000 oakvar-2.9.96/oakvar/gui/www/index.html
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.282796 oakvar-2.9.96/oakvar/lib/
+-rw-r--r--   0 rick       (501) staff       (20)     1946 2024-03-03 16:46:38.000000 oakvar-2.9.96/oakvar/lib/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.283756 oakvar-2.9.96/oakvar/lib/assets/
+-rw-r--r--   0 rick       (501) staff       (20)     9036 2024-04-10 11:35:01.000000 oakvar-2.9.96/oakvar/lib/assets/exampleinput
+-rw-r--r--   0 rick       (501) staff       (20)    16880 2024-02-08 01:06:28.000000 oakvar-2.9.96/oakvar/lib/assets/hg19.chromAlias.txt
+-rw-r--r--   0 rick       (501) staff       (20)    27240 2024-02-08 00:52:40.000000 oakvar-2.9.96/oakvar/lib/assets/hg38.chromAlias.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.283964 oakvar-2.9.96/oakvar/lib/assets/license/
+-rw-r--r--   0 rick       (501) staff       (20)     1707 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/license/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)     1330 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/license/liftover.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.207858 oakvar-2.9.96/oakvar/lib/assets/module_templates/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.284288 oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2109 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1195 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.284602 oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     4366 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1249 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.284908 oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     3078 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1120 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.285226 oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2563 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1335 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.285537 oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2033 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1327 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.285858 oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     3574 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1246 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.yml
+-rw-r--r--   0 rick       (501) staff       (20)      135 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/oakvar.yml
+-rw-r--r--   0 rick       (501) staff       (20)    10314 2024-04-10 12:11:07.000000 oakvar-2.9.96/oakvar/lib/assets/oakvar_example.vcf
+-rw-r--r--   0 rick       (501) staff       (20)     3060 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/assets/output_columns.yml
+-rw-r--r--   0 rick       (501) staff       (20)      768 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/assets/system.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.287905 oakvar-2.9.96/oakvar/lib/base/
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/base/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)    22714 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/aggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)    36762 2024-03-03 18:25:36.000000 oakvar-2.9.96/oakvar/lib/base/annotator.py
+-rw-r--r--   0 rick       (501) staff       (20)     2588 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/base/app.py
+-rw-r--r--   0 rick       (501) staff       (20)     4546 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/base/commonmodule.py
+-rw-r--r--   0 rick       (501) staff       (20)     5216 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/converter.py
+-rw-r--r--   0 rick       (501) staff       (20)    13627 2024-03-03 16:41:12.000000 oakvar-2.9.96/oakvar/lib/base/mapper.py
+-rw-r--r--   0 rick       (501) staff       (20)    43499 2024-02-19 19:29:51.000000 oakvar-2.9.96/oakvar/lib/base/master_converter.py
+-rw-r--r--   0 rick       (501) staff       (20)     4982 2024-03-03 18:25:36.000000 oakvar-2.9.96/oakvar/lib/base/mp_runners.py
+-rw-r--r--   0 rick       (501) staff       (20)    27573 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/postaggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)     8852 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/preparer.py
+-rw-r--r--   0 rick       (501) staff       (20)    44997 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/report_filter.py
+-rw-r--r--   0 rick       (501) staff       (20)    44831 2024-03-07 14:37:13.000000 oakvar-2.9.96/oakvar/lib/base/reporter.py
+-rw-r--r--   0 rick       (501) staff       (20)    84125 2024-03-07 14:36:39.000000 oakvar-2.9.96/oakvar/lib/base/runner.py
+-rw-r--r--   0 rick       (501) staff       (20)    17018 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/base/vcf2vcf.py
+-rw-r--r--   0 rick       (501) staff       (20)     4452 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)     9623 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.288462 oakvar-2.9.96/oakvar/lib/module/
+-rw-r--r--   0 rick       (501) staff       (20)    32253 2024-04-11 21:57:44.000000 oakvar-2.9.96/oakvar/lib/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     5975 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/module/cache.py
+-rw-r--r--   0 rick       (501) staff       (20)     5355 2023-12-05 15:09:56.000000 oakvar-2.9.96/oakvar/lib/module/data_cache.py
+-rw-r--r--   0 rick       (501) staff       (20)    33003 2024-04-13 11:24:40.000000 oakvar-2.9.96/oakvar/lib/module/local.py
+-rw-r--r--   0 rick       (501) staff       (20)    13243 2023-12-09 16:39:48.000000 oakvar-2.9.96/oakvar/lib/module/remote.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.288785 oakvar-2.9.96/oakvar/lib/store/
+-rw-r--r--   0 rick       (501) staff       (20)     6162 2023-12-05 15:09:57.000000 oakvar-2.9.96/oakvar/lib/store/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     2483 2023-12-05 15:09:57.000000 oakvar-2.9.96/oakvar/lib/store/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)    28024 2024-04-11 14:27:45.000000 oakvar-2.9.96/oakvar/lib/store/db.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.288905 oakvar-2.9.96/oakvar/lib/store/ov/
+-rw-r--r--   0 rick       (501) staff       (20)     9948 2024-04-11 04:57:50.000000 oakvar-2.9.96/oakvar/lib/store/ov/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.289032 oakvar-2.9.96/oakvar/lib/store/ov/account/
+-rw-r--r--   0 rick       (501) staff       (20)    23471 2024-04-13 11:26:16.000000 oakvar-2.9.96/oakvar/lib/store/ov/account/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.289724 oakvar-2.9.96/oakvar/lib/system/
+-rw-r--r--   0 rick       (501) staff       (20)    43831 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/system/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     3126 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/system/consts.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.291482 oakvar-2.9.96/oakvar/lib/util/
+-rw-r--r--   0 rick       (501) staff       (20)     2214 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/util/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     7408 2024-04-10 23:40:21.000000 oakvar-2.9.96/oakvar/lib/util/admin_util.py
+-rw-r--r--   0 rick       (501) staff       (20)     2576 2023-12-05 15:09:57.000000 oakvar-2.9.96/oakvar/lib/util/asyn.py
+-rw-r--r--   0 rick       (501) staff       (20)     8251 2024-02-23 15:11:11.000000 oakvar-2.9.96/oakvar/lib/util/db.py
+-rw-r--r--   0 rick       (501) staff       (20)     6939 2023-12-09 16:39:48.000000 oakvar-2.9.96/oakvar/lib/util/download.py
+-rw-r--r--   0 rick       (501) staff       (20)    20964 2024-01-10 14:33:05.000000 oakvar-2.9.96/oakvar/lib/util/download_library.py
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:57.000000 oakvar-2.9.96/oakvar/lib/util/image.py
+-rw-r--r--   0 rick       (501) staff       (20)    23939 2024-02-08 00:22:22.000000 oakvar-2.9.96/oakvar/lib/util/inout.py
+-rw-r--r--   0 rick       (501) staff       (20)    10675 2024-04-13 11:27:05.000000 oakvar-2.9.96/oakvar/lib/util/run.py
+-rw-r--r--   0 rick       (501) staff       (20)    14974 2024-03-22 00:57:28.000000 oakvar-2.9.96/oakvar/lib/util/seq.py
+-rw-r--r--   0 rick       (501) staff       (20)    22127 2024-04-13 11:19:38.000000 oakvar-2.9.96/oakvar/lib/util/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-13 13:14:04.223572 oakvar-2.9.96/oakvar.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-13 13:14:03.000000 oakvar-2.9.96/oakvar.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)    18985 2024-04-13 13:14:04.000000 oakvar-2.9.96/oakvar.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2024-04-13 13:14:03.000000 oakvar-2.9.96/oakvar.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)       44 2024-04-13 13:14:04.000000 oakvar-2.9.96/oakvar.egg-info/entry_points.txt
+-rw-r--r--   0 rick       (501) staff       (20)      291 2024-04-13 13:14:04.000000 oakvar-2.9.96/oakvar.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       14 2024-04-13 13:14:04.000000 oakvar-2.9.96/oakvar.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)      625 2023-12-05 15:09:57.000000 oakvar-2.9.96/pyproject.toml
+-rw-r--r--   0 rick       (501) staff       (20)       38 2024-04-13 13:14:04.291935 oakvar-2.9.96/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)     2443 2024-04-13 13:11:54.000000 oakvar-2.9.96/setup.py
```

### Comparing `oakvar-2.9.95/LICENSE` & `oakvar-2.9.96/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/PKG-INFO` & `oakvar-2.9.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.95
+Version: 2.9.96
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 License: UNKNOWN
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
```

### Comparing `oakvar-2.9.95/README.rst` & `oakvar-2.9.96/README.rst`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/__init__.py` & `oakvar-2.9.96/oakvar/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/__main__.py` & `oakvar-2.9.96/oakvar/__main__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/__init__.py` & `oakvar-2.9.96/oakvar/api/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/config.py` & `oakvar-2.9.96/oakvar/api/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/module/__init__.py` & `oakvar-2.9.96/oakvar/api/module/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,15 @@
 
     Returns:
         `True` if update was successful. `False` if not.
     """
     from ...lib.module.local import search_local
     from ...lib.module import get_updatable
     from ...lib.store.db import try_fetch_ov_store_cache
+    from ...lib.util.util import is_in_jupyter_notebook
 
     if not no_fetch:
         try_fetch_ov_store_cache(
             outer=outer,
         )
     requested_modules = search_local(*module_name_patterns)
     to_update = get_updatable(module_names=requested_modules)
@@ -417,15 +418,19 @@
     if not yes:
         if outer:
             outer.write("Following modules will be updated.")
             for mn in to_update:
                 local_version = to_update[mn][0]
                 remote_version = to_update[mn][1]
                 outer.write(f"- {mn}: {local_version} => {remote_version}")
-            yn = input("Proceed? (y/N) > ")
+            if is_in_jupyter_notebook():
+                print("Interactive mode not supported in Jupyter notebook. Please provide -y as arguments.")
+                return False
+            else:
+                yn = input("Proceed? (y/N) > ")
             if not yn or yn.lower() not in ["y", "yes"]:
                 return True
     ret = install(
         module_names=list(to_update.keys()),
         modules_dir=modules_dir,
         force_data=force_data,
         yes=True,
@@ -453,14 +458,15 @@
 
     Returns:
         `True` if successful. `False` if not.
     """
     from ...lib.module.local import search_local
     from ...lib.module import uninstall_module
     from ...lib.exceptions import ArgumentError
+    from ...lib.util.util import is_in_jupyter_notebook
 
     if not module_names:
         e = ArgumentError("No modules to uninstall.")
         e.traceback = False
         raise e
     module_names = search_local(*module_names)
     if len(module_names) == 0:
@@ -468,15 +474,19 @@
             outer.write("No module to uninstall")
         return True
     if outer:
         outer.write("Uninstalling:")
         for mn in module_names:
             outer.write(f"- {mn}")
     if not yes:
-        yn = input("Proceed? (y/N) > ")
+        if is_in_jupyter_notebook():
+            print("Interactive mode not supported in Jupyter notebook. Please provide -y as arguments.")
+            return False
+        else:
+            yn = input("Proceed? (y/N) > ")
         if not yn or yn.lower() != "y":
             return True
     for module_name in module_names:
         uninstall_module(module_name, outer=outer)
     return True
```

### Comparing `oakvar-2.9.95/oakvar/api/module/install_defs.py` & `oakvar-2.9.96/oakvar/api/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/module/ls_logic.py` & `oakvar-2.9.96/oakvar/api/module/ls_logic.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/new.py` & `oakvar-2.9.96/oakvar/api/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/store/__init__.py` & `oakvar-2.9.96/oakvar/api/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/store/account/__init__.py` & `oakvar-2.9.96/oakvar/api/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/system.py` & `oakvar-2.9.96/oakvar/api/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/test.py` & `oakvar-2.9.96/oakvar/api/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/api/util.py` & `oakvar-2.9.96/oakvar/api/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/__init__.py` & `oakvar-2.9.96/oakvar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/config.py` & `oakvar-2.9.96/oakvar/cli/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/gui.py` & `oakvar-2.9.96/oakvar/cli/gui.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/issue.py` & `oakvar-2.9.96/oakvar/cli/issue.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/license.py` & `oakvar-2.9.96/oakvar/cli/license.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/module/__init__.py` & `oakvar-2.9.96/oakvar/cli/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/module/info_fn.py` & `oakvar-2.9.96/oakvar/cli/module/info_fn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/module/install_defs.py` & `oakvar-2.9.96/oakvar/cli/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/module/ls.py` & `oakvar-2.9.96/oakvar/cli/module/ls.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/new.py` & `oakvar-2.9.96/oakvar/cli/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/report.py` & `oakvar-2.9.96/oakvar/cli/report.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/run.py` & `oakvar-2.9.96/oakvar/cli/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/store/__init__.py` & `oakvar-2.9.96/oakvar/cli/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/store/account/__init__.py` & `oakvar-2.9.96/oakvar/cli/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/system.py` & `oakvar-2.9.96/oakvar/cli/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/test.py` & `oakvar-2.9.96/oakvar/cli/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/update.py` & `oakvar-2.9.96/oakvar/cli/update.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/util.py` & `oakvar-2.9.96/oakvar/cli/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/cli/version.py` & `oakvar-2.9.96/oakvar/cli/version.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/consts.py` & `oakvar-2.9.96/oakvar/gui/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/job_handlers.py` & `oakvar-2.9.96/oakvar/gui/job_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/multiuser.py` & `oakvar-2.9.96/oakvar/gui/multiuser.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/server.py` & `oakvar-2.9.96/oakvar/gui/server.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/serveradmindb.py` & `oakvar-2.9.96/oakvar/gui/serveradmindb.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/store_handlers.py` & `oakvar-2.9.96/oakvar/gui/store_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/system_handlers.py` & `oakvar-2.9.96/oakvar/gui/system_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/system_message_db.py` & `oakvar-2.9.96/oakvar/gui/system_message_db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/system_worker.py` & `oakvar-2.9.96/oakvar/gui/system_worker.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/userjob.py` & `oakvar-2.9.96/oakvar/gui/userjob.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/util.py` & `oakvar-2.9.96/oakvar/gui/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/web_submit.py` & `oakvar-2.9.96/oakvar/gui/web_submit.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/__init__.py` & `oakvar-2.9.96/oakvar/gui/webresult/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/css/pqselect.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/email.png` & `oakvar-2.9.96/oakvar/gui/webresult/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/favicon.ico` & `oakvar-2.9.96/oakvar/gui/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/Inter_Web/inter.css` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/Inter_Web/inter.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-light-webfont.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `oakvar-2.9.96/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/arrows-move.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/camera.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/close.png` & `oakvar-2.9.96/oakvar/gui/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/close.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/download-material-black.png` & `oakvar-2.9.96/oakvar/gui/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/download.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/pin.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/plus-circle-dotted.svg` & `oakvar-2.9.96/oakvar/gui/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/sorry.png` & `oakvar-2.9.96/oakvar/gui/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/images/spinner.gif` & `oakvar-2.9.96/oakvar/gui/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/Chart.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/axios.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/axios.min.js.map` & `oakvar-2.9.96/oakvar/gui/webresult/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/dom-to-image.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/download.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/draggabilly.pkgd.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/draggabilly.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/graphics.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-3.2.1.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery.tools.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/jquery.url.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/masonry.pkgd.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/packery.pkgd.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/pqselect.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/raphael-min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/js/tailwind.min.js` & `oakvar-2.9.96/oakvar/gui/webresult/js/tailwind.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/jsonreporter.py` & `oakvar-2.9.96/oakvar/gui/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/css/singlevariantpage.css` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/css/style.css` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/css/widget.css` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/index.html` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/filter.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/infomgr.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/main.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/setup.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/showvariant.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/singlevariantpage.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/util.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/variables.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/js/widgethelper.js` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/nocache/variant.html` & `oakvar-2.9.96/oakvar/gui/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/question.png` & `oakvar-2.9.96/oakvar/gui/webresult/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webresult/webresult.py` & `oakvar-2.9.96/oakvar/gui/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websocket_handlers.py` & `oakvar-2.9.96/oakvar/gui/websocket_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/chat-dots.svg` & `oakvar-2.9.96/oakvar/gui/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/chat-left-text.svg` & `oakvar-2.9.96/oakvar/gui/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/done.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/email.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/empty.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/folder.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/genericmodulelogo.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/hamburger.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/left_arrow.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/new.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/question.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/webstore/images/right_arrow.png` & `oakvar-2.9.96/oakvar/gui/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/images/background.png` & `oakvar-2.9.96/oakvar/gui/websubmit/images/background.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/images/logo.png` & `oakvar-2.9.96/oakvar/gui/websubmit/images/logo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/images/logo_only.png` & `oakvar-2.9.96/oakvar/gui/websubmit/images/logo_only.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/images/logo_transparent.png` & `oakvar-2.9.96/oakvar/gui/websubmit/images/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/images/logo_transparent_bw.png` & `oakvar-2.9.96/oakvar/gui/websubmit/images/logo_transparent_bw.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/inputexamples/exampleinput` & `oakvar-2.9.96/oakvar/gui/websubmit/inputexamples/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/alerts.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/alerts.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/element_getters.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/element_getters.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/index.html` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/input.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/input.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/jobstable.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/jobstable.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/login.html` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/login.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/multiuser.css` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/multiuser.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/multiuser.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/multiuser.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/select_modules.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/select_modules.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/submit.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/submit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/websubmit.css` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/websubmit/nocache/websubmit.js` & `oakvar-2.9.96/oakvar/gui/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/www/assets/index.3526e7ae.css` & `oakvar-2.9.96/oakvar/gui/www/assets/index.3526e7ae.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/www/assets/index.5e1d7274.js` & `oakvar-2.9.96/oakvar/gui/www/assets/index.5e1d7274.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/www/favicon.ico` & `oakvar-2.9.96/oakvar/gui/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/gui/www/index.html` & `oakvar-2.9.96/oakvar/gui/www/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/__init__.py` & `oakvar-2.9.96/oakvar/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/exampleinput` & `oakvar-2.9.96/oakvar/lib/assets/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/hg19.chromAlias.txt` & `oakvar-2.9.96/oakvar/lib/assets/hg19.chromAlias.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/hg38.chromAlias.txt` & `oakvar-2.9.96/oakvar/lib/assets/hg38.chromAlias.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/license/LICENSE` & `oakvar-2.9.96/oakvar/lib/assets/license/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/license/liftover.txt` & `oakvar-2.9.96/oakvar/lib/assets/license/liftover.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/annotator/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/annotator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/converter/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/converter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/mapper/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/mapper/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/postaggregator/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/postaggregator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/preparer/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/preparer/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.md` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.py` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/module_templates/reporter/template.yml` & `oakvar-2.9.96/oakvar/lib/assets/module_templates/reporter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/oakvar_example.vcf` & `oakvar-2.9.96/oakvar/lib/assets/oakvar_example.vcf`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/output_columns.yml` & `oakvar-2.9.96/oakvar/lib/assets/output_columns.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/assets/system.yml` & `oakvar-2.9.96/oakvar/lib/assets/system.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/__init__.py` & `oakvar-2.9.96/oakvar/lib/base/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/aggregator.py` & `oakvar-2.9.96/oakvar/lib/base/aggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/annotator.py` & `oakvar-2.9.96/oakvar/lib/base/annotator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/app.py` & `oakvar-2.9.96/oakvar/lib/base/app.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/commonmodule.py` & `oakvar-2.9.96/oakvar/lib/base/commonmodule.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/converter.py` & `oakvar-2.9.96/oakvar/lib/base/converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/mapper.py` & `oakvar-2.9.96/oakvar/lib/base/mapper.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/master_converter.py` & `oakvar-2.9.96/oakvar/lib/base/master_converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/mp_runners.py` & `oakvar-2.9.96/oakvar/lib/base/mp_runners.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/postaggregator.py` & `oakvar-2.9.96/oakvar/lib/base/postaggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/preparer.py` & `oakvar-2.9.96/oakvar/lib/base/preparer.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/report_filter.py` & `oakvar-2.9.96/oakvar/lib/base/report_filter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/reporter.py` & `oakvar-2.9.96/oakvar/lib/base/reporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/runner.py` & `oakvar-2.9.96/oakvar/lib/base/runner.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/base/vcf2vcf.py` & `oakvar-2.9.96/oakvar/lib/base/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/consts.py` & `oakvar-2.9.96/oakvar/lib/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/exceptions.py` & `oakvar-2.9.96/oakvar/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/module/__init__.py` & `oakvar-2.9.96/oakvar/lib/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/module/cache.py` & `oakvar-2.9.96/oakvar/lib/module/cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/module/data_cache.py` & `oakvar-2.9.96/oakvar/lib/module/data_cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/module/local.py` & `oakvar-2.9.96/oakvar/lib/module/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -793,14 +793,15 @@
     from os import getcwd
     from shutil import copytree
     from shutil import ignore_patterns
     from oyaml import dump
     from ..exceptions import IncompleteModuleError
     from ..exceptions import SystemMissingException
     from ..system import get_modules_dir
+    from ..util.util import is_in_jupyter_notebook
 
     cls = instance.__class__
     if not cls:
         raise Exception("Only an OakVar class can be saved into module files.")
     modules_dir = get_modules_dir()
     if not modules_dir:
         raise SystemMissingException(
@@ -820,46 +821,61 @@
     module_title: Optional[str] = getattr(instance, "title", module_conf.get("title"))
     module_level: Optional[str] = getattr(instance, "level", module_conf.get("level"))
     output_columns: Optional[List[Dict[str, Any]]] = getattr(
         instance, "output_columns", module_conf.get("output_columns", [])
     )
     if not module_name:
         if interactive:
-            module_name = input("Module name:")
+            if is_in_jupyter_notebook():
+                print("Interactive mode is not available in Jupyter notebook. Please provide module name in the instance argument.")
+            else:
+                module_name = input("Module name:")
     if not module_name:
         raise IncompleteModuleError(
             msg="name property does not exist in the module. Consider "
             + "giving 'name' argument at initializing the module."
         )
     if not module_version:
         if interactive:
-            module_version = input("Module version:")
+            if is_in_jupyter_notebook():
+                print("Interactive mode is not available in Jupyter notebook. Please provide module version in the instance argument.")
+            else:
+                module_version = input("Module version:")
     if not module_version:
         raise IncompleteModuleError(
             msg="code_version property does not exist in the module. Consider "
             + "giving 'code_version' argument at initializing the module."
         )
     if not module_title:
         if interactive:
-            module_title = input("Module title:")
+            if is_in_jupyter_notebook():
+                print("Interactive mode is not available in Jupyter notebook. Please provide module title in the instance argument.")
+            else:
+                module_title = input("Module title:")
     if not module_title:
         raise IncompleteModuleError(
             msg="title property does not exist in the module. Consider giving "
             + "'title' argument at initializing the module."
         )
     if not module_type:
-        module_type = input("Module type:")
+        if is_in_jupyter_notebook():
+            print("Interactive mode is not available in Jupyter notebook. Please provide module type in the instance argument.")
+        else:
+            module_type = input("Module type:")
     if not module_type:
         raise IncompleteModuleError(
             msg="module_type property does not exist in the module."
         )
     module_dir = modules_dir / (module_type + "s") / module_name
     if module_type in ["annotator", "postaggregator"]:
         if not module_level:
-            module_level = input("Module level:")
+            if is_in_jupyter_notebook():
+                print("Interactive mode is not available in Jupyter notebook. Please provide module level in the instance argument.")
+            else:
+                module_level = input("Module level:")
         if not module_level:
             raise IncompleteModuleError(
                 msg="title property does not exist in the module. Consider giving "
                 + "'level' argument at initializing the module."
             )
         if not output_columns:
             raise IncompleteModuleError(
```

### Comparing `oakvar-2.9.95/oakvar/lib/module/remote.py` & `oakvar-2.9.96/oakvar/lib/module/remote.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/store/__init__.py` & `oakvar-2.9.96/oakvar/lib/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/store/consts.py` & `oakvar-2.9.96/oakvar/lib/store/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/store/db.py` & `oakvar-2.9.96/oakvar/lib/store/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/store/ov/__init__.py` & `oakvar-2.9.96/oakvar/lib/store/ov/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/store/ov/account/__init__.py` & `oakvar-2.9.96/oakvar/lib/store/ov/account/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,19 +59,24 @@
 
 
 def get_email_pw_interactively(
     email: Optional[str] = None, pw: Optional[str] = None, pwconfirm=False, outer=None
 ) -> Tuple:
     from ....util.util import email_is_valid
     from ....util.util import pw_is_valid
+    from ....util.util import is_in_jupyter_notebook
     from getpass import getpass
 
     if not email:
         while True:
-            email = input("Email: ")
+            if is_in_jupyter_notebook():
+                print("Interactive mode not supported in Jupyter notebook. Please provide email and password as arguments.")
+                return email, pw
+            else:
+                email = input("Email: ")
             if email_is_valid(email):
                 break
             if outer:
                 outer.error("Email is not vaild.")
     if not pw:
         while True:
             pw = getpass("Password (alphabets, numbers, and !?&@-+): ")
@@ -94,18 +99,26 @@
     pwconfirm=True,
     interactive: bool = False,
     outer=None,
 ) -> dict:
     from requests import post
     from ....system import get_system_conf
     from ....store.consts import store_url_key
-    from ....store.ov.account import get_email_pw_interactively
+    from ....util.util import is_in_jupyter_notebook
 
     if (not email or not pw) and interactive:
-        email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=pwconfirm)
+        if is_in_jupyter_notebook():
+            return {
+                "status_code": 403,
+                "msg": "Interactive mode not supported in Jupyter notebook. Please provide email and password as arguments.",
+                "success": False,
+                "email": email,
+            }
+        else:
+            email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=pwconfirm)
     if not email:
         return {"msg": "no email", "success": False, "email": email}
     sys_conf = get_system_conf()
     store_url = sys_conf[store_url_key]
     create_account_url = store_url + "/account/create"
     params = {
         "email": email,
@@ -250,27 +263,36 @@
     pw: Optional[str] = None,
     interactive: bool = False,
     relogin: bool = False,
     outer=None,
 ) -> Dict[str, Any]:
     from requests import post
     from ...ov import get_store_url
+    from ....util.util import is_in_jupyter_notebook
 
     if not relogin and not email:
         ret, token_set_email = try_login_with_token(email=email)
         if ret is True:
             return {
                 "success": True,
                 "msg": f"Logged in as {token_set_email}",
                 "email": token_set_email,
             }
     if not email or not pw:
         email, pw = get_email_pw_from_user_conf(email=email, pw=pw)
     if (not email or not pw) and interactive:
-        email, pw = get_email_pw_interactively(email=email, pw=pw)
+        if is_in_jupyter_notebook():
+            return {
+                "status_code": 403,
+                "msg": "Interactive mode not supported in Jupyter notebook. Please provide email and password as arguments.",
+                "success": False,
+                "email": email,
+            }
+        else:
+            email, pw = get_email_pw_interactively(email=email, pw=pw)
     if not email:
         return {"success": False, "msg": "No email", "email": email}
     if not pw:
         return {"success": False, "msg": "No password", "email": email}
     login_url = get_store_url() + "/account/login"
     params = {"email": email, "pw": pw}
     try:
@@ -649,14 +671,15 @@
         }
 
 
 def total_login(
         email=None, pw=None, create_account: bool=False, install_mode: str = "", conf: Optional[Dict] = None, outer=None
 ) -> dict:
     from ....system import show_no_user_account_prelude
+    from ....util.util import is_in_jupyter_notebook
 
     if email is None or pw is None:
         ret, logged_email = login_with_token_set(email=email, outer=outer)
         if ret is True:
             return {"success": True, "email": logged_email}
     ret = login_with_email_pw(email=email, pw=pw, conf=conf, outer=outer)
     if ret.get("success"):
@@ -670,25 +693,46 @@
     if create_account:
         ret = create(email=email, pw=pw, outer=outer)
         if not ret.get("success"):
             if outer:
                 outer.write(ret)
         return ret
     yn = None
+    import sys; print("ipkernel" in sys.modules)
     while True:
-        yn = input("Do you already have an OakVar store account? (y/N): ")
+        if is_in_jupyter_notebook():
+            print("Interactive mode is not available in Jupyter notebook. Assuming that you have an OakVar account...")
+            break
+        else:
+            yn = input("Do you already have an OakVar store account? (y/N): ")
         if yn.lower() in ["y", "n", ""]:
             break
     if yn == "y":
-        email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=False, outer=outer)
+        if is_in_jupyter_notebook():
+            return {
+                "status_code": 403,
+                "msg": "Interactive mode not supported in Jupyter notebook. Please provide email and password as arguments.",
+                "success": False,
+                "email": email,
+            }
+        else:
+            email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=False, outer=outer)
         ret = login_with_email_pw(email=email, pw=pw, conf=conf)
         return ret
     else:
         show_no_user_account_prelude()
-        email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=True)
+        if is_in_jupyter_notebook():
+            return {
+                "status_code": 403,
+                "msg": "Interactive mode not supported in Jupyter notebook. Please provide email and password as arguments.",
+                "success": False,
+                "email": email,
+            }
+        else:
+            email, pw = get_email_pw_interactively(email=email, pw=pw, pwconfirm=True)
         ret = create(email=email, pw=pw, outer=outer)
         if not ret.get("success"):
             if outer:
                 outer.write(ret)
             return ret
         announce_on_email_verification_if_needed(email, outer=outer)
         ret = login(email=email, pw=pw, outer=outer)
```

### Comparing `oakvar-2.9.95/oakvar/lib/system/__init__.py` & `oakvar-2.9.96/oakvar/lib/system/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/system/consts.py` & `oakvar-2.9.96/oakvar/lib/system/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/__init__.py` & `oakvar-2.9.96/oakvar/lib/util/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/admin_util.py` & `oakvar-2.9.96/oakvar/lib/util/admin_util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/asyn.py` & `oakvar-2.9.96/oakvar/lib/util/asyn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/db.py` & `oakvar-2.9.96/oakvar/lib/util/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/download.py` & `oakvar-2.9.96/oakvar/lib/util/download.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/download_library.py` & `oakvar-2.9.96/oakvar/lib/util/download_library.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/image.py` & `oakvar-2.9.96/oakvar/lib/util/image.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/inout.py` & `oakvar-2.9.96/oakvar/lib/util/inout.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/run.py` & `oakvar-2.9.96/oakvar/lib/util/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,22 @@
 #                for h in v.handlers:
 #                    print("     +++", str(h.__class__)[8:-2])
 #                    for fld, val in h.__dict__.items():
 #                        print("%s%s=%s" % ("   -", fld, val))
 
 
 def get_y_or_n():
+    from .util import is_in_jupyter_notebook
+
     while True:
-        resp = input("Proceed? ([y]/n) > ")
+        if is_in_jupyter_notebook():
+            print("Interactive mode is not available in Jupyter notebook. Proceeding...")
+            return True
+        else:
+            resp = input("Proceed? ([y]/n) > ")
         if resp == "y" or resp == "":
             return True
         if resp == "n":
             return False
         else:
             continue
```

### Comparing `oakvar-2.9.95/oakvar/lib/util/seq.py` & `oakvar-2.9.96/oakvar/lib/util/seq.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/oakvar/lib/util/util.py` & `oakvar-2.9.96/oakvar/lib/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,7 +858,11 @@
         df = pl.read_database(
             sql, conn_url, partition_on=partition_on, partition_num=num_cores # type: ignore
         )
     else:
         df = pl.read_database(sql, conn_url) # type: ignore
     return df
 
+def is_in_jupyter_notebook() -> bool:
+    import os
+
+    return "JPY_SESSION_NAME" in os.environ
```

### Comparing `oakvar-2.9.95/oakvar.egg-info/PKG-INFO` & `oakvar-2.9.96/oakvar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.95
+Version: 2.9.96
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 License: UNKNOWN
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
```

### Comparing `oakvar-2.9.95/oakvar.egg-info/SOURCES.txt` & `oakvar-2.9.96/oakvar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/pyproject.toml` & `oakvar-2.9.96/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.95/setup.py` & `oakvar-2.9.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 long_description = (this_directory / "README.rst").read_text()
 oakvar_files = []
 cravat_files = []
 walk_and_add("oakvar", oakvar_files)
 walk_and_add("cravat", cravat_files)
 setup(
     name="oakvar",
-    version="2.9.95",
+    version="2.9.96",
     description="A genomic variant analysis platform",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rkimoakbioinformatics/oakvar",
     author="Ryangguk Kim",
     author_email="rkim@oakbioinformatics.com",
     license="",
```

