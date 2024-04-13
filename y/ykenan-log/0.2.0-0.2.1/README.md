# Comparing `tmp/ykenan_log-0.2.0.tar.gz` & `tmp/ykenan_log-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_log-0.2.0.tar", last modified: Fri Mar 17 08:49:28 2023, max compression
+gzip compressed data, was "ykenan_log-0.2.1.tar", last modified: Sat Apr 13 04:51:32 2024, max compression
```

## Comparing `ykenan_log-0.2.0.tar` & `ykenan_log-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 08:49:28.384430 ykenan_log-0.2.0/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_log-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_log-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2399 2023-03-17 08:49:28.384430 ykenan_log-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-03-17 08:49:27.000000 ykenan_log-0.2.0/README.md
--rw-rw-rw-   0        0        0      652 2023-03-17 08:49:27.000000 ykenan_log-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       17 2023-03-17 07:15:38.000000 ykenan_log-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 08:49:28.384430 ykenan_log-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-17 08:49:28.370431 ykenan_log-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-17 08:49:28.377431 ykenan_log-0.2.0/src/ykenan_log/
--rw-rw-rw-   0        0        0     8503 2023-03-17 08:49:27.000000 ykenan_log-0.2.0/src/ykenan_log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-17 08:49:28.383431 ykenan_log-0.2.0/src/ykenan_log.egg-info/
--rw-rw-rw-   0        0        0     2399 2023-03-17 08:49:28.000000 ykenan_log-0.2.0/src/ykenan_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-03-17 08:49:28.000000 ykenan_log-0.2.0/src/ykenan_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 08:49:28.000000 ykenan_log-0.2.0/src/ykenan_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-17 08:49:28.000000 ykenan_log-0.2.0/src/ykenan_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-17 08:49:28.000000 ykenan_log-0.2.0/src/ykenan_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 04:51:32.184096 ykenan_log-0.2.1/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_log-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_log-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2459 2024-04-13 04:51:32.184096 ykenan_log-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1931 2024-04-13 04:51:08.000000 ykenan_log-0.2.1/README.md
+-rw-rw-rw-   0        0        0      652 2024-04-13 04:13:56.000000 ykenan_log-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2023-03-17 07:15:38.000000 ykenan_log-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 04:51:32.184096 ykenan_log-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 04:51:32.161817 ykenan_log-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 04:51:32.165817 ykenan_log-0.2.1/src/ykenan_log/
+-rw-rw-rw-   0        0        0     8519 2024-04-13 04:17:57.000000 ykenan_log-0.2.1/src/ykenan_log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:51:32.183097 ykenan_log-0.2.1/src/ykenan_log.egg-info/
+-rw-rw-rw-   0        0        0     2459 2024-04-13 04:51:32.000000 ykenan_log-0.2.1/src/ykenan_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-13 04:51:32.000000 ykenan_log-0.2.1/src/ykenan_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 04:51:32.000000 ykenan_log-0.2.1/src/ykenan_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 04:51:32.000000 ykenan_log-0.2.1/src/ykenan_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-13 04:51:32.000000 ykenan_log-0.2.1/src/ykenan_log.egg-info/top_level.txt
```

### Comparing `ykenan_log-0.2.0/LICENSE` & `ykenan_log-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_log-0.2.0/PKG-INFO` & `ykenan_log-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ykenan_log
-Version: 0.2.0
+Version: 0.2.1
 Summary: Log information: Print the log, export the log file.
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_log
 Keywords: ykenan,log,file
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: coloredlogs>=15.0
 
 # ykenan_log
 
 > **`Print and save a simple log to a file`**
 
 This is a simple log package. You can see
 [Github-ykenan_log](https://github.com/YuZhengM/ykenan_log)
+[PyPI-ykenan_log](https://pypi.org/project/ykenan-log/)
 
 > upload
 
 ```shell
 py -m build
 twine check dist/*
 twine upload dist/*
@@ -36,63 +38,62 @@
 ```
 
 > use
 
 ```python
 # -*- coding: utf-8 -*-
 
-import ykenan_log
+from ykenan_log import Logger
 
-logger = ykenan_log.Logger("name", "log")
+log = Logger("name", "log")
 
 if __name__ == '__main__':
     print("run...")
-    logger.debug("info......")
-    logger.info("info......")
-    logger.warn("info......")
-    logger.error("info......")
+    log.debug("info......")
+    log.info("info......")
+    log.warn("info......")
+    log.error("info......")
 ```
 
 > output
 
 ```shell
-run...
 2023-03-17 09:21:36 root name[34768] DEBUG info......
 2023-03-17 09:21:36 root name[34768] INFO info......
 2023-03-17 09:21:36 root name[34768] WARNING info......
 2023-03-17 09:21:36 root name[34768] ERROR info......
 
 ```
 
 ## Introduction
 
 > **main function**
 
-> ykenan_log.Logger(
+> ykenan_log.`Logger`(
 >> name: str = None,
-> 
+>
 >> log_path: str = None,
-> 
->> level: str = "DEBUG",
-> 
+>
+>> level: str = "INFO",
+>
 >> is_solitary: bool = True,
-> 
+>
 >> is_form_file: bool = True,
-> 
+>
 >> size: int = 104857600,
-> 
+>
 >> backup_count: int = 10,
-> 
+>
 >> encoding: str = "UTF-8"
-> 
-> ) 
+>
+> )
 
 ```
 :param name: Project Name
 :param log_path: Log file output path. Default is log_%Y%m%d.log.
-:param level: Log printing level. Default is DEBUG.
+:param level: Log printing level. Default is INFO.
 :param is_solitary: When the file path is consistent (here, the log_path parameter is not a specific file name, but a file path), whether the file is formed independently according to the name parameter. Default is True.
 :param is_form_file: Whether to form a log file. Default is True.
 :param size: Setting the file size if a file is formed. Default is 104857600. (100MB)
 :param backup_count: Setting the number of rotating files if a file is formed. Default is 10.
 :param encoding: Setting of file encoding if a file is formed. Default is UTF-8.
 ```
```

### Comparing `ykenan_log-0.2.0/README.md` & `ykenan_log-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ykenan_log
 
 > **`Print and save a simple log to a file`**
 
 This is a simple log package. You can see
 [Github-ykenan_log](https://github.com/YuZhengM/ykenan_log)
+[PyPI-ykenan_log](https://pypi.org/project/ykenan-log/)
 
 > upload
 
 ```shell
 py -m build
 twine check dist/*
 twine upload dist/*
@@ -22,63 +23,62 @@
 ```
 
 > use
 
 ```python
 # -*- coding: utf-8 -*-
 
-import ykenan_log
+from ykenan_log import Logger
 
-logger = ykenan_log.Logger("name", "log")
+log = Logger("name", "log")
 
 if __name__ == '__main__':
     print("run...")
-    logger.debug("info......")
-    logger.info("info......")
-    logger.warn("info......")
-    logger.error("info......")
+    log.debug("info......")
+    log.info("info......")
+    log.warn("info......")
+    log.error("info......")
 ```
 
 > output
 
 ```shell
-run...
 2023-03-17 09:21:36 root name[34768] DEBUG info......
 2023-03-17 09:21:36 root name[34768] INFO info......
 2023-03-17 09:21:36 root name[34768] WARNING info......
 2023-03-17 09:21:36 root name[34768] ERROR info......
 
 ```
 
 ## Introduction
 
 > **main function**
 
-> ykenan_log.Logger(
+> ykenan_log.`Logger`(
 >> name: str = None,
-> 
+>
 >> log_path: str = None,
-> 
->> level: str = "DEBUG",
-> 
+>
+>> level: str = "INFO",
+>
 >> is_solitary: bool = True,
-> 
+>
 >> is_form_file: bool = True,
-> 
+>
 >> size: int = 104857600,
-> 
+>
 >> backup_count: int = 10,
-> 
+>
 >> encoding: str = "UTF-8"
-> 
-> ) 
+>
+> )
 
 ```
 :param name: Project Name
 :param log_path: Log file output path. Default is log_%Y%m%d.log.
-:param level: Log printing level. Default is DEBUG.
+:param level: Log printing level. Default is INFO.
 :param is_solitary: When the file path is consistent (here, the log_path parameter is not a specific file name, but a file path), whether the file is formed independently according to the name parameter. Default is True.
 :param is_form_file: Whether to form a log file. Default is True.
 :param size: Setting the file size if a file is formed. Default is 104857600. (100MB)
 :param backup_count: Setting the number of rotating files if a file is formed. Default is 10.
 :param encoding: Setting of file encoding if a file is formed. Default is UTF-8.
 ```
```

### Comparing `ykenan_log-0.2.0/pyproject.toml` & `ykenan_log-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "coloredlogs>=15.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_log"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "log", "file"]
 description = "Log information: Print the log, export the log file."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_log-0.2.0/src/ykenan_log/__init__.py` & `ykenan_log-0.2.1/src/ykenan_log/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,36 +41,38 @@
 
 
 class LoggerExec:
     """
     Log Set
     """
 
-    def __init__(self, name: str = None, log_path: str = None, level: str = "DEBUG", is_solitary: bool = True,
-                 is_form_file: bool = True, size: int = 104857600, backup_count: int = 10, encoding: str = "UTF-8"):
+    def __init__(
+        self, name: str = None, log_path: str = None, level: str = "INFO", is_solitary: bool = True,
+        is_form_file: bool = False, size: int = 104857600, backup_count: int = 10, encoding: str = "UTF-8"
+    ):
         """
         Log initialization
         :param name: Project Name
         :param log_path: Log file output path. Default is log_%Y%m%d.log.
-        :param level: Log printing level. Default is DEBUG.
+        :param level: Log printing level. Default is INFO.
         :param is_solitary: When the file path is consistent (here, the log_path parameter is not a specific file name, but a file path), whether the file is formed independently according to the name parameter. Default is True.
         :param is_form_file: Whether to form a log file. Default is True.
         :param size: Setting the file size if a file is formed. Default is 104857600. (100MB)
         :param backup_count: Setting the number of rotating files if a file is formed. Default is 10.
         :param encoding: Setting of file encoding if a file is formed. Default is UTF-8.
         """
         self.name = name
         self.log_path = log_path
         self.level = level
         # Get Today's Time
         self.today = datetime.datetime.now().strftime("%Y%m%d")
         # Default File Name
         self.default_log_file = f"{name}_log_{self.today}.log" if name and is_solitary else f"log_{self.today}.log"
 
-        self.log_path_name = self.getLogPath() if is_form_file else None
+        self.log_path_name = self.get_log_path() if is_form_file else None
 
         # Define two log output formats
         standard_format = '[%(asctime)s] [%(threadName)s:%(thread)d] [task_id:%(name)s] [%(filename)s:%(lineno)d] [%(levelname)s] ===> %(message)s'
         simple_format = '[%(levelname)s] [%(asctime)s] [%(filename)s:%(lineno)d] ===> %(message)s'
 
         # Log printed to the terminal
         handlers_sh = {
@@ -142,15 +144,15 @@
             },
             'error': {
                 'color': 'red',
                 'bold': True,
             }
         }
 
-    def getLogPath(self) -> str:
+    def get_log_path(self) -> str:
         """
         Get log output path
         :return:
         """
         # Determine whether it exists
         if self.log_path:
             log_path_file = self.log_path if self.log_path.endswith(".log") else os.path.join(self.log_path, self.default_log_file)
@@ -177,21 +179,23 @@
 
 
 class Logger:
     """
     Log initialization
     """
 
-    def __init__(self, name: str = None, log_path: str = None, level: str = "DEBUG", is_solitary: bool = True,
-                 is_form_file: bool = True, size: int = 104857600, backup_count: int = 10, encoding: str = "UTF-8"):
+    def __init__(
+        self, name: str = None, log_path: str = None, level: str = "INFO", is_solitary: bool = True,
+        is_form_file: bool = False, size: int = 104857600, backup_count: int = 10, encoding: str = "UTF-8"
+    ):
         """
         Log initialization
         :param name: Project Name
         :param log_path: Log file output path. Default is log_%Y%m%d.log.
-        :param level: Log printing level. Default is DEBUG.
+        :param level: Log printing level. Default is INFO.
         :param is_solitary: When the file path is consistent (here, the log_path parameter is not a specific file name, but a file path), whether the file is formed independently according to the name parameter. Default is True.
         :param is_form_file: Whether to form a log file. Default is True.
         :param size: Setting the file size if a file is formed. Default is 104857600. (100MB)
         :param backup_count: Setting the number of rotating files if a file is formed. Default is 10.
         :param encoding: Setting of file encoding if a file is formed. Default is UTF-8.
         """
         self.name = name
```

### Comparing `ykenan_log-0.2.0/src/ykenan_log.egg-info/PKG-INFO` & `ykenan_log-0.2.1/src/ykenan_log.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: ykenan-log
-Version: 0.2.0
+Name: ykenan_log
+Version: 0.2.1
 Summary: Log information: Print the log, export the log file.
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_log
 Keywords: ykenan,log,file
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: coloredlogs>=15.0
 
 # ykenan_log
 
 > **`Print and save a simple log to a file`**
 
 This is a simple log package. You can see
 [Github-ykenan_log](https://github.com/YuZhengM/ykenan_log)
+[PyPI-ykenan_log](https://pypi.org/project/ykenan-log/)
 
 > upload
 
 ```shell
 py -m build
 twine check dist/*
 twine upload dist/*
@@ -36,63 +38,62 @@
 ```
 
 > use
 
 ```python
 # -*- coding: utf-8 -*-
 
-import ykenan_log
+from ykenan_log import Logger
 
-logger = ykenan_log.Logger("name", "log")
+log = Logger("name", "log")
 
 if __name__ == '__main__':
     print("run...")
-    logger.debug("info......")
-    logger.info("info......")
-    logger.warn("info......")
-    logger.error("info......")
+    log.debug("info......")
+    log.info("info......")
+    log.warn("info......")
+    log.error("info......")
 ```
 
 > output
 
 ```shell
-run...
 2023-03-17 09:21:36 root name[34768] DEBUG info......
 2023-03-17 09:21:36 root name[34768] INFO info......
 2023-03-17 09:21:36 root name[34768] WARNING info......
 2023-03-17 09:21:36 root name[34768] ERROR info......
 
 ```
 
 ## Introduction
 
 > **main function**
 
-> ykenan_log.Logger(
+> ykenan_log.`Logger`(
 >> name: str = None,
-> 
+>
 >> log_path: str = None,
-> 
->> level: str = "DEBUG",
-> 
+>
+>> level: str = "INFO",
+>
 >> is_solitary: bool = True,
-> 
+>
 >> is_form_file: bool = True,
-> 
+>
 >> size: int = 104857600,
-> 
+>
 >> backup_count: int = 10,
-> 
+>
 >> encoding: str = "UTF-8"
-> 
-> ) 
+>
+> )
 
 ```
 :param name: Project Name
 :param log_path: Log file output path. Default is log_%Y%m%d.log.
-:param level: Log printing level. Default is DEBUG.
+:param level: Log printing level. Default is INFO.
 :param is_solitary: When the file path is consistent (here, the log_path parameter is not a specific file name, but a file path), whether the file is formed independently according to the name parameter. Default is True.
 :param is_form_file: Whether to form a log file. Default is True.
 :param size: Setting the file size if a file is formed. Default is 104857600. (100MB)
 :param backup_count: Setting the number of rotating files if a file is formed. Default is 10.
 :param encoding: Setting of file encoding if a file is formed. Default is UTF-8.
 ```
```

