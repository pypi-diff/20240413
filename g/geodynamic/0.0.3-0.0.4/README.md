# Comparing `tmp/geodynamic-0.0.3.tar.gz` & `tmp/geodynamic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.3.tar", last modified: Tue Apr  9 12:59:21 2024, max compression
+gzip compressed data, was "geodynamic-0.0.4.tar", last modified: Sat Apr 13 15:41:43 2024, max compression
```

## Comparing `geodynamic-0.0.3.tar` & `geodynamic-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.494100 geodynamic-0.0.3/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.3/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-09 12:59:21.494015 geodynamic-0.0.3/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.3/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.481637 geodynamic-0.0.3/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.3/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.491118 geodynamic-0.0.3/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.3/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10290 2024-04-08 16:47:18.000000 geodynamic-0.0.3/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    23251 2024-03-01 12:40:39.000000 geodynamic-0.0.3/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12689 2024-03-01 18:21:15.000000 geodynamic-0.0.3/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.3/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    29798 2024-04-09 12:54:44.000000 geodynamic-0.0.3/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.492970 geodynamic-0.0.3/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.3/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.3/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     6740 2024-04-09 12:40:41.000000 geodynamic-0.0.3/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.3/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.3/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.493688 geodynamic-0.0.3/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-09 12:59:21.494724 geodynamic-0.0.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-08 16:25:07.000000 geodynamic-0.0.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.555226 geodynamic-0.0.4/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.4/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-13 15:41:43.555140 geodynamic-0.0.4/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.4/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.549727 geodynamic-0.0.4/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.4/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.552781 geodynamic-0.0.4/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.4/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.4/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    23540 2024-04-13 14:55:14.000000 geodynamic-0.0.4/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.4/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.4/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    29798 2024-04-09 12:54:44.000000 geodynamic-0.0.4/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.554211 geodynamic-0.0.4/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.4/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.4/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7316 2024-04-13 14:58:22.000000 geodynamic-0.0.4/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.4/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.4/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.554827 geodynamic-0.0.4/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-13 15:41:43.555619 geodynamic-0.0.4/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-13 15:41:09.000000 geodynamic-0.0.4/setup.py
```

### Comparing `geodynamic-0.0.3/PKG-INFO` & `geodynamic-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.3/geodynamic/geo/construction.py` & `geodynamic-0.0.4/geodynamic/geo/construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             self.add(Command(nameCommand, inputs, outputs))
 
     def element(self, name: str): #) -> Element | None:
         result = list(filter(lambda elem: elem.name == name, self.elements))
         if result:
             return result[0]
         else:
-            print(f'Element {name} is not exist')
+            #print(f'Element {name} is not exist')
             return None
 
     def var(self, name:str): #) -> Var | None:
         result = list(filter(lambda var: var.name == name, self.vars))
         return result[0] if result else None
 
     def objectByName(self, name: str): #) -> Element | Var | None:
@@ -218,16 +218,19 @@
             output_data = f(*input_data)
             if not isinstance(output_data, list): output_data = [output_data]
             if debug: print(f"{f.__name__}: {output_data} >> {command.outputs}")
 
             # здесь идет проверка выходных данных output_data и запись соответствующих данных в command.outputs
             for i in range(len(output_data)):
                 if (i < len(command.outputs)) and (output_data[i] is not None):
-                    self.update(command.outputs[i], output_data[i], log = log)
-
+                    if self.element(command.outputs[i]) is not None:
+                        if not self.element(command.outputs[i]).fixed:
+                            self.update(command.outputs[i], output_data[i], log = log)
+                    else:
+                        self.update(command.outputs[i], output_data[i], log = log)
         elif debug:
             print(f"NONE {strFullCommand(command.name, command.inputs)}: {command.inputs}")
 
 def is_number(s):
     try:
         float(s)
         return True
```

### Comparing `geodynamic-0.0.3/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.4/geodynamic/geo/lib_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,16 +322,16 @@
     y = line.c - np.dot(line.n, circle.c)
     x_squared = circle.r_squared - y ** 2
     if np.isclose(x_squared, 0): return Point(y * line.n + circle.c)
     assert(x_squared > 0)
 
     x = np.sqrt(x_squared)
     return [
-        Point(x * line.v + y * line.n + circle.c),
         Point(-x * line.v + y * line.n + circle.c),
+        Point(x * line.v + y * line.n + circle.c),
     ]
 
 def intersect_lci(line, circle, index):
     res = intersect_lc(line, circle)
     index = int(max(0, index-1))
     if len(res) > index: return res[len(res) - index - 1]
     else: return None
@@ -364,86 +364,94 @@
     
 def intersect_cl(c,l):
     return intersect_lc(l,c)
 
 def intersect_cli(c,l,i):
     return intersect_lci(l,c,i)
 
+def intersect_cr(c,r):
+    return intersect_rc(r,c)
+
+def intersect_cri(c,r,i):
+    return intersect_rci(r,c,i)
+
 def intersect_Cl(arc, line):
     results = intersect_lc(line,arc)
     if not isinstance(results, Iterable) or isinstance(results, str): results = (results,)
-    return [x for x in results if arc.contains(x.a)]
+    return [p for p in results if arc.contains(p.a)]
 
 def intersect_cs(circle, segment):
     results = intersect_lc(segment, circle)
-    if not isinstance(results, Iterable) or isinstance(results, str): results = (results,)
-    return [x for x in results if segment.contains(x.a)]
+    if (not isinstance(results, Iterable)) or isinstance(results, str): results = (results,)
+    return [p for p in results if segment.contains(p.a)]
 
 def intersect_csi(circle, segment, index):
     res = intersect_cs(circle, segment)
     index = int(max(0, index-1))
     if len(res) > index: return res[index]
     else: return None
 
+def intersect_rc(ray, circle):
+    results = intersect_lc(ray, circle)
+    if (not isinstance(results, Iterable)) or isinstance(results, str): results = (results,)
+    return [p for p in results if ray.contains(p.a)]
+
+def intersect_rci(ray, circle, index):
+    res = intersect_rc(ray, circle)
+    index = int(max(0, index-1))
+    if len(res) > index: return res[index]
+    else: return None
+
 def intersect_sc(segment, circle):
     return intersect_cs(circle, segment)
 
 def intersect_sci(segment, circle, index):
     return intersect_csi(circle, segment, index)
 
 def intersect_lr(line, ray):
     result = intersect_ll(line, ray)
     if result is None: return None
     #assert(ray.contains(result.a))
-    if not ray.contains(result.a): return None
-    return result
+    return result if ray.contains(result.a) else None
 
 def intersect_ls(line, segment):
     result = intersect_ll(line, segment)
     if result is None: return None
     #assert(segment.contains(result.a))
-    if not segment.contains(result.a): return None
-    return result
+    return result if segment.contains(result.a) else None
 
 def intersect_rl(ray, line):
-    result = intersect_ll(ray, line)
-    if result is None: return None
-    #assert(ray.contains(result.a))
-    if not ray.contains(result.a): return None
-    return result
+    return intersect_lr(line, ray)
 
 def intersect_rr(r1, r2):
     result = intersect_ll(r1, r2)
     if result is None: return None
     #assert(r1.contains(result.a))
     #assert(r2.contains(result.a))
-    if (not r1.contains(result.a)) | (not r2.contains(result.a)): return None
-    return result
+    return result if r1.contains(result.a) & r2.contains(result.a) else None
 
 def intersect_rs(ray, segment):
     result = intersect_ll(ray, segment)
     if result is None: return None
     #assert(ray.contains(result.a))
     #assert(segment.contains(result.a))
-    if (not ray.contains(result.a)) | (not segment.contains(result.a)): return None
-    return result
+    return result if ray.contains(result.a) & segment.contains(result.a) else None
 
 def intersect_sl(segment, line):
     return intersect_ls(line, segment)
 
 def intersect_sr(segment, ray):
     return intersect_rs(ray, segment)
 
 def intersect_ss(s1, s2):
     result = intersect_ll(s1, s2)
     if result is None: return None
     #assert(s1.contains(result.a))
     #assert(s2.contains(result.a))
-    if (not s1.contains(result.a)) | (not s2.contains(result.a)): return None
-    return result
+    return result if s1.contains(result.a) & s2.contains(result.a) else None
 
 def line_bisector_pp(p1, p2):
     p = (p1.a + p2.a) / 2
     n = p2.a - p1.a
     assert((n != 0).any())
     return Line(n, np.dot(n, p))
```

### Comparing `geodynamic-0.0.3/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.4/geodynamic/geo/lib_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import numpy as np
 
 from .lib_vars import *
 
 #--------------------------------------------------------------------------
 
 class Element:
-    def __init__(self, name, data = None, visible = True):
+    def __init__(self, name, data = None, visible = True, fixed = False):
         self.name = name
         self.data = data
+        self.fixed = fixed
         self.visible = visible
         self.style = {}
         if data is not None:
-            self.style = data.style
+            if hasattr(data, 'style'):
+                self.style = data.style
 
     def __repr__(self):
         return "{}:\t{}".format(self.name, self.data)
 
     def drawable(self):
         return isinstance(self.data, (Point, Line, Angle, Polygon, Circle, Vector))
     def draw(self, cr, corners):
@@ -169,15 +171,15 @@
     def scale(self, ratio):
         self.c *= ratio
         self.end_points *= ratio
     def important_points(self):
         return [np.average(self.end_points, axis = 0)]
 
     def __repr__(self):
-        return 'Segment({}, {})'.format(self.end_points[0], self.end_points[1]) + ':\n\t' + Line.__repr__(self)
+        return 'Segment({}, {})'.format(self.end_points[0], self.end_points[1])# + ':\n\t' + Line.__repr__(self)
 
     def get_endpoints(self, corners):
         return self.end_points
 
     def contains(self, x):
         if not Line.contains(self, x): return False
         p1, p2 = self.end_points
@@ -196,14 +198,17 @@
         self.c += np.dot(vec, self.n)
         self.start_point += vec
     def scale(self, ratio):
         self.c *= ratio
         self.start_point *= ratio
     def important_points(self):
         return [self.start_point]
+    
+    def __repr__(self):
+        return 'Ray({}, ...)'.format(self.start_point)# + Line.__repr__(self)
 
     def get_endpoints(self, corners):
         line_endpoints = Line.get_endpoints(self, corners)
         if line_endpoints is None: return None
         pos_endpoints = [
             point
             for point in line_endpoints
@@ -212,15 +217,18 @@
         if len(pos_endpoints) == 0: return None
         elif len(pos_endpoints) == 1:
             return [self.start_point, pos_endpoints[0]]
         else: return pos_endpoints
 
     def contains(self, x):
         if not Line.contains(self, x): return False
-        return np.dot(self.v, x-self.start_point) >= 0
+        if np.dot(self.v, x-self.start_point) >= 0:
+            return True
+        else:
+            return np.isclose(self.start_point, x).all()
 
 class Angle:
     def __init__(self, p, v1, v2):
         self.p = p
         self.angle = np.arctan2(v2[1], v2[0]) - np.arctan2(v1[1], v1[0]) #np.angle(a_to_cpx(v2) / a_to_cpx(v1))
 
         if self.angle < 0:
```

### Comparing `geodynamic-0.0.3/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.4/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/geodynamic/manim_dynamic.py` & `geodynamic-0.0.4/geodynamic/manim_dynamic.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.4/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.4/geodynamic/parsers/ggb_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from zipfile import ZipFile
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element as XElement  # shortened "XML Element"
 
 from ..geo.construction import Construction
 from ..geo.lib_commands import Command
 from ..geo.lib_vars import *
+from ..geo.lib_elements import *
 
 temp_path = os.path.join(os.getcwd(), "temp")
 
 #--------------------------------------------------------------------------
 
 def rgb_to_hex(r, g, b):
     return '#{:02x}{:02x}{:02x}'.format(r, g, b)
@@ -32,17 +33,20 @@
     
     shutil.rmtree(temp_path)
     
     return root.find("construction"), root.find("euclidianView")
 
 def parse_constr(constr: Construction, constr_xelem: XElement, debug = False):
     xelems_left_to_pass = 0
+    fixed_element = False
 
     style = {}
     
+    unknown_objs = {}
+    
     for xelem in constr_xelem:            
         if xelem.tag == "element":
             name = xelem.attrib['label']
             #print(f'ELEMENT {name}')
             if xelem.attrib["type"] != "numeric":
                 style[name] = {}
 
@@ -61,15 +65,15 @@
                 if elem is not None:
                     caption = xelem.find("caption")
                     if (elem.attrib['val'] == '3') & (caption is not None):
                         style[name]['label'] = caption.attrib['val']
                         
                 elem = xelem.find("labelOffset")
                 if elem is not None: 
-                    style[name]['offset'] = [float(elem.attrib['x']) / 100, -float(elem.attrib['y']) / 100]
+                    style[name]['offset'] = [0.3 + float(elem.attrib['x']) / 50, 0.4 - float(elem.attrib['y']) / 50]
  
                 elem = xelem.find("arcSize")
                 if elem is not None: 
                     if xelem.attrib['type'] == 'angle':
                         style[name]['r_offset'] = (float(elem.attrib['val']) - 30) / 30
                         
                 elem = xelem.find("objColor")
@@ -88,47 +92,57 @@
                             if int(tt) > 0: style[name]['stroke_dash'] = 0.65
                         
         if xelems_left_to_pass:
             xelems_left_to_pass -= 1
             continue
 
         if xelem.tag == "expression":
+            #unknown_objs[xelem.attrib["label"]] = True
             #xelems_left_to_pass = 1
             continue
         if xelem.tag == "command":
             comm_name = xelem.attrib["name"]
+            input_xelem, output_xelem = xelem.find("input"), xelem.find("output")
+            inputs, outputs = list(input_xelem.attrib.values()), list(output_xelem.attrib.values())
+            
+            if comm_name == "Point":
+                if len(inputs) == 1:
+                    print('Point FIXED')
+                    fixed_element = True
+                else:
+                    xelems_left_to_pass = 1
+                continue
             if comm_name == "PointIn":
                 xelems_left_to_pass = 1
                 continue
-            
-            input_xelem = xelem.find("input")
-            output_xelem = xelem.find("output")
-            
-            constr.add(Command(comm_name, list(input_xelem.attrib.values()), list(output_xelem.attrib.values())))
+
+            constr.add(Command(comm_name, inputs, outputs))
             xelems_left_to_pass = len(output_xelem.attrib)
             continue
         
         # Here xelem has to be a commandless point or numeric (Var)
         
         if xelem.tag == "element":
             if xelem.attrib["type"] == "point":
                 coords = list(xelem.find("coords").attrib.values())
                 coords.pop(-1) #  removing z coordinate
-                constr.add(Command("Point", coords, xelem.attrib["label"]))
+                constr.add(Element(xelem.attrib["label"], Point([float(x) for x in coords]), fixed = fixed_element))
+                fixed_element = False
                 continue
             if xelem.attrib["type"] == "numeric":
                 value_xelem = xelem.find("value")
                 constr.add(Var(xelem.attrib["label"], float(value_xelem.attrib["val"])))
                 continue
             if xelem.attrib["type"] == "angle":
                 value_xelem = xelem.find("value")
                 constr.add(Var(xelem.attrib["label"], AngleSize(float(value_xelem.attrib["val"]))))
                 continue
         
-        raise ElementTree.ParseError(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
+        #raise ElementTree.ParseError(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
+        print(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
 
     constr.rebuild(debug = debug)
 
     #styling elements
     for name in style:
         for key in style[name]:
             #print(f'STYLE >> {name} >> {key} = {style[name][key]}')
```

### Comparing `geodynamic-0.0.3/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.4/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/geodynamic/parsers/svg_parser.py` & `geodynamic-0.0.4/geodynamic/parsers/svg_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.4/geodynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.3/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.4/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.3/setup.py` & `geodynamic-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.3',
+  version='0.0.4',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

