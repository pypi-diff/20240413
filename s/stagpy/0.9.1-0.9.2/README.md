# Comparing `tmp/stagpy-0.9.1.tar.gz` & `tmp/stagpy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stagpy-0.9.1.tar", last modified: Wed Mar 14 20:33:15 2018, max compression
+gzip compressed data, was "dist/stagpy-0.9.2.tar", last modified: Fri Apr 20 11:59:28 2018, max compression
```

## Comparing `stagpy-0.9.1.tar` & `stagpy-0.9.2.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/
--rw-r--r--   0 adrien    (1000) adrien    (1000)    18027 2017-07-01 16:31:14.000000 stagpy-0.9.1/LICENSE
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2114 2018-03-14 20:33:15.000000 stagpy-0.9.1/PKG-INFO
--rw-r--r--   0 adrien    (1000) adrien    (1000)      280 2018-01-25 17:56:39.000000 stagpy-0.9.1/.travis.yml
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/docs/
--rw-r--r--   0 adrien    (1000) adrien    (1000)    10218 2018-01-19 11:27:10.000000 stagpy-0.9.1/docs/conf.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     7249 2017-07-01 16:31:14.000000 stagpy-0.9.1/docs/make.bat
--rw-r--r--   0 adrien    (1000) adrien    (1000)     7656 2017-07-01 16:31:14.000000 stagpy-0.9.1/docs/Makefile
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/docs/sources/
--rw-r--r--   0 adrien    (1000) adrien    (1000)      836 2018-01-25 01:43:01.000000 stagpy-0.9.1/docs/sources/maintainers.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     8328 2018-01-17 23:24:22.000000 stagpy-0.9.1/docs/sources/stagyydata.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2008 2018-01-03 11:14:00.000000 stagpy-0.9.1/docs/sources/cli.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5846 2018-01-10 19:31:26.000000 stagpy-0.9.1/docs/sources/cookbook.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     4660 2018-01-10 18:51:59.000000 stagpy-0.9.1/docs/sources/tuto.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     3531 2018-02-11 19:17:16.000000 stagpy-0.9.1/docs/sources/developers.rst
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/docs/sources/apiref/
--rw-r--r--   0 adrien    (1000) adrien    (1000)       63 2018-01-12 19:13:08.000000 stagpy-0.9.1/docs/sources/apiref/args.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       79 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/stagyyparsers.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       64 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/commands.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2793 2018-01-08 00:01:00.000000 stagpy-0.9.1/docs/sources/apiref/phyvars.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       62 2018-01-13 23:48:36.000000 stagpy-0.9.1/docs/sources/apiref/plates.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)      148 2018-01-07 23:50:43.000000 stagpy-0.9.1/docs/sources/apiref/stagyydata.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)      396 2018-01-11 18:55:03.000000 stagpy-0.9.1/docs/sources/apiref/parfile.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/error.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       70 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/processing.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/field.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       73 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/time.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)      514 2018-02-19 16:39:55.000000 stagpy-0.9.1/docs/sources/apiref/config.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)      629 2018-01-30 00:17:34.000000 stagpy-0.9.1/docs/sources/apiref/stagpy.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       52 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/misc.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2017-12-30 16:34:21.000000 stagpy-0.9.1/docs/sources/apiref/rprof.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2121 2018-02-11 19:17:16.000000 stagpy-0.9.1/docs/sources/install.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)      982 2018-01-13 23:47:54.000000 stagpy-0.9.1/docs/index.rst
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/tests/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1033 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_commands.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      880 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_field.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      523 2018-01-28 12:12:07.000000 stagpy-0.9.1/tests/conftest.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      147 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_init.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1713 2018-01-25 18:05:48.000000 stagpy-0.9.1/tests/test_stagyydata.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1462 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_processing.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      449 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_rprof.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2061 2018-01-29 00:47:50.000000 stagpy-0.9.1/tests/test_args.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      978 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_misc.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1413 2018-02-20 23:31:09.000000 stagpy-0.9.1/tests/test_parsers.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      713 2018-02-21 23:44:59.000000 stagpy-0.9.1/tests/test_parfile.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      548 2018-01-25 01:44:08.000000 stagpy-0.9.1/tests/test_time_series.py
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     7520 2018-02-26 23:57:09.000000 stagpy-0.9.1/stagpy/field.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)    31936 2018-03-06 19:10:11.000000 stagpy-0.9.1/stagpy/stagyydata.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)    25325 2018-03-14 19:54:34.000000 stagpy-0.9.1/stagpy/stagyyparsers.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)    18410 2018-02-21 23:30:55.000000 stagpy-0.9.1/stagpy/parfile.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5700 2018-02-28 18:19:56.000000 stagpy-0.9.1/stagpy/error.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     6013 2018-02-28 18:35:42.000000 stagpy-0.9.1/stagpy/time_series.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)    37722 2018-02-11 19:33:13.000000 stagpy-0.9.1/stagpy/plates.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     3145 2018-03-14 00:11:17.000000 stagpy-0.9.1/stagpy/args.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5862 2018-02-24 18:02:54.000000 stagpy-0.9.1/stagpy/rprof.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2338 2018-03-13 23:33:00.000000 stagpy-0.9.1/stagpy/__init__.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)      880 2018-02-11 19:32:35.000000 stagpy-0.9.1/stagpy/__main__.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5740 2018-03-13 23:29:32.000000 stagpy-0.9.1/stagpy/config.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     6424 2018-02-25 18:56:03.000000 stagpy-0.9.1/stagpy/misc.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5227 2018-03-14 19:30:28.000000 stagpy-0.9.1/stagpy/commands.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)    10283 2018-02-22 19:08:10.000000 stagpy-0.9.1/stagpy/processing.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     8031 2018-02-11 19:33:04.000000 stagpy-0.9.1/stagpy/phyvars.py
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1146 2018-02-19 16:32:27.000000 stagpy-0.9.1/README.rst
--rw-r--r--   0 adrien    (1000) adrien    (1000)       38 2018-03-14 20:33:15.000000 stagpy-0.9.1/setup.cfg
--rw-r--r--   0 adrien    (1000) adrien    (1000)      209 2018-01-25 01:44:08.000000 stagpy-0.9.1/tox.ini
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1355 2018-03-14 20:31:11.000000 stagpy-0.9.1/setup.py
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/annulus/
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/annulus/+op/
--rw-r--r--   0 adrien    (1000) adrien    (1000)   529304 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/annulus/+op/test_vp00100
--rw-r--r--   0 adrien    (1000) adrien    (1000)  2308018 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/annulus/+op/test_time.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)    68496 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/annulus/+op/test_t00100
--rw-r--r--   0 adrien    (1000) adrien    (1000)  2969199 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/annulus/+op/test_rprof.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)      993 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/annulus/par
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-1000/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1188 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/par
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-1000/Op/
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_time.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_vp00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_t00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-1000/Op/out_rprof.dat
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-10000/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1189 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/par
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-10000/Op/
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_time.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_vp00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_t00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-10000/Op/out_rprof.dat
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-100000/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1190 2018-01-11 18:47:53.000000 stagpy-0.9.1/Examples/ra-100000/par
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/Examples/ra-100000/Op/
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00002
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_time.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00001
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00003
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_vp00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00000
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00005
--rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_t00004
--rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-07-01 16:31:14.000000 stagpy-0.9.1/Examples/ra-100000/Op/out_rprof.dat
--rw-r--r--   0 adrien    (1000) adrien    (1000)     1270 2018-02-19 16:32:27.000000 stagpy-0.9.1/Makefile
--rw-r--r--   0 adrien    (1000) adrien    (1000)      191 2018-01-25 01:44:08.000000 stagpy-0.9.1/.landscape.yml
--rw-r--r--   0 adrien    (1000) adrien    (1000)      119 2018-02-10 23:21:51.000000 stagpy-0.9.1/.gitignore
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     2114 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/PKG-INFO
--rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/dependency_links.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)        7 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/top_level.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)       49 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/entry_points.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)     3127 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/SOURCES.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)      126 2018-03-14 20:33:15.000000 stagpy-0.9.1/stagpy.egg-info/requires.txt
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     3142 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      126 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/requires.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       49 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/entry_points.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2077 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        7 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy.egg-info/top_level.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1294 2018-04-18 09:02:37.000000 stagpy-0.9.2/Makefile
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/docs/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     7656 2017-01-24 11:37:56.000000 stagpy-0.9.2/docs/Makefile
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     7249 2017-01-24 11:37:56.000000 stagpy-0.9.2/docs/make.bat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      982 2018-01-15 08:34:53.000000 stagpy-0.9.2/docs/index.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    10218 2018-01-22 08:52:51.000000 stagpy-0.9.2/docs/conf.py
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/docs/sources/
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/docs/sources/apiref/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       63 2018-01-15 08:34:53.000000 stagpy-0.9.2/docs/sources/apiref/args.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       73 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/time.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       62 2018-01-15 08:34:53.000000 stagpy-0.9.2/docs/sources/apiref/plates.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/field.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      514 2018-02-20 09:22:07.000000 stagpy-0.9.2/docs/sources/apiref/config.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/rprof.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       52 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/misc.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2793 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/phyvars.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       79 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/stagyyparsers.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       70 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/processing.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       64 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/commands.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      629 2018-01-30 09:13:35.000000 stagpy-0.9.2/docs/sources/apiref/stagpy.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       55 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/error.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      396 2018-01-12 09:20:59.000000 stagpy-0.9.2/docs/sources/apiref/parfile.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      148 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/apiref/stagyydata.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5846 2018-01-11 08:53:14.000000 stagpy-0.9.2/docs/sources/cookbook.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     4660 2018-01-11 08:53:14.000000 stagpy-0.9.2/docs/sources/tuto.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2121 2018-02-12 09:08:48.000000 stagpy-0.9.2/docs/sources/install.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     3531 2018-02-12 09:08:48.000000 stagpy-0.9.2/docs/sources/developers.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      836 2018-01-25 08:57:48.000000 stagpy-0.9.2/docs/sources/maintainers.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2008 2018-01-08 08:31:09.000000 stagpy-0.9.2/docs/sources/cli.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     8328 2018-01-18 09:33:56.000000 stagpy-0.9.2/docs/sources/stagyydata.rst
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      191 2018-01-25 08:58:12.000000 stagpy-0.9.2/.landscape.yml
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/stagpy/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    32074 2018-03-22 09:39:49.000000 stagpy-0.9.2/stagpy/stagyydata.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      880 2018-02-12 09:08:48.000000 stagpy-0.9.2/stagpy/__main__.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     8081 2018-04-20 11:39:24.000000 stagpy-0.9.2/stagpy/phyvars.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    11165 2018-04-20 11:43:12.000000 stagpy-0.9.2/stagpy/processing.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     6424 2018-02-26 09:05:26.000000 stagpy-0.9.2/stagpy/misc.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    25325 2018-03-13 10:30:36.000000 stagpy-0.9.2/stagpy/stagyyparsers.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     6013 2018-03-01 09:16:46.000000 stagpy-0.9.2/stagpy/time_series.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5862 2018-02-26 09:05:26.000000 stagpy-0.9.2/stagpy/rprof.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2338 2018-03-15 09:12:36.000000 stagpy-0.9.2/stagpy/__init__.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    37722 2018-02-12 09:08:48.000000 stagpy-0.9.2/stagpy/plates.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     7520 2018-02-26 14:19:01.000000 stagpy-0.9.2/stagpy/field.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    18410 2018-02-22 12:57:39.000000 stagpy-0.9.2/stagpy/parfile.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     3066 2018-03-16 12:32:10.000000 stagpy-0.9.2/stagpy/args.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5700 2018-03-01 09:16:46.000000 stagpy-0.9.2/stagpy/error.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5227 2018-03-15 09:12:36.000000 stagpy-0.9.2/stagpy/commands.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5738 2018-03-15 09:12:36.000000 stagpy-0.9.2/stagpy/config.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      271 2018-04-18 09:02:37.000000 stagpy-0.9.2/tox.ini
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      119 2018-02-12 09:08:48.000000 stagpy-0.9.2/.gitignore
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    18027 2016-11-29 14:55:16.000000 stagpy-0.9.2/LICENSE
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/tests/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1462 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_processing.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      880 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_field.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      713 2018-02-22 12:57:39.000000 stagpy-0.9.2/tests/test_parfile.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1413 2018-02-21 14:17:12.000000 stagpy-0.9.2/tests/test_parsers.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      449 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_rprof.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1033 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_commands.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1713 2018-01-26 09:14:03.000000 stagpy-0.9.2/tests/test_stagyydata.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      147 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_init.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      523 2018-01-30 09:13:35.000000 stagpy-0.9.2/tests/conftest.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      548 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_time_series.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      978 2018-01-25 08:58:12.000000 stagpy-0.9.2/tests/test_misc.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2061 2018-01-30 09:13:35.000000 stagpy-0.9.2/tests/test_args.py
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      463 2018-04-18 09:02:37.000000 stagpy-0.9.2/.travis.yml
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1143 2018-04-20 11:13:40.000000 stagpy-0.9.2/README.rst
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-100000/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1190 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/par
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-100000/Op/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_rprof.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_t00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_vp00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-100000/Op/out_time.dat
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/annulus/
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/annulus/+op/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)  2308018 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/annulus/+op/test_time.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   529304 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/annulus/+op/test_vp00100
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    68496 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/annulus/+op/test_t00100
+-rw-r--r--   0 adrien    (1000) adrien    (1000)  2969199 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/annulus/+op/test_rprof.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      993 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/annulus/par
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-10000/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1189 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/par
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-10000/Op/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-03 07:47:11.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_rprof.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_t00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_vp00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-10000/Op/out_time.dat
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-1000/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1188 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/par
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2018-04-20 11:59:28.000000 stagpy-0.9.2/Examples/ra-1000/Op/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00001
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00000
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   152581 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_rprof.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00005
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00002
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    17808 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_t00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00004
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   134552 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_vp00003
+-rw-r--r--   0 adrien    (1000) adrien    (1000)   444685 2017-04-10 14:26:00.000000 stagpy-0.9.2/Examples/ra-1000/Op/out_time.dat
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     2077 2018-04-20 11:59:28.000000 stagpy-0.9.2/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       38 2018-04-20 11:59:28.000000 stagpy-0.9.2/setup.cfg
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       68 2018-04-18 09:02:37.000000 stagpy-0.9.2/pyproject.toml
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     1316 2018-04-18 09:02:37.000000 stagpy-0.9.2/setup.py
```

### Comparing `stagpy-0.9.1/LICENSE` & `stagpy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/PKG-INFO` & `stagpy-0.9.2/stagpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: stagpy
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tool for StagYY output files processing
 Home-page: https://github.com/StagPython/StagPy
 Author: Martina Ulvrova, Adrien Morison, Stéphane Labrosse
 Author-email: adrien.morison@gmail.com
 License: GPLv2
-Description-Content-Type: UNKNOWN
 Description: .. image:: https://landscape.io/github/StagPython/StagPy/master/landscape.svg?style=flat-square
            :target: https://landscape.io/github/StagPython/StagPy/master
            :alt: Code Health
         
         .. image:: https://travis-ci.org/StagPython/StagPy.svg?branch=master
            :target: https://travis-ci.org/StagPython/StagPy
            :alt: Travis CI
@@ -34,15 +33,15 @@
         access StagYY output data directly in a Python script.
         
         You can install StagPy with ``pip`` from the `Python Package Index`__.
         
         See `the complete documentation`__ for more information on the installation and
         explanations on how to use StagPy.
         
-        .. __: https://pypi.python.org/pypi/stagpy
+        .. __: https://pypi.org/project/stagpy/
         .. __: http://stagpy.readthedocs.org
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `stagpy-0.9.1/docs/conf.py` & `stagpy-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/make.bat` & `stagpy-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/Makefile` & `stagpy-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/maintainers.rst` & `stagpy-0.9.2/docs/sources/maintainers.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/stagyydata.rst` & `stagpy-0.9.2/docs/sources/stagyydata.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/cli.rst` & `stagpy-0.9.2/docs/sources/cli.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/cookbook.rst` & `stagpy-0.9.2/docs/sources/cookbook.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/tuto.rst` & `stagpy-0.9.2/docs/sources/tuto.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/developers.rst` & `stagpy-0.9.2/docs/sources/developers.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/apiref/phyvars.rst` & `stagpy-0.9.2/docs/sources/apiref/phyvars.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/apiref/config.rst` & `stagpy-0.9.2/docs/sources/apiref/config.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/apiref/stagpy.rst` & `stagpy-0.9.2/docs/sources/apiref/stagpy.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/sources/install.rst` & `stagpy-0.9.2/docs/sources/install.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/docs/index.rst` & `stagpy-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_commands.py` & `stagpy-0.9.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_field.py` & `stagpy-0.9.2/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/conftest.py` & `stagpy-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_stagyydata.py` & `stagpy-0.9.2/tests/test_stagyydata.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_processing.py` & `stagpy-0.9.2/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_args.py` & `stagpy-0.9.2/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_misc.py` & `stagpy-0.9.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_parsers.py` & `stagpy-0.9.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_parfile.py` & `stagpy-0.9.2/tests/test_parfile.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/tests/test_time_series.py` & `stagpy-0.9.2/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/field.py` & `stagpy-0.9.2/stagpy/field.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/stagyydata.py` & `stagpy-0.9.2/stagpy/stagyydata.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,21 +428,25 @@
                 :class:`_Steps` instance.
         """
         self.sdat = sdat
         self._last = UNDETERMINED
         super().__init__()
         super().__setitem__(None, _EmptyStep())  # for non existent snaps
 
+    def __repr__(self):
+        return '{}.steps'.format(repr(self.sdat))
+
     def __setitem__(self, key, value):
         pass
 
     def __getitem__(self, key):
-        if isinstance(key, slice):
+        try:
             return _StepsView(self, key)
-        return super().__getitem__(key)
+        except AttributeError:
+            return super().__getitem__(key)
 
     def __missing__(self, istep):
         try:
             istep = int(istep)
         except ValueError:
             raise error.InvalidTimestepError(
                 self.sdat, istep, 'Time step should be an integer value')
@@ -505,18 +509,22 @@
             sdat (:class:`StagyyData`): the StagyyData instance owning the
                 :class:`_Snaps` instance.
         """
         self._isteps = {}
         self._all_isteps_known = False
         super().__init__(sdat)
 
+    def __repr__(self):
+        return '{}.snaps'.format(repr(self.sdat))
+
     def __getitem__(self, key):
-        if isinstance(key, slice):
+        try:
             return _StepsView(self, key)
-        return self.__missing__(key)
+        except AttributeError:
+            return self.__missing__(key)
 
     def __missing__(self, isnap):
         if isnap < 0:
             isnap += len(self)
         istep = self._isteps.get(
             isnap, None if self._all_isteps_known else UNDETERMINED)
         if istep is UNDETERMINED:
@@ -605,15 +613,15 @@
             'rprof': False,
             'fields': [],
             'func': lambda _: True,
         }
         self._dflt_func = self._flt['func']
 
     def __repr__(self):
-        rep = 'snaps' if isinstance(self._col, _Snaps) else 'steps'
+        rep = repr(self._col)
         rep += '[{}:{}:{}]'.format(*self._idx)
         flts = []
         for flt in ('snap', 'rprof', 'fields'):
             if self._flt[flt]:
                 flts.append('{}={}'.format(flt, repr(self._flt[flt])))
         if self._flt['func'] is not self._dflt_func:
             flts.append('func={}'.format(repr(self._flt['func'])))
```

### Comparing `stagpy-0.9.1/stagpy/stagyyparsers.py` & `stagpy-0.9.2/stagpy/stagyyparsers.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/parfile.py` & `stagpy-0.9.2/stagpy/parfile.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/error.py` & `stagpy-0.9.2/stagpy/error.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/time_series.py` & `stagpy-0.9.2/stagpy/time_series.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/plates.py` & `stagpy-0.9.2/stagpy/plates.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/args.py` & `stagpy-0.9.2/stagpy/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from . import commands, field, rprof, time_series, plates
 from .misc import baredoc
 from .config import CONFIG_DIR
 
 
 def _sub(cmd, *sections):
     """Build Subcmd instance."""
-    return Subcmd(baredoc(cmd), *sections, func=cmd)
+    cmd_func = cmd if isfunction(cmd) else cmd.cmd
+    return Subcmd(baredoc(cmd), *sections, func=cmd_func)
 
 
 SUB_CMDS = OrderedDict((
     ('common_', Subcmd('read and process StagYY binary data', 'common',
                        func=lambda: print('stagpy -h for usage'))),
     ('field', _sub(field, 'core', 'plot')),
     ('rprof', _sub(rprof, 'core', 'plot')),
@@ -29,24 +30,26 @@
     ('version', _sub(commands.version_cmd)),
     ('config', _sub(commands.config_cmd)),
 ))
 
 
 def _steps_to_slices():
     """parse timesteps and snapshots arguments and return slices"""
-    if conf.core.timesteps is None and conf.core.snapshots is None:
+    if not (conf.core.timesteps or conf.core.snapshots):
         # default to the last snap
+        conf.core.timesteps = None
         conf.core.snapshots = slice(-1, None, None)
         return
-    elif conf.core.snapshots is not None:
+    elif conf.core.snapshots:
         # snapshots take precedence over timesteps
         # if both are defined
         conf.core.timesteps = None
         steps = conf.core.snapshots
     else:
+        conf.core.snapshots = None
         steps = conf.core.timesteps
     steps = steps.split(':')
     steps[0] = int(steps[0]) if steps[0] else None
     if len(steps) == 1:
         steps.append(steps[0] + 1)
     steps[1] = int(steps[1]) if steps[1] else None
     if len(steps) != 3:
@@ -55,20 +58,14 @@
     steps = slice(*steps)
     if conf.core.snapshots is not None:
         conf.core.snapshots = steps
     else:
         conf.core.timesteps = steps
 
 
-def _update_func(cmd_args):
-    """Extract command func if necessary"""
-    if not isfunction(cmd_args.func):
-        cmd_args.func = cmd_args.func.cmd
-
-
 def parse_args(arglist=None):
     """Parse cmd line arguments.
 
     Update :attr:`stagpy.conf` accordingly.
 
     Args:
         arglist (list of str): the list of cmd line arguments. If set to
@@ -87,16 +84,14 @@
 
     if sub_cmd is None:
         return cmd_args.func
 
     if sub_cmd != 'config':
         commands.report_parsing_problems(PARSING_OUT)
 
-    _update_func(cmd_args)
-
     if conf.common.set:
         set_conf_str(conf, conf.common.set)
 
     if conf.common.config:
         commands.config_pp(all_subs)
 
     try:
```

### Comparing `stagpy-0.9.1/stagpy/rprof.py` & `stagpy-0.9.2/stagpy/rprof.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/__init__.py` & `stagpy-0.9.2/stagpy/__init__.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/__main__.py` & `stagpy-0.9.2/stagpy/__main__.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/config.py` & `stagpy-0.9.2/stagpy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 CONF_DEF['core'] = OrderedDict((
     ('path', Conf('./', True, 'p', {},
                   True, 'path of StagYY run directory or par file', '_files')),
     ('outname', Conf('stagpy', True, 'n', {},
                      True, 'StagPy output file name prefix')),
     ('timesteps', Conf(None, True, 't',
-                       {'nargs': '?', 'const': ':', 'type': str},
+                       {'nargs': '?', 'const': '', 'type': str},
                        False, 'timesteps slice')),
     ('snapshots', Conf(None, True, 's',
-                       {'nargs': '?', 'const': ':', 'type': str},
+                       {'nargs': '?', 'const': '', 'type': str},
                        False, 'snapshots slice')),
 ))
 
 CONF_DEF['plot'] = OrderedDict((
     ('raster', switch_opt(True, None, 'rasterize field plots')),
     ('format', Conf('pdf', True, None, {},
                     True, 'figure format (pdf, eps, svg, png)')),
```

### Comparing `stagpy-0.9.1/stagpy/misc.py` & `stagpy-0.9.2/stagpy/misc.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/commands.py` & `stagpy-0.9.2/stagpy/commands.py`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/stagpy/processing.py` & `stagpy-0.9.2/stagpy/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,38 @@
     dtdt, time = dt_dt(sdat, tstart, tend)
     ftop = tseries['ftop'].values * coefsurf
     fbot = tseries['fbot'].values
     ebal = ftop[:-1] - fbot[:-1] + volume * dtdt
     return ebal, time
 
 
+def mobility(sdat, tstart=None, tend=None):
+    """Plates mobility.
+
+    Compute the ratio vsurf / vrms.
+
+    Args:
+        sdat (:class:`~stagpy.stagyydata.StagyyData`): a StagyyData instance.
+        tstart (float): time at which the computation should start. Use the
+            beginning of the time series data if set to None.
+        tend (float): time at which the computation should end. Use the
+            end of the time series data if set to None.
+    Returns:
+        tuple of :class:`numpy.array`: mobility and time arrays.
+    """
+    tseries = sdat.tseries_between(tstart, tend)
+    steps = sdat.steps[tseries.index[0]:tseries.index[-1]]
+    time = []
+    mob = []
+    for step in steps.filter(rprof=True):
+        time.append(step.timeinfo['t'])
+        mob.append(step.rprof.iloc[-1].loc['vrms'] / step.timeinfo['vrms'])
+    return np.array(mob), np.array(time)
+
+
 def r_edges(step):
     """Cell border.
 
     Args:
         step (:class:`~stagpy.stagyydata._Step`): a step of a StagyyData
             instance.
     Returns:
```

### Comparing `stagpy-0.9.1/stagpy/phyvars.py` & `stagpy-0.9.2/stagpy/phyvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     ('topT_val', Vart('Temperature at top', 'T')),
     ('botT_val', Vart('Temperature at bottom', 'T')),
 ))
 
 TIME_EXTRA = OrderedDict((
     ('dTdt', Vart(processing.dt_dt, r'dT/dt')),
     ('ebalance', Vart(processing.ebalance, r'\mathrm{Nu}')),
+    ('mobility', Vart(processing.mobility, 'M')),
 ))
 
 Varp = namedtuple('Varp', ['description'])
 PLATES = OrderedDict((
     ('c', Varp('Composition')),
     ('eta', Varp('Viscosity')),
     ('sc', Varp('Topography')),
```

### Comparing `stagpy-0.9.1/README.rst` & `stagpy-0.9.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 access StagYY output data directly in a Python script.
 
 You can install StagPy with ``pip`` from the `Python Package Index`__.
 
 See `the complete documentation`__ for more information on the installation and
 explanations on how to use StagPy.
 
-.. __: https://pypi.python.org/pypi/stagpy
+.. __: https://pypi.org/project/stagpy/
 .. __: http://stagpy.readthedocs.org
```

### Comparing `stagpy-0.9.1/setup.py` & `stagpy-0.9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,10 +44,9 @@
         'Programming Language :: Python :: 3.6',
     ],
 
     packages=['stagpy'],
     entry_points={
         'console_scripts': ['stagpy = stagpy.__main__:main']
     },
-    setup_requires=['setuptools_scm'],
     install_requires=DEPENDENCIES,
 )
```

### Comparing `stagpy-0.9.1/Examples/annulus/+op/test_vp00100` & `stagpy-0.9.2/Examples/annulus/+op/test_vp00100`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/annulus/+op/test_time.dat` & `stagpy-0.9.2/Examples/annulus/+op/test_time.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/annulus/+op/test_t00100` & `stagpy-0.9.2/Examples/annulus/+op/test_t00100`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/annulus/+op/test_rprof.dat` & `stagpy-0.9.2/Examples/annulus/+op/test_rprof.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/annulus/par` & `stagpy-0.9.2/Examples/annulus/par`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/par` & `stagpy-0.9.2/Examples/ra-1000/par`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00002` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00002` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00003` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_time.dat` & `stagpy-0.9.2/Examples/ra-1000/Op/out_time.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00000` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00001` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00001` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00003` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00004` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_vp00005` & `stagpy-0.9.2/Examples/ra-1000/Op/out_vp00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00000` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00005` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_t00004` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-1000/Op/out_rprof.dat` & `stagpy-0.9.2/Examples/ra-1000/Op/out_rprof.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/par` & `stagpy-0.9.2/Examples/ra-10000/par`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00002` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00002` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00003` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_time.dat` & `stagpy-0.9.2/Examples/ra-10000/Op/out_time.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00000` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00001` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00001` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00003` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00004` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_vp00005` & `stagpy-0.9.2/Examples/ra-10000/Op/out_vp00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00000` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00005` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_t00004` & `stagpy-0.9.2/Examples/ra-10000/Op/out_t00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-10000/Op/out_rprof.dat` & `stagpy-0.9.2/Examples/ra-10000/Op/out_rprof.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/par` & `stagpy-0.9.2/Examples/ra-100000/par`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00002` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00002` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00002`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00003` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_time.dat` & `stagpy-0.9.2/Examples/ra-100000/Op/out_time.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00000` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00001` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00001` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00001`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00003` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00003`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00004` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_vp00005` & `stagpy-0.9.2/Examples/ra-100000/Op/out_vp00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00000` & `stagpy-0.9.2/Examples/ra-1000/Op/out_t00000`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00005` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00005`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_t00004` & `stagpy-0.9.2/Examples/ra-100000/Op/out_t00004`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Examples/ra-100000/Op/out_rprof.dat` & `stagpy-0.9.2/Examples/ra-100000/Op/out_rprof.dat`

 * *Files identical despite different names*

### Comparing `stagpy-0.9.1/Makefile` & `stagpy-0.9.2/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	ln -sf $(PWD)/$(STAGPY) $(LINK)
 
 $(STAGPY): $(VENV_DIR) $(OBJS)
 	$(VPIP) install -e .
 
 $(VENV_DIR):
 	$(PY) -m venv --system-site-packages $@
+	$(VPIP) install -U pip
 
 info: infopath infozsh infobash
 
 infopath:
 	@echo
 	@echo 'Add $(LINK_DIR) to your path to be able to call StagPy from anywhere'
```

### Comparing `stagpy-0.9.1/stagpy.egg-info/PKG-INFO` & `stagpy-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: stagpy
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tool for StagYY output files processing
 Home-page: https://github.com/StagPython/StagPy
 Author: Martina Ulvrova, Adrien Morison, Stéphane Labrosse
 Author-email: adrien.morison@gmail.com
 License: GPLv2
-Description-Content-Type: UNKNOWN
 Description: .. image:: https://landscape.io/github/StagPython/StagPy/master/landscape.svg?style=flat-square
            :target: https://landscape.io/github/StagPython/StagPy/master
            :alt: Code Health
         
         .. image:: https://travis-ci.org/StagPython/StagPy.svg?branch=master
            :target: https://travis-ci.org/StagPython/StagPy
            :alt: Travis CI
@@ -34,15 +33,15 @@
         access StagYY output data directly in a Python script.
         
         You can install StagPy with ``pip`` from the `Python Package Index`__.
         
         See `the complete documentation`__ for more information on the installation and
         explanations on how to use StagPy.
         
-        .. __: https://pypi.python.org/pypi/stagpy
+        .. __: https://pypi.org/project/stagpy/
         .. __: http://stagpy.readthedocs.org
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `stagpy-0.9.1/stagpy.egg-info/SOURCES.txt` & `stagpy-0.9.2/stagpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .landscape.yml
 .travis.yml
 LICENSE
 Makefile
 README.rst
+pyproject.toml
 setup.py
 tox.ini
 Examples/annulus/par
 Examples/annulus/+op/test_rprof.dat
 Examples/annulus/+op/test_t00100
 Examples/annulus/+op/test_time.dat
 Examples/annulus/+op/test_vp00100
```

