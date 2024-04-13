# Comparing `tmp/wwpdb.apps.editormodule-0.17.3.tar.gz` & `tmp/wwpdb.apps.editormodule-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.editormodule-0.17.3.tar", last modified: Tue Dec  5 23:13:54 2023, max compression
+gzip compressed data, was "wwpdb.apps.editormodule-0.18.tar", last modified: Sat Apr 13 10:13:23 2024, max compression
```

## Comparing `wwpdb.apps.editormodule-0.17.3.tar` & `wwpdb.apps.editormodule-0.18.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.137165 wwpdb.apps.editormodule-0.17.3/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2023-12-05 23:13:54.137165 wwpdb.apps.editormodule-0.17.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2023-12-05 23:13:54.137165 wwpdb.apps.editormodule-0.17.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.129165 wwpdb.apps.editormodule-0.17.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (127)      290 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7741 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)   144958 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (127)   213050 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     4873 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   163711 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8061 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1616 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)     6211 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    13947 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    17945 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (127)    15904 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (127)     3502 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (127)     2470 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    79034 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:04.000000 wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 23:13:54.133165 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2023-12-05 23:13:54.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1637 2023-12-05 23:13:54.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-05 23:13:54.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-05 23:13:43.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2023-12-05 23:13:54.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2023-12-05 23:13:54.000000 wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7864 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   144958 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (127)   216512 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4873 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   163711 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8061 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1616 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6211 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    13947 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    17945 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    15904 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     3502 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     2470 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    79034 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:13:11.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.editormodule-0.17.3/LICENSE` & `wwpdb.apps.editormodule-0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/PKG-INFO` & `wwpdb.apps.editormodule-0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17.3
+Version: 0.18
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17.3/setup.py` & `wwpdb.apps.editormodule-0.18/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,21 +163,25 @@
         "struct_ref_seq",
     ]
 
     # list of categories for which deletion of last remaining row will be allowed in the UI
     arrAllowLastRowDeleteCtgries = [
         "em_db_reference",
         "em_entity_assembly_molwt",
+        "em_entity_assembly_recombinant",
         "em_single_particle_entity",
         "em_vitrification",
+        "entity_src_gen",
         "entity_src_nat",
         "pdbx_database_related",
+        "pdbx_entity_src_syn",
         "pdbx_SG_project",
         "pdbx_nmr_refine",
         "refine_ls_shell",
+        "reflns_shell",
         "struct_conn",
         "struct_ncs_dom",
         "pdbx_initial_refinement_model",
         "pdbx_related_exp_data_set",
         "pdbx_serial_crystallography_measurement",
         "pdbx_serial_crystallography_sample_delivery",
         "pdbx_serial_crystallography_sample_delivery_injection",
```

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,29 @@
 # EM7 EM Fitting
 # EM8 EM Files
 
 loop_
 _pdbx_view_combine.exptl
 _pdbx_view_combine.viewName
 _pdbx_view_combine.sections
-X-RAY    AV1      XraySum,T1,T1contacts,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T4,T5,T6,XRAY1,XRAY2,XRAY_SX,T7
-NMR      NMR1     T1,T1contacts,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T4,T5,T6,NMR1,T7
+X-RAY    AV1      SumBase,XraySum,T1,T1contacts,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T4,T5,T6,XRAY1,XRAY2,XRAY_SX,T7
+NMR      NMR1     SumBase,NMRSum,T1,T1contacts,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T4,T5,T6,NMR1,T7
 EM       EM1      T1,T1contacts,EM1A,EM1C,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T3EM,T4,T5,T6,T7,EM2,EM3,EM4,EM5,EM6,EM7,EM8,EM9_REFI
 EMmap    EM2      EM1A,T1contacts,EM1B,EM1C,T2A,T2C,T2D,T3B,T3EM,T6EM,T6,EM2,EM3,EM4,EM5,EM6,EM7,EM8
 EM_NMR   EM1      T1,T1contacts,EM1A,EM1C,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T3EM,T4,T5,T6,NMR1,T7,EM2,EM3,EM4,EM5,EM6,EM7,EM8,EM9_REFI
 EC       EM1      T1,T1contacts,EM1A,EM1C,T2A,T2B,T2C,T2D,T2E,T3A,T3B,T3C,T3EM,T4,T5,T6,XRAY1,XRAY2,T7,EM2,EM3,EM4,EM5,EM6,EM7,EM8
 
 ###############################################################################################################
 data_XraySum
 loop_
 _pdbx_display_view_category_info.category_menu_display_name
 _pdbx_display_view_category_info.category_name
 _pdbx_display_view_category_info.category_group_display_name
 _pdbx_display_view_category_info.category_display_name
 _pdbx_display_view_category_info.category_cardinality
-Summary                   struct                              Summary                   Title                                  unit
-Summary                   citation                            Summary                   Citation                               multi
-Summary                   audit_author                        Summary                   'Entry Authors'                        multi
-Summary                   citation_author                     Summary                   'Citation Authors'                     multi
-Summary                   pdbx_database_related               Summary                   'Related Entries'                      multi
-Summary                   struct_keywords                     Summary                   'Struct Keywords'                      multi
-Summary                   entity                              Summary                   'Entity Description'                   multi
 Summary                   exptl_crystal_grow                  Summary                   exptl_crystal_grow                     multi
 Summary                   diffrn_source                       Summary                   diffrn_source                          multi
 Summary                   diffrn_detector                     Summary                   Detector                               multi
 Summary                   software                            Summary                   Software                               multi
 Summary                   reflns                              Summary                   'Overall Data0'                        unit
 Summary                   reflns_shell                        Summary                   'Highest Resolution Shell0'            multi
 Summary                   refine                              Summary                   'Overall Refinement Data0'             multi
@@ -158,14 +151,46 @@
 'Starting Model0'                      '_pdbx_initial_refinement_model.id'                           ID                                          N
 'Starting Model0'                      '_pdbx_initial_refinement_model.type'                         'Type'                                      N
 'Starting Model0'                      '_pdbx_initial_refinement_model.entity_id_list'               'Entity list'                               N
 'Starting Model0'                      '_pdbx_initial_refinement_model.source_name'                  'Source name'                               N
 'Starting Model0'                      '_pdbx_initial_refinement_model.accession_code'               'Accession code'                            N
 'Starting Model0'                      '_pdbx_initial_refinement_model.details'                       'Details'                                   N
 
+###############################################################################################################
+data_SumBase
+loop_
+_pdbx_display_view_category_info.category_menu_display_name
+_pdbx_display_view_category_info.category_name
+_pdbx_display_view_category_info.category_group_display_name
+_pdbx_display_view_category_info.category_display_name
+_pdbx_display_view_category_info.category_cardinality
+Summary                   struct                              Summary                   Title                                  unit
+Summary                   citation                            Summary                   Citation                               multi
+Summary                   audit_author                        Summary                   'Entry Authors'                        multi
+Summary                   citation_author                     Summary                   'Citation Authors'                     multi
+Summary                   pdbx_database_related               Summary                   'Related Entries'                      multi
+Summary                   struct_keywords                     Summary                   'Struct Keywords'                      multi
+Summary                   entity                              Summary                   'Entity Description'                   multi
+
+
+###############################################################################################################
+##### NMR Summary ####
+data_NMRSum
+loop_
+_pdbx_display_view_category_info.category_menu_display_name
+_pdbx_display_view_category_info.category_name
+_pdbx_display_view_category_info.category_group_display_name
+_pdbx_display_view_category_info.category_display_name
+_pdbx_display_view_category_info.category_cardinality
+Summary                   pdbx_nmr_ensemble                  Summary     pdbx_nmr_ensemble                    unit
+Summary                   pdbx_nmr_sample_details            Summary     pdbx_nmr_sample_details              multi
+Summary                   pdbx_nmr_exptl_sample              Summary     pdbx_nmr_exptl_sample                multi
+Summary                   pdbx_nmr_spectrometer              Summary     pdbx_nmr_spectrometer                multi
+Summary                   pdbx_nmr_software                  Summary     pdbx_nmr_software                    multi
+Summary                   pdbx_nmr_chem_shift_ref            Summary     pdbx_nmr_chem_shift_ref              multi
 
 
 ###############################################################################################################
 data_T1
 loop_
 _pdbx_display_view_category_info.category_menu_display_name
 _pdbx_display_view_category_info.category_name
@@ -895,35 +920,54 @@
 pdbx_refine_tls_group                 '_pdbx_refine_tls_group.beg_auth_asym_id'                     beg_auth_asym_id                            N
 pdbx_refine_tls_group                 '_pdbx_refine_tls_group.beg_auth_seq_id'                      beg_auth_seq_id                             N
 pdbx_refine_tls_group                 '_pdbx_refine_tls_group.end_auth_asym_id'                     end_auth_asym_id                            N
 pdbx_refine_tls_group                 '_pdbx_refine_tls_group.end_auth_seq_id'                      end_auth_seq_id                             N
 pdbx_refine_tls_group                 '_pdbx_refine_tls_group.selection_details'                    selection_details                           N
 struct_ncs_ens                        '_struct_ncs_ens.id'                                          id                                          N
 struct_ncs_ens                        '_struct_ncs_ens.details'                                     details                                     N
+struct_ncs_dom                        '_struct_ncs_dom.id'                                          id                                          N
 struct_ncs_dom                        '_struct_ncs_dom.details'                                     details                                     N
 struct_ncs_dom                        '_struct_ncs_dom.pdbx_ens_id'                                 pdbx_ens_id                                 N
+
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.dom_id'                                  dom_id                                      N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_auth_asym_id'                        beg_auth_asym_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_auth_seq_id'                         beg_auth_seq_id                             N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_alt_id'                        beg_label_alt_id                            N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_asym_id'                       beg_label_asym_id                           N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_comp_id'                       beg_label_comp_id                           N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_seq_id'                        beg_label_seq_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_auth_asym_id'                        end_auth_asym_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_auth_seq_id'                         end_auth_seq_id                             N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_alt_id'                        end_label_alt_id                            N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_asym_id'                       end_label_asym_id                           N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_comp_id'                       end_label_comp_id                           N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_seq_id'                        end_label_seq_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_component_id'                       pdbx_component_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_refine_code'                        pdbx_refine_code                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_ens_id'                             pdbx_ens_id                                 N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.selection_details'                       selection_details                           N
+
+
+
 refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_auth_asym_id'                      pdbx_auth_asym_id                           N
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_refine_id'                         pdbx_refine_id                              Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.dom_id'                                 dom_id                                      Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_ens_id'                            pdbx_ens_id                                 Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_ordinal'                           pdbx_ordinal                                Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.ncs_model_details'                      ncs_model_details                           Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.rms_dev_position'                       rms_dev_position                            Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.weight_position'                        weight_position                             Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.rms_dev_B_iso'                          rms_dev_B_iso                               Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.weight_B_iso'                           weight_B_iso                                Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_number'                            pdbx_number                                 Y
-refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_type'                              pdbx_type                                   Y
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_refine_id'                         pdbx_refine_id                              N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.dom_id'                                 dom_id                                      N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_ens_id'                            pdbx_ens_id                                 N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_ordinal'                           pdbx_ordinal                                N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.ncs_model_details'                      ncs_model_details                           N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.rms_dev_position'                       rms_dev_position                            N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.weight_position'                        weight_position                             N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.rms_dev_B_iso'                          rms_dev_B_iso                               N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.weight_B_iso'                           weight_B_iso                                N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_number'                            pdbx_number                                 N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_type'                              pdbx_type                                   N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_rms'                               pdbx_rms                                    N
+refine_ls_restr_ncs                   '_refine_ls_restr_ncs.pdbx_weight'                            pdbx_weight                                 N
+
+
 
 refine_ls_restr                       '_refine_ls_restr.pdbx_refine_id'                             pdbx_refine_id                              N
 refine_ls_restr                       '_refine_ls_restr.type'                                       type                                        N
 refine_ls_restr                       '_refine_ls_restr.dev_ideal'                                  dev_ideal                                   N
 refine_ls_restr                       '_refine_ls_restr.dev_ideal_target'                           dev_ideal_target                            N
 refine_ls_restr                       '_refine_ls_restr.number'                                     number                                      N
 refine_ls_restr                       '_refine_ls_restr.pdbx_restraint_function'                    pdbx_restraint_function                     N
@@ -1526,15 +1570,15 @@
 em_specimen                        '_em_specimen.details'                                        details                                          N
 em_specimen                        '_em_specimen.embedding_applied'                              embedding_applied                                N
 em_specimen                        '_em_specimen.shadowing_applied'                              shadowing_applied                                N
 em_specimen                        '_em_specimen.staining_applied'                               staining_applied                                 N
 em_specimen                        '_em_specimen.vitrification_applied'                          vitrification_applied                            N
 em_buffer                          '_em_buffer.id'                                               id                                               N
 em_buffer                          '_em_buffer.specimen_id'                                      specimen_id                                      N
-em_buffer                          '_em_buffer.pH'                                               ph                                               N
+em_buffer                          '_em_buffer.pH'                                               pH                                               N
 em_buffer                          '_em_buffer.details'                                          details                                          N
 em_buffer_component                '_em_buffer_component.id'                                     id                                               N
 em_buffer_component                '_em_buffer_component.buffer_id'                              buffer_id                                        N
 em_buffer_component                '_em_buffer_component.name'                                   name                                             N
 em_buffer_component                '_em_buffer_component.concentration'                          concentration                                    N
 em_buffer_component                '_em_buffer_component.concentration_units'                    concentration_units                              N
 em_buffer_component                '_em_buffer_component.formula'                                formula                                          N
@@ -1711,15 +1755,15 @@
 em_image_processing                '_em_image_processing.details'                                details                                          N
 em_3d_reconstruction               '_em_3d_reconstruction.id'                                    id                                               N
 em_3d_reconstruction               '_em_3d_reconstruction.image_processing_id'                   image_processing_id                              N
 em_3d_reconstruction               '_em_3d_reconstruction.algorithm'                             algorithm                                        N
 em_3d_reconstruction               '_em_3d_reconstruction.refinement_type'                             refinement_type                                  N
 em_3d_reconstruction               '_em_3d_reconstruction.details'                               details                                          N
 em_3d_reconstruction               '_em_3d_reconstruction.num_class_averages'                    num_classes_used                                 N
-em_3d_reconstruction               '_em_3d_reconstruction.num_particles'                         num_images_used                                  N
+em_3d_reconstruction               '_em_3d_reconstruction.num_particles'                         num_particles                                    N
 # em_3d_reconstruction               '_em_3d_reconstruction.num_subtomograms'                      num_subtomograms_used                            N
 em_3d_reconstruction               '_em_3d_reconstruction.resolution'                            resolution                                       N
 em_3d_reconstruction               '_em_3d_reconstruction.resolution_method'                     resolution_method                                N
 em_software                        '_em_software.id'                                             id                                               N
 em_software                        '_em_software.category'                                       category                                         N
 em_software                        '_em_software.name'                                           name                                             N
 em_software                        '_em_software.version'                                        version                                          N
```

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 <script type="text/javascript" src="/editormodule/js/jquery/ui-src/jquery-ui-1.10.3.custom.min.js" defer></script>
 <script type="text/javascript" src="/js/jquery/plugins/jquery.form.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/category.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/jquery.dataTables-1.10.5.wwpdb-editormod.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/jquery.jeditable-1.7.1.wwpdb.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/dataTables.colReorder.min.js" defer></script>
-<script type="text/javascript" src="/editormodule/js/editor-fxn-defs.min.js?v=20180703" defer></script>
+<script type="text/javascript" src="/editormodule/js/editor-fxn-defs.min.js?v=20240330" defer></script>
 <script type="text/javascript" src="/editormodule/js/custom-jeditable-input-types.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/json2.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/Transpose-1.0.0.min.js" defer></script>
 
 <script type="text/javascript" src="/editormodule/js/editor-main.min.js?v=20180703"></script>
 </head>
 <body class="oneColLiqCtrHdr">
```

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 <script type="text/javascript" src="/editormodule/js/jquery/ui-src/jquery-ui-1.10.3.custom.min.js" defer></script>
 <script type="text/javascript" src="/js/jquery/plugins/jquery.form.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/category.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/jquery.dataTables-1.10.5.wwpdb-editormod.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/jquery.jeditable-1.7.1.wwpdb.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/dataTables.colReorder.min.js" defer></script>
-<script type="text/javascript" src="/editormodule/js/editor-fxn-defs.min.js?v=20180703" defer></script>
+<script type="text/javascript" src="/editormodule/js/editor-fxn-defs.min.js?v=20240330" defer></script>
 <script type="text/javascript" src="/editormodule/js/custom-jeditable-input-types.min.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/json2.js" defer></script>
 <script type="text/javascript" src="/editormodule/js/jquery/plugins-src/Transpose-1.0.0.min.js" defer></script>
 
 <script type="text/javascript" src="/editormodule/js/editor-main.min.js?v=20180703"></script>
 </head>
 <body class="oneColLiqCtrHdr">
```

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17.3
+Version: 0.18
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17.3/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

