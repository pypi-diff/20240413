# Comparing `tmp/trame-client-3.0.0.tar.gz` & `tmp/trame-client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-3.0.0.tar", last modified: Wed Apr 10 23:24:30 2024, max compression
+gzip compressed data, was "trame-client-3.0.1.tar", last modified: Fri Apr 12 22:23:23 2024, max compression
```

## Comparing `trame-client-3.0.0.tar` & `trame-client-3.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.334217 trame-client-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-10 23:24:01.000000 trame-client-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-10 23:24:01.000000 trame-client-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3539 2024-04-10 23:24:30.334217 trame-client-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-10 23:24:01.000000 trame-client-3.0.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      935 2024-04-10 23:24:30.334217 trame-client-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 23:24:01.000000 trame-client-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.322217 trame-client-3.0.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.322217 trame-client-3.0.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.322217 trame-client-3.0.0/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    25939 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/js/app.534cb160.js
--rw-r--r--   0 root         (0) root         (0)   156057 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
--rw-r--r--   0 root         (0) root         (0)     2890 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2024-04-10 23:24:20.000000 trame-client-3.0.0/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.330217 trame-client-3.0.0/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.330217 trame-client-3.0.0/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   102015 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/assets/index-a289433b.js
--rw-r--r--   0 root         (0) root         (0)     1359 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/assets/index-e80c1ba5.css
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     2890 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   147534 2024-04-10 23:24:26.000000 trame-client-3.0.0/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.330217 trame-client-3.0.0/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.330217 trame-client-3.0.0/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9364 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.330217 trame-client-3.0.0/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1134 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/formatter.py
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     3816 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/testing.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/version.py
--rw-r--r--   0 root         (0) root         (0)     3190 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/utils/web_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.334217 trame-client-3.0.0/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22879 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     8810 2024-04-10 23:24:01.000000 trame-client-3.0.0/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:24:30.326217 trame-client-3.0.0/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3539 2024-04-10 23:24:30.000000 trame-client-3.0.0/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-10 23:24:30.000000 trame-client-3.0.0/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 23:24:30.000000 trame-client-3.0.0/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-10 23:24:30.000000 trame-client-3.0.0/trame_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 23:24:30.000000 trame-client-3.0.0/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-12 22:22:53.000000 trame-client-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-12 22:22:53.000000 trame-client-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-04-12 22:23:23.328211 trame-client-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-12 22:22:53.000000 trame-client-3.0.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      935 2024-04-12 22:23:23.332212 trame-client-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 22:22:53.000000 trame-client-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    26004 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/js/app.7c11979c.js
+-rw-r--r--   0 root         (0) root         (0)   156057 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   102078 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/assets/index-26129a2a.js
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/assets/index-e80c1ba5.css
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   147534 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9364 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/formatter.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/testing.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/version.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/web_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22879 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-3.0.0/LICENSE` & `trame-client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/PKG-INFO` & `trame-client-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.0/README.rst` & `trame-client-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/setup.cfg` & `trame-client-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 3.0.0
+version = 3.0.1
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-3.0.0/trame_client/LICENSE` & `trame-client-3.0.1/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/encoders/numpy.py` & `trame-client-3.0.1/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-3.0.1/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/index.html` & `trame-client-3.0.1/trame_client/module/vue2-www/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="" data-app-name="trame"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,minimum-scale=1"><meta name="description" content="Application built with trame, a product from Kitware"><meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware"><meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate"/><meta http-equiv="Pragma" content="no-cache"/><meta http-equiv="Expires" content="0"/><link rel="icon" href="logo.png"><script src="vue.global.js"></script><title>trame is built by Kitware</title><script defer="defer" src="js/chunk-vendors.3aa0189c.js"></script><script defer="defer" src="js/app.534cb160.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script>fetch("./loading.tpl").then((r) => r.text()).then((c) => document.querySelector("#app").innerHTML = c)</script></body></html>
+<!doctype html><html lang="" data-app-name="trame"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,minimum-scale=1"><meta name="description" content="Application built with trame, a product from Kitware"><meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware"><meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate"/><meta http-equiv="Pragma" content="no-cache"/><meta http-equiv="Expires" content="0"/><link rel="icon" href="logo.png"><script src="vue.global.js"></script><title>trame is built by Kitware</title><script defer="defer" src="js/chunk-vendors.3aa0189c.js"></script><script defer="defer" src="js/app.7c11979c.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script>fetch("./loading.tpl").then((r) => r.text()).then((c) => document.querySelector("#app").innerHTML = c)</script></body></html>
```

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/js/app.534cb160.js` & `trame-client-3.0.1/trame_client/module/vue2-www/js/app.7c11979c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -165,22 +165,22 @@
                         resetClient: _,
                         getStatus: C,
                         configDecorator: b
                     },
                     $ = (n(8324), n(9274)),
                     R = n(7117);
                 n(5137);
-                const O = {};
+                const x = {};
 
-                function x(e, t) {
+                function O(e, t) {
                     return e.priority - t.priority
                 }
 
                 function L(e) {
-                    O.addAttachement = e
+                    x.addAttachement = e
                 }
                 const U = {
                         priority: 0,
                         async decorate(e) {
                             if (null === e || void 0 === e) return e;
                             if (e.constructor && e.constructor === File) {
                                 const {
@@ -235,15 +235,15 @@
                             }
                             return e
                         }
                     },
                     j = [U, A, k];
 
                 function N(e) {
-                    j.push(e), j.sort(x)
+                    j.push(e), j.sort(O)
                 }
                 async function V(e) {
                     let t = e;
                     for (let n = 0; n < j.length; n++) {
                         if (null === t || void 0 === t) return t;
                         t = await j[n].decorate(t)
                     }
@@ -840,16 +840,16 @@
                         spin: "style_spin_BAaPb",
                         message: "style_message_rmggO"
                     };
 
                 function Re(e) {
                     this["$style"] = $e.locals || $e
                 }
-                var Oe = (0, le.Z)(Se, Te, _e, !1, Re, null, null),
-                    xe = Oe.exports,
+                var xe = (0, le.Z)(Se, Te, _e, !1, Re, null, null),
+                    Oe = xe.exports,
                     Le = function() {
                         var e = this,
                             t = e._self._c;
                         return t("div", {
                             class: e.$style.container
                         }, [t("div", {
                             class: e.$style.center
@@ -1107,27 +1107,29 @@
                     }
                 };
                 const {
                     onMounted: ct,
                     onBeforeUnmount: ut
                 } = window.Vue;
                 var ht = {
-                    emits: ["mounted", "created", "beforeDestroy", "beforeUnmount"],
+                    emits: ["mounted", "created", "beforeDestroy", "beforeUnmount", "exit"],
                     setup(e, {
                         emit: t,
                         expose: n
                     }) {
                         function s(e, n) {
                             t(e, n)
                         }
                         return ct((() => t("mounted"))), ut((() => {
                             t("beforeDestroy"), t("beforeUnmount")
                         })), n({
                             emit: s
-                        }), t("created"), {
+                        }), window.addEventListener("beforeunload", (() => {
+                            t("exit")
+                        })), t("created"), {
                             emit: s
                         }
                     }
                 };
                 const {
                     onMounted: mt,
                     onUpdated: dt,
@@ -1225,47 +1227,47 @@
                             }
                         },
                         template: '<div ref="elem" style="overflow: hidden; position: relative; width: 100%; height: 100%; margin: 0; padding: 0;"><slot></slot></div>'
                     },
                     Rt = {
                         TrameApp: we,
                         TrameConnect: ue,
-                        TrameLoading: xe,
+                        TrameLoading: Oe,
                         TrameReconnect: Ee,
                         TrameTemplate: ye,
                         TrameStateResolver: Ke,
                         TrameStyle: Ye,
                         TrameExec: Qe,
                         TrameGetter: it,
                         TrameClientStateChange: lt,
                         TrameClientTriggers: ht,
                         TrameLifeCycleMonitor: wt,
                         TrameSizeObserver: $t
                     },
-                    Ot = {
+                    xt = {
                         install(e) {
                             Object.keys(Rt).forEach((t => {
                                 e.component(t, Rt[t])
                             }))
                         }
                     };
-                const xt = "TrameConnect";
+                const Ot = "TrameConnect";
 
                 function Lt() {
-                    const e = S.getStatus(xt),
+                    const e = S.getStatus(Ot),
                         t = document.querySelector(".trame__message");
                     t ? t.innerHTML = e.message || e.type : console.error("WsError", e.message || e.type)
                 }
                 async function Ut(e) {
                     try {
                         var t, n, r;
                         null !== (t = window) && void 0 !== t && null !== (n = t.parent) && void 0 !== n && null !== (r = n.trameJupyter) && void 0 !== r && r.init && (window.WSLINK = window.parent.trameJupyter.init(window))
                     } catch (o) {}
-                    e.use(Ot);
-                    const i = S.getClient(xt);
+                    e.use(xt);
+                    const i = S.getClient(Ot);
                     try {
                         await i.connect(S.configDecorator({
                             application: "trame",
                             useUrl: !0
                         }))
                     } catch (o) {
                         return void Lt()
@@ -1375,8 +1377,8 @@
             s.forEach(t.bind(null, 0)), s.push = t.bind(null, s.push.bind(s))
         }();
     var s = n.O(void 0, [998], (function() {
         return n(7660)
     }));
     s = n.O(s)
 })();
-//# sourceMappingURL=app.534cb160.js.map
+//# sourceMappingURL=app.7c11979c.js.map
```

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js` & `trame-client-3.0.1/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/loading.tpl` & `trame-client-3.0.1/trame_client/module/vue2-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/logo.png` & `trame-client-3.0.1/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue2-www/vue.global.js` & `trame-client-3.0.1/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/assets/index-a289433b.js` & `trame-client-3.0.1/trame_client/module/vue3-www/assets/index-26129a2a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4211,24 +4211,26 @@
         }
     },
     {
         onMounted: cs,
         onBeforeUnmount: us
     } = window.Vue,
     fs = {
-        emits: ["mounted", "created", "beforeDestroy", "beforeUnmount"],
+        emits: ["mounted", "created", "beforeDestroy", "beforeUnmount", "exit"],
         setup(t, {
             emit: e,
             expose: n
         }) {
             function r(i, o) {
                 e(i, o)
             }
             return cs(() => e("mounted")), us(() => {
                 e("beforeDestroy"), e("beforeUnmount")
+            }), window.addEventListener("beforeunload", () => {
+                e("exit")
             }), n({
                 emit: r
             }), e("created"), {
                 emit: r
             }
         }
     },
```

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/assets/index-e80c1ba5.css` & `trame-client-3.0.1/trame_client/module/vue3-www/assets/index-e80c1ba5.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/index.html` & `trame-client-3.0.1/trame_client/module/vue3-www/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware">
     <meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate" />
     <meta http-equiv="Pragma" content="no-cache" />
     <meta http-equiv="Expires" content="0" />
     <link rel="icon" href="logo.png">
     <title>trame is built by Kitware</title>
     <script src="vue.global.js"></script>
-    <script type="module" crossorigin src="./assets/index-a289433b.js"></script>
+    <script type="module" crossorigin src="./assets/index-26129a2a.js"></script>
     <link rel="stylesheet" href="./assets/index-e80c1ba5.css">
   </head>
   <body>
     <noscript>
       <strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
     </noscript>
     <div id="app"></div>
```

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/loading.tpl` & `trame-client-3.0.1/trame_client/module/vue3-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/logo.png` & `trame-client-3.0.1/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/module/vue3-www/vue.global.js` & `trame-client-3.0.1/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/resources/attributes.json` & `trame-client-3.0.1/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/resources/vue.json` & `trame-client-3.0.1/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/ui/core.py` & `trame-client-3.0.1/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/ui/html.py` & `trame-client-3.0.1/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/utils/formatter.py` & `trame-client-3.0.1/trame_client/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/utils/testing.py` & `trame-client-3.0.1/trame_client/utils/testing.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/utils/version.py` & `trame-client-3.0.1/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/utils/web_module.py` & `trame-client-3.0.1/trame_client/utils/web_module.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/widgets/core.py` & `trame-client-3.0.1/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/widgets/generator.py` & `trame-client-3.0.1/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/widgets/html.py` & `trame-client-3.0.1/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.0/trame_client/widgets/trame.py` & `trame-client-3.0.1/trame_client/widgets/trame.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,20 +188,31 @@
 # -----------------------------------------------------------------------------
 class ClientTriggers(AbstractElement):
     """
     Allow to trigger an event on the client side
 
     :param ref: Identifier for the client side DOM elem
     :param **kwargs: List of events to registers with their callbacks
+
+    Built-in events are:
+       - mounted
+       - created
+       - before_destroy
+       - before_unmount
+       - exit
     """
 
     def __init__(self, ref="trame_triggers", children=None, **kwargs):
         self.__name = ref
         super().__init__("trame-client-triggers", children=None, ref=ref, **kwargs)
         self._attr_names += ["ref"]
+        self._event_names += [
+            ("before_destroy", "beforeDestroy"),
+            ("before_unmount", "beforeUnmount"),
+        ]
         self._event_names += list(kwargs.keys())
 
     def call(self, method, *args):
         """
         Perform the call on the client
 
         :param method: Key used in the kwargs at construction time
```

### Comparing `trame-client-3.0.0/trame_client.egg-info/PKG-INFO` & `trame-client-3.0.1/trame_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.0
+Version: 3.0.1
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.0/trame_client.egg-info/SOURCES.txt` & `trame-client-3.0.1/trame_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 trame_client/module/vue2.py
 trame_client/module/vue3.py
 trame_client/module/vue2-www/index.html
 trame_client/module/vue2-www/loading.tpl
 trame_client/module/vue2-www/logo.png
 trame_client/module/vue2-www/vue.global.js
 trame_client/module/vue2-www/css/app.0b077e70.css
-trame_client/module/vue2-www/js/app.534cb160.js
+trame_client/module/vue2-www/js/app.7c11979c.js
 trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
 trame_client/module/vue3-www/index.html
 trame_client/module/vue3-www/loading.tpl
 trame_client/module/vue3-www/logo.png
 trame_client/module/vue3-www/vue.global.js
-trame_client/module/vue3-www/assets/index-a289433b.js
+trame_client/module/vue3-www/assets/index-26129a2a.js
 trame_client/module/vue3-www/assets/index-e80c1ba5.css
 trame_client/resources/attributes.json
 trame_client/resources/events.json
 trame_client/resources/vue.json
 trame_client/ui/__init__.py
 trame_client/ui/core.py
 trame_client/ui/html.py
```

