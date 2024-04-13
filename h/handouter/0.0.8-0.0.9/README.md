# Comparing `tmp/handouter-0.0.8.tar.gz` & `tmp/handouter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handouter-0.0.8.tar", last modified: Thu Jan  4 13:35:46 2024, max compression
+gzip compressed data, was "handouter-0.0.9.tar", last modified: Sat Apr 13 20:46:01 2024, max compression
```

## Comparing `handouter-0.0.8.tar` & `handouter-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-01-04 13:35:46.237527 handouter-0.0.8/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1061 2023-12-16 16:20:04.000000 handouter-0.0.8/LICENSE.md
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      790 2024-01-04 13:35:46.236012 handouter-0.0.8/PKG-INFO
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1081 2024-01-03 13:30:12.000000 handouter-0.0.8/README.md
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-01-04 13:35:46.223834 handouter-0.0.8/handouter/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2023-12-16 15:58:36.000000 handouter-0.0.8/handouter/__init__.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     8509 2024-01-04 12:01:41.000000 handouter-0.0.8/handouter/__main__.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     2604 2024-01-04 12:03:37.000000 handouter-0.0.8/handouter/gen.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1326 2023-12-21 09:23:20.000000 handouter-0.0.8/handouter/tex_internals.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      531 2023-12-21 13:14:21.000000 handouter-0.0.8/handouter/utils.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       21 2024-01-04 12:02:44.000000 handouter-0.0.8/handouter/version.py
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-01-04 13:35:46.234308 handouter-0.0.8/handouter.egg-info/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      790 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/PKG-INFO
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      357 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/SOURCES.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        1 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/dependency_links.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       79 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/entry_points.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       32 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/requires.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       10 2024-01-04 13:35:46.000000 handouter-0.0.8/handouter.egg-info/top_level.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       38 2024-01-04 13:35:46.237617 handouter-0.0.8/setup.cfg
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1233 2023-12-21 13:11:48.000000 handouter-0.0.8/setup.py
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-04-13 20:46:01.782559 handouter-0.0.9/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1061 2024-03-05 21:26:15.000000 handouter-0.0.9/LICENSE.md
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      790 2024-04-13 20:46:01.782382 handouter-0.0.9/PKG-INFO
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1081 2024-03-05 21:26:15.000000 handouter-0.0.9/README.md
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-04-13 20:46:01.781330 handouter-0.0.9/handouter/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-03-05 21:26:16.000000 handouter-0.0.9/handouter/__init__.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     8674 2024-04-13 20:44:16.000000 handouter-0.0.9/handouter/__main__.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     2604 2024-03-05 21:26:16.000000 handouter-0.0.9/handouter/gen.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1326 2024-03-05 21:26:16.000000 handouter-0.0.9/handouter/tex_internals.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      531 2024-03-05 21:26:16.000000 handouter-0.0.9/handouter/utils.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       21 2024-04-13 20:45:40.000000 handouter-0.0.9/handouter/version.py
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2024-04-13 20:46:01.782126 handouter-0.0.9/handouter.egg-info/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      790 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/PKG-INFO
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      357 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/SOURCES.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        1 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/dependency_links.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       79 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/entry_points.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       32 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/requires.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       10 2024-04-13 20:46:01.000000 handouter-0.0.9/handouter.egg-info/top_level.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       38 2024-04-13 20:46:01.782616 handouter-0.0.9/setup.cfg
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1233 2024-03-05 21:26:15.000000 handouter-0.0.9/setup.py
```

### Comparing `handouter-0.0.8/LICENSE.md` & `handouter-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `handouter-0.0.8/PKG-INFO` & `handouter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handouter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Handouter is a script that wraps tectonic to generate handouts for [Chgk](https://en.wikipedia.org/wiki/What%3F_Where%3F_When%3F)
 Home-page: https://gitlab.com/peczony/handouter
 Author: Alexander Pecheny
 Author-email: ap@pecheny.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `handouter-0.0.8/README.md` & `handouter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `handouter-0.0.8/handouter/__main__.py` & `handouter-0.0.9/handouter/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     RESERVED_WORDS = [
         "image",
         "for_question",
         "columns",
         "rows",
         "resize_image",
         "font_size",
+        "font_family",
         "no_center",
         "raw_tex",
     ]
     SPACE = 1.5  # mm
 
     def __init__(self, args):
         self.args = args
@@ -93,16 +94,19 @@
         else:
             align = ", align=center"
         textwidth = ", text width=\\boxwidthinner"
         fs = block.get("font_size") or self.args.font_size
         fontsize = "\\fontsize{FSpt}{LHpt}\\selectfont ".replace("FS", str(fs)).replace(
             "LH", str(math.floor(fs * 1.2))
         )
+        contents = block["contents"]
+        if block.get("font_family"):
+            contents = "\\fontspec{" + block["font_family"] + "}" + contents
         return (
-            TIKZBOX_INNER.replace("<CONTENTS>", block["contents"])
+            TIKZBOX_INNER.replace("<CONTENTS>", contents)
             .replace("<ALIGN>", align)
             .replace("<TEXTWIDTH>", textwidth)
             .replace("<FONTSIZE>", fontsize)
         )
 
     def get_page_width(self):
         return self.args.paperwidth - self.args.margin_left - self.args.margin_right - 2
```

### Comparing `handouter-0.0.8/handouter/gen.py` & `handouter-0.0.9/handouter/gen.py`

 * *Files identical despite different names*

### Comparing `handouter-0.0.8/handouter/tex_internals.py` & `handouter-0.0.9/handouter/tex_internals.py`

 * *Files identical despite different names*

### Comparing `handouter-0.0.8/handouter/utils.py` & `handouter-0.0.9/handouter/utils.py`

 * *Files identical despite different names*

### Comparing `handouter-0.0.8/handouter.egg-info/PKG-INFO` & `handouter-0.0.9/handouter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handouter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Handouter is a script that wraps tectonic to generate handouts for [Chgk](https://en.wikipedia.org/wiki/What%3F_Where%3F_When%3F)
 Home-page: https://gitlab.com/peczony/handouter
 Author: Alexander Pecheny
 Author-email: ap@pecheny.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `handouter-0.0.8/setup.py` & `handouter-0.0.9/setup.py`

 * *Files identical despite different names*

