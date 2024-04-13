# Comparing `tmp/odoo_addons_oca_timesheet-16.0.20240301.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_timesheet-16.0.20240308.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1499 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1459 b- defN 24-Mar-02 07:07 odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-02 07:07 odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-02 07:07 odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      409 b- defN 24-Mar-02 07:07 odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/RECORD
-4 files, 1961 bytes uncompressed, 693 bytes compressed:  64.7%
+Zip file size: 1510 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1527 b- defN 24-Mar-09 07:21 odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 07:21 odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Mar-09 07:21 odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      409 b- defN 24-Mar-09 07:21 odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/RECORD
+4 files, 2029 bytes uncompressed, 704 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/METADATA
+Filename: odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/WHEEL
+Filename: odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/RECORD
+Filename: odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_timesheet-16.0.20240301.0.dist-info/METADATA` & `odoo_addons_oca_timesheet-16.0.20240308.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-timesheet
-Version: 16.0.20240301.0
+Version: 16.0.20240308.0
 Summary: Meta package for oca-timesheet Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -19,11 +19,12 @@
 Requires-Dist: odoo-addon-hr-timesheet-task-domain <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-task-required <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-task-stage <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-time-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-project-task-analytic-propagation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-project-task-stage-allow-timesheet <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-timesheet-line-exclude <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-sale-timesheet-rounded <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-timesheet-task-exclude <16.1dev,>=16.0dev
 
 UNKNOWN
```

