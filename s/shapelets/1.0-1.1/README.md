# Comparing `tmp/shapelets-1.0.tar.gz` & `tmp/shapelets-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-1.0.tar", last modified: Mon Apr  1 12:27:47 2024, max compression
+gzip compressed data, was "shapelets-1.1.tar", last modified: Fri Apr 12 22:53:31 2024, max compression
```

## Comparing `shapelets-1.0.tar` & `shapelets-1.1.tar`

### file list

```diff
@@ -1,41 +1,51 @@
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-03-19 17:11:15.000000 shapelets-1.0/AUTHORS.md
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    26526 2023-03-12 20:57:22.000000 shapelets-1.0/LICENSE
--rw-r--r--   0 nasser    (1000) nasser    (1000)    31817 2024-04-01 12:27:47.682821 shapelets-1.0/PKG-INFO
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     4281 2024-03-19 17:12:44.000000 shapelets-1.0/README.md
--rw-rw-r--   0 nasser    (1000) nasser    (1000)       90 2023-03-12 20:58:29.000000 shapelets-1.0/pyproject.toml
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     1163 2024-04-01 12:27:47.682821 shapelets-1.0/setup.cfg
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     6731 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/__init__.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     4345 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/_entry_points.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     7512 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/_run.py
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/astronomy/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     1981 2023-11-15 23:55:24.000000 shapelets-1.0/shapelets/astronomy/__init__.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    12668 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/astronomy/galaxy.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    11847 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/astronomy/misc.py
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.678821 shapelets-1.0/shapelets/discrete_transform/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     1768 2023-03-12 21:05:17.000000 shapelets-1.0/shapelets/discrete_transform/__init__.py
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets/docs/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     4184 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/WSL_support.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     2162 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/__init__.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     2816 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/custom_commands.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     7234 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_1.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     7003 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_2.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     6543 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_3.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     7211 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/example_4.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     4547 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/installation_guide.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     2764 2024-04-01 12:11:51.000000 shapelets-1.0/shapelets/docs/package_interface.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    13422 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/functions.py
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets/self_assembly/
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     2004 2023-11-15 23:55:24.000000 shapelets-1.0/shapelets/self_assembly/__init__.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    14659 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/misc.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)    22223 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/quant.py
--rw-rw-r--   0 nasser    (1000) nasser    (1000)     7638 2024-03-19 17:11:15.000000 shapelets-1.0/shapelets/self_assembly/wavelength.py
-drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-01 12:27:47.682821 shapelets-1.0/shapelets.egg-info/
--rw-r--r--   0 nasser    (1000) nasser    (1000)    31817 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/PKG-INFO
--rw-rw-r--   0 nasser    (1000) nasser    (1000)      921 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/SOURCES.txt
--rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/dependency_links.txt
--rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/entry_points.txt
--rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-01-09 18:39:05.000000 shapelets-1.0/shapelets.egg-info/not-zip-safe
--rw-rw-r--   0 nasser    (1000) nasser    (1000)       97 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/requires.txt
--rw-rw-r--   0 nasser    (1000) nasser    (1000)       10 2024-04-01 12:27:47.000000 shapelets-1.0/shapelets.egg-info/top_level.txt
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.831808 shapelets-1.1/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-03-19 17:11:15.000000 shapelets-1.1/AUTHORS.md
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    26526 2023-03-12 20:57:22.000000 shapelets-1.1/LICENSE
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      130 2024-04-12 22:51:33.000000 shapelets-1.1/MANIFEST.in
+-rw-r--r--   0 nasser    (1000) nasser    (1000)    32110 2024-04-12 22:53:31.831808 shapelets-1.1/PKG-INFO
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4574 2024-04-12 22:51:33.000000 shapelets-1.1/README.md
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       90 2023-03-12 20:58:29.000000 shapelets-1.1/pyproject.toml
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1162 2024-04-12 22:53:31.831808 shapelets-1.1/setup.cfg
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.823808 shapelets-1.1/shapelets/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6875 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     3698 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/_entry_points.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7145 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/_run.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.823808 shapelets-1.1/shapelets/astronomy/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1981 2023-11-15 23:55:24.000000 shapelets-1.1/shapelets/astronomy/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    12668 2024-03-19 17:11:15.000000 shapelets-1.1/shapelets/astronomy/galaxy.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    11847 2024-03-19 17:11:15.000000 shapelets-1.1/shapelets/astronomy/misc.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.823808 shapelets-1.1/shapelets/discrete_transform/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1768 2023-03-12 21:05:17.000000 shapelets-1.1/shapelets/discrete_transform/__init__.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.827808 shapelets-1.1/shapelets/docs/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2134 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     3045 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/custom_commands.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7195 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/example_1.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6510 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/example_2.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6450 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/example_3.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7331 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/example_4.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     3785 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/installation_guide.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2771 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/docs/package_interface.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    13422 2024-03-19 17:11:15.000000 shapelets-1.1/shapelets/functions.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.827808 shapelets-1.1/shapelets/self_assembly/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2004 2023-11-15 23:55:24.000000 shapelets-1.1/shapelets/self_assembly/__init__.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    15601 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/self_assembly/misc.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    21265 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/self_assembly/quant.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     7638 2024-03-19 17:11:15.000000 shapelets-1.1/shapelets/self_assembly/wavelength.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.831808 shapelets-1.1/shapelets/tests/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     2043 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/__init__.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.831808 shapelets-1.1/shapelets/tests/images/
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)  1082880 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/images/galaxies.fits
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)   355074 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/images/hexSIM1.png
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)    70681 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/images/lamSIM1.png
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6367 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/test_astronomy_basic.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     4358 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/test_self_assembly_basic.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6712 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/test_self_assembly_methods.py
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     6427 2024-04-12 22:51:33.000000 shapelets-1.1/shapelets/tests/test_shapelet_functions.py
+drwxrwxr-x   0 nasser    (1000) nasser    (1000)        0 2024-04-12 22:53:31.831808 shapelets-1.1/shapelets.egg-info/
+-rw-r--r--   0 nasser    (1000) nasser    (1000)    32110 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/PKG-INFO
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)     1211 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/SOURCES.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/dependency_links.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)      121 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/entry_points.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)        1 2024-01-09 18:39:05.000000 shapelets-1.1/shapelets.egg-info/not-zip-safe
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       97 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/requires.txt
+-rw-rw-r--   0 nasser    (1000) nasser    (1000)       10 2024-04-12 22:53:31.000000 shapelets-1.1/shapelets.egg-info/top_level.txt
```

### Comparing `shapelets-1.0/LICENSE` & `shapelets-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/PKG-INFO` & `shapelets-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets
-Version: 1.0
+Version: 1.1
 Summary: Shapelets is a module providing both reference access to various shapelet functions and some significant applications of them in science and astronomy.
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
 Keywords: shapelets,image analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -27,47 +27,51 @@
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
 
 ## What is shapelets? 
 
-shapelets is a python package that implements several shapelet functions and some of their significant applications in science and astronomy. These functions form a complete and orthonormal set, allowing them to capture complex geometries and information from any physical shape. Furthermore, shapelets are localized and can be scaled to match that of any physical feature. 
+Shapelets is a Python package that implements several shapelet functions and some of their significant applications in science and astronomy. Shapelet functions are a complete and orthogonal set of localized basis functions with mathematical properties convenient for manipulation and analysis of images from a broad range of applications.
 
-Due to these properties, they have seen extensive use in recent years, with several different formulations and applications:
+Due to these properties, they have seen extensive use in recent years, including:
 
 * Astronomy/astrophysics ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x), [R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445), [J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
-* Nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
+* Self-assembled nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
 * Computational neuroscience ([J. D. Victor (2006)](https://doi.org/10.1152/jn.00498.2005), [T. O. Sharpee (2009)](https://doi.org/10.1007%2Fs10827-008-0107-5))
 * Medical imaging ([J. Weissman (2004)](https://doi.org/10.1364/OPEX.12.005760))
 
-The shapelets package provides reference documentation and code for four (4) shapelet functions: 
+The shapelets package provides reference code and documentation for 4 shapelet function definitions: 
 
 * Cartesian shapelets ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x)), 
 * Polar shapelets ([R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445)),
 * Orthonormal polar shapelets with constant radial scale ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353)), and 
 * Exponential shapelets ([J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
 
 ## Getting Started
 
-Users are directed to the shapelets [official website](https://uw-comphys.github.io/shapelets/shapelets.html) for all documentation, including installation instructions, detailed examples, and more. 
-If you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below or the "Cite this repository" dropdown on the right sidebar.
+If you have Python 3.10+ installed on your machine, you can install the shapelets package in the terminal via pip: `pip install shapelets`
+
+If you do not have Python 3.10+ installed on your machine, consult the [installation guide](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html). 
+
+New users are also encouraged to visit the [official website](https://uw-comphys.github.io/shapelets/shapelets.html) to understand how the shapelets package can be used along with detailed examples, custom terminal commands provided by the package, and more. 
+Additionally, if you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below.
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with shapelets, please create a post using our package [issue tracker](https://github.com/uw-comphys/shapelets/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
 
 ## Contribute
 
 The authors of the shapelets package welcome external contributions to the source code. This process will be easiest if users adhere to the contribution policy:
 
 * Open an issue on the package [issue tracker](https://github.com/uw-comphys/shapelets/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the shapelets package, specifically detailed documentation for new methods (see existing methods for example documentation)
-* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the custom command: `shapelets-test`
-* Once the issue has been discussed with a package author, you may open a pull request containing your modifications
+* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the entry point: `shapelets-test`
+* Once the issue has been discussed with a package author, you may open a pull request containing your code modifications
 
 ## Citation
 
 If you plan to use shapelets in your own work, please cite using the following Bibtex citation:
 
 ```
 @article{TinoShapelets2024,
@@ -81,15 +85,15 @@
 year = {2024},
 url = {https://joss.theoj.org/papers/10.21105/joss.06058}
 }
 ```
 
 ## Authors
 
-* Matthew Peres Tino
+* Matthew Peres Tino (mptino@uwaterloo.ca)
 * Abbas Yusuf Abdulaziz 
 * Nasser Mohieddin Abukhdeir
 * Robert Suderman 
 * Thomas Akdeniz
 
                   GNU LESSER GENERAL PUBLIC LICENSE
                        Version 2.1, February 1999
```

### Comparing `shapelets-1.0/README.md` & `shapelets-1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,47 +6,51 @@
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
 
 ## What is shapelets? 
 
-shapelets is a python package that implements several shapelet functions and some of their significant applications in science and astronomy. These functions form a complete and orthonormal set, allowing them to capture complex geometries and information from any physical shape. Furthermore, shapelets are localized and can be scaled to match that of any physical feature. 
+Shapelets is a Python package that implements several shapelet functions and some of their significant applications in science and astronomy. Shapelet functions are a complete and orthogonal set of localized basis functions with mathematical properties convenient for manipulation and analysis of images from a broad range of applications.
 
-Due to these properties, they have seen extensive use in recent years, with several different formulations and applications:
+Due to these properties, they have seen extensive use in recent years, including:
 
 * Astronomy/astrophysics ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x), [R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445), [J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
-* Nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
+* Self-assembled nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
 * Computational neuroscience ([J. D. Victor (2006)](https://doi.org/10.1152/jn.00498.2005), [T. O. Sharpee (2009)](https://doi.org/10.1007%2Fs10827-008-0107-5))
 * Medical imaging ([J. Weissman (2004)](https://doi.org/10.1364/OPEX.12.005760))
 
-The shapelets package provides reference documentation and code for four (4) shapelet functions: 
+The shapelets package provides reference code and documentation for 4 shapelet function definitions: 
 
 * Cartesian shapelets ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x)), 
 * Polar shapelets ([R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445)),
 * Orthonormal polar shapelets with constant radial scale ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353)), and 
 * Exponential shapelets ([J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
 
 ## Getting Started
 
-Users are directed to the shapelets [official website](https://uw-comphys.github.io/shapelets/shapelets.html) for all documentation, including installation instructions, detailed examples, and more. 
-If you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below or the "Cite this repository" dropdown on the right sidebar.
+If you have Python 3.10+ installed on your machine, you can install the shapelets package in the terminal via pip: `pip install shapelets`
+
+If you do not have Python 3.10+ installed on your machine, consult the [installation guide](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html). 
+
+New users are also encouraged to visit the [official website](https://uw-comphys.github.io/shapelets/shapelets.html) to understand how the shapelets package can be used along with detailed examples, custom terminal commands provided by the package, and more. 
+Additionally, if you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below.
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with shapelets, please create a post using our package [issue tracker](https://github.com/uw-comphys/shapelets/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
 
 ## Contribute
 
 The authors of the shapelets package welcome external contributions to the source code. This process will be easiest if users adhere to the contribution policy:
 
 * Open an issue on the package [issue tracker](https://github.com/uw-comphys/shapelets/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the shapelets package, specifically detailed documentation for new methods (see existing methods for example documentation)
-* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the custom command: `shapelets-test`
-* Once the issue has been discussed with a package author, you may open a pull request containing your modifications
+* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the entry point: `shapelets-test`
+* Once the issue has been discussed with a package author, you may open a pull request containing your code modifications
 
 ## Citation
 
 If you plan to use shapelets in your own work, please cite using the following Bibtex citation:
 
 ```
 @article{TinoShapelets2024,
@@ -60,12 +64,12 @@
 year = {2024},
 url = {https://joss.theoj.org/papers/10.21105/joss.06058}
 }
 ```
 
 ## Authors
 
-* Matthew Peres Tino
+* Matthew Peres Tino (mptino@uwaterloo.ca)
 * Abbas Yusuf Abdulaziz 
 * Nasser Mohieddin Abukhdeir
 * Robert Suderman 
 * Thomas Akdeniz
```

### Comparing `shapelets-1.0/setup.cfg` & `shapelets-1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = shapelets
-version = 1.0
+version = 1.1
 description = Shapelets is a module providing both reference access to various shapelet functions and some significant applications of them in science and astronomy.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 keywords = shapelets, image analysis
 license = GNU Lesser General Public License v2 or later (LGPLv2+)
 classifiers = 
 	Topic :: Scientific/Engineering :: Physics
 	License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 zip_safe = False
-include_package_data = False
+include_package_data = True
 packages = find:
 install_requires = 
 	numpy;python_version>'3.10.0'
 	scipy;python_version>'3.10.0'
 	matplotlib;python_version>'3.10.0'
 	opencv-python;python_version>'3.10.0'
 	configparser;python_version>'3.10.0'
```

### Comparing `shapelets-1.0/shapelets/__init__.py` & `shapelets-1.1/shapelets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,37 +19,38 @@
 
 # shapelets
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.06058/status.svg)](https://doi.org/10.21105/joss.06058)
 
 ## What is shapelets? 
 
-shapelets is a python package that implements several shapelet functions and some of their significant applications in science and astronomy. These functions form a complete and orthonormal set, allowing them to capture complex geometries and information from any physical shape. Furthermore, shapelets are localized and can be scaled to match that of any physical feature. 
+Shapelets is a Python package that implements several shapelet functions and some of their significant applications in science and astronomy. Shapelet functions are a complete and orthogonal set of localized basis functions with mathematical properties convenient for manipulation and analysis of images from a broad range of applications.
 
-Due to these properties, they have seen extensive use in recent years, with several different formulations and applications:
+Due to these properties, they have seen extensive use in recent years, including:
 
 * Astronomy/astrophysics ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x), [R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445), [J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
-* Nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
+* Self-assembled nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
 * Computational neuroscience ([J. D. Victor (2006)](https://doi.org/10.1152/jn.00498.2005), [T. O. Sharpee (2009)](https://doi.org/10.1007%2Fs10827-008-0107-5))
 * Medical imaging ([J. Weissman (2004)](https://doi.org/10.1364/OPEX.12.005760))
 
-The shapelets package provides reference documentation and code for four (4) shapelet functions: 
+The shapelets package provides reference code and documentation for 4 shapelet function definitions: 
 
 * Cartesian shapelets ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x)), 
 * Polar shapelets ([R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445)),
 * Orthonormal polar shapelets with constant radial scale ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353)), and 
 * Exponential shapelets ([J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
 
 ## Getting Started
 
 New users should kindly follow these instructions to use the shapelets package:
 
-1. Consult the [installation guide](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for installation instructions on Linux, Mac OS, and Windows machines.
+1. If you have Python 3.10+ installed, you can install the shapelets package via pip from your terminal/command line: `pip install shapelets` 
+2. If you do not have Python 3.10+ installed, consult the [installation guide](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for helpful instructions on Linux, Mac OS, and Windows machines.
 3. Consult the [examples](https://uw-comphys.github.io/shapelets/shapelets/docs.html) to see specific applications implemented in the package and a walkthrough of how to interact with the package correctly.
-2. Checkout other documentation, such as
+4. Checkout other documentation, such as
     * [Custom Commands](https://uw-comphys.github.io/shapelets/shapelets/docs/custom_commands.html) - describes command-line arguments specifically designed for this package
     * [Package Interface](https://uw-comphys.github.io/shapelets/shapelets/docs/package_interface.html) - describes two different ways of using the `shapelets` package (configuration files or traditional Python programming)
 
 If you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below.
 
 ## Issues
 
@@ -80,14 +81,14 @@
 year = {2024},
 url = {https://joss.theoj.org/papers/10.21105/joss.06058}
 }
 ```
 
 ## Authors
 
-* Matthew Peres Tino
+* Matthew Peres Tino (mptino@uwaterloo.ca)
 * Abbas Yusuf Abdulaziz 
 * Nasser Mohieddin Abukhdeir
 * Robert Suderman 
 * Thomas Akdeniz
 
 """
```

### Comparing `shapelets-1.0/shapelets/_entry_points.py` & `shapelets-1.1/shapelets/_entry_points.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,70 +11,54 @@
 # warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more  #
 # details.                                                                                                             #
 #                                                                                                                      #
 # You should have received a copy of the GNU Lesser General Public License along with shapelets. If not, see           #
 # <https://www.gnu.org/licenses/>.                                                                                     #
 ########################################################################################################################
 
-import contextlib
 import os
+from pathlib import Path
 import platform
 import sys 
+import time
 
 from . import _run
 
 def _run_shapelets():
     r"""
-    Main function that runs shapelets. This is only invoked via the entry point "shapelets CONFIG" where CONFIG is the name of the configuration plaintext file.      
+    Main function that runs shapelets. This is only invoked via the entry point "shapelets CONFIG" where CONFIG is the name of the configuration plaintext file that exists in the same directory level as the working directory.  
 
     """
-    # Arguments for command line use
-
-    if len(sys.argv) == 1: # if user did not provide any configuration path (which is required)
+    # if user did not provide any configuration filename (which is required)
+    if len(sys.argv) == 1: 
         raise RuntimeError('Please provide name of config file, i.e. "shapelets config".')
 
-    elif len(sys.argv) == 2: # if user did provide a configuration filename/path
+     # if user did provide a configuration filename/path
+    elif len(sys.argv) == 2:
         config_file = sys.argv[1]
-        _run._run(config_file)
+        working_dir = os.getcwd() 
+        _run._run(config_file, working_dir)
+
+    # if the user provides more than 1 argument (in addition to shapelets). Print error messages and quit.
+    else: 
+        raise RuntimeError('Please provide one argument (configuration filename), i.e.: "shapelets config".')
 
-    else: # if the user provides more than 1 argument (in addition to shapelets). Print error messages and quit.
-        raise RuntimeError('shapelets entry point only supports the config file name. I.e. "shapelets config".')
 
 def _run_tests():
     r"""
-    Main function that runs all the unit tests from shapelets/tests/ via unittest from Python STL. This is only invoked via the entry point "shapelets-test" from the top-most shapelets directory.
+    Main function that runs all the unit tests via unittest from Python STL. This is only invoked via the entry point "shapelets-test".
     
     """
-    @contextlib.contextmanager
-    def tempWorkingDir(path):
-        r"""
-        Temporarily create a working directory to execute CLI commands without actually changing the root of the global directory.
-
-        From stackoverflow:
-        https://stackoverflow.com/questions/75048986/way-to-temporarily-change-the-directory-in-python-to-execute-code-without-affect
-        
-        """
-        oldir = os.getcwd()
-        os.chdir(os.path.abspath(path))
-        try: yield
-        finally: os.chdir(oldir)
-
-    # get platform and then assume entry point "shapelets-test" executed from top-level directory
-    user_os = str(platform.system())
-
-    if user_os == 'Windows':
-        os.chdir("tests\\")
-        runcom = "python -B -m"
+    # notify user tests may take more than a few seconds
+    print("Initiating shapelets unit tests. This will likely take a few minutes.")
+    time.sleep(10)
+    
+    # navigate to tests/ folder relative to this file
+    tests_dir = os.path.join(Path(__file__).parents[0], 'tests')
+    os.chdir(tests_dir)
+
+    # command line arguments based on user OS
+    # automatically find all tests using unittest built-in discovery component
+    if str(platform.system()) == 'Windows':
+        os.system('python -B -m unittest -v')
     else:
-        os.chdir("tests/")
-        runcom = "python3 -B -m"
-
-    # find all .py files nested in tests/, and run them sequentially
-    for root, dirs, files in os.walk('.'):
-        for file in files:
-            if file.endswith('.py'):
-                with tempWorkingDir(root):
-                    print(f"\n\nRunning tests in {file}")
-                    if user_os == 'Windows': 
-                        os.system(f"{runcom} {file}")
-                    else: 
-                        os.system(f"{runcom} {file[:-3]}")                    
+        os.system('python3 -B -m unittest -v')
```

### Comparing `shapelets-1.0/shapelets/_run.py` & `shapelets-1.1/shapelets/_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,62 +14,68 @@
 # You should have received a copy of the GNU Lesser General Public License along with shapelets. If not, see           #
 # <https://www.gnu.org/licenses/>.                                                                                     #
 ########################################################################################################################
 
 import ast
 import configparser
 import os
+from pathlib import Path
 
 from .astronomy.galaxy import *
 
 from .self_assembly.misc import *
 from .self_assembly.quant import *
 from .self_assembly.wavelength import *
 
-def _run(config_file: str) -> None:
+def _run(config_file: str, working_dir: str) -> None:
     r"""
     Main run function that handles input configuration file.
     
     Parameters
     ----------
     * config_file : str
-        * The name of the configuration file
+        * The name of the configuration file in working_dir
+    * working_dir : str
+        * The absolute path (working directory) where the entry point was invoked from
     
     Notes
     -----
     Differentiation between submodule use is based on image_name or fits_name provided in config file. Note that this may need to be changed in the future if more astronomy functionality is added.
 
     """
     ## configparser setup and input/output path organization ##
 
     # instantiate and read
     config = configparser.ConfigParser()
-    config.read(config_file)
+    config_file = os.path.join(working_dir, config_file)
+    if not os.path.exists(config_file):
+        raise RuntimeError(f"Configuration file {config_file} does not exist. Check config filename spelling and ensure that it is located in {working_dir}.")
+    else:
+        config.read(config_file)
 
     # handle method
     method = config.get('general', 'method')
 
     # image and output paths
-    image_path = os.getcwd()+'/images/'
-    save_path = os.getcwd()+'/output/'
+    image_path = os.path.join(working_dir, 'images')
+    save_path = os.path.join(working_dir, 'output')
     if not os.path.exists(image_path): 
         raise RuntimeError(f"Path '{image_path}' does not exist.")
     if not os.path.exists(save_path): 
-        os.mkdir("output")
+        os.mkdir(save_path)
 
     ## self_assembly submodule use ##
         
     # parsing input image of nanostructure
     if config.get('general', 'image_name', fallback=None):
+
+        # read image to be analyzed
         image_name = config.get('general', 'image_name')
         image = read_image(image_name = image_name, image_path = image_path)
 
-        # obtain characteristic wavelength, needed for all self-assembly applications
-        char_wavelength = get_wavelength(image = image)
-
         if method == 'response_distance':
             shapelet_order = config.get('response_distance', 'shapelet_order', fallback = 'default')
             if shapelet_order != 'default':
                 shapelet_order = ast.literal_eval(shapelet_order)
 
             num_clusters = config.get('response_distance', 'num_clusters', fallback = 'default')
             if num_clusters != 'default':
@@ -78,56 +84,50 @@
             ux = config.get('response_distance', 'ux', fallback = 'default')
             uy = config.get('response_distance', 'uy', fallback = 'default')
             if ux != 'default':
                 ux = ast.literal_eval(ux)
             if uy != 'default':
                 uy = ast.literal_eval(uy)
 
-            response = convresponse(image = image, l = char_wavelength, shapelet_order = shapelet_order, normresponse = 'Vector')[0]
-            rd_field = rdistance(image = image, response = response, num_clusters = num_clusters, ux = ux, uy = uy)
+            rd_field = rdistance(image = image, num_clusters = num_clusters, shapelet_order = shapelet_order, ux = ux, uy = uy)
+
             process_output(image = image, image_name = image_name, save_path = save_path, output_from = 'response_distance', d = rd_field, num_clusters = num_clusters)
 
         elif method == 'orientation':
             pattern_order = config.get('orientation', 'pattern_order')
 
-            response, orients = convresponse(image = image, l = char_wavelength, shapelet_order = 6, normresponse = 'Individual')
-            mask, dilate, blended, maxval = orientation(pattern_order = pattern_order, l = char_wavelength, response = response, orients = orients)
+            mask, dilate, blended, maxval = orientation(image = image, pattern_order = pattern_order)
+
             process_output(image = image, image_name = image_name, save_path = save_path, output_from = 'orientation', mask = mask, dilate = dilate, orientation = blended, maxval = maxval)
-    
+            
         elif method == 'identify_defects':
             pattern_order = config.get('identify_defects', 'pattern_order')
 
-            num_clusters = config.get('identify_defects', 'num_clusters', fallback = 'default') 
-            if num_clusters != 'default':
-                num_clusters = ast.literal_eval(num_clusters)
+            centroids, clusterMembers, defects = defectid(image = image, pattern_order = pattern_order)
 
-            response = convresponse(image = image, l = char_wavelength, shapelet_order = 'default', normresponse = 'Vector')[0]
-            centroids, clusterMembers, defects = defectid(response = response, l = char_wavelength,
-                                                          pattern_order = pattern_order, num_clusters = num_clusters)
             process_output(image = image, image_name = image_name, save_path = save_path, output_from = 'identify_defects', centroids = centroids, clusterMembers = clusterMembers, defects = defects)
-        
+
         else:
             raise ValueError('"method" parameter from configuration file not recognized by shapelets.')
 
     ## astronomy submodule use ##
         
     # retrieving .fits path (if .fits file is provided)
     elif config.get('general', 'fits_name', fallback=None):
-        fits_path = os.getcwd()+'/images/' + config.get('general', 'fits_name')
+        fits_path = os.path.join(working_dir, 'images', config.get('general', 'fits_name'))
 
         if method == 'galaxy_decompose':
             shapelet_order = config.get('galaxy_decompose', 'shapelet_order', fallback = 'default')
             compression_order = config.get('galaxy_decompose', 'compression_order', fallback = 'default')
 
             output_base_path = save_path+fits_path[fits_path.rfind('/'):-5]
             n_max = int([shapelet_order, 10][shapelet_order == 'default'])
             compression_factor = int([compression_order, 25][compression_order == 'default'])
 
             fits_data = load_fits_data(fits_path)
             (galaxy_stamps, star_stamps, noiseless_data) = get_postage_stamps(fits_data, output_base_path)
             decompose_galaxies(galaxy_stamps, star_stamps, noiseless_data, n_max, compression_factor, output_base_path)
-
         else:
             raise ValueError('"method" parameter from configuration file not recognized by shapelets.')
         
     else:
         raise NameError('No image (from image_name) or FITS (from fits_name) listed in configuration file.')
```

### Comparing `shapelets-1.0/shapelets/astronomy/__init__.py` & `shapelets-1.1/shapelets/astronomy/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/astronomy/galaxy.py` & `shapelets-1.1/shapelets/astronomy/galaxy.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/astronomy/misc.py` & `shapelets-1.1/shapelets/astronomy/misc.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/discrete_transform/__init__.py` & `shapelets-1.1/shapelets/discrete_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/docs/__init__.py` & `shapelets-1.1/shapelets/docs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 
 from .example_1 import *
 from .example_2 import *
 from .example_3 import *
 from .example_4 import *
 from .installation_guide import *
 from .package_interface import *
-from .custom_commands import *
-from .WSL_support import *
+from .custom_commands import *
```

### Comparing `shapelets-1.0/shapelets/docs/custom_commands.py` & `shapelets-1.1/shapelets/docs/custom_commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 r"""
 
 # Custom Commands
 
 The shapelets package makes use of [entry points](https://packaging.python.org/en/latest/specifications/entry-points/).
 These are custom command-line arguments that trigger specific programming tasks in the background.
 
-* `shapelets CONFIG` - here, `CONFIG` is the name of the text-based configuration file that will perform some specific analysis based on the parameters present in the file. See the package [examples](https://uw-comphys.github.io/shapelets/shapelets/docs.html).
-* `shapelets-test` - triggers all unit tests in the [tests](https://github.com/uw-comphys/shapelets/tree/main/tests) directory and will report any failures. It is encouraged to use this command if modifying the package source code and after initially [installing](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) the `shapelets` package.
+* `shapelets CONFIG` - this entry point is used to interact with the shapelets package via configuration files. Here `CONFIG` is the name of the text-based configuration file that will perform a particular analysis based on its contents. See the package [examples](https://uw-comphys.github.io/shapelets/shapelets/docs.html) for useful demonstration. Note that the configuration file must be in the same directory as your working (terminal) directory to use this entry point correctly.
+* `shapelets-test` - triggers all [unit tests](https://github.com/uw-comphys/shapelets/tree/main/shapelets/tests) and will report any failures. It is encouraged to use this command if (1) you are modifying the package source code and (2) after initial [installation](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) of the shapelets package.
 
 """
```

### Comparing `shapelets-1.0/shapelets/docs/example_1.py` & `shapelets-1.1/shapelets/docs/example_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 This example demonstrates the response distance method ([R. Suderman (2015)](https://doi.org/10.1103/PhysRevE.91.033307)) for self-assembly microscopy imaging using the ``shapelets.self_assembly`` submodule.
 
 This example can be run in two different ways:
 * (1) text-based configuration files (shown here), and 
 * (2) programmatically via script-based Python programming (`example_1.py`)
 
+This example will go through the text-based configuration file approach (1). For users comfortable with Python programming, the example_1.py file is setup to run the same analysis described below. The outputs will appear in the same directory.
+
 ## Overview
 
 The response distance ([R. Suderman (2015)](https://doi.org/10.1103/PhysRevE.91.033307)) is calculated as:
 
 $$ d_{i, j} = \min \| \vec{R} - \vec{r_{i,j}} \|_2 $$
 
 where $\vec{r_{i,j}}$ denotes the given response vector at pixel location $\{i, j\}$ and $\vec{R}$ is the reference set (or subdomain) of response vectors.
@@ -51,41 +53,41 @@
 
 	[general]
 	image_name = lamSIM1.png
 	method = response_distance
 
 	[response_distance]
 	shapelet_order = default
-	num_clusters = 20
+	num_clusters = default
 	ux = [50, 80]
 	uy = [150, 180]
 
 where **image_name** and **method** are required parameters that specify the image filename and method used for analysis.
 
-The method outlined in the configuration file will also have its own header with specific parameters. The **response_distance** method may contain up to four parameters. Note that *default* refers to the default value if the parameter is excluded from the configuration file.
+The method outlined in the configuration file will also have its own header with specific parameters. The **response_distance** method may contain up to four parameters. Certain parameters also have defaults, these can be excluded from the configuration file if desired.
 
 **shapelet_order** `int`
 
 * The maximum shapelet order ($m'$) used for convolution operations, i.e. $m \in [1, m']$ shapelets are used 
-* default = $m'$ $\rightarrow$ computed by the higher-order shapelet algorithm ([M.P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
+* Default value is computed by the higher-order shapelet algorithm ([M.P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
 
 **num_clusters** `int`
 
-* The number of clusters for k-means clustering. Note using 0 is acceptable and will use all response vectors in the reference region (subdomain) ([R. Suderman (2015)](https://doi.org/10.1103/PhysRevE.91.033307))
-* default = 20 $\rightarrow$ as determined by a distortion analysis ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353))
+* The number of clusters for k-means clustering. Note using 0 is acceptable and will use all response vectors in the reference region ([R. Suderman (2015)](https://doi.org/10.1103/PhysRevE.91.033307))
+* Default value is 20 clusters as determined by a distortion analysis ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353))
 
 **ux** `list`
 
-* The lower and upper x-coordinates (respectively) of the reference region (subdomain)
-* default $\rightarrow$ user is required to select x-bounds during runtime, see [here](#selecting-subdomain-bounds-during-runtime) for instructions
+* The lower and upper x-coordinates (respectively) of the reference region 
+* Default requires user to select x-bounds during runtime, see [here](#selecting-subdomain-bounds-during-runtime) for instructions
 
 **uy** `list`
 
-* The lower and upper y-coordinates (respectively) of the reference region (subdomain)
-* default $\rightarrow$ user is required to select y-bounds during runtime, see [here](#selecting-subdomain-bounds-during-runtime) for instructions
+* The lower and upper y-coordinates (respectively) of the reference region 
+* Default requires user to select y-bounds during runtime, see [here](#selecting-subdomain-bounds-during-runtime) for instructions
 
 ### Run Example
 
 Please ensure that `shapelets` is properly installed before proceeding.
 See [here](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for installation instructions.
 
 Navigate your terminal to "shapelets/examples/example_1". When you are ready, execute ``shapelets config`` in the command line.
@@ -110,12 +112,8 @@
 **Additional Tips**
 
 * You may use the **magnifying glass** (bottom left) to zoom in on a specific region
 * You may use the **left arrow** (bottom left) to return to original zoom
 * Failure to choose 4 points/corners (i.e., choosing less or more than 4) will restart the process automatically
 * Please choose a region of the pattern that contains zero observable defects in order to maximize the response distance results
 
-## Scripting Method
-
-For users comfortable with Python programming, the **example_1.py** file is structured to run the same analysis as described previously. The outputs will appear in the same directory.
-
 """
```

### Comparing `shapelets-1.0/shapelets/docs/example_2.py` & `shapelets-1.1/shapelets/docs/example_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 This example demonstrates the defect identification method ([M.P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4)) for self-assembly microscopy imaging using the ``shapelets.self_assembly`` submodule.
 
 This example can be run in two different ways:
 * (1) text-based configuration files (shown here), and 
 * (2) programmatically via script-based Python programming (`example_2.py`)
 
+This example will go through the text-based configuration file approach (1). For users comfortable with Python programming, the example_2.py file is setup to run the same analysis described below. The outputs will appear in the same directory.
+
 ## Overview
 
 The defect identification method ([M.P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4)) is a modification of the response distance method ([R. Suderman (2015)](https://doi.org/10.1103/PhysRevE.91.033307)), whereby the user is required to manually select clusters associated with defects or defect structures, and the defect response distance is computed for each response vector in each cluster. 
 
 The defect response distance is similar to the response distance, but the reference subdomain is the centroid response vector of each cluster (and not a set of reference response vectors). For example, for a given cluster $C$ with centroid $C_c$, the defect response distance for response vector $c_i$ belonging to cluster $C$ with centroid response vector $C_c$ is computed as:
 
 $$ d_i = \| C_c - c_i \|_2 $$
@@ -53,33 +55,22 @@
 
 	[general]
 	image_name = hexSIM1.png
 	method = identify_defects
 
 	[identify_defects]
 	pattern_order = hexagonal
-	num_clusters = 10
 
 where **image_name** and **method** are required parameters that specify the image filename and method used for analysis.
 
-The method outlined in the configuration file will also have its own header with specific parameters. The **identify_defects** method may contain up to two parameters. Note that default refers to the default value if the parameter is excluded from the configuration file.
+The method outlined in the configuration file will also have its own header with specific parameters. The **identify_defects** method must contain one parameter, described below.
 
 **pattern_order** `str`
 
 * The pattern order (symmetry) observed in the image. Options are `stripe`, `square`, `hexagonal`
-* This parameter **does not have a default value**
-
-**num_clusters** `int`
-
-* The number of clusters for k-means clustering. Must be $\geq$ 1.
-* Default values are as follows,
-	* If pattern_order = stripe $\rightarrow$ 4
-	* If pattern_order = square $\rightarrow$ 8
-	* If pattern_order = hexagonal $\rightarrow$ 10
-* If an integer value is provided that is below the above default, the code will defer to the default value
 
 ### Run Example
 
 Please ensure that `shapelets` is properly installed before proceeding.
 See [here](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for installation instructions.
 
 Navigate your terminal to "shapelets/examples/example_2". When you are ready, execute ``shapelets config`` in the command line.
@@ -98,13 +89,8 @@
 The output (shown below) will be available in "shapelets/examples/example_2/output" containing the location of each cluster (top left), radar chart of centroid response vectors (top right), the defect response distance scalar field (bottom left), and this field superimposed onto the original pattern (bottom right). In this example, clusters 2, 5, and 8 were chosen by the user as defect clusters. 
 
 ![](images/hexSIM1_defectid_clustloc_k10.png)
 ![](images/hexSIM1_defectid_rc_k10.png)
 
 ![](images/hexSIM1_defectid_drd_k10.png)
 ![](images/hexSIM1_defectid_drd_overlay_k10.png)
-
-## Scripting Method
-
-For users comfortable with Python programming, the example_2.py file is structured to run the same analysis as described previously. The outputs will appear in the same directory.
-
 """
```

### Comparing `shapelets-1.0/shapelets/docs/example_3.py` & `shapelets-1.1/shapelets/docs/example_3.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 This example demonstrates computation of the local pattern orientation  for self-assembly microscopy imaging using the ``shapelets.self_assembly`` submodule.
 
 This example can be run in two different ways:
 * (1) text-based configuration files (shown here), and 
 * (2) programmatically via script-based Python programming (`example_3.py`)
 
+This example will go through the text-based configuration file approach (1). For users comfortable with Python programming, the example_3.py file is setup to run the same analysis described below. The outputs will appear in the same directory.
+
 ## Overview
 
 Local pattern orientation is concerned with the relative orientation of nanostructure along grain boundaries and in between grains. The local pattern orientation method ([M.P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4)) contains three (3) main steps:
 
 * (1) **Masking**: Performed for well-defined features using a specific response threshold. This threshold is found via an interative scheme. Only the orientation values from these well-defined features are retained after masking.
 * (2) **Dilation**: Performed via morphological greyscale dilation from ``scipy.ndimage.grey_dilation`` ([P. Virtanen (2020)](https://doi.org/10.1038/s41592-019-0686-2)) to expand the orientation from well-defined features and define orientation in void space (between well-defined features and over orientational boundaries). The dilation kernel size is chosen to be $2\lambda$, where $\lambda$ is the characteristic wavelength of the pattern and is also the approximate distance between well-defined features. 
 * (3) **Blending**: Performed via a median filter from `scipy.ndimage.median_filter`` ([P. Virtanen (2020)](https://doi.org/10.1038/s41592-019-0686-2)) to allow for effective transition in orientations between neighbouring well-defined features and across orientational boundaries. The blending kernel size is chosen to be $4\lambda$ so that the orientation is averaged from two layers of surrounding neighbouring features.
@@ -56,20 +58,19 @@
 	method = orientation
 
 	[orientation]
 	pattern_order = square
 
 where **image_name** and **method** are required parameters that specify the image filename and method used for analysis.
 
-The method outlined in the configuration file will also have its own header with specific parameters. The orientation method must contain one parameter. Note that default refers to the default value if the parameter is excluded from the configuration file.
+The method outlined in the configuration file will also have its own header with specific parameters. The orientation method must contain one parameter, described below.
 
 **pattern_order** `str`
 
 * The pattern order (symmetry) observed in the image. Options are `stripe`, `square`, `hexagonal`
-* This parameter does not have a default value
 
 ## Run Example
 
 Please ensure that `shapelets` is properly installed before proceeding. 
 See [here](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for installation instructions.
 
 Navigate your terminal to "shapelets/examples/example_3". When you are ready, execute ``shapelets config`` in the command line.
@@ -79,13 +80,8 @@
 The output (shown below) will then be available in "shapelets/examples/example_3/output" containing the mask (top left), dilated feature orientation (top right), smoothed orientation result, and the smoothed orientation result superimposed onto the original pattern (shown below, respectively).
 
 ![](images/sqrAFM2_orientation_maskedresp.png)
 ![](images/sqrAFM2_orientation_dilate.png)
 
 ![](images/sqrAFM2_orientation_blend.png)
 ![](images/sqrAFM2_orientation_overlay.png)
-
-## Scripting Method 
-
-For users comfortable with Python programming, the example_3.py file is structured to run the same analysis as described previously. The outputs will appear in the same directory.
-
 """
```

### Comparing `shapelets-1.0/shapelets/docs/example_4.py` & `shapelets-1.1/shapelets/docs/example_4.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 
 	[galaxy_decompose] 
 	shapelet_order = default 
 	compression_order = 20 
 
 where **image_name** and **method** are required parameters that specify the image filename and method used for analysis.
 
-The method outlined in the configuration file will also have its own header with specific parameters. The **galaxy_decompose** method may contain up to two parameters. Note that default refers to the default value if the parameter is excluded from the configuration file.
+The method outlined in the configuration file will also have its own header with specific parameters. The **galaxy_decompose** method may contain up to two parameters.  Only values that have a default value may be omitted from the configuration file (see below, if no default value is written then it must be present in configuration file). 
 
 **shapelet_order** `int`
 
 * The maximum shapelet order (i.e. cartesian shapelets ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x))) to calculate coefficients such that $n_1 + n_2 \leq n_{max}$.
-* default = 10
+* Default value is 10
 
 **compression_order** `int`
 
 * The number of shapelet coefficients to use for final image reconstruction
-* default = 25
+* Default value is 25. Here 20 is used just as an example
 
 ### Run Example
 
 Please ensure that `shapelets` is properly installed before proceeding.
 See [here](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html) for installation instructions.
 
 Navigate your terminal to "shapelets/examples/example_4". When you are ready, execute ``shapelets config`` in the command line.
```

### Comparing `shapelets-1.0/shapelets/docs/package_interface.py` & `shapelets-1.1/shapelets/docs/package_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 2. Scripting method (intended for those comfortable with Python programming)
     * A more traditional format where relevant methods are imported in python files, i.e. 
 
 ```python 
 from shapelets.functions import cartesian2D
 ```
 
-The [examples](https://uw-comphys.github.io/shapelets/shapelets/docs.html) are implemented primarily using the text-based configuration file method (#1).
-However, the examples also have Python files (.py) that perform the exact same analysis as shown via the configuration file method. 
+The [examples](https://uw-comphys.github.io/shapelets/shapelets/docs.html) are implemented via the text-based configuration file method (#1 above).
+However, these examples also have associated Python files (.py) that perform the exact same analysis as shown via the configuration file method. 
 
 """
```

### Comparing `shapelets-1.0/shapelets/functions.py` & `shapelets-1.1/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/self_assembly/__init__.py` & `shapelets-1.1/shapelets/self_assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets/self_assembly/misc.py` & `shapelets-1.1/shapelets/self_assembly/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,30 +85,44 @@
         * The image as a numpy.ndarray.
 
     Notes
     -----
     Re-scaling of image to greyscale on [-1, 1] is intentional to align with the minimum and maximum of shapelet function values.
     
     """
-    if os.path.exists(image_path):
-        if image_path[-1] != '/':
-            f = cv2.imread(image_path+'/'+image_name)
-        else:
-            f = cv2.imread(image_path+image_name)
-        f = cv2.cvtColor(f, cv2.COLOR_BGR2GRAY )
-        if verbose:
-            print('Successfully loaded {}'.format(image_name))
-            print('Shape of image is:', f.shape)
-        
-        f = ( ((f-f.min()) / (f.max()-f.min())) * 2 ) - 1
-        if verbose: 
-            print('Image normalized to greyscale on [-1, 1]')
-        return f
-    else: 
-        raise RuntimeError('Image path does not exist.')
+    # Ensure image_path provided exists
+    if not os.path.exists(image_path):
+        raise RuntimeError(f'Image path: {image_path} does not exist.')
+    
+    # read image then ensure image does exist (by evaluating result of cv2.imread)
+    f = cv2.imread(os.path.join(image_path, image_name))
+    if not isinstance(f, np.ndarray):
+        raise RuntimeError(f"Could not read image: {image_name}. Ensure it is located in {image_path} and is of image format.")
+
+    # convert to grayscale
+    f = cv2.cvtColor(f, cv2.COLOR_BGR2GRAY)
+
+    # check if re-scaling is needed b/c k-means clustering cannot handle very large images
+    init_shape = f.shape
+    resized = False 
+    while any(dim >= 1000 for dim in f.shape):
+        dim0, dim1 = round(f.shape[0]*0.8), round(f.shape[1]*0.8)
+        f = cv2.resize(f, dsize=(dim0, dim1))
+        resized = True
+
+    # rescale to [-1, 1] greyscale 
+    f = ( ((f-f.min()) / (f.max()-f.min())) * 2 ) - 1
+
+    if verbose: 
+        print(f"Successfully loaded image: {image_name}")
+        if resized: print(f"New image dimensions are: {f.shape} as initial size {init_shape} too large")
+        else: print(f"Image dimensions are: {f.shape}")
+        print(f"Image {image_name} normalized to greyscale on [-1, 1] to align with shapelet kernels")
+
+    return f
 
 def process_output(image: np.ndarray, image_name: str, save_path: str, output_from: str, **kwargs) -> None:
     r""" 
     Processes and saves output from any of the functions below,
     * shapelets.self_assembly.quant.rdistance
     * shapelets.self_assembly.quant.orientation
     * shapelets.self_assembly.quant.defectid
@@ -136,22 +150,29 @@
     * output_from = 'identify_defects'    -->     defects, centroids, clusterMembers (see shapelets.self_assembly.quant.defectid)
 
     References
     ----------
     .. [1] http://dx.doi.org/10.1088/1361-6528/ad1df4
 
     """
+    # check that save_path exists
+    if not os.path.exists(save_path):
+        os.mkdir(save_path)
+        
     os.chdir(save_path)
 
+    # need to get characteristic wavelength for image trimming
     char_wavelength = get_wavelength(image = image, verbose = False)
 
     if output_from == 'response_distance':
         # get kwargs
         d = kwargs['d']
         num_clusters = kwargs['num_clusters']
+        if num_clusters == 'default':
+            num_clusters = '20'
 
         # final image processing for response distance scalar field
         d = (d-d.min()) / (d.max()-d.min())
         d = 1-d
         d = trim_image(im=d, l=char_wavelength)
 
         # plot and save
@@ -355,9 +376,9 @@
     The characteristic wavelength[1]_ is roughly the distance between feature centers, thus making it an appropriate size for image trim or truncation after convolution.
 
     References
     ----------
     .. [1] http://dx.doi.org/10.1103/PhysRevE.91.033307
 
     """
-    trim = int(l)
+    trim = round(l/2)
     return im[trim:-trim, trim:-trim]
```

### Comparing `shapelets-1.0/shapelets/self_assembly/quant.py` & `shapelets-1.1/shapelets/self_assembly/quant.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,80 +21,77 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.cluster.vq import kmeans, vq
 from scipy.signal import fftconvolve
 from scipy.ndimage import grey_dilation, median_filter
 
 from .misc import trim_image, make_grid
-from .wavelength import lambda_to_beta
+from .wavelength import get_wavelength, lambda_to_beta
 from ..functions import orthonormalpolar2D
 
 __all__ = [
     'convresponse',
     'defectid',
     'orientation',
     'rdistance'
 ]
 
-def convresponse(image: np.ndarray, l: float, shapelet_order: Union[str,int] = 'default', normresponse: str = 'Vector', verbose: bool = True):
+def convresponse(image: np.ndarray, shapelet_order: Union[str,int] = 'default', normresponse: str = 'Vector', verbose: bool = True):
     r""" 
     This function computes the convolution between a range of shapelets kernels and an image, extracting the magnitude of response as well as the shapelet-based orientation.
     
     Parameters
     ----------
     * image: np.ndarray
         * The image to be convolved with shapelet kernels
-    * l: float
-        * The characteristic wavelength of the image[1]_
     * shapelet_order: Union[str,int]
-        * Set as 'default' to use higher-order shapelets[3]_ ($m \leq m'$). Can also accept integer value such that analysis uses $m \in [1, shapelet_{order}]$
+        * Set as 'default' to use higher-order shapelets[2]_ ($m \leq m'$). Can also accept integer value such that analysis uses $m \in [1, shapelet_{order}]$
     * normresponse: str, optional
         * Normalize magnitude of response (omega) in terms of response vectors = "Vector" (default). Normalize each m-fold response w.r.t itself on [0, 1) = "Individual"
     * verbose: bool, optional
         * True (default) to print out information from convolution operation to console
 
     Returns
     -------
     * omega: numpy.ndarray
         * The magnitude of (maximum) convolutional response as a 3D array
     * phi: numpy.ndarray
         * The shapelet orientation at maximum response normalized to $[0, 2pi/m)$
 
     Notes
     -----
-    This function uses the orthonormal polar shapelet definition[2]_ (see shapelets.functions.orthonormalpolar2D).
+    This function uses the orthonormal polar shapelet definition[1]_ (see shapelets.functions.orthonormalpolar2D).
 
     References
     ----------
-    .. [1] http://dx.doi.org/10.1103/PhysRevE.91.033307
-    .. [2] https://doi.org/10.1088/1361-6528/aaf353
-    .. [3] http://dx.doi.org/10.1088/1361-6528/ad1df4
+    .. [1] https://doi.org/10.1088/1361-6528/aaf353
+    .. [2] http://dx.doi.org/10.1088/1361-6528/ad1df4
 
     """
     if not isinstance(image, np.ndarray):
         raise TypeError('image parameter must be a numpy array.')
 
     if isinstance(shapelet_order, str):
         if shapelet_order == 'default': 
             mmax = None
         else:
             raise ValueError('shapelet_order parameter as a str must be "default".')
-        
     elif isinstance(shapelet_order, int):
         mmax = shapelet_order
-
     else:
         raise TypeError('shapelet_order parameter must either be "default" or integer value.')
     
     if not isinstance(normresponse, str):
         raise TypeError('normresponse parameter must be of type str.')
-    
     elif normresponse not in ['Vector', 'Individual']:
         raise ValueError('Valid normresponse parameters are "Vector" or "Individual".')
 
+    # get characteristic wavelength of image 
+    l = get_wavelength(image=image, verbose=verbose)
+
     minRespTol = 0.1
     
     Ny, Nx = image.shape
     omegaTotal = []
 
     if mmax != None:
         omega = np.empty((Ny, Nx, mmax)) 
@@ -183,140 +180,107 @@
     # to correct angles on [0, 2pi/m] as per steerable shapelet theory from ref [1].
     for i in range(phi.shape[2]):
         phi[:,:,i] = (phi[:,:,i] - phi[:,:,i].min()) / (phi[:,:,i].max() - phi[:,:,i].min())
         phi[:,:,i] *=  2*np.pi / (i+1)
 
     return omega, phi
 
-def defectid(response: np.ndarray, l: float, pattern_order: str, num_clusters: Union[str,int]):
+def defectid(image: np.ndarray, pattern_order: str, verbose: bool = True):
     r""" 
     Computes the defect identification method[1]_. Also known as the defect response distance method.
 
     Parameters
     ----------
-    * response: np.ndarray
-        * The magnitude of (maximum) convolutional response as a 3D array, obtained from shapelets.self_assembly.quant.convresponse
-    * l: float
-        * The characteristic wavelength of the image
+    * image: numpy.ndarray
+        * The image loaded as a numpy array
     * pattern_order: str
         * Pattern order (symmetry type). Options are: 'stripe', 'square', 'hexagonal'
-    * num_clusters: str or int
-        * The number of clusters as input to k-means clustering[2]_. Use "default" to get default value based on pattern_order. For stripe, square, and hexagonal patterns, the minimum value is 4, 8, and 10 respectively
+    * verbose: bool, optional
+        * True (default) to print out information from convolution operation to console
     
     Returns
     -------
     * centroids: np.ndarray
         * The centroids from k-means clustering[2]_. Each centroid is a row vector
     * clusterMembers2D: np.ndarray
-        * Shows which cluster each pixel from image is a member of. I.e., value of 1 would mean it belongs to the cluster who's centroid is centroids[1]
+        * Shows which cluster each pixel from image is a member of. I.e., value of 1 would mean it belongs to the cluster who's centroid is dedfined by centroids[1]
     * defects: np.ndarray
-        The result of the defect response distance method[1]_
+        * The result of the defect response distance method[1]_
 
     References
     ----------
     .. [1] http://dx.doi.org/10.1088/1361-6528/ad1df4
     .. [2] https://doi.org/10.1007/978-3-642-29807-3
 
     """
-    if not isinstance(response, np.ndarray):
-        raise TypeError('response parameter must be a numpy array.')
-    
-    if isinstance(num_clusters, str):
-        if num_clusters != 'default':
-            raise ValueError('num_clusters as str type must be "default".')
-    elif not isinstance(num_clusters, int):
-        raise TypeError('num_clusters must be integer or "default".')
+    if not isinstance(image, np.ndarray):
+        raise TypeError('image must be a numpy array.')
 
     if not isinstance(pattern_order, str):
         raise TypeError('pattern_order parameter must be of str type.')
+    elif pattern_order not in ['stripe', 'square', 'hexagonal']:
+        raise ValueError('pattern_order parameter only accepts "stripe", "square", "hexagonal" str values.')
     
-    if pattern_order == 'stripe': 
-        if num_clusters == 'default':
-            num_clusters = 4
-        elif int(num_clusters) < 4:
-            print("num_clusters parameter too low, defaulting to 4.")
-            num_clusters = 4
-        else:
-            num_clusters = int(num_clusters)
-            
-    elif pattern_order == 'square': 
-        if num_clusters == 'default':
-            num_clusters = 8
-        elif int(num_clusters) < 8:
-            print("num_clusters parameter too low, defaulting to 8.")
-            num_clusters = 8
-        else:
-            num_clusters = int(num_clusters)
-            
-    elif pattern_order == 'hexagonal': 
-        if num_clusters == 'default':
-            num_clusters = 10
-        elif int(num_clusters) < 10:
-            print("num_clusters parameter too low, defaulting to 10.")
-            num_clusters = 10
-        else:
-            num_clusters = int(num_clusters)
-            
-    else: 
-        raise ValueError('Valid pattern_order parameters are "stripe", "square", "hexagonal".')
+    # enforce appropriate number of clusters depending on pattern_order
+    min_clusters = {'stripe': 4, 'square': 8, 'hexagonal': 10}
+    num_clusters = min_clusters[pattern_order]
     
+    # get convolutional response data 
+    response = convresponse(image = image, shapelet_order = 'default', normresponse = 'Vector', verbose=verbose)[0]
     response2D = response.reshape(-1, response.shape[-1])
     
     # clustering 
     t1 = time.time()
-    print(f"Performing k-means clustering with k={num_clusters}, this may take a while...")
+    if verbose:
+        print(f"Performing k-means clustering with k={num_clusters}, this may take a while...")
     centroids = kmeans(response2D, num_clusters)[0]
     clusterMembers1D, dists1D = vq(response2D, centroids)
     clusterMembers2D = clusterMembers1D.reshape(response.shape[0:2]) 
     
     t2 = time.time() - t1
-    print(f"Clustering runtime = {t2:0.3} s")
+    if verbose:
+        print(f"Clustering runtime = {t2:0.3} s")
 
     # get inputs of selected clusters
-    clusterMembers2DTrim = trim_image(clusterMembers2D, l)
-    plt.imshow(clusterMembers2DTrim, cmap='jet')
+    plt.imshow(clusterMembers2D, cmap='jet')
     plt.axis('off')
     plt.title('a = add point; del/backspace = remove point; enter = finish')
     win_positions = np.array(plt.ginput(n = -1, timeout = -1, mouse_add=None, mouse_pop=None, mouse_stop=None))
     win_positions = np.round(win_positions, 0).astype(int)
 
     # now mask out non-selected clusters
     dists1D = (dists1D - dists1D.min()) / (dists1D.max() - dists1D.min())
     dists2D = dists1D.reshape(response.shape[0:2])
     defects = np.zeros((response.shape[0], response.shape[1]))
 
     selected_clusters = []
     for i in range(win_positions.shape[0]):
         x, y = win_positions[i][0], win_positions[i][1]
-        cluster = clusterMembers2DTrim[y, x] 
+        cluster = clusterMembers2D[y, x] 
 
         if cluster not in selected_clusters:
             selected_clusters.append(cluster)
             # mask out the cluster from non-trimmed data, clusterMembers2D
             defects += np.where(clusterMembers2D == int(cluster), 1, 0)
     
     # compute defect response distance
     defects = defects * dists2D
     
     return centroids, clusterMembers2D, defects 
 
-def orientation(pattern_order: str, l: float, response: np.ndarray, orients: np.ndarray, verbose: bool = True):
+def orientation(image: np.ndarray, pattern_order: str, verbose: bool = True):
     r""" 
     Computes the local pattern orientation[1]_ via an iterative scheme using shapelet orientation at maximum response from steerable filter theory[2]_.
 
     Parameters
     ----------
+    * image: numpy.ndarray
+        * The image loaded as a numpy array
     * pattern_order: str
         * Pattern order (symmetry type). Options are: 'stripe', 'square', 'hexagonal'
-    * l: float
-        * The characteristic wavelength of the image
-    * response: np.ndarray
-        * The magnitude of (maximum) convolutional response as a 3D array, obtained from shapelets.self_assembly.quant.convresponse
-    * orients: np.ndarray
-        * The optimal shapelet filter orientation at maximum response as a 3D array, obtained from shapelets.self_assembly.quant.convresponse
     * verbose: bool, optional
         * True (default) to print out results of orientation algorithm to console
 
     Returns
     -------
     * mask: np.ndarray
         * The mask for well-defined features
@@ -334,32 +298,33 @@
     References
     ----------
     .. [1] http://dx.doi.org/10.1088/1361-6528/ad1df4
     .. [2] https://doi.org/10.1109/34.93808
     .. [3] https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.median_filter.html
     
     """
-    if (not isinstance(response, np.ndarray)) or (not isinstance(orients, np.ndarray)):
-        raise TypeError('response and orients parameters must be np.ndarray types.')
-
+    if not isinstance(image, np.ndarray):
+        raise TypeError('image must be a numpy array.')
+    
     if not isinstance(pattern_order, str):
         raise TypeError('pattern_order parameter must be of str type.')
+    elif pattern_order not in ['stripe', 'square', 'hexagonal']:
+        raise ValueError('pattern_order parameter only accepts "stripe", "square", "hexagonal" str values.')
 
-    params = {
-        'stripe': 0,
-        'square': 3, 
-        'hexagonal': 5
-    }
-
-    if pattern_order not in params:
-        raise ValueError('Valid pattern_order parameters are "stripe", "square", "hexagonal".')
-    
+    # get orientation information based on pattern_order
+    params = {'stripe': 0, 'square': 3, 'hexagonal': 5}
     ind = params[pattern_order]
     maxval = 2*np.pi / (ind+1)
-        
+    
+    # get characteristic wavelength of image 
+    l = get_wavelength(image=image, verbose=False)
+
+    # get convolutional response data up to m=6 (higher-order shapelets not needed for this method)
+    response, orients = convresponse(image = image, shapelet_order = 6, normresponse = 'Individual', verbose=verbose)
+
     # find the response threshold iteratively 
     orient = orients[:,:,ind].copy()
     resp_og = response[:,:,ind].copy()
     dilationsize = int( np.round(2*l, 0) )
     blendsize = int( np.round(4*l, 0) )
     
     accept_solution = False
@@ -376,40 +341,40 @@
         dilate = grey_dilation(mask, size=dilationsize)
         orientation_final = median_filter(dilate, size=blendsize)
     
         # compute error on undefined values after blending
         err = (orientation_final == 0.0).sum() / orientation_final.size
             
         if err > errtol:
-            #TODO: alex@matthew: adaptive step width for resptol
+            # TODO: Adaptive step width for resptol to decrease runtime
             resptol -= 0.01
             resptol = np.round(resptol, 2)
             if verbose:
                 print(f"Orientation failed with error {err:0.5}. Reducing threshold to {resptol}")
         elif resptol < 0:
             raise RuntimeError('Orientation failed to produce plot.')
         else:
             if verbose:
                 print(f"Orientation successful with error {err:0.5}")
             accept_solution = True  
 
     return mask, dilate, orientation_final, maxval
 
-def rdistance(image: np.ndarray, response: np.ndarray, num_clusters: Union[str,int], ux: Union[str,list] = 'default', uy: Union[str,list] = 'default', verbose: bool = True):
+def rdistance(image: np.ndarray, num_clusters: Union[str,int] = 'default', shapelet_order: Union[str,int] = 'default', ux: Union[str,list] = 'default', uy: Union[str,list] = 'default', verbose: bool = True):
     r""" 
     Compute the response distance method from ref.[1]_ using the methodology from ref.[2]_.
 
     Parameters
     ----------
     * image: numpy.ndarray
         * The image loaded as a numpy array
-    * response: np.ndarray
-        * The magnitude of (maximum) convolutional response as a 3D array, obtained from shapelets.self_assembly.quant.convresponse
     * num_clusters: Union[str,int]
         * The number of clusters as input to k-means clustering[3]_. If str, acceptable value is "default" (which uses 20 clusters[2]_)
+    * shapelet_order: Union[str,int]
+        * Set as 'default' to use higher-order shapelets[4]_ ($m \leq m'$). Can also accept integer value such that analysis uses $m \in [1, shapelet_{order}]$
     * ux: Union[str,list]
         * The bounds in the x-direction for the reference region. If using list option, must be 2 element list. Choosing "default" will force user to choose ref. region during runtime
     * uy: Union[str,list]
         * The bounds in the y-direction for the reference region. If using list option, must be 2 element list. Choosing "default" will force user to choose ref. region during runtime
     * verbose: bool, optional
         True (default) to print out results of response distance method to console
 
@@ -419,28 +384,25 @@
         * The response distance scalar field. Its dimensions are the same as the input image
 
     References
     ----------
     .. [1] http://dx.doi.org/10.1103/PhysRevE.91.033307
     .. [2] https://doi.org/10.1088/1361-6528/aaf353
     .. [3] https://doi.org/10.1007/978-3-642-29807-3
+    .. [4] http://dx.doi.org/10.1088/1361-6528/ad1df4
 
     """
     if not isinstance(image, np.ndarray):
         raise TypeError('image must be a numpy array.')
-    
-    if not isinstance(response, np.ndarray):
-        raise TypeError('response must be a numpy array.')
-
+        
     if isinstance(num_clusters, str):
         if num_clusters == 'default': 
             num_clusters = 20
         else:
             raise ValueError('If num_clusters is str type, must be "default" otherwise use int.')
-        
     elif not isinstance(num_clusters, int):
         raise TypeError('If num_clusters is not str type, must be int.')
 
     if type(ux) != type(uy):
         raise TypeError('ux and uy parameters must be both be "default" or both 2-element lists.')
     
     elif isinstance(ux, str):
@@ -487,14 +449,18 @@
         plt.figure(1, figsize=(7,7))
         plt.imshow(image, cmap = 'gray')
         plt.imshow(win, cmap = 'jet', alpha = 0.5)
         plt.title('Image with reference region', fontsize = 12)
         plt.axis('off')
         plt.show()"""
     
+    # get convolutional response data 
+    # shapelet_order parameter valid input check is enforced in the convresponse() function
+    response = convresponse(image = image, shapelet_order = shapelet_order, normresponse = 'Vector', verbose=verbose)[0]
+
     # compute response distance
     Ny, Nx = response.shape[0], response.shape[1]
     uX, uY = np.meshgrid(np.arange(ux[0], ux[1] + 1), np.arange(uy[0], uy[1] + 1))
     response_ref_whole = response[uY, uX] 
     response_ref_whole = response_ref_whole.reshape( -1, response_ref_whole.shape[-1] )
 
     if num_clusters != 0:
```

### Comparing `shapelets-1.0/shapelets/self_assembly/wavelength.py` & `shapelets-1.1/shapelets/self_assembly/wavelength.py`

 * *Files identical despite different names*

### Comparing `shapelets-1.0/shapelets.egg-info/PKG-INFO` & `shapelets-1.1/shapelets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets
-Version: 1.0
+Version: 1.1
 Summary: Shapelets is a module providing both reference access to various shapelet functions and some significant applications of them in science and astronomy.
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
 Keywords: shapelets,image analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -27,47 +27,51 @@
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
 
 ## What is shapelets? 
 
-shapelets is a python package that implements several shapelet functions and some of their significant applications in science and astronomy. These functions form a complete and orthonormal set, allowing them to capture complex geometries and information from any physical shape. Furthermore, shapelets are localized and can be scaled to match that of any physical feature. 
+Shapelets is a Python package that implements several shapelet functions and some of their significant applications in science and astronomy. Shapelet functions are a complete and orthogonal set of localized basis functions with mathematical properties convenient for manipulation and analysis of images from a broad range of applications.
 
-Due to these properties, they have seen extensive use in recent years, with several different formulations and applications:
+Due to these properties, they have seen extensive use in recent years, including:
 
 * Astronomy/astrophysics ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x), [R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445), [J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
-* Nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
+* Self-assembled nanomaterials ([R. Suderman (2015)](http://dx.doi.org/10.1103/PhysRevE.91.033307), [T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353), [M. P. Tino (2024)](http://dx.doi.org/10.1088/1361-6528/ad1df4))
 * Computational neuroscience ([J. D. Victor (2006)](https://doi.org/10.1152/jn.00498.2005), [T. O. Sharpee (2009)](https://doi.org/10.1007%2Fs10827-008-0107-5))
 * Medical imaging ([J. Weissman (2004)](https://doi.org/10.1364/OPEX.12.005760))
 
-The shapelets package provides reference documentation and code for four (4) shapelet functions: 
+The shapelets package provides reference code and documentation for 4 shapelet function definitions: 
 
 * Cartesian shapelets ([A. Refregier (2003)](https://doi.org/10.1046/j.1365-8711.2003.05901.x)), 
 * Polar shapelets ([R. Massey (2005)](https://doi.org/10.48550/arXiv.astro-ph/0408445)),
 * Orthonormal polar shapelets with constant radial scale ([T. Akdeniz (2018)](https://doi.org/10.1088/1361-6528/aaf353)), and 
 * Exponential shapelets ([J. Berge (2019)](https://doi.org/10.48550/arXiv.1903.05837))
 
 ## Getting Started
 
-Users are directed to the shapelets [official website](https://uw-comphys.github.io/shapelets/shapelets.html) for all documentation, including installation instructions, detailed examples, and more. 
-If you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below or the "Cite this repository" dropdown on the right sidebar.
+If you have Python 3.10+ installed on your machine, you can install the shapelets package in the terminal via pip: `pip install shapelets`
+
+If you do not have Python 3.10+ installed on your machine, consult the [installation guide](https://uw-comphys.github.io/shapelets/shapelets/docs/installation_guide.html). 
+
+New users are also encouraged to visit the [official website](https://uw-comphys.github.io/shapelets/shapelets.html) to understand how the shapelets package can be used along with detailed examples, custom terminal commands provided by the package, and more. 
+Additionally, if you plan to use the shapelets package for your own work, please cite appropriately using the [citation](#citation) below.
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with shapelets, please create a post using our package [issue tracker](https://github.com/uw-comphys/shapelets/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
 
 ## Contribute
 
 The authors of the shapelets package welcome external contributions to the source code. This process will be easiest if users adhere to the contribution policy:
 
 * Open an issue on the package [issue tracker](https://github.com/uw-comphys/shapelets/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the shapelets package, specifically detailed documentation for new methods (see existing methods for example documentation)
-* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the custom command: `shapelets-test`
-* Once the issue has been discussed with a package author, you may open a pull request containing your modifications
+* Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests via the entry point: `shapelets-test`
+* Once the issue has been discussed with a package author, you may open a pull request containing your code modifications
 
 ## Citation
 
 If you plan to use shapelets in your own work, please cite using the following Bibtex citation:
 
 ```
 @article{TinoShapelets2024,
@@ -81,15 +85,15 @@
 year = {2024},
 url = {https://joss.theoj.org/papers/10.21105/joss.06058}
 }
 ```
 
 ## Authors
 
-* Matthew Peres Tino
+* Matthew Peres Tino (mptino@uwaterloo.ca)
 * Abbas Yusuf Abdulaziz 
 * Nasser Mohieddin Abukhdeir
 * Robert Suderman 
 * Thomas Akdeniz
 
                   GNU LESSER GENERAL PUBLIC LICENSE
                        Version 2.1, February 1999
```

