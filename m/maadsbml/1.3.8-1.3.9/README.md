# Comparing `tmp/maadsbml-1.3.8.tar.gz` & `tmp/maadsbml-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadsbml-1.3.8.tar", last modified: Mon Apr  8 17:13:02 2024, max compression
+gzip compressed data, was "maadsbml-1.3.9.tar", last modified: Sat Apr 13 18:22:42 2024, max compression
```

## Comparing `maadsbml-1.3.8.tar` & `maadsbml-1.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 17:13:02.063946 maadsbml-1.3.8/
--rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8825 2024-04-08 17:13:02.062886 maadsbml-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 17:13:02.033000 maadsbml-1.3.8/maadsbml/
--rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.8/maadsbml/__init__.py
--rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.8/maadsbml/balancedata.py
--rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.8/maadsbml/callmas.py
--rw-rw-rw-   0        0        0     7791 2024-04-08 17:12:36.000000 maadsbml-1.3.8/maadsbml/sendfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:13:02.060834 maadsbml-1.3.8/maadsbml.egg-info/
--rw-rw-rw-   0        0        0     8825 2024-04-08 17:13:01.000000 maadsbml-1.3.8/maadsbml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-08 17:13:01.000000 maadsbml-1.3.8/maadsbml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 17:13:01.000000 maadsbml-1.3.8/maadsbml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 17:13:01.000000 maadsbml-1.3.8/maadsbml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 17:13:01.000000 maadsbml-1.3.8/maadsbml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 17:13:02.063946 maadsbml-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1037 2024-04-08 17:12:46.000000 maadsbml-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:22:42.640938 maadsbml-1.3.9/
+-rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8825 2024-04-13 18:22:42.639800 maadsbml-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 18:22:42.606825 maadsbml-1.3.9/maadsbml/
+-rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.9/maadsbml/__init__.py
+-rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.9/maadsbml/balancedata.py
+-rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.9/maadsbml/callmas.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 18:20:50.000000 maadsbml-1.3.9/maadsbml/sendfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:22:42.638413 maadsbml-1.3.9/maadsbml.egg-info/
+-rw-rw-rw-   0        0        0     8825 2024-04-13 18:22:42.000000 maadsbml-1.3.9/maadsbml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-13 18:22:42.000000 maadsbml-1.3.9/maadsbml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 18:22:42.000000 maadsbml-1.3.9/maadsbml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-13 18:22:42.000000 maadsbml-1.3.9/maadsbml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 18:22:42.000000 maadsbml-1.3.9/maadsbml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 18:22:42.640938 maadsbml-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2024-04-13 18:21:02.000000 maadsbml-1.3.9/setup.py
```

### Comparing `maadsbml-1.3.8/LICENSE.txt` & `maadsbml-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.8/PKG-INFO` & `maadsbml-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.8
+Version: 1.3.9
 Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadsbml-1.3.8/README.md` & `maadsbml-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.8/maadsbml/balancedata.py` & `maadsbml-1.3.9/maadsbml/balancedata.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.8/maadsbml/callmas.py` & `maadsbml-1.3.9/maadsbml/callmas.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.8/maadsbml/sendfiles.py` & `maadsbml-1.3.9/maadsbml/sendfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
        domain=host[7:]
     host=domain  
 
     if usereverseproxy:
         geturl=formaturl(message,host,microserviceid,hbuf,port) #host contains http:// or https://
         message="GET %s\n\n" % geturl 
 
-    reader, writer = await asyncio.open_connection(host, port, loop=loop)
+    reader, writer = await asyncio.open_connection(host, port)
     try:
       mystr=str.encode(message)
       writer.write(mystr)
       datam=''
       while True:
         data = await reader.read(1024)
       #  print(data)
```

### Comparing `maadsbml-1.3.8/maadsbml.egg-info/PKG-INFO` & `maadsbml-1.3.9/maadsbml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.8
+Version: 1.3.9
 Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadsbml-1.3.8/setup.py` & `maadsbml-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadsbml',
-    version='1.3.8',
+    version='1.3.9',
     description='Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)',
     license='MIT License',
     packages=['maadsbml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

