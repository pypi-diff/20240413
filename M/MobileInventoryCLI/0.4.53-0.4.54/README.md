# Comparing `tmp/MobileInventoryCLI-0.4.53.tar.gz` & `tmp/MobileInventoryCLI-0.4.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.53.tar", last modified: Sat Apr 13 16:35:48 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.54.tar", last modified: Sat Apr 13 18:49:28 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.53.tar` & `MobileInventoryCLI-0.4.54.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.422903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.422903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   104240 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.426236 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    16709 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    60445 2024-04-13 16:35:24.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28296 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-13 16:35:43.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1105 2024-04-13 16:31:57.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.429570 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-12 23:19:11.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4946 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-13 16:35:48.432903 MobileInventoryCLI-0.4.53/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-13 16:35:48.000000 MobileInventoryCLI-0.4.53/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.336579 MobileInventoryCLI-0.4.54/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.326579 MobileInventoryCLI-0.4.54/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.326579 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-13 18:34:53.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   104240 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.329913 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    16709 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    60445 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-13 18:10:39.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-13 18:48:18.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1230 2024-04-13 18:49:24.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-13 16:35:56.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-13 18:49:28.333246 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5020 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-13 18:49:28.336579 MobileInventoryCLI-0.4.54/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-13 18:49:28.336579 MobileInventoryCLI-0.4.54/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-13 18:49:28.000000 MobileInventoryCLI-0.4.54/setup.py
```

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 import upcean
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExtractPkg.ExtractPkg2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Lookup.Lookup import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DayLog.DayLogger import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.db import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.ResetTools import *
 
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ConvertCode.ConvertCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.setCode.setCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Locator.Locator import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ListMode2.ListMode2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.TasksMode.Tasks import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExportList.ExportListCurrent import *
@@ -458,15 +459,16 @@
 					sfile="./db.csv"
 					print(f'{Fore.orange_3}{Path(sfile).absolute()}{Style.reset}')
 				df=df[['Barcode','Code']]
 				df.to_csv(sfile,index=False)
 			return Prompt(func=save_csv,ptext="Save Where",helpText=self.help(print_no=True),data=self).state
 		elif args[0].lower() in ["factory_reset"]:
 			#just delete db file and re-generate much simpler
-			reInit()
+			ResetTools(engine=self.engine,parent=self)
+			#reInit()
 			'''with Session(self.engine) as session:
 				done=session.query(Entry).delete()
 				session.commit()
 				session.flush()
 				print(done)'''
 			return True
 		elif args[0].lower() in ["fields","f","flds"]:
```

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 04:22 pm 04-1-2024 -- add new functionality to POS module for Billing Table management
 12:04 pm 04-2-2024 -- add massive functionality to brand new POS mode with receipt generation now in your hands
 11:59 am 04-4-2024 -- add protective measures in plus versions of Collect Mode (11) to prevent duplicate entries of data, with non-plus versions retaining initial duplicity issues should duplicity be required
 06:37 am 04-9-2024 -- add a new field userUpdated to entry so if Entry is edited with 'ie' then field will be marked true, for reference on Entries the User has edited, import will add duplicated codes to Inlist==True so Entries can be reviewed, added total_entries to unified to shortlist total entries
 09:30 am 04-13-2024 -- added new functionalty for task mode whereby if a code
 is not found a search prompt is presented, with 'r' to rset search or 'b' to
 cancel entry; added new prompts for PunchCard
+11:48 am 04-13-2024 -- replaced unified's factory_reset with a class based toolset to reset only certain, or all, components
```

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.53
+Version: 0.4.54
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.53/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.54/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
```

### Comparing `MobileInventoryCLI-0.4.53/PKG-INFO` & `MobileInventoryCLI-0.4.54/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.53
+Version: 0.4.54
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.53/setup.py` & `MobileInventoryCLI-0.4.54/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.53'
+version='0.4.54'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

