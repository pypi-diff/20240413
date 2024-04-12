# Comparing `tmp/MobileInventoryCLI-0.4.49.tar.gz` & `tmp/MobileInventoryCLI-0.4.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.49.tar", last modified: Wed Apr 10 17:00:24 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.50.tar", last modified: Fri Apr 12 17:05:37 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.49.tar` & `MobileInventoryCLI-0.4.50.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.241023 MobileInventoryCLI-0.4.49/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.241023 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   104240 2024-04-10 16:58:46.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.244356 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28296 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-10 17:00:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.247690 MobileInventoryCLI-0.4.49/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-09 17:38:18.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-10 17:00:24.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4810 2024-04-10 17:00:24.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-10 17:00:24.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-10 17:00:24.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-10 17:00:24.000000 MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-10 17:00:24.251023 MobileInventoryCLI-0.4.49/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-10 17:00:23.000000 MobileInventoryCLI-0.4.49/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.827962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.831296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.831296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6346 2024-04-12 17:05:15.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   104240 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.834629 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    16273 2024-04-12 16:38:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28296 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-12 17:05:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-10 19:14:50.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.837962 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-10 17:00:32.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4946 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-12 17:05:37.841296 MobileInventoryCLI-0.4.50/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-12 17:05:37.000000 MobileInventoryCLI-0.4.50/setup.py
```

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ConvertCode.ConvertCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.setCode.setCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Locator.Locator import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ListMode2.ListMode2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.TasksMode.Tasks import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExportList.ExportListCurrent import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
-
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.DatePicker import *
 
 import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.possibleCode as pc
 
 class PunchCard:
 	datePicker=datePickerF
 	datetimePicker=datetimePickerF
 	""" def datePicker(self):
@@ -118,14 +118,15 @@
 {Fore.light_green}vdr|view_date_range{Style.reset} -{Fore.cyan} view a date ranges data{Style.reset}
 {Fore.light_green}d|duration{Style.reset} -{Fore.cyan} view current punch's duration{Style.reset}
 {Fore.light_green}va|view_all{Style.reset} -{Fore.cyan} view all punches{Style.reset}
 {Fore.light_green}gross{Style.reset} -{Fore.cyan}calculate gross income from prompted date's total duration with rate of pay as hourly{Style.reset}
 {Fore.light_green}e[4..8]{Style.reset} -{Fore.cyan}estimate shift punches from datetime.now(){Style.reset}
 {Fore.light_green}me[4..8]|manual_estimate_[4..8]h{Style.reset} -{Fore.cyan}manually estimate shift punches from datetime.now(){Style.reset}
 {Fore.light_green}enow|estimate_now|shift_help{Style.reset} -{Fore.cyan}show estimated punch data for Right-Now!{Style.reset}
+{Fore.light_green}calculate_earnings_1|ce1{Style.reset} -{Fore.cyan}show estimated earnings!{Style.reset}
 '''
 		def mkT(text,self):
 			return text
 		while True:
 			cmd=Prompt.__init2__(None,func=mkT,ptext="Do What?",helpText=self.helpText,data=self)
 			if cmd in [None,]:
 				return
@@ -151,14 +152,16 @@
 									break
 								s.gross(rate=rate)
 							else:
 								print(f"{Fore.light_red}No Punches For that date!{Style.reset}")
 							break
 					except Exception as e:
 						print(e)
+			elif cmd.lower() in 'calculate_earnings_1|ce1'.split('|'):
+				CalculateEarnings()
 			elif cmd.lower() in ['e8']:
 				Shift.estimatedPunches_8h(None)
 			elif cmd.lower() in ['me8','manual_estimate_8h']:
 				Shift.manual_estimate_8(Shift)
 			elif cmd.lower() in ['e7']:
 				Shift.estimatedPunches_7h(None)
 			elif cmd.lower() in ['me7','manual_estimate_7h']:
```

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.49
+Version: 0.4.50
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.49/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.50/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
```

### Comparing `MobileInventoryCLI-0.4.49/PKG-INFO` & `MobileInventoryCLI-0.4.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.49
+Version: 0.4.50
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.49/setup.py` & `MobileInventoryCLI-0.4.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.49'
+version='0.4.50'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

