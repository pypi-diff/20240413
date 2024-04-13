# Comparing `tmp/bcelogger-1.2.0.2-py3-none-any.whl.zip` & `tmp/bcelogger-1.2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9275 bytes, number of entries: 13
--rw-r--r--  2.0 unx      611 b- defN 24-Apr-11 11:35 bcelogger/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-11 11:36 bcelogger/base_logger.py
--rw-r--r--  2.0 unx     2537 b- defN 24-Apr-11 11:35 bcelogger/db_logger.py
--rw-r--r--  2.0 unx     2286 b- defN 24-Apr-11 11:35 bcelogger/default_logger.py
--rw-r--r--  2.0 unx     1501 b- defN 24-Apr-11 11:35 bcelogger/multi_logger.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 11:35 bcelogger/conf/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_conf.py
--rw-r--r--  2.0 unx     1373 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_db_conf.py
--rw-r--r--  2.0 unx     1596 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_multi_conf.py
--rw-r--r--  2.0 unx      218 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1060 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/RECORD
-13 files, 19305 bytes uncompressed, 7501 bytes compressed:  61.1%
+Zip file size: 9341 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      610 b- defN 24-Apr-13 05:12 bcelogger/__init__.py
+-rw-r--r--  2.0 unx     6867 b- defN 24-Apr-13 05:09 bcelogger/base_logger.py
+-rw-r--r--  2.0 unx     2537 b- defN 24-Mar-06 03:13 bcelogger/db_logger.py
+-rw-r--r--  2.0 unx     2286 b- defN 24-Mar-06 03:21 bcelogger/default_logger.py
+-rw-r--r--  2.0 unx     1501 b- defN 24-Mar-06 03:13 bcelogger/multi_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-06 03:13 bcelogger/conf/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_conf.py
+-rw-r--r--  2.0 unx     1373 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_db_conf.py
+-rw-r--r--  2.0 unx     1596 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_multi_conf.py
+-rw-r--r--  2.0 unx      218 b- defN 24-Apr-13 05:12 bcelogger-1.2.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 05:12 bcelogger-1.2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-13 05:12 bcelogger-1.2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1060 b- defN 24-Apr-13 05:12 bcelogger-1.2.0.3.dist-info/RECORD
+13 files, 19606 bytes uncompressed, 7567 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: bcelogger/conf/logit_db_conf.py
 Comment: 
 
 Filename: bcelogger/conf/logit_multi_conf.py
 Comment: 
 
-Filename: bcelogger-1.2.0.2.dist-info/METADATA
+Filename: bcelogger-1.2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: bcelogger-1.2.0.2.dist-info/WHEEL
+Filename: bcelogger-1.2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: bcelogger-1.2.0.2.dist-info/top_level.txt
+Filename: bcelogger-1.2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bcelogger-1.2.0.2.dist-info/RECORD
+Filename: bcelogger-1.2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bcelogger/__init__.py

```diff
@@ -1,13 +1,12 @@
 # #########################################################################################
 # logit用到了logger的stacklevel参数，此参数在py3.8版本加入的，所以需要进行版本区分
 # python version < 3.8 版本，logit不支持tag，例如：
 # logit.debug("this is %s log", "debug", log_id=123456, tag1="value1", tag2=123456)
 # #########################################################################################
-
 from . import base_logger
 if base_logger._logger is None:
     _logger = base_logger.setup_logger()
 
 from .default_logger import *
```

## bcelogger/base_logger.py

```diff
@@ -61,14 +61,20 @@
             file_path = os.path.join(os.getcwd(), conf_file_path)
             log_dir = os.path.dirname(file_path)
 
         # 创建log目录
         Logger.make_log_dir(log_dir)
 
         logger_name = config_dict.get("logger_name")
+        if logger_name in logging.Logger.manager.loggerDict:
+            logging.getLogger(logger_name).handlers = []
+            logging.getLogger(logger_name).propagate = False
+            logging.getLogger(logger_name).disabled = True
+            logging.Logger.manager.loggerDict.pop(logger_name)
+
         self.logger = logging.getLogger(logger_name)
         self.logger.setLevel(logging.DEBUG)
 
         # 日志格式
         log_fmt = '%(levelname)s: %(asctime)s %(filename)s[line:%(lineno)d] Thread:%(thread)d %(message)s'
         # 默认日志时间精确到秒，default_ms参数精确到毫秒
         date_fmt = '%Y-%m-%d %H:%M:%S'
```

