# Comparing `tmp/vs-colabi-1.1.2.tar.gz` & `tmp/vs-colabi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vs-colabi-1.1.2.tar", last modified: Thu Feb  8 13:02:21 2024, max compression
+gzip compressed data, was "vs-colabi-1.1.3.tar", last modified: Sat Apr 13 05:40:14 2024, max compression
```

## Comparing `vs-colabi-1.1.2.tar` & `vs-colabi-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 13:02:21.238844 vs-colabi-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-02-08 13:02:21.237844 vs-colabi-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-02-08 13:02:12.000000 vs-colabi-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-08 13:02:21.238844 vs-colabi-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2599 2024-02-08 13:02:12.000000 vs-colabi-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 13:02:21.237844 vs-colabi-1.1.2/vs_colabi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-02-08 13:02:21.000000 vs-colabi-1.1.2/vs_colabi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2024-02-08 13:02:21.000000 vs-colabi-1.1.2/vs_colabi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-08 13:02:21.000000 vs-colabi-1.1.2/vs_colabi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-02-08 13:02:21.000000 vs-colabi-1.1.2/vs_colabi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-08 13:02:21.000000 vs-colabi-1.1.2/vs_colabi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 13:02:21.237844 vs-colabi-1.1.2/vscolabi/
--rw-rw-rw-   0 root         (0) root         (0)     3314 2024-02-08 13:02:12.000000 vs-colabi-1.1.2/vscolabi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.166562 vs-colabi-1.1.3/vs_colabi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.166562 vs-colabi-1.1.3/vscolabi/
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/vscolabi/__init__.py
```

### Comparing `vs-colabi-1.1.2/PKG-INFO` & `vs-colabi-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.2
+Version: 1.1.3
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.2/README.md` & `vs-colabi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.2/setup.py` & `vs-colabi-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.2/vs_colabi.egg-info/PKG-INFO` & `vs-colabi-1.1.3/vs_colabi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.2
+Version: 1.1.3
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.2/vscolabi/__init__.py` & `vs-colabi-1.1.3/vscolabi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from IPython.display import HTML , Javascript 
 from google.colab.output import clear as clear_output
 import bashi as b 
 from google.colab import drive
 
 
 
-def configure(clear = True, mount = False  , tab = False ) : 
+def configure(clear = True, mount = False  , tab = False ,folder = "content" ) : 
     if clear : clear_output()
     if mount : drive.mount('/content/drive')
     singletab = "" if tab else ",'width=500,height=400,scrollbars=yes'"
     html_code = """
     <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Section with Button</title> <style> body {{margin: 0; padding: 0; font-family: Arial, sans-serif; }} .section {{background-color: #fff; padding: 50px; text-align: center; }} .button {{display: inline-block; padding: 20px 40px; /* Adjust padding to make the button bigger */ font-size: 25px; /* Increase font size */ background-color: #007bff; color: #fff; border: none; border-radius: 5px; cursor: pointer; width: 80%; font-weight: 400; letter-spacing: 2px ; }} </style> </head> <body> <section class="section"> <button onclick="navigator.clipboard.writeText('{code_to_authenticate}').then(function() {{window.open('https://microsoft.com/devicelogin', '_blank', 'width=500,height=400,scrollbars=yes');}} );" class = "button">Open https://microsoft.com/devicelogin and Paste code </button> </section> </body> </html>    """
-    openpath = "https://vscode.dev/tunnel/colab/content"
+    openpath = os.path.join("https://vscode.dev/tunnel/colab",folder)
     vs_code_btn  = """
       <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Section with Button</title> <style> body {{ margin: 0; padding: 0; font-family: Arial, sans-serif; }} .section {{background-color: #fff; padding: 50px; text-align: center; }} .button {{display: inline-block; padding: 20px 40px; /* Adjust padding to make the button bigger */ font-size: 25px; /* Increase font size */ background-color: #007bff; color: #fff; border: none; border-radius: 5px; cursor: pointer; width: 80%; font-weight: 400; letter-spacing: 2px ; }} </style> </head> <body> <section class="section"> <button onclick="window.open('{openpath}', '_blank' {singletab});" class = "button" >Open vs-code .</button> </section> </body> </html>    
     """.format(openpath = openpath, singletab = singletab )
     if not os.path.exists("./code") : 
         assert b.bash('''
         curl -Lk 'https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64' --output vscode_cli.tar.gz && tar -xf vscode_cli.tar.gz && rm vscode_cli.tar.gz
         ''').ok
```

