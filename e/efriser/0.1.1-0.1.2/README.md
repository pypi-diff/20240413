# Comparing `tmp/efriser-0.1.1.tar.gz` & `tmp/efriser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.1.tar", last modified: Sat Apr 13 17:29:45 2024, max compression
+gzip compressed data, was "efriser-0.1.2.tar", last modified: Sat Apr 13 17:44:23 2024, max compression
```

## Comparing `efriser-0.1.1.tar` & `efriser-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:29:45.435062 efriser-0.1.1/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      273 2024-04-13 17:29:45.435062 efriser-0.1.1/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      158 2024-04-13 17:29:42.000000 efriser-0.1.1/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:29:45.431062 efriser-0.1.1/efriser/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       29 2024-04-13 17:24:52.000000 efriser-0.1.1/efriser/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6226 2024-04-13 17:21:14.000000 efriser-0.1.1/efriser/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.1/efriser/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.1/efriser/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.1/efriser/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.1/efriser/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:29:45.435062 efriser-0.1.1/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      273 2024-04-13 17:29:45.000000 efriser-0.1.1/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      295 2024-04-13 17:29:45.000000 efriser-0.1.1/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 17:29:45.000000 efriser-0.1.1/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 17:29:45.000000 efriser-0.1.1/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        8 2024-04-13 17:29:45.000000 efriser-0.1.1/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 17:29:45.435062 efriser-0.1.1/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      356 2024-04-13 17:26:41.000000 efriser-0.1.1/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.292012 efriser-0.1.2/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:44:23.292012 efriser-0.1.2/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      158 2024-04-13 17:29:42.000000 efriser-0.1.2/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.288011 efriser-0.1.2/efriser/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       54 2024-04-13 17:43:29.000000 efriser-0.1.2/efriser/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6221 2024-04-13 17:33:36.000000 efriser-0.1.2/efriser/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.2/efriser/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.2/efriser/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.2/efriser/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.2/efriser/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.292012 efriser-0.1.2/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      295 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        8 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 17:44:23.292012 efriser-0.1.2/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 17:43:52.000000 efriser-0.1.2/setup.py
```

### Comparing `efriser-0.1.1/efriser/invoicing.py` & `efriser-0.1.2/efriser/invoicing.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
         }
     
         message = "000f"
 
         return self.efris_post(ic, message)
 
 
-
-#invoicing = Efriser('198.74.52.28:9880', 'TCS1613912751699535','1000032574', 'WideSpectrum')
-#tax_payer = invoicing.query_invoice_details('323128406449')
+invoicing = Efriser('198.74.52.28:9880', 'TCS1613912751699535','1000032574', 'WideSpectrum')
+tax_payer = invoicing.query_invoice_details('323128406449')
 #tax_payer = invoicing.acquiring_exchange_rate("USD")
 
 
-#print('**********************************')
-#print(tax_payer)
+print('**********************************')
+print(tax_payer)
```

### Comparing `efriser-0.1.1/efriser/output_cleaner.py` & `efriser-0.1.2/efriser/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.1/efriser/services.py` & `efriser-0.1.2/efriser/services.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.1/efriser/utils.py` & `efriser-0.1.2/efriser/utils.py`

 * *Files identical despite different names*

