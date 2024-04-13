# Comparing `tmp/leonranp-0.1.1.tar.gz` & `tmp/leonranp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leonranp-0.1.1.tar", last modified: Fri Apr 12 13:17:03 2024, max compression
+gzip compressed data, was "leonranp-0.1.2.tar", last modified: Fri Apr 12 14:55:01 2024, max compression
```

## Comparing `leonranp-0.1.1.tar` & `leonranp-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.346235 leonranp-0.1.1/
--rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      889 2024-04-12 13:17:03.345235 leonranp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.335228 leonranp-0.1.1/leonranp/
--rw-rw-rw-   0        0        0     1067 2024-04-12 12:32:27.000000 leonranp-0.1.1/leonranp/InfoWindow.py
--rw-rw-rw-   0        0        0     6193 2024-04-12 13:12:02.000000 leonranp-0.1.1/leonranp/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-12 12:46:20.000000 leonranp-0.1.1/leonranp/test.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:17:03.345235 leonranp-0.1.1/leonranp.egg-info/
--rw-rw-rw-   0        0        0      889 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 13:17:03.000000 leonranp-0.1.1/leonranp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 13:17:03.346235 leonranp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1110 2024-04-12 13:16:52.000000 leonranp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:55:01.793640 leonranp-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      889 2024-04-12 14:55:01.792639 leonranp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 14:55:01.778114 leonranp-0.1.2/leonranp/
+-rw-rw-rw-   0        0        0     1067 2024-04-12 12:32:27.000000 leonranp-0.1.2/leonranp/InfoWindow.py
+-rw-rw-rw-   0        0        0     7319 2024-04-12 14:54:44.000000 leonranp-0.1.2/leonranp/__init__.py
+-rw-rw-rw-   0        0        0       46 2024-04-12 14:53:25.000000 leonranp-0.1.2/leonranp/test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:55:01.791641 leonranp-0.1.2/leonranp.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-04-12 14:55:01.000000 leonranp-0.1.2/leonranp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-04-12 14:55:01.000000 leonranp-0.1.2/leonranp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:55:01.000000 leonranp-0.1.2/leonranp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 14:55:01.000000 leonranp-0.1.2/leonranp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:55:01.793640 leonranp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-04-12 14:54:58.000000 leonranp-0.1.2/setup.py
```

### Comparing `leonranp-0.1.1/LICENSE.txt` & `leonranp-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `leonranp-0.1.1/PKG-INFO` & `leonranp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1.1/leonranp/InfoWindow.py` & `leonranp-0.1.2/leonranp/InfoWindow.py`

 * *Files identical despite different names*

### Comparing `leonranp-0.1.1/leonranp/__init__.py` & `leonranp-0.1.2/leonranp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,21 +95,44 @@
 #To print it,"print(randcodebs())"
 def randcodebs(digits):
     if digits == 0:
         raise RandomError("digits can't be 0!")
     randcodebs = ''
     for rsbs in range(digits):
         rcbsR = randint(0,2)
-        if rcbsR==0:
+        if rcbsR == 0:
             randcodebs = randcodebs + str(randint(0, 9))
-        elif rcbsR==1:
+        elif rcbsR == 1:
             randcodebs = randcodebs + str(rcrandstr())
         else:
             randcodebs = randcodebs + str(randstrbs())
     return randcodebs
+#randsymbol:random symbol.
+#Use print(randsymbol()) to print it.
+def randsymbol():
+    rsym = ['`','!','@','#','$','%','^','&','*','(',')','_','-','=','+','[','{',']','}',';',':','"',"'",'<','>',',','.','/','?','\\','|']
+    rsymbol = choice(rsym)
+    return rsymbol
+#randcodeall:random all rand
+#Use print(randcodeall()) to print it.
+def randcodeall(digits):
+    if digits == 0:
+        raise RandomError("digits can't be 0!")
+    randcodeall = ''
+    for rcall in range(digits):
+        rcaR = randint(0,3)
+        if rcaR == 0:
+            randcodeall = randcodeall + str(randint(0,9))     #I was so annoying of this!Has lot of bugs when I update!!!
+        elif rcaR == 1:                                             #From LeonMMcoset at 2024/4/12,22:50
+            randcodeall = randcodeall + str(rcrandstr())            #Fix this annoying bug at 2024/4/12,22:54
+        elif rcaR == 2:
+            randcodeall = randcodeall + str(randstrbs())
+        else:
+            randcodeall = randcodeall + str(randsymbol())
+    return randcodeall
 #THIS MAY CRASH YOUR IDLE,PLEASE SAVE YOUR ALL FILES!!!
 def crashidle():
     print('This may crash your IDLE!!!')
     print('Please sure you save your code!')
     while True:
         yorn = str(input('Input Y/N:'))
         if yorn =='Y' or yorn =='y':
@@ -134,14 +157,15 @@
     print('randbool() -> Random bool')
     print('dellrp() -> Delete Leon Random Plus')
     print('sample() -> Sample code')
     print('crashidle() -> Crash my IDLE')
     print('randstrbs() -> Random string that is big and small')
     print('randcodebs() -> Random code string that is big and small')
     print('lrpinfo() -> Leon Random Plus info')
+    print('randcodeall() -> Random all random thing')
     print('---Leon Random Plus Help End---')
 #Del. Leon Random Plus
 #OMG you are gonna delete Leon Random Plus???
 def dellrp():
     system(f'pip uninstall leonranp')
     print('Thanks for using Leon Random Plus!')
     print('Please restart your IDLE.')
```

### Comparing `leonranp-0.1.1/leonranp.egg-info/PKG-INFO` & `leonranp-0.1.2/leonranp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1.1/setup.py` & `leonranp-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leonranp",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1.1",  # 包版本号，便于维护版本
+    version="0.1.2",  # 包版本号，便于维护版本
     author="LeonMMcoset",  # 作者，可以写自己的姓名
     author_email="leonmmcoset@outlook.com",  # 作者联系方式，可写自己的邮箱地址
     description="This is Leon Random Plus,that add more functions to the random!",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Leonmmcoset/leonranp",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

