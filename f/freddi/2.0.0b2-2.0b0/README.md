# Comparing `tmp/freddi-2.0.0b2.tar.gz` & `tmp/freddi-2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/dist/freddi-2.0.0b2.tar", last modified: Mon Jan  3 20:59:56 2022, max compression
+gzip compressed data, was "/dist/freddi-2.0b0.tar", last modified: Fri Jun 11 16:10:56 2021, max compression
```

## Comparing `freddi-2.0.0b2.tar` & `freddi-2.0b0.tar`

### file list

```diff
@@ -1,74 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/
--rw-r--r--   0 root         (0) root         (0)     4673 2022-01-03 03:57:02.000000 freddi-2.0.0b2/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    83467 2022-01-03 20:59:56.000000 freddi-2.0.0b2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    82694 2022-01-03 05:48:11.000000 freddi-2.0.0b2/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/include/
--rw-r--r--   0 root         (0) root         (0)     1110 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/application.hpp
--rw-r--r--   0 root         (0) root         (0)    11696 2021-11-14 15:15:36.000000 freddi-2.0.0b2/cpp/include/arguments.hpp
--rw-r--r--   0 root         (0) root         (0)      193 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/constants.hpp
--rw-r--r--   0 root         (0) root         (0)      262 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/exceptions.hpp
--rw-r--r--   0 root         (0) root         (0)     1623 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/freddi_evolution.hpp
--rw-r--r--   0 root         (0) root         (0)    15197 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/freddi_state.hpp
--rw-r--r--   0 root         (0) root         (0)     3991 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/geometry.hpp
--rw-r--r--   0 root         (0) root         (0)     6779 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/gsl_const_cgsm.h
--rw-r--r--   0 root         (0) root         (0)     1138 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/nonlinear_diffusion.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/include/ns/
--rw-r--r--   0 root         (0) root         (0)     5599 2021-11-11 17:42:46.000000 freddi-2.0.0b2/cpp/include/ns/ns_arguments.hpp
--rw-r--r--   0 root         (0) root         (0)     9727 2021-11-11 17:42:46.000000 freddi-2.0.0b2/cpp/include/ns/ns_evolution.hpp
--rw-r--r--   0 root         (0) root         (0)     1424 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/ns/ns_options.hpp
--rw-r--r--   0 root         (0) root         (0)      889 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/ns/ns_output.hpp
--rw-r--r--   0 root         (0) root         (0)      814 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/opacity_related.hpp
--rw-r--r--   0 root         (0) root         (0)     3611 2021-12-28 20:09:00.000000 freddi-2.0.0b2/cpp/include/options.hpp
--rw-r--r--   0 root         (0) root         (0)     1007 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/orbit.hpp
--rw-r--r--   0 root         (0) root         (0)     2753 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/output.hpp
--rw-r--r--   0 root         (0) root         (0)     1625 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/passband.hpp
--rw-r--r--   0 root         (0) root         (0)     1594 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/rochelobe.hpp
--rw-r--r--   0 root         (0) root         (0)      953 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/spectrum.hpp
--rw-r--r--   0 root         (0) root         (0)     4948 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/star.hpp
--rw-r--r--   0 root         (0) root         (0)     2223 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/unit_transformation.hpp
--rw-r--r--   0 root         (0) root         (0)      913 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/include/util.hpp
--rw-r--r--   0 root         (0) root         (0)      293 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/main-ns.cpp
--rw-r--r--   0 root         (0) root         (0)      248 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/pywrap/
--rw-r--r--   0 root         (0) root         (0)     3569 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/converters.cpp
--rw-r--r--   0 root         (0) root         (0)      274 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/converters.hpp
--rw-r--r--   0 root         (0) root         (0)      385 2021-12-31 01:02:51.000000 freddi-2.0.0b2/cpp/pywrap/module.cpp
--rw-r--r--   0 root         (0) root         (0)     7177 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_arguments.cpp
--rw-r--r--   0 root         (0) root         (0)     3438 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_arguments.hpp
--rw-r--r--   0 root         (0) root         (0)    12225 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_evolution.cpp
--rw-r--r--   0 root         (0) root         (0)      134 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_evolution.hpp
--rw-r--r--   0 root         (0) root         (0)     2563 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_state.cpp
--rw-r--r--   0 root         (0) root         (0)      118 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_state.hpp
--rw-r--r--   0 root         (0) root         (0)      358 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/pywrap/util.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/src/
--rw-r--r--   0 root         (0) root         (0)    13724 2021-12-28 20:09:00.000000 freddi-2.0.0b2/cpp/src/arguments.cpp
--rw-r--r--   0 root         (0) root         (0)     2489 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/freddi_evolution.cpp
--rw-r--r--   0 root         (0) root         (0)    28047 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/freddi_state.cpp
--rw-r--r--   0 root         (0) root         (0)     5937 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/geometry.cpp
--rw-r--r--   0 root         (0) root         (0)     3349 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/nonlinear_diffusion.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/src/ns/
--rw-r--r--   0 root         (0) root         (0)     7176 2021-11-14 15:15:36.000000 freddi-2.0.0b2/cpp/src/ns/ns_arguments.cpp
--rw-r--r--   0 root         (0) root         (0)    17930 2021-11-11 17:42:46.000000 freddi-2.0.0b2/cpp/src/ns/ns_evolution.cpp
--rw-r--r--   0 root         (0) root         (0)    12962 2021-12-28 20:09:00.000000 freddi-2.0.0b2/cpp/src/ns/ns_options.cpp
--rw-r--r--   0 root         (0) root         (0)     2369 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/ns/ns_output.cpp
--rw-r--r--   0 root         (0) root         (0)     2283 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/opacity_related.cpp
--rw-r--r--   0 root         (0) root         (0)    21485 2021-12-28 20:09:00.000000 freddi-2.0.0b2/cpp/src/options.cpp
--rw-r--r--   0 root         (0) root         (0)      766 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/orbit.cpp
--rw-r--r--   0 root         (0) root         (0)    13433 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/output.cpp
--rw-r--r--   0 root         (0) root         (0)     1824 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/passband.cpp
--rw-r--r--   0 root         (0) root         (0)     5217 2021-11-14 15:15:36.000000 freddi-2.0.0b2/cpp/src/rochelobe.cpp
--rw-r--r--   0 root         (0) root         (0)     2155 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/spectrum.cpp
--rw-r--r--   0 root         (0) root         (0)     7612 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/star.cpp
--rw-r--r--   0 root         (0) root         (0)     3233 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/src/util.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/cpp/test/
--rw-r--r--   0 root         (0) root         (0)     8991 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/test/geometry.cpp
--rw-r--r--   0 root         (0) root         (0)     2760 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/test/rochelobe.cpp
--rw-r--r--   0 root         (0) root         (0)    21704 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/test/star.cpp
--rw-r--r--   0 root         (0) root         (0)     1699 2021-10-19 12:10:38.000000 freddi-2.0.0b2/cpp/test/util.cpp
--rw-r--r--   0 root         (0) root         (0)      215 2021-10-19 12:10:38.000000 freddi-2.0.0b2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-03 20:59:56.000000 freddi-2.0.0b2/python/freddi/
--rw-r--r--   0 root         (0) root         (0)     4670 2021-10-19 12:10:38.000000 freddi-2.0.0b2/python/freddi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2397 2021-10-19 12:10:38.000000 freddi-2.0.0b2/python/freddi/evolution_result.py
--rw-r--r--   0 root         (0) root         (0)     1074 2022-01-03 20:21:44.000000 freddi-2.0.0b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/
+-rw-r--r--   0 root         (0) root         (0)     4267 2021-06-11 15:51:07.000000 freddi-2.0b0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    30875 2021-06-11 16:10:56.000000 freddi-2.0b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    30106 2021-06-11 15:51:01.000000 freddi-2.0b0/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:55.000000 freddi-2.0b0/cpp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/include/
+-rw-r--r--   0 root         (0) root         (0)      764 2021-05-28 13:40:38.000000 freddi-2.0b0/cpp/include/application.hpp
+-rw-r--r--   0 root         (0) root         (0)    10425 2021-05-28 13:32:19.000000 freddi-2.0b0/cpp/include/arguments.hpp
+-rw-r--r--   0 root         (0) root         (0)     1229 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/constants.hpp
+-rw-r--r--   0 root         (0) root         (0)     1623 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/freddi_evolution.hpp
+-rw-r--r--   0 root         (0) root         (0)    15631 2021-06-11 15:55:50.000000 freddi-2.0b0/cpp/include/freddi_state.hpp
+-rw-r--r--   0 root         (0) root         (0)     3991 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/geometry.hpp
+-rw-r--r--   0 root         (0) root         (0)     6779 2020-03-23 10:23:49.000000 freddi-2.0b0/cpp/include/gsl_const_cgsm.h
+-rw-r--r--   0 root         (0) root         (0)     1138 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/nonlinear_diffusion.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/include/ns/
+-rw-r--r--   0 root         (0) root         (0)     3971 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/include/ns/ns_arguments.hpp
+-rw-r--r--   0 root         (0) root         (0)     9718 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/include/ns/ns_evolution.hpp
+-rw-r--r--   0 root         (0) root         (0)     1132 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/include/ns/ns_options.hpp
+-rw-r--r--   0 root         (0) root         (0)      889 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/ns/ns_output.hpp
+-rw-r--r--   0 root         (0) root         (0)      814 2020-03-23 10:23:49.000000 freddi-2.0b0/cpp/include/opacity_related.hpp
+-rw-r--r--   0 root         (0) root         (0)     3530 2021-06-09 09:51:33.000000 freddi-2.0b0/cpp/include/options.hpp
+-rw-r--r--   0 root         (0) root         (0)     1007 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/orbit.hpp
+-rw-r--r--   0 root         (0) root         (0)     2753 2021-05-28 12:43:03.000000 freddi-2.0b0/cpp/include/output.hpp
+-rw-r--r--   0 root         (0) root         (0)     1625 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/passband.hpp
+-rw-r--r--   0 root         (0) root         (0)     1594 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/rochelobe.hpp
+-rw-r--r--   0 root         (0) root         (0)      953 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/spectrum.hpp
+-rw-r--r--   0 root         (0) root         (0)     4948 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/star.hpp
+-rw-r--r--   0 root         (0) root         (0)     2223 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/include/unit_transformation.hpp
+-rw-r--r--   0 root         (0) root         (0)      913 2020-04-27 12:14:49.000000 freddi-2.0b0/cpp/include/util.hpp
+-rw-r--r--   0 root         (0) root         (0)      293 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/main-ns.cpp
+-rw-r--r--   0 root         (0) root         (0)      248 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/main.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/pywrap/
+-rw-r--r--   0 root         (0) root         (0)     3569 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/converters.cpp
+-rw-r--r--   0 root         (0) root         (0)      274 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/converters.hpp
+-rw-r--r--   0 root         (0) root         (0)      385 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/module.cpp
+-rw-r--r--   0 root         (0) root         (0)     7177 2021-05-28 13:30:38.000000 freddi-2.0b0/cpp/pywrap/pywrap_arguments.cpp
+-rw-r--r--   0 root         (0) root         (0)     3438 2021-01-18 10:49:38.000000 freddi-2.0b0/cpp/pywrap/pywrap_arguments.hpp
+-rw-r--r--   0 root         (0) root         (0)    12213 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/pywrap/pywrap_freddi_evolution.cpp
+-rw-r--r--   0 root         (0) root         (0)      134 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/pywrap_freddi_evolution.hpp
+-rw-r--r--   0 root         (0) root         (0)     2803 2020-08-05 07:41:21.000000 freddi-2.0b0/cpp/pywrap/pywrap_freddi_state.cpp
+-rw-r--r--   0 root         (0) root         (0)      118 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/pywrap_freddi_state.hpp
+-rw-r--r--   0 root         (0) root         (0)      358 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/pywrap/util.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/src/
+-rw-r--r--   0 root         (0) root         (0)    11904 2021-05-29 09:28:47.000000 freddi-2.0b0/cpp/src/arguments.cpp
+-rw-r--r--   0 root         (0) root         (0)     2487 2021-01-18 10:49:38.000000 freddi-2.0b0/cpp/src/freddi_evolution.cpp
+-rw-r--r--   0 root         (0) root         (0)    26963 2021-06-11 15:55:50.000000 freddi-2.0b0/cpp/src/freddi_state.cpp
+-rw-r--r--   0 root         (0) root         (0)     5937 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/geometry.cpp
+-rw-r--r--   0 root         (0) root         (0)     3349 2020-03-23 10:23:49.000000 freddi-2.0b0/cpp/src/nonlinear_diffusion.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/src/ns/
+-rw-r--r--   0 root         (0) root         (0)     3725 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/src/ns/ns_arguments.cpp
+-rw-r--r--   0 root         (0) root         (0)    17977 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/src/ns/ns_evolution.cpp
+-rw-r--r--   0 root         (0) root         (0)    10760 2021-02-05 13:37:33.000000 freddi-2.0b0/cpp/src/ns/ns_options.cpp
+-rw-r--r--   0 root         (0) root         (0)     2369 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/ns/ns_output.cpp
+-rw-r--r--   0 root         (0) root         (0)     2283 2020-03-23 10:23:49.000000 freddi-2.0b0/cpp/src/opacity_related.cpp
+-rw-r--r--   0 root         (0) root         (0)    17780 2021-06-11 15:55:50.000000 freddi-2.0b0/cpp/src/options.cpp
+-rw-r--r--   0 root         (0) root         (0)      766 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/orbit.cpp
+-rw-r--r--   0 root         (0) root         (0)    13853 2021-05-28 12:45:48.000000 freddi-2.0b0/cpp/src/output.cpp
+-rw-r--r--   0 root         (0) root         (0)     1824 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/passband.cpp
+-rw-r--r--   0 root         (0) root         (0)     4668 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/rochelobe.cpp
+-rw-r--r--   0 root         (0) root         (0)     2155 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/src/spectrum.cpp
+-rw-r--r--   0 root         (0) root         (0)     7612 2020-08-05 07:41:21.000000 freddi-2.0b0/cpp/src/star.cpp
+-rw-r--r--   0 root         (0) root         (0)     3233 2020-04-27 12:14:49.000000 freddi-2.0b0/cpp/src/util.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/cpp/test/
+-rw-r--r--   0 root         (0) root         (0)     8991 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/test/geometry.cpp
+-rw-r--r--   0 root         (0) root         (0)     2760 2020-04-10 06:19:23.000000 freddi-2.0b0/cpp/test/rochelobe.cpp
+-rw-r--r--   0 root         (0) root         (0)    21704 2020-06-11 07:22:56.000000 freddi-2.0b0/cpp/test/star.cpp
+-rw-r--r--   0 root         (0) root         (0)     1699 2020-04-24 09:19:13.000000 freddi-2.0b0/cpp/test/util.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:55.000000 freddi-2.0b0/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-11 16:10:56.000000 freddi-2.0b0/python/freddi/
+-rw-r--r--   0 root         (0) root         (0)     4267 2020-04-10 06:19:23.000000 freddi-2.0b0/python/freddi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2020-08-05 07:41:21.000000 freddi-2.0b0/python/freddi/evolution_result.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2021-06-11 16:08:33.000000 freddi-2.0b0/setup.py
```

### Comparing `freddi-2.0.0b2/CMakeLists.txt` & `freddi-2.0b0/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     cpp/src/rochelobe.cpp
     cpp/src/spectrum.cpp
     cpp/src/star.cpp
     cpp/src/util.cpp
 
     cpp/include/arguments.hpp
     cpp/include/constants.hpp
-    cpp/include/exceptions.hpp
     cpp/include/freddi_evolution.hpp
     cpp/include/freddi_state.hpp
     cpp/include/geometry.hpp
     cpp/include/gsl_const_cgsm.h
     cpp/include/nonlinear_diffusion.hpp
     cpp/include/opacity_related.hpp
     cpp/include/orbit.hpp
@@ -141,24 +140,15 @@
 
 function(CREATE_PY_EXT)
     set(TARGET _freddi)
 
     find_package(PythonExtensions REQUIRED)
     find_package(NumPy REQUIRED)
 
-    set(PYTHON_EXE "${PYTHON_PREFIX}/bin/python")
-    set(PYTHON_VERSION_SCRIPT "import sys; vi = sys.version_info; print(f'{vi.major}{vi.minor}')")
-    execute_process(
-            COMMAND
-            ${PYTHON_EXE} -c "${PYTHON_VERSION_SCRIPT}"
-            OUTPUT_STRIP_TRAILING_WHITESPACE
-            OUTPUT_VARIABLE PYTHON_VERSION
-    )
-
-    find_package(Boost REQUIRED COMPONENTS python${PYTHON_VERSION} numpy${PYTHON_VERSION} filesystem)
+    find_package(Boost COMPONENTS python numpy filesystem REQUIRED)
 
     add_library(${TARGET} MODULE ${MIN_SRC} ${NS_MIN_SRC} ${PYWRAP_SRC})
     target_include_directories(${TARGET} PUBLIC ${Boost_INCLUDE_DIRS} ${NumPy_INCLUDE_DIRS})
     target_link_libraries(${TARGET} ${Boost_LIBRARIES})
     python_extension_module(${TARGET})
     install(TARGETS ${TARGET} LIBRARY DESTINATION python/freddi)
```

### Comparing `freddi-2.0.0b2/cpp/include/application.hpp` & `freddi-2.0b0/cpp/include/application.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #ifndef FREDDI_APPLICATION_H
 #define FREDDI_APPLICATION_H
 
 #include <iostream>
 
 #include <boost/program_options.hpp>
 
-#include "exceptions.hpp"
 #include "options.hpp"
 #include "output.hpp"
-#include "unit_transformation.hpp"
 
 namespace po = boost::program_options;
 
 
 template <typename Output, typename Options, typename Evolution>
 bool run_application(int ac, char *av[]) {
 	po::variables_map vm;
@@ -22,26 +20,13 @@
 	Options opts(vm);
 	std::shared_ptr<Evolution> freddi{new Evolution(opts)};
 	Output output(freddi, vm);
 	for (int i_t = 0; i_t <= static_cast<int>(freddi->args().calc->time / freddi->args().calc->tau); i_t++) {
 		if (i_t % freddi->args().general->temp_sparsity_output == 0) {
 			output.dump();
 		}
-		try {
-			freddi->step();
-		} catch (const RadiusCollapseException &e) {
-			std::cerr
-				<< "Freddi terminated prematurely"
-				<< ", "
-				<< "i_t = " << i_t
-				<< ", "
-				<< "t = " << sToDay(freddi->t()) << " (days)"
-				<< ", "
-				<< "reason: " << e.what()
-				<< std::endl;
-			return true;
-		}
+		freddi->step();
 	}
 	return true;
 }
 
 #endif //FREDDI_APPLICATION_H
```

### Comparing `freddi-2.0.0b2/cpp/include/arguments.hpp` & `freddi-2.0b0/cpp/include/arguments.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -60,20 +60,17 @@
 	double Topt;
 	double rin;
 	double rout;
 	double risco;
 protected:
 	static inline double rinFromMxKerr(double Mx, double kerr) { return r_kerrISCO(Mx, kerr); }
 	static inline double routFromMxMoptPeriod(double Mx, double Mopt, double period) {
-		// 0.9 is the approximation for the tidal radius found by Papaloizou & Pringle, 1977. 
-		// It is close to r_max value from Paczyncki, 1977, who used the grain model of accretting matter,
-		// and such disk should be presumably smaller than a gaseous disk with pressure. r_max could be a 
-		// better approximation than r_1 or r_2 for an axial-symmetric gaseous disk. 
-		// Compare also with approximation suggested by Gilfanov & Arefiev, 2005
-		// see http://xray.sai.msu.ru/~galja/images/tidal_radius.pdf
+		// 0.9 is approximation for r_max value from Paczyncki, 1977. He used grain model of accretting matter,
+		// so his disk should be smaller than gas disk with pressure. So, probably, r_max is better approximation
+		// than r_1 or r_2 for axial-symmetric gas disk. Also this factor is in agreement with Gilfanov & Arefiev, 2005
 		return 0.9 * rocheLobeVolumeRadius(Mx, Mopt, period);
 	}
 	static inline double riscoFromMxKerr(double Mx, double kerr) { return r_kerrISCO(Mx, kerr); }
 public:
 	BasicDiskBinaryArguments(
 			double alpha, std::optional<double> alphacold,
 			double Mx, double kerr,
@@ -105,15 +102,14 @@
 		double Mdot0;
 		double Mdisk0;
 	public:
 		InitialFFunction(double F0, double Mdot0, double Mdisk0):
 				F0(F0), Mdot0(Mdot0), Mdisk0(Mdisk0) {}
 		virtual ~InitialFFunction() = 0;
 		virtual vecd operator()(const vecd& h) const = 0;
-		virtual size_t first(const vecd& h) const { return 0; }
 	};
 
 	class InitialFPowerF: public InitialFFunction {
 	protected:
 		double powerorder;
 	public:
 		InitialFPowerF(double F0, double Mdot0, double Mdisk0, double powerorder):
@@ -128,18 +124,18 @@
 		InitialFLinearF(double F0, double Mdot0, double Mdisk0):
 				InitialFPowerF(F0, Mdot0, Mdisk0, 1.0) {}
 	};
 
 	class InitialFPowerSigma: public InitialFFunction {
 	protected:
 		double powerorder;
-		OpacityRelated oprel;
+		std::shared_ptr<const OpacityRelated> oprel;
 	public:
 		InitialFPowerSigma(double F0, double Mdot0, double Mdisk0, double powerorder,
-				const OpacityRelated &oprel):
+				std::shared_ptr<const OpacityRelated> oprel):
 				InitialFFunction(F0, Mdot0, Mdisk0),
 				powerorder(powerorder),
 				oprel(oprel) {}
 		~InitialFPowerSigma() override = default;
 		vecd operator()(const vecd& h) const override;
 	};
 
@@ -148,19 +144,17 @@
 		using InitialFFunction::InitialFFunction;
 		~InitialFSineF() override = default;
 		vecd operator()(const vecd& h) const override;
 	};
 
 	class InitialFQuasistat: public InitialFFunction {
 	protected:
-		const OpacityRelated oprel;
+		std::shared_ptr<const OpacityRelated> oprel;
 	public:
-		static double Coeff(double h_in, double h_out, const OpacityRelated &oprel);
-	public:
-		InitialFQuasistat(double F0, double Mdot0, double Mdisk0, const OpacityRelated& oprel):
+		InitialFQuasistat(double F0, double Mdot0, double Mdisk0, const std::shared_ptr<const OpacityRelated>& oprel):
 				InitialFFunction(F0, Mdot0, Mdisk0),
 				oprel(oprel) {}
 		~InitialFQuasistat() override = default;
 		vecd operator()(const vecd& h) const override;
 	};
 
 	class InitialFGaussF: public InitialFFunction {
@@ -182,64 +176,40 @@
 	constexpr static const double default_Tirr2Tvishot = 0.;
 	constexpr static const char default_initialcond[] = "powerF";
 	constexpr static const char default_wind[] = "no";
 public:
 	constexpr static const double mu = 0.62;
 public:
 	std::string opacity;
-	const OpacityRelated oprel;
+	std::shared_ptr<const OpacityRelated> oprel;
 	double Mdotout;
 	std::string boundcond;
 	double Thot;
 	double Tirr2Tvishot;
 	double F0;
 	double Mdisk0;
 	double Mdot0;
 	std::string initialcond;
 	std::string wind;
 	pard windparams;
 protected:
 	std::shared_ptr<InitialFFunction> initial_F_function;
-protected:
-	static std::shared_ptr<InitialFFunction> initializeInitialFFunction(
-			const OpacityRelated& oprel,
-			const BasicDiskBinaryArguments &bdb_args, const std::string& initialcond,
-			std::optional<double> F0, std::optional<double> Mdisk0, std::optional<double> Mdot0,
-			std::optional<double> powerorder,
-			std::optional<double> gaussmu, std::optional<double> gausssigma);
 public:
 	DiskStructureArguments(
 			const BasicDiskBinaryArguments &bdb_args,
 			const std::string& opacity,
 			double Mdotout,
 			const std::string& boundcond, double Thot, double Tirr2Tvishot,
 			const std::string& initialcond,
 			std::optional<double> F0,
 			std::optional<double> Mdisk0, std::optional<double> Mdot0,
 			std::optional<double> powerorder,
 			std::optional<double> gaussmu, std::optional<double> gausssigma,
 			const std::string& wind, const pard& windparams);
-	DiskStructureArguments(
-			const std::string &opacity,
-			const OpacityRelated &oprel,
-			double Mdotout,
-			const std::string &boundcond,
-			double Thot,
-			double Tirr2Tvishot,
-			const std::string &initialcond,
-			const std::shared_ptr<InitialFFunction> initial_F_function,
-			const std::string &wind, const pard &windparams):
-			opacity(opacity), oprel(oprel),
-			Mdotout(Mdotout),
-			boundcond(boundcond), Thot(Thot), Tirr2Tvishot(Tirr2Tvishot),
-			initialcond(initialcond),
-			initial_F_function(initial_F_function),
-			wind(wind), windparams(windparams) {}
 	inline vecd initial_F(const vecd& h) const { return (*initial_F_function)(h); }
-	inline size_t initial_first(const vecd& h) const { return initial_F_function->first(h); }
 };
 
 
 class SelfIrradiationArguments {
 public:
 	constexpr static const double default_Cirr = 0.0;
 	constexpr static const double default_irrindex = 0.0;
```

### Comparing `freddi-2.0.0b2/cpp/include/freddi_evolution.hpp` & `freddi-2.0b0/cpp/include/freddi_evolution.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/freddi_state.hpp` & `freddi-2.0b0/cpp/include/freddi_state.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -96,92 +96,92 @@
 		testCWind(const testCWind&) = default;
 		virtual testCWind* clone() const override { return new testCWind(*this); }
 	};
 
 	class testCq0Shields1986Wind: public BasicWind {
 	private:
 		// windparams
-		const double C_w;
-		const double R_w;
+		const double kC;
+		const double R_windmin2out;
 	public:
 		explicit testCq0Shields1986Wind(const FreddiState& state);
 		~testCq0Shields1986Wind() override = default;
 		testCq0Shields1986Wind(const testCq0Shields1986Wind&) = default;
 		virtual testCq0Shields1986Wind* clone() const override { return new testCq0Shields1986Wind(*this); }
 		virtual void update(const FreddiState&) override;
 	};
-	
+
+	class Shields1986Wind: public BasicWind {
+	//G. A. Shields, C. F. McKee, D. N. C. Lin, and M. C. Begelman. Compton-heated winds andcoronae above accretion disks. II - Instability and oscillations. ApJ, 306:90–106, July 1986.
+	//doi:10.1086/164322
+	private:
+		// windparams
+		const double f_X;
+		const double X_f;
+		const double T_iC;
+	public:
+		explicit Shields1986Wind(const FreddiState& state);
+		~Shields1986Wind() override = default;
+		Shields1986Wind(const Shields1986Wind&) = default;
+		virtual Shields1986Wind* clone() const override { return new Shields1986Wind(*this); }
+		virtual void update(const FreddiState&) override;
+	};
+
 	class Janiuk2015Wind: public BasicWind {
 	//Janiuk A., Grzedzielski M., Capitanio F., Bianchi S., 2015, Interplay between heartbeat oscillations and wind outflow in microquasar IGR J17091-3624 A&A, 574, A92
 	//doi:10.1051/0004-6361/201425003
 	private:
 		// windparams
 		const double A_0;
 		const double B_1;
 	public:
 		explicit Janiuk2015Wind(const FreddiState& state);
 		~Janiuk2015Wind() override = default;
 		Janiuk2015Wind(const  Janiuk2015Wind&) = default;
 		virtual Janiuk2015Wind* clone() const override { return new Janiuk2015Wind(*this); }
 		virtual void update(const FreddiState&) override;
 	};
-	
-	class Shields1986Wind: public BasicWind {
-	//G. A. Shields, C. F. McKee, D. N. C. Lin, and M. C. Begelman. Compton-heated winds andcoronae above accretion disks. II - Instability and oscillations. ApJ, 306:90–106, July 1986.
-	//doi:10.1086/164322
-	private:
-		// windparams
-		const double Xi_max;
-		const double T_ic;
-		const double Pow;
-	public:
-		explicit Shields1986Wind(const FreddiState& state);
-		~Shields1986Wind() override = default;
-		Shields1986Wind(const Shields1986Wind&) = default;
-		virtual Shields1986Wind* clone() const override { return new Shields1986Wind(*this); }
-		virtual void update(const FreddiState&) override;
-	};
 
-	class Woods1996AGNWind: public BasicWind {
+	class Woods1996Wind: public BasicWind {
 	//D. T. Woods, R. I. Klein, J. I. Castor, C. F. McKee, and J. B. Bell. X-Ray–heated Coronae andWinds from Accretion Disks: Time-dependent Two-dimensional Hydrodynamics with AdaptiveMesh Refinement. ApJ, 461:767, April 1996
 	//doi:10.1086/177101
 	private:
 		// windparams
 		const double C_0;
-		const double T_ic;
+		const double T_iC;
 	public:
-		explicit Woods1996AGNWind(const FreddiState& state);
-		~Woods1996AGNWind() override = default;
-		Woods1996AGNWind(const Woods1996AGNWind&) = default;
-		virtual Woods1996AGNWind* clone() const override { return new Woods1996AGNWind(*this); }
+		explicit Woods1996Wind(const FreddiState& state);
+		~Woods1996Wind() override = default;
+		Woods1996Wind(const Woods1996Wind&) = default;
+		virtual Woods1996Wind* clone() const override { return new Woods1996Wind(*this); }
 		virtual void update(const FreddiState&) override;
 	};
 
 	class Woods1996ShieldsApproxWind : public BasicWind {
 	//D. T. Woods, R. I. Klein, J. I. Castor, C. F. McKee, and J. B. Bell. X-Ray–heated Coronae andWinds from Accretion Disks: Time-dependent Two-dimensional Hydrodynamics with AdaptiveMesh Refinement. ApJ, 461:767, April 1996
 	//doi:10.1086/177101
 	private:
 		// windparams
 		const double Xi_max;
-		const double T_ic;
-		const double Pow;
+		const double T_iC;
+		const double W_pow;
 	public:
 		explicit Woods1996ShieldsApproxWind(const FreddiState& state);
 		~Woods1996ShieldsApproxWind() override = default;
 		Woods1996ShieldsApproxWind(const Woods1996ShieldsApproxWind&) = default;
 		virtual Woods1996ShieldsApproxWind* clone() const override { return new Woods1996ShieldsApproxWind(*this); }
 		virtual void update(const FreddiState&) override;
 	};
 	
 	class PeriodPaperWind : public BasicWind {
 	// Avakyan, 2021
 	// https://ui.adsabs.harvard.edu/abs/2021arXiv210511974A/
 	private:
 		// windparams
-		const double C_w;
+		const double W_pow;
 	public:
 		explicit PeriodPaperWind(const FreddiState& state);
 		~PeriodPaperWind() override = default;
 		PeriodPaperWind(const PeriodPaperWind&) = default;
 		virtual PeriodPaperWind* clone() const override { return new PeriodPaperWind(*this); }
 		virtual void update(const FreddiState&) override;
 	};
@@ -249,22 +249,22 @@
 		size_t last;
 		vecd F;
 		double F_in;
 		explicit CurrentState(const DiskStructure& str);
 		CurrentState(const CurrentState&) = default;
 		CurrentState& operator=(const CurrentState&) = default;
 	private:
-		static size_t initializeFirst(const DiskStructure& str);
 		static vecd initializeF(const DiskStructure& str);
 	};
 
 	struct DiskOptionalStructure {
 		boost::optional<double> Mdisk;
 		boost::optional<double> Lx;
 		boost::optional<double> Mdot_wind;
+		boost::optional<double> mU, mB, mV, mR, mI, mJ;
 		boost::optional<vecd> W, Tph, Qx, Tph_vis, Tph_X, Tirr, Kirr, Sigma, Height;
 	};
 
 protected:
 	std::shared_ptr<const DiskStructure> str_;
 	CurrentState current_;
 	DiskOptionalStructure opt_str_;
@@ -416,14 +416,20 @@
 	}
 	inline double flux(const double lambda) { return flux_region<HotRegion>(lambda); }
 	inline double flux(const Passband& passband) { return flux_region<HotRegion>(passband); }
 	double flux_star(double lambda, double phase);
 	double flux_star(const Passband& passband, double phase);
 	inline double flux_star(double lambda) { return flux_star(lambda, phase_opt()); }
 	inline double flux_star(const Passband& passband) { return flux_star(passband, phase_opt()); }
+	inline double mU() { return lazy_magnitude(opt_str_.mU, lambdaU, irr0U); }
+	inline double mB() { return lazy_magnitude(opt_str_.mB, lambdaB, irr0B); }
+	inline double mV() { return lazy_magnitude(opt_str_.mV, lambdaV, irr0V); }
+	inline double mR() { return lazy_magnitude(opt_str_.mR, lambdaR, irr0R); }
+	inline double mI() { return lazy_magnitude(opt_str_.mI, lambdaI, irr0I); }
+	inline double mJ() { return lazy_magnitude(opt_str_.mJ, lambdaJ, irr0J); }
 	inline double Mdisk() { return lazy_integrate<HotRegion>(opt_str_.Mdisk, Sigma()); }
 	double Mdot_wind();
 	double Sigma_minus(double r) const;
 	double Sigma_plus(double r) const;
 	double R_cooling_front(double r);
 	double v_cooling_front(double r);
 };
```

### Comparing `freddi-2.0.0b2/cpp/include/geometry.hpp` & `freddi-2.0b0/cpp/include/geometry.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/gsl_const_cgsm.h` & `freddi-2.0b0/cpp/include/gsl_const_cgsm.h`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/nonlinear_diffusion.hpp` & `freddi-2.0b0/cpp/include/nonlinear_diffusion.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/ns/ns_arguments.hpp` & `freddi-2.0b0/cpp/include/ns/ns_arguments.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 	constexpr static const double default_freqx_dummy = 0.;
 public:
 	std::string nsprop;
 	double freqx;
 	double Rx;
 	double Bx;
 	double hotspotarea;
-	double mu_magn;
 	double epsilonAlfven;
 	double inversebeta;
 	double Rdead;
 	std::string fptype;
 	pard fpparams;
 	std::string kappat_type;
 	pard kappat_params;
@@ -45,29 +44,28 @@
 protected:
 	static double initializeFreqx(const std::string& nsprop);
 	static double initializeRx(const std::string& nsprop, std::optional<double> freqx);
 public:
 	NeutronStarArguments(
 			const std::string& nsprop,
 			std::optional<double> freqx,
-			std::optional<double> Rx_,
+			std::optional<double> Rx,
 			double Bx, double hotspotarea,
 			double epsilonAlfven, double inversebeta, double Rdead,
 			const std::string& fptype, const pard& fpparams,
 			const std::string& kappat_type, const pard& kappat_params,
 			const std::string& ns_grav_redshift):
 			nsprop(nsprop),
 			freqx(freqx ? *freqx : initializeFreqx(nsprop)),
-			Rx(Rx_ ? *Rx_ : initializeRx(nsprop, freqx)),
-			Bx(Bx), hotspotarea(hotspotarea), mu_magn(0.5 * Bx * m::pow<3>(Rx)),
+			Rx(Rx ? *Rx : initializeRx(nsprop, freqx)),
+			Bx(Bx), hotspotarea(hotspotarea),
 			epsilonAlfven(epsilonAlfven), inversebeta(inversebeta), Rdead(Rdead),
 			fptype(fptype), fpparams(fpparams),
 			kappat_type(kappat_type), kappat_params(kappat_params),
 			ns_grav_redshift(ns_grav_redshift) {}
-	double R_Alfven(double GM, double Mdot) const;
 };
 
 
 class NeutronStarBasicDiskBinaryArguments: public BasicDiskBinaryArguments {
 protected:
 	static std::optional<double> initializeRisco(const NeutronStarArguments& ns_args, std::optional<double> risco);
 public:
@@ -78,55 +76,14 @@
 			double period_,
 			double Mopt_, double roche_lobe_fill_, double Topt_,
 			std::optional<double> rin_, std::optional<double> rout_, std::optional<double> risco_
 	);
 };
 
 
-class NeutronStarDiskStructureArguments: public DiskStructureArguments {
-protected:
-	class InitialFQuasistatNS: public DiskStructureArguments::InitialFFunction {
-	protected:
-		const OpacityRelated oprel;
-		const double h_in;
-	public:
-		InitialFQuasistatNS(double F0, double Mdot0, double Mdisk0, const OpacityRelated& oprel, double h_in):
-				InitialFFunction(F0, Mdot0, Mdisk0),
-				oprel(oprel),
-				h_in(h_in) {}
-		~InitialFQuasistatNS() override = default;
-		vecd operator()(const vecd& h) const override;
-		size_t first(const vecd& h) const override;
-	};
-protected:
-	static std::shared_ptr<InitialFFunction> initializeInitialFFunctionNS(
-			const OpacityRelated& oprel,
-			const NeutronStarArguments& ns_args,
-			const BasicDiskBinaryArguments &bdb_args,
-			const std::string& initialcond,
-			std::optional<double> F0, std::optional<double> Mdisk0, std::optional<double> Mdot0,
-			std::optional<double> powerorder,
-			std::optional<double> gaussmu, std::optional<double> gausssigma);
-
-public:
-	NeutronStarDiskStructureArguments(
-			const NeutronStarArguments& ns_args,
-			const BasicDiskBinaryArguments &bdb_args,
-			const std::string& opacity,
-			double Mdotout,
-			const std::string& boundcond, double Thot, double Tirr2Tvishot,
-			const std::string& initialcond,
-			std::optional<double> F0,
-			std::optional<double> Mdisk0, std::optional<double> Mdot0,
-			std::optional<double> powerorder,
-			std::optional<double> gaussmu, std::optional<double> gausssigma,
-			const std::string& wind, const pard& windparams);
-};
-
-
 class NeutronStarSelfIrradiationArguments: public SelfIrradiationArguments {
 public:
 	constexpr static const char default_angular_dist_ns[] = "isotropic";
 public:
 	std::string angular_dist_ns;
 public:
 	NeutronStarSelfIrradiationArguments(
```

### Comparing `freddi-2.0.0b2/cpp/include/ns/ns_evolution.hpp` & `freddi-2.0b0/cpp/include/ns/ns_evolution.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -52,22 +52,21 @@
 //		double F_dead;
 		double inverse_beta;
 		double epsilon_Alfven;
 		double hot_spot_area;
 		vecd Fmagn;
 		vecd dFmagn_dh;
 		vecd d2Fmagn_dh2;
+		NeutronStarStructure(const NeutronStarArguments& args_ns, FreddiEvolution* evolution);
 	protected:
 		static double initialize_redshift(const FreddiEvolution* evolution, const NeutronStarArguments& args_ns);
 		static std::shared_ptr<BasicKappaT> initialize_kappa_t(const NeutronStarArguments& args_ns);
 		vecd initialize_Fmagn(FreddiEvolution* evolution) const;
 		vecd initialize_dFmagn_dh(FreddiEvolution* evolution) const;
 		vecd initialize_d2Fmagn_dh2(FreddiEvolution* evolution) const;
-	public:
-		NeutronStarStructure(const NeutronStarArguments& args_ns, FreddiEvolution* evolution);
 	};
 
 	struct NeutronStarOptionalStructure {
 		boost::optional<double> Lx_ns_rest_frame;
 	};
 
 	class BasicNSMdotFraction {
@@ -209,19 +208,19 @@
 // fp_
 public:
 	inline double fp(double radius) const { return (*fp_)(*this, radius); }
 	inline double fp() const { return fp(R()[first()]); }
 // eta_ns_
 public:
 	inline double eta_ns(double Rm) const { return (*eta_ns_)(*this, Rm); }
-	inline double eta_ns() const { return eta_ns(R_Alfven()); }
+	inline double eta_ns() const { return eta_ns(R_alfven()); }
 public:
 	using FreddiEvolution::step;
 	virtual double Mdot_in() const override;
-	double R_Alfven() const;
+	double R_alfven() const;
 protected:
 	virtual void invalidate_optional_structure() override;
 	virtual void truncateInnerRadius() override;
 	virtual vecd windC() const override;
 	virtual IrradiatedStar::sources_t star_irr_sources() override;
 public:
 	FreddiNeutronStarEvolution(const FreddiNeutronStarArguments& args);
```

### Comparing `freddi-2.0.0b2/cpp/include/ns/ns_options.hpp` & `freddi-2.0b0/cpp/include/ns/ns_options.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,14 @@
 
 class NeutronStarBasicDiskBinaryOptions: public NeutronStarBasicDiskBinaryArguments {
 public:
 	NeutronStarBasicDiskBinaryOptions(const po::variables_map& vm, const NeutronStarArguments& ns_args);
 	static po::options_description description();
 };
 
-class NeutronStarDiskStructureOptions: public NeutronStarDiskStructureArguments {
-public:
-	NeutronStarDiskStructureOptions(const po::variables_map& vm, const NeutronStarArguments& ns_args,
-									const BasicDiskBinaryArguments& bdb_args);
-	static po::options_description description();
-};
-
 class NeutronStarSelfIrradiationOptions: public NeutronStarSelfIrradiationArguments {
 public:
 	NeutronStarSelfIrradiationOptions(const po::variables_map& vm, const DiskStructureArguments& dsa_args);
 	static po::options_description description();
 };
 
 class FreddiNeutronStarOptions: public FreddiNeutronStarArguments {
```

### Comparing `freddi-2.0.0b2/cpp/include/ns/ns_output.hpp` & `freddi-2.0b0/cpp/include/ns/ns_output.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/opacity_related.hpp` & `freddi-2.0b0/cpp/include/opacity_related.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/options.hpp` & `freddi-2.0b0/cpp/include/options.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 	static std::optional<double> routInitializer(const po::variables_map& vm);
 	static std::optional<double> riscoInitializer(const po::variables_map& vm);
 };
 
 
 class DiskStructureOptions: public DiskStructureArguments {
 public:
-	constexpr static const char caption[] = "Parameters of the disk model";
-public:
 	DiskStructureOptions(const po::variables_map& vm, const BasicDiskBinaryArguments& bdb_args);
 	static po::options_description description();
 	static pard windparamsInitializer(const po::variables_map& vm);
 };
 
 
 class SelfIrradiationOptions: public SelfIrradiationArguments {
```

### Comparing `freddi-2.0.0b2/cpp/include/orbit.hpp` & `freddi-2.0b0/cpp/include/orbit.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/output.hpp` & `freddi-2.0b0/cpp/include/output.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/passband.hpp` & `freddi-2.0b0/cpp/include/passband.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/rochelobe.hpp` & `freddi-2.0b0/cpp/include/rochelobe.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/spectrum.hpp` & `freddi-2.0b0/cpp/include/spectrum.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/star.hpp` & `freddi-2.0b0/cpp/include/star.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/unit_transformation.hpp` & `freddi-2.0b0/cpp/include/unit_transformation.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/include/util.hpp` & `freddi-2.0b0/cpp/include/util.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/pywrap/converters.cpp` & `freddi-2.0b0/cpp/pywrap/converters.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/pywrap/pywrap_arguments.cpp` & `freddi-2.0b0/cpp/pywrap/pywrap_arguments.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/pywrap/pywrap_arguments.hpp` & `freddi-2.0b0/cpp/pywrap/pywrap_arguments.hpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_evolution.cpp` & `freddi-2.0b0/cpp/pywrap/pywrap_freddi_evolution.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	kw["Qirr2Qvishot"] = m::pow<4>(DiskStructureArguments::default_Tirr2Tvishot);
 	kw["F0"] = object();
 	kw["Mdisk0"] = object();
 	kw["Mdot0"] = object();
 	kw["powerorder"] = object();
 	kw["gaussmu"] = object();
 	kw["gausssigma"] = object();
-	kw["windtype"] = DiskStructureArguments::default_wind;
+	kw["wind"] = DiskStructureArguments::default_wind;
 	kw["windparams"] = tuple();
 
 	kw["Cirr"] = SelfIrradiationArguments::default_Cirr;
 	kw["irrindex"] = SelfIrradiationArguments::default_irrindex;
 	kw["Cirrcold"] = SelfIrradiationArguments::default_Cirr_cold;
 	kw["irrindexcold"] = SelfIrradiationArguments::default_irrindex_cold;
 	kw["h2rcold"] = SelfIrradiationArguments::default_height_to_radius_cold;
@@ -145,15 +145,15 @@
 			extract<std::string>(kw["opacity"]),
 			extract<double>(kw["Mdotout"]),
 			extract<std::string>(kw["boundcond"]), extract<double>(kw["Thot"]),
 			std::pow(extract<double>(kw["Qirr2Qvishot"]), 0.25),
 			extract<std::string>(kw["initialcond"]),
 			kw["F0"], kw["Mdisk0"], kw["Mdot0"],
 			kw["powerorder"], kw["gaussmu"], kw["gausssigma"],
-			extract<std::string>(kw["windtype"]), kw["windparams"]);
+			extract<std::string>(kw["wind"]), kw["windparams"]);
 	const auto irr = make_self_irradiation_arguments(
 			extract<double>(kw["Cirr"]),
 			extract<double>(kw["irrindex"]),
 			extract<double>(kw["Cirrcold"]),
 			extract<double>(kw["irrindexcold"]),
 			extract<double>(kw["h2rcold"]),
 			extract<std::string>(kw["angulardistdisk"]));
@@ -247,15 +247,15 @@
 			extract<std::string>(kw["opacity"]),
 			extract<double>(kw["Mdotout"]),
 			extract<std::string>(kw["boundcond"]), extract<double>(kw["Thot"]),
 			std::pow(extract<double>(kw["Qirr2Qvishot"]), 0.25),
 			extract<std::string>(kw["initialcond"]),
 			kw["F0"], kw["Mdisk0"], kw["Mdot0"],
 			kw["powerorder"], kw["gaussmu"], kw["gausssigma"],
-			extract<std::string>(kw["windtype"]), kw["windparams"]);
+			extract<std::string>(kw["wind"]), kw["windparams"]);
 	const auto irr = make_neutron_star_self_irradiation_arguments(
 			extract<double>(kw["Cirr"]),
 			extract<double>(kw["irrindex"]),
 			extract<double>(kw["Cirrcold"]),
 			extract<double>(kw["irrindexcold"]),
 			extract<double>(kw["h2rcold"]),
 			extract<std::string>(kw["angulardistdisk"]),
```

### Comparing `freddi-2.0.0b2/cpp/pywrap/pywrap_freddi_state.cpp` & `freddi-2.0b0/cpp/pywrap/pywrap_freddi_state.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 		.add_property("Lx", &FreddiState::Lx)
 		.add_property("t", &FreddiState::t)
 		.add_property("i_t", &FreddiState::i_t)
 		.add_property("Nt", &FreddiState::Nt)
 		.add_property("Nx", &FreddiState::Nx)
 		.add_property("first", &FreddiState::first)
 		.add_property("last", &FreddiState::last)
+		.add_property("mU", &FreddiState::mU)
+		.add_property("mB", &FreddiState::mB)
+		.add_property("mV", &FreddiState::mV)
+		.add_property("mR", &FreddiState::mR)
+		.add_property("mI", &FreddiState::mI)
+		.add_property("mJ", &FreddiState::mJ)
 		.add_property("Mdisk", &FreddiState::Mdisk)
 		.add_property("Mdot_wind", &FreddiState::Mdot_wind)
 		.add_property("h", make_function(&FreddiState::h, return_value_policy<copy_const_reference>()))
 		.add_property("R", make_function(&FreddiState::R, return_value_policy<copy_const_reference>()))
 		.add_property("F", make_function(&FreddiState::F, return_value_policy<copy_const_reference>()))
 		.add_property("W", make_function(&FreddiState::W, return_value_policy<copy_const_reference>()))
 		.add_property("Tph", make_function(&FreddiState::Tph, return_value_policy<copy_const_reference>()))
```

### Comparing `freddi-2.0.0b2/cpp/src/freddi_evolution.cpp` & `freddi-2.0b0/cpp/src/freddi_evolution.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #include "freddi_evolution.hpp"
 
 #include <cmath>
 #include <string>
 
 #include "arguments.hpp"
-#include "exceptions.hpp"
 #include "nonlinear_diffusion.hpp"
 
 using namespace std::placeholders;
 
 
 FreddiEvolution::FreddiEvolution(const FreddiArguments &args):
 		FreddiState(args, std::bind(&FreddiEvolution::wunction, this, _1, _2, _3, _4)) {}
@@ -44,28 +43,28 @@
 
 	auto ii = last() + 1;
 	if (Tirr().at(last()) / Tph_vis().at(last()) < args().disk->Tirr2Tvishot) {
 	// when irradiation is not important
 	// hot disc extends as far as Sigma>Sigma_max_cold(alpha_cold) and not farther than R_cooling_front and Tirr <= Thot 
 		do {
 			ii--;
-			if (ii <= first()) throw RadiusCollapseException();
+			if (ii <= first()) throw std::runtime_error("Rout <= Rin");
 		  } while( ( R().at(ii) > R_cooling_front ( R().at(ii)) ) && ( Sigma().at(ii) < Sigma_minus(R().at(ii)) ) && ( Tirr().at(ii) < args().disk->Thot ) );
 		//} while( ( R().at(ii) > R_cooling_front ( R().at(ii)) ) && ( Sigma().at(ii) < Sigma_minus(R().at(ii)) ) );
 	} else if (args().disk->boundcond == "Teff") {
 	// irradiation is important, the boundary is at fixed Teff
 		do {
 			ii--;
-			if (ii <= first()) throw RadiusCollapseException();
+			if (ii <= first()) throw std::runtime_error("Rout <= Rin");
 		} while( Tph().at(ii) < args().disk->Thot );
 	} else if (args().disk->boundcond == "Tirr") {
 	// irradiation is important, the boundary is at fixed Tir
 		do {
 			ii--;
-			if (ii <= first()) throw RadiusCollapseException();
+			if (ii <= first()) throw std::runtime_error("Rout <= Rin");
 		} while( Tirr().at(ii) < args().disk->Thot );
 	} else{
 		throw std::invalid_argument("Wrong boundcond");
 	}
 
 	if ( ii <= last() - 1 ){
 		current_.last = ii;
```

### Comparing `freddi-2.0.0b2/cpp/src/freddi_state.cpp` & `freddi-2.0b0/cpp/src/freddi_state.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 		R_g(GSL_CONST_CGSM_GRAVITATIONAL_CONSTANT * args.basic->Mx / m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT)),
 		eta(efficiency_of_accretion(args.basic->kerr)),
 		semiaxis(args.basic->semiaxis(args.basic->Mx, args.basic->Mopt, args.basic->period)),
 		inclination(args.flux->inclination / 180.0 * M_PI),
 		cosi(std::cos(args.flux->inclination / 180.0 * M_PI)),
 		distance(args.flux->distance),
 		cosiOverD2(cosi / m::pow<2>(distance)),
-		oprel(args.disk->oprel),
+		oprel(*(args.disk->oprel.get())),
 		h(initialize_h(args, Nx)),
 		R(initialize_R(h, GM)),
 		wunc(wunc) {}
 
 vecd FreddiState::DiskStructure::initialize_h(const FreddiArguments& args, size_t Nx) {
 	const double h_in = args.basic->h(args.basic->rin);
 	const double h_out = args.basic->h(args.basic->rout);
@@ -53,23 +53,19 @@
 }
 
 
 FreddiState::CurrentState::CurrentState(const DiskStructure& str):
 		Mdot_out(str.args.disk->Mdotout),
 		t(str.args.calc->init_time),
 		i_t(0),
-		first(initializeFirst(str)),
+		first(0),
 		last(str.Nx - 1),
 		F(initializeF(str)),
 		F_in(0) {}
 
-size_t FreddiState::CurrentState::initializeFirst(const DiskStructure& str) {
-	return str.args.disk->initial_first(str.h);
-}
-
 vecd FreddiState::CurrentState::initializeF(const DiskStructure& str) {
 	return str.args.disk->initial_F(str.h);
 }
 
 
 FreddiState::FreddiState(const FreddiArguments& args, const wunc_t& wunc):
 		str_(new DiskStructure(args, wunc)),
@@ -100,22 +96,22 @@
 		wind_.reset(static_cast<BasicWind*>(new Cambier2013Wind(*this)));
 	} else if (args().disk->wind == "__testA__") {
 		wind_.reset(static_cast<BasicWind*>(new testAWind(*this)));
 	} else if (args().disk->wind == "__testB__") {
 		wind_.reset(static_cast<BasicWind*>(new testBWind(*this)));
 	} else if (args().disk->wind == "__testC__") {
 		wind_.reset(static_cast<BasicWind*>(new testCWind(*this)));
-	} else if (args().disk->wind == "ShieldsOscil1986") {
+	} else if (args().disk->wind == "__testC_q0_Shields1986__") {
 		wind_.reset(static_cast<BasicWind*>(new testCq0Shields1986Wind(*this)));
-    } else if (args().disk->wind == "Janiuk2015") {
-        wind_.reset(static_cast<BasicWind*>(new Janiuk2015Wind(*this)));
     } else if (args().disk->wind == "Shields1986") {
         wind_.reset(static_cast<BasicWind*>(new Shields1986Wind(*this)));
+    } else if (args().disk->wind == "Janiuk2015") {
+        wind_.reset(static_cast<BasicWind*>(new Janiuk2015Wind(*this)));
     } else if (args().disk->wind == "Woods1996AGN") {
-        wind_.reset(static_cast<BasicWind*>(new Woods1996AGNWind(*this)));
+        wind_.reset(static_cast<BasicWind*>(new Woods1996Wind(*this)));
     } else if (args().disk->wind == "Woods1996") {
         wind_.reset(static_cast<BasicWind*>(new Woods1996ShieldsApproxWind(*this)));
     } else if (args().disk->wind == "toy") {
         wind_.reset(static_cast<BasicWind*>(new PeriodPaperWind(*this)));
 	} else {
 		throw std::invalid_argument("Wrong wind");
 	}
@@ -442,112 +438,107 @@
 			C_[i] = C0 * 0.5 * (std::cos(2. * M_PI * (state.h()[i] - h_wind_min) / (state.h().back() - h_wind_min)) - 1);
 		}
 	}
 }
 
 FreddiState::testCq0Shields1986Wind::testCq0Shields1986Wind(const FreddiState& state):
 		BasicWind(state),
-		C_w(state.args().disk->windparams.at("C_w")),
-		R_w(state.args().disk->windparams.at("R_w")) {}
+		kC(state.args().disk->windparams.at("kC")),
+		R_windmin2out(state.args().disk->windparams.at("Rwind")) {}
 
 void FreddiState::testCq0Shields1986Wind::update(const FreddiState& state) {
 	BasicWind::update(state);
-	const double h_wind_min = std::sqrt(R_w) * state.h().back();
+	const double h_wind_min = std::sqrt(R_windmin2out) * state.h().back();
 	for (size_t i = state.first(); i <= state.last(); ++i) {
 		if (state.h()[i] > h_wind_min) {
-			C_[i] = -0.5/M_PI * C_w * state.Mdot_in() /
-					(std::log(1 / R_w) * m::pow<2>(state.R()[i])) *
+			C_[i] = -0.5/M_PI * kC * state.Mdot_in() /
+					(std::log(1 / R_windmin2out) * m::pow<2>(state.R()[i])) *
 					(4 * M_PI * m::pow<3>(state.h()[i])) / m::pow<2>(state.GM());
 		}
 	}
 }
 
-FreddiState::Janiuk2015Wind::Janiuk2015Wind(const FreddiState& state):
+FreddiState::Shields1986Wind::Shields1986Wind(const FreddiState& state):
         BasicWind(state),
-        A_0(state.args().disk->windparams.at("A_0")),
-        B_1(state.args().disk->windparams.at("B_1")) {
+	f_X(state.args().disk->windparams.at("f_X")),
+	X_f(state.args().disk->windparams.at("X_f")),
+        T_iC(state.args().disk->windparams.at("T_iC")) {
     update(state);
 }
 
-void FreddiState::Janiuk2015Wind::update(const FreddiState& state) {
+void FreddiState::Shields1986Wind::update(const FreddiState& state) {
     BasicWind::update(state);
     const auto disk = state.args().disk;
+    //  1983ApJ...271...70B page 4
     const double L = state.Mdot_in() * m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT) * state.eta();
-    const double R_g = 2*state.GM()/(m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT));
+    //  1983ApJ...271...70B page 3
+    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_iC);
+    const double P_0 = (f_X/X_f)*L/(4 * M_PI * GSL_CONST_CGSM_SPEED_OF_LIGHT * m::pow<2>(R_iC));
+    const double C_ch = std::sqrt((GSL_CONST_CGSM_BOLTZMANN * T_iC)/(disk->mu * GSL_CONST_CGSM_MASS_PROTON));
+    const double m_ch0 = P_0/C_ch;
     const double L_edd = (4.0 * M_PI * state.GM()* 2.0 * disk->mu * GSL_CONST_CGSM_MASS_PROTON * GSL_CONST_CGSM_SPEED_OF_LIGHT / GSL_CONST_CGSM_THOMSON_CROSS_SECTION);
-    const double lol = L/L_edd;
-	//std::cerr << R_g << "\t" << L/L_edd << "\t" << state.R()[state.last()]/R_g << std::endl;
+    const double L_crit = 0.03 * std::sqrt(1e8/T_iC) * L_edd;
+    const double el = L/L_crit;
+
+	//std::cerr << "\t" << L << "\t" << R_iC  << "\t" << L_edd << "\t" << C_ch << "\t" << P_0 << "\t" << m_ch0 << std::endl;
 
     for (size_t i = state.first(); i <= state.last(); ++i) {
-        //  https://arxiv.org/pdf/1411.4434.pdf
-        if (state.R()[i] > 70.0*R_g) {
-       //C_[i] =  B_1 * 3000.0 * v_r * R_g * fout * ( std::pow((state.R()[state.last()]/R_g), 0.2) - std::pow((state.R()[i]/R_g), 0.2) );
-       //*( std::pow((state.R()[state.last()]/R_g), 0.2) - std::pow((state.R()[i]/R_g), 0.2)
-            const double fout = 1 - 1/(1+A_0*m::pow<2>(lol));
-            const double C_0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
-            const double Q = 2 * (3/(8 * M_PI)) * ((m::pow<4>(state.GM()))/(m::pow<7>(state.h()[i])))  ;
-            B_[i] =  - 0.75 * C_0 * (1/B_1) * ((4 * Q * state.R()[i])/(3* state.GM()))*fout ; }
+        //  1986ApJ...306...90S page 2
+        if (state.R()[i] > 0.1*R_iC) {
+            const double xi = state.R()[i] / R_iC;
+            const double C0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
+            //  1986ApJ...306...90S appendix B page 16
+            const double y = std::sqrt(1 + 1/(4*m::pow<2>(xi)) + ((m::pow<2>(xi))/(1 + m::pow<2>(xi)))*((1.2*xi/(xi + el) + 2.2/(1 + m::pow<2>(el)*xi))*(1.2*xi/(xi + el) + 2.2/(1 + m::pow<2>(el)*xi))));
+            const double Mach_cc = std::cbrt(((1 + (el + 1)/xi)/(1 + 1/((1 + m::pow<2>(xi))*m::pow<4>(el)))));
+	    const double p_po = 0.5 * std::exp(-(((1 - 1/y)*(1 - 1/y))/(2*xi)));
+	    C_[i] = -2.0 * C0 * m_ch0 * Mach_cc * p_po * m::pow<2>(y) * std::pow(xi, -5/3);		}
     }
 }
 
-
-FreddiState::Shields1986Wind::Shields1986Wind(const FreddiState& state):
+FreddiState::Janiuk2015Wind::Janiuk2015Wind(const FreddiState& state):
         BasicWind(state),
-        Xi_max(state.args().disk->windparams.at("Xi_max")),
-        T_ic(state.args().disk->windparams.at("T_ic")),
-        Pow(state.args().disk->windparams.at("Pow")) {
+        A_0(state.args().disk->windparams.at("A_0")),
+        B_1(state.args().disk->windparams.at("B_1")) {
     update(state);
 }
 
-void FreddiState::Shields1986Wind::update(const FreddiState& state) {
+void FreddiState::Janiuk2015Wind::update(const FreddiState& state) {
     BasicWind::update(state);
     const auto disk = state.args().disk;
-    //  1983ApJ...271...70B page 4
     const double L = state.Mdot_in() * m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT) * state.eta();
-    //  1983ApJ...271...70B page 3
-    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_ic);
+    const double R_g = 2*state.GM()/(m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT));
     const double L_edd = (4.0 * M_PI * state.GM()* 2.0 * disk->mu * GSL_CONST_CGSM_MASS_PROTON * GSL_CONST_CGSM_SPEED_OF_LIGHT / GSL_CONST_CGSM_THOMSON_CROSS_SECTION);
-    const double L_crit = (1.0 / 8.0) * std::sqrt(GSL_CONST_CGSM_MASS_ELECTRON / (disk->mu * GSL_CONST_CGSM_MASS_PROTON)) * std::sqrt((GSL_CONST_CGSM_MASS_ELECTRON * GSL_CONST_CGSM_SPEED_OF_LIGHT * GSL_CONST_CGSM_SPEED_OF_LIGHT ) / (GSL_CONST_CGSM_BOLTZMANN * T_ic)) * L_edd;
-    const double P_iC = L / (4.0 * M_PI * m::pow<2>(R_iC) * Xi_max * GSL_CONST_CGSM_SPEED_OF_LIGHT);
-    const double el = L/L_crit;
-    
-    	std::cerr << R_iC << "\t" << disk->mu << "\t" << P_iC << "\t" << state.eta() << "\t" << state.Mdot_in() << "\t" <<  L << "\t" << L_edd << "\t" << L_crit << "\t" <<  GSL_CONST_CGSM_MASS_ELECTRON << std::endl; 
-	//std::cerr << "\t" << L << "\t" << R_iC  << "\t" << L_edd << "\t" << C_ch << "\t" << P_0 << "\t" << m_ch0 << std::endl;
+    const double lol = L/L_edd;
+	//std::cerr << R_g << "\t" << L/L_edd << "\t" << state.R()[state.last()]/R_g << std::endl;
 
     for (size_t i = state.first(); i <= state.last(); ++i) {
-        //  1986ApJ...306...90S page 2
-        if (state.R()[i] > 0.1*R_iC) {
-            const double xi = state.R()[i] / R_iC;
-            const double T_ch = T_ic * std::pow(el, 2.0 / 3.0) * std::pow(xi, -2.0 / 3.0);
-            const double P_0 = L / (4.0 * M_PI * m::pow<2>(state.R()[i]) * Xi_max * GSL_CONST_CGSM_SPEED_OF_LIGHT);
-            const double C_ch = std::sqrt((GSL_CONST_CGSM_BOLTZMANN * T_ch) / (disk->mu * GSL_CONST_CGSM_MASS_PROTON));
-            const double m_ch0 = P_0/C_ch;
-            const double C0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
-            //  1986ApJ...306...90S appendix B page 16
-            const double y = std::sqrt(1. + 1./(4.*m::pow<2>(xi)) + ((m::pow<2>(xi))/(1. + m::pow<2>(xi)))*((1.2*xi/(xi + el) + 2.2/(1. + m::pow<2>(el)*xi))*(1.2*xi/(xi + el) + 2.2/(1. + m::pow<2>(el)*xi))));
-            const double Mach_cc = std::cbrt(((1. + (el + 1.)/xi)/(1. + 1./((1. + m::pow<2>(xi))*m::pow<4>(el)))));
-	    const double p_po = 0.5 * std::exp(-(((1. - 1./y)*(1. - 1./y))/(2.*xi)));
-	    C_[i] = - 2.0 * Pow * C0 * m_ch0 * Mach_cc * p_po * m::pow<2>(y);		}
+        //  https://arxiv.org/pdf/1411.4434.pdf
+        if (state.R()[i] > 70.0*R_g) {
+			const double fout = 1 - 1/(1+A_0*m::pow<2>(lol));
+            const double C_0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
+			//C_[i] =  B_1 * 3000.0 * v_r * R_g * fout * ( std::pow((state.R()[state.last()]/R_g), 0.2) - std::pow((state.R()[i]/R_g), 0.2) );
+            //*( std::pow((state.R()[state.last()]/R_g), 0.2) - std::pow((state.R()[i]/R_g), 0.2)
+            const double Q = 2 * (3/(8 * M_PI)) * ((m::pow<4>(state.GM()))/(m::pow<7>(state.h()[i])))  ;
+            B_[i] =  - 0.75 * C_0 * (1/B_1) * ((4 * Q * state.R()[i])/(3* state.GM()))*fout ; }
     }
 }
 
-
-FreddiState::Woods1996AGNWind::Woods1996AGNWind(const FreddiState& state):
+FreddiState::Woods1996Wind::Woods1996Wind(const FreddiState& state):
         BasicWind(state),
         C_0(state.args().disk->windparams.at("C_0")),
-        T_ic(state.args().disk->windparams.at("T_ic")) {
+        T_iC(state.args().disk->windparams.at("T_iC")) {
     update(state);
 }
 
-void FreddiState::Woods1996AGNWind::update(const FreddiState& state) {
+void FreddiState::Woods1996Wind::update(const FreddiState& state) {
     BasicWind::update(state);
     const auto disk = state.args().disk;
     const double L = state.Mdot_in() * m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT) * state.eta();
     const double L_edd = (4.0 * M_PI * state.GM()* 2.0 * disk->mu * GSL_CONST_CGSM_MASS_PROTON * GSL_CONST_CGSM_SPEED_OF_LIGHT / GSL_CONST_CGSM_THOMSON_CROSS_SECTION);
-    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_ic);
+    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_iC);
     const double le = L/L_edd;
     double R_tr;
     if ( le <= 0.01 ) {
         R_tr = 6.0*R_iC;
     }
     else
         {
@@ -581,74 +572,74 @@
     }
 
 
 
 FreddiState::Woods1996ShieldsApproxWind::Woods1996ShieldsApproxWind(const FreddiState& state):
 BasicWind(state),
         Xi_max(state.args().disk->windparams.at("Xi_max")),
-        T_ic(state.args().disk->windparams.at("T_ic")),
-        Pow(state.args().disk->windparams.at("Pow")) {
+        T_iC(state.args().disk->windparams.at("T_iC")),
+        W_pow(state.args().disk->windparams.at("W_pow")) {
     update(state);
 }
 
 void FreddiState::Woods1996ShieldsApproxWind::update(const FreddiState& state) {
     BasicWind::update(state);
     const auto disk = state.args().disk;
     const double L = state.Mdot_in() * m::pow<2>(GSL_CONST_CGSM_SPEED_OF_LIGHT) * state.eta();
-    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_ic);
-    //const double VeL = std::sqrt(state.GM()/R_iC) ;
-    //const double C_iC = std::sqrt((GSL_CONST_CGSM_BOLTZMANN * T_ic)/( GSL_CONST_CGSM_MASS_PROTON));
+    const double R_iC = (state.GM() * disk->mu * GSL_CONST_CGSM_MASS_PROTON)/(GSL_CONST_CGSM_BOLTZMANN * T_iC);
+    const double VeL = std::sqrt(state.GM()/R_iC) ;
+    const double C_iC = std::sqrt((GSL_CONST_CGSM_BOLTZMANN * T_iC)/( GSL_CONST_CGSM_MASS_PROTON));
     //const double m_ch0 = disk->Mdot0 / (M_PI * state.R().back()*state.R().back());
     const double L_edd = (4.0 * M_PI * state.GM()* 2.0 * disk->mu * GSL_CONST_CGSM_MASS_PROTON * GSL_CONST_CGSM_SPEED_OF_LIGHT / GSL_CONST_CGSM_THOMSON_CROSS_SECTION);
-    const double L_crit = (1.0 / 8.0) * std::sqrt(GSL_CONST_CGSM_MASS_ELECTRON / (disk->mu * GSL_CONST_CGSM_MASS_PROTON)) * std::sqrt((GSL_CONST_CGSM_MASS_ELECTRON * GSL_CONST_CGSM_SPEED_OF_LIGHT* GSL_CONST_CGSM_SPEED_OF_LIGHT ) / (GSL_CONST_CGSM_BOLTZMANN * T_ic)) * L_edd;
-    const double el = L/L_crit;
-    
-   //std::cerr << "\t" << Lcrit << "\t" << L_crit   << "\t" << std::endl;
+    const double L_crit = 0.03 * std::sqrt(1e8/T_iC) * L_edd;
+    const double el = L / L_crit;
+
+
 
     //std::cerr << "\t" << L << " \t" << L_edd << "\t" << L/L_edd  << "\t" << L_crit << "\t" << R_iC << "\t" << state.eta() << "\t" << std::endl;
 
     for (size_t i = state.first(); i <= state.last(); ++i) {
         if (state.R()[i] > 0.1*R_iC) {
             //  1986ApJ...306...90S page 2
             const double xi = state.R()[i] / R_iC;
             const double xi1 = R_iC / state.R()[i];
-            const double T_ch = T_ic * std::pow(el, 2.0 / 3.0) * std::pow(xi, -2.0 / 3.0);
+            const double T_ch = T_iC * std::pow(el, 2.0 / 3.0) * std::pow(xi, -2.0 / 3.0);
             const double C_ch = std::sqrt((GSL_CONST_CGSM_BOLTZMANN * T_ch) / (disk->mu * GSL_CONST_CGSM_MASS_PROTON));
             const double C0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
             const double Fr =
                     L / (4.0 * M_PI * m::pow<2>(state.R()[i]) * Xi_max * C_ch * GSL_CONST_CGSM_SPEED_OF_LIGHT);
 //const double Fc = std::pow(((1.0 + ( ((0.125 * el + 0.00382)/ xi) *((0.125 * el + 0.00382)/ xi) ))/( 1 + 1/( (el*el*el*el*(1 + 262.0*xi*xi))*(el*el*el*el*(1 + 262.0*xi*xi)) ) ) ), 1.0/6.0) ;
             const double Fc = ((std::pow((1 + m::pow<2>(((0.125 * el + 0.00382) * xi1))), (1.0 / 6.0))) /
                                std::pow((1 + m::pow<-2>((m::pow<4>(el)* (1.0 + 262.0 * m::pow<2>(xi))))),
                                         (1.0 / 6.0)));
 	    //const double Fc = ((std::pow((1 + std::pow(((0.125 * el + 0.00382) * xi1), 2.0)), (1.0 / 6.0))) /
               //                 std::pow((1 + std::pow((el * el * el * el * (1.0 + 262.0 * xi * xi)), -2.0)),
                 //                        (1.0 / 6.0)));
             const double Expo = std::exp(-(((1.0 - (1 / std::sqrt(1.0 + 0.25 * m::pow<2>(xi1)))) *
                                             (1.0 - (1 / std::sqrt(1.0 + 0.25 * m::pow<2>(xi1))))) / (2.0 * xi)));
-            C_[i] = - 2.0 * Pow * C0 * Fr * Fc * Expo;
+            C_[i] = - 2.0 * W_pow * C0 * Fr * Fc * Expo;
         }
 
     }
 }
 
 FreddiState::PeriodPaperWind::PeriodPaperWind(const FreddiState& state):
 	BasicWind(state),
-	C_w(state.args().disk->windparams.at("C_w")) {
+	W_pow(state.args().disk->windparams.at("W_pow")) {
     update(state);
 }
 
 void FreddiState::PeriodPaperWind::update(const FreddiState& state) {
     BasicWind::update(state);
     const auto disk = state.args().disk;
 
     for (size_t i = state.first(); i <= state.last(); ++i) {
 	//const double C0 = (4.0 * M_PI * m::pow<3>(state.h()[i])) / (m::pow<2>(state.GM()));
 	const double Mdot = state.Mdot_in() * (state.h()[i] - state.h()[state.first()]) /(m::pow<2>(state.h()[state.last()] - state.h()[state.first()])) ;
-	C_[i] = - 2.0 * C_w * Mdot;
+	C_[i] = - 2.0 * W_pow * Mdot;
     }
 }
 
 FreddiState::BasicFreddiIrradiationSource::~BasicFreddiIrradiationSource() {}
 
 
 Vec3 FreddiState::BasicFreddiIrradiationSource::position(const FreddiState& state) const {
```

### Comparing `freddi-2.0.0b2/cpp/src/geometry.cpp` & `freddi-2.0b0/cpp/src/geometry.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/nonlinear_diffusion.cpp` & `freddi-2.0b0/cpp/src/nonlinear_diffusion.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/ns/ns_evolution.cpp` & `freddi-2.0b0/cpp/src/ns/ns_evolution.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #include <exception>
 
-#include "exceptions.hpp"
 #include "ns/ns_evolution.hpp"
 
 
 FreddiNeutronStarEvolution::ConstKappaT::ConstKappaT(double value):
 		value(value) {}
 
 double FreddiNeutronStarEvolution::ConstKappaT::operator()(const FreddiNeutronStarEvolution& freddi, double R) const {
@@ -45,15 +44,15 @@
 FreddiNeutronStarEvolution::NeutronStarStructure::NeutronStarStructure(
 		const NeutronStarArguments &args_ns, FreddiEvolution* evolution):
 		args_ns(args_ns),
 		kappa_t(initialize_kappa_t(args_ns)),
 		R_x(args_ns.Rx),
 		redshift(initialize_redshift(evolution, args_ns)),
 		R_m_min(std::max(R_x, evolution->R()[evolution->first()])),
-		mu_magn(args_ns.mu_magn),
+		mu_magn(0.5 * args_ns.Bx * m::pow<3>(R_x)),
 		R_cor(std::cbrt(evolution->GM() / m::pow<2>(2*M_PI * args_ns.freqx))),
 		R_dead(args_ns.Rdead > 0. ? args_ns.Rdead : INFINITY),
 //		F_dead((*kappa_t)(R_dead / R_cor) * m::pow<2>(mu_magn) / m::pow<3>(R_dead)),
 		inverse_beta(args_ns.inversebeta),
 		epsilon_Alfven(args_ns.epsilonAlfven),
 		hot_spot_area(args_ns.hotspotarea),
 		Fmagn(initialize_Fmagn(evolution)),
@@ -431,24 +430,24 @@
 		return;
 	}
 	// check that Mdot decaying:
 	if ( Mdot_in() > Mdot_in_prev() ) {
 		return;
 	}
 
-	double R_m = std::max(R_m_min(), R_Alfven());
+	double R_m = std::max(R_m_min(), R_alfven());
 	R_m = std::min(R_m, R_dead());
 	size_t ii;
 	for (ii = first(); ii <= last() - 2; ii++) {
 		if (R()[ii + 1] > R_m){
 			break;
 		}
 	}
 	if (ii >= last() - 2) {
-		throw RadiusCollapseException();
+		throw std::runtime_error("R_in > R_out");
 	}
 	R_m = R()[ii];
 	current_.first = ii;
 
 	double new_F_in = 0;
 	if (inverse_beta() <= 0.) {
 		if (R_m <= R_cor()) {
@@ -463,16 +462,16 @@
 
 
 double FreddiNeutronStarEvolution::Mdot_in() const {
 	const double dF_dh = (F()[first() + 1] - F()[first()]) / (h()[first() + 1] - h()[first()]);
 	return dF_dh + dFmagn_dh()[first()];
 }
 
-double FreddiNeutronStarEvolution::R_Alfven() const {
-	return ns_str_->args_ns.R_Alfven(GM(), Mdot_in());
+double FreddiNeutronStarEvolution::R_alfven() const {
+	return epsilon_Alfven() * std::pow(m::pow<4>(mu_magn()) / (m::pow<2>(Mdot_in()) * GM()), 1./7.);
 }
 
 IrradiatedStar::sources_t FreddiNeutronStarEvolution::star_irr_sources() {
 	auto sources = FreddiEvolution::star_irr_sources();
 	sources.push_back(ns_irr_source_->irr_source(*this, Lbol_ns()));
 	return sources;
 }
```

### Comparing `freddi-2.0.0b2/cpp/src/ns/ns_options.cpp` & `freddi-2.0b0/cpp/src/ns/ns_options.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -103,57 +103,57 @@
 		};
 	}
 
 	throw po::invalid_option_value("Unknown --kappattype=" + kappattype);
 }
 
 po::options_description NeutronStarOptions::description() {
-	po::options_description od("Parameters of accreting neutron star:\n");
+	po::options_description od("Parameters of accreting neutron star");
 	od.add_options()
 			( "nsprop", po::value<std::string>()->default_value(default_nsprop),
-					"Neutron star properties name: defines geometry (default values of --Rx, --Risco, and --freqx) and accretion->radiation efficiency of NS\n\n"
+					"Neutron star geometry and radiation properties name and specifies default values of --Rx, --Risco and --freqx\n\n"
 	 				"Values:\n"
-	  				"  dummy: NS accretion->radiation efficiency is R_g * (1 / R_x - 1 / 2R_in), default --freqx is 0, default Rx is 1e6, default Risco is Kerr value\n"
-	   				"  newt: NS accretion->radiation efficiency is a function of NS frequency, calculated in Newtonian mechanics (see Lipunova+2021), that's why --freqx must be specified explicitly\n"
-					"  sibgatullin-sunyaev2000: NS accretion->radiation efficiency and default values of Rx and Risco are functions of NS frequency, calculated for a specific equation of state for a NS with weak magnetic field (Sibgatullin & Sunyaev, 2000, Astronomy Letters, 26, 699), that's why --freqx must be specified explicitly\n")
-			( "freqx", po::value<double>(), "Accretor rotation frequency, Hz. This parameter is not linked to --kerr, which could be reconciled manually (currently, --kerr is not needed for freddi-ns)\n" )
-			( "Rx", po::value<double>(), "Accretor radius, cm\n" )
-			( "Bx", po::value<double>()->required(), "Accretor polar magnetic induction, G\n" )
-			( "hotspotarea", po::value<double>()->default_value(default_hotspotarea), "Total area of the region on the accretor radiating because of accretion, normalized by the accretor surface area\n" )
-			( "epsilonAlfven", po::value<double>()->default_value(default_epsilonAlfven), "Magnetosphere radius in units of the Alfven radius, which is defined as (mu^4/G/M/sqrt(Mdot))^(1/7)\n" ) 
-			( "inversebeta", po::value<double>()->default_value(default_inversebeta), "Not currently in use\n" )
-			( "Rdead", po::value<double>()->default_value(default_Rdead), "Maximum inner radius of the disk that can be achieved, cm\n" )
+	  				"  dummy: NS radiation efficiency is R_g * (1 / R_x - 1 / 2R_in), default --freqx is 0, default Rx is 1e6, default Risco is Kerr value\n"
+	   				"  newt: NS radiation efficiency is a functions of NS frequency, that's why --freqx must be specified explicitly\n"
+					"  sibgatullin-sunyaev2000: NS radiation efficiency, and default values of Rx and Risco are functions of NS frequency, that's why --freqx must be specified explicitly")
+			( "freqx", po::value<double>(), "Accretor rotation frequency, Hz. This parameter is not linked to --kerr, agree them yourself" )
+			( "Rx", po::value<double>(), "Accretor radius, cm" )
+			( "Bx", po::value<double>()->required(), "Accretor polar magnetic induction, G" )
+			( "hotspotarea", po::value<double>()->default_value(default_hotspotarea), "??? Relative area of hot spot on the accretor" )
+			( "epsilonAlfven", po::value<double>()->default_value(default_epsilonAlfven), "Factor in Alfven radius formula" )
+			( "inversebeta", po::value<double>()->default_value(default_inversebeta), "???" )
+			( "Rdead", po::value<double>()->default_value(default_Rdead), "Maximum inner radius of the disk that can be obtained, it characterises minimum torque in the dead disk, cm" )
 			( "fptype", po::value<std::string>()->default_value(default_fptype),
-					"Scenario to determine the fraction fp of accreted mass. The rest of the disk inner accretion rate is propelled away.\n\n"
+					"??? Accretor Mdot fraction mode fp.\n\n"
 					"Values:\n"
-	 				"  no-outflow: the matter reaching the inner disk radius always falls onto NS, fp = 1\n"
-	  				"  propeller: the matter always flows away, fp = 0\n"
-	   				"  corotation-block: like 'no-outflow' when the inner disk radius is smaller than the corotation radius, like 'propeller' otherwise\n"
-					"  geometrical: experimental. Generalization of 'corotation-block' for the case of misaligned NS magnetic axis. Requires --fp-geometrical-chi to be specified\n"
-					"  eksi-kutlu2010: Under construction\n"
-	 				"  romanova2018: fp is an analytical function of the fastness, found from MHD simulations by Romanova et al. (2018, NewA, 62, 94): fp = 1 - par1*fastness^par2. This requires --romanova2018-par1 and --romanova2018-par2 to be specified\n" )
-			( "fp-geometrical-chi", po::value<double>(), "angle between the disk rotation axis and the NS magnetic axis, used for --fptype=geometrical, degrees\n" )
-			( "romanova2018-par1", po::value<double>(), "par1 value for --fptype=romanova2018 and --kappattype=romanova2018\n" )
-			( "romanova2018-par2", po::value<double>(), "par2 value for --fptype=romanova2018 and --kappattype=romanova2018\n" )
+	 				"  no-outflow: all the matter passing inner disk radius falling onto neutron star, fp = 1\n"
+	  				"  propeller: all the matter flows away from both disk and neutron star, fp = 0\n"
+	   				"  corotation-block: like 'no-otflow' when Alfven radius is smaller than corotation radius, like 'propeller' otherwise\n"
+					"  geometrical: generalisation of 'corotation-block' for the case of not co-directional of disk rotation axis and neutron star magnetic field axis. Requires --fp-geometrical-chi to be specified\n"
+					"  eksi-kutlu2010: ???\n"
+	 				"  romanova2018: ???, requires --romanova2018-par1 and --romanova2018-par2 to be specified" )
+			( "fp-geometrical-chi", po::value<double>(), "angle between disk rotation axis and neutron star magnetic axis for --fptype=geometrical, degrees" )
+			( "romanova2018-par1", po::value<double>(), "??? par1 value for --fptype=romanova2018 and --kappattype=romanova2018" )
+			( "romanova2018-par2", po::value<double>(), "??? par2 value for --fptype=romanova2018 and --kappattype=romanova2018" )
 			( "kappattype", po::value<std::string>()->default_value(default_kappat_type),
-					"kappa_t describes how strong is the interaction between the NS magnetosphere and disk: total (accelerating) magnetic torque applied to the disc is kappa_t(R) * mu^2 / R^3.\n\n"
+					"kappa_t describes how strong is interaction between neutron star magnitosphere and disk, magnetic torque is kappa_t(R) * mu^2 / R^3. This parameter describes type of radial destribution of this parameter\n\n"
 					"Values:\n"
 					"  const: doesn't depend on radius, kappa_t = value. Requires --kappat-const-value to be specified\n"
-					"  corstep: kappa_t can be different inside and outside the corotation radius. Requires --kappat-corstep-in and --kappat-corstep-out to be specified\n"
-					"  romanova2018: experimental. Similar to corstep option, but the outside value is reduced by the portion taken away by the outflow (see Table 2 of Romanova+2018, NewA, 62, 94). Requires --kappat-romanova2018-in, --kappat-romanova2018-out --romanova2018-par1 and --romanova-par2 to be specified\n" )
-			( "kappat-const-value", po::value<double>()->default_value(default_kappat_value), "kappa_t value for --kappattype=const\n" )
-			( "kappat-corstep-in", po::value<double>()->default_value(default_kappat_value), "kappa_t value inside the corotation radius for --kappattype=corstep\n" )
-			( "kappat-corstep-out", po::value<double>()->default_value(default_kappat_value), "kappa_t value outside the corotation radius for --kappattype=corstep\n" )
-			( "kappat-romanova2018-in", po::value<double>()->default_value(default_kappat_value), "kappa_t value inside the corotation radius for --kappattype=romanova2018\n" )
-			( "kappat-romanova2018-out", po::value<double>()->default_value(default_kappat_value), "kappa_t value outside the corotation radius for --kappattype=romanova2018\n" )
+					"  corstep: kappa_t is 'in' inside corotation radius, and 'out' outside. Requires --kappat-corstep-in and --kappat-corstep-out to be specified\n"
+					"  romanova2018: similar to corstep option, but the outside value is reduced by the portion taken away by wind (see Table 2 of Romanova+2018,NewA,62,94). Requires --kappat-romanova2018-in, --kappat-romanova2018-out --romanova2018-par1 and --romanova-par2 to be specified" )
+			( "kappat-const-value", po::value<double>()->default_value(default_kappat_value), "kappa_t value for --kappattype=const" )
+			( "kappat-corstep-in", po::value<double>()->default_value(default_kappat_value), "kappa_t value inside corotation radius for --kappattype=corstep" )
+			( "kappat-corstep-out", po::value<double>()->default_value(default_kappat_value), "kappa_t value outside corotation radius for --kappattype=corstep" )
+			( "kappat-romanova2018-in", po::value<double>()->default_value(default_kappat_value), "kappa_t value inside corotation radius for --kappattype=romanova2018" )
+			( "kappat-romanova2018-out", po::value<double>()->default_value(default_kappat_value), "kappa_t value outside corotation radius for --kappattype=romanova2018" )
 			( "nsgravredshift", po::value<std::string>()->default_value(default_ns_grav_redshift),
-					"Neutron star gravitational redshift flag.\n\n"
+					"Neutron star gravitational redshift type.\n\n"
 					"Values:\n"
-					"  off: gravitational redshift is not taken into account\n"
-					"  on: redshift is (1 - R_sch / Rx), where R_sch = 2GM/c^2\n" )
+					"  off: gravitational redshift doesn't taken into account\n"
+					"  on: redshift is (1 - R_sch / Rx), where R_sch = 2GM/c^2" )
 			;
 	return od;
 }
 
 
 NeutronStarBasicDiskBinaryOptions::NeutronStarBasicDiskBinaryOptions(const po::variables_map &vm, const NeutronStarArguments& args_ns):
 		NeutronStarBasicDiskBinaryArguments(
@@ -171,51 +171,14 @@
 				BasicDiskBinaryOptions::riscoInitializer(vm)) {}
 
 po::options_description NeutronStarBasicDiskBinaryOptions::description() {
 	return BasicDiskBinaryOptions::description();
 }
 
 
-NeutronStarDiskStructureOptions::NeutronStarDiskStructureOptions(const po::variables_map& vm,
-																 const NeutronStarArguments& ns_args,
-																 const BasicDiskBinaryArguments& bdb_args):
-		NeutronStarDiskStructureArguments(
-				ns_args,
-				bdb_args,
-				vm["opacity"].as<std::string>(),
-				vm["Mdotout"].as<double>(),
-				vm["boundcond"].as<std::string>(),
-				vm["Thot"].as<double>(),
-				std::pow(vm["Qirr2Qvishot"].as<double>(), 0.25),
-				vm["initialcond"].as<std::string>(),
-				varToOpt<double>(vm, "F0"),
-				varToOpt<double>(vm, "Mdisk0"),
-				varToOpt<double>(vm, "Mdot0"),
-				varToOpt<double>(vm, "powerorder"),
-				varToOpt<double>(vm, "gaussmu"),
-				varToOpt<double>(vm, "gausssigma"),
-				vm["windtype"].as<std::string>(),
-				DiskStructureOptions::windparamsInitializer(vm)) {}
-
-po::options_description NeutronStarDiskStructureOptions::description() {
-	auto non_ns_od = DiskStructureOptions::description();
-	po::options_description od(DiskStructureOptions::caption);
-	for (const auto &non_ns_option : non_ns_od.options()) {
-		if (non_ns_option->long_name() == "initialcond") {
-			od.add_options()
-					( "initialcond", po::value<std::string>()->default_value(default_initialcond), (non_ns_option->description() + "  quasistat-ns: Distibution of the initial viscous torque in the disc is  F = F0 * f_F(xi) * (1-h_in/h_out/xi) / (1-h_in/h_out), where xi=h/h_out and f_F(xi) is taken from Lipunova & Shakura (2000)\n").c_str() )
-					;
-		} else {
-			od.add(non_ns_option);
-		}
-	}
-	return od;
-}
-
-
 NeutronStarSelfIrradiationOptions::NeutronStarSelfIrradiationOptions(const po::variables_map& vm, const DiskStructureArguments& dsa_args):
 		NeutronStarSelfIrradiationArguments(
 				vm["Cirr"].as<double>(),
 				vm["irrindex"].as<double>(),
 				vm["Cirrcold"].as<double>(),
 				vm["irrindexcold"].as<double>(),
 				vm["h2rcold"].as<double>(),
@@ -225,36 +188,36 @@
 		throw po::error("Set positive --Cirr when --boundcond=Tirr");
 	}
 }
 
 po::options_description NeutronStarSelfIrradiationOptions::description() {
 	auto od = SelfIrradiationOptions::description();
 	od.add_options()
-			( "angulardistns", po::value<std::string>()->default_value(default_angular_dist_ns), "Flag to calculate angular distribution the NS emission. Values: isotropic, plane\n" )
+			( "angulardistns", po::value<std::string>()->default_value(default_angular_dist_ns), "Angular distribution type of the neutron star X-ray radiation. Values: isotropic, plane" )
 			;
 	return od;
 }
 
 
 FreddiNeutronStarOptions::FreddiNeutronStarOptions(const po::variables_map &vm) {
 	ns.reset(new NeutronStarOptions(vm));
 
 	general.reset(new GeneralOptions(vm));
 	basic.reset(new NeutronStarBasicDiskBinaryOptions(vm, *ns));
-	disk.reset(new NeutronStarDiskStructureOptions(vm, *ns, *basic));
+	disk.reset(new DiskStructureOptions(vm, *basic));
 	irr_ns.reset(new NeutronStarSelfIrradiationOptions(vm, *disk));
 	irr = irr_ns;
 	flux.reset(new FluxOptions(vm));
 	calc.reset(new CalculationOptions(vm));
 }
 
 po::options_description FreddiNeutronStarOptions::description() {
 	po::options_description desc("Freddi NS: numerical calculation of accretion disk evolution");
 	desc.add(GeneralOptions::description());
 	desc.add(NeutronStarBasicDiskBinaryOptions::description());
-	desc.add(NeutronStarDiskStructureOptions::description());
+	desc.add(DiskStructureOptions::description());
 	desc.add(NeutronStarOptions::description());
 	desc.add(NeutronStarSelfIrradiationOptions::description());
 	desc.add(FluxOptions::description());
 	desc.add(CalculationOptions::description());
 	return desc;
 }
```

### Comparing `freddi-2.0.0b2/cpp/src/ns/ns_output.cpp` & `freddi-2.0b0/cpp/src/ns/ns_output.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/opacity_related.cpp` & `freddi-2.0b0/cpp/src/opacity_related.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/options.cpp` & `freddi-2.0b0/cpp/src/options.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 				vm["dir"].as<std::string>(),
 				vm["precision"].as<unsigned int>(),
 				vm["tempsparsity"].as<unsigned int>(),
 				(vm.count("fulldata") > 0),
 				(vm.count("stdout") > 0)) {}
 
 po::options_description GeneralOptions::description() {
-	po::options_description od("General options:");
+	po::options_description od("General options");
 	od.add_options()
-			( "help,h", "Produce help message\n" )
-			( "config", po::value<std::string>(), "Set filepath for additional configuration file. There is no need to declare a configuration file with the default name freddi.ini\n" )
-			( "prefix", po::value<std::string>()->default_value(default_prefix), "Set prefix for output filenames. Output file with distribution of parameters over time is PREFIX.dat\n" )
-			( "stdout", "Output temporal distribution to stdout instead of PREFIX.dat file\n" )
-			( "dir,d", po::value<std::string>()->default_value(default_dir), "Choose the directory to write output files. It should exist\n" )
-			( "precision", po::value<unsigned int>()->default_value(default_output_precision), "Number of digits to print into output files\n" )
-			( "tempsparsity", po::value<unsigned int>()->default_value(default_temp_sparsity_output), "Output every k-th time moment\n" )
-			( "fulldata", "Output files PREFIX_%d.dat with radial structure for every time step. Default is to output only PREFIX.dat with global disk parameters for every time step\n" )
+			( "help,h", "Produce help message" )
+			( "config", po::value<std::string>(), "Set additional configuration filepath" )
+			( "prefix", po::value<std::string>()->default_value(default_prefix), "Set prefix for output filenames. Output file with distribution of parameters over time is PREFIX.dat" )
+			( "stdout", "Output temporal distribution to stdout instead of PREFIX.dat file" )
+			( "dir,d", po::value<std::string>()->default_value(default_dir), "Choose the directory to write output files. It should exist" )
+			( "precision", po::value<unsigned int>()->default_value(default_output_precision), "Number of digits to print into output files" )
+			( "tempsparsity", po::value<unsigned int>()->default_value(default_temp_sparsity_output), "Output every k-th time moment" )
+			( "fulldata", "Output files PREFIX_%d.dat with radial structure for every time step. Default is to output only PREFIX.dat with global disk parameters for every time step" )
 			;
 	return od;
 }
 
 
 BasicDiskBinaryOptions::BasicDiskBinaryOptions(const po::variables_map &vm):
 		BasicDiskBinaryArguments(
@@ -71,27 +71,27 @@
 		const double Mx = sunToGram(vm["Mx"].as<double>());
 		return rgToCm(vm["risco"].as<double>(), Mx);
 	}
 	return {};
 }
 
 po::options_description BasicDiskBinaryOptions::description() {
-	po::options_description od("Basic binary and disk parameters\n");
+	po::options_description od("Basic binary and disk parameter");
 	od.add_options()
-			( "alpha,a", po::value<double>()->required(), "Alpha parameter of Shakura-Sunyaev model\n" )
-			( "alphacold", po::value<double>(), "Alpha parameter of cold disk, currently it is used only for the critical maximum value of the surface density of the cold disk Sigma_minus (Lasota et al., 2008, A&A 486, 523) and the cooling front velocity (Ludwig et al., 1994, A&A 290, 473), see --Qirr2Qvishot. Default value is --alpha divided by ten\n" )  // default_alpha_to_alphacold
-			( "Mx,M", po::value<double>()->required(), "Mass of the central object, in the units of solar masses\n" )
-			( "kerr", po::value<double>()->default_value(default_kerr), "Dimensionless Kerr parameter of the black hole\n" )
-			( "Mopt",	po::value<double>()->required(), "Mass of the optical star, in units of solar masses\n" )
-			( "rochelobefill", po::value<double>()->default_value(default_roche_lobe_fill), "Dimensionless factor describing a size of the optical star. Polar radius of the star is rochelobefill * (polar radius of critical Roche lobe)\n" )
-			( "Topt", po::value<double>()->default_value(default_Topt), "Effective temperature of the optical star, in units of Kelvins\n" )
-			( "period,P", po::value<double>()->required(), "Orbital period of the binary system, in units of days\n" )
-			( "rin", po::value<double>(), "Inner radius of the disk, in the units of the gravitational radius of the central object GM/c^2. There is no need to set it for a neutron star. If it isn't set for a black hole then the radius of ISCO orbit is used, defined by --Mx and --kerr values\n" )
-			( "rout,R", po::value<double>(), "Outer radius of the disk, in units of solar radius. If it isn't set then the tidal radius is used, defined by --Mx, --Mopt and --period values as 90% of the Roche lobe radius (Papaloizou & Pringle, 1977, MNRAS, 181, 441; see also Artymowicz & Lubow, 1994, ApJ, 421, 651; http://xray.sai.msu.ru/~galja/images/tidal_radius.pdf)\n" )
-			( "risco", po::value<double>(), "Innermost stable circular orbit, in units of gravitational radius of the central object GM/c^2. If it isn't set then the radius of ISCO orbit is used defined by --Mx and --kerr values\n" )
+			( "alpha,a", po::value<double>()->required(), "Alpha parameter of Shakura-Sunyaev model" )
+			( "alphacold", po::value<double>(), "Alpha parameter of cold disk, currently it is used only for Sigma_minus, see --Qirr2Qvishot. Default is --alpha values divided by ten" )  // default_alpha_to_alphacold
+			( "Mx,M", po::value<double>()->required(), "Mass of the central object, in the units of solar masses" )
+			( "kerr", po::value<double>()->default_value(default_kerr), "Dimensionless Kerr parameter of the black hole" )
+			( "Mopt",	po::value<double>()->required(), "Mass of the optical star, in units of solar masses" )
+			( "rochelobefill", po::value<double>()->default_value(default_roche_lobe_fill), "Dimensionless factor describing a size of the optical star. Polar radius of the star is rochelobefill * (polar radius of critical Roche lobe)" )
+			( "Topt", po::value<double>()->default_value(default_Topt), "Thermal temperature of the optical star, in units of kelvins" )
+			( "period,P", po::value<double>()->required(), "Orbital period of the binary system, in units of days" )
+			( "rin", po::value<double>(), "Inner radius of the disk, in the units of the gravitational radius of the central object GM/c^2. If it isn't set then the radius of ISCO orbit is used defined by --Mx and --kerr values" )
+			( "rout,R", po::value<double>(), "Outer radius of the disk, in units of solar radius. If it isn't set then the tidal radius is used defined by --Mx, --Mopt and --period values" )
+			( "risco", po::value<double>(), "Innermost stable circular orbit, in units of gravitational radius of the central object GM/c^2. If it isn't set then the radius of ISCO orbit is used defined by --Mx and --kerr values" )
 			;
 	return od;
 }
 
 
 DiskStructureOptions::DiskStructureOptions(const po::variables_map &vm, const BasicDiskBinaryArguments& bdb_args):
 		DiskStructureArguments(
@@ -117,143 +117,84 @@
 
 	if (windtype == "no") {
 		return {};
 	}
 	if (windtype == "SS73C") {
 		return {};
 	}
-	if (windtype == "ShieldsOscil1986"){
-		if (vm.count("windC_w") == 0) {
-			throw po::error("--windC_w is required if --windtype=ShieldsOscil1986");
-		}
-		if (vm.count("windR_w") == 0) {
-			throw po::error("--windR_w is required if --windtype=ShieldsOscil1986");
-		}
-		return {
-				{"C_w", vm["windC_w"].as<double>()},
-				{"R_w", vm["windR_w"].as<double>()}
-		};
-	}
-	if (windtype == "Janiuk2015"){
-		if (vm.count("windA_0") == 0) {
-			throw po::error("--windA_0 is required if --windtype=Janiuk2015");
-		}
-		if (vm.count("windB_1") == 0) {
-			throw po::error("--windB_1 is required if --windtype=Janiuk2015");
-		}
-		return {
-				{"A_0", vm["windA_0"].as<double>()},
-				{"B_1", vm["windB_1"].as<double>()}
-		};
-	}
-	if (windtype == "Shields1986"){
-		if (vm.count("windXi_max") == 0) {
-			throw po::error("--windXi_max is required if --windtype=Shields1986");
-		}
-		if (vm.count("windT_ic") == 0) {
-			throw po::error("--windT_ic is required if --windtype=Shields1986");
-		}
-		if (vm.count("windPow") == 0) {
-			throw po::error("--windPow is required if --windtype=Shields1986");
-		}
-		return {
-				{"Xi_max", vm["windXi_max"].as<double>()},
-				{"T_ic", vm["windT_ic"].as<double>()},
-				{"Pow", vm["windPow"].as<double>()}
-		};
-	}
-	if (windtype == "Woods1996AGN"){
-		if (vm.count("windC_0") == 0) {
-			throw po::error("--windC_0 is required if --windtype=Woods1996AGN");
-		}
-		if (vm.count("windT_ic") == 0) {
-			throw po::error("--windT_ic is required if --windtype=Woods1996AGN");
-		}
-		return {
-				{"C_0", vm["windC_0"].as<double>()},
-				{"T_ic", vm["windT_ic"].as<double>()}
-		};
-	}
 	if (windtype == "Woods1996"){
-		if (vm.count("windXi_max") == 0) {
-			throw po::error("--windXi_max is required if --windtype=Woods1996");
+		if (vm.count("windXi") == 0) {
+			throw po::error("--windXi is required if --windtype=Woods1996");
 		}
-		if (vm.count("windT_ic") == 0) {
-			throw po::error("--windT_ic is required if --windtype=Woods1996");
+		if (vm.count("windTic") == 0) {
+			throw po::error("--windTic is required if --windtype=Woods1996");
 		}
 		if (vm.count("windPow") == 0) {
 			throw po::error("--windPow is required if --windtype=Woods1996");
 		}
 		return {
-				{"Xi_max", vm["windXi_max"].as<double>()},
-				{"T_ic", vm["windT_ic"].as<double>()},
-				{"Pow", vm["windPow"].as<double>()}
+				{"Xi_max", vm["windXi"].as<double>()},
+				{"T_iC", vm["windTic"].as<double>()},
+				{"W_pow", vm["windPow"].as<double>()}
 		};
 	}
 	if (windtype == "toy"){
-		if (vm.count("windC_w") == 0) {
-			throw po::error("--windC_w is required if --windtype=toy");
+		if (vm.count("windPow") == 0) {
+			throw po::error("--windPow is required if --windtype=toy");
 		}
 		return {
 
-				{"C_w", vm["windC_w"].as<double>()}
+				{"W_pow", vm["windPow"].as<double>()}
 		};
 	}
 	
 
 	throw po::invalid_option_value("Unknown --windtype=" + windtype);
 }
 
 
 po::options_description DiskStructureOptions::description() {
-	po::options_description od(DiskStructureOptions::caption);
+	po::options_description od("Parameters of the disk mode");
 	od.add_options()
-			( "opacity,O", po::value<std::string>()->default_value(default_opacity), "Opacity law: Kramers (varkappa ~ rho / T^7/2) or OPAL (varkappa ~ rho / T^5/2)\n" )
-			( "Mdotout", po::value<double>()->default_value(default_Mdotout), "Accretion rate onto the disk through its outer radius\n" )
+			( "opacity,O", po::value<std::string>()->default_value(default_opacity), "Opacity law: Kramers (varkappa ~ rho / T^7/2) or OPAL (varkappa ~ rho / T^5/2)" )
+			( "Mdotout", po::value<double>()->default_value(default_Mdotout), "Accretion rate onto the disk through its outer radius" )
 			( "boundcond", po::value<std::string>()->default_value(default_boundcond),
-					"Outer-boundary movement condition\n\n"
+					"Outer boundary movement condition\n\n"
 					"Values:\n"
 					"  Teff: outer radius of the disk moves inwards to keep photosphere temperature of the disk larger than some value. This value is specified by --Thot option\n"
-					"  Tirr: outer radius of the disk moves inwards to keep irradiation flux of the disk larger than some value. The value of this minimal irradiation flux is [Stefan-Boltzmann constant] * Tirr^4, where Tirr is specified by --Thot option\n" ) // fourSigmaCrit, MdotOut
-			( "Thot", po::value<double>()->default_value(default_Thot), "Minimum photosphere or irradiation temperature at the outer edge of the hot disk, Kelvin. For details see --boundcond description\n" )
-			( "Qirr2Qvishot", po::value<double>()->default_value(m::pow<4>(default_Tirr2Tvishot)), "Minimum Qirr / Qvis ratio at the outer edge of the hot disk to switch the control over the evolution of the hot disk radius: from temperature-based regime to Sigma-based cooling-front regime (see Lipunova et al. (2021, Section 2.4) and Eq. A.1 in Lasota et al. 2008; --alpha value is used for Sigma_plus and --alphacold value is used for Sigma_minus)\n" )
+					"  Tirr: outer radius of the disk moves inwards to keep irradiation flux of the disk larger than some value. The value of this minimal irradiation flux is [Stefan-Boltzmann constant] * Tirr^4, where Tirr is specified by --Thot option" ) // fourSigmaCrit, MdotOut
+			( "Thot", po::value<double>()->default_value(default_Thot), "Minimum photosphere or irradiation temperature at the outer edge of the hot disk, Kelvin. For details see --boundcond description" )
+			( "Qirr2Qvishot", po::value<double>()->default_value(m::pow<4>(default_Tirr2Tvishot)), "Minimum Qirr / Qvis ratio at the outer edge of the hot disk to switch evolution from temperature-based regime to Sigma_minus-based regime (see Eq. A.1 in Lasota et al. 2008, --alphacold value is used as alpha parameter)" )
 			( "initialcond", po::value<std::string>()->default_value(default_initialcond),
 					"Type of the initial condition for viscous torque F or surface density Sigma\n\n"
 					"Values:\n"
-					"  [NB! Here below dimensionless xi = (h - h_in) / (h_out - h_in)]\n\n"
 					"  powerF: F ~ xi^powerorder, powerorder is specified by --powerorder option\n" // power does the same
-					"  linearF: F ~ xi, specific case of powerF but can be normalised by --Mdot0, see its description for details\n" // linear does the same
+					"  linearF: F ~ xi, specific case of powerF but can be normalised by --Mdot0, see its description for details" // linear does the same
 					"  powerSigma: Sigma ~ xi^powerorder, powerorder is specified by --powerorder option\n"
 					"  sineF: F ~ sin( xi * pi/2 )\n" // sinus option does the same
 					"  gaussF: F ~ exp(-(xi-mu)**2 / 2 sigma**2), mu and sigma are specified by --gaussmu and --gausssigma options\n"
-					"  quasistat: F ~ f(h/h_out) * xi * h_out/h, where f is quasi-stationary solution found in Lipunova & Shakura 2000. f(xi=0) = 0, df/dxi(xi=1) = 0\n")
-			( "F0", po::value<double>(), "Initial maximum viscous torque in the disk, dyn*cm. Can be overwritten via --Mdisk0 and --Mdot0\n" )
-			( "Mdisk0", po::value<double>(), "Initial disk mass, g. If both --F0 and --Mdisk0 are specified then --Mdisk0 is used. If both --Mdot0 and --Mdisk0 are specified then --Mdot0 is used\n" )
-			( "Mdot0", po::value<double>(), "Initial mass accretion rate through the inner radius, g/s. If --F0, --Mdisk0 and --Mdot0 are specified then --Mdot0 is used. Works only when --initialcond is set to linearF, sinusF or quasistat\n" )
-			( "powerorder", po::value<double>(), "Parameter for the powerlaw initial condition distribution. This option works only with --initialcond=powerF or powerSigma\n" )
-			( "gaussmu", po::value<double>(), "Position of the maximum for Gauss distribution, positive number not greater than unity. This option works only with --initialcond=gaussF\n" )
-			( "gausssigma", po::value<double>(), "Width of for Gauss distribution. This option works only with --initialcond=gaussF\n" )
+					"  quasistat: F ~ f(h/h_out) * xi * h_out/h, where f is quasi-stationary solution found in Lipunova & Shakura 2000. f(xi=0) = 0, df/dxi(xi=1) = 0\n\n"
+					"Here xi is (h - h_in) / (h_out - h_in)\n")
+			( "F0", po::value<double>(), "Initial maximum viscous torque in the disk, dyn*cm. Can be overwritten via --Mdisk0 and --Mdot0" )
+			( "Mdisk0", po::value<double>(), "Initial disk mass, g. If both --F0 and --Mdisk0 are specified then --Mdisk0 is used. If both --Mdot0 and --Mdisk0 are specified then --Mdot0 is used" )
+			( "Mdot0", po::value<double>(), "Initial mass accretion rate through the inner radius, g/s. If --F0, --Mdisk0 and --Mdot0 are specified then --Mdot0 is used. Works only when --initialcond is set to linearF, sinusF or quasistat" )
+			( "powerorder", po::value<double>(), "Parameter for the powerlaw initial condition distribution. This option works only with --initialcond=powerF or powerSigma" )
+			( "gaussmu", po::value<double>(), "Position of the maximum for Gauss distribution, positive number not greater than unity. This option works only with --initialcond=gaussF" )
+			( "gausssigma", po::value<double>(), "Width of for Gauss distribution. This option works only with --initialcond=gaussF" )
 			( "windtype", po::value<std::string>()->default_value(default_wind),
 			        "Type of the wind\n\n"
+					"Values:\n"
 					"  no: no wind\n"
 					"  SS73C: super-Eddington spherical wind from Shakura-Sunyaev 1973\n"
-					"  ShieldsOscil1986: toy wind model from Shields et al. 1986 which was used to obtain oscillations in the disk luminosity. Requires --windC_w and --windR_w to be specified\n"
-					"  Janiuk2015: super-Eddington wind from Janiuk et al 2015. Requires --windA_0 and --windB_1 to be specified\n"
-					"  Shields1986: thermal wind from Begelman et al. 1983 and Shields et al. 1986. Requires --windXi_max, --windT_ic and --windPow to be specified\n"
-					"  Woods1996AGN: thermal AGN wind from Woods et al. 1996. Requires --windC_0 and --windT_ic to be specified\n"
-					"  Woods1996: thermal wind from Woods et al. 1996. Requires --windXi_max, --windT_ic and --windPow to be specified\n"
-					"  toy: a toy wind model used in arXiv:2105.11974, the mass loss rate is proportional to the central accretion rate. Requires --windC_w to be specified\n")
-			( "windC_w", po::value<double>(), "The ratio of the mass loss rate due to wind to the central accretion rate, |Mwind|/Macc\n")
-			( "windR_w", po::value<double>(), "The ratio of the wind launch radius to the outer disk radius, Rwind/Rout\n")		
-			( "windA_0", po::value<double>(), "Dimensionless parameter characterizing the strength of the super-Eddington wind in the framework of the model Janiuk et al. 2015. Effective value range from 10 to 25\n")
-			( "windB_1", po::value<double>(), "The quantity is of the order of unity. Characterizes the relationship between the change in energy per particle and virial energy.\nE = B_1 * k * T\n")
-			( "windXi_max", po::value<double>(), "Ionization parameter, the ratio of the radiation and gas pressures\n" )
-			( "windT_ic", po::value<double>(), "Inverse Compton temperature, K. Characterizes the hardness of the irradiating spectrum\n")
-			( "windPow", po::value<double>(), "Multiplicative coefficient to control wind power\n")
-			( "windC_0", po::value<double>(), "Characteristic column density of the wind mass loss rate from Woods et al. 1996 model, g/(s*cm^2). For AGN approx value is 3e-13 g/(s*cm^2)\n")
+					"  Janiuk2015: super-Eddington Janiuk et al. 2015\n"
+					"  Woods1996: thermal wind Woods et al. 1996. Requires --windXi, --windTic and --windPow to be specified"
+					"  toy: a toy wind model used in arXiv:2105.11974, the mass loss rate is proportional to the central accretion rate. Requires --windPow to be specified")
+			( "windXi", po::value<double>(), "Ionization parameter, the ratio of the radiation and gas pressures" )
+			( "windTic", po::value<double>(), "Inverse Compton temperature, K. Characterizes the hardness of the irradiating spectrum")
+			( "windPow", po::value<double>(), "Multiplicative coefficient to control wind power")
 			;
 	return od;
 }
 
 
 SelfIrradiationOptions::SelfIrradiationOptions(const po::variables_map &vm, const DiskStructureArguments &dsa_args):
 		SelfIrradiationArguments(
@@ -265,22 +206,22 @@
 				vm["angulardistdisk"].as<std::string>()) {
 	if (Cirr <= 0. && dsa_args.boundcond == "Tirr") {
 		throw po::error("Set positive --Cirr when --boundcond=Tirr");
 	}
 }
 
 po::options_description SelfIrradiationOptions::description() {
-	po::options_description od("Parameters of self-irradiation:\nQirr = Cirr * (H/r / 0.05)^irrindex * L * psi / (4 pi R^2), where psi is the angular distribution of X-ray radiation\n");
+	po::options_description od("Parameters of self-irradiation.\nQirr = Cirr * (H/r / 0.05)^irrindex * L * psi / (4 pi R^2), where psi is angular distrbution of X-ray radiation");
 	od.add_options()
-			( "Cirr", po::value<double>()->default_value(default_Cirr), "Irradiation factor for the hot disk\n" )
-			( "irrindex", po::value<double>()->default_value(default_irrindex), "Irradiation index for the hot disk\n" )
-			( "Cirrcold", po::value<double>()->default_value(default_Cirr_cold), "Irradiation factor for the cold disk\n" )
-			( "irrindexcold", po::value<double>()->default_value(default_irrindex_cold), "Irradiation index for the cold disk\n" )
-			( "h2rcold", po::value<double>()->default_value(default_height_to_radius_cold), "Semi-height to radius ratio for the cold disk\n" )
-			( "angulardistdisk", po::value<std::string>()->default_value(default_angular_dist_disk), "Angular distribution of the disk X-ray radiation. Values: isotropic, plane\n" )
+			( "Cirr", po::value<double>()->default_value(default_Cirr), "Irradiation factor for the hot disk" )
+			( "irrindex", po::value<double>()->default_value(default_irrindex), "Irradiation index for the hot disk" )
+			( "Cirrcold", po::value<double>()->default_value(default_Cirr_cold), "Irradiation factor for the cold disk" )
+			( "irrindexcold", po::value<double>()->default_value(default_irrindex_cold), "Irradiation index for the cold disk" )
+			( "h2rcold", po::value<double>()->default_value(default_height_to_radius_cold), "Seme-height to radius ratio for the cold disk, it affects disk shadow in star" )
+			( "angulardistdisk", po::value<std::string>()->default_value(default_angular_dist_disk), "Angular distribution of the disk X-ray radiation. Values: isotropic, plane" )
 			;
 	return od;
 }
 
 
 FluxOptions::FluxOptions(const po::variables_map &vm):
 		FluxArguments(
@@ -318,27 +259,27 @@
 			throw po::invalid_option_value("Passband file doesn't exist");
 		}
 	}
 	return passbands;
 }
 
 po::options_description FluxOptions::description() {
-	po::options_description od("Parameters of flux calculation:\n");
+	po::options_description od("Parameters of flux calculation");
 	od.add_options()
-			( "colourfactor", po::value<double>()->default_value(default_colourfactor), "Colour factor to calculate X-ray flux\n"  )
-			( "emin", po::value<double>()->default_value(hertzToKev(default_emin)), "Minimum energy of X-ray band, keV\n" )
-			( "emax", po::value<double>()->default_value(hertzToKev(default_emax)), "Maximum energy of X-ray band, keV\n" )
-			( "staralbedo", po::value<double>()->default_value(default_star_albedo), "Part of X-ray radiation reflected by optical star, (1 - albedo) heats star's photosphere. Used only when --starflux is specified\n" )
-			( "inclination,i", po::value<double>()->default_value(default_inclination), "Inclination of the system, degrees\n" )
-			( "ephemerist0", po::value<double>()->default_value(default_ephemeris_t0), "Ephemeris for the time of the minimum of the orbital light curve T0, phase zero corresponds to inferior conjunction of the optical star, days\n" )
-			( "distance", po::value<double>()->required(), "Distance to the system, kpc\n" )
-			( "colddiskflux", "Add Fnu for cold disk into output file. Default output is for hot disk only\n" )
-			( "starflux", "Add Fnu for irradiated optical star into output file. See --Topt, --starlod and --h2rcold options. Default is output for the hot disk only\n" )
-			( "lambda", po::value<vecd>()->multitoken()->composing(), "Wavelength to calculate Fnu, Angstrom. You can use this option multiple times. For each lambda one additional column with values of spectral flux density Fnu [erg/s/cm^2/Hz] is produced\n" )
-			( "passband", po::value<std::vector<std::string>>()->multitoken()->composing(), "Path of a file containing tabulated passband, the first column for wavelength in Angstrom, the second column for transmission factor, columns should be separated by spaces\n" )
+			( "colourfactor", po::value<double>()->default_value(default_colourfactor), "Colour factor to calculate X-ray flux"  )
+			( "emin", po::value<double>()->default_value(hertzToKev(default_emin)), "Minimum energy of X-ray band, keV" )
+			( "emax", po::value<double>()->default_value(hertzToKev(default_emax)), "Maximum energy of X-ray band, keV" )
+			( "staralbedo", po::value<double>()->default_value(default_star_albedo), "Part of X-ray radiation reflected by optical star, (1 - albedo) heats star's photosphere. Used only when --starflux is specified" )
+			( "inclination,i", po::value<double>()->default_value(default_inclination), "Inclination of the system, degrees" )
+			( "ephemerist0", po::value<double>()->default_value(default_ephemeris_t0), "Ephemeris for the time of the minimum of the orbital light curve T0, phase zero corresponds to inferior conjunction of the optical star, days" )
+			( "distance", po::value<double>()->required(), "Distance to the system, kpc" )
+			( "colddiskflux", "Add Fnu for cold disk into output file. Default output is for hot disk only" )
+			( "starflux", "Add Fnu for irradiated optical star into output file. See --Topt, --starlod and --h2rcold options. Default is output for the hot disk only" )
+			( "lambda", po::value<vecd>()->multitoken()->composing(), "Wavelength to calculate Fnu, Angstrom. You can use this option multiple times. For each lambda one additional column with values of spectral flux density Fnu [erg/s/cm^2/Hz] is produced" )
+			( "passband", po::value<std::vector<std::string>>()->multitoken()->composing(), "Path of a file containing tabulated passband, the first column for wavelength in Angstrom, the second column for transmission factor, columns should be separated by spaces" )
 			;
 	return od;
 }
 
 
 CalculationOptions::CalculationOptions(const po::variables_map &vm):
 		CalculationArguments(
@@ -357,22 +298,22 @@
 	if (vm.count("tau")) {
 		return dayToS(vm["tau"].as<double>());
 	}
 	return {};
 }
 
 po::options_description CalculationOptions::description() {
-	po::options_description od("Parameters of disk evolution calculation:\n");
+	po::options_description od("Parameters of disk evolution calculation");
 	od.add_options()
-			("inittime", po::value<double>()->default_value(default_init_time), "Initial time moment, days\n" )
-			( "time,T", po::value<double>()->required(), "Time interval to calculate evolution, days\n" )
-			( "tau",	po::value<double>(), "Time step, days\n" )
-			( "Nx",	po::value<unsigned int>()->default_value(default_Nx), "Size of calculation grid\n" )
-			( "gridscale", po::value<std::string>()->default_value(default_gridscale), "Type of grid for angular momentum h: log or linear\n" )
-			( "starlod", po::value<unsigned int>()->default_value(default_starlod), "Level of detail of the optical star 3-D model. The optical star is represented by a triangular tile, the number of tiles is 20 * 4^starlod\n" )
+			("inittime", po::value<double>()->default_value(default_init_time), "Initial time moment, days" )
+			( "time,T", po::value<double>()->required(), "Time interval to calculate evolution, days" )
+			( "tau",	po::value<double>(), "Time step, days" )
+			( "Nx",	po::value<unsigned int>()->default_value(default_Nx), "Size of calculation grid" )
+			( "gridscale", po::value<std::string>()->default_value(default_gridscale), "Type of grid for angular momentum h: log or linear" )
+			( "starlod", po::value<unsigned int>()->default_value(default_starlod), "Level of detail of the optical star 3-D model. The optical star is represented by a triangular tile, the number of tiles is 20 * 4^starlod" )
 			;
 	return od;
 }
 
 
 
 FreddiOptions::FreddiOptions(const po::variables_map& vm) {
```

### Comparing `freddi-2.0.0b2/cpp/src/orbit.cpp` & `freddi-2.0b0/cpp/src/orbit.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/output.cpp` & `freddi-2.0b0/cpp/src/output.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,20 @@
 			{"Tirrout", "K", "Irradiation temperature (Qirr / sigma_SB)^1/4 at the outer radius of the hot disk", [freddi]() {return freddi->Tirr()[freddi->last()];}},
 			{"Qirr2Qvisout", "float", "Irradiation flux to viscous flux ratio at the outer radius of the hot disk", [freddi]() {return m::pow<4>(freddi->Tirr()[freddi->last()] / freddi->Tph_vis()[freddi->last()]);}},
 			{"TphXmax", "keV", "Maximum effective temperature of the disk", [freddi]() {return kToKev(*std::max_element(freddi->Tph_X().begin() + freddi->first(), freddi->Tph_X().begin() + freddi->last() + 1));}},
 			{"Lx", "erg/s", "X-ray luminosity of the disk in the given energy range [emin, emax]", [freddi]() {return freddi->Lx();}},
 			{"Lbol", "erg/s", "Bolometric luminosity of the disk", [freddi]() {return freddi->Lbol_disk();}},
 			{"Fx", "erg/s/cm^2", "X-ray flux of the disk in the given energy range [emin, emax]", [freddi]() {return freddi->Lx() * freddi->angular_dist_disk(freddi->cosi()) / (FOUR_M_PI * m::pow<2>(freddi->distance()));}},
 			{"Fbol", "erg/s/cm^2", "Bolometric flux of the disk", [freddi]() {return freddi->Lbol_disk() * freddi->angular_dist_disk(freddi->cosi()) / (FOUR_M_PI * m::pow<2>(freddi->distance()));}},
+			{"mU", "mag", "TO BE REMOVED", [freddi]() {return freddi->mU();}},
+			{"mB", "mag", "TO BE REMOVED", [freddi]() {return freddi->mB();}},
+			{"mV", "mag", "TO BE REMOVED", [freddi]() {return freddi->mV();}},
+			{"mR", "mag", "TO BE REMOVED", [freddi]() {return freddi->mR();}},
+			{"mI", "mag", "TO BE REMOVED", [freddi]() {return freddi->mI();}},
+			{"mJ", "mag", "TO BE REMOVED", [freddi]() {return freddi->mJ();}},
 	};
 	const bool cold_disk = freddi->args().flux->cold_disk;
 	const bool star = freddi->args().flux->star;
 	const auto& lambdas = freddi->args().flux->lambdas;
 	for (size_t i = 0; i < lambdas.size(); ++i) {
 		const double lambda = lambdas[i];
 		fields.emplace_back(
```

### Comparing `freddi-2.0.0b2/cpp/src/passband.cpp` & `freddi-2.0b0/cpp/src/passband.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/rochelobe.cpp` & `freddi-2.0b0/cpp/src/rochelobe.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 #include <orbit.hpp>
 #include <rochelobe.hpp>
 #include <util.hpp>
 
 using boost::math::tools::halley_iterate;
 
 
-// omega(r,lambda,nu) - Roche potential
-// lambda, nu - cosines of angles
-// find_r - routine to find distance from the star where the Roche potential equals requested value, for chosen lambda and nu
-// initializeLagrangianPoint - find distance from the star to L1
-// initializePolarRadius - find distance in the polar direction (PolarRadius) where the potential equals the potential at L1
-// fill_factor - user-defined parameter : radius of the star = fill_factor * PolarRadius
-
 RochePotential::RochePotential(const double mass_ratio):
 		mass_ratio(mass_ratio),
 		volume_radius(BinaryFunctions::rocheLobeVolumeRadiusSemiaxis(mass_ratio)) {}
 
 double RochePotential::omega(const double r, const double lambda, const double nu) const {
 	// Cherepashchuk, Fismatlit, Moscow, 2013, Volume 1, Eq. 365, but our mass_ratio = 1/q
 	return mass_ratio / r
@@ -70,15 +63,14 @@
 		polar_radius(initializePolarRadius(roche_potential, lagrangian_point, omega)) {}
 
 double CriticalRocheLobe::initializeLagrangianPoint(const RochePotential& roche_potential) {
 	// q <= 1
 	double q = roche_potential.mass_ratio <= 1.0 ? roche_potential.mass_ratio : 1.0 / roche_potential.mass_ratio;
 	// Initial guess is a Hill radius for small mass_ratio, one minus Hill radius for large mass_ratio and 0.5 for
 	// mass_ratio = 1
-	// x0 is the initial guess, the result lies in the interval [x1,x2]
 	double x0 = std::cbrt(q / 3.0) + (0.5 - std::cbrt(1.0/3.0)) * q;
 	double x1 = 0.5 * x0;
 	double x2 = std::min(0.5, 2 * x0);
 	if (roche_potential.mass_ratio > 1.0) {
 		x0 = 1.0 - x0;
 		const double tmp = 1.0 - x1;
 		x1 = 1.0 - x2;
```

### Comparing `freddi-2.0.0b2/cpp/src/spectrum.cpp` & `freddi-2.0b0/cpp/src/spectrum.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/star.cpp` & `freddi-2.0b0/cpp/src/star.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/src/util.cpp` & `freddi-2.0b0/cpp/src/util.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/test/geometry.cpp` & `freddi-2.0b0/cpp/test/geometry.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/test/rochelobe.cpp` & `freddi-2.0b0/cpp/test/rochelobe.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/test/star.cpp` & `freddi-2.0b0/cpp/test/star.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/cpp/test/util.cpp` & `freddi-2.0b0/cpp/test/util.cpp`

 * *Files identical despite different names*

### Comparing `freddi-2.0.0b2/python/freddi/__init__.py` & `freddi-2.0b0/python/freddi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from functools import partial, singledispatch
+from functools import partial
 
 import numpy as np
 
 from ._freddi import _Freddi, _FreddiNeutronStar
 from .evolution_result import EvolutionResult
 
 
@@ -44,56 +44,40 @@
     @classmethod
     def _from_boost(cls, boost_freddi):
         obj = cls.__new__(cls)
         obj._freddi = boost_freddi
         return obj
 
     @classmethod
-    def from_astropy(cls, **kwargs):
-        """Alternative Freddi constructor accepting astropy Quantity
+    def alt(cls, **kwargs):
+        """Alternative Freddi constructor accepting astropy Quantity and str
 
         All physical values can be passed as `astropy.units.Quantity`, and all
-        string values can be passed as `str`. Requires `astropy` package
+        string values can be passed as `str`. Needs `astropy` module to run
 
         Parameters
         ----------
         **kwargs :
             `Freddi` arguments
 
         Returns
         -------
         Freddi
 
         """
-        from collections.abc import Mapping
-        from functools import singledispatch
-        
         from astropy.units import Quantity
 
-        @singledispatch
-        def convert(value):
-            return value
-
-        @convert.register(Quantity)
-        def _(value):
-            return value.cgs.value
-
-        @convert.register(Mapping)
-        def _(value):
-            return {k: convert(v) for k, v in value.items()}
-
-        kwargs = {key: convert(value) for key, value in kwargs.items()}
-        
+        for item, value in kwargs.items():
+            if isinstance(value, Quantity):
+                kwargs[item] = value.cgs.value
+                continue
+            if isinstance(value, str):
+                kwargs[item] = value.encode()
         return cls(**kwargs)
 
-    @classmethod
-    def alt(cls, **kwargs):
-        """Alias to .from_astropy()"""
-        return cls.from_astropy(**kwargs)
-
     def evolve(self):
         """Calculate disk evolution
 
         Returns
         -------
         EvolutionResults
 
@@ -105,28 +89,28 @@
         return self._freddi._flux_hot(lmbd)
 
     def _flux_cold(self, lmbd, phase):
         del phase
         return self._freddi._flux_cold(lmbd)
 
     def _flux_star(self, lmbd, phase):
-        if phase is None:
-            raise ValueError('Phase must be specified if star flux is required')
         return self._freddi._flux_star(lmbd, phase)
 
     def flux(self, lmbd, region='hot', phase=None):
         region = region.lower()
         if 'hot'.startswith(region):
             flux = self._flux_hot
         elif 'cold'.startswith(region):
             flux = self._flux_cold
         elif 'disk'.startswith(region):
             def flux(lmbd, phase):
                 return self._flux_hot(lmbd, phase) + self._flux_cold(lmbd, phase)
         elif 'star'.startswith(region):
+            if phase is None:
+                raise ValueError('Phase must be specified if star flux is required')
             flux = self._flux_star
         elif 'all'.startswith(region):
             def flux(lmbd, phase):
                 return self._flux_hot(lmbd, phase) + self._flux_cold(lmbd, phase) + self._flux_star(lmbd, phase)
         else:
             raise ValueError(f'Zone {region} is not supported')
 
@@ -144,10 +128,7 @@
 
 class Freddi(_BasePyFreddi, metaclass=_MetaFreddi, boost_cls=_Freddi):
     pass
 
 
 class FreddiNeutronStar(_BasePyFreddi, metaclass=_MetaFreddi, boost_cls=_FreddiNeutronStar):
     pass
-
-
-__all__ = ('Freddi', 'FreddiNeutronStar')
```

### Comparing `freddi-2.0.0b2/python/freddi/evolution_result.py` & `freddi-2.0b0/python/freddi/evolution_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if isinstance(phase, Iterable):
             phase = np.asarray(phase)
             if phase.shape != (self.__len_states, ):
                 raise ValueError('phase length should be {}'.format(self.__len_states))
         else:
             phase = [phase] * self.__len_states
         lmbd = np.asarray(lmbd)
-        arr = np.empty((self.__len_states,) + lmbd.shape, dtype=float)
+        arr = np.empty((self.__len_states,) + lmbd.shape, dtype=np.float)
         for i in range(self.__len_states):
             arr[i] = self.__states[i].flux(lmbd, region, phase[i])
         return arr
 
     def __getattr__(self, attr) -> np.ndarray:
         first_val = np.asarray(getattr(self.__states[0], attr))
         if first_val.ndim == 0:
```

