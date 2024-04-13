# Comparing `tmp/AstroToolkit-1.4.0.tar.gz` & `tmp/astrotoolkit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroToolkit-1.4.0.tar", last modified: Sat Apr  6 13:59:17 2024, max compression
+gzip compressed data, was "astrotoolkit-1.4.1.tar", last modified: Sat Apr 13 21:33:39 2024, max compression
```

## Comparing `AstroToolkit-1.4.0.tar` & `astrotoolkit-1.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.929451 AstroToolkit-1.4.0/
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/LICENSE
--rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 AstroToolkit-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    40407 2024-04-06 13:59:17.928451 AstroToolkit-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    39363 2024-04-06 00:56:04.000000 AstroToolkit-1.4.0/README.md
--rw-rw-rw-   0        0        0     1058 2024-04-06 13:58:43.000000 AstroToolkit-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 13:59:17.930451 AstroToolkit-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.738862 AstroToolkit-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.755423 AstroToolkit-1.4.0/src/AstroToolkit/
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.826170 AstroToolkit-1.4.0/src/AstroToolkit/Data/
--rw-rw-rw-   0        0        0    14952 2024-03-28 11:05:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/data.py
--rw-rw-rw-   0        0        0     6296 2024-04-05 17:18:50.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/imaging.py
--rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurve_sigma_clip.py
--rw-rw-rw-   0        0        0    23062 2024-04-05 17:22:00.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurves.py
--rw-rw-rw-   0        0        0    10534 2024-04-05 17:25:55.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/overlays.py
--rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/photometry.py
--rw-rw-rw-   0        0        0     2618 2024-04-05 17:44:53.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/reddening.py
--rw-rw-rw-   0        0        0     4300 2024-04-05 17:17:38.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/sed.py
--rw-rw-rw-   0        0        0     1978 2024-04-05 17:27:41.000000 AstroToolkit-1.4.0/src/AstroToolkit/Data/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.830217 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/
--rw-rw-rw-   0        0        0     2751 2024-04-05 17:28:09.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/buttons.py
--rw-rw-rw-   0        0        0     3785 2024-03-24 00:14:23.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/grid.py
--rw-rw-rw-   0        0        0     8244 2024-04-05 17:28:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Datapages/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.838219 AstroToolkit-1.4.0/src/AstroToolkit/Examples/
--rw-rw-rw-   0        0        0     3072 2024-04-06 09:17:47.000000 AstroToolkit-1.4.0/src/AstroToolkit/Examples/datapage_creation.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.848981 AstroToolkit-1.4.0/src/AstroToolkit/Misc/
--rw-rw-rw-   0        0        0     2388 2024-02-07 17:32:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/ProperMotionCorrection.py
--rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/coord_conversion.py
--rw-rw-rw-   0        0        0     1625 2024-04-05 17:29:14.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/database_queries.py
--rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_handling.py
--rw-rw-rw-   0        0        0     4308 2024-04-05 22:43:02.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_naming.py
--rw-rw-rw-   0        0        0     2937 2024-04-05 17:40:17.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/input_validation.py
--rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 AstroToolkit-1.4.0/src/AstroToolkit/Misc/read_fits.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.858984 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/
--rw-rw-rw-   0        0        0     4533 2024-04-05 22:49:09.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/HRD.py
--rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
--rw-rw-rw-   0        0        0     4576 2024-03-24 13:19:53.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/imaging.py
--rw-rw-rw-   0        0        0     5609 2024-03-23 23:37:51.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/lightcurves.py
--rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/powspec.py
--rw-rw-rw-   0        0        0     2629 2024-02-27 18:54:15.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/sed.py
--rw-rw-rw-   0        0        0     3676 2024-03-23 22:29:45.000000 AstroToolkit-1.4.0/src/AstroToolkit/Plotting/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.860984 AstroToolkit-1.4.0/src/AstroToolkit/Settings/
--rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 AstroToolkit-1.4.0/src/AstroToolkit/Settings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.926451 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/
--rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README - Windows.txt
--rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README.txt
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/__init__.py
--rw-rw-rw-   0        0        0   167936 2024-01-14 17:57:05.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.f90
--rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovconst.f90
--rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovsub.f90
--rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/build.sh
--rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/buildwin.bat
--rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.pdf
--rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.py
--rw-rw-rw-   0        0        0    31600 2024-04-02 12:42:59.000000 AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/ztfanalysis.py
--rw-rw-rw-   0        0        0    33302 2024-04-06 09:19:55.000000 AstroToolkit-1.4.0/src/AstroToolkit/Tools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 13:59:17.927451 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/
--rw-rw-rw-   0        0        0    40407 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1826 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-06 13:59:17.000000 AstroToolkit-1.4.0/src/AstroToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.853540 astrotoolkit-1.4.1/
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 astrotoolkit-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    38441 2024-04-13 21:33:39.852539 astrotoolkit-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    37520 2024-04-13 21:24:35.000000 astrotoolkit-1.4.1/README.md
+-rw-rw-rw-   0        0        0      968 2024-04-13 19:56:39.000000 astrotoolkit-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 21:33:39.853540 astrotoolkit-1.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.493459 astrotoolkit-1.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.507462 astrotoolkit-1.4.1/src/AstroToolkit/
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.638491 astrotoolkit-1.4.1/src/AstroToolkit/Data/
+-rw-rw-rw-   0        0        0    14934 2024-04-13 19:49:21.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/data.py
+-rw-rw-rw-   0        0        0     6345 2024-04-13 19:48:56.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/imaging.py
+-rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/lightcurve_sigma_clip.py
+-rw-rw-rw-   0        0        0    23062 2024-04-05 17:22:00.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/lightcurves.py
+-rw-rw-rw-   0        0        0    10513 2024-04-13 19:53:03.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/overlays.py
+-rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/photometry.py
+-rw-rw-rw-   0        0        0     2618 2024-04-05 17:44:53.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/reddening.py
+-rw-rw-rw-   0        0        0     4282 2024-04-13 19:53:18.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/sed.py
+-rw-rw-rw-   0        0        0     1978 2024-04-05 17:27:41.000000 astrotoolkit-1.4.1/src/AstroToolkit/Data/spectra.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.643493 astrotoolkit-1.4.1/src/AstroToolkit/Datapages/
+-rw-rw-rw-   0        0        0     2751 2024-04-05 17:28:09.000000 astrotoolkit-1.4.1/src/AstroToolkit/Datapages/buttons.py
+-rw-rw-rw-   0        0        0     3771 2024-04-13 19:53:32.000000 astrotoolkit-1.4.1/src/AstroToolkit/Datapages/grid.py
+-rw-rw-rw-   0        0        0     8223 2024-04-13 19:53:36.000000 astrotoolkit-1.4.1/src/AstroToolkit/Datapages/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.653494 astrotoolkit-1.4.1/src/AstroToolkit/Examples/
+-rw-rw-rw-   0        0        0     2844 2024-04-13 21:06:25.000000 astrotoolkit-1.4.1/src/AstroToolkit/Examples/datapage_creation.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.710507 astrotoolkit-1.4.1/src/AstroToolkit/Misc/
+-rw-rw-rw-   0        0        0     2364 2024-04-13 19:54:09.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/ProperMotionCorrection.py
+-rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/coord_conversion.py
+-rw-rw-rw-   0        0        0     1625 2024-04-05 17:29:14.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/database_queries.py
+-rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/file_handling.py
+-rw-rw-rw-   0        0        0     4308 2024-04-05 22:43:02.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/file_naming.py
+-rw-rw-rw-   0        0        0     2937 2024-04-05 17:40:17.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/input_validation.py
+-rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 astrotoolkit-1.4.1/src/AstroToolkit/Misc/read_fits.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.730511 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/
+-rw-rw-rw-   0        0        0     4489 2024-04-13 19:54:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/HRD.py
+-rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
+-rw-rw-rw-   0        0        0     4547 2024-04-13 19:55:04.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/imaging.py
+-rw-rw-rw-   0        0        0     5617 2024-04-13 20:13:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/lightcurves.py
+-rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/powspec.py
+-rw-rw-rw-   0        0        0     2636 2024-04-13 20:14:08.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/sed.py
+-rw-rw-rw-   0        0        0     3635 2024-04-13 19:55:43.000000 astrotoolkit-1.4.1/src/AstroToolkit/Plotting/spectra.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.731511 astrotoolkit-1.4.1/src/AstroToolkit/Settings/
+-rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 astrotoolkit-1.4.1/src/AstroToolkit/Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.848538 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/
+-rw-rw-rw-   0        0        0     3780 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/README - Windows.txt
+-rw-rw-rw-   0        0        0     3269 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/README.txt
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/__init__.py
+-rw-rw-rw-   0        0        0   167936 2024-04-13 19:06:19.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aov.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0    33000 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aov.f90
+-rw-rw-rw-   0        0        0      554 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aovconst.f90
+-rw-rw-rw-   0        0        0    36089 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aovsub.f90
+-rw-rw-rw-   0        0        0      577 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/build.sh
+-rwxrwxrwx   0        0        0      635 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/buildwin.bat
+-rw-rw-rw-   0        0        0   256433 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/pyaov.pdf
+-rw-rw-rw-   0        0        0    24550 2024-01-11 16:40:26.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/pyaov.py
+-rw-rw-rw-   0        0        0    31600 2024-04-02 12:42:59.000000 astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/ztfanalysis.py
+-rw-rw-rw-   0        0        0    32053 2024-04-13 20:28:43.000000 astrotoolkit-1.4.1/src/AstroToolkit/Tools.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:33:39.850538 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/
+-rw-rw-rw-   0        0        0    38441 2024-04-13 21:33:39.000000 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-04-13 21:33:39.000000 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 21:33:39.000000 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2024-04-13 21:33:39.000000 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 21:33:39.000000 astrotoolkit-1.4.1/src/AstroToolkit.egg-info/top_level.txt
```

### Comparing `AstroToolkit-1.4.0/PKG-INFO` & `astrotoolkit-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: AstroToolkit
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for the gathering and plotting of astronomical data.
 Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
 Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: astropy==5.2.2
+Requires-Dist: astropy==6.0.1
 Requires-Dist: astroquery==0.4.7
-Requires-Dist: bokeh==3.1.1
-Requires-Dist: cmasher==1.6.3
+Requires-Dist: bokeh==3.4.1
+Requires-Dist: cmasher==1.8.0
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: importlib_resources==6.4.0
-Requires-Dist: matplotlib==3.7.5
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.24.4
-Requires-Dist: pandas==2.0.3
-Requires-Dist: Pillow==10.2.0
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: PyQt5_sip==12.13.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: pandas==2.2.2
 Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn==1.3.2
-Requires-Dist: scipy==1.10.1
 Requires-Dist: selenium==4.17.2
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: scipy==1.13.0
 
 # AstroToolkit
 
 AstroToolkit (ATK) is a set of tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
 
@@ -596,15 +592,15 @@
 
 <br>
 
 **Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
+**Supported plot types:** image, lightcurve, sed, spectra, hrd
 
 <br>
 
 Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
 <br>
 
@@ -616,18 +612,14 @@
 
 [SED Plotting](#23-sed-plotting)
 
 [Spectrum Plotting](#24-spectrum-plotting)
 
 [HRD Plotting](#25-hrd-plotting)
 
-[Power Spectra Plotting](#26-power-spectra-plotting)
-
-<br>
-
 ### 2.1 Image Plotting<a id="21-image-plotting"></a>
 
 Type argument: 'image'
 
 Description: Plots images in format returned by [image queries](#15-imaging-query).
 
 <br>
@@ -746,57 +738,14 @@
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
 <br><br>
 
-### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
-
-Type argument: 'powspec'
-
-Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Returns:** dict
-
-```
-{
-'type' : 'powspec'
-'survey' : str, survey of lightcurve data given to the powspec tool
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-<br><br>
-
-### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
-
-Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Usage:**
-
-```
-tsanalysis(data)
-```
-
-where:
-
-```
-data = dict or list in format returned by lightcurve queries
-```
-
-<br><br>
-
 ## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
@@ -1434,74 +1383,48 @@
 showplot(plot)
 ```
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
 
 <br><br>
 
-### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
-
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
-<br><br>
-
-### Example 7: Fetching Gaia parallax and WISE data
+### Example 6: Fetching Gaia parallax and WISE data
 
 ```
 from AstroToolkit.Tools import query
 
 source = 6050296829033196032
 
 parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
 wise_data = query(type='data',survey='wise',source=source)['data']
 ```
 
-### Example 8: Fetching 2MASS photometry for an object
+### Example 7: Fetching 2MASS photometry for an object
 
 ```
 from AstroToolkit.Tools import query
 
 data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
 ```
 
-### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+### Example 8: Fetching photometry from all available surveys using a bulk photometry query
 
 ```
 from AstroToolkit.Tools import query
 
 bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
 
 gaia_data=bulk_phot['gaia']
 galex_data=bulk_phot['galex']
 ```
 
 <br><br>
 
-### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
-
-```
-from AstroToolkit.Tools import query,tsanalysis
-
-data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
-<br><br>
 
-### Example 11: Proper motion correction
+### Example 9: Proper motion correction
 
 ```
 from AstroToolkit.Tools import query,correctpm
 
 gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
 ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
```

### Comparing `AstroToolkit-1.4.0/README.md` & `astrotoolkit-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -567,15 +567,15 @@
 
 <br>
 
 **Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
+**Supported plot types:** image, lightcurve, sed, spectra, hrd
 
 <br>
 
 Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
 <br>
 
@@ -587,18 +587,14 @@
 
 [SED Plotting](#23-sed-plotting)
 
 [Spectrum Plotting](#24-spectrum-plotting)
 
 [HRD Plotting](#25-hrd-plotting)
 
-[Power Spectra Plotting](#26-power-spectra-plotting)
-
-<br>
-
 ### 2.1 Image Plotting<a id="21-image-plotting"></a>
 
 Type argument: 'image'
 
 Description: Plots images in format returned by [image queries](#15-imaging-query).
 
 <br>
@@ -717,57 +713,14 @@
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
 <br><br>
 
-### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
-
-Type argument: 'powspec'
-
-Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Returns:** dict
-
-```
-{
-'type' : 'powspec'
-'survey' : str, survey of lightcurve data given to the powspec tool
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-<br><br>
-
-### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
-
-Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Usage:**
-
-```
-tsanalysis(data)
-```
-
-where:
-
-```
-data = dict or list in format returned by lightcurve queries
-```
-
-<br><br>
-
 ## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
@@ -1405,74 +1358,48 @@
 showplot(plot)
 ```
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
 
 <br><br>
 
-### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
-
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
-<br><br>
-
-### Example 7: Fetching Gaia parallax and WISE data
+### Example 6: Fetching Gaia parallax and WISE data
 
 ```
 from AstroToolkit.Tools import query
 
 source = 6050296829033196032
 
 parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
 wise_data = query(type='data',survey='wise',source=source)['data']
 ```
 
-### Example 8: Fetching 2MASS photometry for an object
+### Example 7: Fetching 2MASS photometry for an object
 
 ```
 from AstroToolkit.Tools import query
 
 data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
 ```
 
-### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+### Example 8: Fetching photometry from all available surveys using a bulk photometry query
 
 ```
 from AstroToolkit.Tools import query
 
 bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
 
 gaia_data=bulk_phot['gaia']
 galex_data=bulk_phot['galex']
 ```
 
 <br><br>
 
-### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
-
-```
-from AstroToolkit.Tools import query,tsanalysis
-
-data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
-<br><br>
 
-### Example 11: Proper motion correction
+### Example 9: Proper motion correction
 
 ```
 from AstroToolkit.Tools import query,correctpm
 
 gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
 ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
```

### Comparing `AstroToolkit-1.4.0/pyproject.toml` & `astrotoolkit-1.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,40 +3,36 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "AstroToolkit"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Ethan Moorfield", email="ethan.moorfield@hotmail.co.uk"},
 ]
 description = "A package for the gathering and plotting of astronomical data."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "astropy==5.2.2",
+    "astropy==6.0.1",
     "astroquery==0.4.7",
-    "bokeh==3.1.1",
-    "cmasher==1.6.3",
+    "bokeh==3.4.1",
+    "cmasher==1.8.0",
+    "matplotlib==3.8.4",
     "importlib_resources==6.4.0",
-    "matplotlib==3.7.5",
-    "numba==0.58.1",
-    "numpy==1.24.4",
-    "pandas==2.0.3",
-    "Pillow==10.2.0",
-    "PyQt5==5.15.10",
-    "PyQt5_sip==12.13.0",
+    "numpy==1.26.4",
+    "pandas==2.2.2",
     "Requests==2.31.0",
-    "scikit_learn==1.3.2",
-    "scipy==1.10.1",
-    "selenium==4.17.2"
+    "selenium==4.17.2",
+    "beautifulsoup4==4.12.3",
+    "scipy==1.13.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/WD-planets/AstroToolkit"
 Issues = "https://github.com/WD-planets/AstroToolkit/issues"
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/data.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import astropy.coordinates as coord
 import astropy.units as u
 import requests
 from io import BytesIO
 import pandas as pd
 import warnings
 import xml.etree.ElementTree as ET
-import itertools
 
 from ..Misc.ProperMotionCorrection import PMCorrection
 
 # ignores a pandas warning about some columns being duplicated in returned data and therefore omitted
 warnings.simplefilter(action='ignore', category=UserWarning)
 
 # ensure that the row limit in returned data is infinite
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/imaging.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/imaging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-from tkinter import W
 from astropy.table import Table
 from astropy.io import fits
-import astropy
 from astropy.visualization import PercentileInterval, AsinhStretch
 from astropy.wcs import WCS
-import PIL
-from PIL import Image
 from io import BytesIO
 import numpy as np
 import requests
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 import pandas as pd
 from astropy.time import Time
@@ -30,15 +26,15 @@
 	ra,dec=location[0],location[1]
 
 	if survey=='panstarrs':
 		# convert size to pixel size
 		url_size=size*4
 		service='https://ps1images.stsci.edu/cgi-bin/ps1filenames.py'
 		url=f'{service}?ra={ra}&dec={dec}&band={band}'
-	
+
 		# get table of returned image filenames
 		try:
 			table=Table.read(url, format='ascii')
 		except:
 			print(f'Note: Experiencing issues with {survey}.')
 			return failed_search()
 		
@@ -85,17 +81,22 @@
 		# convert size to pixel size
 		url_size=size/60
 		
 		service='http://archive.stsci.edu/cgi-bin/dss_search'
 		urlMain=f'{service}?ra={ra}&d={dec}&v=3&e=J2000&f=fits&h={url_size}&w={url_size}'
 
 	# send request using the URL returned for the selected survey
-	r=requests.get(urlMain,timeout=15)
+	try:
+		r=requests.get(urlMain,timeout=15)
+	except:
+		print(f'Note: Experiencing issues with {survey}.')
+		return failed_search()
 	if r.status_code!=200:
 		print(f'Note: Experiencing issues with {survey}.')
+		return failed_search()
 
 	try:
 		fh=fits.open(BytesIO(r.content))
 	except:
 		print(f'Note: No data returned from {survey} imagequery.')
 		return failed_search()
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurve_sigma_clip.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/lightcurve_sigma_clip.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/lightcurves.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/lightcurves.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/overlays.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/overlays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pandas as pd
 import math
 
 from ..Misc.ProperMotionCorrection import PMCorrection
 from ..Misc.ProperMotionCorrection import get_adapted_radius
 from ..Tools import query
 from ..Data.data import get_survey_times
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/photometry.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/photometry.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/reddening.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/reddening.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/sed.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/sed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from re import S
 import astropy.units as u
 import numpy as np
 import pandas as pd
 
 from ..Tools import query
 from .data import get_survey_times
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Data/spectra.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Data/spectra.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/buttons.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Datapages/buttons.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/grid.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Datapages/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bokeh.plotting import figure
 from bokeh.models import Label, Range1d
-import bokeh
 
 def get_grid(dimensions,plots,grid_size=250):
 	# Calculates the area occupied by the input plots (i.e. just normalized by /grid_size)
 	unit_area=0
 	for i,plot_info_dict in enumerate(plots):
 		keys=list(plot_info_dict.keys())
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Datapages/metadata.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Datapages/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from bokeh.models import ColumnDataSource,DataTable,TableColumn
-import pandas as pd
 
 from ..Tools import query
 from ..Data.data import get_survey_list
 
 '''
 appends data points to the lists in list_dict
 '''
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Examples/datapage_creation.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Examples/datapage_creation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from AstroToolkit.Tools import query,plot,getbuttons,gridsetup,getmdtable,showplot
+from AstroToolkit.Tools import query,plot,getbuttons,gridsetup,getmdtable,showplot,export
 from bokeh.layouts import column,row,layout
 from bokeh.plotting import output_file
+import chromedriver_binary
 
 # source = Hu Leo
-#source=2552928187080872832
 source=587316166180416640
 
 # set grid size (scales overally size of datapage)
 grid_size=275
 
 # get image data and plot it
 image_data=query(type='image',survey='any',source=source,overlays='gaia,galex_nuv,galex_fuv')
@@ -27,17 +27,14 @@
 
 # get lightcurve data [g,r,i]
 lightcurve_data=query(type='lightcurve',survey='ztf',source=source)
 
 # plot each lightcurve in lightcurve_data and set colour of each plot
 lightcurves=plot(lightcurve_data,colours=['green','red','blue'])
 
-# plot power spectrum data (lightcurve_data)
-power_spectrum=plot(lightcurve_data,type='powspec',)
-
 # get SIMBAD and Vizier buttons
 buttons=getbuttons(grid_size=grid_size,source=source)
 
 # make a custom metadatatable entry
 custom_entry={
     'parameters':['one'],
     'values':['two'],
@@ -50,22 +47,22 @@
 
 # get plots, formatted into grid dimensions
 grid_plots=gridsetup(dimensions={'width':6,'height':5},plots=[{'name':'image','figure':image,'width':2,'height':2},
                                                               {'name':'hrd','figure':hrd,'width':2,'height':2},
                                                               {'name':'sed','figure':sed,'width':2,'height':1},
                                                               {'name':'lightcurves','figure':lightcurves,'width':2,'height':1},
                                                               {'name':'buttons','figure':buttons,'width':1,'height':1},
-                                                              {'name':'spectrum','figure':spectrum,'width':3,'height':1},
-                                                              {'name':'powspec','figure':power_spectrum,'width':2,'height':1},
+                                                              {'name':'spectrum','figure':spectrum,'width':5,'height':1},
                                                               {'name':'metadata_table','figure':metadata,'width':6,'height':2}],
                                                               grid_size=grid_size)
 
 # set up the final grid
 datapage=layout(column(
                 row(grid_plots['image'],grid_plots['hrd'],column(grid_plots['sed'],grid_plots['lightcurves'])),
-                row(grid_plots['buttons'],grid_plots['spectrum'],grid_plots['powspec']),
+                row(grid_plots['buttons'],grid_plots['spectrum']),
                 row(grid_plots['metadata_table'])
 	            ))
 
 output_file(f'{source}_datapage.html')
 
-showplot(datapage)
+showplot(datapage)
+export(datapage)
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/ProperMotionCorrection.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/ProperMotionCorrection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from calendar import c
 import math
 
 '''
 Takes an input year in format [year,month] and corrects coordinates of an object (using its pmra and pmdec) to correct for its proper motion to a target year in format [year,month]
 '''
 def PMCorrection(input,target,ra,dec,pmra,pmdec):
 	# Filter inputs
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/coord_conversion.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/coord_conversion.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/database_queries.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/database_queries.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_handling.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/file_handling.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/file_naming.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/file_naming.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/input_validation.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/input_validation.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Misc/read_fits.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Misc/read_fits.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/HRD.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/HRD.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from astropy.table import Table
-import matplotlib.pyplot as plt
 import numpy as np
 from scipy import stats
 import math
 import cmasher as cmr
 from bokeh.plotting import figure
-import os
 from importlib_resources import files
 from bokeh.models import CustomJS
 from bokeh import events
 
 from ..Tools import query
 
 fits_file = files('AstroToolkit.Plotting').joinpath('backdrop_hrd_allmags.fits')
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/imaging.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bokeh.models import Range1d, CustomJS
-import astropy
 import numpy as np
-from bokeh.plotting import figure, output_file
+from bokeh.plotting import figure
 from bokeh import events
 
 def plot_image(image_dict):
 	if image_dict['data']==None:
 		print('Note: None object passed to plotimage, suggests no image was found.')
 		return None
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/lightcurves.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/lightcurves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib
 import numpy as np
 from bokeh.plotting import figure
-from bokeh.models import Whisker, ColumnDataSource
+from bokeh.models import ColumnDataSource
 from bokeh.transform import linear_cmap
 from bokeh.models import CustomJS
 from bokeh import events
 
 def plot_lightcurve(data,colour,colours):
 	if isinstance(data,dict):
 		if data['data']==None:
@@ -104,15 +104,15 @@
 
 		# set up data source
 		source=ColumnDataSource(data=dict(time=time,mag=mag))
 
 		mapper=linear_cmap(field_name='mag',palette=palette,low=min(mag),high=max(mag))
 
 		# plot points
-		plot.circle(x='time',y='mag',source=source,color=mapper,legend_label=f"{data_dict['survey']} {data_dict['band']}")
+		plot.scatter(x='time',y='mag',source=source,color=mapper,marker='circle',legend_label=f"{data_dict['survey']} {data_dict['band']}")
 
 		# plot error bars
 		err_xs=[]
 		err_ys=[]
 		for x,y,y_err in zip(time,mag,mag_err):
 			err_xs.append((x,x))
 			err_ys.append((y-y_err,y+y_err))
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/powspec.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/powspec.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/sed.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/sed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bokeh.plotting import figure
-from bokeh.models import Whisker, ColumnDataSource, CustomJS, PrintfTickFormatter
+from bokeh.models import CustomJS, PrintfTickFormatter
 from bokeh import events
 import math
 
 
 def plot_sed(sed_data):
     if sed_data==None:
         print('Note: None object passed to plotsed, suggests no SED data was found.')
@@ -43,17 +43,17 @@
             err_ys.append((y-y_err,y+y_err))
         
         current_survey_index=survey_list.index(survey)
 
         # plot data
         for i,v in enumerate(x_arr):
             if not math.isnan(err_arr[i]):
-                plot.circle(x=x_arr[i],y=y_arr[i],color=colour_arr[current_survey_index],legend_label=f'{survey}')
+                plot.scatter(x=x_arr[i],y=y_arr[i],color=colour_arr[current_survey_index],marker='circle',legend_label=f'{survey}')
             else:
-                plot.cross(x=x_arr[i],y=y_arr[i],color=colour_arr[current_survey_index],legend_label=f'{survey} (Upper Limit)',size=7.5)
+                plot.scatter(x=x_arr[i],y=y_arr[i],color=colour_arr[current_survey_index],marker='cross',legend_label=f'{survey} (Upper Limit)',size=7.5)
            
         # plot errors
         plot.multi_line(err_xs,err_ys,color=colour_arr[current_survey_index],legend_label=f'{survey}',level='underlay',line_width=0.5,line_cap='square')
         
         legend=True
 
     plot.xaxis[0].formatter = PrintfTickFormatter(format="%0e")
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Plotting/spectra.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Plotting/spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import pandas as pd
 from bokeh.plotting import figure
 from bokeh.models import Span, CheckboxGroup, CustomJS, Label, Range1d
-from bokeh.layouts import row,column
+from bokeh.layouts import row
 from bokeh.models import PrintfTickFormatter
 from bokeh import events
-import math
 
 def get_plot(spectrum_dict):
 	if spectrum_dict['data']==None:
 		print('Note: None object passed to plotspectrum, suggests no spectrum was found.')
 		return None	
 
 	x=spectrum_dict['data']['wavelength']
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README - Windows.txt` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/README - Windows.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/README.txt` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/README.txt`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aov.f90` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aov.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovconst.f90` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aovconst.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/aovsub.f90` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/aovsub.f90`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/build.sh` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/build.sh`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/buildwin.bat` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/buildwin.bat`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.pdf` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/pyaov.pdf`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/pyaov.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/pyaov.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Timeseries/ztfanalysis.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Timeseries/ztfanalysis.py`

 * *Files identical despite different names*

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit/Tools.py` & `astrotoolkit-1.4.1/src/AstroToolkit/Tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 - Updated hrd plotting to fit the query/plot tools
 - Updated datapage_creation example for new functionality
 '''
 
 '''
 To-Do:
 HIGH PRIORITY
+- look into plotly
+- astropy readfits warnings
 - Better scaling for detection overlay sizes
 - check config for if all keys are present, if not then make a new config file with existing key:value pairs saved
 - talk to boris about combining lightcurves
 - update README to reflect new changes (plots stored as dictionaries, showplot/saveplot/export now required to use on ATK plot objects, updated grid functionality)
   
 MEDIUM PRIORITY
 - add defaults for newly supported surveys to metadata table
@@ -43,14 +45,49 @@
 
 newline='\n'
 
 # Configuration -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 config_file=files('AstroToolkit.Settings').joinpath('config.ini')	
 
+# Read config file
+def readconfig():
+	Config=configparser.ConfigParser()
+	Config.read(config_file)
+
+	settings=Config['settings']
+	for key in settings:
+		if settings[key]=='True':
+			settings[key]='1'
+		elif settings[key]=='False':
+			settings[key]='0'
+
+	config={}		
+
+	# set up dictionary with key:value pairs of the config file
+	config['ENABLE_NOTIFICATIONS']=int(settings['enable_notifications'])
+	config['DATAQUERY_RADIUS']=float(settings['dataquery_radius'])
+	config['PHOTQUERY_RADIUS']=float(settings['photquery_radius'])
+	config['BULKPHOTQUERY_RADIUS']=float(settings['bulkphotquery_radius'])
+	config['IMAGEQUERY_SIZE']=float(settings['imagequery_size'])
+	config['IMAGEQUERY_OVERLAYS']=str(settings['imagequery_overlays'])
+	config['LIGHTCURVEQUERY_RADIUS']=float(settings['lightcurvequery_radius'])
+	config['ATLAS_USERNAME']=str(settings['atlas_username'])
+	config['ATLAS_PASSWORD']=str(settings['atlas_password'])
+	config['SED_RADIUS']=float(settings['sed_radius'])
+	config['SPECTRUM_RADIUS']=float(settings['spectrum_radius'])
+	config['GRID_SIZE']=int(settings['grid_size'])
+	config['SIMBAD_RADIUS']=int(settings['button_simbad_radius'])
+	config['VIZIER_RADIUS']=int(settings['button_vizier_radius'])
+	config['PLOT_SIZE']=int(settings['plot_size'])
+	config['READFITS_SOURCENAME']=str(settings['readfits_sourcename'])
+	config['READFITS_COORDNAMES']=str(settings['readfits_coordnames']).split(',')
+	
+	return config
+
 # Create default config file if the file doesn't already exist (i.e. when the package is first installed)
 # This handles all default parameters unless they are passed to a tool by the user, in which case these are overwritten
 if not os.path.isfile(config_file):
 	config=configparser.ConfigParser()
 
 	config.add_section('settings')
 	config.set('settings','enable_notifications','True')
@@ -69,14 +106,16 @@
 	config.set('settings','button_vizier_radius','3')
 	config.set('settings','plot_size','400')
 	config.set('settings','readfits_sourcename','source_id')
 	config.set('settings','readfits_coordnames','ra,dec')
 
 	with open(config_file,'w') as configfile:
 		config.write(configfile)
+else:
+	existing_values=readconfig()
 
 # allows user to edit the config file
 def editconfig(options):
 	edit=configparser.ConfigParser()
 	edit.read(config_file)
 	settings=edit['settings']		
 
@@ -86,49 +125,14 @@
 		if key not in accepted_keys:
 			raise Exception(f'Invalid configuration parameter. Accepted parameters are {accepted_keys}.')
 	
 		settings[key]=str(options[key])
 		
 	with open(config_file,'w') as configfile:
 		edit.write(configfile)
-	
-# Read config file
-def readconfig():
-	Config=configparser.ConfigParser()
-	Config.read(config_file)
-
-	settings=Config['settings']
-	for key in settings:
-		if settings[key]=='True':
-			settings[key]='1'
-		elif settings[key]=='False':
-			settings[key]='0'
-
-	config={}		
-
-	# set up dictionary with key:value pairs of the config file
-	config['ENABLE_NOTIFICATIONS']=int(settings['enable_notifications'])
-	config['DATAQUERY_RADIUS']=float(settings['dataquery_radius'])
-	config['PHOTQUERY_RADIUS']=float(settings['photquery_radius'])
-	config['BULKPHOTQUERY_RADIUS']=float(settings['bulkphotquery_radius'])
-	config['IMAGEQUERY_SIZE']=float(settings['imagequery_size'])
-	config['IMAGEQUERY_OVERLAYS']=str(settings['imagequery_overlays'])
-	config['LIGHTCURVEQUERY_RADIUS']=float(settings['lightcurvequery_radius'])
-	config['ATLAS_USERNAME']=str(settings['atlas_username'])
-	config['ATLAS_PASSWORD']=str(settings['atlas_password'])
-	config['SED_RADIUS']=float(settings['sed_radius'])
-	config['SPECTRUM_RADIUS']=float(settings['spectrum_radius'])
-	config['GRID_SIZE']=int(settings['grid_size'])
-	config['SIMBAD_RADIUS']=int(settings['button_simbad_radius'])
-	config['VIZIER_RADIUS']=int(settings['button_vizier_radius'])
-	config['PLOT_SIZE']=int(settings['plot_size'])
-	config['READFITS_SOURCENAME']=str(settings['readfits_sourcename'])
-	config['READFITS_COORDNAMES']=str(settings['readfits_coordnames']).split(',')
-	
-	return config
 
 # prints the current value of a given config parameter to the terminal, and returns it
 def getconfigvalue(parameter):
 	config=readconfig()
 
 	# make parameters returned by readconfig lower case to match the config file
 	accepted_parameters=list(config.keys())
@@ -447,15 +451,15 @@
 		
 
 # Plotting ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def plot(data,type=None,colour='black',colours=None):
 	config=readconfig()
 
-	accepted_types=['image','lightcurve','sed','spectra','powspec','hrd']
+	accepted_types=['image','lightcurve','sed','spectra','hrd']
 
 	if colour!='black':
 		print('Note: argument "colour" only has an effect in lightcurve plotting.')
 	if colours!=None:
 		print('Note: argument "colours" only has an effect in lightcurve plotting.')
 
 	# if a type is not given, try to find the data type
@@ -601,48 +605,14 @@
 		else:
 			filename=None
 
 		plot_dict={'type':'spectra','survey':data['survey'],'source':data['source'],'pos':data['pos'],'plot':plot,'ATKfilename':filename}
 
 		return plot_dict
 	
-
-	elif type=='powspec':
-		import copy
-		
-		from .Plotting.powspec import get_plot
-	
-		# stops data from being flattened by the powspec plotting
-		data_copy=copy.deepcopy(data)
-
-		plot=get_plot(dataset=data_copy)
-
-		if plot!=None:
-			# name file
-			filename=name_file(data=data,data_type='ATKpowspec')
-			output_file(filename)
-		
-			# set size of file according to defaults in config
-			plot.width,plot.height=config['PLOT_SIZE']*2,config['PLOT_SIZE']
-		else:
-			filename=None
-
-		plot_dict={'type':'powspec'}
-		for i,val in enumerate(data):
-			if val!=None:
-				plot_dict['survey']=val['survey']
-				plot_dict['source']=val['source']
-				plot_dict['pos']=val['pos']
-
-		plot_dict['plot']=plot
-		plot_dict['ATKfilename']=filename
-
-		return plot_dict
-	
-
 	elif type=='hrd':
 		from .Plotting.HRD import get_plot
 
 		plot=get_plot(data)
 
 		if plot!=None:
 			# name file
@@ -654,28 +624,14 @@
 		else:
 			filename=None
 
 		plot_dict={'sources':data['sources'],'type':'hrd','plot':plot,'ATKfilename':filename}
 		
 		return plot_dict
 
-# Timeseries --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-def tsanalysis(data):
-	config=readconfig()
-
-	# enables notifications of currently running tool if enabled in config
-	if config['ENABLE_NOTIFICATIONS']==1:
-		print(f'Running time series analysis...{newline}')	
-
-	from .Timeseries.ztfanalysis import get_analysis
-	
-	# load timeseries analysis tool
-	get_analysis(dataset=data)
-
 # Data Pages --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def gridsetup(dimensions,plots,grid_size=None):
 	config=readconfig()
 	
 	# sets the grid size to the default given in config if one isn't supplied
 	if grid_size==None:
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit.egg-info/PKG-INFO` & `astrotoolkit-1.4.1/src/AstroToolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: AstroToolkit
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for the gathering and plotting of astronomical data.
 Author-email: Ethan Moorfield <ethan.moorfield@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/WD-planets/AstroToolkit
 Project-URL: Issues, https://github.com/WD-planets/AstroToolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: astropy==5.2.2
+Requires-Dist: astropy==6.0.1
 Requires-Dist: astroquery==0.4.7
-Requires-Dist: bokeh==3.1.1
-Requires-Dist: cmasher==1.6.3
+Requires-Dist: bokeh==3.4.1
+Requires-Dist: cmasher==1.8.0
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: importlib_resources==6.4.0
-Requires-Dist: matplotlib==3.7.5
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.24.4
-Requires-Dist: pandas==2.0.3
-Requires-Dist: Pillow==10.2.0
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: PyQt5_sip==12.13.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: pandas==2.2.2
 Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn==1.3.2
-Requires-Dist: scipy==1.10.1
 Requires-Dist: selenium==4.17.2
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: scipy==1.13.0
 
 # AstroToolkit
 
 AstroToolkit (ATK) is a set of tools for fetching, plotting, and analysing astronomical data.
 
 ## Table of Contents
 
@@ -596,15 +592,15 @@
 
 <br>
 
 **Note:** If no plot is returned, the 'plot' key of the returned dictionary will be set to None.
 
 <br>
 
-**Supported plot types:** image, lightcurve, sed, spectra, powspec, hrd
+**Supported plot types:** image, lightcurve, sed, spectra, hrd
 
 <br>
 
 Below is an outline of the usage and output of each plot type. Note that additonal arguments not listed above may be used, see individual plot types below for details.
 
 <br>
 
@@ -616,18 +612,14 @@
 
 [SED Plotting](#23-sed-plotting)
 
 [Spectrum Plotting](#24-spectrum-plotting)
 
 [HRD Plotting](#25-hrd-plotting)
 
-[Power Spectra Plotting](#26-power-spectra-plotting)
-
-<br>
-
 ### 2.1 Image Plotting<a id="21-image-plotting"></a>
 
 Type argument: 'image'
 
 Description: Plots images in format returned by [image queries](#15-imaging-query).
 
 <br>
@@ -746,57 +738,14 @@
 'plot' : bokeh figure object, the actual plot
 'ATKfilename' : the default filename given by ATK
 }
 ```
 
 <br><br>
 
-### 2.6 Power Spectra Plotting<a id="26-power-spectra-plotting"></a>
-
-Type argument: 'powspec'
-
-Description: Plots power spectra from lightcurve data in the format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Returns:** dict
-
-```
-{
-'type' : 'powspec'
-'survey' : str, survey of lightcurve data given to the powspec tool
-'source' : int/str, source used to get data (None if a pos was used)
-'pos': [ra,dec], pos used to get data (None if a source was used)
-'plot' : bokeh figure object, the actual plot
-'ATKfilename' : the default filename given by ATK
-}
-```
-
-<br><br>
-
-### 2.7 Timeseries Analysis<a id="27-timeseries-analysis"></a>
-
-Description: Not explicitly a plotting function, but included here for completeness. Runs period analysis on lightcurve data in format returned by [lightcurve queries](#16-lightcurve-query).
-
-<br>
-
-**Usage:**
-
-```
-tsanalysis(data)
-```
-
-where:
-
-```
-data = dict or list in format returned by lightcurve queries
-```
-
-<br><br>
-
 ## 3. Datapage Tools<a id="3-datapage-tools"></a>
 
 These functions are used to create custom datapages from any plots/data supported by AstroToolkit.
 
 **NOTE:** An example of datapage creation can be found within the packages 'Examples' folder, named 'datapage_creation.py' (within the …/Lib/site-packages/AstroToolkit from earlier). This can be imported from a python terminal using from AstroToolkit.Examples import datapage_creation.
 
 Below is the datapage produced by this example. Once the script to create these has been written, they can be a very powerful way to quickly retrieve and show a wide range of information on a system, with the below example easily being generated in under 30s.
@@ -1434,74 +1383,48 @@
 showplot(plot)
 ```
 
 ![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/spectrum_example.png?raw=true)
 
 <br><br>
 
-### Example 6: Fetching ZTF ligthcurve data, and then plotting it as a power spectrum
-
-```
-from AstroToolkit.Tools import lightcurvequery,plotpowspec,showplot
-
-data=lightcurvequery(survey='ztf',source=6050296829033196032)
-plot=plotpowspec(data)
-showplot(plot)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/powspec_example.png?raw=true)
-
-<br><br>
-
-### Example 7: Fetching Gaia parallax and WISE data
+### Example 6: Fetching Gaia parallax and WISE data
 
 ```
 from AstroToolkit.Tools import query
 
 source = 6050296829033196032
 
 parallax = query(type='data',survey='gaia',source=source)['data']['parallax']
 wise_data = query(type='data',survey='wise',source=source)['data']
 ```
 
-### Example 8: Fetching 2MASS photometry for an object
+### Example 7: Fetching 2MASS photometry for an object
 
 ```
 from AstroToolkit.Tools import query
 
 data=query(type='phot',survey='twomass',source=6050296829033196032)['data']
 ```
 
-### Example 9: Fetching photometry from all available surveys using a bulk photometry query
+### Example 8: Fetching photometry from all available surveys using a bulk photometry query
 
 ```
 from AstroToolkit.Tools import query
 
 bulk_phot=query(type='bulkphot',source=6050296829033196032)['data']
 
 gaia_data=bulk_phot['gaia']
 galex_data=bulk_phot['galex']
 ```
 
 <br><br>
 
-### Example 10: Fetching ZTF lightcurve data, and performing timeseries analysis
-
-```
-from AstroToolkit.Tools import query,tsanalysis
-
-data=query(type='lightcurve',survey='ztf',source=6050296829033196032)
-plot=tsanalysis(data)
-```
-
-![](https://github.com/WD-planets/AstroToolkit/raw/latest/README_Images/tsanalysis_example.png?raw=true)
-
-<br><br>
 
-### Example 11: Proper motion correction
+### Example 9: Proper motion correction
 
 ```
 from AstroToolkit.Tools import query,correctpm
 
 gaia_data=query(type='data',survey='gaia',source=6050296829033196032)['data']
 ra,dec,pmra,pmdec=gaia_data['ra'][0],gaia_data['dec'][0],gaia_data['pmra'][0],gaia_data['pmdec'][0]
```

### Comparing `AstroToolkit-1.4.0/src/AstroToolkit.egg-info/SOURCES.txt` & `astrotoolkit-1.4.1/src/AstroToolkit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 src/AstroToolkit/Plotting/powspec.py
 src/AstroToolkit/Plotting/sed.py
 src/AstroToolkit/Plotting/spectra.py
 src/AstroToolkit/Settings/__init__.py
 src/AstroToolkit/Timeseries/README - Windows.txt
 src/AstroToolkit/Timeseries/README.txt
 src/AstroToolkit/Timeseries/__init__.py
-src/AstroToolkit/Timeseries/aov.cp38-win_amd64.pyd
+src/AstroToolkit/Timeseries/aov.cp311-win_amd64.pyd
 src/AstroToolkit/Timeseries/aov.f90
 src/AstroToolkit/Timeseries/aovconst.f90
 src/AstroToolkit/Timeseries/aovsub.f90
 src/AstroToolkit/Timeseries/build.sh
 src/AstroToolkit/Timeseries/buildwin.bat
 src/AstroToolkit/Timeseries/pyaov.pdf
 src/AstroToolkit/Timeseries/pyaov.py
```

