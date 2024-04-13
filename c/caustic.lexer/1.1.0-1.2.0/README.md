# Comparing `tmp/caustic.lexer-1.1.0.tar.gz` & `tmp/caustic.lexer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.lexer-1.1.0.tar", last modified: Fri Apr 12 22:42:50 2024, max compression
+gzip compressed data, was "caustic.lexer-1.2.0.tar", last modified: Sat Apr 13 00:10:49 2024, max compression
```

## Comparing `caustic.lexer-1.1.0.tar` & `caustic.lexer-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 22:42:50.510379 caustic.lexer-1.1.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.1.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     7136 2024-04-12 22:42:50.510379 caustic.lexer-1.1.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     6204 2024-04-12 22:11:51.000000 caustic.lexer-1.1.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-12 21:41:50.000000 caustic.lexer-1.1.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 22:42:50.510379 caustic.lexer-1.1.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 22:42:50.500378 caustic.lexer-1.1.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 22:42:50.500378 caustic.lexer-1.1.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 22:42:50.510379 caustic.lexer-1.1.0/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.1.0/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.1.0/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.1.0/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1374 2024-04-12 21:35:57.000000 caustic.lexer-1.1.0/src/caustic/lexer/grammar.cag
--rw-r--r--   0 shae      (1000) shae      (1000)    13068 2024-04-12 21:22:22.000000 caustic.lexer-1.1.0/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3257 2024-04-12 21:56:34.000000 caustic.lexer-1.1.0/src/caustic/lexer/precompiled_nodes.pkl
--rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.1.0/src/caustic/lexer/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.1.0/src/caustic/lexer/util.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 22:42:50.510379 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     7136 2024-04-12 22:42:50.000000 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-12 22:42:50.000000 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 22:42:50.000000 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 22:42:50.000000 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 22:42:50.000000 caustic.lexer-1.1.0/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:10:49.886871 caustic.lexer-1.2.0/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.2.0/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     7389 2024-04-13 00:10:49.886871 caustic.lexer-1.2.0/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     6457 2024-04-12 23:41:08.000000 caustic.lexer-1.2.0/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-12 23:38:21.000000 caustic.lexer-1.2.0/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-13 00:10:49.886871 caustic.lexer-1.2.0/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:10:49.880205 caustic.lexer-1.2.0/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:10:49.880205 caustic.lexer-1.2.0/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:10:49.886871 caustic.lexer-1.2.0/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.2.0/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.2.0/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.2.0/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1377 2024-04-12 23:40:42.000000 caustic.lexer-1.2.0/src/caustic/lexer/grammar.cag
+-rw-r--r--   0 shae      (1000) shae      (1000)    14142 2024-04-12 23:45:20.000000 caustic.lexer-1.2.0/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3260 2024-04-13 00:10:46.000000 caustic.lexer-1.2.0/src/caustic/lexer/precompiled_nodes.pkl
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.2.0/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.2.0/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:10:49.886871 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     7389 2024-04-13 00:10:49.000000 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-13 00:10:49.000000 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-13 00:10:49.000000 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-13 00:10:49.000000 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-13 00:10:49.000000 caustic.lexer-1.2.0/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic.lexer-1.1.0/LICENSE` & `caustic.lexer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/PKG-INFO` & `caustic.lexer-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -81,26 +81,32 @@
 
 Note: `basic_compiler` will not accept node names with periods
 
 #### Anonymous
 "Anonymous" named nodes are expressions prefixed with `:`, but with
 no leading name
 
+#### Unpack
+"Unpack" nodes are expressions prefixed with `^:`
+
+Note: `basic_compiler` will not accept unpack nodes
+
 ### Group
 > `nodes.NodeGroup`
 
 The top level of an expression is implicitly grouped
 
 A simple group node is opened by `(` and closed by `)`  
 Groups match the nodes inside of them in a sequence in order  
 The return value of this group will be dependent on its contents' [naming](#naming):
 
 - A group containing no named nodes will return a list of its nodes' results
 - A group containing nodes with "[anonymous](#anonymous)" names returns the last matched anonymous nodes' return value
 - A group containing [named](#naming) nodes returns a dict containing a mapping of the names to the nodes' results
+- Any [unpack](#unpack) nodes will unpack either their elements (sequence) or their names and values into the surrounding group's result
 
 Mixing anonymous and named expressions in a single group will result in an error
 
 #### Whitespace sensitive group
 > `nodes.NodeGroup`, `keep_whitespace=True`
 
 A whitespace sensitive group is opened by `{` and closed by `}`
```

### Comparing `caustic.lexer-1.1.0/README.md` & `caustic.lexer-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,32 @@
 
 Note: `basic_compiler` will not accept node names with periods
 
 #### Anonymous
 "Anonymous" named nodes are expressions prefixed with `:`, but with
 no leading name
 
+#### Unpack
+"Unpack" nodes are expressions prefixed with `^:`
+
+Note: `basic_compiler` will not accept unpack nodes
+
 ### Group
 > `nodes.NodeGroup`
 
 The top level of an expression is implicitly grouped
 
 A simple group node is opened by `(` and closed by `)`  
 Groups match the nodes inside of them in a sequence in order  
 The return value of this group will be dependent on its contents' [naming](#naming):
 
 - A group containing no named nodes will return a list of its nodes' results
 - A group containing nodes with "[anonymous](#anonymous)" names returns the last matched anonymous nodes' return value
 - A group containing [named](#naming) nodes returns a dict containing a mapping of the names to the nodes' results
+- Any [unpack](#unpack) nodes will unpack either their elements (sequence) or their names and values into the surrounding group's result
 
 Mixing anonymous and named expressions in a single group will result in an error
 
 #### Whitespace sensitive group
 > `nodes.NodeGroup`, `keep_whitespace=True`
 
 A whitespace sensitive group is opened by `{` and closed by `}`
```

### Comparing `caustic.lexer-1.1.0/pyproject.toml` & `caustic.lexer-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "1.1.0"
+version = "1.2.0"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
```

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/__init__.py` & `caustic.lexer-1.2.0/src/caustic/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/basic_compiler.py` & `caustic.lexer-1.2.0/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/compiler.py` & `caustic.lexer-1.2.0/src/caustic/lexer/compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/grammar.cag` & `caustic.lexer-1.2.0/src/caustic/lexer/grammar.cag`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Statements / comments
 COMMENT = "#" ! /.*?$/m ;
 STATEMENT = name:1/([\w\.]+)/ "=" ! expr: - @EXPRESSION ";" ;
 PRAGMA = "$" type:0/\w+/ args:1/(.*?)$/m ;
 
 # Expression supergroup
-EXPRESSION = name:1/(?:([\w\.]*):)?/ expr:[
+EXPRESSION = name:1/(?:(\^|[\w\.]*):)?/ expr:[
     ( type:<"group"> val:@NODE_GROUP )
     ( type:<"group_ws_sensitive"> val:@NODE_GROUP_WS_SENSITIVE )
     ( type:<"union"> val:@NODE_UNION )
     ( type:<"range"> val:@NODE_RANGE )
     ( type:<"range_ws_sensitive"> val:@NODE_RANGE_WS_SENSITIVE )
     ( type:<"string"> val:@STRING_NODE )
     ( type:<"pattern"> val:@PATTERN_NODE )
```

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/nodes.py` & `caustic.lexer-1.2.0/src/caustic/lexer/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,36 @@
                 assert not stealer
                 bm.load_pos(save)
                 return NO_MATCH
             # Check how we should return results
             if n.name is None: # not assigned a name ("[name]:<node>")
                 if isinstance(results, dict): continue # don't add it
                 if not single_result: results.append(res)
+            elif n.name == b'^': # unpack name
+                if single_result:
+                    te = TypeError(f'Conflicting return types: unpack result cannot be added to single result')
+                    te.add_note(str(n))
+                    te.add_note(f'In {self}')
+                    raise te
+                if isinstance(res, dict):
+                    if not isinstance(results, dict):
+                        results = {}
+                    results.update(res)
+                elif isinstance(res, cabc.Sequence):
+                    if isinstance(results, dict):
+                        te = TypeError(f'Conflicting return types: cannot unpack sequence result into named results')
+                        te.add_note(str(n))
+                        te.add_note(f'In {self}')
+                        raise te
+                    results.extend(res)
+                else:
+                    te = TypeError(f'Cannot unpack return {res!r}')
+                    te.add_note(str(n))
+                    te.add_note(f'In {self}')
+                    raise te
             elif n.name: # name is not blank ("<name>:<node>")
                 if isinstance(results, dict):
                     results[n.name] = res
                 elif single_result:
                     te = TypeError(f'Conflicting return types: named result {n.name} cannot be added to single result')
                     te.add_note(str(n))
                     te.add_note(f'In {self}')
```

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/precompiled_nodes.pkl` & `caustic.lexer-1.2.0/src/caustic/lexer/precompiled_nodes.pkl`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95ae 0c00 0000 0000 0028 4307 434f  ...........(C.CO
+00000000: 8004 95b1 0c00 0000 0000 0028 4307 434f  ...........(C.CO
 00000010: 4d4d 454e 544b 0251 2981 4e7d 288c 056e  MMENTK.Q).N}(..n
 00000020: 6f64 6573 944b 0551 2981 4e7d 288c 0673  odes.K.Q).N}(..s
 00000030: 7472 696e 6794 4301 238c 046e 616d 6594  tring.C.#..name.
 00000040: 4e75 8662 4b07 5129 814e 7d68 024e 7386  Nu.bK.Q).N}h.Ns.
 00000050: 624b 0651 2981 4e7d 288c 0770 6174 7465  bK.Q).N}(..patte
 00000060: 726e 948c 0272 658c 085f 636f 6d70 696c  rn...re.._compil
 00000070: 6593 9443 042e 2a3f 244b 0886 528c 0567  e..C..*?$K..R..g
@@ -16,189 +16,189 @@
 000000f0: 0143 013d 6802 4e75 8662 4b07 5129 814e  .C.=h.Nu.bK.Q).N
 00000100: 7d68 024e 7386 624b 0451 2981 4e7d 288c  }h.Ns.bK.Q).N}(.
 00000110: 036d 696e 944b 008c 036d 6178 944e 8c04  .min.K...max.N..
 00000120: 6e6f 6465 944b 0951 2981 4e7d 288c 0b74  node.K.Q).N}(..t
 00000130: 6172 6765 745f 6e61 6d65 9443 0a45 5850  arget_name.C.EXP
 00000140: 5245 5353 494f 4e8c 0674 6172 6765 7494  RESSION..target.
 00000150: 4b02 5129 8194 4e7d 2868 004b 0651 2981  K.Q)..N}(h.K.Q).
-00000160: 4e7d 2868 0368 0443 0f28 3f3a 285b 5c77  N}(h.h.C.(?:([\w
-00000170: 5c2e 5d2a 293a 293f 4b00 8652 6805 4b01  \.]*):)?K..Rh.K.
-00000180: 6802 8c04 6e61 6d65 7586 624b 0351 2981  h...nameu.bK.Q).
-00000190: 4e7d 2868 0028 4b02 5129 814e 7d28 6800  N}(h.(K.Q).N}(h.
-000001a0: 4b08 5129 814e 7d28 8c03 7661 6c94 4305  K.Q).N}(..val.C.
-000001b0: 6772 6f75 7068 028c 0474 7970 6575 8662  grouph...typeu.b
-000001c0: 4b09 5129 814e 7d28 680a 430a 4e4f 4445  K.Q).N}(h.C.NODE
-000001d0: 5f47 524f 5550 680b 4e68 028c 0376 616c  _GROUPh.Nh...val
-000001e0: 7586 6286 6806 8968 024e 7586 624b 0251  u.b.h..h.Nu.bK.Q
-000001f0: 2981 4e7d 2868 004b 0851 2981 4e7d 2868  ).N}(h.K.Q).N}(h
-00000200: 0d43 1267 726f 7570 5f77 735f 7365 6e73  .C.group_ws_sens
-00000210: 6974 6976 6568 028c 0474 7970 6575 8662  itiveh...typeu.b
-00000220: 4b09 5129 814e 7d28 680a 4317 4e4f 4445  K.Q).N}(h.C.NODE
-00000230: 5f47 524f 5550 5f57 535f 5345 4e53 4954  _GROUP_WS_SENSIT
-00000240: 4956 4568 0b4e 6802 8c03 7661 6c75 8662  IVEh.Nh...valu.b
-00000250: 8668 0689 6802 4e75 8662 4b02 5129 814e  .h..h.Nu.bK.Q).N
-00000260: 7d28 6800 4b08 5129 814e 7d28 680d 4305  }(h.K.Q).N}(h.C.
-00000270: 756e 696f 6e68 028c 0474 7970 6575 8662  unionh...typeu.b
-00000280: 4b09 5129 814e 7d28 680a 430a 4e4f 4445  K.Q).N}(h.C.NODE
-00000290: 5f55 4e49 4f4e 680b 4e68 028c 0376 616c  _UNIONh.Nh...val
-000002a0: 7586 6286 6806 8968 024e 7586 624b 0251  u.b.h..h.Nu.bK.Q
-000002b0: 2981 4e7d 2868 004b 0851 2981 4e7d 2868  ).N}(h.K.Q).N}(h
-000002c0: 0d43 0572 616e 6765 6802 8c04 7479 7065  .C.rangeh...type
-000002d0: 7586 624b 0951 2981 4e7d 2868 0a43 0a4e  u.bK.Q).N}(h.C.N
-000002e0: 4f44 455f 5241 4e47 4568 0b4e 6802 8c03  ODE_RANGEh.Nh...
-000002f0: 7661 6c75 8662 8668 0689 6802 4e75 8662  valu.b.h..h.Nu.b
-00000300: 4b02 5129 814e 7d28 6800 4b08 5129 814e  K.Q).N}(h.K.Q).N
-00000310: 7d28 680d 4312 7261 6e67 655f 7773 5f73  }(h.C.range_ws_s
-00000320: 656e 7369 7469 7665 6802 8c04 7479 7065  ensitiveh...type
-00000330: 7586 624b 0951 2981 4e7d 2868 0a43 174e  u.bK.Q).N}(h.C.N
-00000340: 4f44 455f 5241 4e47 455f 5753 5f53 454e  ODE_RANGE_WS_SEN
-00000350: 5349 5449 5645 680b 4e68 028c 0376 616c  SITIVEh.Nh...val
-00000360: 7586 6286 6806 8968 024e 7586 624b 0251  u.b.h..h.Nu.bK.Q
-00000370: 2981 4e7d 2868 004b 0851 2981 4e7d 2868  ).N}(h.K.Q).N}(h
-00000380: 0d43 0673 7472 696e 6768 028c 0474 7970  .C.stringh...typ
-00000390: 6575 8662 4b09 5129 814e 7d28 680a 430b  eu.bK.Q).N}(h.C.
-000003a0: 5354 5249 4e47 5f4e 4f44 4568 0b4e 6802  STRING_NODEh.Nh.
-000003b0: 8c03 7661 6c75 8662 8668 0689 6802 4e75  ..valu.b.h..h.Nu
-000003c0: 8662 4b02 5129 814e 7d28 6800 4b08 5129  .bK.Q).N}(h.K.Q)
-000003d0: 814e 7d28 680d 4307 7061 7474 6572 6e68  .N}(h.C.patternh
-000003e0: 028c 0474 7970 6575 8662 4b09 5129 814e  ...typeu.bK.Q).N
-000003f0: 7d28 680a 430c 5041 5454 4552 4e5f 4e4f  }(h.C.PATTERN_NO
-00000400: 4445 680b 4e68 028c 0376 616c 7586 6286  DEh.Nh...valu.b.
-00000410: 6806 8968 024e 7586 624b 0251 2981 4e7d  h..h.Nu.bK.Q).N}
-00000420: 2868 004b 0851 2981 4e7d 2868 0d43 0773  (h.K.Q).N}(h.C.s
-00000430: 7465 616c 6572 6802 8c04 7479 7065 7586  tealerh...typeu.
-00000440: 624b 0951 2981 4e7d 2868 0a43 0753 5445  bK.Q).N}(h.C.STE
-00000450: 414c 4552 680b 4e68 024e 7586 6286 6806  ALERh.Nh.Nu.b.h.
-00000460: 8968 024e 7586 624b 0251 2981 4e7d 2868  .h.Nu.bK.Q).N}(h
-00000470: 004b 0851 2981 4e7d 2868 0d43 0763 6f6e  .K.Q).N}(h.C.con
-00000480: 7465 7874 6802 8c04 7479 7065 7586 624b  texth...typeu.bK
-00000490: 0951 2981 4e7d 2868 0a43 0743 4f4e 5445  .Q).N}(h.C.CONTE
-000004a0: 5854 680b 4e68 028c 0376 616c 7586 6286  XTh.Nh...valu.b.
-000004b0: 6806 8968 024e 7586 624b 0251 2981 4e7d  h..h.Nu.bK.Q).N}
-000004c0: 2868 004b 0851 2981 4e7d 2868 0d43 076e  (h.K.Q).N}(h.C.n
-000004d0: 6f64 6572 6566 6802 8c04 7479 7065 7586  oderefh...typeu.
-000004e0: 624b 0951 2981 4e7d 2868 0a43 074e 4f44  bK.Q).N}(h.C.NOD
-000004f0: 4552 4546 680b 4e68 028c 0376 616c 7586  EREFh.Nh...valu.
-00000500: 6286 6806 8968 024e 7586 6274 6802 8c04  b.h..h.Nu.bth...
-00000510: 6578 7072 7586 6286 6806 8968 024e 7586  expru.b.h..h.Nu.
-00000520: 6268 024e 7586 6268 0689 6802 8c04 6578  bh.Nu.bh..h...ex
-00000530: 7072 7586 624b 0551 2981 4e7d 2868 0143  pru.bK.Q).N}(h.C
-00000540: 013b 6802 4e75 8662 7468 0689 6802 4e75  .;h.Nu.bth..h.Nu
-00000550: 8662 8643 0650 5241 474d 414b 0251 2981  .b.C.PRAGMAK.Q).
-00000560: 4e7d 2868 004b 0551 2981 4e7d 2868 0143  N}(h.K.Q).N}(h.C
-00000570: 0124 6802 4e75 8662 4b06 5129 814e 7d28  .$h.Nu.bK.Q).N}(
-00000580: 6803 6804 4303 5c77 2b4b 0086 5268 054b  h.h.C.\w+K..Rh.K
-00000590: 0068 028c 0474 7970 6575 8662 4b06 5129  .h...typeu.bK.Q)
-000005a0: 814e 7d28 6803 6804 4306 282e 2a3f 2924  .N}(h.h.C.(.*?)$
-000005b0: 4b08 8652 6805 4b01 6802 8c04 6172 6773  K..Rh.K.h...args
-000005c0: 7586 6287 6806 8968 024e 7586 6286 430a  u.b.h..h.Nu.b.C.
-000005d0: 4558 5052 4553 5349 4f4e 680c 8643 0a4e  EXPRESSIONh..C.N
-000005e0: 4f44 455f 4752 4f55 504b 0251 2981 4e7d  ODE_GROUPK.Q).N}
-000005f0: 2868 0028 4b05 5129 814e 7d28 6801 4301  (h.(K.Q).N}(h.C.
-00000600: 2868 024e 7586 624b 0751 2981 4e7d 6802  (h.Nu.bK.Q).N}h.
-00000610: 4e73 8662 4b04 5129 814e 7d28 6807 4b00  Ns.bK.Q).N}(h.K.
-00000620: 6808 4e68 094b 0951 2981 4e7d 2868 0a43  h.Nh.K.Q).N}(h.C
-00000630: 0a45 5850 5245 5353 494f 4e68 0b68 0c68  .EXPRESSIONh.h.h
-00000640: 024e 7586 6268 0689 6802 8c00 9475 8662  .Nu.bh..h....u.b
-00000650: 4b07 5129 814e 7d68 024e 7386 624b 0551  K.Q).N}h.Ns.bK.Q
-00000660: 2981 4e7d 2868 0143 0129 6802 4e75 8662  ).N}(h.C.)h.Nu.b
-00000670: 7468 0689 6802 4e75 8662 8643 174e 4f44  th..h.Nu.b.C.NOD
-00000680: 455f 4752 4f55 505f 5753 5f53 454e 5349  E_GROUP_WS_SENSI
-00000690: 5449 5645 4b02 5129 814e 7d28 6800 284b  TIVEK.Q).N}(h.(K
-000006a0: 0551 2981 4e7d 2868 0143 017b 6802 4e75  .Q).N}(h.C.{h.Nu
-000006b0: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
-000006c0: 0451 2981 4e7d 2868 074b 0068 084e 6809  .Q).N}(h.K.h.Nh.
-000006d0: 4b09 5129 814e 7d28 680a 430a 4558 5052  K.Q).N}(h.C.EXPR
-000006e0: 4553 5349 4f4e 680b 680c 6802 4e75 8662  ESSIONh.h.h.Nu.b
-000006f0: 6806 8968 0268 0e75 8662 4b07 5129 814e  h..h.h.u.bK.Q).N
-00000700: 7d68 024e 7386 624b 0551 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
-00000710: 0143 017d 6802 4e75 8662 7468 0689 6802  .C.}h.Nu.bth..h.
-00000720: 4e75 8662 8643 0a4e 4f44 455f 554e 494f  Nu.b.C.NODE_UNIO
-00000730: 4e4b 0251 2981 4e7d 2868 0028 4b05 5129  NK.Q).N}(h.(K.Q)
-00000740: 814e 7d28 6801 4301 5b68 024e 7586 624b  .N}(h.C.[h.Nu.bK
-00000750: 0751 2981 4e7d 6802 4e73 8662 4b04 5129  .Q).N}h.Ns.bK.Q)
-00000760: 814e 7d28 6807 4b00 6808 4e68 094b 0951  .N}(h.K.h.Nh.K.Q
-00000770: 2981 4e7d 2868 0a43 0a45 5850 5245 5353  ).N}(h.C.EXPRESS
-00000780: 494f 4e68 0b68 0c68 024e 7586 6268 0689  IONh.h.h.Nu.bh..
-00000790: 6802 680e 7586 624b 0751 2981 4e7d 6802  h.h.u.bK.Q).N}h.
-000007a0: 4e73 8662 4b05 5129 814e 7d28 6801 4301  Ns.bK.Q).N}(h.C.
-000007b0: 5d68 024e 7586 6274 6806 8968 024e 7586  ]h.Nu.bth..h.Nu.
-000007c0: 6286 430a 4e4f 4445 5f52 414e 4745 4b02  b.C.NODE_RANGEK.
-000007d0: 5129 814e 7d28 6800 284b 0651 2981 4e7d  Q).N}(h.(K.Q).N}
-000007e0: 2868 0368 0443 035c 642a 4b00 8652 9468  (h.h.C.\d*K..R.h
-000007f0: 054b 0068 028c 036d 696e 7586 624b 0551  .K.h...minu.bK.Q
-00000800: 2981 4e7d 2868 0143 012d 6802 4e75 8662  ).N}(h.C.-h.Nu.b
-00000810: 4b07 5129 814e 7d68 024e 7386 624b 0651  K.Q).N}h.Ns.bK.Q
-00000820: 2981 4e7d 2868 0368 0443 0628 5c64 2b29  ).N}(h.h.C.(\d+)
-00000830: 3f4b 0086 5294 6805 4b01 6802 8c03 6d61  ?K..R.h.K.h...ma
-00000840: 7875 8662 4b07 5129 814e 7d68 024e 7386  xu.bK.Q).N}h.Ns.
-00000850: 624b 0951 2981 4e7d 2868 0a43 0a45 5850  bK.Q).N}(h.C.EXP
-00000860: 5245 5353 494f 4e68 0b4e 6802 8c04 6e6f  RESSIONh.Nh...no
-00000870: 6465 7586 6274 6806 8968 024e 7586 6286  deu.bth..h.Nu.b.
-00000880: 4317 4e4f 4445 5f52 414e 4745 5f57 535f  C.NODE_RANGE_WS_
-00000890: 5345 4e53 4954 4956 454b 0251 2981 4e7d  SENSITIVEK.Q).N}
-000008a0: 2868 0028 4b06 5129 814e 7d28 6803 680f  (h.(K.Q).N}(h.h.
-000008b0: 6805 4b00 6802 8c03 6d69 6e75 8662 4b05  h.K.h...minu.bK.
-000008c0: 5129 814e 7d28 6801 4301 7e68 024e 7586  Q).N}(h.C.~h.Nu.
-000008d0: 624b 0751 2981 4e7d 6802 4e73 8662 4b06  bK.Q).N}h.Ns.bK.
-000008e0: 5129 814e 7d28 6803 6810 6805 4b01 6802  Q).N}(h.h.h.K.h.
-000008f0: 8c03 6d61 7875 8662 4b09 5129 814e 7d28  ..maxu.bK.Q).N}(
-00000900: 680a 430a 4558 5052 4553 5349 4f4e 680b  h.C.EXPRESSIONh.
-00000910: 4e68 028c 046e 6f64 6575 8662 7468 0689  Nh...nodeu.bth..
-00000920: 6802 4e75 8662 8643 0b53 5452 494e 475f  h.Nu.b.C.STRING_
-00000930: 4e4f 4445 4b02 5129 814e 7d28 6800 4b03  NODEK.Q).N}(h.K.
-00000940: 5129 814e 7d28 6800 4b02 5129 814e 7d28  Q).N}(h.K.Q).N}(
-00000950: 6800 284b 0551 2981 4e7d 2868 0143 0122  h.(K.Q).N}(h.C."
-00000960: 9468 024e 7586 624b 0751 2981 4e7d 6802  .h.Nu.bK.Q).N}h.
-00000970: 4e73 8662 4b06 5129 814e 7d28 6803 6804  Ns.bK.Q).N}(h.h.
-00000980: 4313 283f 3a5b 5e22 5c5c 5d7c 283f 3a5c  C.(?:[^"\\]|(?:\
-00000990: 5c2e 2929 2a4b 0086 5268 054b 0068 0268  \.))*K..Rh.K.h.h
-000009a0: 0e75 8662 4b05 5129 814e 7d28 6801 6811  .u.bK.Q).N}(h.h.
-000009b0: 6802 4e75 8662 7468 0689 6802 4e75 8662  h.Nu.bth..h.Nu.b
-000009c0: 4b02 5129 814e 7d28 6800 284b 0551 2981  K.Q).N}(h.(K.Q).
-000009d0: 4e7d 2868 0143 0127 9468 024e 7586 624b  N}(h.C.'.h.Nu.bK
-000009e0: 0751 2981 4e7d 6802 4e73 8662 4b06 5129  .Q).N}h.Ns.bK.Q)
-000009f0: 814e 7d28 6803 6804 4313 283f 3a5b 5e27  .N}(h.h.C.(?:[^'
-00000a00: 5c5c 5d7c 283f 3a5c 5c2e 2929 2a4b 0086  \\]|(?:\\.))*K..
-00000a10: 5268 054b 0068 0268 0e75 8662 4b05 5129  Rh.K.h.h.u.bK.Q)
-00000a20: 814e 7d28 6801 6812 6802 4e75 8662 7468  .N}(h.h.h.Nu.bth
-00000a30: 0689 6802 4e75 8662 8668 0268 0e75 8662  ..h.Nu.b.h.h.u.b
-00000a40: 8568 0689 6802 4e75 8662 8643 0c50 4154  .h..h.Nu.b.C.PAT
-00000a50: 5445 524e 5f4e 4f44 454b 0251 2981 4e7d  TERN_NODEK.Q).N}
-00000a60: 2868 0028 4b06 5129 814e 7d28 6803 6804  (h.(K.Q).N}(h.h.
-00000a70: 4306 285c 642a 293f 4b00 8652 6805 4b01  C.(\d*)?K..Rh.K.
-00000a80: 6802 8c05 6772 6f75 7075 8662 4b05 5129  h...groupu.bK.Q)
-00000a90: 814e 7d28 6801 4301 2f94 6802 4e75 8662  .N}(h.C./.h.Nu.b
-00000aa0: 4b07 5129 814e 7d68 024e 7386 624b 0651  K.Q).N}h.Ns.bK.Q
-00000ab0: 2981 4e7d 2868 0368 0443 1428 3f3a 5b5e  ).N}(h.h.C.(?:[^
-00000ac0: 5c2f 5c5c 5d7c 283f 3a5c 5c2e 2929 2a4b  \/\\]|(?:\\.))*K
-00000ad0: 0086 5268 054b 0068 028c 0770 6174 7465  ..Rh.K.h...patte
-00000ae0: 726e 7586 624b 0751 2981 4e7d 6802 4e73  rnu.bK.Q).N}h.Ns
-00000af0: 8662 4b05 5129 814e 7d28 6801 6813 6802  .bK.Q).N}(h.h.h.
-00000b00: 4e75 8662 4b07 5129 814e 7d68 024e 7386  Nu.bK.Q).N}h.Ns.
-00000b10: 624b 0651 2981 4e7d 2868 0368 0443 065b  bK.Q).N}(h.h.C.[
-00000b20: 696d 735d 2a4b 0086 5268 054b 0068 028c  ims]*K..Rh.K.h..
-00000b30: 0566 6c61 6773 7586 6274 6806 8968 024e  .flagsu.bth..h.N
-00000b40: 7586 6286 4307 5354 4541 4c45 524b 0251  u.b.C.STEALERK.Q
-00000b50: 2981 4e7d 2868 004b 0551 2981 4e7d 2868  ).N}(h.K.Q).N}(h
-00000b60: 0143 0121 6802 4e75 8662 8568 0689 6802  .C.!h.Nu.b.h..h.
-00000b70: 4e75 8662 8643 0743 4f4e 5445 5854 4b02  Nu.b.C.CONTEXTK.
-00000b80: 5129 814e 7d28 6800 284b 0551 2981 4e7d  Q).N}(h.(K.Q).N}
-00000b90: 2868 0143 013c 6802 4e75 8662 4b07 5129  (h.C.<h.Nu.bK.Q)
-00000ba0: 814e 7d68 024e 7386 624b 0351 2981 4e7d  .N}h.Ns.bK.Q).N}
-00000bb0: 2868 004b 0251 2981 4e7d 2868 004b 0951  (h.K.Q).N}(h.K.Q
-00000bc0: 2981 4e7d 2868 0a43 0b53 5452 494e 475f  ).N}(h.C.STRING_
-00000bd0: 4e4f 4445 680b 4e68 028c 0373 7472 7586  NODEh.Nh...stru.
-00000be0: 6285 6806 8968 024e 7586 624b 0251 2981  b.h..h.Nu.bK.Q).
-00000bf0: 4e7d 2868 004b 0651 2981 4e7d 2868 0368  N}(h.K.Q).N}(h.h
-00000c00: 0443 035c 772a 4b00 8652 6805 4b00 6802  .C.\w*K..Rh.K.h.
-00000c10: 8c03 7261 7775 8662 8568 0689 6802 4e75  ..rawu.b.h..h.Nu
-00000c20: 8662 8668 0268 0e75 8662 4b07 5129 814e  .b.h.h.u.bK.Q).N
-00000c30: 7d68 024e 7386 624b 0551 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
-00000c40: 0143 013e 6802 4e75 8662 7468 0689 6802  .C.>h.Nu.bth..h.
-00000c50: 4e75 8662 8643 074e 4f44 4552 4546 4b02  Nu.b.C.NODEREFK.
-00000c60: 5129 814e 7d28 6800 4b05 5129 814e 7d28  Q).N}(h.K.Q).N}(
-00000c70: 6801 4301 4068 024e 7586 624b 0751 2981  h.C.@h.Nu.bK.Q).
-00000c80: 4e7d 6802 4e73 8662 4b06 5129 814e 7d28  N}h.Ns.bK.Q).N}(
-00000c90: 6803 6804 4307 5b5c 775c 2e5d 2b4b 0086  h.h.C.[\w\.]+K..
-00000ca0: 5268 054b 0068 0268 0e75 8662 8768 0689  Rh.K.h.h.u.b.h..
-00000cb0: 6802 4e75 8662 8674 2e                   h.Nu.b.t.
+00000160: 4e7d 2868 0368 0443 1228 3f3a 285c 5e7c  N}(h.h.C.(?:(\^|
+00000170: 5b5c 775c 2e5d 2a29 3a29 3f4b 0086 5268  [\w\.]*):)?K..Rh
+00000180: 054b 0168 028c 046e 616d 6575 8662 4b03  .K.h...nameu.bK.
+00000190: 5129 814e 7d28 6800 284b 0251 2981 4e7d  Q).N}(h.(K.Q).N}
+000001a0: 2868 004b 0851 2981 4e7d 288c 0376 616c  (h.K.Q).N}(..val
+000001b0: 9443 0567 726f 7570 6802 8c04 7479 7065  .C.grouph...type
+000001c0: 7586 624b 0951 2981 4e7d 2868 0a43 0a4e  u.bK.Q).N}(h.C.N
+000001d0: 4f44 455f 4752 4f55 5068 0b4e 6802 8c03  ODE_GROUPh.Nh...
+000001e0: 7661 6c75 8662 8668 0689 6802 4e75 8662  valu.b.h..h.Nu.b
+000001f0: 4b02 5129 814e 7d28 6800 4b08 5129 814e  K.Q).N}(h.K.Q).N
+00000200: 7d28 680d 4312 6772 6f75 705f 7773 5f73  }(h.C.group_ws_s
+00000210: 656e 7369 7469 7665 6802 8c04 7479 7065  ensitiveh...type
+00000220: 7586 624b 0951 2981 4e7d 2868 0a43 174e  u.bK.Q).N}(h.C.N
+00000230: 4f44 455f 4752 4f55 505f 5753 5f53 454e  ODE_GROUP_WS_SEN
+00000240: 5349 5449 5645 680b 4e68 028c 0376 616c  SITIVEh.Nh...val
+00000250: 7586 6286 6806 8968 024e 7586 624b 0251  u.b.h..h.Nu.bK.Q
+00000260: 2981 4e7d 2868 004b 0851 2981 4e7d 2868  ).N}(h.K.Q).N}(h
+00000270: 0d43 0575 6e69 6f6e 6802 8c04 7479 7065  .C.unionh...type
+00000280: 7586 624b 0951 2981 4e7d 2868 0a43 0a4e  u.bK.Q).N}(h.C.N
+00000290: 4f44 455f 554e 494f 4e68 0b4e 6802 8c03  ODE_UNIONh.Nh...
+000002a0: 7661 6c75 8662 8668 0689 6802 4e75 8662  valu.b.h..h.Nu.b
+000002b0: 4b02 5129 814e 7d28 6800 4b08 5129 814e  K.Q).N}(h.K.Q).N
+000002c0: 7d28 680d 4305 7261 6e67 6568 028c 0474  }(h.C.rangeh...t
+000002d0: 7970 6575 8662 4b09 5129 814e 7d28 680a  ypeu.bK.Q).N}(h.
+000002e0: 430a 4e4f 4445 5f52 414e 4745 680b 4e68  C.NODE_RANGEh.Nh
+000002f0: 028c 0376 616c 7586 6286 6806 8968 024e  ...valu.b.h..h.N
+00000300: 7586 624b 0251 2981 4e7d 2868 004b 0851  u.bK.Q).N}(h.K.Q
+00000310: 2981 4e7d 2868 0d43 1272 616e 6765 5f77  ).N}(h.C.range_w
+00000320: 735f 7365 6e73 6974 6976 6568 028c 0474  s_sensitiveh...t
+00000330: 7970 6575 8662 4b09 5129 814e 7d28 680a  ypeu.bK.Q).N}(h.
+00000340: 4317 4e4f 4445 5f52 414e 4745 5f57 535f  C.NODE_RANGE_WS_
+00000350: 5345 4e53 4954 4956 4568 0b4e 6802 8c03  SENSITIVEh.Nh...
+00000360: 7661 6c75 8662 8668 0689 6802 4e75 8662  valu.b.h..h.Nu.b
+00000370: 4b02 5129 814e 7d28 6800 4b08 5129 814e  K.Q).N}(h.K.Q).N
+00000380: 7d28 680d 4306 7374 7269 6e67 6802 8c04  }(h.C.stringh...
+00000390: 7479 7065 7586 624b 0951 2981 4e7d 2868  typeu.bK.Q).N}(h
+000003a0: 0a43 0b53 5452 494e 475f 4e4f 4445 680b  .C.STRING_NODEh.
+000003b0: 4e68 028c 0376 616c 7586 6286 6806 8968  Nh...valu.b.h..h
+000003c0: 024e 7586 624b 0251 2981 4e7d 2868 004b  .Nu.bK.Q).N}(h.K
+000003d0: 0851 2981 4e7d 2868 0d43 0770 6174 7465  .Q).N}(h.C.patte
+000003e0: 726e 6802 8c04 7479 7065 7586 624b 0951  rnh...typeu.bK.Q
+000003f0: 2981 4e7d 2868 0a43 0c50 4154 5445 524e  ).N}(h.C.PATTERN
+00000400: 5f4e 4f44 4568 0b4e 6802 8c03 7661 6c75  _NODEh.Nh...valu
+00000410: 8662 8668 0689 6802 4e75 8662 4b02 5129  .b.h..h.Nu.bK.Q)
+00000420: 814e 7d28 6800 4b08 5129 814e 7d28 680d  .N}(h.K.Q).N}(h.
+00000430: 4307 7374 6561 6c65 7268 028c 0474 7970  C.stealerh...typ
+00000440: 6575 8662 4b09 5129 814e 7d28 680a 4307  eu.bK.Q).N}(h.C.
+00000450: 5354 4541 4c45 5268 0b4e 6802 4e75 8662  STEALERh.Nh.Nu.b
+00000460: 8668 0689 6802 4e75 8662 4b02 5129 814e  .h..h.Nu.bK.Q).N
+00000470: 7d28 6800 4b08 5129 814e 7d28 680d 4307  }(h.K.Q).N}(h.C.
+00000480: 636f 6e74 6578 7468 028c 0474 7970 6575  contexth...typeu
+00000490: 8662 4b09 5129 814e 7d28 680a 4307 434f  .bK.Q).N}(h.C.CO
+000004a0: 4e54 4558 5468 0b4e 6802 8c03 7661 6c75  NTEXTh.Nh...valu
+000004b0: 8662 8668 0689 6802 4e75 8662 4b02 5129  .b.h..h.Nu.bK.Q)
+000004c0: 814e 7d28 6800 4b08 5129 814e 7d28 680d  .N}(h.K.Q).N}(h.
+000004d0: 4307 6e6f 6465 7265 6668 028c 0474 7970  C.noderefh...typ
+000004e0: 6575 8662 4b09 5129 814e 7d28 680a 4307  eu.bK.Q).N}(h.C.
+000004f0: 4e4f 4445 5245 4668 0b4e 6802 8c03 7661  NODEREFh.Nh...va
+00000500: 6c75 8662 8668 0689 6802 4e75 8662 7468  lu.b.h..h.Nu.bth
+00000510: 028c 0465 7870 7275 8662 8668 0689 6802  ...expru.b.h..h.
+00000520: 4e75 8662 6802 4e75 8662 6806 8968 028c  Nu.bh.Nu.bh..h..
+00000530: 0465 7870 7275 8662 4b05 5129 814e 7d28  .expru.bK.Q).N}(
+00000540: 6801 4301 3b68 024e 7586 6274 6806 8968  h.C.;h.Nu.bth..h
+00000550: 024e 7586 6286 4306 5052 4147 4d41 4b02  .Nu.b.C.PRAGMAK.
+00000560: 5129 814e 7d28 6800 4b05 5129 814e 7d28  Q).N}(h.K.Q).N}(
+00000570: 6801 4301 2468 024e 7586 624b 0651 2981  h.C.$h.Nu.bK.Q).
+00000580: 4e7d 2868 0368 0443 035c 772b 4b00 8652  N}(h.h.C.\w+K..R
+00000590: 6805 4b00 6802 8c04 7479 7065 7586 624b  h.K.h...typeu.bK
+000005a0: 0651 2981 4e7d 2868 0368 0443 0628 2e2a  .Q).N}(h.h.C.(.*
+000005b0: 3f29 244b 0886 5268 054b 0168 028c 0461  ?)$K..Rh.K.h...a
+000005c0: 7267 7375 8662 8768 0689 6802 4e75 8662  rgsu.b.h..h.Nu.b
+000005d0: 8643 0a45 5850 5245 5353 494f 4e68 0c86  .C.EXPRESSIONh..
+000005e0: 430a 4e4f 4445 5f47 524f 5550 4b02 5129  C.NODE_GROUPK.Q)
+000005f0: 814e 7d28 6800 284b 0551 2981 4e7d 2868  .N}(h.(K.Q).N}(h
+00000600: 0143 0128 6802 4e75 8662 4b07 5129 814e  .C.(h.Nu.bK.Q).N
+00000610: 7d68 024e 7386 624b 0451 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
+00000620: 074b 0068 084e 6809 4b09 5129 814e 7d28  .K.h.Nh.K.Q).N}(
+00000630: 680a 430a 4558 5052 4553 5349 4f4e 680b  h.C.EXPRESSIONh.
+00000640: 680c 6802 4e75 8662 6806 8968 028c 0094  h.h.Nu.bh..h....
+00000650: 7586 624b 0751 2981 4e7d 6802 4e73 8662  u.bK.Q).N}h.Ns.b
+00000660: 4b05 5129 814e 7d28 6801 4301 2968 024e  K.Q).N}(h.C.)h.N
+00000670: 7586 6274 6806 8968 024e 7586 6286 4317  u.bth..h.Nu.b.C.
+00000680: 4e4f 4445 5f47 524f 5550 5f57 535f 5345  NODE_GROUP_WS_SE
+00000690: 4e53 4954 4956 454b 0251 2981 4e7d 2868  NSITIVEK.Q).N}(h
+000006a0: 0028 4b05 5129 814e 7d28 6801 4301 7b68  .(K.Q).N}(h.C.{h
+000006b0: 024e 7586 624b 0751 2981 4e7d 6802 4e73  .Nu.bK.Q).N}h.Ns
+000006c0: 8662 4b04 5129 814e 7d28 6807 4b00 6808  .bK.Q).N}(h.K.h.
+000006d0: 4e68 094b 0951 2981 4e7d 2868 0a43 0a45  Nh.K.Q).N}(h.C.E
+000006e0: 5850 5245 5353 494f 4e68 0b68 0c68 024e  XPRESSIONh.h.h.N
+000006f0: 7586 6268 0689 6802 680e 7586 624b 0751  u.bh..h.h.u.bK.Q
+00000700: 2981 4e7d 6802 4e73 8662 4b05 5129 814e  ).N}h.Ns.bK.Q).N
+00000710: 7d28 6801 4301 7d68 024e 7586 6274 6806  }(h.C.}h.Nu.bth.
+00000720: 8968 024e 7586 6286 430a 4e4f 4445 5f55  .h.Nu.b.C.NODE_U
+00000730: 4e49 4f4e 4b02 5129 814e 7d28 6800 284b  NIONK.Q).N}(h.(K
+00000740: 0551 2981 4e7d 2868 0143 015b 6802 4e75  .Q).N}(h.C.[h.Nu
+00000750: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
+00000760: 0451 2981 4e7d 2868 074b 0068 084e 6809  .Q).N}(h.K.h.Nh.
+00000770: 4b09 5129 814e 7d28 680a 430a 4558 5052  K.Q).N}(h.C.EXPR
+00000780: 4553 5349 4f4e 680b 680c 6802 4e75 8662  ESSIONh.h.h.Nu.b
+00000790: 6806 8968 0268 0e75 8662 4b07 5129 814e  h..h.h.u.bK.Q).N
+000007a0: 7d68 024e 7386 624b 0551 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
+000007b0: 0143 015d 6802 4e75 8662 7468 0689 6802  .C.]h.Nu.bth..h.
+000007c0: 4e75 8662 8643 0a4e 4f44 455f 5241 4e47  Nu.b.C.NODE_RANG
+000007d0: 454b 0251 2981 4e7d 2868 0028 4b06 5129  EK.Q).N}(h.(K.Q)
+000007e0: 814e 7d28 6803 6804 4303 5c64 2a4b 0086  .N}(h.h.C.\d*K..
+000007f0: 5294 6805 4b00 6802 8c03 6d69 6e75 8662  R.h.K.h...minu.b
+00000800: 4b05 5129 814e 7d28 6801 4301 2d68 024e  K.Q).N}(h.C.-h.N
+00000810: 7586 624b 0751 2981 4e7d 6802 4e73 8662  u.bK.Q).N}h.Ns.b
+00000820: 4b06 5129 814e 7d28 6803 6804 4306 285c  K.Q).N}(h.h.C.(\
+00000830: 642b 293f 4b00 8652 9468 054b 0168 028c  d+)?K..R.h.K.h..
+00000840: 036d 6178 7586 624b 0751 2981 4e7d 6802  .maxu.bK.Q).N}h.
+00000850: 4e73 8662 4b09 5129 814e 7d28 680a 430a  Ns.bK.Q).N}(h.C.
+00000860: 4558 5052 4553 5349 4f4e 680b 4e68 028c  EXPRESSIONh.Nh..
+00000870: 046e 6f64 6575 8662 7468 0689 6802 4e75  .nodeu.bth..h.Nu
+00000880: 8662 8643 174e 4f44 455f 5241 4e47 455f  .b.C.NODE_RANGE_
+00000890: 5753 5f53 454e 5349 5449 5645 4b02 5129  WS_SENSITIVEK.Q)
+000008a0: 814e 7d28 6800 284b 0651 2981 4e7d 2868  .N}(h.(K.Q).N}(h
+000008b0: 0368 0f68 054b 0068 028c 036d 696e 7586  .h.h.K.h...minu.
+000008c0: 624b 0551 2981 4e7d 2868 0143 017e 6802  bK.Q).N}(h.C.~h.
+000008d0: 4e75 8662 4b07 5129 814e 7d68 024e 7386  Nu.bK.Q).N}h.Ns.
+000008e0: 624b 0651 2981 4e7d 2868 0368 1068 054b  bK.Q).N}(h.h.h.K
+000008f0: 0168 028c 036d 6178 7586 624b 0951 2981  .h...maxu.bK.Q).
+00000900: 4e7d 2868 0a43 0a45 5850 5245 5353 494f  N}(h.C.EXPRESSIO
+00000910: 4e68 0b4e 6802 8c04 6e6f 6465 7586 6274  Nh.Nh...nodeu.bt
+00000920: 6806 8968 024e 7586 6286 430b 5354 5249  h..h.Nu.b.C.STRI
+00000930: 4e47 5f4e 4f44 454b 0251 2981 4e7d 2868  NG_NODEK.Q).N}(h
+00000940: 004b 0351 2981 4e7d 2868 004b 0251 2981  .K.Q).N}(h.K.Q).
+00000950: 4e7d 2868 0028 4b05 5129 814e 7d28 6801  N}(h.(K.Q).N}(h.
+00000960: 4301 2294 6802 4e75 8662 4b07 5129 814e  C.".h.Nu.bK.Q).N
+00000970: 7d68 024e 7386 624b 0651 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
+00000980: 0368 0443 1328 3f3a 5b5e 225c 5c5d 7c28  .h.C.(?:[^"\\]|(
+00000990: 3f3a 5c5c 2e29 292a 4b00 8652 6805 4b00  ?:\\.))*K..Rh.K.
+000009a0: 6802 680e 7586 624b 0551 2981 4e7d 2868  h.h.u.bK.Q).N}(h
+000009b0: 0168 1168 024e 7586 6274 6806 8968 024e  .h.h.Nu.bth..h.N
+000009c0: 7586 624b 0251 2981 4e7d 2868 0028 4b05  u.bK.Q).N}(h.(K.
+000009d0: 5129 814e 7d28 6801 4301 2794 6802 4e75  Q).N}(h.C.'.h.Nu
+000009e0: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
+000009f0: 0651 2981 4e7d 2868 0368 0443 1328 3f3a  .Q).N}(h.h.C.(?:
+00000a00: 5b5e 275c 5c5d 7c28 3f3a 5c5c 2e29 292a  [^'\\]|(?:\\.))*
+00000a10: 4b00 8652 6805 4b00 6802 680e 7586 624b  K..Rh.K.h.h.u.bK
+00000a20: 0551 2981 4e7d 2868 0168 1268 024e 7586  .Q).N}(h.h.h.Nu.
+00000a30: 6274 6806 8968 024e 7586 6286 6802 680e  bth..h.Nu.b.h.h.
+00000a40: 7586 6285 6806 8968 024e 7586 6286 430c  u.b.h..h.Nu.b.C.
+00000a50: 5041 5454 4552 4e5f 4e4f 4445 4b02 5129  PATTERN_NODEK.Q)
+00000a60: 814e 7d28 6800 284b 0651 2981 4e7d 2868  .N}(h.(K.Q).N}(h
+00000a70: 0368 0443 0628 5c64 2a29 3f4b 0086 5268  .h.C.(\d*)?K..Rh
+00000a80: 054b 0168 028c 0567 726f 7570 7586 624b  .K.h...groupu.bK
+00000a90: 0551 2981 4e7d 2868 0143 012f 9468 024e  .Q).N}(h.C./.h.N
+00000aa0: 7586 624b 0751 2981 4e7d 6802 4e73 8662  u.bK.Q).N}h.Ns.b
+00000ab0: 4b06 5129 814e 7d28 6803 6804 4314 283f  K.Q).N}(h.h.C.(?
+00000ac0: 3a5b 5e5c 2f5c 5c5d 7c28 3f3a 5c5c 2e29  :[^\/\\]|(?:\\.)
+00000ad0: 292a 4b00 8652 6805 4b00 6802 8c07 7061  )*K..Rh.K.h...pa
+00000ae0: 7474 6572 6e75 8662 4b07 5129 814e 7d68  tternu.bK.Q).N}h
+00000af0: 024e 7386 624b 0551 2981 4e7d 2868 0168  .Ns.bK.Q).N}(h.h
+00000b00: 1368 024e 7586 624b 0751 2981 4e7d 6802  .h.Nu.bK.Q).N}h.
+00000b10: 4e73 8662 4b06 5129 814e 7d28 6803 6804  Ns.bK.Q).N}(h.h.
+00000b20: 4306 5b69 6d73 5d2a 4b00 8652 6805 4b00  C.[ims]*K..Rh.K.
+00000b30: 6802 8c05 666c 6167 7375 8662 7468 0689  h...flagsu.bth..
+00000b40: 6802 4e75 8662 8643 0753 5445 414c 4552  h.Nu.b.C.STEALER
+00000b50: 4b02 5129 814e 7d28 6800 4b05 5129 814e  K.Q).N}(h.K.Q).N
+00000b60: 7d28 6801 4301 2168 024e 7586 6285 6806  }(h.C.!h.Nu.b.h.
+00000b70: 8968 024e 7586 6286 4307 434f 4e54 4558  .h.Nu.b.C.CONTEX
+00000b80: 544b 0251 2981 4e7d 2868 0028 4b05 5129  TK.Q).N}(h.(K.Q)
+00000b90: 814e 7d28 6801 4301 3c68 024e 7586 624b  .N}(h.C.<h.Nu.bK
+00000ba0: 0751 2981 4e7d 6802 4e73 8662 4b03 5129  .Q).N}h.Ns.bK.Q)
+00000bb0: 814e 7d28 6800 4b02 5129 814e 7d28 6800  .N}(h.K.Q).N}(h.
+00000bc0: 4b09 5129 814e 7d28 680a 430b 5354 5249  K.Q).N}(h.C.STRI
+00000bd0: 4e47 5f4e 4f44 4568 0b4e 6802 8c03 7374  NG_NODEh.Nh...st
+00000be0: 7275 8662 8568 0689 6802 4e75 8662 4b02  ru.b.h..h.Nu.bK.
+00000bf0: 5129 814e 7d28 6800 4b06 5129 814e 7d28  Q).N}(h.K.Q).N}(
+00000c00: 6803 6804 4303 5c77 2a4b 0086 5268 054b  h.h.C.\w*K..Rh.K
+00000c10: 0068 028c 0372 6177 7586 6285 6806 8968  .h...rawu.b.h..h
+00000c20: 024e 7586 6286 6802 680e 7586 624b 0751  .Nu.b.h.h.u.bK.Q
+00000c30: 2981 4e7d 6802 4e73 8662 4b05 5129 814e  ).N}h.Ns.bK.Q).N
+00000c40: 7d28 6801 4301 3e68 024e 7586 6274 6806  }(h.C.>h.Nu.bth.
+00000c50: 8968 024e 7586 6286 4307 4e4f 4445 5245  .h.Nu.b.C.NODERE
+00000c60: 464b 0251 2981 4e7d 2868 004b 0551 2981  FK.Q).N}(h.K.Q).
+00000c70: 4e7d 2868 0143 0140 6802 4e75 8662 4b07  N}(h.C.@h.Nu.bK.
+00000c80: 5129 814e 7d68 024e 7386 624b 0651 2981  Q).N}h.Ns.bK.Q).
+00000c90: 4e7d 2868 0368 0443 075b 5c77 5c2e 5d2b  N}(h.h.C.[\w\.]+
+00000ca0: 4b00 8652 6805 4b00 6802 680e 7586 6287  K..Rh.K.h.h.u.b.
+00000cb0: 6806 8968 024e 7586 6286 742e            h..h.Nu.b.t.
```

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/serialize.py` & `caustic.lexer-1.2.0/src/caustic/lexer/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/src/caustic/lexer/util.py` & `caustic.lexer-1.2.0/src/caustic/lexer/util.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.1.0/src/caustic.lexer.egg-info/PKG-INFO` & `caustic.lexer-1.2.0/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -81,26 +81,32 @@
 
 Note: `basic_compiler` will not accept node names with periods
 
 #### Anonymous
 "Anonymous" named nodes are expressions prefixed with `:`, but with
 no leading name
 
+#### Unpack
+"Unpack" nodes are expressions prefixed with `^:`
+
+Note: `basic_compiler` will not accept unpack nodes
+
 ### Group
 > `nodes.NodeGroup`
 
 The top level of an expression is implicitly grouped
 
 A simple group node is opened by `(` and closed by `)`  
 Groups match the nodes inside of them in a sequence in order  
 The return value of this group will be dependent on its contents' [naming](#naming):
 
 - A group containing no named nodes will return a list of its nodes' results
 - A group containing nodes with "[anonymous](#anonymous)" names returns the last matched anonymous nodes' return value
 - A group containing [named](#naming) nodes returns a dict containing a mapping of the names to the nodes' results
+- Any [unpack](#unpack) nodes will unpack either their elements (sequence) or their names and values into the surrounding group's result
 
 Mixing anonymous and named expressions in a single group will result in an error
 
 #### Whitespace sensitive group
 > `nodes.NodeGroup`, `keep_whitespace=True`
 
 A whitespace sensitive group is opened by `{` and closed by `}`
```

