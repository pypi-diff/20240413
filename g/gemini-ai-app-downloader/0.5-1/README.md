# Comparing `tmp/gemini_ai_app_downloader-0.5.tar.gz` & `tmp/gemini_ai_app_downloader-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ai_app_downloader-0.5.tar", last modified: Sun Mar 24 07:43:34 2024, max compression
+gzip compressed data, was "gemini_ai_app_downloader-1.tar", last modified: Sat Apr 13 09:17:00 2024, max compression
```

## Comparing `gemini_ai_app_downloader-0.5.tar` & `gemini_ai_app_downloader-1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-03-24 07:43:34.516929 gemini_ai_app_downloader-0.5/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-0.5/LICENSE
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      798 2024-03-24 07:43:34.516848 gemini_ai_app_downloader-0.5/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      124 2024-03-24 07:06:10.000000 gemini_ai_app_downloader-0.5/README.md
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-03-24 07:43:34.516581 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      798 2024-03-24 07:43:34.000000 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-03-24 07:43:34.000000 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-03-24 07:43:34.000000 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-03-24 07:43:34.000000 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/entry_points.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-03-24 07:43:34.000000 gemini_ai_app_downloader-0.5/gemini_ai_app_downloader.egg-info/top_level.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-03-24 07:43:34.517386 gemini_ai_app_downloader-0.5/setup.cfg
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1104 2024-03-24 07:39:30.000000 gemini_ai_app_downloader-0.5/setup.py
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-13 09:17:00.507322 gemini_ai_app_downloader-1/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-1/LICENSE
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3346 2024-04-13 09:17:00.507240 gemini_ai_app_downloader-1/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     2675 2024-04-13 09:10:55.000000 gemini_ai_app_downloader-1/README.md
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-13 09:17:00.506885 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3346 2024-04-13 09:17:00.000000 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-04-13 09:17:00.000000 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-04-13 09:17:00.000000 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-04-13 09:17:00.000000 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-04-13 09:17:00.000000 gemini_ai_app_downloader-1/gemini_ai_app_downloader.egg-info/top_level.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-04-13 09:17:00.507653 gemini_ai_app_downloader-1/setup.cfg
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1102 2024-04-13 08:50:47.000000 gemini_ai_app_downloader-1/setup.py
```

### Comparing `gemini_ai_app_downloader-0.5/LICENSE` & `gemini_ai_app_downloader-1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_ai_app_downloader-0.5/setup.py` & `gemini_ai_app_downloader-1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
         return long_description
 
 
 setup(
     name='gemini_ai_app_downloader',
-    version='0.5',
+    version='1',
     packages=['gemini_ai_app_downloader'],
     url='https://github.com/SoftwareApkDev/gemini_ai_app_downloader',
     license='MIT',
     author='SoftwareApkDev',
     author_email='softwareapkdev2022@gmail.com',
     description='This package contains implementation of the downloader of applications with '
                 'Google Gemini AI integrated into them.',
```

