# Comparing `tmp/statmorph-0.5.5.tar.gz` & `tmp/statmorph-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statmorph-0.5.5.tar", last modified: Mon Feb 12 03:27:22 2024, max compression
+gzip compressed data, was "statmorph-0.5.6.tar", last modified: Sat Apr 13 00:24:10 2024, max compression
```

## Comparing `statmorph-0.5.5.tar` & `statmorph-0.5.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.405896 statmorph-0.5.5/
--rw-r--r--   0 vrg       (1000) users      (985)     1528 2024-02-12 03:04:55.000000 statmorph-0.5.5/LICENSE
--rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.5/MANIFEST.in
--rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-02-12 03:27:22.402563 statmorph-0.5.5/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.5/README.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/docs/
--rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/Makefile
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/docs/_static/
--rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/_static/banner.svg
--rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/_static/favicon.ico
--rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/_static/logo.png
--rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/api.rst
--rw-r--r--   0 vrg       (1000) users      (985)     2613 2024-02-12 03:04:42.000000 statmorph-0.5.5/docs/conf.py
--rw-r--r--   0 vrg       (1000) users      (985)     5009 2023-08-03 22:44:15.000000 statmorph-0.5.5/docs/description.rst
--rw-r--r--   0 vrg       (1000) users      (985)       88 2023-08-01 00:03:20.000000 statmorph-0.5.5/docs/examples.rst
--rw-r--r--   0 vrg       (1000) users      (985)     1424 2023-08-01 00:01:24.000000 statmorph-0.5.5/docs/index.rst
--rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/installation.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/docs/notebooks/
--rw-r--r--   0 vrg       (1000) users      (985)    16723 2024-02-12 03:13:47.000000 statmorph-0.5.5/docs/notebooks/doublesersic.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)    13531 2024-02-12 03:12:20.000000 statmorph-0.5.5/docs/notebooks/tutorial.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)     1904 2023-07-31 22:59:58.000000 statmorph-0.5.5/docs/overview.rst
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.5/docs/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.5/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       38 2024-02-12 03:27:22.405896 statmorph-0.5.5/setup.cfg
--rw-r--r--   0 vrg       (1000) users      (985)     1363 2024-02-12 03:03:55.000000 statmorph-0.5.5/setup.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph/
--rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.5/statmorph/__init__.py
--rw-r--r--   0 vrg       (1000) users      (985)   120811 2024-02-12 03:04:07.000000 statmorph-0.5.5/statmorph/statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph/tests/
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.5/statmorph/tests/__init__.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph/tests/data/
--rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.5/statmorph/tests/data/slice.fits
--rw-r--r--   0 vrg       (1000) users      (985)    15096 2023-11-14 15:53:08.000000 statmorph-0.5.5/statmorph/tests/test_statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph/utils/
--rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.5/statmorph/utils/__init__.py
--rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.5/statmorph/utils/image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph/utils/tests/
--rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.5/statmorph/utils/tests/test_image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-02-12 03:27:22.402563 statmorph-0.5.5/statmorph.egg-info/
--rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-02-12 03:27:22.000000 statmorph-0.5.5/statmorph.egg-info/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)      763 2024-02-12 03:27:22.000000 statmorph-0.5.5/statmorph.egg-info/SOURCES.txt
--rw-r--r--   0 vrg       (1000) users      (985)        1 2024-02-12 03:27:22.000000 statmorph-0.5.5/statmorph.egg-info/dependency_links.txt
--rw-r--r--   0 vrg       (1000) users      (985)      103 2024-02-12 03:27:22.000000 statmorph-0.5.5/statmorph.egg-info/requires.txt
--rw-r--r--   0 vrg       (1000) users      (985)       10 2024-02-12 03:27:22.000000 statmorph-0.5.5/statmorph.egg-info/top_level.txt
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/
+-rw-r--r--   0 vrg       (1000) users      (985)     1528 2024-02-12 03:04:55.000000 statmorph-0.5.6/LICENSE
+-rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.6/MANIFEST.in
+-rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-13 00:24:10.621439 statmorph-0.5.6/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.6/README.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.618105 statmorph-0.5.6/docs/
+-rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/Makefile
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/docs/_static/
+-rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/banner.svg
+-rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/favicon.ico
+-rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/logo.png
+-rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/api.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     2613 2024-04-12 23:54:40.000000 statmorph-0.5.6/docs/conf.py
+-rw-r--r--   0 vrg       (1000) users      (985)     5009 2023-08-03 22:44:15.000000 statmorph-0.5.6/docs/description.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       88 2023-08-01 00:03:20.000000 statmorph-0.5.6/docs/examples.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     1424 2023-08-01 00:01:24.000000 statmorph-0.5.6/docs/index.rst
+-rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/installation.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/docs/notebooks/
+-rw-r--r--   0 vrg       (1000) users      (985)    16723 2024-04-12 23:59:38.000000 statmorph-0.5.6/docs/notebooks/doublesersic.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)    13570 2024-04-12 23:58:51.000000 statmorph-0.5.6/docs/notebooks/tutorial.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)     1943 2024-04-13 00:02:01.000000 statmorph-0.5.6/docs/overview.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.6/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       38 2024-04-13 00:24:10.621439 statmorph-0.5.6/setup.cfg
+-rw-r--r--   0 vrg       (1000) users      (985)     1363 2024-04-12 23:53:31.000000 statmorph-0.5.6/setup.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/
+-rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/__init__.py
+-rw-r--r--   0 vrg       (1000) users      (985)   121807 2024-04-13 00:18:58.000000 statmorph-0.5.6/statmorph/statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/tests/__init__.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/tests/data/
+-rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/tests/data/slice.fits
+-rw-r--r--   0 vrg       (1000) users      (985)    15145 2024-04-12 23:24:50.000000 statmorph-0.5.6/statmorph/tests/test_statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/utils/
+-rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/utils/__init__.py
+-rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.6/statmorph/utils/image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/utils/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/utils/tests/test_image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph.egg-info/
+-rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)      763 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/SOURCES.txt
+-rw-r--r--   0 vrg       (1000) users      (985)        1 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/dependency_links.txt
+-rw-r--r--   0 vrg       (1000) users      (985)      103 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/requires.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       10 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/top_level.txt
```

### Comparing `statmorph-0.5.5/LICENSE` & `statmorph-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/PKG-INFO` & `statmorph-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.5
+Version: 0.5.6
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.5/README.rst` & `statmorph-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/Makefile` & `statmorph-0.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/_static/banner.svg` & `statmorph-0.5.6/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/_static/favicon.ico` & `statmorph-0.5.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/_static/logo.png` & `statmorph-0.5.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/conf.py` & `statmorph-0.5.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'statmorph'
 copyright = '2017-2024, Vicente Rodriguez-Gomez'
 author = 'Vicente Rodriguez-Gomez'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.5'
+release = '0.5.6'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `statmorph-0.5.5/docs/description.rst` & `statmorph-0.5.6/docs/description.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/index.rst` & `statmorph-0.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/installation.rst` & `statmorph-0.5.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/notebooks/doublesersic.ipynb` & `statmorph-0.5.6/docs/notebooks/doublesersic.ipynb`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/docs/notebooks/tutorial.ipynb` & `statmorph-0.5.6/docs/notebooks/tutorial.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998664529914529%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(2, 'Other morphological measurements that are more general "*

 * *            'and robust to noise, which are also calculated by statmorph, include the Gini-M20 '*

 * *            '(Lotz et al. 2004), CAS (Conselice 2003) and MID (Freeman et al. 2013) statistics, as '*

 * *            'well as the RMS asymmetry (Sazonova et al. 2024), outer asymmetry (Wen et al. 2014), '*

 * *            "and shape asymmetry (Pawlik et al. 2016).\\n')], delete: [2]}}}"}*

```diff
@@ -283,15 +283,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that the fitted Sersic model is in very good agreement with the \"true\" Sersic model that we originally defined (n = 2.5, rhalf = 20, etc.) and that the reduced chi-squared statistic (sersic_chi2_dof) is close to 1, indicating a good fit without overfitting. However, such good agreement tends to deteriorate somewhat at higher noise levels, and one has to keep in mind that not all galaxies are well described by Sersic profiles.\n",
                 "\n",
-                "Other morphological measurements that are more general and robust to noise, which are also calculated by statmorph, include the Gini-M20 (Lotz et al. 2004), CAS (Conselice 2003) and MID (Freeman et al. 2013) statistics, as well as the outer asymmetry (Wen et al. 2014) and shape asymmetry (Pawlik et al. 2016).\n",
+                "Other morphological measurements that are more general and robust to noise, which are also calculated by statmorph, include the Gini-M20 (Lotz et al. 2004), CAS (Conselice 2003) and MID (Freeman et al. 2013) statistics, as well as the RMS asymmetry (Sazonova et al. 2024), outer asymmetry (Wen et al. 2014), and shape asymmetry (Pawlik et al. 2016).\n",
                 "\n",
                 "Also note that statmorph returns two quality flags:\n",
                 "\n",
                 "1. ``flag`` : indicates the quality of the basic morphological measurements, taking one of the following values: 0 (good), 1 (suspect), 2 (bad), or 4 (catastrophic). More details can be found [here](../description.html#output).\n",
                 "\n",
                 "2. ``flag_sersic`` : indicates the quality of the Sersic fit, also taking values of 0 (good), 1 (suspect), 2 (bad), or 4 (catastrophic).\n",
                 "\n",
```

### Comparing `statmorph-0.5.5/docs/overview.rst` & `statmorph-0.5.6/docs/overview.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 morphological statistics for each source:
 
 - Gini-M20 statistics (Lotz et al. 2004; Snyder et al. 2015a,b)
 - Concentration, Asymmetry and Smoothness (CAS) statistics
   (Bershady et al. 2000; Conselice 2003; Lotz et al. 2004)
 - Multimode, Intensity and Deviation (MID) statistics (Freeman et al. 2013;
   Peth et al. 2016)
-- Outer asymmetry and shape asymmetry (Wen et al. 2014; Pawlik et al. 2016)
+- RMS asymmetry (Sazonova et al. 2024), outer asymmetry (Wen et al. 2014) and shape asymmetry (Pawlik et al. 2016)
 - Single and double Sérsic indices (Sérsic 1968)
 - Several shape and size measurements associated to the above statistics
   (ellipticity, Petrosian radius, half-light radius, etc.)
 
 .. ~ For more information, please see:
 
 .. ~ - `Rodriguez-Gomez et al. (2019) <https://ui.adsabs.harvard.edu/abs/2019MNRAS.483.4140R>`_
```

### Comparing `statmorph-0.5.5/setup.py` & `statmorph-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='statmorph',
-    version='0.5.5',
+    version='0.5.6',
     description='Non-parametric morphological diagnostics of galaxy images',
     long_description=long_description,
     url='https://github.com/vrodgom/statmorph',
     author='Vicente Rodriguez-Gomez',
     author_email='vrodgom.astro@gmail.com',
     license='BSD',
     classifiers=[
```

### Comparing `statmorph-0.5.5/statmorph/statmorph.py` & `statmorph-0.5.6/statmorph/statmorph.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'DoubleSersic2D',
     'ConvolvedDoubleSersic2D',
     'SourceMorphology',
     'source_morphology',
     '__version__',
 ]
 
-__version__ = '0.5.5'
+__version__ = '0.5.6'
 
 # A list of the quantities calculated by SourceMorphology,
 # excluding the double Sersic parameters:
 _quantity_names = [
     'xc_centroid',
     'yc_centroid',
     'ellipticity_centroid',
@@ -65,14 +65,15 @@
     'sn_per_pixel',
     'concentration',
     'asymmetry',
     'smoothness',
     'multimode',
     'intensity',
     'deviation',
+    'rms_asymmetry',
     'outer_asymmetry',
     'shape_asymmetry',
     'sersic_amplitude',
     'sersic_rhalf',
     'sersic_n',
     'sersic_xc',
     'sersic_yc',
@@ -1650,17 +1651,17 @@
 
         Parameters
         ----------
         center : tuple or array-like
             The (x,y) position of the center.
         image : array-like
             The 2D image.
-        kind : {'cas', 'outer', 'shape'}
+        kind : {'cas', 'rms', 'outer', 'shape'}
             Whether to calculate the traditional CAS asymmetry (default),
-            outer asymmetry or shape asymmetry.
+            RMS asymmetry, outer asymmetry, or shape asymmetry.
 
         Returns
         -------
         asym : The asymmetry statistic for the given center.
 
         """
         image = np.float64(image)  # skimage wants double
@@ -1682,15 +1683,15 @@
         mask_180 = skimage.transform.rotate(mask, 180.0, center=center)
         mask_180 = mask_180 >= 0.5  # convert back to bool
         mask_symmetric = mask | mask_180
         image = np.where(~mask_symmetric, image, 0.0)
         image_180 = np.where(~mask_symmetric, image_180, 0.0)
 
         # Create aperture for the chosen kind of asymmetry
-        if kind == 'cas':
+        if kind == 'cas' or kind == 'rms':
             r = self._petro_extent_cas * self._rpetro_circ_centroid
             ap = photutils.aperture.CircularAperture(center, r)
         elif kind == 'outer':
             a_in = self.rhalf_ellip
             a_out = self.rmax_ellip
             b_out = a_out / self.elongation_asymmetry
             theta = self.orientation_asymmetry
@@ -1702,33 +1703,44 @@
                               AstropyUserWarning)
                 self.flag = 2
                 return -99.0  # invalid
             ap = photutils.aperture.CircularAperture(center, self.rmax_circ)
         else:
             raise NotImplementedError('Asymmetry kind not understood:', kind)
 
+        # Aperture area (in pixels)
+        ap_area = _aperture_area(ap, mask_symmetric)
+
         # Apply eq. 10 from Lotz et al. (2004)
         ap_abs_sum = ap.do_photometry(np.abs(image), method='exact')[0][0]
         ap_abs_diff = ap.do_photometry(np.abs(image_180-image), method='exact')[0][0]
 
         if ap_abs_sum == 0.0:
             warnings.warn('[asymmetry_function] Zero flux sum.',
                           AstropyUserWarning)
             self.flag = 1
             # Return large value to get minimizer out of masked region:
             return 100.0
 
         if kind == 'shape':
             # The shape asymmetry of the background is zero
             asym = ap_abs_diff / ap_abs_sum
+        elif kind == 'rms':
+            # Apply eq. 27 from Sazonova et al. (2024)
+            ap_sqr_sum = ap.do_photometry(image**2, method='exact')[0][0]
+            ap_sqr_diff = ap.do_photometry((image_180-image)**2, method='exact')[0][0]
+            if self.sky_sigma == -99.0:  # invalid skybox
+                asym = ap_sqr_diff / ap_sqr_sum
+            else:
+                asym = (ap_sqr_diff - 2*ap_area*self.sky_sigma**2) / (
+                        ap_sqr_sum - ap_area*self.sky_sigma**2)
         else:
             if self._sky_asymmetry == -99.0:  # invalid skybox
                 asym = ap_abs_diff / ap_abs_sum
             else:
-                ap_area = _aperture_area(ap, mask_symmetric)
                 asym = (ap_abs_diff - ap_area*self._sky_asymmetry) / ap_abs_sum
 
         return asym
 
     @lazyproperty
     def _asymmetry_center(self):
         """
@@ -1838,14 +1850,26 @@
         """
         image = self._cutout_stamp_maskzeroed
         asym = self._asymmetry_function(self._asymmetry_center,
                                         image, 'cas')
 
         return asym
 
+    @lazyproperty
+    def rms_asymmetry(self):
+        """
+        Calculate the RMS asymmetry as in eq. 27 of Sazonova et al. (2024).
+        Note that this actually corresponds to the *square* of A_rms.
+        """
+        image = self._cutout_stamp_maskzeroed
+        asym = self._asymmetry_function(self._asymmetry_center,
+                                        image, 'rms')
+
+        return asym
+
     def _radius_at_fraction_of_total_cas(self, fraction):
         """
         Specialization of ``_radius_at_fraction_of_total_circ`` for
         the CAS calculations.
         """
         image = self._cutout_stamp_maskzeroed
         center = self._asymmetry_center
```

### Comparing `statmorph-0.5.5/statmorph/tests/data/slice.fits` & `statmorph-0.5.6/statmorph/tests/data/slice.fits`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/statmorph/tests/test_statmorph.py` & `statmorph-0.5.6/statmorph/tests/test_statmorph.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,15 @@
             'sn_per_pixel': 6.80319166183472,
             'concentration': 2.19100140632153,
             'asymmetry': 0.00377345808887,
             'smoothness': 0.00430880839402,
             'multimode': 0.23423423423423,
             'intensity': 0.51203949030140,
             'deviation': 0.01522525597953,
+            'rms_asymmetry': 0.0053900924481633,
             'outer_asymmetry': -0.01821399684443,
             'shape_asymmetry': 0.16308278287864,
             'sersic_amplitude': 1296.95288208155739,
             'sersic_rhalf': 22.45788866502031,
             'sersic_n': 0.61206828194077,
             'sersic_xc': 81.56197595338546,
             'sersic_yc': 80.40465135599014,
```

### Comparing `statmorph-0.5.5/statmorph/utils/image_diagnostics.py` & `statmorph-0.5.6/statmorph/utils/image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/statmorph/utils/tests/test_image_diagnostics.py` & `statmorph-0.5.6/statmorph/utils/tests/test_image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.5/statmorph.egg-info/PKG-INFO` & `statmorph-0.5.6/statmorph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.5
+Version: 0.5.6
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.5/statmorph.egg-info/SOURCES.txt` & `statmorph-0.5.6/statmorph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

