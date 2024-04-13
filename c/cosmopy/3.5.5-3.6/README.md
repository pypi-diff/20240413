# Comparing `tmp/cosmopy-3.5.5.tar.gz` & `tmp/cosmopy-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmopy-3.5.5.tar", last modified: Mon Aug  8 03:21:28 2022, max compression
+gzip compressed data, was "cosmopy-3.6.tar", last modified: Sat Apr 13 19:13:19 2024, max compression
```

## Comparing `cosmopy-3.5.5.tar` & `cosmopy-3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.415507 cosmopy-3.5.5/
--rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-08-08 03:21:17.000000 cosmopy-3.5.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-08 03:21:17.000000 cosmopy-3.5.5/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-08 03:21:17.000000 cosmopy-3.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-08 03:21:17.000000 cosmopy-3.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-08-08 03:21:28.415507 cosmopy-3.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-08-08 03:21:17.000000 cosmopy-3.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.411507 cosmopy-3.5.5/cosmopy/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12408 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17973 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/cosmology.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.411507 cosmopy-3.5.5/cosmopy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11261 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/tests/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (121)     4919 2022-08-08 03:21:17.000000 cosmopy-3.5.5/cosmopy/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.411507 cosmopy-3.5.5/cosmopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-08 03:21:28.000000 cosmopy-3.5.5/cosmopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.415507 cosmopy-3.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)  1269374 2022-08-08 03:21:17.000000 cosmopy-3.5.5/docs/Hinshaw+2013-NineYearWMAP_1212.5226v3.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   346077 2022-08-08 03:21:17.000000 cosmopy-3.5.5/docs/Hogg99-DistanceMeasures_astroph9905116v4.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   337768 2022-08-08 03:21:17.000000 cosmopy-3.5.5/docs/Lahav&Liddle-CosmologicalParameters-2011.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   124812 2022-08-08 03:21:17.000000 cosmopy-3.5.5/docs/cosmopy_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 03:21:28.415507 cosmopy-3.5.5/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)     8352 2022-08-08 03:21:17.000000 cosmopy-3.5.5/notebooks/test.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-08 03:21:17.000000 cosmopy-3.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-08 03:21:17.000000 cosmopy-3.5.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-08 03:21:17.000000 cosmopy-3.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 03:21:28.415507 cosmopy-3.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-08 03:21:17.000000 cosmopy-3.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.054191 cosmopy-3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-13 19:13:15.000000 cosmopy-3.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-13 19:13:15.000000 cosmopy-3.6/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-13 19:13:15.000000 cosmopy-3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 19:13:15.000000 cosmopy-3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-13 19:13:19.054191 cosmopy-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-13 19:13:15.000000 cosmopy-3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.046191 cosmopy-3.6/cosmopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20837 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/cosmology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.050191 cosmopy-3.6/cosmopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11249 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/tests/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-13 19:13:15.000000 cosmopy-3.6/cosmopy/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.054191 cosmopy-3.6/cosmopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 19:13:19.000000 cosmopy-3.6/cosmopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.054191 cosmopy-3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  1269374 2024-04-13 19:13:15.000000 cosmopy-3.6/docs/Hinshaw+2013-NineYearWMAP_1212.5226v3.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   346077 2024-04-13 19:13:15.000000 cosmopy-3.6/docs/Hogg99-DistanceMeasures_astroph9905116v4.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   337768 2024-04-13 19:13:15.000000 cosmopy-3.6/docs/Lahav&Liddle-CosmologicalParameters-2011.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   124812 2024-04-13 19:13:15.000000 cosmopy-3.6/docs/cosmopy_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:13:19.054191 cosmopy-3.6/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-13 19:13:15.000000 cosmopy-3.6/notebooks/test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 19:13:15.000000 cosmopy-3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-13 19:13:15.000000 cosmopy-3.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 19:13:15.000000 cosmopy-3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:13:19.054191 cosmopy-3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 19:13:15.000000 cosmopy-3.6/setup.py
```

### Comparing `cosmopy-3.5.5/CHANGES.rst` & `cosmopy-3.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     -   Online documentation.
     -   Allow better usage of custom cosmo parameters
     -   Test against astropy instance using custom cosmological parameters
 
 
 Current
 -------
-    -   Added redshift to comoving and luminosity distance methods.
-    -   Added differential volume calculation (dVc/dz)
 
 
-v3.2 - 2018-01-03
+v3.6 - 2024-04-13
 -------------------
+    -   Added redshift to comoving-, luminosity-, and angular-diameter- distance methods.
+    -   Added differential volume calculation (dVc/dz)
 
 
 v3.1.3 - 2018-01-03
 -------------------
     -   Added colored output using the 'click' package (added to dependencies).
     -   Added significant unit-testing.  Coverage currently at 98%.
     -   Added function documentation.
```

### Comparing `cosmopy-3.5.5/LICENSE` & `cosmopy-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/PKG-INFO` & `cosmopy-3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: cosmopy
-Version: 3.5.5
+Version: 3.6
 Home-page: https://github.com/lzkelley/cosmopy
-Download-URL: https://github.com/lzkelley/cosmopy/archive/v3.5.5.tar.gz
+Download-URL: https://github.com/lzkelley/cosmopy/archive/v3.6.tar.gz
 Author: Luke Zoltan Kelley
-Author-email: lzkelley@northwestern.edu
+Author-email: lzkelley@berkeley.edu
 License: MIT
 Keywords: utilities,physics,astronomy,cosmology,astrophysics,calculator
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: astropy
+Requires-Dist: future
+Requires-Dist: click
 
 cosmopy
 =======
 
 |version| |build-status| |coverage|
```

### Comparing `cosmopy-3.5.5/README.rst` & `cosmopy-3.6/README.rst`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/cosmopy/__init__.py` & `cosmopy-3.6/cosmopy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 """
 
-__version__ = "3.2.1"
-__author__ = "Luke Zoltan Kelley <lzkelley@northwestern.edu>"
+__version__ = "3.6"
+__author__ = "Luke Zoltan Kelley <lzkelley@berkeley.edu>"
 __license__ = "MIT"
 
 import astropy as ap
 import astropy.constants  # noqa
 import astropy.units  # noqa
```

### Comparing `cosmopy-3.5.5/cosmopy/__main__.py` & `cosmopy-3.6/cosmopy/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 import numpy as np
 import astropy as ap
 
 from . cosmology import Cosmology
 from . import PC, ARCSEC, U_SEC, U_CM
 
-_RESULTS_FUNCS = ['luminosity_distance', 'comoving_distance', 'lookback_time', 'age']
+_RESULTS_FUNCS = ['comoving_distance', 'luminosity_distance', 'angular_diameter_distance', 'lookback_time', 'age']
+_RESULTS_FUNC_PARS = ['dc', 'dl', 'da', 'tl', 'ta']
 
-_RESULTS_FUNC_PARS = ['dl', 'dc', 'tl', 'ta']
 _RESULTS_PARS = ['z', 'a'] + _RESULTS_FUNC_PARS
 
-_COLOR_BASE = "magenta"  # "cyan"
-_COLOR_CONV = "green"  # "yellow"
+_COLOR_BASE = "magenta"
+_COLOR_CONV = "green"
 _COLOR_NAME = "red"
 
 # Enable imperial units (e.g. 'miles')
 ap.units.imperial.enable()
 
 
 def calc_basic(cosmo, sets):
@@ -67,36 +67,51 @@
         redz = cosmo.tlbk_to_z(tlbk.cgs.value)
         results['tl'] = tlbk
 
     # Comoving Distance
     elif sets.dc is not None:
         dcom = parse_input(sets.dc, U_CM)
         redz = cosmo.dcom_to_z(dcom.cgs.value)
-        # Calculate luminosity-distance manually
+        # Calculate distances manually
         dlum = dcom * (1.0 + redz)
+        dang = dcom / (1.0 + redz)
         results['dc'] = dcom
         results['dl'] = dlum
+        results['da'] = dang
 
     # Luminosity Distance
     elif sets.dl is not None:
         dlum = parse_input(sets.dl, U_CM)
         redz = cosmo.dlum_to_z(dlum.cgs.value)
-        # Calculate comoving-distance manually
+        # Calculate distances manually
         dcom = dlum / (1.0 + redz)
+        dang = dlum / (1.0 + redz)**2
         results['dc'] = dcom
         results['dl'] = dlum
+        results['da'] = dang
+
+    # Angular-diameter Distance
+    elif sets.da is not None:
+        dang = parse_input(sets.da, U_CM)
+        redz = cosmo.dang_to_z(dang.cgs.value)
+        # Calculate distances manually
+        dcom = dang * (1.0 + redz)
+        dlum = dcom * (1.0 + redz)
+        results['dc'] = dcom
+        results['dl'] = dlum
+        results['da'] = dang
 
     # No arguments set, raise error
     else:
         print("__main__.calc()")
         print("\t`sets` = '{}'".format(sets))
         raise ValueError("No input given!")
 
     # Calculate scale-factor if needed
-    scale = cosmo.z_to_a(redz) if scale is None else scale
+    scale = cosmo.z_to_a(redz) if (scale is None) else scale
     results['a'] = scale
     results['z'] = redz
 
     # Calculate the values not already set
     for pp, ff in zip(_RESULTS_FUNC_PARS, _RESULTS_FUNCS):
         if results[pp] is None:
             func = getattr(cosmo, ff)
@@ -166,14 +181,15 @@
              'Age of the Universe', 'Distance Modulus']
 
     retvals = {}
     printvals = []
     outs = []
     for kk, ss, tt, nn in zip(keys, symbs, types, names):
         vv = results[kk]
+        # print(f"key={kk}, symb={ss}, type={tt}, name={nn}, results[{kk}]={vv}")
         try:
             vv = vv.item()
         except AttributeError:
             pass
         v_std = vv if tt is None else vv.to(tt)
         base = "{:>10s} = {:.4f}".format(ss, v_std)
         # try:
@@ -306,14 +322,16 @@
                         help='target redshift z')
     parser.add_argument('-a', type=float, default=None,
                         help='target scale factor a')
     parser.add_argument('-dc', '-cd', default=None,
                         help='target coming distance D_C')
     parser.add_argument('-dl', '-ld', default=None,
                         help='target luminosity distance D_L')
+    parser.add_argument('-da', '-ad', default=None,
+                        help='target angular-diameter distance D_a')
     parser.add_argument('-tl', '-lt', default=None,
                         help='target look-back time T_L')
     parser.add_argument('-ta', '-at', default=None,
                         help='target universe age T_A')
 
     parser.add_argument('-v', '--version', action="store_true", default=False,
                         help='print version information.')
```

### Comparing `cosmopy-3.5.5/cosmopy/cosmology.py` & `cosmopy-3.6/cosmopy/cosmology.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         self._sort_lbk = np.argsort(self._grid_lbk)
         #    Comoving distances in centimeters
         self._grid_dcom = self.comoving_distance(zgrid).cgs.value
         self._sort_dcom = np.argsort(self._grid_dcom)
         #    Luminosity distances in centimeters
         self._grid_dlum = self.luminosity_distance(zgrid).cgs.value
         self._sort_dlum = np.argsort(self._grid_dlum)
+        #    Angular-diameter distances in centimeters
+        self._grid_dang = self.angular_diameter_distance(zgrid).cgs.value
+        self._sort_dang = np.argsort(self._grid_dang)
         return
 
     def __str__(self):
         """Return a string description of this instance.
         """
         rstr = "{} :: H0 = {:.8f}, Om0 = {:.8f}, Ob0 = {:.8f}".format(
             # __class__, self.Hubble0, self.Omega0, self.OmegaBaryon
@@ -155,14 +158,17 @@
         Returns
         -------
         float or array
             Redshift at the input scale-factors.
 
         """
         sf = np.asarray(sf)
+        if np.any(sf > 1) or np.any(sf <= 0):
+            raise ValueError(f"Number < than 1 and > 0 expected, got: {sf}")
+
         return (1.0/sf) - 1.0
 
     @staticmethod
     def z_to_a(redz):
         """Convert from redshift to scale-factor.
 
         :math:`a = 1.0 / (1 + z)`
@@ -175,14 +181,18 @@
         Returns
         -------
         float or array
             Scale factor(s) at the inpur redshift(s).
 
         """
         redz = np.asarray(redz)
+        # If blueshifting: don't
+        if np.any(redz < 0):
+            raise ValueError(f"Number >= than 0 expected, got: {redz}")
+
         return 1.0/(redz + 1.0)
 
     @staticmethod
     def _interp(vals, xx, yy, inds=None):
         """Interpolate to the target locations.
         """
         if inds is None:
@@ -261,14 +271,31 @@
         dl : array_like
             Luminosity distance to the given scale-factors.  Units of [cm].
 
         """
         dl = self._interp(scafa, self._grid_a, self._grid_dlum, self._sort_a)
         return dl
 
+    def a_to_dang(self, scafa):
+        """Get the angular-diameter distance [cm] at the given scale factor(s).
+
+        Parameters
+        ----------
+        scafa : array_like,
+            Scale-factor ($a$) describing the distance/time of the universe. Unitless in (0.0, 1.0].
+
+        Returns
+        -------
+        da : array_like
+            Luminosity distance to the given scale-factors.  Units of [cm].
+
+        """
+        da = self._interp(scafa, self._grid_a, self._grid_dang, self._sort_a)
+        return da
+
     def a_to_tage(self, sca):
         """Get the age of the universe [seconds] at the given scale factor(s).
 
         Parameters
         ----------
         scafa : array_like,
             Scale-factor ($a$) describing the distance/time of the universe. Unitless in (0.0, 1.0].
@@ -311,14 +338,16 @@
 
         Returns
         -------
         dc : array_like
             Comoving distance to the given redshift(s).  Units of [cm].
 
         """
+        if np.any(redz < 0):
+            raise ValueError(f"Number >= than 0 expected, got: {redz}")
         dc = self._interp(redz, self._grid_z, self._grid_dcom, self._sort_z)
         return dc
 
     def z_to_dlum(self, redz):
         """Get the luminosity distance [cm] at the given redshift(s).
 
         Parameters
@@ -328,31 +357,52 @@
 
         Returns
         -------
         dl : array_like
             Luminosity distance to the given redshift(s).  Units of [cm].
 
         """
+        if np.any(redz < 0):
+            raise ValueError(f"Number >= than 0 expected, got: {redz}")
         dl = self._interp(redz, self._grid_z, self._grid_dlum, self._sort_z)
         return dl
 
+    def z_to_dang(self, redz):
+        """Get the angular-diameter distance [cm] at the given redshift(s).
+
+        Parameters
+        ----------
+        redz : array_like,
+            Redshift ($z$) describing the distance/time of the universe. Unitless in [0.0, inf).
+
+        Returns
+        -------
+        da : array_like
+            Angular-diameter distance to the given redshift(s).  Units of [cm].
+
+        """
+        da = self._interp(redz, self._grid_z, self._grid_dang, self._sort_z)
+        return da
+
     def z_to_tage(self, redz):
         """Get the age of the universe [seconds] at the given redshift(s).
 
         Parameters
         ----------
         redz : array_like,
             Redshift ($z$) describing the distance/time of the universe. Unitless in [0.0, inf).
 
         Returns
         -------
         tage : array_like
             Age of the universe at the given redshift(s).  Units of [sec].
 
         """
+        if np.any(redz < 0):
+            raise ValueError(f"Number >= than 0 expected, got: {redz}")
         tage = self._interp(redz, self._grid_z, self._grid_age, self._sort_z)
         return tage
 
     def z_to_tlbk(self, redz):
         """Get the lookback time [seconds] at the given redshift(s).
 
         Parameters
@@ -362,14 +412,16 @@
 
         Returns
         -------
         tlook : array_like
             Lookback time to the universe at the given redshift(s).  Units of [sec].
 
         """
+        if np.any(redz < 0):
+            raise ValueError(f"Number >= than 0 expected, got: {redz}")
         zz = self._interp(redz, self._grid_z, self._grid_lbk, self._sort_z)
         return zz
 
     # ==== distance measures to a ====
 
     def dcom_to_a(self, dc):
         """Convert from comoving distance [cm] to scale-factor.
@@ -401,14 +453,31 @@
         scafa : array_like,
             Scale-factor ($a$) describing the distance/time of the universe. Unitless in (0.0, 1.0].
 
         """
         scafa = self._interp(dl, self._grid_dlum, self._grid_a, self._sort_dlum)
         return scafa
 
+    def dang_to_a(self, da):
+        """Convert from angular-diameter distance [cm] to scale-factor.
+
+        Parameters
+        ----------
+        da : array_like
+            Angular-diameter distance.  Units of [cm].
+
+        Returns
+        -------
+        scafa : array_like,
+            Scale-factor ($a$) describing the distance/time of the universe. Unitless in (0.0, 1.0].
+
+        """
+        scafa = self._interp(da, self._grid_dang, self._grid_a, self._sort_dang)
+        return scafa
+
     def tage_to_a(self, tage):
         """Convert from age of the universe [seconds] to scale-factor.
 
         Parameters
         ----------
         tage : array_like
             Age of the universe.  Units of [sec].
@@ -471,14 +540,31 @@
         redz : array_like,
             Redshift ($z$) describing the distance/time of the universe. Unitless in [0.0, inf).
 
         """
         zz = self._interp(dl, self._grid_dlum, self._grid_z, self._sort_dlum)
         return zz
 
+    def dang_to_z(self, da):
+        """Convert from angular-diameter distance [cm] to redshift.
+
+        Parameters
+        ----------
+        da : array_like
+            Angular-diameter distance.  Units of [cm].
+
+        Returns
+        -------
+        redz : array_like,
+            Redshift ($z$) describing the distance/time of the universe. Unitless in [0.0, inf).
+
+        """
+        zz = self._interp(da, self._grid_dang, self._grid_z, self._sort_dang)
+        return zz
+
     def tage_to_z(self, age):
         """Convert from age of the universe [seconds] to redshift.
 
         Parameters
         ----------
         tage : array_like
             Age of the universe.  Units of [sec].
```

### Comparing `cosmopy-3.5.5/cosmopy/tests/test_cosmology.py` & `cosmopy-3.6/cosmopy/tests/test_cosmology.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,20 +102,20 @@
             assert np.isclose(a, _a)
 
         # Test array input
         assert (np.allclose(Cosmology.z_to_a(zz), aa))
         assert (np.allclose(Cosmology.a_to_z(aa), zz))
 
         # Test out-of-domain errors
-        # with pytest.raises(ValueError):
-        #     Cosmology.a_to_z(-0.1)
-        # with pytest.raises(ValueError):
-        #     Cosmology.a_to_z(1.1)
-        # with pytest.raises(ValueError):
-        #     Cosmology.z_to_a(-0.2)
+        with pytest.raises(ValueError):
+            Cosmology.a_to_z(-0.1)
+        with pytest.raises(ValueError):
+            Cosmology.a_to_z(1.1)
+        with pytest.raises(ValueError):
+            Cosmology.z_to_a(-0.2)
 
         return
 
     def test_forward(self):
         """Test "forward" conversion from redshift to other parameters
         """
         from cosmopy.cosmology import Cosmology
```

### Comparing `cosmopy-3.5.5/cosmopy/tests/test_main.py` & `cosmopy-3.6/cosmopy/tests/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,17 @@
 
         args = ['dc', '423.1241Mpc']
         compare(args)
 
         args = ['dc', '0.4231241Gpc']
         compare(args)
 
+        args = ['da', '384.4342Mpc']
+        compare(args)
+
         return
 
     def test__calc_basic(self):
         from cosmopy.__main__ import calc_basic, _RESULTS_PARS, get_cosmology
         import argparse
 
         cosmo = get_cosmology()
```

### Comparing `cosmopy-3.5.5/cosmopy.egg-info/PKG-INFO` & `cosmopy-3.6/cosmopy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: cosmopy
-Version: 3.5.5
+Version: 3.6
 Home-page: https://github.com/lzkelley/cosmopy
-Download-URL: https://github.com/lzkelley/cosmopy/archive/v3.5.5.tar.gz
+Download-URL: https://github.com/lzkelley/cosmopy/archive/v3.6.tar.gz
 Author: Luke Zoltan Kelley
-Author-email: lzkelley@northwestern.edu
+Author-email: lzkelley@berkeley.edu
 License: MIT
 Keywords: utilities,physics,astronomy,cosmology,astrophysics,calculator
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: astropy
+Requires-Dist: future
+Requires-Dist: click
 
 cosmopy
 =======
 
 |version| |build-status| |coverage|
```

### Comparing `cosmopy-3.5.5/cosmopy.egg-info/SOURCES.txt` & `cosmopy-3.6/cosmopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/docs/Hinshaw+2013-NineYearWMAP_1212.5226v3.pdf` & `cosmopy-3.6/docs/Hinshaw+2013-NineYearWMAP_1212.5226v3.pdf`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/docs/Hogg99-DistanceMeasures_astroph9905116v4.pdf` & `cosmopy-3.6/docs/Hogg99-DistanceMeasures_astroph9905116v4.pdf`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/docs/Lahav&Liddle-CosmologicalParameters-2011.pdf` & `cosmopy-3.6/docs/Lahav&Liddle-CosmologicalParameters-2011.pdf`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/docs/cosmopy_demo.gif` & `cosmopy-3.6/docs/cosmopy_demo.gif`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/notebooks/test.ipynb` & `cosmopy-3.6/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `cosmopy-3.5.5/setup.py` & `cosmopy-3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open(FNAME_VERSION, "r") as inn:
     version = inn.read().strip()
 
 setup(
     name="cosmopy",
     author="Luke Zoltan Kelley",
-    author_email="lzkelley@northwestern.edu",
+    author_email="lzkelley@berkeley.edu",
     version=version,
     description="",
     license="MIT",
     url="https://github.com/lzkelley/cosmopy",
     download_url="https://github.com/lzkelley/cosmopy/archive/v{}.tar.gz".format(version),
     packages=['cosmopy'],
     entry_points={
@@ -29,9 +29,9 @@
         ]
     },
     include_package_data=True,
     install_requires=requirements,
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['utilities', 'physics', 'astronomy', 'cosmology', 'astrophysics', 'calculator'],
-    python_requires=">=3.5",
+    python_requires=">=3.8",
 )
```

