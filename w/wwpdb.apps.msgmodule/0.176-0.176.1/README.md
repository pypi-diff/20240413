# Comparing `tmp/wwpdb.apps.msgmodule-0.176.tar.gz` & `tmp/wwpdb.apps.msgmodule-0.176.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.msgmodule-0.176.tar", last modified: Mon Apr  8 20:33:10 2024, max compression
+gzip compressed data, was "wwpdb.apps.msgmodule-0.176.1.tar", last modified: Sat Apr 13 10:10:32 2024, max compression
```

## Comparing `wwpdb.apps.msgmodule-0.176.tar` & `wwpdb.apps.msgmodule-0.176.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      301 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.352669 wwpdb.apps.msgmodule-0.176/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      151 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)    38649 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26771 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     1491 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/DateUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4420 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7771 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7384 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   269531 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingIo.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/
--rw-r--r--   0 vsts      (1001) docker     (127)    17412 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/Message.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.356669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/
--rw-r--r--   0 vsts      (1001) docker     (127)     5613 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/AutoMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27867 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/ExtractMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    83116 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4918 2024-04-08 20:31:05.000000 wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 20:33:10.360669 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 20:32:52.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-08 20:33:10.000000 wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      301 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-13 10:10:32.934486 wwpdb.apps.msgmodule-0.176.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2326 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.926486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      153 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38649 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26771 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingTemplates.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1491 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/DateUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4420 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7771 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7384 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   269531 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingIo.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17412 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/Message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5613 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/AutoMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27417 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/ExtractMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    83116 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4918 2024-04-13 10:09:00.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:10:32.930486 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1131 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:10:19.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 10:10:32.000000 wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.msgmodule-0.176/PKG-INFO` & `wwpdb.apps.msgmodule-0.176.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.176
+Version: 0.176.1
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.176/setup.py` & `wwpdb.apps.msgmodule-0.176.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingDepict.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/depict/MessagingTemplates.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/depict/MessagingTemplates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/DateUtil.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/DateUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/EmHeaderUtils.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataExport.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingDataImport.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/io/MessagingIo.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/io/MessagingIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/models/Message.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/models/Message.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/AutoMessage.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/AutoMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/util/ExtractMessage.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/util/ExtractMessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,87 +136,81 @@
         input: arg l_context_type_to_search is a list of the context types to search for.
         list is used because some searches invole multiple context_type, e.g. ["release-publ", "release-nopubl"]
 
         output: return datetime
 
         """
         ret = None
-        dc0 = self.__lc[0]
-        catObj = dc0.getObj("pdbx_deposition_message_info")
-        if catObj is None:
-            logger.warning("cannot find pdbx_deposition_message_info category in the message file for %s", self.__depid)
-            return None
-        else:
+        try:
+            dc0 = self.__lc[0]
+            catObj = dc0.getObj("pdbx_deposition_message_info")
             itDict = {}
             itNameList = catObj.getItemNameList()
             for idxIt, itName in enumerate(itNameList):
                 itDict[str(itName).lower()] = idxIt
-                #
+
             idxOrdinalId = itDict["_pdbx_deposition_message_info.ordinal_id"]
             idxLastCommDate = itDict["_pdbx_deposition_message_info.timestamp"]
             idxContextType = itDict["_pdbx_deposition_message_info.context_type"]
 
             maxOrdId = 0
             for row in catObj.getRowList():
-                try:
-                    ordinalId = int(row[idxOrdinalId])
-                    context_type_recorded = row[idxContextType]
-
-                    if context_type_recorded in l_context_type_to_search:
-                        if ordinalId > maxOrdId:
-                            maxOrdId = ordinalId
-                            ret = self.convertStrToDatetime(str(row[idxLastCommDate]))
+                ordinalId = int(row[idxOrdinalId])
+                context_type_recorded = row[idxContextType]
+
+                if context_type_recorded in l_context_type_to_search:
+                    if ordinalId > maxOrdId:
+                        maxOrdId = ordinalId
+                        ret = self.convertStrToDatetime(str(row[idxLastCommDate]))
+
+        except Exception as e:
+            logger.error("Error processing message file for %s, %s", self.__depid, e)
+            return None
 
-                except Exception as e:
-                    logger.error("Error processing message file for %s, %s", self.__depid, e)
         return ret
 
     # CS 2024-04-04 add validation letter search below by context_type/context_value
     def __getLastValidationByContextType(self):
         """Returns (datetime, major issue)  of the last time a validation was sent as determined by
         context_type and context_value
         """
 
         lastvalid = None
         major = None
-
-        dc0 = self.__lc[0]
-        catObj = dc0.getObj("pdbx_deposition_message_info")
-        if catObj is None:
-            logger.warning("cannot find pdbx_deposition_message_info category in the message file for %s", self.__depid)
-            return None
-        else:
+        try:
+            dc0 = self.__lc[0]
+            catObj = dc0.getObj("pdbx_deposition_message_info")
             itDict = {}
             itNameList = catObj.getItemNameList()
             for idxIt, itName in enumerate(itNameList):
                 itDict[str(itName).lower()] = idxIt
-                #
+
             idxOrdinalId = itDict["_pdbx_deposition_message_info.ordinal_id"]
             idxLastCommDate = itDict["_pdbx_deposition_message_info.timestamp"]
             idxContextType = itDict["_pdbx_deposition_message_info.context_type"]
             idxContextValue = itDict["_pdbx_deposition_message_info.context_value"]
 
             maxOrdId = 0
             for row in catObj.getRowList():
-                try:
-                    ordinalId = int(row[idxOrdinalId])
-                    context_type_recorded = row[idxContextType]
-                    context_value_recorded = row[idxContextValue]
-
-                    if context_type_recorded == "vldtn":
-                        if ordinalId > maxOrdId:
-                            maxOrdId = ordinalId
-                            lastvalid = self.convertStrToDatetime(str(row[idxLastCommDate]))
-                            if context_value_recorded == "major-issue-in-validation":
-                                major = True
-                            else:
-                                major = False
-
-                except Exception as e:
-                    logger.error("Error processing message file for %s, %s", self.__depid, e)
+                ordinalId = int(row[idxOrdinalId])
+                context_type_recorded = row[idxContextType]
+                context_value_recorded = row[idxContextValue]
+
+                if context_type_recorded == "vldtn":
+                    if ordinalId > maxOrdId:
+                        maxOrdId = ordinalId
+                        lastvalid = self.convertStrToDatetime(str(row[idxLastCommDate]))
+                        if context_value_recorded == "major-issue-in-validation":
+                            major = True
+                        else:
+                            major = False
+
+        except Exception as e:
+            logger.error("Error processing message file for %s, %s", self.__depid, e)
+            return (None, None)
 
         return (lastvalid, major)
 
     def convertStrToDatetime(self, s_datetime):
         return datetime.datetime.strptime(str(s_datetime), "%Y-%m-%d %H:%M:%S")
 
     def getLastMsgDatetime(self, depid, to_from="both", b_use_cache=True, test_folder=None):
```

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/MessagingWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb/apps/msgmodule/webapp/wsgi.py` & `wwpdb.apps.msgmodule-0.176.1/wwpdb/apps/msgmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/PKG-INFO` & `wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.msgmodule
-Version: 0.176
+Version: 0.176.1
 Summary: wwPDB messaging module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.msgmodule-0.176/wwpdb.apps.msgmodule.egg-info/SOURCES.txt` & `wwpdb.apps.msgmodule-0.176.1/wwpdb.apps.msgmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

