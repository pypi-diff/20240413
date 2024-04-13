# Comparing `tmp/rowingdata-3.6.6.tar.gz` & `tmp/rowingdata-3.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rowingdata-3.6.6.tar", last modified: Thu Feb 15 15:50:27 2024, max compression
+gzip compressed data, was "rowingdata-3.6.7.tar", last modified: Sat Apr 13 07:15:45 2024, max compression
```

## Comparing `rowingdata-3.6.6.tar` & `rowingdata-3.6.7.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.607750 rowingdata-3.6.6/
--rw-r--r--   0 sander    (1000) sander    (1000)     1074 2023-06-04 14:45:11.000000 rowingdata-3.6.6/LICENSE
--rw-r--r--   0 sander    (1000) sander    (1000)      276 2023-06-04 14:45:11.000000 rowingdata-3.6.6/MANIFEST.in
--rw-r--r--   0 sander    (1000) sander    (1000)    31748 2024-02-15 15:50:27.611083 rowingdata-3.6.6/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)    31386 2023-06-04 14:45:11.000000 rowingdata-3.6.6/README.rst
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.587750 rowingdata-3.6.6/bin/
--rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.6/bin/crewnerddata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2933658 2023-06-04 14:45:11.000000 rowingdata-3.6.6/bin/crewnerddata.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    53177 2023-06-04 14:45:11.000000 rowingdata-3.6.6/bin/testdata.csv
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.587750 rowingdata-3.6.6/docs/
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.587750 rowingdata-3.6.6/docs/_build/
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.591083 rowingdata-3.6.6/docs/_build/html/
--rw-r--r--   0 sander    (1000) sander    (1000)      166 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/.buildinfo
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.591083 rowingdata-3.6.6/docs/_build/html/_images/
--rw-r--r--   0 sander    (1000) sander    (1000)   124024 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/2x20min.png
--rw-r--r--   0 sander    (1000) sander    (1000)    85796 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/editrower.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)   156560 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/greghoc.png
--rw-r--r--   0 sander    (1000) sander    (1000)   118169 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/image001.png
--rw-r--r--   0 sander    (1000) sander    (1000)    42789 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/otwlogbook.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    59925 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/otwscreenshot.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    58348 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/screenshot.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    37995 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/screenshotlogbook.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)   156147 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_images/woensdag.png
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.591083 rowingdata-3.6.6/docs/_build/html/_sources/
--rw-r--r--   0 sander    (1000) sander    (1000)      463 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_sources/index.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       67 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_sources/modules.txt
--rw-r--r--   0 sander    (1000) sander    (1000)     3149 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_sources/rowingdata.txt
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.591083 rowingdata-3.6.6/docs/_build/html/_static/
--rw-r--r--   0 sander    (1000) sander    (1000)      673 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 sander    (1000) sander    (1000)    10507 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 sander    (1000) sander    (1000)     9740 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/basic.css
--rw-r--r--   0 sander    (1000) sander    (1000)     3500 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 sander    (1000) sander    (1000)     3578 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 sander    (1000) sander    (1000)     3445 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/comment.png
--rw-r--r--   0 sander    (1000) sander    (1000)       42 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/custom.css
--rw-r--r--   0 sander    (1000) sander    (1000)     8166 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/doctools.js
--rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/down.png
--rw-r--r--   0 sander    (1000) sander    (1000)      358 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/file.png
--rw-r--r--   0 sander    (1000) sander    (1000)   282766 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/jquery-1.11.1.js
--rw-r--r--   0 sander    (1000) sander    (1000)    95786 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/jquery.js
--rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/minus.png
--rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/plus.png
--rw-r--r--   0 sander    (1000) sander    (1000)     4149 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/pygments.css
--rw-r--r--   0 sander    (1000) sander    (1000)    18862 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 sander    (1000) sander    (1000)    35168 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 sander    (1000) sander    (1000)    12140 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/underscore.js
--rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/up.png
--rw-r--r--   0 sander    (1000) sander    (1000)    25351 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/_static/websupport.js
--rw-r--r--   0 sander    (1000) sander    (1000)    25780 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/genindex.html
--rw-r--r--   0 sander    (1000) sander    (1000)    68960 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/index.html
--rw-r--r--   0 sander    (1000) sander    (1000)     6140 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/modules.html
--rw-r--r--   0 sander    (1000) sander    (1000)     1101 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/objects.inv
--rw-r--r--   0 sander    (1000) sander    (1000)     7330 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/py-modindex.html
--rw-r--r--   0 sander    (1000) sander    (1000)    58474 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/rowingdata.html
--rw-r--r--   0 sander    (1000) sander    (1000)     3164 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/search.html
--rw-r--r--   0 sander    (1000) sander    (1000)    17380 2023-06-04 14:45:11.000000 rowingdata-3.6.6/docs/_build/html/searchindex.js
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.594417 rowingdata-3.6.6/rowingdata/
--rw-r--r--   0 sander    (1000) sander    (1000)       27 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/__init__.py
--rw-r--r--   0 sander    (1000) sander    (1000)       36 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/__main__.py
--rw-r--r--   0 sander    (1000) sander    (1000)      303 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/boatedit.py
--rw-r--r--   0 sander    (1000) sander    (1000)     6201 2023-11-21 15:51:59.000000 rowingdata-3.6.6/rowingdata/checkdatafiles.py
--rw-r--r--   0 sander    (1000) sander    (1000)      425 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/copystats.py
--rw-r--r--   0 sander    (1000) sander    (1000)      758 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/crewnerdplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      771 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/crewnerdplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)    98758 2023-11-18 13:14:27.000000 rowingdata-3.6.6/rowingdata/csvparsers.py
--rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergdataplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      610 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergdataplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      623 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergdatatotcx.py
--rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergstickplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergstickplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      628 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/ergsticktotcx.py
--rw-r--r--   0 sander    (1000) sander    (1000)     1491 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/gpxtools.py
--rw-r--r--   0 sander    (1000) sander    (1000)     5327 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/gpxwrite.py
--rw-r--r--   0 sander    (1000) sander    (1000)      429 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/konkatenaadje.py
--rw-r--r--   0 sander    (1000) sander    (1000)    13014 2023-11-21 13:19:41.000000 rowingdata-3.6.6/rowingdata/laptesting.py
--rw-r--r--   0 sander    (1000) sander    (1000)    22121 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/obsolete.py
--rw-r--r--   0 sander    (1000) sander    (1000)    23514 2023-11-18 13:14:27.000000 rowingdata-3.6.6/rowingdata/otherparsers.py
--rw-r--r--   0 sander    (1000) sander    (1000)      587 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsled_desktop_plot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      521 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsled_desktop_plottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      569 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsled_desktop_toc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      508 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsledplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      522 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsledplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      441 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/painsledtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      315 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/roweredit.py
--rw-r--r--   0 sander    (1000) sander    (1000)   232014 2024-02-15 15:50:10.000000 rowingdata-3.6.6/rowingdata/rowingdata.py
--rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/rowproplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      609 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/rowproplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/speedcoachplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      613 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/speedcoachplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      691 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/speedcoachtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      694 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/tcxplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      700 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/tcxplot_nogeo.py
--rw-r--r--   0 sander    (1000) sander    (1000)      683 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/tcxplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      689 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/tcxplottime_nogeo.py
--rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/tcxtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)    14568 2023-11-21 09:46:06.000000 rowingdata-3.6.6/rowingdata/tcxtools.py
--rw-r--r--   0 sander    (1000) sander    (1000)     7714 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/trainingparser.py
--rw-r--r--   0 sander    (1000) sander    (1000)     3676 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/utils.py
--rw-r--r--   0 sander    (1000) sander    (1000)     1095 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/windcorrected.py
--rw-r--r--   0 sander    (1000) sander    (1000)    10102 2023-06-04 14:45:11.000000 rowingdata-3.6.6/rowingdata/writetcx.py
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.594417 rowingdata-3.6.6/rowingdata.egg-info/
--rw-r--r--   0 sander    (1000) sander    (1000)    31748 2024-02-15 15:50:27.000000 rowingdata-3.6.6/rowingdata.egg-info/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)     5562 2024-02-15 15:50:27.000000 rowingdata-3.6.6/rowingdata.egg-info/SOURCES.txt
--rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-02-15 15:50:27.000000 rowingdata-3.6.6/rowingdata.egg-info/dependency_links.txt
--rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:56:39.000000 rowingdata-3.6.6/rowingdata.egg-info/not-zip-safe
--rw-r--r--   0 sander    (1000) sander    (1000)      185 2024-02-15 15:50:27.000000 rowingdata-3.6.6/rowingdata.egg-info/requires.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       11 2024-02-15 15:50:27.000000 rowingdata-3.6.6/rowingdata.egg-info/top_level.txt
--rw-r--r--   0 sander    (1000) sander    (1000)      202 2024-02-15 15:50:27.611083 rowingdata-3.6.6/setup.cfg
--rw-r--r--   0 sander    (1000) sander    (1000)     3846 2023-06-04 14:45:11.000000 rowingdata-3.6.6/setup.py
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.607750 rowingdata-3.6.6/testdata/
--rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/2016-03-25-0758.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   416618 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/2016-03-25-0758_data.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    56355 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/2x20min_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    17496 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/3km_cd_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   539777 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/EUBoatCoach.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    97777 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/EmpowerSpeedCoachForce.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    72367 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/NKEmporfromgreg.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   111860 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/NKLiNKv130.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2827124 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/NoHR.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    70850 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/PainsledForce.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   104085 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/RP_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   124341 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/RP_interval.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    63080 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/RP_testdata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    98860 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpdCoach2_imp_inconsistent.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   159697 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpdCoachAmbiguous.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    62781 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpeedCoach GPS Workout.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    17242 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpeedCoach2Link_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   185339 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpeedCoach2Linkv1.27.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    12146 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/SpeedCoach2v2.12.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     4976 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/Speedcoach2example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    53949 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/aritmo.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   459974 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/bc1.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   340372 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/bc2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   365508 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/bc3.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    18887 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/boatcoach.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    95234 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/boatcoach_fixed_distance.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   520154 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/boatcoach_otw.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    74347 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/correctedpainsled.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     5461 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/coxmate.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  1479971 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/crewnerd_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)      381 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/crewnerddata.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)  2945286 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/crewnerddata.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   420603 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/crewnerddata_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)      453 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/cumvalues.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7424 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergdata_example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    11261 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergdata_example.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   462959 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergstick.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   262276 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergstick.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    40411 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergstick2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   231959 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ergstick_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   378971 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   416716 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/example_data.csv
--rw-r--r--   0 sander    (1000) sander    (1000)       17 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/faketcx.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    64254 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/float.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23400 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/herodata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   215236 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/humon.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   157127 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/impeller_empower.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   484172 2023-11-18 12:40:31.000000 rowingdata-3.6.6/testdata/invalidchar.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   115182 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/kinomap.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   397003 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/mystery.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   792595 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/nk_logbook.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    56673 2023-11-18 13:14:27.000000 rowingdata-3.6.6/testdata/painsled.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   369891 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/painsled_desktop_example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    41434 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/painsled_out_data.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   923421 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    76485 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/quiske_per_stroke_left.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   366614 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/quiske_per_stroke_new.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   277062 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/quiske_per_stroke_right.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   511961 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/quiske_per_stroke_seat.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    20254 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/recover.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   106145 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/ritmointervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    14216 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowingdata_eth.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2744646 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowinginmotionexample.TCX
--rw-r--r--   0 sander    (1000) sander    (1000)   657715 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowinginmotionexample.TCX_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   184978 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowperfect.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     4490 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowpro5.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   144225 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rowpro_carrick.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   253794 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rp3_curve.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   420248 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rp3intervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   417209 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rp3intervals2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    85870 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/rp_out.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    41141 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/smartrow.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    34271 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/smartrow_intervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    31104 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/spdcoach2noheader.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    13731 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/speedcoach2test2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7840 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/speedcoach3test3.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    28352 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/speedcoachexample.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23429 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/speedcoachexample.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   422653 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/summarytest.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testdata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    11130 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testdata_part1.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     9315 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testdata_part2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7227 2023-11-22 08:47:10.000000 rowingdata-3.6.6/testdata/testdatasummary.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    19849 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testlapidx.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   427961 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testtcs_210614.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    51127 2023-11-22 08:47:37.000000 rowingdata-3.6.6/testdata/testtcx.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   427951 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/testtcx_210614.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    74249 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/tim.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.6/testdata/划船.csv
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-02-15 15:50:27.607750 rowingdata-3.6.6/tests/
--rw-r--r--   0 sander    (1000) sander    (1000)    27955 2023-11-21 17:59:17.000000 rowingdata-3.6.6/tests/test_rowingdata.py
--rw-r--r--   0 sander    (1000) sander    (1000)     3424 2023-06-04 14:45:11.000000 rowingdata-3.6.6/tests/testparser.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/
+-rw-r--r--   0 sander    (1000) sander    (1000)     1074 2023-06-04 14:45:11.000000 rowingdata-3.6.7/LICENSE
+-rw-r--r--   0 sander    (1000) sander    (1000)      276 2023-06-04 14:45:11.000000 rowingdata-3.6.7/MANIFEST.in
+-rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-13 07:15:45.993515 rowingdata-3.6.7/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)    31386 2023-06-04 14:45:11.000000 rowingdata-3.6.7/README.rst
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.960181 rowingdata-3.6.7/bin/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/crewnerddata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2933658 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    53177 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/testdata.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.953515 rowingdata-3.6.7/docs/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.956848 rowingdata-3.6.7/docs/_build/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.960181 rowingdata-3.6.7/docs/_build/html/
+-rw-r--r--   0 sander    (1000) sander    (1000)      166 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/.buildinfo
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.963515 rowingdata-3.6.7/docs/_build/html/_images/
+-rw-r--r--   0 sander    (1000) sander    (1000)   124024 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/2x20min.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    85796 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/editrower.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156560 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/greghoc.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   118169 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/image001.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    42789 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/otwlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    59925 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/otwscreenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    58348 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/screenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    37995 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/screenshotlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156147 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/woensdag.png
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.963515 rowingdata-3.6.7/docs/_build/html/_sources/
+-rw-r--r--   0 sander    (1000) sander    (1000)      463 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/index.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       67 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/modules.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)     3149 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/rowingdata.txt
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.966848 rowingdata-3.6.7/docs/_build/html/_static/
+-rw-r--r--   0 sander    (1000) sander    (1000)      673 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 sander    (1000) sander    (1000)    10507 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     9740 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/basic.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     3500 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3578 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3445 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment.png
+-rw-r--r--   0 sander    (1000) sander    (1000)       42 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/custom.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     8166 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/down.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      358 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/file.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   282766 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    95786 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     4149 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 sander    (1000) sander    (1000)    18862 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    35168 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    12140 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/up.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    25351 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/websupport.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    25780 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/genindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    68960 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/index.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     6140 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/modules.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     1101 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/objects.inv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7330 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/py-modindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    58474 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/rowingdata.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     3164 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/search.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    17380 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/searchindex.js
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.970181 rowingdata-3.6.7/rowingdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)       27 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/__init__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)       36 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/__main__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      303 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/boatedit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     6404 2024-04-13 07:15:29.000000 rowingdata-3.6.7/rowingdata/checkdatafiles.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      425 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/copystats.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      758 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/crewnerdplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      771 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/crewnerdplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    98961 2024-04-13 07:15:29.000000 rowingdata-3.6.7/rowingdata/csvparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdataplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      610 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdataplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      623 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdatatotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergstickplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergstickplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      628 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergsticktotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1491 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/gpxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     5327 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/gpxwrite.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      429 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/konkatenaadje.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    13014 2024-02-15 15:52:54.000000 rowingdata-3.6.7/rowingdata/laptesting.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    22121 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/obsolete.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    23514 2023-11-18 13:14:27.000000 rowingdata-3.6.7/rowingdata/otherparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      587 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_plot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      521 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_plottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      569 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_toc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      508 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      522 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      441 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      315 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/roweredit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)   243331 2024-04-13 07:15:33.000000 rowingdata-3.6.7/rowingdata/rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/rowproplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      609 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/rowproplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      613 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      691 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      694 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      700 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplot_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      683 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      689 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplottime_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    14568 2023-11-21 09:46:06.000000 rowingdata-3.6.7/rowingdata/tcxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     7714 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/trainingparser.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3676 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/utils.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1095 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/windcorrected.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    10102 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/writetcx.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/rowingdata.egg-info/
+-rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)     5562 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/SOURCES.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/dependency_links.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:56:39.000000 rowingdata-3.6.7/rowingdata.egg-info/not-zip-safe
+-rw-r--r--   0 sander    (1000) sander    (1000)      185 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/requires.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       11 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/top_level.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)      202 2024-04-13 07:15:45.993515 rowingdata-3.6.7/setup.cfg
+-rw-r--r--   0 sander    (1000) sander    (1000)     3846 2023-06-04 14:45:11.000000 rowingdata-3.6.7/setup.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/testdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2016-03-25-0758.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   416618 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2016-03-25-0758_data.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    56355 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2x20min_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17496 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/3km_cd_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   539777 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/EUBoatCoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    97777 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/EmpowerSpeedCoachForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    72367 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NKEmporfromgreg.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   111860 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NKLiNKv130.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2827124 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NoHR.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    70850 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/PainsledForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   104085 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   124341 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_interval.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    63080 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    98860 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpdCoach2_imp_inconsistent.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   159697 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpdCoachAmbiguous.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    62781 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach GPS Workout.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17242 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2Link_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   185339 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2Linkv1.27.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    12146 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2v2.12.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4976 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/Speedcoach2example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    53949 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/aritmo.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   459974 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   340372 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   365508 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    18887 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    95234 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach_fixed_distance.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   520154 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach_otw.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    74347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/correctedpainsled.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     5461 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/coxmate.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  1479971 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerd_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)      381 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)  2945286 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   420603 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)      453 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/cumvalues.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7424 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergdata_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11261 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergdata_example.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   462959 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   262276 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    40411 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   231959 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   378971 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   416716 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/example_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)       17 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/faketcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    64254 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/float.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23400 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/herodata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   215236 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/humon.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   157127 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/impeller_empower.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   484172 2023-11-18 12:40:31.000000 rowingdata-3.6.7/testdata/invalidchar.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   115182 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/kinomap.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   397003 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/mystery.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   792595 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/nk_logbook.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    56673 2023-11-18 13:14:27.000000 rowingdata-3.6.7/testdata/painsled.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   369891 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_desktop_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41434 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_out_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   923421 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    76485 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_left.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   366614 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_new.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   277062 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_right.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   511961 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_seat.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    20254 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/recover.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   106145 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ritmointervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    14216 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowingdata_eth.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2744646 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowinginmotionexample.TCX
+-rw-r--r--   0 sander    (1000) sander    (1000)   657715 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowinginmotionexample.TCX_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   184978 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowperfect.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4490 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowpro5.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   144225 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowpro_carrick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   253794 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3_curve.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   420248 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   417209 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3intervals2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    85870 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp_out.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41141 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/smartrow.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    34271 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/smartrow_intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    31104 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/spdcoach2noheader.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    13731 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoach2test2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7840 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoach3test3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    28352 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoachexample.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23429 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoachexample.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   422653 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/summarytest.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11130 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata_part1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     9315 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata_part2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7061 2024-04-13 07:15:29.000000 rowingdata-3.6.7/testdata/testdatasummary.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    19849 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testlapidx.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   427961 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testtcs_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    51127 2024-04-13 07:12:19.000000 rowingdata-3.6.7/testdata/testtcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   427951 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testtcx_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    74249 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/tim.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/划船.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/tests/
+-rw-r--r--   0 sander    (1000) sander    (1000)    27734 2024-04-13 07:15:29.000000 rowingdata-3.6.7/tests/test_rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3424 2023-06-04 14:45:11.000000 rowingdata-3.6.7/tests/testparser.py
```

### Comparing `rowingdata-3.6.6/LICENSE` & `rowingdata-3.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/PKG-INFO` & `rowingdata-3.6.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: rowingdata
-Version: 3.6.6
-Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
-Home-page: 
-Author: Sander Roosendaal
-Author-email: roosendaalsander@gmail.com
-License: MIT
-Keywords: rowing ergometer concept2
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 **************
 Rowingdata
 **************
 ==============
 Introduction
 ==============
```

### Comparing `rowingdata-3.6.6/README.rst` & `rowingdata-3.6.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: rowingdata
+Version: 3.6.7
+Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
+Home-page: 
+Author: Sander Roosendaal
+Author-email: roosendaalsander@gmail.com
+License: MIT
+Keywords: rowing ergometer concept2
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Requires-Dist: Cython
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: fitparse
+Requires-Dist: arrow>=1.0.2
+Requires-Dist: python-dateutil
+Requires-Dist: docopt
+Requires-Dist: tqdm
+Requires-Dist: rowingphysics>=0.2.3
+Requires-Dist: iso8601
+Requires-Dist: lxml
+Requires-Dist: xmltodict
+Requires-Dist: nose_parameterized
+Requires-Dist: timezonefinder
+Requires-Dist: pycairo
+Requires-Dist: tk
+Requires-Dist: requests
+
 **************
 Rowingdata
 **************
 ==============
 Introduction
 ==============
```

### Comparing `rowingdata-3.6.6/bin/crewnerddata.csv` & `rowingdata-3.6.7/bin/crewnerddata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/bin/crewnerddata.tcx` & `rowingdata-3.6.7/bin/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/bin/testdata.csv` & `rowingdata-3.6.7/bin/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/2x20min.png` & `rowingdata-3.6.7/docs/_build/html/_images/2x20min.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/editrower.JPG` & `rowingdata-3.6.7/docs/_build/html/_images/editrower.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/greghoc.png` & `rowingdata-3.6.7/docs/_build/html/_images/greghoc.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/image001.png` & `rowingdata-3.6.7/docs/_build/html/_images/image001.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/otwlogbook.JPG` & `rowingdata-3.6.7/docs/_build/html/_images/otwlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/otwscreenshot.JPG` & `rowingdata-3.6.7/docs/_build/html/_images/otwscreenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/screenshot.JPG` & `rowingdata-3.6.7/docs/_build/html/_images/screenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/screenshotlogbook.JPG` & `rowingdata-3.6.7/docs/_build/html/_images/screenshotlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_images/woensdag.png` & `rowingdata-3.6.7/docs/_build/html/_images/woensdag.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_sources/rowingdata.txt` & `rowingdata-3.6.7/docs/_build/html/_sources/rowingdata.txt`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/ajax-loader.gif` & `rowingdata-3.6.7/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/alabaster.css` & `rowingdata-3.6.7/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/basic.css` & `rowingdata-3.6.7/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/comment-bright.png` & `rowingdata-3.6.7/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/comment-close.png` & `rowingdata-3.6.7/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/comment.png` & `rowingdata-3.6.7/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/doctools.js` & `rowingdata-3.6.7/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/jquery-1.11.1.js` & `rowingdata-3.6.7/docs/_build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/jquery.js` & `rowingdata-3.6.7/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/pygments.css` & `rowingdata-3.6.7/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/searchtools.js` & `rowingdata-3.6.7/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/underscore-1.3.1.js` & `rowingdata-3.6.7/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/underscore.js` & `rowingdata-3.6.7/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/_static/websupport.js` & `rowingdata-3.6.7/docs/_build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/genindex.html` & `rowingdata-3.6.7/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/index.html` & `rowingdata-3.6.7/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/modules.html` & `rowingdata-3.6.7/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/objects.inv` & `rowingdata-3.6.7/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/py-modindex.html` & `rowingdata-3.6.7/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/rowingdata.html` & `rowingdata-3.6.7/docs/_build/html/rowingdata.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/search.html` & `rowingdata-3.6.7/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/docs/_build/html/searchindex.js` & `rowingdata-3.6.7/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/checkdatafiles.py` & `rowingdata-3.6.7/rowingdata/checkdatafiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import absolute_import
 from __future__ import print_function
+import polars as pl
 
 try:
     from . import rowingdata
 except (ValueError,ImportError):
     import rowingdata
 
 import os
@@ -147,14 +148,19 @@
 
         if notread:
             row = rowingdata.rowingdata(df=row.df)
 
     else:
         row = rowingdata.rowingdata(csvfile=f2)
 
+    row.write_csv(f2+'pl.csv')
+    row2 = rowingdata.rowingdata_pl(csvfile=f2 + 'pl.csv')
+    os.remove(f2 + 'pl.csv')
+    row2 = rowingdata.rowingdata_pl(df=pl.from_pandas(row.df))
+
     nr_of_rows = row.number_of_rows
     distmax = row.df['cum_dist'].max()
     timemax = row.df['TimeStamp (sec)'].max() - row.df['TimeStamp (sec)'].min()
     nrintervals = len(row.df[' lapIdx'].unique())
     mintime = row.df['TimeStamp (sec)'].min()
     maxtime = row.df['TimeStamp (sec)'].max()
     if verbose:
```

### Comparing `rowingdata-3.6.6/rowingdata/crewnerdplot.py` & `rowingdata-3.6.7/rowingdata/crewnerdplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/crewnerdplottime.py` & `rowingdata-3.6.7/rowingdata/crewnerdplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/csvparsers.py` & `rowingdata-3.6.7/rowingdata/csvparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1965,32 +1965,40 @@
         self.to_standard()
 
         # pace column
 
 
 class SmartRowParser(CSVParser):
     def __init__(self, *args, **kwargs):
+        if args:
+            csvfile = args[0]
+        else: # pragma: no cover
+            csvfile = kwargs['csvfile']
+
+        separator = get_separator(5, csvfile)
+        kwargs['sep'] = separator
+
         super(SmartRowParser, self).__init__(*args, **kwargs)
 
         self.cols = [
-            'Second (#)',
+            'Timestamp (UTC)',
             'Distance (m)',
             'Stroke rate (SPM)',
             'Heart rate (bpm)',
             'Actual split (s)',
             'Actual power (W)',
             '', # 'DriveLength (meters)',
             '', #' StrokeDistance (meters)',
             '', #' DriveTime (ms)',
             '', #' DragFactor',
             '', #' StrokeRecoveryTime (ms)',
             '', #' AverageDriveForce (lbs)',
             '', #' PeakDriveForce (lbs)',
             '', #' lapIdx',
-            '', #Second (#)',
+            'Second (#)',
             '', #' latitude',
             '', #' longitude',
             ]
 
         self.cols = [b if a == '' else a
                      for a,b in zip(self.cols, self.defaultcolumnnames)]
         self.columns = dict(list(zip(self.defaultcolumnnames, self.cols)))
```

### Comparing `rowingdata-3.6.6/rowingdata/ergdataplot.py` & `rowingdata-3.6.7/rowingdata/ergdataplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/ergdataplottime.py` & `rowingdata-3.6.7/rowingdata/ergdataplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/ergdatatotcx.py` & `rowingdata-3.6.7/rowingdata/ergdatatotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/ergstickplot.py` & `rowingdata-3.6.7/rowingdata/ergstickplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/ergstickplottime.py` & `rowingdata-3.6.7/rowingdata/ergstickplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/ergsticktotcx.py` & `rowingdata-3.6.7/rowingdata/ergsticktotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/gpxtools.py` & `rowingdata-3.6.7/rowingdata/gpxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/gpxwrite.py` & `rowingdata-3.6.7/rowingdata/gpxwrite.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/laptesting.py` & `rowingdata-3.6.7/rowingdata/laptesting.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/obsolete.py` & `rowingdata-3.6.7/rowingdata/obsolete.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/otherparsers.py` & `rowingdata-3.6.7/rowingdata/otherparsers.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/painsled_desktop_plot.py` & `rowingdata-3.6.7/rowingdata/painsled_desktop_plot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/painsled_desktop_plottime.py` & `rowingdata-3.6.7/rowingdata/painsled_desktop_plottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/painsled_desktop_toc2.py` & `rowingdata-3.6.7/rowingdata/painsled_desktop_toc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/painsledplottime.py` & `rowingdata-3.6.7/rowingdata/painsledplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/rowingdata.py` & `rowingdata-3.6.7/rowingdata/rowingdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=C0103, C0303, C0325, C0413, W0403, W0611
 
 from __future__ import absolute_import
 from __future__ import print_function
 from six.moves import range
 from six.moves import input
 
-__version__ = "3.6.6"
+__version__ = "3.6.7"
 
 from collections import Counter
 
 from matplotlib import figure
 import matplotlib
 try:
     matplotlib.use('TkCairo')
@@ -36,15 +36,15 @@
 import datetime
 import getpass
 
 import math
 from math import cos
 
 import pickle
-
+import gzip
 import time
 import warnings
 import sys
 if sys.version_info < (3,): # pragma: no cover
     warnings.warn(
         """You are using master of 'rowingdata' with Python 2.
         Rowingdata will soon be Python 3 only.""",
@@ -54,14 +54,15 @@
 
 import arrow
 
 import numpy as np
 from numpy import isinf, isnan
 
 import pandas as pd
+import polars as pl
 from pandas import DataFrame, Series
 
 
 from fitparse import FitFile
 
 
 from scipy import integrate
@@ -1774,14 +1775,48 @@
         pass
 
     #df = df.fillna(method='ffill')
     df = df.ffill()
 
     return df
 
+def addpowerzones_pl(df, ftp, powerperc):
+    percut2, percut1, percat, perctr, percan = np.array(powerperc) / 100.
+
+    ut2, ut1, at, tr, an = ftp * np.array(powerperc) / 100.
+
+    df = df.with_columns([
+        (pl.when(pl.col(" Power (watts)") <= ut2).then(pl.col(" Power (watts)"))
+         .otherwise(pl.lit(0))).alias("pw_ut2"),
+        (pl.when(pl.col(" Power (watts)") > ut2, pl.col(" Power (watts)") <= ut1).then(pl.col(" Power (watts)"))
+         .otherwise(pl.lit(0))).alias("pw_ut1"),
+        (pl.when(pl.col(" Power (watts)") > ut1, pl.col(" Power (watts)") <= at).then(pl.col(" Power (watts)"))
+         .otherwise(pl.lit(0))).alias("pw_at"),
+        (pl.when(pl.col(" Power (watts)") > at, pl.col(" Power (watts)") <= tr).then(pl.col(" Power (watts)")).otherwise(pl.lit(0))).alias("pw_tr"),
+        (pl.when(pl.col(" Power (watts)") > tr, pl.col(" Power (watts)") <= an).then(pl.col(" Power (watts)")).otherwise(pl.lit(0))).alias("pw_an"),
+        (pl.when(pl.col(" Power (watts)") > an, pl.col(" Power (watts)") <= 360).then(pl.col(" Power (watts)")).otherwise(pl.lit(0))).alias("pw_max"),
+    ]
+                         )
+
+    return df
+
+
+def addzones_pl(df, ut2, ut1, at, tr, an, mmax):
+    df = df.with_columns([
+        (pl.when(pl.col(" HRCur (bpm)") <= ut2).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_ut2"),
+        (pl.when(pl.col(" HRCur (bpm)") > ut2, pl.col(" HRCur (bpm)") <= ut1).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_ut1"),
+        (pl.when(pl.col(" HRCur (bpm)") > ut1, pl.col(" HRCur (bpm)") <= at).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_at"),
+        (pl.when(pl.col(" HRCur (bpm)") > at, pl.col(" HRCur (bpm)") <= tr).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_tr"),
+        (pl.when(pl.col(" HRCur (bpm)") > tr, pl.col(" HRCur (bpm)") <= an).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_an"),
+        (pl.when(pl.col(" HRCur (bpm)") > an, pl.col(" HRCur (bpm)") <= 360).then(pl.col(" HRCur (bpm)")).otherwise(pl.lit(0))).alias("hr_max"),
+    ]
+                         )
+
+    return df
+
 def addzones(df, ut2, ut1, at, tr, an, mmax):
         # define an additional data frame that will hold the multiple bar plot data and the hr
         # limit data for the plot, it also holds a cumulative distance column
 
     number_of_rows = df.shape[0]
 
     df['hr_ut2'] = np.zeros(number_of_rows)
@@ -1864,14 +1899,257 @@
     vbrel = min([max([vbrel,0]),1])
 
 
     k = int((Nvb-1)*vbrel)
 
     return i,j,k
 
+
+class rowingdata_pl:
+    """
+    This is used if you want to get a polars DataFrame. This class is much more finicky about
+    the data, and might fail reading a csv file where the class rowingdata succeeds.
+
+    There are no plans to exactly reproduce the pandas version's functionality here.
+
+    The intention is to be strict about the width and data types of the resulting data frame. 
+    """
+    def __init__(self, *args, **kwargs):
+        if 'debug' in kwargs: # pragma: no cover
+            debug = kwargs['debug']
+        else:
+            debug = False
+
+        self.debug = debug
+
+        readFile = None
+        if 'csvfile' in kwargs:
+            readFile = kwargs['csvfile']
+
+        rwr = kwargs.get('rower', rower())
+
+        rowtype = kwargs.get('rowtype', 'Indoor Rower')
+            
+
+        sled_df = pl.DataFrame()
+        if 'df' in kwargs:
+            sled_df = kwargs['df']
+            readFile = None
+        elif readFile:
+            try:
+                try:
+                    sled_df = pl.read_csv(readFile,encoding='utf-8', infer_schema_length=1000)
+                except IOError: # pragma: no cover
+                    sled_df = pl.read_csv(readFile + '.gz',encoding='utf-8')
+                except:
+                    sled_df = pl.DataFrame()
+            except IOError: # pragma: no cover
+                try:
+                    f = open(readFile)
+                    sled_df = pl.read_csv(f)
+                    f.close()
+                except IOError:
+                    try:
+                        f = open(readFile + '.gz')
+                        sled_df = pl.read_csv(f)
+                        f.close()
+                    except:
+                        sled_df = pl.DataFrame()
+            except UnicodeEncodeError: # pragma: no cover
+                try:
+                    f = open(readFile)
+                    sled_df = pl.read_csv(f)
+                    f.close()
+                except IOError:
+                    try:
+                        f = open(readFile + '.gz')
+                        sled_df = pl.read_csv(f)
+                        f.close()
+                    except:
+                        sled_df = pl.DataFrame()
+
+
+        self.readfilename = 'rowing dataframe'
+
+        if readFile:
+            try:
+                self.readfilename = readFile.name
+            except AttributeError:
+                self.readfilename = readFile
+
+        self.readFile = readFile
+        self.rwr = rwr
+        self.rowtype = rowtype
+
+        self.empty = False
+        if sled_df.is_empty():
+            self.empty = True
+
+        othernames = ['catch','finish','peakforceangle',
+                      'wash','slip','index',
+                      'cum_dist',
+                      'hr_an','hr_at','hr_tr','hr_ut1','hr_ut2','hr_max',
+#                      'lim_an','lim_at','lim_tr','lim_ut1','lim_ut2',
+#                      'limpw_an','limpw_at','limpw_tr',
+#                      'limpw_ut1','limpw_ut2',
+                      'pw_an','pw_at','pw_max','pw_tr','pw_ut1','pw_ut2',
+#                      'lim_max','hr_max',
+                      ' latitude',' longitude']
+
+        # check for missing column names
+        mandatorynames = [
+            'TimeStamp (sec)',
+            ' Horizontal (meters)',
+            ' Cadence (stokes/min)',
+            ' HRCur (bpm)',
+            ' Stroke500mPace (sec/500m)',
+            ' Power (watts)',
+            ' DriveLength (meters)',
+            ' StrokeDistance (meters)',
+            ' DriveTime (ms)',
+            ' DragFactor',
+            ' StrokeRecoveryTime (ms)',
+            ' AverageDriveForce (lbs)',
+            ' AverageBoatSpeed (m/s)',
+            ' PeakDriveForce (lbs)',
+            ' AverageDriveForce (N)',
+            ' PeakDriveForce (N)',
+            ' lapIdx',
+            ' ElapsedTime (sec)',
+            ' Calories (kCal)',
+            ' WorkoutState',
+        ]
+
+
+        self.defaultnames = othernames+mandatorynames
+
+        if readFile and not sled_df.is_empty():
+            for name in self.defaultnames:
+                if name in sled_df.columns:
+                    if sled_df[name].dtype == pl.String:
+                        if name != ' lapIdx':
+                            sled_df = sled_df.with_columns(
+                                (pl.col(name).str.strip_chars_start()).cast(pl.Float64).alias(name)
+                            )
+                
+
+        if ' ElapsedTime (sec)' not in sled_df.columns and not sled_df.is_empty():
+            sled_df = sled_df.with_columns((pl.col("TimeStamp (sec)")-sled_df[0, "TimeStamp (sec)"]).alias(" ElapsedTime (sec)"))
+
+        if not sled_df.is_empty():
+            for name in self.defaultnames:
+                if name not in sled_df.columns:
+                    if debug:
+                        print(name + " is not found in data")
+                    sled_df = sled_df.with_columns((pl.lit(0)).alias(name))
+                    if name == "TimeStamp (sec)":
+                        sled_df = sled_df.rename({"TimeStamp (sec utc)" : name})
+                    if name == ' WorkoutState':
+                        sled_df = sled_df.with_columns((pl.lit(4)).alias(name))
+                    if name == ' Calories (kCal)':
+                        sled_df = sled_df.with_columns((pl.lit(1)).alias(name))
+                    if name == ' Stroke500mPace (sec/500m)': # pragma: no cover
+                        dd = sled_df[' Horizontal (meters)'].diff()
+                        dt = sled_df[' ElapsedTime (sec)'].diff()
+                        velo = dd / dt
+                        sled_df = sled_df.with_columns((500. / velo).alias(name))
+                    if name == ' AverageBoatSpeed (m/s)':
+                        try:
+                            velo = 500./sled_df[' Stroke500mPace (sec/500m)']
+                        except (KeyError,ValueError): # pragma: no cover
+                            dd = sled_df[' Horizontal (meters)'].diff()
+                            dt = sled_df[' ElapsedTime (sec)'].diff()
+                            velo = dd / dt
+                        sled_df = sled_df.with_columns((velo).alias(name))
+                    if name == ' AverageDriveForce (lbs)':
+                        try: # pragma: no cover
+                            forcen = sled_df[' AverageDriveForce (N)']
+                            sled_df = sled_df.with_columns((pl.col(" AverageDriveForce (lbs)") / lbstoN).alias(name))
+                        except (KeyError, TypeError):
+                            sled_df = sled_df.with_columns((pl.lit(0)).alias(name))
+                    if name == ' AverageDriveForce (N)':
+                        try:
+                            forcelbs = sled_df[' AverageDriveForce (lbs)']
+                            sled_df = sled_df.with_columns((pl.col(" AverageDriveForce (lbs)") * lbstoN).alias(name))
+                        except KeyError: # pragma: no cover
+                            sled_df = sled_df.with_columns((pl.lit(0)).alias(name))
+                    if name == ' PeakDriveForce (lbs)':
+                        try: # pragma: no cover
+                            forcen = sled_df[' PeakDriveForce (N)']
+                            sled_df = sled_df.with_columns((pl.col(forcen / lbstoN).alias(name)))
+                        except (KeyError, TypeError):
+                            sled_df = sled_df.with_columns((pl.lit(0)).alias(name))
+                    if name == ' PeakDriveForce (N)':
+                        try:
+                            forcelbs = sled_df[' PeakDriveForce (lbs)']
+                            sled_df = sled_df.with_columns((pl.col(" PeakDriveForce (lbs)") * lbstoN).alias(name))
+                        except KeyError: # pragma: no cover
+                            sled_df = sled_df.with_columns((pl.lit(0)).alias(name))
+                    if name == ' Cadence (stokes/min)':
+                        try:
+                            spm = sled_df[' Cadence (strokes/min)']
+                            if debug: # pragma: no cover
+                                print('Cadence found')
+                            sled_df = sled_df.with_columns((spm).alias(name))
+                        except KeyError: # pragma: no cover
+                            pass
+
+        sled_df = sled_df.drop([c for c in sled_df.columns if c not in self.defaultnames])
+
+        # add drive energy
+        sled_df = sled_df.with_columns((pl.col(" Power (watts)")/pl.col(" Cadence (stokes/min)")).alias("driveenergy"))
+
+        self.duration = 0
+        
+        if not sled_df.is_empty():
+            sled_df = addzones_pl(
+                sled_df,
+                self.rwr.ut2,
+                self.rwr.ut1,
+                self.rwr.at,
+                self.rwr.tr,
+                self.rwr.an,
+                self.rwr.max
+            )
+
+            sled_df = sled_df.filter(pl.col(" WorkoutState") != 12)
+            sled_df = sled_df.with_columns(pl.col(" Cadence (stokes/min)").cast(pl.Float64))
+
+            sled_df = addpowerzones_pl(sled_df, self.rwr.ftp, self.rwr.powerperc)
+
+            self.duration = sled_df['TimeStamp (sec)'].max()-sled_df['TimeStamp (sec)'].min()
+            
+        self.df = sled_df
+        self.number_of_rows = self.df.shape[0]
+
+
+    def write_csv(self, writeFile, compressed=False):
+        data = self.df.clone()
+        data = data.drop([
+            'hr_ut2',
+            'hr_ut1',
+            'hr_at',
+            'hr_tr',
+            'hr_an',
+            'hr_max',
+            'pw_ut2',
+            'pw_ut1',
+            'pw_at',
+            'pw_tr',
+            'pw_an',
+            'pw_max',
+        ])
+
+        if compressed:
+            with gzip.open(writeFile + '.gz','wb') as f:
+                return data.write_csv(f)
+
+        return data.write_csv(writeFile)
+            
+
 class rowingdata:
     """ This is the main class. Read the data from the csv file and do all
     kinds
     of cool stuff with it.
 
     Usage: row=rowingdata.rowingdata(csvfile="testdata.csv",
                                        rowtype="Indoor Rower",
@@ -2093,19 +2371,14 @@
             pass
 
         if len(sled_df):
             # Remove zeros from HR
             hrmean = sled_df[' HRCur (bpm)'].mean()
             hrstd = sled_df[' HRCur (bpm)'].std()
 
-            if hrmean != 0 and hrstd != 0:
-                sled_df[' HRCur (bpm)'].replace(to_replace=0, value=np.nan,
-                                                inplace=True)
-                sled_df[' HRCur (bpm)'].ffill(inplace=True)
-
             self.dragfactor = sled_df[' DragFactor'].mean()
             # do stroke count
             dt = sled_df['TimeStamp (sec)'].diff()
             dstroke = dt*sled_df[' Cadence (stokes/min)']/60.
             self.stroke_count = int(dstroke.sum())
         else:
             self.dragfactor = 0
@@ -2169,15 +2442,16 @@
             sled_df['driveenergy'] = 0
 
         # these parameters are handy to have available in other routines
         self.number_of_rows = number_of_rows
 
         # add HR zone data to dataframe
         if len(sled_df):
-            self.df = addzones(sled_df, self.rwr.ut2,
+            self.df = addzones(sled_df,
+                               self.rwr.ut2,
                                self.rwr.ut1,
                                self.rwr.at,
                                self.rwr.tr,
                                self.rwr.an,
                                self.rwr.max
             )
         else:
@@ -2195,15 +2469,15 @@
 
         # duration
         if len(sled_df):
             self.duration = self.df['TimeStamp (sec)'].max()-self.df['TimeStamp (sec)'].min()
         else:
             self.duration = 0
 
-
+            
     def __add__(self, other):
         self_df = self.df.copy()
         other_df = other.df.copy()
 
         if self.empty: # pragma: no cover
             return other
         if len(self.df) < 30: # pragma: no cover
@@ -2274,28 +2548,14 @@
                           rowtype=self.rowtype,
                           absolutetimestamps=self.absolutetimestamps)
 
     def change_drag(self, dragfactor): # pragma: no cover
         self.df[' DragFactor'] = dragfactor
         self.dragfactor = dragfactor
 
-    def get_minutes_averages(self, columnname):
-        """ Returns a list of values, the mean for each minute of the session
-        """
-
-        df = self.df.copy()
-        df['dt'] = df['TimeStamp (sec)'].apply(lambda x: arrow.get(x).datetime)
-        df.set_index('dt',inplace=True)
-
-        try:
-            result = df[columnname].resample('T').mean().values
-        except KeyError:
-            return []
-
-        return result
 
     def getvalues(self, keystring):
         """ Just a tool to get a column of the row data as a numpy array
 
         You can also just access row.df[keystring] to get a pandas Series
 
         """
```

### Comparing `rowingdata-3.6.6/rowingdata/rowproplot.py` & `rowingdata-3.6.7/rowingdata/rowproplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/rowproplottime.py` & `rowingdata-3.6.7/rowingdata/rowproplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/speedcoachplot.py` & `rowingdata-3.6.7/rowingdata/speedcoachplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/speedcoachplottime.py` & `rowingdata-3.6.7/rowingdata/speedcoachplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/speedcoachtoc2.py` & `rowingdata-3.6.7/rowingdata/speedcoachtoc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxplot.py` & `rowingdata-3.6.7/rowingdata/tcxplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxplot_nogeo.py` & `rowingdata-3.6.7/rowingdata/tcxplot_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxplottime.py` & `rowingdata-3.6.7/rowingdata/tcxplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxplottime_nogeo.py` & `rowingdata-3.6.7/rowingdata/tcxplottime_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxtoc2.py` & `rowingdata-3.6.7/rowingdata/tcxtoc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/tcxtools.py` & `rowingdata-3.6.7/rowingdata/tcxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/trainingparser.py` & `rowingdata-3.6.7/rowingdata/trainingparser.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/utils.py` & `rowingdata-3.6.7/rowingdata/utils.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/windcorrected.py` & `rowingdata-3.6.7/rowingdata/windcorrected.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata/writetcx.py` & `rowingdata-3.6.7/rowingdata/writetcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/rowingdata.egg-info/PKG-INFO` & `rowingdata-3.6.7/rowingdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 Metadata-Version: 2.1
 Name: rowingdata
-Version: 3.6.6
+Version: 3.6.7
 Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
 Home-page: 
 Author: Sander Roosendaal
 Author-email: roosendaalsander@gmail.com
 License: MIT
 Keywords: rowing ergometer concept2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: Cython
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: fitparse
+Requires-Dist: arrow>=1.0.2
+Requires-Dist: python-dateutil
+Requires-Dist: docopt
+Requires-Dist: tqdm
+Requires-Dist: rowingphysics>=0.2.3
+Requires-Dist: iso8601
+Requires-Dist: lxml
+Requires-Dist: xmltodict
+Requires-Dist: nose_parameterized
+Requires-Dist: timezonefinder
+Requires-Dist: pycairo
+Requires-Dist: tk
+Requires-Dist: requests
 
 **************
 Rowingdata
 **************
 ==============
 Introduction
 ==============
```

### Comparing `rowingdata-3.6.6/rowingdata.egg-info/SOURCES.txt` & `rowingdata-3.6.7/rowingdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/setup.py` & `rowingdata-3.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/2016-03-25-0758.CSV` & `rowingdata-3.6.7/testdata/2016-03-25-0758.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/2016-03-25-0758_data.CSV` & `rowingdata-3.6.7/testdata/2016-03-25-0758_data.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/2x20min_o.csv` & `rowingdata-3.6.7/testdata/2x20min_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/3km_cd_o.csv` & `rowingdata-3.6.7/testdata/3km_cd_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/EUBoatCoach.csv` & `rowingdata-3.6.7/testdata/EUBoatCoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/EmpowerSpeedCoachForce.csv` & `rowingdata-3.6.7/testdata/EmpowerSpeedCoachForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/NKEmporfromgreg.csv` & `rowingdata-3.6.7/testdata/NKEmporfromgreg.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/NKLiNKv130.csv` & `rowingdata-3.6.7/testdata/NKLiNKv130.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/NoHR.tcx` & `rowingdata-3.6.7/testdata/NoHR.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/PainsledForce.csv` & `rowingdata-3.6.7/testdata/PainsledForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/RP_interval.csv` & `rowingdata-3.6.7/testdata/RP_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/RP_interval.csv_o.CSV` & `rowingdata-3.6.7/testdata/RP_interval.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/RP_testdata.csv` & `rowingdata-3.6.7/testdata/RP_testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpdCoach2_imp_inconsistent.csv` & `rowingdata-3.6.7/testdata/SpdCoach2_imp_inconsistent.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpdCoachAmbiguous.csv` & `rowingdata-3.6.7/testdata/SpdCoachAmbiguous.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpeedCoach GPS Workout.csv` & `rowingdata-3.6.7/testdata/SpeedCoach GPS Workout.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpeedCoach2Link_interval.csv` & `rowingdata-3.6.7/testdata/SpeedCoach2Link_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpeedCoach2Linkv1.27.csv` & `rowingdata-3.6.7/testdata/SpeedCoach2Linkv1.27.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/SpeedCoach2v2.12.csv` & `rowingdata-3.6.7/testdata/SpeedCoach2v2.12.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/Speedcoach2example.csv` & `rowingdata-3.6.7/testdata/Speedcoach2example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/aritmo.csv` & `rowingdata-3.6.7/testdata/aritmo.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/bc1.csv` & `rowingdata-3.6.7/testdata/bc1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/bc2.csv` & `rowingdata-3.6.7/testdata/bc2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/bc3.csv` & `rowingdata-3.6.7/testdata/bc3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/boatcoach.csv` & `rowingdata-3.6.7/testdata/boatcoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/boatcoach_fixed_distance.csv` & `rowingdata-3.6.7/testdata/boatcoach_fixed_distance.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/boatcoach_otw.csv` & `rowingdata-3.6.7/testdata/boatcoach_otw.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/correctedpainsled.csv` & `rowingdata-3.6.7/testdata/correctedpainsled.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/coxmate.csv` & `rowingdata-3.6.7/testdata/coxmate.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/crewnerd_interval.csv` & `rowingdata-3.6.7/testdata/crewnerd_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/crewnerddata.tcx` & `rowingdata-3.6.7/testdata/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/crewnerddata_o.CSV` & `rowingdata-3.6.7/testdata/crewnerddata_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergdata_example.csv` & `rowingdata-3.6.7/testdata/ergdata_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergdata_example.csv_o.CSV` & `rowingdata-3.6.7/testdata/ergdata_example.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergstick.csv` & `rowingdata-3.6.7/testdata/ergstick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergstick.csv_o.CSV` & `rowingdata-3.6.7/testdata/ergstick.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergstick2.csv` & `rowingdata-3.6.7/testdata/ergstick2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ergstick_o.csv` & `rowingdata-3.6.7/testdata/ergstick_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/example.csv` & `rowingdata-3.6.7/testdata/example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/example_data.csv` & `rowingdata-3.6.7/testdata/example_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/float.csv` & `rowingdata-3.6.7/testdata/float.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/herodata.csv` & `rowingdata-3.6.7/testdata/herodata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/humon.csv` & `rowingdata-3.6.7/testdata/humon.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/impeller_empower.csv` & `rowingdata-3.6.7/testdata/impeller_empower.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/invalidchar.tcx` & `rowingdata-3.6.7/testdata/invalidchar.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/kinomap.csv` & `rowingdata-3.6.7/testdata/kinomap.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/mystery.csv` & `rowingdata-3.6.7/testdata/mystery.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/nk_logbook.csv` & `rowingdata-3.6.7/testdata/nk_logbook.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/painsled.tcx` & `rowingdata-3.6.7/testdata/painsled.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/painsled_desktop_example.csv` & `rowingdata-3.6.7/testdata/painsled_desktop_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/painsled_out_data.csv` & `rowingdata-3.6.7/testdata/painsled_out_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv` & `rowingdata-3.6.7/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/quiske_per_stroke_left.csv` & `rowingdata-3.6.7/testdata/quiske_per_stroke_left.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/quiske_per_stroke_new.csv` & `rowingdata-3.6.7/testdata/quiske_per_stroke_new.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/quiske_per_stroke_right.csv` & `rowingdata-3.6.7/testdata/quiske_per_stroke_right.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/quiske_per_stroke_seat.csv` & `rowingdata-3.6.7/testdata/quiske_per_stroke_seat.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/recover.tcx` & `rowingdata-3.6.7/testdata/recover.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/ritmointervals.csv` & `rowingdata-3.6.7/testdata/ritmointervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowingdata_eth.csv` & `rowingdata-3.6.7/testdata/rowingdata_eth.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowinginmotionexample.TCX` & `rowingdata-3.6.7/testdata/rowinginmotionexample.TCX`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowinginmotionexample.TCX_o.CSV` & `rowingdata-3.6.7/testdata/rowinginmotionexample.TCX_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowperfect.csv` & `rowingdata-3.6.7/testdata/rowperfect.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowpro5.csv` & `rowingdata-3.6.7/testdata/rowpro5.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rowpro_carrick.csv` & `rowingdata-3.6.7/testdata/rowpro_carrick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rp3_curve.csv` & `rowingdata-3.6.7/testdata/rp3_curve.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rp3intervals.csv` & `rowingdata-3.6.7/testdata/rp3intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rp3intervals2.csv` & `rowingdata-3.6.7/testdata/rp3intervals2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/rp_out.csv` & `rowingdata-3.6.7/testdata/rp_out.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/smartrow.csv` & `rowingdata-3.6.7/testdata/smartrow.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/smartrow_intervals.csv` & `rowingdata-3.6.7/testdata/smartrow_intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/spdcoach2noheader.csv` & `rowingdata-3.6.7/testdata/spdcoach2noheader.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/speedcoach2test2.csv` & `rowingdata-3.6.7/testdata/speedcoach2test2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/speedcoach3test3.csv` & `rowingdata-3.6.7/testdata/speedcoach3test3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/speedcoachexample.csv` & `rowingdata-3.6.7/testdata/speedcoachexample.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/speedcoachexample.csv_o.CSV` & `rowingdata-3.6.7/testdata/speedcoachexample.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/summarytest.csv` & `rowingdata-3.6.7/testdata/summarytest.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testdata.csv` & `rowingdata-3.6.7/testdata/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testdata_part1.csv` & `rowingdata-3.6.7/testdata/testdata_part1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testdata_part2.csv` & `rowingdata-3.6.7/testdata/testdata_part2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testdatasummary.csv` & `rowingdata-3.6.7/testdata/testdatasummary.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 filename,type,nr_lines,year,month,day,hour,minute,second,dist,seconds,nrintervals,lap 1 time,lap 1 dist,timezone,lap 1 time new,lap 1 dist new,,,,
 quiske_per_stroke_new.csv,quiske,139,2022,11,7,7,58,35,930,382,1,382,930,UTC,382,928,,,,
 boatcoach_fixed_distance.csv,boatcoach,493,2022,6,13,12,31,37,1996,495,4,109,494,UTC,109,494,,,,
-smartrow_intervals.csv,smartrow,739,0,0,0,0,0,0,6979,2335,1,2335,6979,UTC,2335,6970,,,,
-smartrow.csv,smartrow,878,0,0,0,0,0,0,7836,3005,1,3005,7836,UTC,3005,7829,,,,
 rowpro_carrick.csv,rp,1212,2022,1,19,17,33,0,10023,3608,10,422,1495,UTC,422,1493,,,,
 fromnk.csv.gz,nklinklogbook,430,2021,7,7,17,33,28,3005,1062,12,60,250,UTC,60,250,,,,
 herodata.csv,hero,300,2021,4,26,13,37,33,3512,896,1,896,3512,UTC,896,3509,,,,
 nk_logbook.csv,nklinklogbook,1613,2021,3,30,11,13,4,12155,3901,1,3901,12155,UTC,3901,12155,,,,
 SpdCoachAmbiguous.csv,speedcoach2,0,2021,0,0,0,0,0,0,0,0,0,0,UTC,0,0,,,,
 rowingdata_eth.csv,eth,45,0,0,0,0,0,0,481,122,1,122,481,UTC,122,469,,,,
 spdcoach2noheader.csv,speedcoach2,255,0,0,0,0,0,0,2372,737,1,737,2372,UTC,737,2366,,,,
```

### Comparing `rowingdata-3.6.6/testdata/testlapidx.csv` & `rowingdata-3.6.7/testdata/testlapidx.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testtcs_210614.tcx` & `rowingdata-3.6.7/testdata/testtcs_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/testtcx.tcx` & `rowingdata-3.6.7/testdata/testtcx.tcx`

 * *Files 0% similar despite different names*

#### Comparing `rowingdata-3.6.6/testdata/testtcx.tcx` & `rowingdata-3.6.7/testdata/testtcx.tcx`

```diff
@@ -1276,15 +1276,15 @@
               <TPX xmlns="http://www.garmin.com/xmlschemas/ActivityExtension/v2">
                 <Watts>0</Watts>
               </TPX>
             </Extensions>
           </Trackpoint>
         </Track>
       </Lap>
-      <Notes>&lt;Element 'Notes' at 0x7f4989bccae0&gt;</Notes>
+      <Notes>&lt;Element 'Notes' at 0x7f7e54795680&gt;</Notes>
     </Activity>
   </Activities>
   <Creator>
     <Name>rowsandall.com/rowingdata</Name>
   </Creator>
   <Author xsi:type="Application_t">
     <Name>rowingdata</Name>
```

### Comparing `rowingdata-3.6.6/testdata/testtcx_210614.tcx` & `rowingdata-3.6.7/testdata/testtcx_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/tim.csv` & `rowingdata-3.6.7/testdata/tim.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/testdata/划船.csv` & `rowingdata-3.6.7/testdata/划船.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.6/tests/test_rowingdata.py` & `rowingdata-3.6.7/tests/test_rowingdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,20 +254,14 @@
         assert_equal(t2,d2)
         assert_equal(t3,d3)
         assert_equal(t4,d4)
         assert_equal(t5,d5)
         assert_equal(t6,d6)
         assert_equal(t7,d7)
 
-class TestMinutes:
-    def test_minutes(self):
-        row = rowingdata.rowingdata(csvfile='testdata/testdata.csv')
-
-        res = row.get_minutes_averages(' Cadence (stokes/min)')
-        assert_equal(len(res),9)
 
 class TestPhysics:
     row = rowingdata.rowingdata(csvfile='testdata/testdata.csv')
 
     def test_getpower(self):
         velo = 4.0
         r = rowingdata.getrower()
@@ -727,15 +721,15 @@
     def test_check(self, name, filename, expected):
         f2='testdata/'+filename
         res=rowingdata.checkdatafiles.checkfile(f2)
         filetype = rowingdata.get_file_type(f2)
         if filetype  not in ['unknown','c2log']:
             assert_not_equal(res,0)
         if res != 0:
-            for key,value in six.iteritems(res):
+            for key,value in res.items():
                 if key not in ['summary']:
                     if expected[key] != 0:
                         assert_equal(value,expected[key])
                 elif key == 'summary':
                     assert_not_equal(value,'')
```

### Comparing `rowingdata-3.6.6/tests/testparser.py` & `rowingdata-3.6.7/tests/testparser.py`

 * *Files identical despite different names*

