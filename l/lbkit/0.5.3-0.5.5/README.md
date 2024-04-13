# Comparing `tmp/lbkit-0.5.3.tar.gz` & `tmp/lbkit-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbkit-0.5.3.tar", last modified: Wed Mar 27 16:24:06 2024, max compression
+gzip compressed data, was "lbkit-0.5.5.tar", last modified: Sat Apr 13 15:08:04 2024, max compression
```

## Comparing `lbkit-0.5.3.tar` & `lbkit-0.5.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/
--rw-rw-r--   0 root         (0) root         (0)      122 2024-03-27 16:23:59.000000 lbkit-0.5.3/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-03-27 16:23:59.000000 lbkit-0.5.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      149 2024-03-27 16:23:59.000000 lbkit-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2024-03-27 16:24:06.919228 lbkit-0.5.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      388 2024-03-27 16:23:59.000000 lbkit-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.915228 lbkit-0.5.3/lbkit/
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/ci_robot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/ci_robot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12840 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/ci_robot/gitee.py
--rw-rw-r--   0 root         (0) root         (0)     8454 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/codegen/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3871 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/codegen.py
--rw-rw-r--   0 root         (0) root         (0)     7893 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/ctype_defination.py
--rw-rw-r--   0 root         (0) root         (0)    21001 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/idf_interface.py
--rw-rw-r--   0 root         (0) root         (0)      287 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/codegen/template/
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/client.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2888 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/client.h.mako
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/interface.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2297 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/interface.introspect.xml.mako
--rw-rw-r--   0 root         (0) root         (0)    26093 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/public.c.mako
--rw-rw-r--   0 root         (0) root         (0)     8059 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/public.h.mako
--rw-rw-r--   0 root         (0) root         (0)     3950 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/server.c.mako
--rw-rw-r--   0 root         (0) root         (0)     1492 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/codegen/template/server.h.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/component/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2155 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/arg_parser.py
--rw-rw-r--   0 root         (0) root         (0)     9926 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/component/template/
--rw-rw-r--   0 root         (0) root         (0)     8320 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/template/conanbase.mako
--rw-rw-r--   0 root         (0) root         (0)      452 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/template/deploy.mako
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/component/test.py
--rw-rw-r--   0 root         (0) root         (0)     1886 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/errors.py
--rw-rw-r--   0 root         (0) root         (0)      829 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2762 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/build_manifest.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/build_prepare.py
--rw-rw-r--   0 root         (0) root         (0)     8475 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/build_rootfs.py
--rw-rw-r--   0 root         (0) root         (0)     2890 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/config.py
--rw-rw-r--   0 root         (0) root         (0)     4637 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit/integration/template/
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/integration/template/conanfile.py.mako
--rw-rw-r--   0 root         (0) root         (0)      114 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/lbkit.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/log.py
--rw-rw-r--   0 root         (0) root         (0)     3021 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/misc.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-03-27 16:23:59.000000 lbkit-0.5.3/lbkit/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:24:06.919228 lbkit-0.5.3/lbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1268 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-27 16:24:06.000000 lbkit-0.5.3/lbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 16:24:06.919228 lbkit-0.5.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1295 2024-03-27 16:23:59.000000 lbkit-0.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.931476 lbkit-0.5.5/
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-04-13 15:07:56.000000 lbkit-0.5.5/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-13 15:07:56.000000 lbkit-0.5.5/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      149 2024-04-13 15:07:56.000000 lbkit-0.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-13 15:08:04.927476 lbkit-0.5.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-04-13 15:07:56.000000 lbkit-0.5.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.923476 lbkit-0.5.5/lbkit/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-13 15:07:57.000000 lbkit-0.5.5/lbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.923476 lbkit-0.5.5/lbkit/ci_robot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/ci_robot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/ci_robot/gitee.py
+-rw-rw-r--   0 root         (0) root         (0)     8454 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/codegen/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3881 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/codegen.py
+-rw-rw-r--   0 root         (0) root         (0)     7893 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/ctype_defination.py
+-rw-rw-r--   0 root         (0) root         (0)    23132 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/idf_interface.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/codegen/template/
+-rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/client.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/client.h.mako
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/interface.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/interface.introspect.xml.mako
+-rw-rw-r--   0 root         (0) root         (0)    26271 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/public.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     8106 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/public.h.mako
+-rw-rw-r--   0 root         (0) root         (0)    12974 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/server.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     1492 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/server.h.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/component/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/arg_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    10709 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/component/template/
+-rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/template/conanbase.mako
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/template/deploy.mako
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/test.py
+-rw-rw-r--   0 root         (0) root         (0)     1886 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/errors.py
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/integration/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_prepare.py
+-rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_rootfs.py
+-rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/integration/template/
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/template/conanfile.py.mako
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/lbkit.py
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3180 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 15:08:04.931476 lbkit-0.5.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-13 15:07:56.000000 lbkit-0.5.5/setup.py
```

### Comparing `lbkit-0.5.3/LICENSE` & `lbkit-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/PKG-INFO` & `lbkit-0.5.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.3
+Version: 0.5.5
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.3/lbkit/ci_robot/gitee.py` & `lbkit-0.5.5/lbkit/ci_robot/gitee.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/cli.py` & `lbkit-0.5.5/lbkit/cli.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/codegen/codegen.py` & `lbkit-0.5.5/lbkit/codegen/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from lbkit.helper import Helper
 from lbkit.errors import ArgException
 from lbkit.misc import SmartFormatter
 
 lb_cwd = os.path.split(os.path.realpath(__file__))[0]
 log = Logger("codegen")
 
+__version__=1
 
 class CodeGen(object):
     def __init__(self, args):
         self.args = args
         pass
 
     def _gen(self, idf_file, directory="."):
@@ -62,15 +63,15 @@
                     log.error("%s的自动代码生成配置不正确, %s的文件名不是以.yaml结束", package_yml, file)
                     sys.exit(-1)
                 if not os.path.isfile(file):
                     log.error("%s的自动代码生成配置不正确, %s不是一个文件", package_yml, file)
                     sys.exit(-1)
                 outdir = cfg.get("outdir", os.getcwd())
                 self._gen(file, outdir)
-                return
+            return
 
         parser = argparse.ArgumentParser(description=self.run.__doc__,
                                          prog="lbkit gen",
                                          formatter_class=SmartFormatter)
         parser.add_argument("-i", "--input", help='A IDF file to be processed e.g.: com.litebmc.Upgrade.xml', required=True)
         parser.add_argument("-d", "--directory", help='generate code directory', default=".")
```

### Comparing `lbkit-0.5.3/lbkit/codegen/ctype_defination.py` & `lbkit-0.5.5/lbkit/codegen/ctype_defination.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/codegen/idf_interface.py` & `lbkit-0.5.5/lbkit/codegen/idf_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 
 METHOD_NAME_REGEX = "[A-Z][a-zA-Z0-9_]*"
 SIGNAL_NAME_REGEX = METHOD_NAME_REGEX
 STRU_NAME_REGEX = METHOD_NAME_REGEX
 ENUM_NAME_REGEX = METHOD_NAME_REGEX
 DICT_NAME_REGEX = METHOD_NAME_REGEX
 
-CTYPE_REGEX = "boolean|byte|int16|uint16|int32|uint32|int64|uint64|size|ssize|double|string|object_path|signature|unixfd|variant"
+CTYPE_BASE_REG = "boolean|byte|int16|uint16|int32|uint32|int64|uint64|size|ssize|double|string|object_path|signature|unixfd"
+CTYPE_REGEX = CTYPE_BASE_REG + "|variant"
 
 CTYPE_SIGNATURE_MAP = {
     "boolean": "b",
     "byte": "y",
     "int16": "n",
     "uint16": "q",
     "int32": "i",
@@ -132,15 +133,15 @@
         # 如果set类型由转换成数组，当前不具备对set类型独立处理能力
         if match:
             self.ctype = f"array[enum[{match.group(1)}]]"
 
     def declare(self):
         """变量申明，用于结构体（接口类、方法请求和响应、信号消息等）申明"""
         log.debug(f"Get declare info, name: {self.name}, ctype: {self.ctype}")
-        match = re.match(f"^array\[({CTYPE_REGEX})\]$", self.ctype)
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.declare
         match = re.match(f"^({CTYPE_REGEX})$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.declare
@@ -172,15 +173,15 @@
                 return [f"{stru_name} *<const>*<arg_name>"]
             else:
                 return [f"<const>{stru_name} *<arg_name>"]
 
     def free_func(self):
         """生成释放数据的C函数，如果是结构体、字典需要生成对象的释放函数"""
         log.debug(f"Get free function info, name: {self.name}, ctype: {self.ctype}")
-        match = re.match(f"^array\[({CTYPE_REGEX})\]$", self.ctype)
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.free_func
         match = re.match(f"^({CTYPE_REGEX})$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.free_func
@@ -201,15 +202,15 @@
             if is_array:
                 return [f"{stru_name}_free_v(&<arg_name>)"]
             else:
                 return [f"{stru_name}_free(&<arg_name>)"]
 
     def encode_func(self):
         log.debug(f"Get encode function info, name: {self.name}, ctype: {self.ctype}")
-        match = re.match(f"^array\[({CTYPE_REGEX})\]$", self.ctype)
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.encode_func
         match = re.match(f"^({CTYPE_REGEX})$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.encode_func
@@ -234,15 +235,15 @@
                 return [f"<arg_out> = {stru_name}_encode_v(<arg_name>)"]
             else:
                 return [f"<arg_out> = {stru_name}_encode(<arg_name>)"]
 
 
     def decode_func(self):
         log.debug(f"Get decode info, name: {self.name}, ctype: {self.ctype}")
-        match = re.match(f"^array\[({CTYPE_REGEX})\]$", self.ctype)
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.decode_func
         match = re.match(f"^({CTYPE_REGEX})$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.decode_func
@@ -264,26 +265,71 @@
         else:
             if is_array:
                 # 入参为二级指针
                 return [f"<arg_in> = {stru_name}_decode_v(<arg_name>)"]
             else:
                 return [f"<arg_in> = {stru_name}_decode(<arg_name>)"]
 
+    def odf_load_func(self):
+        log.debug(f"Get odf_load function, name: {self.name}, ctype: {self.ctype}")
+        # odf不支持gariant
+        match = re.match(f"^array\[(variant)\]$", self.ctype)
+        if match:
+            return None
+        match = re.match(f"^variant$", self.ctype)
+        if match:
+            return None
+        # 字符串数组由结束NULL表示，不需要长度
+        match = re.match(f"^array\[(string|object_path|signature)\]$", self.ctype)
+        if match:
+            return "<arg_name> = load_odf_as_" + match.group(1) + "_v(doc, <node>)"
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
+        if match:
+            return "<arg_name> = load_odf_as_" + match.group(1) + "_v(doc, <node>, &n_<arg_name>)"
+        match = re.match(f"^({CTYPE_REGEX})$", self.ctype)
+        if match:
+            return "<arg_name> = load_odf_as_" + match.group(1) + "(doc, <node>)"
+        # 非基础类型
+        is_array = False
+        ctype = self.ctype
+        match = re.match(f"^array\[(.*)\]$", ctype)
+        if match:
+            is_array = True
+            ctype = match.group(1)
+        match = re.match(f"^(struct|enum|dict)\[(.*)\]$", ctype)
+        _, stru_name = get_intfname_and_ctype(match.group(2))
+        if match.group(1) == "enum":
+            if is_array:
+                # 入参为二级指针
+                return f"<arg_name> = _load_odf_as_{stru_name}_v(doc, <node>, &n_<arg_name>)"
+            else:
+                return f"<arg_name> = _load_odf_as_{stru_name}(doc, <node>)"
+        else:
+            if is_array:
+                # 入参为二级指针
+                return f"<arg_name> = _load_odf_as_{stru_name}_v(doc, <node>)"
+            else:
+                return f"<arg_name> = _load_odf_as_{stru_name}(doc, <node>)"
+
 class IdfProperty(IdfCtypeRender):
     def __init__(self, intf: IdfInterfaceBase, prop_data):
         self.intf = intf
         self.ctype = prop_data.get("type", "")
         super().__init__()
         self.name = prop_data.get("name")
         self.access = "read"
         self.annotations: list[IdfAnnotation] = []
         self.description = prop_data.get("description", "")
         flags = prop_data.get("flags", "").split(",")
+        self.flags = flags
         self.private = True if ("private" in flags) else False
         self.deprecated = True if ("deprecated" in flags) else False
+        # refobj的ctype只能是s或as
+        if "refobj" in flags and self.ctype != "string" and self.ctype != "array[string]":
+                raise IDFException(f"property {self.name} with refobj flag but type is neither s nor as")
         for k, v in ACCESS_MAP.items():
             if k in flags:
                 self.access = v
                 break
         self.access_flag = ACCESS_FLAG_MAP.get(self.access)
         for k, v in ANNOTATION_MAP.items():
             if k in flags:
```

### Comparing `lbkit-0.5.3/lbkit/codegen/template/client.c.mako` & `lbkit-0.5.5/lbkit/codegen/template/client.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/codegen/template/client.h.mako` & `lbkit-0.5.5/lbkit/codegen/template/client.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/codegen/template/interface.introspect.xml.mako` & `lbkit-0.5.5/lbkit/codegen/template/interface.introspect.xml.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/codegen/template/public.c.mako` & `lbkit-0.5.5/lbkit/codegen/template/public.c.mako`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,22 @@
 ## 枚举序列化和反序列化函数
 static const gchar *_${name}StrMap[] = {
 % for value in enum.values.parameters:
     "${intf.name}.${name}.${value.name}",
 % endfor
 };
 
+const gchar *${name}_as_string(${name} value)
+{
+    if (value >= _${name}Invalid) {
+        return "com.litebmc.Errors.Enum.Invalid";
+    }
+    return _${name}StrMap[value];
+}
+
 /* ${name}枚举类型序列化（enum转string）函数 */
 GVariant *${name}_encode(${name} value)
 {
     ## 非法值返回com.litebmc.Errors.Enum.Invalid
     if (value > ${name}_${enum.values.parameters[len(enum.values.parameters) - 1].name}) {
         return g_variant_new_string("com.litebmc.Errors.Enum.Invalid");
     }
@@ -161,14 +169,15 @@
     for (int i = 0; i <= ${len(enum.values.parameters)}; i++) {
         if (g_strcmp0(in_val, _${name}StrMap[i]) == 0) {
             return (${name})i;
         }
     }
     return _${name}Invalid;
 }
+
 /* ${name}枚举类型序列化（enum转string）函数 */
 GVariant *${name}_encode_v(const ${name} *values, gsize n)
 {
     g_assert(n == 0 || values);
 
     GVariantBuilder builder;
     g_variant_builder_init(&builder, G_VARIANT_TYPE("as"));
```

### Comparing `lbkit-0.5.3/lbkit/codegen/template/public.h.mako` & `lbkit-0.5.5/lbkit/codegen/template/public.h.mako`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 enum _${name} {
     % for value in enum.values.parameters:
     ${name}_${value.name},
     % endfor
     _${name}Invalid,
 };
 
+const gchar *${name}_as_string(${name} value);
+
 % endfor
 % for name, dictionary in intf.dictionaries.items():
 
 /* ${dictionary.description} */
 struct _${name}${dictionary.key} {
     % for value in dictionary.values.parameters:
         % for line in value.declare():
@@ -78,15 +80,15 @@
 /* Create a new ${name} object */
 ${name} *${name}_new(void);
 
 % endfor
 
 ## 定义结构体编解码和释放函数
 % for name, stru in intf.structures.items():
-/* ${name} dictionary object */
+/* ${name} structure object */
 /* START: 结构体${name}及其数组类型的序列化、反序列化、释放函数 */
 GVariant *${name}_encode(const ${name} *value);
 ${name} *${name}_decode(GVariant *in);
 // Clean up the memory of structure and it's all members, `*value` will to NULL
 void ${name}_free(${name} **value);
 // Clean up the memory of members managed by structure ${name}
 void ${name}_clean(${name} *value);
```

### Comparing `lbkit-0.5.3/lbkit/codegen/template/server.h.mako` & `lbkit-0.5.5/lbkit/codegen/template/server.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/component/arg_parser.py` & `lbkit-0.5.5/lbkit/component/arg_parser.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/component/build.py` & `lbkit-0.5.5/lbkit/component/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         self.verbose = False if self.options.summary else True
         self.from_source = self.options.from_source
         # 当前组件及其依赖将被部署到rootfs目录
         self.rootfs_dir = os.path.join(cwd, ".temp", "rootfs")
         shutil.rmtree(self.rootfs_dir, ignore_errors=True)
         os.makedirs(self.rootfs_dir, exist_ok=True)
 
+        self.pkg = None
         self.gen_conaninfo()
         self.base_cmd = f" --user {self.user} --channel {self.channel}"
         self.base_cmd += f" -pr {self.profile} -s build_type={self.build_type} -r " + self.options.remote
         self.base_cmd += f" -pr:b {self.profile_build}"
         if self.options.cov:
             self.base_cmd += f" -o {self.name}/*:gcov=True"
         if self.options.test:
@@ -104,14 +105,15 @@
         fp.close()
         self.user = pkg.get("user")
         if self.user is None:
             raise errors.PackageConfigException("metadata/package.yml未正确配置user字段")
         # 构建命令未指定channel时从package.yml中读取
         pkg["channel"] = self.channel
         pkg["version"] = self.get_package_version()
+        self.pkg = pkg
         # 从package.yml加载基础信息
         self.name = pkg.get("name")
         self.version = pkg.get("version")
 
         self.package = self.name + "/" + self.version + \
             "@" + self.user + "/" + self.channel
         # 准备部署依赖
@@ -152,15 +154,15 @@
     def _build_dependencies(self):
         log.success(f"start build dependeicies package of {self.package}")
         if self.from_source:
             return
         # 生成部署deploy命令
         lookup = TemplateLookup(directories=os.path.join(lb_cwd, "template"))
         template = lookup.get_template("deploy.mako")
-        deploy = template.render(lookup=lookup, packages=self.runtime_packages)
+        deploy = template.render(lookup=lookup, pkg=self.pkg, packages=self.runtime_packages)
         dir = os.path.join(cwd, ".temp", "deploy")
         # 创建临时目录并写入conanfile.py文件
         os.makedirs(dir, exist_ok=True)
         conanfile = os.path.join(dir, "conanfile.py")
         fp = open(conanfile, "w")
         fp.write(deploy)
         fp.close()
@@ -174,15 +176,15 @@
     def deploy(self):
         log.success(f"start deplay {self.package} and it's dependencies to ./temp/rootfs")
         # 生成部署deploy命令
         lookup = TemplateLookup(directories=os.path.join(lb_cwd, "template"))
         template = lookup.get_template("deploy.mako")
         packages = self.runtime_packages
         packages.append(self.package)
-        deploy = template.render(lookup=lookup, packages=packages)
+        deploy = template.render(lookup=lookup, pkg=self.pkg, packages=packages)
         dir = os.path.join(cwd, ".temp", "deploy")
         # 创建临时目录并写入conanfile.py文件
         os.makedirs(dir, exist_ok=True)
         conanfile = os.path.join(dir, "conanfile.py")
         fp = open(conanfile, "w")
         fp.write(deploy)
         fp.close()
@@ -198,15 +200,32 @@
             id = info.get("package_id")
             dep = DeployComponent(ref, id, self.rootfs_dir)
             dep.run()
 
         # 设置ROOTFS_DIR环境变量，为DT测试提供相对路径
         os.environ["ROOTFS_DIR"] = self.rootfs_dir
 
+    def _validate_odf_files(self):
+        odf_dirs = self.pkg.get("odf_dirs", [])
+        for dir in odf_dirs:
+            for filename in os.listdir(dir):
+                filename = os.path.join(dir, filename)
+                if not os.path.isfile(filename):
+                    continue
+                if not filename.endswith(".yaml"):
+                    log.debug(f"file {filename} not endswith .yaml, skip validate")
+                    continue
+
+                log.info(f"start validate {filename}")
+                validate_yml_with_json_schema(filename, "/usr/share/litebmc/schema/odf.v1.json")
+
     def run(self):
+        # start validate all odf(Object Description file) files
+        self._validate_odf_files()
+
         cmd = f"conan remove {self.package} -c"
         tools.exec(cmd)
         gen = CodeGen([])
         gen.run("./metadata/package.yml")
         self._build_dependencies()
         log.success(f"start build {self.package}")
         cmd = "conan create . {} -tf=\"\"".format(self.base_cmd)
```

### Comparing `lbkit-0.5.3/lbkit/component/template/conanbase.mako` & `lbkit-0.5.5/lbkit/component/template/conanbase.mako`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,36 @@
             self.requires("${conan.get("conan")}")
             % endif
         % endfor
     % endif
 % endif
         pass
 
+    def configure(self):
+% if len(pkg.get("requires", {})) > 0:
+    % for conan in pkg["requires"].get("compile", []):
+        % if conan.get("option") is not None:
+            % for k, v in conan.get("option").items():
+        self.options["${conan.get("conan").split("/")[0]}"].${k} = ${("\"" + v + "\"") if isinstance(v, str) else str(v)}
+            % endfor
+        % endif
+    % endfor
+<%test_requires=pkg["requires"].get("test", [])%>\
+    % if len(test_requires):
+        % for conan in test_requires:
+            % if conan.get("option") is not None:
+                % for k, v in conan.get("option").items():
+        self.options["${conan.get("conan").split("/")[0]}"].${k} = ${("\"" + v + "\"") if isinstance(v, str) else str(v)}
+                % endfor
+            % endif
+        % endfor
+    % endif
+% endif
+        pass
+
     def _append_default_flags(self):
         flags = []
         if self.options.gcov:
             flags.append("-fprofile-arcs")
             flags.append("-ftest-coverage")
         if self.settings.build_type == "Release" and self.settings.arch == "armv8":
             flags.append("-D_FORTIFY_SOURCE=2")
```

### Comparing `lbkit-0.5.3/lbkit/component/test.py` & `lbkit-0.5.5/lbkit/component/test.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/errors.py` & `lbkit-0.5.5/lbkit/errors.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/helper.py` & `lbkit-0.5.5/lbkit/helper.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/build_manifest.py` & `lbkit-0.5.5/lbkit/integration/build_manifest.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/build_prepare.py` & `lbkit-0.5.5/lbkit/integration/build_prepare.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/build_rootfs.py` & `lbkit-0.5.5/lbkit/integration/build_rootfs.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/config.py` & `lbkit-0.5.5/lbkit/integration/config.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/task.py` & `lbkit-0.5.5/lbkit/integration/task.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/integration/template/conanfile.py.mako` & `lbkit-0.5.5/lbkit/integration/template/conanfile.py.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/log.py` & `lbkit-0.5.5/lbkit/log.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit/misc.py` & `lbkit-0.5.5/lbkit/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,8 +74,10 @@
             tmp = fp.read()
             schema = json.loads(tmp)
     try:
         fp = open(yml_file, "r")
         data = yaml.safe_load(fp)
         validate(data, schema)
     except ValidationError as exc:
-        raise PackageConfigException(f"validate {yml_file} failed, schema file is {schema_file}, message: {exc.message}")
+        raise PackageConfigException(f"validate {yml_file} failed, schema file is {schema_file}, "
+                                     f"message: {exc.message}\n"
+                                     "installing redhat.vscode-yaml plugin in vscode will help you write odf files")
```

### Comparing `lbkit-0.5.3/lbkit/tools.py` & `lbkit-0.5.5/lbkit/tools.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/lbkit.egg-info/PKG-INFO` & `lbkit-0.5.5/lbkit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.3
+Version: 0.5.5
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.3/lbkit.egg-info/SOURCES.txt` & `lbkit-0.5.5/lbkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.3/setup.py` & `lbkit-0.5.5/setup.py`

 * *Files identical despite different names*

