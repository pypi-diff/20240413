# Comparing `tmp/pnu-portstreelint-1.3.0.tar.gz` & `tmp/pnu_portstreelint-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu-portstreelint-1.3.0.tar", last modified: Mon Apr  1 17:02:27 2024, max compression
+gzip compressed data, was "pnu_portstreelint-1.4.0.tar", last modified: Sat Apr 13 16:50:02 2024, max compression
```

## Comparing `pnu-portstreelint-1.3.0.tar` & `pnu_portstreelint-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.841448 pnu-portstreelint-1.3.0/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu-portstreelint-1.3.0/License
--rw-r--r--   0 hubert    (1001) hubert    (1001)    11057 2024-04-01 17:02:27.841415 pnu-portstreelint-1.3.0/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     9822 2024-04-01 16:50:17.000000 pnu-portstreelint-1.3.0/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.836460 pnu-portstreelint-1.3.0/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     3415 2024-04-01 17:02:25.000000 pnu-portstreelint-1.3.0/man/portstreelint.8.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu-portstreelint-1.3.0/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-04-01 17:02:27.842247 pnu-portstreelint-1.3.0/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.817598 pnu-portstreelint-1.3.0/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.841129 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    11057 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1063 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/entry_points.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/requires.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/top_level.txt
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.840932 pnu-portstreelint-1.3.0/src/portstreelint/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu-portstreelint-1.3.0/src/portstreelint/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-04-01 14:27:16.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-04-01 14:27:25.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_comment.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-04-01 14:27:31.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_description_file.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-04-01 14:27:38.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_installation_prefix.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-04-01 14:27:44.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_maintainer.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-04-01 14:27:52.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_marks.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1859 2024-04-01 14:28:00.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_plist.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-04-01 14:28:06.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_port_path.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-04-01 14:28:12.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_unchanging_ports.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5597 2024-04-01 14:28:20.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_vulnerabilities.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7125 2024-04-01 14:29:09.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_www_site.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2008 2024-03-03 22:38:49.000000 pnu-portstreelint-1.3.0/src/portstreelint/library.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7540 2024-04-01 14:11:53.000000 pnu-portstreelint-1.3.0/src/portstreelint/load_config.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4914 2024-04-01 14:29:36.000000 pnu-portstreelint-1.3.0/src/portstreelint/load_data.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    15801 2024-04-01 16:28:57.000000 pnu-portstreelint-1.3.0/src/portstreelint/main.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_maintainers.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1757 2024-04-01 14:30:49.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_notifications.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3940 2024-04-01 14:30:57.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_summary.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.255304 pnu_portstreelint-1.4.0/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu_portstreelint-1.4.0/License
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 16:50:02.255269 pnu_portstreelint-1.4.0/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    10018 2024-04-13 16:32:45.000000 pnu_portstreelint-1.4.0/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.250168 pnu_portstreelint-1.4.0/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     3468 2024-04-13 16:49:59.000000 pnu_portstreelint-1.4.0/man/portstreelint.8.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu_portstreelint-1.4.0/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-04-13 16:50:02.256016 pnu_portstreelint-1.4.0/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.237448 pnu_portstreelint-1.4.0/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.255001 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1099 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/entry_points.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/requires.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.254805 pnu_portstreelint-1.4.0/src/portstreelint/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu_portstreelint-1.4.0/src/portstreelint/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-04-13 16:17:29.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-04-13 16:17:36.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_comment.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-04-13 16:17:46.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_description_file.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-04-13 16:17:54.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_installation_prefix.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4530 2024-04-13 16:46:46.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_licenses.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-04-13 16:18:12.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_maintainer.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-04-13 16:18:18.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_marks.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3096 2024-04-13 16:18:24.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_plist.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-04-13 16:18:30.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_port_path.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-04-13 16:18:35.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_unchanging_ports.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5597 2024-04-13 16:18:41.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_vulnerabilities.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7050 2024-04-13 16:18:47.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_www_site.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2147 2024-04-13 13:34:33.000000 pnu_portstreelint-1.4.0/src/portstreelint/library.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     8013 2024-04-13 16:16:47.000000 pnu_portstreelint-1.4.0/src/portstreelint/load_config.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4912 2024-04-13 16:19:07.000000 pnu_portstreelint-1.4.0/src/portstreelint/load_data.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    16028 2024-04-13 16:19:37.000000 pnu_portstreelint-1.4.0/src/portstreelint/main.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_maintainers.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1756 2024-04-13 16:19:48.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_notifications.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4314 2024-04-13 16:19:54.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_summary.py
```

### Comparing `pnu-portstreelint-1.3.0/License` & `pnu_portstreelint-1.4.0/License`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/PKG-INFO` & `pnu_portstreelint-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.3.0
+Version: 1.4.0
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
@@ -47,15 +47,15 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--nocfg|-n\]
+\[--nocfg\]
 \[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
 \[--tree|-t DIR\]
@@ -126,14 +126,18 @@
 * INDEX:www-site different from Makefile:WWW
 * Ports marked as BROKEN, DEPRECATED, FORBIDDEN, IGNORE, RESTRICTED (info)
 * Ports marked with an EXPIRATION_DATE (warning)
 * Ports marked as BROKEN, FORBIDDEN or DEPRECATED for too long (warning)
 * Ports unchanged for a long time (info)
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
+* Missing Makefile:LICENSE
+* Unofficial licenses (warning)
+* Unnecessary Makefile:LICENSE_COMB=single (warning)
+* Unnecessary Makefile:LICENSE_COMB=multi (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
 one and a number of days for the others. And you can select a port
 tree in a location other than */usr/ports* with the *--tree|-t*
@@ -143,24 +147,25 @@
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
 For convenience, you can put your favourite options in a
 configuration file, which will be read before processing the
-environment and the command line, unless you use the *--nocfg|-n*
+environment and the command line, unless you use the *--nocfg*
 option. You can generate a default configuration file with the
 *--gencfg|-g* option followed by a filename. This file also offers
 full control over the checks to perform, and a way to discard
-false-positive vulnerabilities.
+false-positive vulnerabilities and unwanted licenses report
+messages.
 
 ### OPTIONS
 Options | Use
 ------- | ---
---nocfg\|-n|Don't use the configuration file
+--nocfg|Don't use the configuration file
 --gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
 --tree\|-t DIR|Set ports directory (default=/usr/ports)
@@ -258,13 +263,13 @@
 [Hubert Tournier](https://github.com/HubTou)
 
 ## CAVEATS
 The IGNORE mark check is not reliable because this tool doesn't parse
 the ports' Makefiles, but just loads their variables without regard to
 the conditional tests that may surround them.
 
-The nonexistent plist is not very helpful because there are unaccounted
-autoplist options for some languages (Python)...
+The nonexistent plist check is not very helpful because there are still
+undocumented cases where the list is auto generated.
 
 The ports using exotic versioning schemes will be skipped from the
 vulnerability check because the library we use for version comparisons
 is geared toward Python ports and limited for this usage.
```

### Comparing `pnu-portstreelint-1.3.0/README.md` & `pnu_portstreelint-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--nocfg|-n\]
+\[--nocfg\]
 \[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
 \[--tree|-t DIR\]
@@ -94,14 +94,18 @@
 * INDEX:www-site different from Makefile:WWW
 * Ports marked as BROKEN, DEPRECATED, FORBIDDEN, IGNORE, RESTRICTED (info)
 * Ports marked with an EXPIRATION_DATE (warning)
 * Ports marked as BROKEN, FORBIDDEN or DEPRECATED for too long (warning)
 * Ports unchanged for a long time (info)
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
+* Missing Makefile:LICENSE
+* Unofficial licenses (warning)
+* Unnecessary Makefile:LICENSE_COMB=single (warning)
+* Unnecessary Makefile:LICENSE_COMB=multi (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
 one and a number of days for the others. And you can select a port
 tree in a location other than */usr/ports* with the *--tree|-t*
@@ -111,24 +115,25 @@
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
 For convenience, you can put your favourite options in a
 configuration file, which will be read before processing the
-environment and the command line, unless you use the *--nocfg|-n*
+environment and the command line, unless you use the *--nocfg*
 option. You can generate a default configuration file with the
 *--gencfg|-g* option followed by a filename. This file also offers
 full control over the checks to perform, and a way to discard
-false-positive vulnerabilities.
+false-positive vulnerabilities and unwanted licenses report
+messages.
 
 ### OPTIONS
 Options | Use
 ------- | ---
---nocfg\|-n|Don't use the configuration file
+--nocfg|Don't use the configuration file
 --gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
 --tree\|-t DIR|Set ports directory (default=/usr/ports)
@@ -226,13 +231,13 @@
 [Hubert Tournier](https://github.com/HubTou)
 
 ## CAVEATS
 The IGNORE mark check is not reliable because this tool doesn't parse
 the ports' Makefiles, but just loads their variables without regard to
 the conditional tests that may surround them.
 
-The nonexistent plist is not very helpful because there are unaccounted
-autoplist options for some languages (Python)...
+The nonexistent plist check is not very helpful because there are still
+undocumented cases where the list is auto generated.
 
 The ports using exotic versioning schemes will be skipped from the
 vulnerability check because the library we use for version comparisons
 is geared toward Python ports and limited for this usage.
```

### Comparing `pnu-portstreelint-1.3.0/setup.cfg` & `pnu_portstreelint-1.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pnu-portstreelint
 description = FreeBSD ports tree lint
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.3.0
+version = 1.4.0
 license = BSD 3-Clause License
 license_files = License
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/portstreelint/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/portstreelint/issues
```

### Comparing `pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/PKG-INFO` & `pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.3.0
+Version: 1.4.0
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
@@ -47,15 +47,15 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--nocfg|-n\]
+\[--nocfg\]
 \[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
 \[--tree|-t DIR\]
@@ -126,14 +126,18 @@
 * INDEX:www-site different from Makefile:WWW
 * Ports marked as BROKEN, DEPRECATED, FORBIDDEN, IGNORE, RESTRICTED (info)
 * Ports marked with an EXPIRATION_DATE (warning)
 * Ports marked as BROKEN, FORBIDDEN or DEPRECATED for too long (warning)
 * Ports unchanged for a long time (info)
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
+* Missing Makefile:LICENSE
+* Unofficial licenses (warning)
+* Unnecessary Makefile:LICENSE_COMB=single (warning)
+* Unnecessary Makefile:LICENSE_COMB=multi (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
 one and a number of days for the others. And you can select a port
 tree in a location other than */usr/ports* with the *--tree|-t*
@@ -143,24 +147,25 @@
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
 For convenience, you can put your favourite options in a
 configuration file, which will be read before processing the
-environment and the command line, unless you use the *--nocfg|-n*
+environment and the command line, unless you use the *--nocfg*
 option. You can generate a default configuration file with the
 *--gencfg|-g* option followed by a filename. This file also offers
 full control over the checks to perform, and a way to discard
-false-positive vulnerabilities.
+false-positive vulnerabilities and unwanted licenses report
+messages.
 
 ### OPTIONS
 Options | Use
 ------- | ---
---nocfg\|-n|Don't use the configuration file
+--nocfg|Don't use the configuration file
 --gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
 --tree\|-t DIR|Set ports directory (default=/usr/ports)
@@ -258,13 +263,13 @@
 [Hubert Tournier](https://github.com/HubTou)
 
 ## CAVEATS
 The IGNORE mark check is not reliable because this tool doesn't parse
 the ports' Makefiles, but just loads their variables without regard to
 the conditional tests that may surround them.
 
-The nonexistent plist is not very helpful because there are unaccounted
-autoplist options for some languages (Python)...
+The nonexistent plist check is not very helpful because there are still
+undocumented cases where the list is auto generated.
 
 The ports using exotic versioning schemes will be skipped from the
 vulnerability check because the library we use for version comparisons
 is geared toward Python ports and limited for this usage.
```

### Comparing `pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/SOURCES.txt` & `pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pnu_portstreelint.egg-info/requires.txt
 src/pnu_portstreelint.egg-info/top_level.txt
 src/portstreelint/__init__.py
 src/portstreelint/check_categories.py
 src/portstreelint/check_comment.py
 src/portstreelint/check_description_file.py
 src/portstreelint/check_installation_prefix.py
+src/portstreelint/check_licenses.py
 src/portstreelint/check_maintainer.py
 src/portstreelint/check_marks.py
 src/portstreelint/check_plist.py
 src/portstreelint/check_port_path.py
 src/portstreelint/check_unchanging_ports.py
 src/portstreelint/check_vulnerabilities.py
 src/portstreelint/check_www_site.py
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_categories.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_categories.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_comment.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_comment.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_description_file.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_description_file.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_installation_prefix.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_installation_prefix.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_maintainer.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_maintainer.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_marks.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_marks.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_port_path.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_port_path.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_unchanging_ports.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_unchanging_ports.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_vulnerabilities.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/check_www_site.py` & `pnu_portstreelint-1.4.0/src/portstreelint/check_www_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import urllib.request
 
 from .library import counters, notify_maintainer
 
 # Headers and timeout delay for HTTP(S) requests:
 HTTP_HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:124.0) Gecko/20100101 Firefox/124.0",
-    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
-    "Accept-Language": "en;q=1.0, en-US;q=0.8, *;q=0.5",
+    "Accept": "*/*",
+    "Accept-Language": "en;q=1.0, *;q=0.5",
     "Accept-Encoding": "identity",
     "Connection": "keep-alive",
 }
 CONNECTION_TIMEOUT = 10 # seconds
 
 ####################################################################################################
 def _resolve_hostname(hostname):
@@ -28,15 +28,14 @@
         ip_address = socket.gethostbyname(hostname)
     except socket.gaierror as error:
         error_message = re.sub(r".*] ", "", str(error))
         raise NameError(error_message) from error
 
     return ip_address
 
-
 ####################################################################################################
 def _handle_url_errors(port_name, www_site, error, maintainer):
     """ Decides what to do with the multiple possible fetching errors """
     is_unaccessible = False
     reason = "Unaccessible www-site"
     if error.lower().startswith("http error"):
         error_code = re.sub(r"http error ","", error.lower())
@@ -81,15 +80,14 @@
         logging.debug("%s (%s) '%s' for port %s", reason, error, www_site, port_name)
 
     if is_unaccessible:
         notify_maintainer(maintainer, reason, port_name)
 
     return is_unaccessible
 
-
 ####################################################################################################
 def check_www_site(ports, check_host, check_url):
     """ Checks the www-site field existence
     Rules at https://docs.freebsd.org/en/books/porters-handbook/makefiles/#makefile-www
     """
     unresolvable_hostnames = []
     url_ok = []
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/library.py` & `pnu_portstreelint-1.4.0/src/portstreelint/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     "Marked as IGNORE": 0,
     "Marked as RESTRICTED": 0,
     "Marked with EXPIRATION_DATE": 0,
     "Unchanged for a long time": 0,
     "Both PORTVERSION and DISTVERSION": 0,
     "Vulnerable port version": 0,
     "Skipped vulnerability checks": 0,
+    "Missing LICENSE": 0,
+    "Unofficial licenses": 0,
+    "Unnecessary LICENSE_COMB=single": 0,
+    "Unnecessary LICENSE_COMB=multi": 0,
 }
 
 # Global dictionary of notifications to port maintainers:
 notifications = {}
 
 ####################################################################################################
 def notify_maintainer(maintainer, error, port):
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/load_config.py` & `pnu_portstreelint-1.4.0/src/portstreelint/load_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import configparser
 import logging
 import os
 
 import libpnu
 
-
 ####################################################################################################
 def generate_config(parameters):
     """ Generates a configuration file with the default + environment + command line parameters """
 
     content = f"""# PortsTreeLint configuration file
 
 # Check the following URL for the file format:
@@ -24,27 +23,28 @@
 ports_dir = {parameters['Ports dir']}
 csv_filename =
 debug_level = warning
 #debug_level = info
 #debug_level = debug
 
 [checks]
-port_path = {parameters['Checks']['port-path']}
-installation_prefix = {parameters['Checks']['installation-prefix']}
+categories = {parameters['Checks']['categories']}
 comment = {parameters['Checks']['comment']}
 description_file = {parameters['Checks']['description-file']}
-plist = {parameters['Checks']['plist']}
-maintainer = {parameters['Checks']['maintainer']}
-categories = {parameters['Checks']['categories']}
-www_site = {parameters['Checks']['www-site']}
 hostnames = {parameters['Checks']['Hostnames']}
-url = {parameters['Checks']['URL']}
+installation_prefix = {parameters['Checks']['installation-prefix']}
+licenses = {parameters['Checks']['Licenses']}
+maintainer = {parameters['Checks']['maintainer']}
 marks = {parameters['Checks']['Marks']}
+plist = {parameters['Checks']['plist']}
+port_path = {parameters['Checks']['port-path']}
 unchanging_ports = {parameters['Checks']['Unchanging ports']}
+url = {parameters['Checks']['URL']}
 vulnerabilities = {parameters['Checks']['Vulnerabilities']}
+www_site = {parameters['Checks']['www-site']}
 
 [limits]
 # number of entries:
 plist_abuse = {parameters['Limits']['PLIST abuse']}
 # number of days:
 broken_since = {parameters['Limits']['BROKEN since']}
 forbidden_since = {parameters['Limits']['FORBIDDEN since']}
@@ -54,43 +54,43 @@
 [selections]
 # (multilines) lists of space separated values:
 categories =
 maintainers =
 ports =
 
 [exclusions]
-# (multilines) lists of space separated Vulnerabilities IDs:
-vulnerabilities =
+# (multilines) list of space separated Vulnerabilities IDs:
+vulnerabilities = 92442c4b-6f4a-11db-bd28-0012f06707f0
+    bd579366-5290-11d9-ac20-00065be4b5b6
+# (multilines) list of space separated PORTNAMEs:
+licenses = xfce
 """
 
     with open(parameters["INI filename"], "w", encoding="utf-8") as file:
         file.write(content)
 
-
 ####################################################################################################
 def _string2bool(string):
     """ Converts a string to a boolean without ValueError exception """
     if string.lower() in ("true", "yes", "on", "1"):
         return True
 
     # .getboolean() would generate an exception if string wasn't in "false", "no", "off", 0"...
     return False
 
-
 ####################################################################################################
 def _string2int(string, default):
     """ Converts a string to an int or use a default value without ValueError exception """
     try:
         value = int(string)
     except ValueError:
         value = default
 
     return value
 
-
 ####################################################################################################
 def load_config(parameters):
     """ Loads the user configuration file """
     home = libpnu.get_home_directory()
     if os.name == "nt":
         config_file = home + os.sep + "ptlint.ini"
     else:
@@ -106,40 +106,42 @@
                 parameters["CSV filename"] = config["params"]["csv_filename"]
             if "debug_level" in config["params"]:
                 if config["params"]["debug_level"] == "info":
                     logging.disable(logging.DEBUG)
                 elif config["params"]["debug_level"] == "debug":
                     logging.disable(logging.NOTSET)
         if "checks" in config:
-            if "port_path" in config["checks"]:
-                parameters["Checks"]["port-path"] = _string2bool(config["checks"]["port_path"])
-            if "installation_prefix" in config["checks"]:
-                parameters["Checks"]["installation-prefix"] = _string2bool(config["checks"]["installation_prefix"])
+            if "categories" in config["checks"]:
+                parameters["Checks"]["categories"] = _string2bool(config["checks"]["categories"])
             if "comment" in config["checks"]:
                 parameters["Checks"]["comment"] = _string2bool(config["checks"]["comment"])
             if "description_file" in config["checks"]:
                 parameters["Checks"]["description-file"] = _string2bool(config["checks"]["description_file"])
-            if "plist" in config["checks"]:
-                parameters["Checks"]["plist"] = _string2bool(config["checks"]["plist"])
-            if "maintainer" in config["checks"]:
-                parameters["Checks"]["maintainer"] = _string2bool(config["checks"]["maintainer"])
-            if "categories" in config["checks"]:
-                parameters["Checks"]["categories"] = _string2bool(config["checks"]["categories"])
-            if "www_site" in config["checks"]:
-                parameters["Checks"]["www-site"] = _string2bool(config["checks"]["www_site"])
             if "hostnames" in config["checks"]:
                 parameters["Checks"]["Hostnames"] = _string2bool(config["checks"]["hostnames"])
-            if "url" in config["checks"]:
-                parameters["Checks"]["URL"] = _string2bool(config["checks"]["url"])
+            if "installation_prefix" in config["checks"]:
+                parameters["Checks"]["installation-prefix"] = _string2bool(config["checks"]["installation_prefix"])
+            if "licenses" in config["checks"]:
+                parameters["Checks"]["Licenses"] = _string2bool(config["checks"]["licenses"])
+            if "maintainer" in config["checks"]:
+                parameters["Checks"]["maintainer"] = _string2bool(config["checks"]["maintainer"])
             if "marks" in config["checks"]:
                 parameters["Checks"]["Marks"] = _string2bool(config["checks"]["marks"])
+            if "plist" in config["checks"]:
+                parameters["Checks"]["plist"] = _string2bool(config["checks"]["plist"])
+            if "port_path" in config["checks"]:
+                parameters["Checks"]["port-path"] = _string2bool(config["checks"]["port_path"])
             if "unchanging_ports" in config["checks"]:
                 parameters["Checks"]["Unchanging ports"] = _string2bool(config["checks"]["unchanging_ports"])
+            if "url" in config["checks"]:
+                parameters["Checks"]["URL"] = _string2bool(config["checks"]["url"])
             if "vulnerabilities" in config["checks"]:
                 parameters["Checks"]["Vulnerabilities"] = _string2bool(config["checks"]["vulnerabilities"])
+            if "www_site" in config["checks"]:
+                parameters["Checks"]["www-site"] = _string2bool(config["checks"]["www_site"])
         if "limits" in config:
             if "plist_abuse" in config["limits"]:
                 parameters["Limits"]["PLIST abuse"] = _string2int(config["limits"]["plist_abuse"], parameters["Limits"]["PLIST abuse"])
             if "broken_since" in config["limits"]:
                 parameters["Limits"]["BROKEN since"] = _string2int(config["limits"]["broken_since"], parameters["Limits"]["BROKEN since"])
             if "forbidden_since" in config["limits"]:
                 parameters["Limits"]["FORBIDDEN since"] = _string2int(config["limits"]["forbidden_since"], parameters["Limits"]["FORBIDDEN since"])
@@ -153,9 +155,11 @@
             if "maintainers" in config["selections"]:
                 parameters["Selections"]["Maintainers"] = [m if '@' in m else f"{m}@freebsd.org" for m in config["selections"]["maintainers"].split()]
             if "ports" in config["selections"]:
                 parameters["Selections"]["Ports"] = config["selections"]["ports"].split()
         if "exclusions" in config:
             if "vulnerabilities" in config["exclusions"]:
                 parameters["Exclusions"]["Vulnerabilities"] = config["exclusions"]["vulnerabilities"].split()
+            if "licenses" in config["exclusions"]:
+                parameters["Exclusions"]["Licenses"] = config["exclusions"]["licenses"].split()
 
     return parameters
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/load_data.py` & `pnu_portstreelint-1.4.0/src/portstreelint/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
                     "run-depends": fields[12],
                 }
 
     counters["FreeBSD ports"] = len(ports)
     logging.info("Loaded %d ports from the FreeBSD Ports INDEX file", len(ports))
     return ports
 
-
 ####################################################################################################
 def filter_ports(ports, selected_categories, selected_maintainers, selected_ports):
     """ Filters the list of ports to the specified categories AND maintainers"""
     if selected_categories or selected_maintainers or selected_ports:
         all_ports = " ".join(ports.keys())
         for port in all_ports.split():
             if selected_maintainers:
@@ -89,15 +88,14 @@
                 if port_id not in selected_ports:
                     del ports[port]
 
     counters["Selected ports"] = len(ports)
     logging.info("Selected %d ports", len(ports))
     return ports
 
-
 ####################################################################################################
 def update_with_makefiles(ports, ports_dir):
     """ Loads selected part of port's Makefiles for cross-checking things """
     for name, port in ports.items():
         # Use the PORTSDIR we have been told to, rather than the system's one
         port_path = port["port-path"].replace("/usr/ports", ports_dir)
         if not os.path.isdir(port_path):
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/main.py` & `pnu_portstreelint-1.4.0/src/portstreelint/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,59 +8,59 @@
 import getopt
 import logging
 import os
 import sys
 
 import libpnu
 
-from .load_data import load_freebsd_ports_dict, filter_ports, update_with_makefiles
 from .load_config import generate_config, load_config
-from .check_port_path import check_port_path
-from .check_installation_prefix import check_installation_prefix
+from .load_data import load_freebsd_ports_dict, filter_ports, update_with_makefiles
+from .check_categories import check_categories
 from .check_comment import check_comment
 from .check_description_file import check_description_file
-from .check_plist import check_plist
+from .check_installation_prefix import check_installation_prefix
+from .check_licenses import check_licenses
 from .check_maintainer import check_maintainer
-from .check_categories import check_categories
-from .check_www_site import check_www_site
 from .check_marks import check_marks
+from .check_plist import check_plist
+from .check_port_path import check_port_path
 from .check_unchanging_ports import check_unchanging_ports
 from .check_vulnerabilities import check_vulnerabilities
+from .check_www_site import check_www_site
 from .show_categories import show_categories
 from .show_maintainers import show_maintainers
 from .show_notifications import show_notifications, output_notifications
 from .show_summary import show_summary
 
-
 # Version string used by the what(1) and ident(1) commands:
-ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.3.0 (April 1st, 2024) by Hubert Tournier $"
+ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.4.0 (April 13, 2024) by Hubert Tournier $"
 
 # Default parameters. Can be overcome by command line options:
 parameters = {
-    "Load config": True,
     "INI filename": "",
     "Ports dir": "/usr/ports",
     "CSV filename": "",
     "Show categories": False,
     "Show maintainers": False,
 
     "Checks": {
-        "port-path": True,
-		"installation-prefix": True,
+		"categories": True,
 		"comment": True,
 		"description-file": True,
-		"plist": True,
-		"maintainer": True,
-		"categories": True,
-		"www-site": True,
         "Hostnames": False,
-        "URL": False,
+		"installation-prefix": True,
+		"Licenses": True,
+		"maintainer": True,
 		"Marks": True,
+		"plist": True,
+        "port-path": True,
 		"Unchanging ports": True,
+        "URL": False,
 		"Vulnerabilities": True,
+		"www-site": True,
     },
     "Limits": {
         "PLIST abuse": 7, # entries
         "BROKEN since": 6 * 30, # days
         "FORBIDDEN since": 3 * 30, # days
         "DEPRECATED since": 6 * 30, # days
         "Unchanged since": 3 * 365, # days
@@ -68,30 +68,30 @@
     "Selections": {
         "Categories": [],
         "Maintainers": [],
         "Ports": [],
     },
     "Exclusions": {
         "Vulnerabilities": [],
+        "Licenses": [],
     },
 }
 
-
 ####################################################################################################
 def _display_help():
     """ Display usage and help """
     #pylint: disable=C0301
-    print("usage: portstreelint [--nocfg|-n] [--gencfg|-g FILE]", file=sys.stderr)
+    print("usage: portstreelint [--nocfg] [--gencfg|-g FILE]", file=sys.stderr)
     print("        [--tree|-t DIR] [--show-cat|-C] [--show-mnt|-M]", file=sys.stderr)
     print("        [--cat|-c LIST] [--mnt|-m LIST] [--port|-p LIST] [--plist NUM]", file=sys.stderr)
     print("        [--broken NUM] [--deprecated NUM] [--forbidden NUM] [--unchanged NUM]", file=sys.stderr)
     print("        [--check-host|-h] [--check-url|-u] [--output|-o FILE]", file=sys.stderr)
     print("        [--debug] [--help|-?] [--info] [--version] [--]", file=sys.stderr)
     print("  ------------------  -------------------------------------------------------", file=sys.stderr)
-    print("  --nocfg|-n          Don't use the configuration file", file=sys.stderr)
+    print("  --nocfg             Don't use the configuration file", file=sys.stderr)
     print("  --gencfg|-g FILE    Generate a default configuration file in FILE", file=sys.stderr)
     print("  --show-cat|-C       Show categories with ports count", file=sys.stderr)
     print("  --show-mnt|-M       Show maintainers with ports count", file=sys.stderr)
     print("  --cat|-c LIST       Select only the comma-separated categories in LIST", file=sys.stderr)
     print("  --mnt|-m LIST       Select only the comma-separated maintainers in LIST", file=sys.stderr)
     print("  --port|-p LIST      Select only the comma-separated ports in LIST", file=sys.stderr)
     print("  --tree|-t DIR       Set ports directory (default=/usr/ports)", file=sys.stderr)
@@ -107,15 +107,14 @@
     print("  --info              Enable logging at info level", file=sys.stderr)
     print("  --version           Print version and exit", file=sys.stderr)
     print("  --help|-?           Print usage and this help message and exit", file=sys.stderr)
     print("  --                  Options processing terminator", file=sys.stderr)
     print(file=sys.stderr)
     #pylint: enable=C0301
 
-
 ####################################################################################################
 def _process_environment_variables():
     """ Process environment variables """
     #pylint: disable=C0103, W0602
     global parameters
     #pylint: enable=C0103, W0602
 
@@ -127,25 +126,24 @@
             parameters["Ports dir"] = os.environ["PORTSDIR"][:-1]
         else:
             parameters["Ports dir"] = os.environ["PORTSDIR"]
 
     logging.debug("_process_environment_variables(): parameters:")
     logging.debug(parameters)
 
-
 ####################################################################################################
 def _process_command_line():
     """ Process command line options """
     #pylint: disable=C0103, W0602
     global parameters
     #pylint: enable=C0103, W0602
 
     # option letters followed by : expect an argument
     # same for option strings followed by =
-    character_options = "CMc:g:hm:no:p:t:u?"
+    character_options = "CMc:g:hm:o:p:t:u?"
     string_options = [
         "broken=",
         "cat=",
         "check-host",
         "check-url",
         "debug",
         "deprecated=",
@@ -236,16 +234,16 @@
                 logging.critical("--gencfg|-g argument cannot be an existing filesystem item")
                 sys.exit(1)
 
         elif option in ("--mnt", "-m"):
             maintainers = argument.lower().split(",")
             parameters["Selections"]["Maintainers"] = [m if '@' in m else f"{m}@freebsd.org" for m in maintainers]
 
-        elif option in ("--nocfg", "-n"):
-            parameters["Load config"] = False
+        elif option == "--nocfg":
+            pass # need to be handled BEFORE this function
 
         elif option in ("--output", "-o"):
             parameters["CSV filename"] = argument
 
         elif option == "--plist":
             try:
                 parameters["Checks"]["PLIST abuse"] = int(argument)
@@ -290,28 +288,28 @@
     logging.debug("_process_command_line(): parameters:")
     logging.debug(parameters)
     logging.debug("_process_command_line(): remaining_arguments:")
     logging.debug(remaining_arguments)
 
     return remaining_arguments
 
-
 ####################################################################################################
 def main():
     """ The program's main entry point """
     #pylint: disable=C0103, W0602
     global parameters
     #pylint: enable=C0103, W0602
 
     program_name = os.path.basename(sys.argv[0])
 
     libpnu.initialize_debugging(program_name)
     libpnu.handle_interrupt_signals(libpnu.interrupt_handler_function)
 
-    if parameters["Load config"]:
+    print(sys.argv[1:])
+    if not "--nocfg" in sys.argv[1:]:
         parameters = load_config(parameters)
     _process_environment_variables()
     _ = _process_command_line()
 
     # Load the FreeBSD ports INDEX file
     # and verify structural integrity (ie: 13 pipe-separated fields)
     # and unicity of distribution-names
@@ -386,22 +384,25 @@
         if parameters["Checks"]["Unchanging ports"]:
             check_unchanging_ports(ports, parameters["Limits"]["Unchanged since"])
 
         # Check vulnerabilities
         if parameters["Checks"]["Vulnerabilities"]:
             check_vulnerabilities(ports, parameters["Exclusions"]["Vulnerabilities"])
 
+        # Check licenses
+        if parameters["Checks"]["Licenses"]:
+            check_licenses(ports, parameters["Exclusions"]["Licenses"])
+
         # Print results per maintainer
         show_notifications()
 
         # Output per maintainer results in a CSV file
         if parameters["CSV filename"]:
             output_notifications(parameters["CSV filename"])
 
         # Print summary of findings
         show_summary(parameters["Limits"])
 
     sys.exit(0)
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/show_categories.py` & `pnu_portstreelint-1.4.0/src/portstreelint/show_categories.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/show_maintainers.py` & `pnu_portstreelint-1.4.0/src/portstreelint/show_maintainers.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/show_notifications.py` & `pnu_portstreelint-1.4.0/src/portstreelint/show_notifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         for issue, ports in details.items():
             print(f"    {issue}:")
             all_ports = " ".join(ports)
             for line in textwrap.wrap(all_ports, width=74, break_on_hyphens=False):
                 print(f"      {line}")
         print()
 
-
 ####################################################################################################
 def output_notifications(filename):
     """ Output notifications in a CSV file """
     sorted_notifications = dict(sorted(notifications.items()))
     try:
         file = open(filename, "w",  encoding='utf-8')
     except Exception:
```

### Comparing `pnu-portstreelint-1.3.0/src/portstreelint/show_summary.py` & `pnu_portstreelint-1.4.0/src/portstreelint/show_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 ####################################################################################################
 def _conditional_print(counter, message):
     """ Print a message if the counter is non zero """
     if counters[counter]:
         value = counters[counter]
         print(f"  {value} port{'' if value == 1 else 's'} {message}")
 
-
 ####################################################################################################
 def show_summary(limits):
     """ Pretty prints a summary of findings """
     print(f'Selected {counters["Selected ports"]} ports out of {counters["FreeBSD ports"]} in the FreeBSD port tree, and found:')
     _conditional_print("Nonexistent port-path", "with non existent port-path")
     _conditional_print("Nonexistent Makefile", "without Makefile")
     _conditional_print("Unusual installation-prefix", "with unusual installation-prefix (warning)")
@@ -46,7 +45,11 @@
     _conditional_print("Marked as FORBIDDEN for too long", f"with a FORBIDDEN mark older than {limits['FORBIDDEN since']} days (warning)")
     _conditional_print("Marked as IGNORE", "with a IGNORE mark in some cases (info)")
     _conditional_print("Marked as RESTRICTED", "with a RESTRICTED mark (info)")
     _conditional_print("Marked with EXPIRATION_DATE", "with an EXPIRATION_DATE mark (warning)")
     _conditional_print("Unchanged for a long time", f"with a last modification older than {limits['Unchanged since']} days (info)")
     _conditional_print("Both PORTVERSION and DISTVERSION", "with both PORTVERSION and DISTVERSION")
     _conditional_print("Vulnerable port version", "with a vulnerable version (warning)")
+    _conditional_print("Missing LICENSE", "without defined LICENSE")
+    _conditional_print("Unofficial licenses", "referring to unofficial licenses (warning)")
+    _conditional_print("Unnecessary LICENSE_COMB=single", "with unnecessary LICENSE_COMB=single (warning)")
+    _conditional_print("Unnecessary LICENSE_COMB=multi", "with unnecessary LICENSE_COMB=multi (warning)")
```

