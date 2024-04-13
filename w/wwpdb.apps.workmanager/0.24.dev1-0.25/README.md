# Comparing `tmp/wwpdb.apps.workmanager-0.24.dev1.tar.gz` & `tmp/wwpdb.apps.workmanager-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.workmanager-0.24.dev1.tar", last modified: Fri Dec 29 20:32:35 2023, max compression
+gzip compressed data, was "wwpdb.apps.workmanager-0.25.tar", last modified: Sat Apr 13 10:04:44 2024, max compression
```

## Comparing `wwpdb.apps.workmanager-0.24.dev1.tar` & `wwpdb.apps.workmanager-0.25.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1165 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      380 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2420 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.232535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.232535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.232535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/
--rw-r--r--   0 vsts      (1001) docker     (127)      155 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.236535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/
--rw-r--r--   0 vsts      (1001) docker     (127)     9693 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/ContentDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5797 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/DBLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6928 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7398 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/StatsUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32606 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/StatusDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.236535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)    17674 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30539 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictContent.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3986 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictGroup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2392 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictLevel1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7223 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictOther.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5225 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictSnapShot.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10849 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictWorkFlow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14653 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/Level1Util.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11655 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/ReadConFigFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4973 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/SearchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1950 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/ServerInfoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.240535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/
--rw-r--r--   0 vsts      (1001) docker     (127)     1969 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/AnnotAssignUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9190 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/CopyFileToAutoGroup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2169 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/LogFileUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3551 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/MileStoneFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5303 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/SnapShotDiff.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.240535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/
--rw-r--r--   0 vsts      (1001) docker     (127)     7356 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/BaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5925 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/CifChecker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3222 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/LigandFinder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17352 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/MetaDataEditor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5811 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/MetaDataMerger.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4395 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/PdbFileGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5170 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/SequenceMerger.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9626 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/StatusUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.240535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)    11854 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/LoadRemindMessageTrack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4631 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/ManageSite.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    58618 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/webapp/WorkManagerWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/
--rw-r--r--   0 vsts      (1001) docker     (127)    46458 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/OrderedDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4320 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/WorkflowXMLLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-29 20:31:21.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-29 20:32:35.244535 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1165 2023-12-29 20:32:35.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2376 2023-12-29 20:32:35.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-29 20:32:35.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-29 20:32:22.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      233 2023-12-29 20:32:35.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2023-12-29 20:32:35.000000 wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1203 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      380 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2475 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.729879 wwpdb.apps.workmanager-0.25/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.733878 wwpdb.apps.workmanager-0.25/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.733878 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.737879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9693 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/ContentDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5797 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/DBLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6928 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7398 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/StatsUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32606 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/StatusDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.741879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17674 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30539 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictContent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3986 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictGroup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2392 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictLevel1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7223 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictOther.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5225 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictSnapShot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10849 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictWorkFlow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14653 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/Level1Util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11655 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/ReadConFigFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4973 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/SearchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/ServerInfoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.741879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1969 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/AnnotAssignUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9190 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/CopyFileToAutoGroup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2169 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/LogFileUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3551 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/MileStoneFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5303 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/SnapShotDiff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.741879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7356 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/BaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5925 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/CifChecker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3222 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/LigandFinder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17352 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/MetaDataEditor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/MetaDataMerger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4395 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/PdbFileGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5170 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/SequenceMerger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9626 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/StatusUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.741879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11854 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/LoadRemindMessageTrack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4631 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/ManageSite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    58707 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/webapp/WorkManagerWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/
+-rw-r--r--   0 vsts      (1001) docker     (127)    46458 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/OrderedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4320 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/WorkflowXMLLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:03:03.000000 wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:04:44.745879 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1203 2024-04-13 10:04:44.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2376 2024-04-13 10:04:44.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:04:44.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:04:04.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      261 2024-04-13 10:04:44.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 10:04:44.000000 wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.workmanager-0.24.dev1/PKG-INFO` & `wwpdb.apps.workmanager-0.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.workmanager
-Version: 0.24.dev1
+Version: 0.25
 Summary: wwPDB workflow manager app
 Home-page: https://github.com/rcsb/py-wwpdb_apps_workmanager
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: wwpdb.utils.config~=0.27
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.io~=0.6
 Requires-Dist: rcsb.utils.multiproc
 Requires-Dist: wwpdb.apps.wf_engine>=0.5
+Requires-Dist: wwpdb.apps.msgmodule~=0.176
 Requires-Dist: wwpdb.utils.db>=0.4
 Requires-Dist: wwpdb.utils.session>=0.3
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.detach~=0.3
 Requires-Dist: mysqlclient
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
```

### Comparing `wwpdb.apps.workmanager-0.24.dev1/setup.py` & `wwpdb.apps.workmanager-0.25/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     #
     install_requires=['wwpdb.utils.config ~= 0.27', 'wwpdb.utils.wf', 'wwpdb.io ~= 0.6',
                       'rcsb.utils.multiproc', 'wwpdb.apps.wf_engine >= 0.5',
+                      'wwpdb.apps.msgmodule ~= 0.176',
                       'wwpdb.utils.db >= 0.4', 'wwpdb.utils.session >= 0.3',
                       'mmcif.utils', 'wwpdb.utils.detach ~= 0.3', 'mysqlclient'],
     packages=find_packages(exclude=['wwpdb.apps.tests-workmanager']),
     # Enables Manifest to be used
     # include_package_data = True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
```

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/ContentDbApi.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/ContentDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/DBLoader.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/DBLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/DbApiUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/StatsUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/StatsUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/db_access/StatusDbApi.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/db_access/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictBase.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictContent.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictContent.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictGroup.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictGroup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictLevel1.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictLevel1.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictOther.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictOther.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictSnapShot.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictSnapShot.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/DepictWorkFlow.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/DepictWorkFlow.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/Level1Util.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/Level1Util.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/ReadConFigFile.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/ReadConFigFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/SearchUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/SearchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/depict/ServerInfoUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/depict/ServerInfoUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/AnnotAssignUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/AnnotAssignUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/CopyFileToAutoGroup.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/CopyFileToAutoGroup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/LogFileUtil.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/LogFileUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/MileStoneFile.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/MileStoneFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/file_access/SnapShotDiff.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/file_access/SnapShotDiff.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/BaseClass.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/BaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/CifChecker.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/CifChecker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/LigandFinder.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/LigandFinder.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/MetaDataEditor.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/MetaDataEditor.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/MetaDataMerger.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/MetaDataMerger.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/PdbFileGenerator.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/PdbFileGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/SequenceMerger.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/SequenceMerger.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/task_access/StatusUpdater.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/task_access/StatusUpdater.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/LoadRemindMessageTrack.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/LoadRemindMessageTrack.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/utils/ManageSite.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/utils/ManageSite.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/webapp/WorkManagerWebApp.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/webapp/WorkManagerWebApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import os
 import subprocess
 import sys
 import time
 import traceback
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.apps.wf_engine.engine.WFEapplications import reRunWorkflow, DepUIgetDepositorEmail, WFEsendEmail, getPicklePath, getNotesEmailAddr
+from wwpdb.apps.wf_engine.engine.WFEapplications import reRunWorkflow, getPicklePath
 from wwpdb.apps.workmanager.db_access.DBLoader import DBLoader
 from wwpdb.apps.workmanager.db_access.StatusDbApi import StatusDbApi
 from wwpdb.apps.workmanager.depict.DepictBase import DepictBase
 from wwpdb.apps.workmanager.depict.DepictContent import DepictContent
 from wwpdb.apps.workmanager.depict.DepictGroup import DepictGroup
 from wwpdb.apps.workmanager.depict.DepictLevel1 import DepictLevel1
 from wwpdb.apps.workmanager.depict.DepictOther import DepictOther
@@ -57,14 +57,15 @@
 from wwpdb.apps.workmanager.task_access.SequenceMerger import SequenceMerger
 from wwpdb.apps.workmanager.task_access.StatusUpdater import StatusUpdater
 from wwpdb.utils.detach.DetachUtils import DetachUtils
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.utils.session.WebRequest import InputRequest, ResponseContent
 from wwpdb.utils.session.WebUploadUtils import WebUploadUtils
 from wwpdb.utils.config.ProjectVersionInfo import ProjectVersionInfo
+from wwpdb.apps.msgmodule.util.AutoMessage import AutoMessage
 #
 
 
 class WorkManagerWebApp(object):
     """Handle request and response object processing for release module web application.
 
     """
@@ -524,27 +525,27 @@
         #
         text = ''
         try:
             # create a pickle file, which is used to check if FTP upload was allowed
             storage_pickle_path = self.__get_deposit_storage_pickle_path('externalUpload.pkl')
             self.__dump_deposit_storage_pickle(storage_pickle_path, 'File upload in depUI failed; FTP upload enabled by Annotator from WFM')
             # send instructions email to depositor
-            frm = self.__cI.get("SITE_NOREPLY_EMAIL", "noreply@mail.wwpdb.org")
-            email = DepUIgetDepositorEmail(depositionid)
             subject = 'Instructions for wwPDB FTP upload for deposition ' + depositionid
             myD = {}
             myD['depositionid'] = depositionid
             myD['ftp_host_name'] = self.__cI.get('FTP_HOST_NAME')
             myD['ftp_port_number'] = self.__cI.get('FTP_PORT_NUMBER')
             myD['ftp_connect_details_0'] = self.__cI.get('FTP_CONNECT_DETAILS')[0]
             myD['ftp_connect_details_1'] = self.__cI.get('FTP_CONNECT_DETAILS')[1]
             myD['site_dep_email_url'] = self.__cI.get('SITE_DEP_EMAIL_URL')
             message = self.__processTemplate('ftp_message.txt', myD)
-            WFEsendEmail(email, frm, subject, message, getNotesEmailAddr())
+            am = AutoMessage(siteId=self.__siteId)
+            ret = am.sendSingleMessage(depositionid, subject, message, p_tmpltType="instruction-ftp")  # CS 2024-04-04 add template type
             text = 'FTP upload enabled; email sent to the user'
+            self.__lfh.write("+WorkManagerWebAppWorker._EnableFtpUploadOp() sent message status=%s\n" % ret)
         except Exception as e:
             self.__lfh.write("+WorkManagerWebAppWorker._EnableFtpUploadOp() Failed to enable file import and/or send instructions to the depositor %s\n" % str(e))
             error = 'Failed in enable file import to depUI; instructions not sent'
         #
         return self.__returnJsonObject(text, error)
 
     def _RerunWorkFlowOp(self):
```

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/OrderedDict.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb/apps/workmanager/workflow_access/WorkflowXMLLoader.py` & `wwpdb.apps.workmanager-0.25/wwpdb/apps/workmanager/workflow_access/WorkflowXMLLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/PKG-INFO` & `wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.workmanager
-Version: 0.24.dev1
+Version: 0.25
 Summary: wwPDB workflow manager app
 Home-page: https://github.com/rcsb/py-wwpdb_apps_workmanager
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: wwpdb.utils.config~=0.27
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.io~=0.6
 Requires-Dist: rcsb.utils.multiproc
 Requires-Dist: wwpdb.apps.wf_engine>=0.5
+Requires-Dist: wwpdb.apps.msgmodule~=0.176
 Requires-Dist: wwpdb.utils.db>=0.4
 Requires-Dist: wwpdb.utils.session>=0.3
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.detach~=0.3
 Requires-Dist: mysqlclient
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
```

### Comparing `wwpdb.apps.workmanager-0.24.dev1/wwpdb.apps.workmanager.egg-info/SOURCES.txt` & `wwpdb.apps.workmanager-0.25/wwpdb.apps.workmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

