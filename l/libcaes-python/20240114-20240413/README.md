# Comparing `tmp/libcaes-python-20240114.tar.gz` & `tmp/libcaes-python-20240413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcaes-python-20240114.tar", last modified: Sun Jan 14 19:41:42 2024, max compression
+gzip compressed data, was "libcaes-python-20240413.tar", last modified: Sat Apr 13 12:54:28 2024, max compression
```

## Comparing `libcaes-python-20240114.tar` & `libcaes-python-20240413.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-14 19:36:04.000000 libcaes-20240114/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-14 19:38:35.000000 libcaes-20240114/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:36:04.000000 libcaes-20240114/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-14 19:38:35.000000 libcaes-20240114/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1817 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_tweaked_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-01-14 19:38:42.000000 libcaes-20240114/libcaes/libcaes_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-01-14 19:38:42.000000 libcaes-20240114/libcaes/libcaes.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      980 2023-12-03 08:57:53.000000 libcaes-20240114/libcaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25734 2024-01-14 19:38:35.000000 libcaes-20240114/libcaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes/libcaes_tweaked_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 08:57:53.000000 libcaes-20240114/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 08:57:53.000000 libcaes-20240114/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 08:57:53.000000 libcaes-20240114/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 08:57:53.000000 libcaes-20240114/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 08:57:53.000000 libcaes-20240114/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 08:57:53.000000 libcaes-20240114/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-14 19:38:33.000000 libcaes-20240114/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-14 19:38:33.000000 libcaes-20240114/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 08:57:53.000000 libcaes-20240114/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-14 19:38:33.000000 libcaes-20240114/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 08:57:53.000000 libcaes-20240114/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 08:57:54.000000 libcaes-20240114/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 08:57:53.000000 libcaes-20240114/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-14 19:38:33.000000 libcaes-20240114/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 08:57:53.000000 libcaes-20240114/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 08:57:53.000000 libcaes-20240114/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-14 19:38:33.000000 libcaes-20240114/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 08:57:53.000000 libcaes-20240114/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 08:57:53.000000 libcaes-20240114/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 08:57:54.000000 libcaes-20240114/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 08:57:53.000000 libcaes-20240114/m4/types.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6659 2024-01-14 19:38:42.000000 libcaes-20240114/include/libcaes.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/include/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1188 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2024-01-14 19:38:42.000000 libcaes-20240114/include/libcaes/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4980 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4849 2024-01-14 19:38:42.000000 libcaes-20240114/include/libcaes/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-14 19:38:42.000000 libcaes-20240114/include/libcaes/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2024-01-14 19:36:04.000000 libcaes-20240114/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6659 2024-01-14 19:36:04.000000 libcaes-20240114/include/libcaes.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21369 2024-01-14 19:38:35.000000 libcaes-20240114/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-14 19:36:04.000000 libcaes-20240114/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-14 19:36:04.000000 libcaes-20240114/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-14 19:36:04.000000 libcaes-20240114/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-14 19:36:04.000000 libcaes-20240114/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-14 19:36:04.000000 libcaes-20240114/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-14 19:36:04.000000 libcaes-20240114/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-14 19:36:04.000000 libcaes-20240114/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-14 19:36:04.000000 libcaes-20240114/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-14 19:36:04.000000 libcaes-20240114/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-01-14 19:38:42.000000 libcaes-20240114/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10484 2024-01-14 19:38:35.000000 libcaes-20240114/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11096 2024-01-14 19:38:26.000000 libcaes-20240114/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-14 19:36:04.000000 libcaes-20240114/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-14 19:36:04.000000 libcaes-20240114/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-14 19:36:04.000000 libcaes-20240114/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18417 2024-01-14 19:38:35.000000 libcaes-20240114/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1383 2023-12-03 08:57:52.000000 libcaes-20240114/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 08:57:52.000000 libcaes-20240114/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-14 19:38:35.000000 libcaes-20240114/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/libcaes-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/libcaes.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-01-14 19:38:42.000000 libcaes-20240114/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-14 19:36:04.000000 libcaes-20240114/dpkg/libcaes-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-01-14 19:38:42.000000 libcaes-20240114/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-14 19:36:04.000000 libcaes-20240114/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   921448 2024-01-14 19:38:34.000000 libcaes-20240114/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-14 19:38:35.000000 libcaes-20240114/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-14 19:38:35.000000 libcaes-20240114/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_crypt_ccm/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/caes_test_crypt_ccm/caes_test_crypt_ccm.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/libcaes/libcaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4626 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/caes_test_support/caes_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4869 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/caes_test_context/caes_test_context.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7249 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/libcaes.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4620 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/caes_test_error/caes_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_crypt_cbc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/caes_test_crypt_cbc/caes_test_crypt_cbc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/pycaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5513 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/pycaes/pycaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_crypt_xts/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-01-14 19:36:27.000000 libcaes-20240114/msvscpp/caes_test_crypt_xts/caes_test_crypt_xts.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15951 2024-01-14 19:38:35.000000 libcaes-20240114/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/caes_test_tweaked_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4893 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/caes_test_tweaked_context/caes_test_tweaked_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-14 19:36:06.000000 libcaes-20240114/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      200 2024-01-14 19:36:04.000000 libcaes-20240114/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      295 2024-01-14 19:36:04.000000 libcaes-20240114/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-14 19:38:35.000000 libcaes-20240114/INSTALL
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-14 19:36:04.000000 libcaes-20240114/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-01-14 19:36:04.000000 libcaes-20240114/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-14 19:38:35.000000 libcaes-20240114/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-14 19:36:04.000000 libcaes-20240114/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-01-14 19:36:04.000000 libcaes-20240114/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1972 2024-01-14 19:38:42.000000 libcaes-20240114/libcaes.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 08:57:52.000000 libcaes-20240114/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/pycaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_crypt_modes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7401 2024-01-14 19:36:38.000000 libcaes-20240114/pycaes/pycaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_crypt_modes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      735 2023-12-03 08:58:14.000000 libcaes-20240114/pycaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_crypt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8945 2024-01-14 19:36:38.000000 libcaes-20240114/pycaes/pycaes_tweaked_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-14 19:36:38.000000 libcaes-20240114/pycaes/pycaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6287 2024-01-14 19:36:38.000000 libcaes-20240114/pycaes/pycaes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21284 2024-01-14 19:36:04.000000 libcaes-20240114/pycaes/pycaes_crypt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33239 2024-01-14 19:38:35.000000 libcaes-20240114/pycaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2024-01-14 19:36:38.000000 libcaes-20240114/pycaes/pycaes_tweaked_context.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-14 19:38:35.000000 libcaes-20240114/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      719 2023-12-03 08:57:52.000000 libcaes-20240114/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3172 2024-01-14 19:36:04.000000 libcaes-20240114/manuals/libcaes.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      126 2023-12-03 08:57:53.000000 libcaes-20240114/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18621 2024-01-14 19:38:35.000000 libcaes-20240114/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  1216152 2024-01-14 19:36:27.000000 libcaes-20240114/tests/caes_test_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6243 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_crypt_ccm.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3434 2024-01-14 19:36:04.000000 libcaes-20240114/tests/pycaes_test_crypt_ccm.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28105 2024-01-14 19:36:27.000000 libcaes-20240114/tests/caes_test_tweaked_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-14 19:36:04.000000 libcaes-20240114/tests/pycaes_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2024-01-14 19:36:27.000000 libcaes-20240114/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_memory.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-14 19:36:04.000000 libcaes-20240114/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   175372 2024-01-14 19:36:04.000000 libcaes-20240114/tests/pycaes_test_crypt_cbc.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3815 2024-01-14 19:36:04.000000 libcaes-20240114/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   271703 2024-01-14 19:36:04.000000 libcaes-20240114/tests/pycaes_test_crypt_xts.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-14 19:36:04.000000 libcaes-20240114/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   177604 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_crypt_cbc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   268872 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_crypt_xts.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   174565 2024-01-14 19:36:04.000000 libcaes-20240114/tests/pycaes_test_crypt_ecb.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42102 2024-01-14 19:38:35.000000 libcaes-20240114/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-01-14 19:36:04.000000 libcaes-20240114/tests/caes_test_support.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4075 2024-01-14 19:36:04.000000 libcaes-20240114/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2024-01-14 19:36:04.000000 libcaes-20240114/ossfuzz/crypt_ecb_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2024-01-14 19:36:04.000000 libcaes-20240114/ossfuzz/crypt_xts_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1891 2024-01-14 19:36:04.000000 libcaes-20240114/ossfuzz/crypt_cbc_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2023-12-03 08:57:54.000000 libcaes-20240114/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1792 2024-01-14 19:36:04.000000 libcaes-20240114/ossfuzz/crypt_ccm_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-01-14 19:36:04.000000 libcaes-20240114/ossfuzz/ossfuzz_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29060 2024-01-14 19:38:35.000000 libcaes-20240114/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-14 19:38:33.000000 libcaes-20240114/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:41.000000 libcaes-20240114/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 08:57:54.000000 libcaes-20240114/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 08:57:54.000000 libcaes-20240114/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 08:57:54.000000 libcaes-20240114/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 08:57:54.000000 libcaes-20240114/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 08:57:54.000000 libcaes-20240114/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 08:57:54.000000 libcaes-20240114/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 08:57:54.000000 libcaes-20240114/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 08:57:54.000000 libcaes-20240114/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 08:57:54.000000 libcaes-20240114/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-14 19:38:42.000000 libcaes-20240114/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 08:57:54.000000 libcaes-20240114/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 08:57:54.000000 libcaes-20240114/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33552 2024-01-14 19:38:35.000000 libcaes-20240114/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:41:40.000000 libcaes-20240114/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-14 19:38:30.000000 libcaes-20240114/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22809 2024-01-14 19:38:35.000000 libcaes-20240114/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      304 2024-01-14 19:36:04.000000 libcaes-20240114/libcaes.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56413 2024-01-14 19:38:34.000000 libcaes-20240114/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-14 19:36:04.000000 libcaes-20240114/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-01-14 19:41:42.141732 libcaes-20240114/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-13 12:14:01.000000 libcaes-20240413/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-13 12:50:31.000000 libcaes-20240413/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:14:01.000000 libcaes-20240413/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-13 12:50:31.000000 libcaes-20240413/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1817 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_tweaked_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-04-13 12:50:45.000000 libcaes-20240413/libcaes/libcaes_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-04-13 12:50:45.000000 libcaes-20240413/libcaes/libcaes.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      990 2024-04-13 12:28:37.000000 libcaes-20240413/libcaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25972 2024-04-13 12:50:31.000000 libcaes-20240413/libcaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-04-13 12:14:02.000000 libcaes-20240413/libcaes/libcaes_tweaked_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2024-04-13 12:14:01.000000 libcaes-20240413/libcaes.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 08:57:53.000000 libcaes-20240413/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 08:57:53.000000 libcaes-20240413/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 08:57:53.000000 libcaes-20240413/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 08:57:53.000000 libcaes-20240413/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 08:57:53.000000 libcaes-20240413/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-28 04:50:34.000000 libcaes-20240413/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-13 12:50:27.000000 libcaes-20240413/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-13 12:50:27.000000 libcaes-20240413/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 08:57:53.000000 libcaes-20240413/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-13 12:50:27.000000 libcaes-20240413/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 08:57:53.000000 libcaes-20240413/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-13 12:37:18.000000 libcaes-20240413/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 08:57:53.000000 libcaes-20240413/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-13 12:50:27.000000 libcaes-20240413/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 08:57:53.000000 libcaes-20240413/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 08:57:53.000000 libcaes-20240413/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-13 12:50:27.000000 libcaes-20240413/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 08:57:53.000000 libcaes-20240413/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 08:57:53.000000 libcaes-20240413/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-03-28 04:50:34.000000 libcaes-20240413/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 08:57:53.000000 libcaes-20240413/m4/types.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6659 2024-04-13 12:50:45.000000 libcaes-20240413/include/libcaes.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/include/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1188 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2024-04-13 12:50:45.000000 libcaes-20240413/include/libcaes/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4980 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4849 2024-04-13 12:50:45.000000 libcaes-20240413/include/libcaes/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-13 12:50:45.000000 libcaes-20240413/include/libcaes/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      388 2024-04-13 12:19:48.000000 libcaes-20240413/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6659 2024-04-13 12:14:02.000000 libcaes-20240413/include/libcaes.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21349 2024-04-13 12:50:31.000000 libcaes-20240413/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-13 12:14:02.000000 libcaes-20240413/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-13 12:14:02.000000 libcaes-20240413/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-13 12:14:02.000000 libcaes-20240413/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-13 12:14:02.000000 libcaes-20240413/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-13 12:14:02.000000 libcaes-20240413/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-13 12:14:02.000000 libcaes-20240413/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-13 12:14:02.000000 libcaes-20240413/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-13 12:30:19.000000 libcaes-20240413/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-13 12:14:02.000000 libcaes-20240413/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-13 12:50:45.000000 libcaes-20240413/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10484 2024-04-13 12:50:30.000000 libcaes-20240413/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11096 2024-04-13 12:50:08.000000 libcaes-20240413/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-13 12:14:02.000000 libcaes-20240413/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-13 12:14:02.000000 libcaes-20240413/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-13 12:14:02.000000 libcaes-20240413/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18424 2024-04-13 12:50:31.000000 libcaes-20240413/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1191 2024-04-13 12:40:51.000000 libcaes-20240413/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 08:57:52.000000 libcaes-20240413/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-13 12:50:31.000000 libcaes-20240413/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-13 12:14:03.000000 libcaes-20240413/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/libcaes-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/libcaes.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-13 12:50:45.000000 libcaes-20240413/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-13 12:14:01.000000 libcaes-20240413/dpkg/libcaes-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-04-13 12:50:45.000000 libcaes-20240413/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-13 12:14:01.000000 libcaes-20240413/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   921613 2024-04-13 12:50:30.000000 libcaes-20240413/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-13 12:50:31.000000 libcaes-20240413/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-13 12:50:31.000000 libcaes-20240413/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_crypt_ccm/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-04-13 12:14:58.000000 libcaes-20240413/msvscpp/caes_test_crypt_ccm/caes_test_crypt_ccm.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/libcaes/libcaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4626 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/caes_test_support/caes_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4869 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/caes_test_context/caes_test_context.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      537 2024-04-13 12:22:39.000000 libcaes-20240413/msvscpp/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7249 2024-04-13 12:14:58.000000 libcaes-20240413/msvscpp/libcaes.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4620 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/caes_test_error/caes_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_crypt_cbc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-04-13 12:14:58.000000 libcaes-20240413/msvscpp/caes_test_crypt_cbc/caes_test_crypt_cbc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/pycaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5513 2024-04-13 12:14:58.000000 libcaes-20240413/msvscpp/pycaes/pycaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_crypt_xts/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-04-13 12:14:58.000000 libcaes-20240413/msvscpp/caes_test_crypt_xts/caes_test_crypt_xts.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15951 2024-04-13 12:50:31.000000 libcaes-20240413/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/caes_test_tweaked_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4893 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/caes_test_tweaked_context/caes_test_tweaked_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-13 12:14:05.000000 libcaes-20240413/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      200 2024-04-13 12:14:02.000000 libcaes-20240413/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      295 2024-04-13 12:14:01.000000 libcaes-20240413/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-13 12:50:31.000000 libcaes-20240413/INSTALL
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-13 12:14:01.000000 libcaes-20240413/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-13 12:14:01.000000 libcaes-20240413/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-13 12:50:31.000000 libcaes-20240413/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-13 12:14:01.000000 libcaes-20240413/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-04-13 12:14:58.000000 libcaes-20240413/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1972 2024-04-13 12:50:45.000000 libcaes-20240413/libcaes.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 08:57:52.000000 libcaes-20240413/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/pycaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_crypt_modes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7401 2024-04-13 12:14:58.000000 libcaes-20240413/pycaes/pycaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_crypt_modes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      731 2024-04-13 12:30:28.000000 libcaes-20240413/pycaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_crypt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8945 2024-04-13 12:14:58.000000 libcaes-20240413/pycaes/pycaes_tweaked_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-13 12:14:58.000000 libcaes-20240413/pycaes/pycaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6287 2024-04-13 12:14:58.000000 libcaes-20240413/pycaes/pycaes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21284 2024-04-13 12:14:02.000000 libcaes-20240413/pycaes/pycaes_crypt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33559 2024-04-13 12:50:31.000000 libcaes-20240413/pycaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2024-04-13 12:14:58.000000 libcaes-20240413/pycaes/pycaes_tweaked_context.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-13 12:50:31.000000 libcaes-20240413/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      719 2023-12-03 08:57:52.000000 libcaes-20240413/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3172 2024-04-13 12:14:03.000000 libcaes-20240413/manuals/libcaes.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-13 12:23:47.000000 libcaes-20240413/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18621 2024-04-13 12:50:31.000000 libcaes-20240413/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  1216152 2024-04-13 12:15:43.000000 libcaes-20240413/tests/caes_test_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6243 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_crypt_ccm.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3434 2024-04-13 12:14:03.000000 libcaes-20240413/tests/pycaes_test_crypt_ccm.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28105 2024-04-13 12:15:43.000000 libcaes-20240413/tests/caes_test_tweaked_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-13 12:14:03.000000 libcaes-20240413/tests/pycaes_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2256 2024-04-13 12:30:36.000000 libcaes-20240413/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_memory.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-13 12:39:44.000000 libcaes-20240413/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   175372 2024-04-13 12:14:03.000000 libcaes-20240413/tests/pycaes_test_crypt_cbc.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3784 2024-04-13 12:39:55.000000 libcaes-20240413/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   271703 2024-04-13 12:14:03.000000 libcaes-20240413/tests/pycaes_test_crypt_xts.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-13 12:14:03.000000 libcaes-20240413/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   177604 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_crypt_cbc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   268872 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_crypt_xts.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   174565 2024-04-13 12:14:03.000000 libcaes-20240413/tests/pycaes_test_crypt_ecb.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42491 2024-04-13 12:50:31.000000 libcaes-20240413/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-13 12:14:03.000000 libcaes-20240413/tests/caes_test_support.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4044 2024-04-13 12:39:31.000000 libcaes-20240413/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2024-04-13 12:14:02.000000 libcaes-20240413/ossfuzz/crypt_ecb_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2024-04-13 12:14:02.000000 libcaes-20240413/ossfuzz/crypt_xts_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1891 2024-04-13 12:14:02.000000 libcaes-20240413/ossfuzz/crypt_cbc_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1494 2024-04-13 12:30:45.000000 libcaes-20240413/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1792 2024-04-13 12:14:02.000000 libcaes-20240413/ossfuzz/crypt_ccm_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-13 12:14:02.000000 libcaes-20240413/ossfuzz/ossfuzz_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29246 2024-04-13 12:50:31.000000 libcaes-20240413/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-13 12:50:27.000000 libcaes-20240413/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:27.000000 libcaes-20240413/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 08:57:54.000000 libcaes-20240413/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 08:57:54.000000 libcaes-20240413/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 08:57:54.000000 libcaes-20240413/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 08:57:54.000000 libcaes-20240413/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 08:57:54.000000 libcaes-20240413/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 08:57:54.000000 libcaes-20240413/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 08:57:54.000000 libcaes-20240413/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 08:57:54.000000 libcaes-20240413/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 08:57:54.000000 libcaes-20240413/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-13 12:50:45.000000 libcaes-20240413/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 08:57:54.000000 libcaes-20240413/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 08:57:54.000000 libcaes-20240413/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33434 2024-04-13 12:50:31.000000 libcaes-20240413/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-13 12:54:26.000000 libcaes-20240413/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      663 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-13 12:50:23.000000 libcaes-20240413/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22985 2024-04-13 12:50:31.000000 libcaes-20240413/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      304 2024-04-13 12:14:01.000000 libcaes-20240413/libcaes.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56413 2024-04-13 12:50:29.000000 libcaes-20240413/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-13 12:14:01.000000 libcaes-20240413/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-04-13 12:54:28.717589 libcaes-20240413/PKG-INFO
```

### Comparing `libcaes-20240114/COPYING` & `libcaes-20240413/COPYING`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/install-sh` & `libcaes-20240413/install-sh`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/depcomp` & `libcaes-20240413/depcomp`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_unused.h` & `libcaes-20240413/libcaes/libcaes_unused.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes.c` & `libcaes-20240413/libcaes/libcaes.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_tweaked_context.h` & `libcaes-20240413/libcaes/libcaes_tweaked_context.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_context.h` & `libcaes-20240413/libcaes/libcaes_context.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_error.c` & `libcaes-20240413/libcaes/libcaes_error.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_context.c` & `libcaes-20240413/libcaes/libcaes_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_definitions.h` & `libcaes-20240413/libcaes/libcaes_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBCAES )
 #include <libcaes/definitions.h>
 
 /* The definitions in <libcaes/definitions.h> are copied here
  * for local use of libcaes
  */
 #else
-#define LIBCAES_VERSION				20240114
+#define LIBCAES_VERSION				20240413
 
 /* The libcaes version string
  */
-#define LIBCAES_VERSION_STRING			"20240114"
+#define LIBCAES_VERSION_STRING			"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT		= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libcaes-20240114/libcaes/libcaes.rc` & `libcaes-20240413/libcaes/libcaes.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support cross-platform AES encryption\0"
-      VALUE "FileVersion",		"20240114" "\0"
+      VALUE "FileVersion",		"20240413" "\0"
       VALUE "InternalName",		"libcaes.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libcaes.dll\0"
       VALUE "ProductName",		"libcaes\0"
-      VALUE "ProductVersion",		"20240114" "\0"
+      VALUE "ProductVersion",		"20240413" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libcaes/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libcaes-20240114/libcaes/Makefile.am` & `libcaes-20240413/libcaes/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ \
 	@LIBCAES_DLL_EXPORT@
 
 lib_LTLIBRARIES = libcaes.la
 
 libcaes_la_SOURCES = \
 	libcaes.c \
 	libcaes_context.c libcaes_context.h \
@@ -26,21 +27,19 @@
 libcaes_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libcaes_definitions.h.in \
 	libcaes.rc \
 	libcaes.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libcaes_definitions.h \
+	libcaes.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libcaes_definitions.h
-	-rm -f libcaes.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
```

### Comparing `libcaes-20240114/libcaes/libcaes_definitions.h.in` & `libcaes-20240413/libcaes/libcaes_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_error.h` & `libcaes-20240413/libcaes/libcaes_error.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_types.h` & `libcaes-20240413/libcaes/libcaes_types.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_extern.h` & `libcaes-20240413/libcaes/libcaes_extern.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_support.h` & `libcaes-20240413/libcaes/libcaes_support.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes.rc.in` & `libcaes-20240413/libcaes/libcaes.rc.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_libcerror.h` & `libcaes-20240413/libcaes/libcaes_libcerror.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/libcaes_support.c` & `libcaes-20240413/libcaes/libcaes_support.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes/Makefile.in` & `libcaes-20240413/libcaes/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -406,17 +406,18 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ \
 	@LIBCAES_DLL_EXPORT@
 
 lib_LTLIBRARIES = libcaes.la
 libcaes_la_SOURCES = \
 	libcaes.c \
 	libcaes_context.c libcaes_context.h \
 	libcaes_definitions.h \
@@ -435,15 +436,18 @@
 
 libcaes_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libcaes_definitions.h.in \
 	libcaes.rc \
 	libcaes.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libcaes_definitions.h \
+	libcaes.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -678,24 +682,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcaes.Plo
+	-rm -f ./$(DEPDIR)/libcaes_context.Plo
+	-rm -f ./$(DEPDIR)/libcaes_error.Plo
+	-rm -f ./$(DEPDIR)/libcaes_support.Plo
+	-rm -f ./$(DEPDIR)/libcaes_tweaked_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -783,19 +794,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libcaes_definitions.h
-	-rm -f libcaes.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libcaes-20240114/libcaes/libcaes_tweaked_context.c` & `libcaes-20240413/libcaes/libcaes_tweaked_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes.spec.in` & `libcaes-20240413/libcaes.spec.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/tests.m4` & `libcaes-20240413/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/lib-prefix.m4` & `libcaes-20240413/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/progtest.m4` & `libcaes-20240413/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/gettext.m4` & `libcaes-20240413/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/lib-ld.m4` & `libcaes-20240413/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/common.m4` & `libcaes-20240413/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libcaes-20240114/m4/ltversion.m4` & `libcaes-20240413/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/ltsugar.m4` & `libcaes-20240413/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/host-cpu-c-abi.m4` & `libcaes-20240413/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/libtool.m4` & `libcaes-20240413/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/po.m4` & `libcaes-20240413/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/libcerror.m4` & `libcaes-20240413/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libcaes-20240114/m4/intlmacosx.m4` & `libcaes-20240413/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/lt~obsolete.m4` & `libcaes-20240413/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/lib-link.m4` & `libcaes-20240413/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/iconv.m4` & `libcaes-20240413/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/ltoptions.m4` & `libcaes-20240413/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/nls.m4` & `libcaes-20240413/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/python.m4` & `libcaes-20240413/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/m4/libcrypto.m4` & `libcaes-20240413/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libcaes-20240114/m4/types.m4` & `libcaes-20240413/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes.h` & `libcaes-20240413/include/libcaes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/definitions.h.in` & `libcaes-20240413/include/libcaes/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/definitions.h` & `libcaes-20240413/include/libcaes/definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBCAES_DEFINITIONS_H )
 #define _LIBCAES_DEFINITIONS_H
 
 #include <libcaes/types.h>
 
-#define LIBCAES_VERSION			20240114
+#define LIBCAES_VERSION			20240413
 
 /* The version string
  */
-#define LIBCAES_VERSION_STRING		"20240114"
+#define LIBCAES_VERSION_STRING		"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT	= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT	= 1
```

### Comparing `libcaes-20240114/include/libcaes/types.h.in` & `libcaes-20240413/include/libcaes/types.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/types.h` & `libcaes-20240413/include/libcaes/types.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/features.h.in` & `libcaes-20240413/include/libcaes/features.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/error.h` & `libcaes-20240413/include/libcaes/error.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/extern.h` & `libcaes-20240413/include/libcaes/extern.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes/features.h` & `libcaes-20240413/include/libcaes/features.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/libcaes.h.in` & `libcaes-20240413/include/libcaes.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/include/Makefile.in` & `libcaes-20240413/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -385,15 +385,20 @@
 
 EXTRA_DIST = \
 	libcaes.h.in \
 	libcaes/definitions.h.in \
 	libcaes/features.h.in \
 	libcaes/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libcaes.h \
+	libcaes/definitions.h \
+	libcaes/features.h \
+	libcaes/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -590,23 +595,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -688,17 +695,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libcaes.h
-	-rm -f libcaes/definitions.h
-	-rm -f libcaes/features.h
-	-rm -f libcaes/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/common/config_borlandc.h` & `libcaes-20240413/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/file_stream.h` & `libcaes-20240413/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/memory.h` & `libcaes-20240413/common/memory.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/byte_stream.h` & `libcaes-20240413/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/common.h` & `libcaes-20240413/common/common.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/config_winapi.h` & `libcaes-20240413/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/system_string.h` & `libcaes-20240413/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/types.h.in` & `libcaes-20240413/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/types.h` & `libcaes-20240413/common/types.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/config.h.in` & `libcaes-20240413/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/config.h` & `libcaes-20240413/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -322,24 +322,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libcaes"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libcaes 20240114"
+#define PACKAGE_STRING "libcaes 20240413"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libcaes"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240114"
+#define PACKAGE_VERSION "20240413"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -357,15 +357,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240114"
+#define VERSION "20240413"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libcaes-20240114/common/wide_string.h` & `libcaes-20240413/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/narrow_string.h` & `libcaes-20240413/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/config_msc.h` & `libcaes-20240413/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/common/Makefile.in` & `libcaes-20240413/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -355,15 +357,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -531,23 +536,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -627,15 +634,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/config.guess` & `libcaes-20240413/config.guess`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/dpkg/copyright` & `libcaes-20240413/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/dpkg/control` & `libcaes-20240413/dpkg/control`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/dpkg/rules` & `libcaes-20240413/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/COPYING.LESSER` & `libcaes-20240413/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/configure` & `libcaes-20240413/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libcaes 20240114.
+# Generated by GNU Autoconf 2.71 for libcaes 20240413.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libcaes'
 PACKAGE_TARNAME='libcaes'
-PACKAGE_VERSION='20240114'
-PACKAGE_STRING='libcaes 20240114'
+PACKAGE_VERSION='20240413'
+PACKAGE_STRING='libcaes 20240413'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libcaes.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1459,15 +1459,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libcaes 20240114 to adapt to many kinds of systems.
+\`configure' configures libcaes 20240413 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1530,15 +1530,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libcaes 20240114:";;
+     short | recursive ) echo "Configuration of libcaes 20240413:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1684,15 +1684,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libcaes configure 20240114
+libcaes configure 20240413
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2405,15 +2405,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libcaes $as_me 20240114, which was
+It was created by libcaes $as_me 20240413, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -3894,15 +3894,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libcaes'
- VERSION='20240114'
+ VERSION='20240413'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23373,15 +23373,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -23872,15 +23872,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24022,15 +24023,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24141,15 +24142,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -28125,15 +28126,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libcaes $as_me 20240114, which was
+This file was extended by libcaes $as_me 20240413, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -28193,15 +28194,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libcaes config.status 20240114
+libcaes config.status 20240413
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libcaes-20240114/compile` & `libcaes-20240413/compile`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/missing` & `libcaes-20240413/missing`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_crypt_ccm/caes_test_crypt_ccm.vcproj` & `libcaes-20240413/msvscpp/caes_test_crypt_ccm/caes_test_crypt_ccm.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/libcaes/libcaes.vcproj` & `libcaes-20240413/msvscpp/libcaes/libcaes.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_support/caes_test_support.vcproj` & `libcaes-20240413/msvscpp/caes_test_support/caes_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_context/caes_test_context.vcproj` & `libcaes-20240413/msvscpp/caes_test_context/caes_test_context.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/Makefile.am` & `libcaes-20240413/msvscpp/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -10,13 +10,11 @@
 	libcerror/libcerror.vcproj \
 	pycaes/pycaes.vcproj \
 	libcaes.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libcaes-20240114/msvscpp/libcaes.sln` & `libcaes-20240413/msvscpp/libcaes.sln`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_error/caes_test_error.vcproj` & `libcaes-20240413/msvscpp/caes_test_error/caes_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_crypt_cbc/caes_test_crypt_cbc.vcproj` & `libcaes-20240413/msvscpp/caes_test_crypt_cbc/caes_test_crypt_cbc.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/pycaes/pycaes.vcproj` & `libcaes-20240413/msvscpp/pycaes/pycaes.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/caes_test_crypt_xts/caes_test_crypt_xts.vcproj` & `libcaes-20240413/msvscpp/caes_test_crypt_xts/caes_test_crypt_xts.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/Makefile.in` & `libcaes-20240413/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,16 @@
 	libcerror/libcerror.vcproj \
 	pycaes/pycaes.vcproj \
 	libcaes.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -449,23 +450,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -544,13 +547,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/msvscpp/caes_test_tweaked_context/caes_test_tweaked_context.vcproj` & `libcaes-20240413/msvscpp/caes_test_tweaked_context/caes_test_tweaked_context.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/msvscpp/libcerror/libcerror.vcproj` & `libcaes-20240413/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/INSTALL` & `libcaes-20240413/INSTALL`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/config.sub` & `libcaes-20240413/config.sub`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/setup.py` & `libcaes-20240413/setup.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/acinclude.m4` & `libcaes-20240413/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcaes.spec` & `libcaes-20240413/libcaes.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libcaes
-Version: 20240114
+Version: 20240413
 Release: 1
 Summary: Library to support cross-platform AES encryption
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libcaes
 Requires:  openssl
@@ -76,10 +76,10 @@
 %files -n libcaes-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Sun Jan 14 2024 Joachim Metz <joachim.metz@gmail.com> 20240114-1
+* Sat Apr 13 2024 Joachim Metz <joachim.metz@gmail.com> 20240413-1
 - Auto-generated
```

### Comparing `libcaes-20240114/config.rpath` & `libcaes-20240413/config.rpath`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_crypt_modes.h` & `libcaes-20240413/pycaes/pycaes_crypt_modes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_python.h` & `libcaes-20240413/pycaes/pycaes_python.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_unused.h` & `libcaes-20240413/pycaes/pycaes_unused.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_context.c` & `libcaes-20240413/pycaes/pycaes_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_libcerror.h` & `libcaes-20240413/pycaes/pycaes_libcerror.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_crypt_modes.c` & `libcaes-20240413/pycaes/pycaes_crypt_modes.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_error.h` & `libcaes-20240413/pycaes/pycaes_error.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_crypt.h` & `libcaes-20240413/pycaes/pycaes_crypt.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_tweaked_context.c` & `libcaes-20240413/pycaes/pycaes_tweaked_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes.h` & `libcaes-20240413/pycaes/pycaes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_error.c` & `libcaes-20240413/pycaes/pycaes_error.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_context.h` & `libcaes-20240413/pycaes/pycaes_context.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes.c` & `libcaes-20240413/pycaes/pycaes.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_libcaes.h` & `libcaes-20240413/pycaes/pycaes_libcaes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/pycaes_crypt.c` & `libcaes-20240413/pycaes/pycaes_crypt.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/pycaes/Makefile.in` & `libcaes-20240413/pycaes/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -418,16 +418,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCAES_DLL_IMPORT@
 
 @HAVE_PYTHON_TRUE@pyexec_LTLIBRARIES = pycaes.la
 @HAVE_PYTHON_TRUE@pycaes_la_SOURCES = \
 @HAVE_PYTHON_TRUE@	pycaes.c pycaes.h \
 @HAVE_PYTHON_TRUE@	pycaes_context.c pycaes_context.h \
@@ -442,15 +442,16 @@
 
 @HAVE_PYTHON_TRUE@pycaes_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libcaes/libcaes.la
 
 @HAVE_PYTHON_TRUE@pycaes_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pycaes_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -724,24 +725,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pycaes_la-pycaes.Plo
+	-rm -f ./$(DEPDIR)/pycaes_la-pycaes_context.Plo
+	-rm -f ./$(DEPDIR)/pycaes_la-pycaes_crypt.Plo
+	-rm -f ./$(DEPDIR)/pycaes_la-pycaes_crypt_modes.Plo
+	-rm -f ./$(DEPDIR)/pycaes_la-pycaes_error.Plo
+	-rm -f ./$(DEPDIR)/pycaes_la-pycaes_tweaked_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -831,13 +840,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/pycaes/pycaes_tweaked_context.h` & `libcaes-20240413/pycaes/pycaes_tweaked_context.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/test-driver` & `libcaes-20240413/test-driver`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ChangeLog` & `libcaes-20240413/ChangeLog`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/manuals/libcaes.3` & `libcaes-20240413/manuals/libcaes.3`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/manuals/Makefile.in` & `libcaes-20240413/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libcaes.3
 
 EXTRA_DIST = \
 	libcaes.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -516,23 +517,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -613,13 +616,10 @@
 	mostlyclean mostlyclean-generic mostlyclean-libtool pdf pdf-am \
 	ps ps-am sources-am sources-local splint-am splint-local \
 	tags-am uninstall uninstall-am uninstall-man uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/tests/caes_test_context.c` & `libcaes-20240413/tests/caes_test_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_crypt_ccm.c` & `libcaes-20240413/tests/caes_test_crypt_ccm.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/pycaes_test_crypt_ccm.py` & `libcaes-20240413/tests/pycaes_test_crypt_ccm.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_error.c` & `libcaes-20240413/tests/caes_test_error.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_tweaked_context.c` & `libcaes-20240413/tests/caes_test_tweaked_context.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/pycaes_test_support.py` & `libcaes-20240413/tests/pycaes_test_support.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_unused.h` & `libcaes-20240413/tests/caes_test_unused.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_macros.h` & `libcaes-20240413/tests/caes_test_macros.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/Makefile.am` & `libcaes-20240413/tests/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ \
 	@LIBCAES_DLL_IMPORT@
 
 if HAVE_PYTHON_TESTS
 TESTS_PYCAES = \
 	test_python_module.sh
 endif
 
@@ -104,13 +105,11 @@
 	caes_test_tweaked_context.c \
 	caes_test_unused.h
 
 caes_test_tweaked_context_LDADD = \
 	../libcaes/libcaes.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libcaes-20240114/tests/caes_test_memory.h` & `libcaes-20240413/tests/caes_test_memory.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_memory.c` & `libcaes-20240413/tests/caes_test_memory.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/pycaes_test_crypt_cbc.py` & `libcaes-20240413/tests/pycaes_test_crypt_cbc.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/test_python_module.sh` & `libcaes-20240413/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="";
@@ -120,20 +120,17 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libcaes-20240114/tests/caes_test_libcaes.h` & `libcaes-20240413/tests/caes_test_libcaes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/pycaes_test_crypt_xts.py` & `libcaes-20240413/tests/pycaes_test_crypt_xts.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/test_runner.sh` & `libcaes-20240413/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_libcerror.h` & `libcaes-20240413/tests/caes_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_crypt_cbc.c` & `libcaes-20240413/tests/caes_test_crypt_cbc.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/caes_test_crypt_xts.c` & `libcaes-20240413/tests/caes_test_crypt_xts.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/pycaes_test_crypt_ecb.py` & `libcaes-20240413/tests/pycaes_test_crypt_ecb.py`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/Makefile.in` & `libcaes-20240413/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -612,17 +612,18 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ \
 	@LIBCAES_DLL_IMPORT@
 
 @HAVE_PYTHON_TESTS_TRUE@TESTS_PYCAES = \
 @HAVE_PYTHON_TESTS_TRUE@	test_python_module.sh
 
 TESTS = \
 	test_library.sh \
@@ -710,15 +711,16 @@
 	caes_test_tweaked_context.c \
 	caes_test_unused.h
 
 caes_test_tweaked_context_LDADD = \
 	../libcaes/libcaes.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1123,24 +1125,34 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/caes_test_context.Po
+	-rm -f ./$(DEPDIR)/caes_test_crypt_cbc.Po
+	-rm -f ./$(DEPDIR)/caes_test_crypt_ccm.Po
+	-rm -f ./$(DEPDIR)/caes_test_crypt_xts.Po
+	-rm -f ./$(DEPDIR)/caes_test_error.Po
+	-rm -f ./$(DEPDIR)/caes_test_memory.Po
+	-rm -f ./$(DEPDIR)/caes_test_support.Po
+	-rm -f ./$(DEPDIR)/caes_test_tweaked_context.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1231,13 +1243,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/tests/caes_test_support.c` & `libcaes-20240413/tests/caes_test_support.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/tests/test_library.sh` & `libcaes-20240413/tests/test_library.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="context error support tweaked_context";
 LIBRARY_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libcaes-20240114/ossfuzz/crypt_ecb_fuzzer.cc` & `libcaes-20240413/ossfuzz/crypt_ecb_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ossfuzz/crypt_xts_fuzzer.cc` & `libcaes-20240413/ossfuzz/crypt_xts_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ossfuzz/crypt_cbc_fuzzer.cc` & `libcaes-20240413/ossfuzz/crypt_cbc_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ossfuzz/Makefile.am` & `libcaes-20240413/ossfuzz/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	crypt_cbc_fuzzer \
 	crypt_ccm_fuzzer \
 	crypt_ecb_fuzzer \
 	crypt_xts_fuzzer
 
@@ -38,20 +38,18 @@
 	ossfuzz_libcaes.h
 
 crypt_xts_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libcaes/libcaes.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on crypt_cbc_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_cbc_fuzzer_SOURCES)
 	@echo "Running splint on crypt_ccm_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_ccm_fuzzer_SOURCES)
 	@echo "Running splint on crypt_ecb_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_ecb_fuzzer_SOURCES)
```

### Comparing `libcaes-20240114/ossfuzz/crypt_ccm_fuzzer.cc` & `libcaes-20240413/ossfuzz/crypt_ccm_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ossfuzz/ossfuzz_libcaes.h` & `libcaes-20240413/ossfuzz/ossfuzz_libcaes.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/ossfuzz/Makefile.in` & `libcaes-20240413/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -426,16 +426,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_cbc_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_cbc_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libcaes.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_cbc_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -461,15 +461,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	crypt_xts_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libcaes.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@crypt_xts_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libcaes/libcaes.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -726,23 +727,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/crypt_cbc_fuzzer.Po
+	-rm -f ./$(DEPDIR)/crypt_ccm_fuzzer.Po
+	-rm -f ./$(DEPDIR)/crypt_ecb_fuzzer.Po
+	-rm -f ./$(DEPDIR)/crypt_xts_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -829,17 +836,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on crypt_cbc_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_cbc_fuzzer_SOURCES)
 	@echo "Running splint on crypt_ccm_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_ccm_fuzzer_SOURCES)
 	@echo "Running splint on crypt_ecb_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(crypt_ecb_fuzzer_SOURCES)
```

### Comparing `libcaes-20240114/ltmain.sh` & `libcaes-20240413/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/remove-potcdate.sin` & `libcaes-20240413/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/Makefile.in.in` & `libcaes-20240413/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/en@quot.header` & `libcaes-20240413/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/en@boldquot.header` & `libcaes-20240413/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/insert-header.sin` & `libcaes-20240413/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/Makevars` & `libcaes-20240413/po/Makevars`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/Makevars.in` & `libcaes-20240413/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/po/Rules-quot` & `libcaes-20240413/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/Makefile.in` & `libcaes-20240413/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -489,16 +489,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libcaes.pc \
+	libcaes.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libcaes.pc
 
 all: all-recursive
 
@@ -915,23 +922,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1029,22 +1039,10 @@
 
 library:
 	(cd $(srcdir)/common && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libcaes.pc
-	-rm -f libcaes.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libcaes-20240114/libcerror/libcerror_system.c` & `libcaes-20240413/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_error.c` & `libcaes-20240413/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_extern.h` & `libcaes-20240413/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/Makefile.am` & `libcaes-20240413/libcerror/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libcerror_definitions.h \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libcaes-20240114/libcerror/libcerror_types.h` & `libcaes-20240413/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_support.h` & `libcaes-20240413/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_error.h` & `libcaes-20240413/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_system.h` & `libcaes-20240413/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_definitions.h` & `libcaes-20240413/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libcaes-20240114/libcerror/libcerror_support.c` & `libcaes-20240413/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/libcerror_unused.h` & `libcaes-20240413/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/libcerror/Makefile.in` & `libcaes-20240413/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -380,28 +380,30 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libcerror_definitions.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -603,24 +605,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -706,17 +713,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libcaes-20240114/aclocal.m4` & `libcaes-20240413/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libcaes-20240114/configure.ac` & `libcaes-20240413/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libcaes],
- [20240114],
+ [20240413],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libcaes.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

