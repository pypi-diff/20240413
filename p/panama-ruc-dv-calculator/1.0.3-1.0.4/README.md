# Comparing `tmp/panama-ruc-dv-calculator-1.0.3.tar.gz` & `tmp/panama-ruc-dv-calculator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panama-ruc-dv-calculator-1.0.3.tar", last modified: Fri Jan 26 15:42:51 2024, max compression
+gzip compressed data, was "panama-ruc-dv-calculator-1.0.4.tar", last modified: Fri Apr 12 22:18:19 2024, max compression
```

## Comparing `panama-ruc-dv-calculator-1.0.3.tar` & `panama-ruc-dv-calculator-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 15:42:51.663404 panama-ruc-dv-calculator-1.0.3/
--rw-rw-rw-   0        0        0      271 2024-01-26 15:42:29.000000 panama-ruc-dv-calculator-1.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1092 2024-01-20 21:57:33.000000 panama-ruc-dv-calculator-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      525 2024-01-23 19:30:23.000000 panama-ruc-dv-calculator-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3916 2024-01-26 15:42:51.662351 panama-ruc-dv-calculator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3471 2024-01-23 19:53:42.000000 panama-ruc-dv-calculator-1.0.3/README.md
--rw-rw-rw-   0        0        0     3529 2024-01-23 19:53:42.000000 panama-ruc-dv-calculator-1.0.3/README_ES.md
-drwxrwxrwx   0        0        0        0 2024-01-26 15:42:51.660246 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/
--rw-rw-rw-   0        0        0        0 2024-01-20 19:39:03.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/__init__.py
--rw-rw-rw-   0        0        0      298 2024-01-19 21:29:39.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/calculate_dv_digit.py
--rw-rw-rw-   0        0        0      961 2024-01-19 17:16:09.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/provincia.py
--rw-rw-rw-   0        0        0     1370 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_finca.py
--rw-rw-rw-   0        0        0     2839 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_juridica.py
--rw-rw-rw-   0        0        0     1922 2024-01-26 15:40:22.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_juridica_nt.py
--rw-rw-rw-   0        0        0     5597 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_natural.py
--rw-rw-rw-   0        0        0     1951 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_natural_nt.py
-drwxrwxrwx   0        0        0        0 2024-01-26 15:42:51.661248 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator.egg-info/
--rw-rw-rw-   0        0        0      409 2024-01-26 15:42:51.000000 panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      834 2024-01-22 23:15:43.000000 panama-ruc-dv-calculator-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-26 15:42:51.664404 panama-ruc-dv-calculator-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      798 2024-01-26 15:42:29.000000 panama-ruc-dv-calculator-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:18:19.543949 panama-ruc-dv-calculator-1.0.4/
+-rw-rw-rw-   0        0        0      364 2024-04-12 22:15:24.000000 panama-ruc-dv-calculator-1.0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1092 2024-01-20 21:57:33.000000 panama-ruc-dv-calculator-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      525 2024-01-23 19:30:23.000000 panama-ruc-dv-calculator-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3916 2024-04-12 22:18:19.542941 panama-ruc-dv-calculator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3471 2024-01-23 19:53:42.000000 panama-ruc-dv-calculator-1.0.4/README.md
+-rw-rw-rw-   0        0        0     3529 2024-01-23 19:53:42.000000 panama-ruc-dv-calculator-1.0.4/README_ES.md
+drwxrwxrwx   0        0        0        0 2024-04-12 22:18:19.541359 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/
+-rw-rw-rw-   0        0        0        0 2024-01-20 19:39:03.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/__init__.py
+-rw-rw-rw-   0        0        0      298 2024-01-19 21:29:39.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/calculate_dv_digit.py
+-rw-rw-rw-   0        0        0      961 2024-01-19 17:16:09.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/provincia.py
+-rw-rw-rw-   0        0        0     1370 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_finca.py
+-rw-rw-rw-   0        0        0     2839 2024-04-12 22:11:58.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_juridica.py
+-rw-rw-rw-   0        0        0     1922 2024-01-26 15:40:22.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_juridica_nt.py
+-rw-rw-rw-   0        0        0     5597 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_natural.py
+-rw-rw-rw-   0        0        0     1951 2024-01-23 19:42:37.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_natural_nt.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:18:19.542359 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-04-12 22:18:19.000000 panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      834 2024-01-22 23:15:43.000000 panama-ruc-dv-calculator-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 22:18:19.543949 panama-ruc-dv-calculator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      798 2024-04-12 22:15:25.000000 panama-ruc-dv-calculator-1.0.4/setup.py
```

### Comparing `panama-ruc-dv-calculator-1.0.3/LICENSE` & `panama-ruc-dv-calculator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/MANIFEST.in` & `panama-ruc-dv-calculator-1.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/PKG-INFO` & `panama-ruc-dv-calculator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panama-ruc-dv-calculator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A DV calculator for Panama RUC
 Home-page: https://github.com/juancorradine/panama-ruc-dv-calculator
 Author: Juan Corradine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `panama-ruc-dv-calculator-1.0.3/README.md` & `panama-ruc-dv-calculator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/README_ES.md` & `panama-ruc-dv-calculator-1.0.4/README_ES.md`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/provincia.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/provincia.py`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_finca.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_finca.py`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_juridica.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_juridica.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if len(ruc_parts) != 3:
             raise ValueError("Formato de RUC Juridica incorrecto.")
 
         rollo_tomo = ruc_parts[0]
         folio_imagen = ruc_parts[1]
         asiento_ficha = ruc_parts[2]
 
-        if not rollo_tomo.isnumeric() or len(rollo_tomo) > 8:
+        if not rollo_tomo.isnumeric() or len(rollo_tomo) > 9:
             raise ValueError("Formato de RUC Juridica incorrecto - Rollo/Tomo: " + rollo_tomo)
         if not folio_imagen.isnumeric() or len(folio_imagen) > 4:
             raise ValueError("Formato de RUC Juridica incorrecto - Folio/Imagen: " + folio_imagen)
         if not asiento_ficha.isnumeric() or len(asiento_ficha) > 6:
             raise ValueError("Formato de RUC Juridica incorrecto - Asiento/Ficha: " + asiento_ficha)
 
         self.ruc = ruc
```

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_juridica_nt.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_juridica_nt.py`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_natural.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_natural.py`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/panama_ruc_dv_calculator/ruc_natural_nt.py` & `panama-ruc-dv-calculator-1.0.4/panama_ruc_dv_calculator/ruc_natural_nt.py`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/requirements.txt` & `panama-ruc-dv-calculator-1.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `panama-ruc-dv-calculator-1.0.3/setup.py` & `panama-ruc-dv-calculator-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="panama-ruc-dv-calculator",
-    version="1.0.3",
+    version="1.0.4",
     author="Juan Corradine",
     description="A DV calculator for Panama RUC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/juancorradine/panama-ruc-dv-calculator",
     packages=find_packages(),
     classifiers=[
```

