# Comparing `tmp/EllipSect-3.2.3.tar.gz` & `tmp/EllipSect-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EllipSect-3.2.3.tar", last modified: Tue May 16 22:37:19 2023, max compression
+gzip compressed data, was "EllipSect-3.4.0.tar", last modified: Sat Apr 13 01:31:39 2024, max compression
```

## Comparing `EllipSect-3.2.3.tar` & `EllipSect-3.4.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.282305 EllipSect-3.2.3/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 EllipSect-3.2.3/AUTHORS.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 EllipSect-3.2.3/CHANGELOG.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 EllipSect-3.2.3/CONTRIBUTING.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 EllipSect-3.2.3/LICENSE.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-16 22:37:19.282305 EllipSect-3.2.3/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-03-17 05:15:08.000000 EllipSect-3.2.3/README.rst
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/docs/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/Makefile
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/docs/_static/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/_static/.gitignore
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 EllipSect-3.2.3/docs/api.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/authors.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/changelog.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/conf.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/contributing.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    17760 2022-09-07 23:14:29.000000 EllipSect-3.2.3/docs/howto.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/index.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/license.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 EllipSect-3.2.3/docs/readme.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 EllipSect-3.2.3/docs/requirements.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.266304 EllipSect-3.2.3/example/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 EllipSect-3.2.3/example/README
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/galfit.feedme
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.3/example/psf.fits
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/img/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 EllipSect-3.2.3/img/A2029.ring.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 EllipSect-3.2.3/img/A85.comp.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 EllipSect-3.2.3/img/A85.con-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 EllipSect-3.2.3/img/A85.cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 EllipSect-3.2.3/img/A85.def.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 EllipSect-3.2.3/img/A85.ell-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 EllipSect-3.2.3/img/A85.grid.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 EllipSect-3.2.3/img/A85.log.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 EllipSect-3.2.3/img/A85.pix.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 EllipSect-3.2.3/img/A85.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 EllipSect-3.2.3/img/A85.ranx1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 EllipSect-3.2.3/img/A85.ranx2.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 EllipSect-3.2.3/img/A85.rany1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 EllipSect-3.2.3/pyproject.toml
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2023-05-16 22:37:19.282305 EllipSect-3.2.3/setup.cfg
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 EllipSect-3.2.3/setup.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.262304 EllipSect-3.2.3/src/
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/src/EllipSect.egg-info/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6819 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/SOURCES.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/dependency_links.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/entry_points.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 EllipSect-3.2.3/src/EllipSect.egg-info/not-zip-safe
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/requires.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2023-05-16 22:37:19.000000 EllipSect-3.2.3/src/EllipSect.egg-info/top_level.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.274304 EllipSect-3.2.3/src/ellipsect/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 EllipSect-3.2.3/src/ellipsect/__init__.py
--rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2023-02-08 06:36:48.000000 EllipSect-3.2.3/src/ellipsect/ellipsectors.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/inout/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 EllipSect-3.2.3/src/ellipsect/inout/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-03-14 00:31:50.000000 EllipSect-3.2.3/src/ellipsect/inout/galfit.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 EllipSect-3.2.3/src/ellipsect/inout/gfits.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    23292 2023-05-16 19:51:58.000000 EllipSect-3.2.3/src/ellipsect/inout/plots.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20007 2023-04-19 15:30:49.000000 EllipSect-3.2.3/src/ellipsect/inout/prt.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20009 2023-05-12 21:16:51.000000 EllipSect-3.2.3/src/ellipsect/inout/read.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/lib/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 EllipSect-3.2.3/src/ellipsect/lib/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7905 2023-02-19 04:21:12.000000 EllipSect-3.2.3/src/ellipsect/lib/clas.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-03-14 03:32:46.000000 EllipSect-3.2.3/src/ellipsect/lib/libs.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/phot/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 EllipSect-3.2.3/src/ellipsect/phot/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5474 2023-02-09 23:00:09.000000 EllipSect-3.2.3/src/ellipsect/phot/ned.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 EllipSect-3.2.3/src/ellipsect/phot/phot.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    12271 2023-05-11 07:29:38.000000 EllipSect-3.2.3/src/ellipsect/phot/tidal.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/sectors/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 EllipSect-3.2.3/src/ellipsect/sectors/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 EllipSect-3.2.3/src/ellipsect/sectors/comp.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 EllipSect-3.2.3/src/ellipsect/sectors/ellip.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 EllipSect-3.2.3/src/ellipsect/sectors/num.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    19192 2023-05-12 00:52:31.000000 EllipSect-3.2.3/src/ellipsect/sectors/sect.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/src/ellipsect/sky/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 EllipSect-3.2.3/src/ellipsect/sky/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    24185 2023-02-09 23:00:47.000000 EllipSect-3.2.3/src/ellipsect/sky/sky.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2023-05-16 22:37:19.278304 EllipSect-3.2.3/tests/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 EllipSect-3.2.3/tests/conftest.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.2.3/tests/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 EllipSect-3.2.3/tests/galfit.01
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2023-05-16 22:34:54.000000 EllipSect-3.2.3/tests/imgblock.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.2.3/tests/psf.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    14837 2023-05-13 17:24:07.000000 EllipSect-3.2.3/tests/test_ellipsect.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-19 05:38:00.000000 EllipSect-3.2.3/tox.ini
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 EllipSect-3.4.0/AUTHORS.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 EllipSect-3.4.0/CHANGELOG.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 EllipSect-3.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 EllipSect-3.4.0/LICENSE.txt
+-rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-04-13 01:31:39.437674 EllipSect-3.4.0/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-08-08 07:01:01.000000 EllipSect-3.4.0/README.rst
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/docs/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/Makefile
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/docs/_static/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/_static/.gitignore
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 EllipSect-3.4.0/docs/api.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/authors.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/changelog.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/conf.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/contributing.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    18141 2024-04-11 23:03:41.000000 EllipSect-3.4.0/docs/howto.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/index.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/license.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/readme.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 EllipSect-3.4.0/docs/requirements.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/example/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 EllipSect-3.4.0/example/README
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/galfit.feedme
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/psf.fits
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.429674 EllipSect-3.4.0/img/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 EllipSect-3.4.0/img/A2029.ring.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 EllipSect-3.4.0/img/A85.comp.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 EllipSect-3.4.0/img/A85.con-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 EllipSect-3.4.0/img/A85.cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 EllipSect-3.4.0/img/A85.def.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 EllipSect-3.4.0/img/A85.ell-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 EllipSect-3.4.0/img/A85.grid.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 EllipSect-3.4.0/img/A85.log.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 EllipSect-3.4.0/img/A85.pix.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 EllipSect-3.4.0/img/A85.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 EllipSect-3.4.0/img/A85.ranx1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 EllipSect-3.4.0/img/A85.ranx2.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 EllipSect-3.4.0/img/A85.rany1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 EllipSect-3.4.0/pyproject.toml
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2024-04-13 01:31:39.441674 EllipSect-3.4.0/setup.cfg
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 EllipSect-3.4.0/setup.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.417674 EllipSect-3.4.0/src/
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/src/EllipSect.egg-info/
+-rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/SOURCES.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/dependency_links.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/entry_points.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 EllipSect-3.4.0/src/EllipSect.egg-info/not-zip-safe
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/requires.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/top_level.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 EllipSect-3.4.0/src/ellipsect/__init__.py
+-rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2024-02-09 20:55:40.000000 EllipSect-3.4.0/src/ellipsect/ellipsectors.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/inout/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 EllipSect-3.4.0/src/ellipsect/inout/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-11-15 21:56:50.000000 EllipSect-3.4.0/src/ellipsect/inout/galfit.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 EllipSect-3.4.0/src/ellipsect/inout/gfits.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25023 2024-04-11 22:10:54.000000 EllipSect-3.4.0/src/ellipsect/inout/plots.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20165 2023-06-10 20:46:21.000000 EllipSect-3.4.0/src/ellipsect/inout/prt.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    21218 2024-04-11 22:20:26.000000 EllipSect-3.4.0/src/ellipsect/inout/read.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/lib/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 EllipSect-3.4.0/src/ellipsect/lib/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     8144 2024-04-11 21:55:45.000000 EllipSect-3.4.0/src/ellipsect/lib/clas.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-07-02 05:45:35.000000 EllipSect-3.4.0/src/ellipsect/lib/libs.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/phot/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 EllipSect-3.4.0/src/ellipsect/phot/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5878 2023-10-24 22:42:37.000000 EllipSect-3.4.0/src/ellipsect/phot/ned.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 EllipSect-3.4.0/src/ellipsect/phot/phot.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    12315 2023-10-27 21:26:58.000000 EllipSect-3.4.0/src/ellipsect/phot/tidal.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/sectors/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 EllipSect-3.4.0/src/ellipsect/sectors/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 EllipSect-3.4.0/src/ellipsect/sectors/comp.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 EllipSect-3.4.0/src/ellipsect/sectors/ellip.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 EllipSect-3.4.0/src/ellipsect/sectors/num.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20510 2024-04-11 22:00:26.000000 EllipSect-3.4.0/src/ellipsect/sectors/sect.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/src/ellipsect/sky/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 EllipSect-3.4.0/src/ellipsect/sky/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    24185 2023-02-09 23:00:47.000000 EllipSect-3.4.0/src/ellipsect/sky/sky.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/tests/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 EllipSect-3.4.0/tests/conftest.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.4.0/tests/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 EllipSect-3.4.0/tests/galfit.01
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2024-04-13 01:28:00.000000 EllipSect-3.4.0/tests/imgblock.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.4.0/tests/psf.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    15557 2024-04-12 06:43:05.000000 EllipSect-3.4.0/tests/test_ellipsect.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-19 05:38:00.000000 EllipSect-3.4.0/tox.ini
```

### Comparing `EllipSect-3.2.3/CHANGELOG.rst` & `EllipSect-3.4.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/CONTRIBUTING.rst` & `EllipSect-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/LICENSE.txt` & `EllipSect-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/PKG-INFO` & `EllipSect-3.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.2.3
+Version: 3.4.0
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
@@ -15,16 +15,26 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata
+Requires-Dist: sphinx>=3.2.1
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: astropy>=5.1
+Requires-Dist: scipy>=1.5.2
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: mgefit>=5.0.13
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 .. contents::
    :depth: 3
 ..
 
 --------------
```

### Comparing `EllipSect-3.2.3/README.rst` & `EllipSect-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/docs/Makefile` & `EllipSect-3.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/docs/api.rst` & `EllipSect-3.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/docs/conf.py` & `EllipSect-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/docs/howto.rst` & `EllipSect-3.4.0/docs/howto.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,34 @@
 EllipSect needs is in this file. However, there are some options
 available to use.
 
 The options are:
 
 ::
 
-    ellipsect [GALFIT_File] [--logx] [-q AxisRatio] [-pa PositionAngle] [--comp] [--pix] [--ranx/y Value] [--grid] [--dpi Value] [--noplot] [--phot] [--sbout] [--noplot] [--minlevel Value] [--sectors Value] [--object Name] [--filter Name] [--snr] [--help] [--checkimg] [--noned] [--distmod Value] [--magcor Value] [--scalekpc Value][--sbdim Value] [--model ModelImage] [--keep] [--ned XmlFile] [--gradsky ] [--randsky ] [--skyinit Value] [--skyRadmax Value][--skynum Value] [--skybox Value] [--skywidth Value] [--fwhm Value] [--galax ]
+   
+      
+    ellipsect [-h] [-lx] [-cp] [-px] [-g] [-sb] [-np] [-ph] [-ci] [-nn] [-gsky] [-rsky] [-snr]
+                 [-re] [-r90] [-r95] [-k] [-gx] [-asp] [-t] [-q AXISRAT] [-pa POSANGLE]
+                 [-rx RANX RANX] [-ry RANY RANY] [-dpi DOTSINCH] [-ml MINLEVEL] [-sc SECTORS]
+                 [-ob OBJECT] [-f FILTER] [-dm DISTMOD] [-mc MAGCOR] [-sk SCALEKPC] [-sd SBDIM]
+                 [-md MODEL] [-sky SKY] [-ned NED] [-ri RADINIT] [-srm SKYRADMAX] [-skb SKYBOX]
+                 [-skn SKYNUM] [-skw SKYWIDTH] [-distm DISTMAX] [-fw FWHM] [-br BRIGHTNESS]
+                 [-co CONTRAST] [-cm CMAP] [-nc NUMCOMP] [-ae AEXT] [-hc HCONST] [-om OMEGAM]
+                 [-ov OMEGAV]
+                 GalFile
+
+
 
 Below is an explanation of each parameter:
 
 **Main input parameters**
 -------------------------
 
-**GALFIT_File**: GALFIT output file (e.g. galfit.01). This **must** be
+**GalFile**: GALFIT output file (e.g. galfit.01). This **must** be
 the last GALFIT run. In other words, if there are two files: galfit.01
 and galfit.02, the one you need is galfit.02
 
 **help**: Help menu
 
 **logx**: plots X-axis as logarithm
 
@@ -59,14 +71,19 @@
 **dpi**: dots per inch value to increase/decrease resolution.
 
 **sbout**: Creates output file containing the surface brightness
 profiles.
 
 **galax**: Only the galaxy surface brightness is plotted.
 
+**effrad** Draw a vertical line indicating the effective radius
+**rad90**  Draw a vertical line indicating the 90% of total light
+**rad95**  Draw a vertical line indicating the 95% of total light
+
+
 **Photometric output options**
 ------------------------------
 
 **phot**: Compute photometry. Check the variables created in output
 file.
 
 The below options are used only if ‘phot’ is enabled:
```

### Comparing `EllipSect-3.2.3/docs/index.rst` & `EllipSect-3.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/example/gal.fits` & `EllipSect-3.4.0/example/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/example/galfit.feedme` & `EllipSect-3.4.0/example/galfit.feedme`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/example/psf.fits` & `EllipSect-3.4.0/example/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A2029.ring.png` & `EllipSect-3.4.0/img/A2029.ring.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.comp.png` & `EllipSect-3.4.0/img/A85.comp.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.con-cub.png` & `EllipSect-3.4.0/img/A85.con-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.cub.png` & `EllipSect-3.4.0/img/A85.cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.def.png` & `EllipSect-3.4.0/img/A85.def.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.ell-cub.png` & `EllipSect-3.4.0/img/A85.ell-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.grid.png` & `EllipSect-3.4.0/img/A85.grid.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.log.png` & `EllipSect-3.4.0/img/A85.log.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.pix.png` & `EllipSect-3.4.0/img/A85.pix.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.png` & `EllipSect-3.4.0/img/A85.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.ranx1.png` & `EllipSect-3.4.0/img/A85.ranx1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.ranx2.png` & `EllipSect-3.4.0/img/A85.ranx2.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/img/A85.rany1.png` & `EllipSect-3.4.0/img/A85.rany1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/setup.cfg` & `EllipSect-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/setup.py` & `EllipSect-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/EllipSect.egg-info/PKG-INFO` & `EllipSect-3.4.0/src/EllipSect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.2.3
+Version: 3.4.0
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
@@ -15,16 +15,26 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata
+Requires-Dist: sphinx>=3.2.1
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: astropy>=5.1
+Requires-Dist: scipy>=1.5.2
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: mgefit>=5.0.13
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 .. contents::
    :depth: 3
 ..
 
 --------------
```

### Comparing `EllipSect-3.2.3/src/EllipSect.egg-info/SOURCES.txt` & `EllipSect-3.4.0/src/EllipSect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/__init__.py` & `EllipSect-3.4.0/src/ellipsect/__init__.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/ellipsectors.py` & `EllipSect-3.4.0/src/ellipsect/ellipsectors.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/inout/galfit.py` & `EllipSect-3.4.0/src/ellipsect/inout/galfit.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/inout/gfits.py` & `EllipSect-3.4.0/src/ellipsect/inout/gfits.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/inout/plots.py` & `EllipSect-3.4.0/src/ellipsect/inout/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from ellipsect import *
 
 from ellipsect.sectors.num import Interpol
 from ellipsect.inout.prt import  PrintFilesGax
 from ellipsect.inout.prt import PrintFilesComps
 
-
+from ellipsect.inout.galfit  import conver2Sersic 
+from ellipsect.inout.galfit  import GetReff 
 
 def PlotSB(xradq,ysbq,ysberrq,xradm,ysbm,ysberrm,ellconf,scale):
     """  Produces final best-fitting plot  """
 
     # subplot for arc sec axis
     plt.close('all')
 
@@ -93,26 +94,43 @@
     axsec.tick_params(which='major', length=7)
     axsec.tick_params(which='minor', length=4, color='r')
 
 
     #begin psf fwhm 
     if ellconf.flagfwhm: 
         xpos = ellconf.fwhm*scale
-        axsec.axvline(x=xpos,  linestyle='--', color='k', linewidth=2)
+        axsec.axvline(x=xpos,  linestyle='--', color='k', label='FWHM', linewidth=2)
     # end 
 
+    #effective radius 
+    if ellconf.flagrep: 
+        xre = ellconf.rep*scale
+        axsec.axvline(x=xre,  linestyle='--', color='r', label='Re', linewidth=1.5)
+ 
+    #90% of total light radius 
+    if ellconf.flagr90p: 
+        xr90 = ellconf.r90p*scale
+        axsec.axvline(x = xr90,  linestyle='--', color='b', label='R90', linewidth=1.5)
+ 
+    #95%  of total light radius 
+    if ellconf.flagr95p: 
+        xr95 = ellconf.r95p*scale
+        axsec.axvline(x = xr95,  linestyle='--', color='c', label='R95', linewidth=1.5)
+ 
 
     # ULISES begin
     axsec.axes.xaxis.set_ticklabels([])
     # ULISES end 
 
 
     axsec.yaxis.set_minor_locator(AutoMinorLocator())
     axsec.yaxis.set_major_locator(AutoLocator())
 
+    if ellconf.title:
+        plt.title(ellconf.namefile, fontsize=10)
 
     # ULISES begin
     # Residual plot
     if len(ysbq) < len(ysbm):
         ysbm = ysbm[len(ysbm)-len(ysbq):]
     
     elif len(ysbq) > len(ysbm):
@@ -426,14 +444,19 @@
     
 
         #plt.show()
 
 
 def PlotMul(ellconf, galhead, galcomps, mgegal, mgemod, mgecom):
 
+
+    
+    comps = conver2Sersic(galcomps) #to compute Re
+
+
     fignum = 1
 
     minrad = np.min(mgegal.rad)
     maxrad = np.max(mgegal.rad)
 
     minsb = np.min(mgegal.sb)
     maxsb = np.max(mgegal.sb)
@@ -455,18 +478,28 @@
     if ellconf.flagrany == True:
         (ymin,ymax) = ellconf.rany[0], ellconf.rany[1]
 
 
 
     plt.clf()
 
+
+    if ellconf.title:
+        plt.title(ellconf.namefile, fontsize=10)
+
+
+
     fig, axsec = plt.subplots(nrows, 2, sharex=True, sharey='col', num=fignum)
     fig.subplots_adjust(hspace=0.01)
 
 
+
+
+
+
     if ellconf.flagpix:
         axpix = axsec[0,0].twiny()
         axpix2 = axsec[0,1].twiny()
 
     fig.text(0.04, 0.5, r"Surface Brightness $(mag\; arcsec^{-2})$", va='center', rotation='vertical')
     fig.text(0.96, 0.5, 'error ', va='center', rotation='vertical')
 
@@ -545,14 +578,38 @@
         #begin psf fwhm 
         if ellconf.flagfwhm: 
             xpos = ellconf.fwhm*galhead.scale
             axsec[row, 0].axvline(x=xpos, linestyle='--', color='k', linewidth=2)
         # end 
 
 
+        #effective radius 
+        if ellconf.flagrep: 
+            eff = 0.5
+            xre, tempmag = GetReff().GetReSer(galhead, comps, eff, txtangsky)
+
+            xre = xre*galhead.scale
+            axsec[row, 0].axvline(x=xre,  linestyle='--', color='r', label='Re', linewidth=1.5)
+     
+        #90% radius 
+        if ellconf.flagr90p: 
+            eff = 0.9
+            xr90, tempmag = GetReff().GetReSer(galhead, comps, eff, txtangsky)
+
+            xr90 = xr90*galhead.scale
+            axsec[row, 0].axvline(x = xr90,  linestyle='--', color='b', label='R90', linewidth=1.5)
+ 
+        #95% radius 
+        if ellconf.flagr95p: 
+            eff = 0.95
+            xr95, tempmag = GetReff().GetReSer(galhead, comps, eff, txtangsky)
+
+            xr95 = xr95*galhead.scale
+            axsec[row, 0].axvline(x = xr95,  linestyle='--', color='c', label='R95', linewidth=1.5)
+ 
 
 
 
         if ellconf.flaglogx == False:
 
             #axsec[row, 0].plot(r, mgesb[angal], 'C3o') 
             #change lines instead of dots
```

### Comparing `EllipSect-3.2.3/src/ellipsect/inout/prt.py` & `EllipSect-3.4.0/src/ellipsect/inout/prt.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,20 @@
 
     lineout = "# Photometry for object: {} (use -object option to change it) \n".format(ellconf.objname)
     OUTPHOT.write(lineout)
 
     lineout = "# All photometric quantities are computed for filter {} (use -filter option to change it) \n".format(ellconf.band)
     OUTPHOT.write(lineout)
 
+
+
+    lineout = '# Cosmology: hconst = {}, omega m = {}, omega lambda= {}'.format(ellconf.hconst,ellconf.omegam,ellconf.omegav) 
+    OUTPHOT.write(lineout)
+
+
     lineout = "# Magnitudes are not corrected by K-Correction \n"
     OUTPHOT.write(lineout)
 
     lineout= "# Total magnitude and other variables are NOT computed for: \n"
     OUTPHOT.write(lineout)
 
     lineout= "# ferrer, nuker, edgedisk and king components.  \n"
```

### Comparing `EllipSect-3.2.3/src/ellipsect/inout/read.py` & `EllipSect-3.4.0/src/ellipsect/inout/read.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,35 +64,47 @@
     parser.add_argument("-np","--noplot", action="store_true", help="avoids pop up windows and only creates images files")
     parser.add_argument("-ph","--phot", action="store_true", help="Compute photometry. Check the created output file")
     parser.add_argument("-ci","--checkimg", action="store_true", help="save the images used for sectors_photometry in individual files")
     parser.add_argument("-nn","--noned", action="store_true", help="it avoids to connect to NED")
     parser.add_argument("-gsky","--gradsky", action="store_true", help="computes sky using the gradient method")
     parser.add_argument("-rsky","--randsky", action="store_true", help="computes sky using random boxes")
     parser.add_argument("-snr","--snr", action="store_true", help="Creates Signal to Noise image if phot is activated")
-    parser.add_argument("-chi","--chisqr", action="store_true", help="Creates Chi-square image if phot is activated")
+    #parser.add_argument("-chi","--chisqr", action="store_true", help="Creates Chi-square image if phot is activated")
+
+
+    parser.add_argument("-re","--effrad", action="store_true", help="Draw a vertical line indicating the effective radius")
+
+    parser.add_argument("-r90","--rad90", action="store_true", help="Draw a vertical line indicating the 90%% of total light")
+
+    parser.add_argument("-r95","--rad95", action="store_true", help="Draw a vertical line indicating the 95%% of total light")
+
 
     parser.add_argument("-k","--keep", action="store_true", help="use existing file to compute subcomponents")
     parser.add_argument("-gx","--galax", action="store_true", help="only the galaxy surface brightness is shown in the plot")
 
 
     linehelp="includes all the sky pixels for gradsky and randsky. "  \
             + "Default mode removes top %%80 and bottom %%20 sky pixels "
     parser.add_argument("-asp","--allskypx", action="store_true", 
                         help=linehelp)
- 
+
+
+
+    parser.add_argument("-t","--title", action="store_true", help="put title on plots")
+
     #options with arguments
     #parser.add_argument("-cn","--center",nargs=2,action="store", type=float, help="galaxy's center ")
 
     parser.add_argument("-q","--axisrat", type=float, help="galaxy axis ratio ")
     parser.add_argument("-pa","--posangle", type=float, help="position angle (same as GALFIT)  ",default=0)
     parser.add_argument("-rx","--ranx",nargs=2, type=float, help="provide a range for x-axis: xmin - xmax ")
     parser.add_argument("-ry","--rany", nargs=2,type=float, help="provide a range for y-axis: ymin - ymax  ")
     parser.add_argument("-dpi","--dotsinch", type=int, help="dots per inch used for images files ")
-    parser.add_argument("-ml","--minlevel", type=float, help="parameter given directly to sectors_photometry. ")
-    parser.add_argument("-sc","--sectors", type=int, help="parameter given directly to sectors_photometry. Divide elipse in 'sectors'")
+    parser.add_argument("-ml","--minlevel", type=float, help="parameter given to sectors_photometry. ")
+    parser.add_argument("-sc","--sectors", type=int, help="parameter given to sectors_photometry. It divides the ellipse in 'sectors'")
     parser.add_argument("-ob","--object",  help="used for 'phot' to search in NED")
     parser.add_argument("-f","--filter",  help="used for 'phot' to indicate band for NED  ")
     parser.add_argument("-dm","--distmod", type=float, help="Introduce Distance Modulus  ")
     parser.add_argument("-mc","--magcor", type=float, help="Introduce Galactic Extinction ")
     parser.add_argument("-sk","--scalekpc", type=float, help="Introduce equivalence of ''/kiloparsec ")
     parser.add_argument("-sd","--sbdim", type=float, help="surface brightness dimming ")
     parser.add_argument("-md","--model",  help="User can introduce its own image model. ")
@@ -126,15 +138,23 @@
                         + "select for galaxy center. Default = first component. The "
                         + "component order follows as it is shown in galfit file ",default=1)
 
 
     parser.add_argument("-ae","--aext", type=float, 
                         help="Surface brightness correction for plots only ", default=0)
  
-
+    parser.add_argument("-hc","--hconst", type=float, 
+                        help="hubble constant to download xml file from NED ", default=67.8)
+ 
+    parser.add_argument("-om","--omegam", type=float, 
+                        help="omega matter value to download xml file from NED ", default=.308)
+ 
+    parser.add_argument("-ov","--omegav", type=float, 
+                        help="omega lambda value to download xml file from NED ", default=0.692)
+ 
 
     # every new parameter added here must be
     # also added in function PassArgs() in ellipsect/sectors/sect.py
 
 
     return parser
 
@@ -486,45 +506,53 @@
     ellconf.namefile = root_ext[0]
     
     #adding numbers of galfit file for output
     gal_ext = os.path.splitext(ellconf.galfile)
     numstr = gal_ext[1] 
     numstr = numstr[1:]
 
+    if ellconf.numcomp:
+        precomp = "-nc" + str(ellconf.numcomp)
+    else:
+        precomp = ""
+
+
+
+
     if numstr.isnumeric():
 
         # names for the different png
-        ellconf.namepng = ellconf.namefile + '-' + numstr + ".png"
-        ellconf.namesec = ellconf.namefile + '-' + numstr + "-gal.png"
-        ellconf.namemod = ellconf.namefile + '-' + numstr + "-mod.png"
-        ellconf.namemul = ellconf.namefile + '-' + numstr + "-mul.png"
-        ellconf.namesub = ellconf.namefile + '-' + numstr + "-comp.fits"
-
-        ellconf.namesig = ellconf.namefile + '-' + numstr + "-sig.fits"
-
-
-        ellconf.sboutput = ellconf.namefile + '-' + numstr + "-sbout"
-        ellconf.output = ellconf.namefile + '-' + numstr + "-out.txt"
-
-        ellconf.namened = ellconf.namefile + '-' + numstr + "-ned.xml"
-
-        ellconf.namesnr = ellconf.namefile + '-' + numstr + "-snr.fits"
-        ellconf.namecheck = ellconf.namefile + '-' + numstr + "-check.fits"
-        ellconf.namering = ellconf.namefile + '-' + numstr + "-ring.fits"
-        ellconf.nameringmask = ellconf.namefile + '-' + numstr + "-ringmask.fits"
-        ellconf.namecube = ellconf.namefile + '-' + numstr + "-cub.png"
-        ellconf.namechi = ellconf.namefile + '-' + numstr + "-chi.fits"
+        ellconf.namepng = ellconf.namefile + '-g' + numstr + precomp + "-splot.png"
+        ellconf.namesec = ellconf.namefile + '-g' + numstr + precomp + "-gal.png"
+        ellconf.namemod = ellconf.namefile + '-g' + numstr + precomp + "-mod.png"
+        ellconf.namemul = ellconf.namefile + '-g' + numstr + precomp + "-mplot.png"
+        ellconf.namesub = ellconf.namefile + '-g' + numstr + precomp + "-comp.fits"
+
+        ellconf.namesig = ellconf.namefile + '-g' + numstr + precomp + "-sig.fits"
+
+
+        ellconf.sboutput = ellconf.namefile + '-g' + numstr + precomp + "-sbout"
+        ellconf.output = ellconf.namefile + '-g' + numstr + precomp +  "-out.txt"
+
+        ellconf.namened = ellconf.namefile + '-g' + numstr + precomp + "-ned.xml"
+
+        ellconf.namesnr = ellconf.namefile + '-g' + numstr + precomp + "-snr.fits"
+        ellconf.namecheck = ellconf.namefile + '-g' + numstr + precomp + "-check.fits"
+        ellconf.namering = ellconf.namefile + '-g' + numstr + precomp + "-ring.fits"
+        ellconf.nameringmask = ellconf.namefile + '-g' + numstr + precomp + "-ringmask.fits"
+        ellconf.namecube = ellconf.namefile + '-g' + numstr + precomp + "-cub.png"
+        ellconf.namechi = ellconf.namefile + '-g' + numstr + precomp + "-chi.fits"
 
     else:
 
         # names for the different png
-        ellconf.namepng = ellconf.namefile + ".png"
+        ellconf.namepng = ellconf.namefile + "-splot.png"
         ellconf.namesec = ellconf.namefile + "-gal.png"
         ellconf.namemod = ellconf.namefile + "-mod.png"
-        ellconf.namemul = ellconf.namefile + "-mul.png"
+        ellconf.namemul = ellconf.namefile + "-mplot.png"
         ellconf.namesub = ellconf.namefile + "-comp.fits"
 
         ellconf.namesig = ellconf.namefile + "-sig.fits"
 
 
         ellconf.sboutput = ellconf.namefile + "-sbout"
         ellconf.output = ellconf.namefile + "-out.txt"
```

### Comparing `EllipSect-3.2.3/src/ellipsect/lib/clas.py` & `EllipSect-3.4.0/src/ellipsect/lib/clas.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     flagphot=False
     flagminlevel=False
     flagsectors=False
     flagobj=False
     flagband=False
     flagweb=False # to check connection to ned
     flagsnr = False
-    flagchi = False
+    #flagchi = False
 
     flagcheck=False
     flagned=False
 
     flagmod=False
     flagmag=False
     flagscale=False
@@ -70,14 +70,17 @@
     flagskynum = False
     flagskywidth = False
     
     flagdistmax = False
 
     flagfwhm = False
 
+    flagrep = False
+    flagr90p = False
+    flagr95p = False
     #flagcent = False 
 
     flagrmsky=True
 
 
 
     #init
@@ -93,15 +96,15 @@
     dplot=True
 
     dpival=100
 
     minlevel=0
     sectors=19
 
-
+    title = False
 
     #input file
     galfile= "galfit.01"
 
     #sb output file
     sboutput = "sbout.txt"
 
@@ -149,14 +152,18 @@
     skyRad = 50 # minimum radius
     skybox = 20
     skynum = 20
     skywidth = 20
 
     fwhm = 2
 
+    rep = 0
+    r90p = 0
+    r95p = 0
+
     distmax = 10
 
     brightness = 0 
     contrast = 1 
 
     cmap="viridis"
 
@@ -172,14 +179,19 @@
 
     randskymean = 0
     randskystd = 0
     randskymed = 0
 
     Aext = 0  # surface brightness correction for plots
 
+    hconst = 67.8 
+    omegam  = 0.308
+    omegav = 0.692
+
+
 
 #class to comunicate externally:
 class PhotAPI:
 
     #################
     #from InputParams
 
@@ -233,14 +245,19 @@
     xmax=2
     ymin=1
     ymax=2
     band="R"
     inputimage="galaxy.fits"
     Aext = 0
 
+    hconst = 67.8 
+    omegam  = 0.308
+    omegav = 0.692
+
+
     # from gradsky
     gradskymean = 0
     gradskystd = 0
     gradskymed = 0
 
     # from randboxsky
     randskymean = 0
```

### Comparing `EllipSect-3.2.3/src/ellipsect/lib/libs.py` & `EllipSect-3.4.0/src/ellipsect/lib/libs.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/phot/ned.py` & `EllipSect-3.4.0/src/ellipsect/phot/ned.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,40 +39,50 @@
 
     ellconf.flagweb=True
 
     objname=ellconf.objname
 
     nedweb="https://ned.ipac.caltech.edu/cgi-bin/nph-objsearch?extend=no&of=xml_all&objname="
 
+
+
     if ellconf.flagnedfile:
         filened = ellconf.nedfile
     else:
         filened=ellconf.namened
 
     if ellconf.flagmod or ellconf.flagmag or ellconf.flagscale or ellconf.flagdim:
 
         GalExt=ellconf.InMagCor
         DistMod=ellconf.InDistMod
         DistMod2=ellconf.InDistMod
         Scalekpc=ellconf.InScale
         SbDim=ellconf.InSbDim
     else:
-        #checar si el archivo existe para no hacer conexion a internet
         if(not(os.path.isfile(filened))):
+        #verifica si el archivo existe para no hacer conexion a internet
 
             if ellconf.flagnedfile:
                 print("can't find user's ned {} file ".format(filened))
                 ellconf.flagweb=False
             else:
                 # command for wget
                 #wget -O NED_51.xml "https://ned.ipac.caltech.edu/cgi-bin/nph-objsearch?extend=no&of=xml_all&objname=m+51"
-                wgetcmd = 'wget -O {} "{}{}"'.format(filened,nedweb,objname)
+
+                #https://ned.ipac.caltech.edu/cgi-bin/nph-objsearch?extend=no&of=xml_all&objname=ngc+6166&hconst=67.8&omegam=0.308&omegav=0.692
+
+
+                wgetcmd = 'wget -O {} "{}{}&hconst={:.1f}\&omegam={:.3f}\&omegav={:.3f}"'.format(
+                            filened,nedweb,objname,ellconf.hconst,ellconf.omegam,ellconf.omegav)
 
                 print("Running: ",wgetcmd)
 
+                print('Cosmology: hconst = {}, omega m= {}, omega lambda= {}'.format(ellconf.hconst,ellconf.omegam,ellconf.omegav)) 
+
+
                 errwg = sp.run([wgetcmd], shell=True, stdout=sp.PIPE,stderr=sp.PIPE, universal_newlines=True)
 
                 if errwg.returncode != 0:
                     print("can't connect to NED webserver. Is your internet connection working? ")
                     print("Luminosity and absolute magnitude will not be computed") 
                     ellconf.flagweb=False
         else:
```

### Comparing `EllipSect-3.2.3/src/ellipsect/phot/phot.py` & `EllipSect-3.4.0/src/ellipsect/phot/phot.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/phot/tidal.py` & `EllipSect-3.4.0/src/ellipsect/phot/tidal.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,36 +175,41 @@
         print("SNR image created.. ",ellconf.namesnr)
 
 
     ##################################
     # creation of the Chi-square image 
     ##################################
 
-    if ellconf.flagchi:
-        header['TypeIMG'] = ('CHI-SQR', 'Chi-Square image')
-        hdu[0].header  = header
+    #if ellconf.flagchi:
 
+    header['TypeIMG'] = ('CHI-SQR', 'Chi-Square image')
+    hdu[0].header  = header
 
-        maskchi = immask == True # big image coordinates
 
+    maskchi = immask == True # big image coordinates
 
-        if imgal.shape == imsigma.shape:
-            dataimg.imchi = (imgal - immodel)**2 / imsigma**2
-            if maskchi.any():
-                dataimg.imchi[maskchi] = 0
-        else:
-            print("WARNING: Chi-square image can not be computed" +
-                    "because galaxy and sigma images have different shapes")
-            dataimg.imchi = np.ones(imgal.shape)
-        
-        hdu[0].data = dataimg.imchi
 
-        hdu.writeto(ellconf.namechi, overwrite=True)
-        print("Chi square image created.. ", ellconf.namechi)
+    if imgal.shape == imsigma.shape:
+        dataimg.imchi = (imgal - immodel)**2 / imsigma**2
+        if maskchi.any():
+            dataimg.imchi[maskchi] = 0
+    else:
+        print("WARNING: Chi-square image can not be computed" +
+                "because galaxy and sigma images have different shapes")
+        dataimg.imchi = np.ones(imgal.shape)
+    
+    hdu[0].data = dataimg.imchi
+
+    hdu.writeto(ellconf.namechi, overwrite=True)
+    print("Chi square image created.. ", ellconf.namechi)
+
 
+    ##################################
+    # end of the Chi-square image 
+    ##################################
 
 
 
 
     hdu.close()
 
 
@@ -429,18 +434,18 @@
 #phot/tidal.py
 
 def ExtractEllip(imagemat, idn, x, y, R, theta, ell, xmin, xmax, ymin, ymax):
     "This subroutine extract an ellipse within an box to compute photometric parameters "
     "It returns the area of ellipse with idn values. "
 
 
-    xmin = np.int(xmin)
-    xmax = np.int(xmax)
-    ymin = np.int(ymin)
-    ymax = np.int(ymax)
+    xmin = int(xmin)
+    xmax = int(xmax)
+    ymin = int(ymin)
+    ymax = int(ymax)
 
     q = (1 - ell)
     bim = q * R
 
     theta = theta * np.pi / 180  # Rads!!!
 
     ypos, xpos = np.mgrid[ymin - 1: ymax + 1, xmin - 1: xmax + 1]
```

### Comparing `EllipSect-3.2.3/src/ellipsect/sectors/comp.py` & `EllipSect-3.4.0/src/ellipsect/sectors/comp.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/sectors/ellip.py` & `EllipSect-3.4.0/src/ellipsect/sectors/ellip.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/sectors/num.py` & `EllipSect-3.4.0/src/ellipsect/sectors/num.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/src/ellipsect/sectors/sect.py` & `EllipSect-3.4.0/src/ellipsect/sectors/sect.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 from ellipsect.phot.phot import OutPhot
 
 from ellipsect.lib.clas import EllipSectConfig
 
 
 from ellipsect.inout.galfit  import Galfit 
 from ellipsect.inout.galfit  import numComps
+from ellipsect.inout.galfit  import conver2Sersic 
 from ellipsect.inout.galfit  import readDataImg
+from ellipsect.inout.galfit  import GetReff 
+
+from ellipsect.inout.gfits import GetFits
 
 from ellipsect.inout.prt import printEllinfo
 
 from ellipsect.sky.sky import skyCall
 
 
 from ellipsect.lib.clas import PhotAPI 
@@ -77,15 +81,18 @@
 
     ellconf.tot = N
 
     #creates names of the output files based on prefix of galfit output
     prefixNames(ellconf, galhead.outimage)
 
     if os.path.isfile(galhead.sigimage):
-        ellconf.namesig = galhead.sigimage #using existing sigma file
+        #ellconf.namesig = galhead.sigimage #using existing sigma file
+        GetFits(galhead.sigimage, ellconf.namesig, galhead.xmin, galhead.xmax, 
+                galhead.ymin, galhead.ymax)
+
 
 
 
 
     if ellconf.flagsbout == True: 
 
         if not os.path.exists("sbfiles"):
@@ -103,15 +110,19 @@
 
     dataimg = readDataImg(ellconf, galhead)
 
     # removing background from galaxy and model images 
     dataimg.img = dataimg.img - ellconf.skylevel
     dataimg.model = dataimg.model - ellconf.skylevel
 
-    plotCube(ellconf, galhead, galcomps) #plots the cube image
+
+
+    comps = conver2Sersic(galcomps) 
+
+    plotCube(ellconf, galhead, comps) #plots the cube image
 
 
     #   numsectors=19 default
     numsectors = ellconf.sectors
 
     minlevel = ellconf.minlevel  # minimun value for sky
 
@@ -133,14 +144,31 @@
                                     n_sectors = numsectors, minlevel = 0)
         
 
     #computing sky
     skyCall(ellconf, galhead, galcomps)
 
 
+    #computing fraction of light radius
+    if ellconf.flagrep:
+        eff = 0.5
+        ellconf.rep, tempmag = GetReff().GetReSer(galhead, comps, eff, ellconf.parg)
+
+    if ellconf.flagr90p:
+        eff = 0.9
+        ellconf.r90p, tempmag = GetReff().GetReSer(galhead, comps, eff, ellconf.parg)
+
+    if ellconf.flagr95p:
+        eff = 0.95
+        ellconf.r95p, tempmag = GetReff().GetReSer(galhead, comps, eff, ellconf.parg)
+
+
+
+
+
 
     print("creating plots..")
 
     limx, limy = EllipSectors(ellconf, galhead, galcomps, sectgalax, 
                                 sectmodel, sectcomps, n_sectors = numsectors)
 
     print("plot file: ", ellconf.namepng)
@@ -385,16 +413,16 @@
     while(n < len(galcomps.N)):
 
 
         if galcomps.Active[n] == True:
 
             subim = subimgs[i]
 
-            eps = 1 - galcomps.AxRat[n]
-            angsec = 90 - galcomps.PosAng[n]
+            #eps = 1 - galcomps.AxRat[n]   #removed because it must follow the axrat of galaxy
+            #angsec = 90 - galcomps.PosAng[n] #same but for angle
 
 
             if ellconf.flagcheck:
 
                 scmp = sectors_photometry(subim, eps, angsec, xctemp, yctemp, minlevel = minlevel, 
                                             plot = 1, badpixels = maskb, n_sectors = n_sectors)
 
@@ -533,14 +561,22 @@
     photapi.Flux = galcomps.Flux.copy()
     photapi.PerLight = galcomps.PerLight.copy()
     photapi.me = galcomps.me.copy()
     photapi.mme = galcomps.mme.copy()
     photapi.kser = galcomps.kser.copy()
 
 
+    photapi.hconst = ellconf.hconst 
+
+    photapi.omegam = ellconf.omegam 
+
+    photapi.omegav = ellconf.omegav
+
+
+
 
 
 def PassArgs(args):
     '''function to pass arguments from args to ellconf'''
 
     # Note: This function shouldn't exist, but since 
     # I didn't know about the argparse library when 
@@ -601,17 +637,20 @@
 
     if args.galax:
         ellconf.flagalax=True
 
     if args.allskypx:
         ellconf.flagrmsky=False
 
-    if args.chisqr:
-        ellconf.flagchi = True
+    #if args.chisqr:
+    #    ellconf.flagchi = True
  
+    if args.title:
+        ellconf.title = args.title
+
 
     #options with arguments
 
     #if args.center: #removed because of number of component is selected
     #    ellconf.flagcent = True
     #    ellconf.xc = args.center[0]
     #    ellconf.yc = args.center[1]
@@ -724,14 +763,37 @@
     if args.numcomp:
         ellconf.numcomp = args.numcomp
 
     if args.aext:
         ellconf.Aext = args.aext
 
 
+    if args.hconst:
+        ellconf.hconst = args.hconst
+
+    if args.omegam:
+        ellconf.omegam = args.omegam
+
+    if args.omegav:
+        ellconf.omegav = args.omegav
+
+
+
+    if args.effrad:
+        ellconf.flagrep = True
+
+
+    if args.rad90:
+        ellconf.flagr90p = True
+
+
+    if args.rad95:
+        ellconf.flagr95p = True
+
+
 
 
     return ellconf
```

### Comparing `EllipSect-3.2.3/src/ellipsect/sky/sky.py` & `EllipSect-3.4.0/src/ellipsect/sky/sky.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/tests/gal.fits` & `EllipSect-3.4.0/tests/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/tests/galfit.01` & `EllipSect-3.4.0/tests/galfit.01`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/tests/imgblock.fits` & `EllipSect-3.4.0/tests/imgblock.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/tests/psf.fits` & `EllipSect-3.4.0/tests/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.2.3/tests/test_ellipsect.py` & `EllipSect-3.4.0/tests/test_ellipsect.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 # checking the creation of files
 def test_files():
 
     arg=['tests/galfit.01', '-np']
 
     path="tests/"
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
     if os.path.isfile(filepng):
         os.remove(filepng)
     if os.path.isfile(filemulpng):
@@ -74,23 +74,25 @@
 # checking the creation of the components file
 def test_comp():
 
     arg=['tests/galfit.01','--comp', '--noplot']
 
     path="tests/"
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
+
+
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
 
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
 
     filecomp= path+filecomp
 
     if os.path.isfile(filecomp):
         os.remove(filecomp)
 
 
@@ -124,30 +126,32 @@
 def test_phot():
 
 
     arg=['tests/galfit.01','--phot', '--noned', '--noplot']
 
     path="tests/"
 
-    filephot = "imgblock-01-out.txt"
+    filephot = "imgblock-g01-nc1-out.txt"
     filephot= path+filephot
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
     filecomp= path+filecomp
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
+
 
-    filesig = "imgblock-01-sig.fits"
+
+    filesig = "imgblock-g01-nc1-sig.fits"
     filesig= path+filesig
 
-    filecheck = "imgblock-01-check.fits"
+    filecheck = "imgblock-g01-nc1-check.fits"
     filecheck= path+filecheck
 
-    filecube = "imgblock-01-cub.png"
+    filecube = "imgblock-g01-nc1-cub.png"
     filecube = path+filecube
 
 
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
@@ -255,38 +259,44 @@
 def test_gsky():
 
 
     arg=['tests/galfit.01','-gsky', '-ri','2', '-skw','3','--noplot']
 
     path="tests/"
 
-    filephot = "imgblock-01-out.txt"
+
+    filephot = "imgblock-g01-nc1-out.txt"
     filephot= path+filephot
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
     filecomp= path+filecomp
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
 
-    filesig = "imgblock-01-sig.fits"
+    filesig = "imgblock-g01-nc1-sig.fits"
     filesig= path+filesig
 
-    filecheck = "imgblock-01-check.fits"
+    filecheck = "imgblock-g01-nc1-check.fits"
     filecheck= path+filecheck
 
-    filecube = "imgblock-01-cub.png"
+    filecube = "imgblock-g01-nc1-cub.png"
     filecube = path+filecube
 
-    filersky = "imgblock-01-ring.fits"
+    filersky = "imgblock-g01-nc1-ring.fits"
     filersky = path + filersky
 
-    filermsky = "imgblock-01-ringmask.fits"
+    filermsky = "imgblock-g01-nc1-ringmask.fits"
     filermsky = path + filermsky
 
+    filechi = "imgblock-g01-nc1-chi.fits"
+    filechi = path + filechi
+
+
+
 
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
     if os.path.isfile(filepng):
         os.remove(filepng)
@@ -370,38 +380,45 @@
 def test_rsky():
 
 
     arg=['tests/galfit.01','-rsky','--noplot']
 
     path="tests/"
 
-    filephot = "imgblock-01-out.txt"
+    filephot = "imgblock-g01-nc1-out.txt"
     filephot= path+filephot
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
     filecomp= path+filecomp
 
-    filepng = "imgblock.01-png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
 
-    filesig = "imgblock-01-sig.fits"
+    filesig = "imgblock-g01-nc1-sig.fits"
     filesig= path+filesig
 
-    filecheck = "imgblock-01-check.fits"
+    filecheck = "imgblock-g01-nc1-check.fits"
     filecheck= path+filecheck
 
-    filecube = "imgblock-01-cub.png"
+    filecube = "imgblock-g01-nc1-cub.png"
     filecube = path+filecube
 
-    filersky = "imgblock-01-ring.fits"
+    filersky = "imgblock-g01-nc1-ring.fits"
     filersky = path + filersky
 
-    filermsky = "imgblock-01-ringmask.fits"
+    filermsky = "imgblock-g01-nc1-ringmask.fits"
     filermsky = path + filermsky
 
+    filechi = "imgblock-g01-nc1-chi.fits"
+    filechi = path + filechi
+
+
+
+
+
 
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
     if os.path.isfile(filepng):
         os.remove(filepng)
@@ -487,38 +504,43 @@
 def test_freepar():
 
 
     arg=['tests/galfit.01','--noplot']
 
     path="tests/"
 
-    filephot = "imgblock-01-out.txt"
+    filephot = "imgblock-g01-nc1-out.txt"
     filephot= path+filephot
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
     filecomp= path+filecomp
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
 
-    filesig = "imgblock-01-sig.fits"
+    filesig = "imgblock-g01-nc1-sig.fits"
     filesig= path+filesig
 
-    filecheck = "imgblock-01-check.fits"
+    filecheck = "imgblock-g01-nc1-check.fits"
     filecheck= path+filecheck
 
-    filecube = "imgblock-01-cub.png"
+    filecube = "imgblock-g01-nc1-cub.png"
     filecube = path+filecube
 
-    filersky = "imgblock-01-ring.fits"
+    filersky = "imgblock-g01-nc1-ring.fits"
     filersky = path + filersky
 
-    filermsky = "imgblock-01-ringmask.fits"
+    filermsky = "imgblock-g01-nc1-ringmask.fits"
     filermsky = path + filermsky
 
+    filechi = "imgblock-g01-nc1-chi.fits"
+    filechi = path + filechi
+
+
+
 
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
     if os.path.isfile(filepng):
         os.remove(filepng)
@@ -620,38 +642,41 @@
 def test_img_size():
 
 
     arg=['tests/galfit.01','--noplot']
 
     path="tests/"
 
-    filephot = "imgblock-01-out.txt"
+    filephot = "imgblock-g01-nc1-out.txt"
     filephot= path+filephot
 
-    filecomp = "imgblock-01-comp.fits"
+    filecomp = "imgblock-g01-nc1-comp.fits"
     filecomp= path+filecomp
 
-    filepng = "imgblock-01.png"
-    filemulpng = "imgblock-01-mul.png"
+    filepng = "imgblock-g01-nc1-splot.png"
+    filemulpng = "imgblock-g01-nc1-mplot.png"
 
-    filesig = "imgblock-01-sig.fits"
+    filesig = "imgblock-g01-nc1-sig.fits"
     filesig= path+filesig
 
-    filecheck = "imgblock-01-check.fits"
+    filecheck = "imgblock-g01-nc1-check.fits"
     filecheck= path+filecheck
 
-    filecube = "imgblock-01-cub.png"
+    filecube = "imgblock-g01-nc1-cub.png"
     filecube = path+filecube
 
-    filersky = "imgblock-01-ring.fits"
+    filersky = "imgblock-g01-nc1-ring.fits"
     filersky = path + filersky
 
-    filermsky = "imgblock-01-ringmask.fits"
+    filermsky = "imgblock-g01-nc1-ringmask.fits"
     filermsky = path + filermsky
 
+    filechi = "imgblock-g01-nc1-chi.fits"
+    filechi = path + filechi
+
 
     tempmask="tempmask.fits"
     filetempmask = tempmask 
 
     filepng = path+filepng
     filemulpng = path+filemulpng
 
@@ -680,15 +705,17 @@
 
     if os.path.isfile(filermsky):
         os.remove(filermsky)
 
     if os.path.isfile(filetempmask):
         os.remove(filetempmask)
  
-
+    if os.path.isfile(filechi):
+        os.remove(filechi)
+ 
 
     from ellipsect.inout.galfit  import Galfit 
     from ellipsect.sectors.sect  import PassArgs 
     from ellipsect.inout.galfit import SelectGal 
 
     # read user's input 
     args = ArgParsing(arg)
@@ -757,13 +784,15 @@
 
     if os.path.isfile(filermsky):
         os.remove(filermsky)
 
     if os.path.isfile(filetempmask):
         os.remove(filetempmask)
  
-
+    if os.path.isfile(filechi):
+        os.remove(filechi)
+
```

### Comparing `EllipSect-3.2.3/tox.ini` & `EllipSect-3.4.0/tox.ini`

 * *Files identical despite different names*

