# Comparing `tmp/imap_box-0.1.7.tar.gz` & `tmp/imap_box-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imap_box-0.1.7.tar", last modified: Mon Aug 28 14:33:21 2023, max compression
+gzip compressed data, was "dist/imap_box-0.1.8.tar", last modified: Sat Apr 13 13:41:46 2024, max compression
```

## Comparing `imap_box-0.1.7.tar` & `imap_box-0.1.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2023-08-28 14:33:21.000000 imap_box-0.1.7/
--rw-rw-r--   0 zero      (1000) zero      (1000)    11359 2023-08-06 03:53:35.000000 imap_box-0.1.7/LICENSE
--rw-rw-r--   0 zero      (1000) zero      (1000)     2959 2023-08-28 14:33:21.000000 imap_box-0.1.7/PKG-INFO
--rw-rw-r--   0 zero      (1000) zero      (1000)     2440 2023-08-06 03:53:35.000000 imap_box-0.1.7/README.md
-drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap/
--rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:35.000000 imap_box-0.1.7/imap/__init__.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     2145 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/editor.py
--rw-rw-r--   0 zero      (1000) zero      (1000)      949 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/global_var.py
-drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap/lib/
--rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/__init__.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     3299 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/common.py
--rw-rw-r--   0 zero      (1000) zero      (1000)    24340 2023-08-28 14:25:30.000000 imap_box-0.1.7/imap/lib/convertor.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     1980 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/convex_hull.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     2223 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/draw.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     6642 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/odr_spiral.py
-drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap/lib/opendrive/
--rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/__init__.py
--rw-rw-r--   0 zero      (1000) zero      (1000)      962 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/common.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     2450 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/header.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     3302 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/junction.py
--rw-rw-r--   0 zero      (1000) zero      (1000)    13943 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/lanes.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     4401 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/map.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     8140 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/plan_view.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     2681 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/profile.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     6141 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/road.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     4576 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/signals.py
--rw-rw-r--   0 zero      (1000) zero      (1000)      771 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/opendrive/user_data.py
--rw-rw-r--   0 zero      (1000) zero      (1000)      988 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/polynoms.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     2173 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/proj_helper.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     4528 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/proto_utils.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     1910 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/lib/transform.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     3943 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/main.py
--rw-rw-r--   0 zero      (1000) zero      (1000)     4800 2023-08-06 03:53:36.000000 imap_box-0.1.7/imap/map.py
-drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/
--rw-rw-r--   0 zero      (1000) zero      (1000)     2959 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/PKG-INFO
--rw-rw-r--   0 zero      (1000) zero      (1000)      905 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/SOURCES.txt
--rw-rw-r--   0 zero      (1000) zero      (1000)        1 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/dependency_links.txt
--rw-rw-r--   0 zero      (1000) zero      (1000)       40 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/entry_points.txt
--rw-rw-r--   0 zero      (1000) zero      (1000)       53 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/requires.txt
--rw-rw-r--   0 zero      (1000) zero      (1000)        5 2023-08-28 14:33:21.000000 imap_box-0.1.7/imap_box.egg-info/top_level.txt
--rw-rw-r--   0 zero      (1000) zero      (1000)       85 2023-08-06 03:53:36.000000 imap_box-0.1.7/pyproject.toml
--rw-rw-r--   0 zero      (1000) zero      (1000)       38 2023-08-28 14:33:21.000000 imap_box-0.1.7/setup.cfg
--rw-rw-r--   0 zero      (1000) zero      (1000)     1045 2023-08-28 14:30:52.000000 imap_box-0.1.7/setup.py
+drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2024-04-13 13:41:46.000000 imap_box-0.1.8/
+-rw-rw-r--   0 zero      (1000) zero      (1000)    11359 2023-08-06 03:53:35.000000 imap_box-0.1.8/LICENSE
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2959 2024-04-13 13:41:46.000000 imap_box-0.1.8/PKG-INFO
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2440 2023-08-06 03:53:35.000000 imap_box-0.1.8/README.md
+drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2024-04-13 13:41:46.000000 imap_box-0.1.8/imap/
+-rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:35.000000 imap_box-0.1.8/imap/__init__.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2145 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/editor.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)      949 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/global_var.py
+drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2024-04-13 13:41:46.000000 imap_box-0.1.8/imap/lib/
+-rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/__init__.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     3333 2024-04-13 13:39:03.000000 imap_box-0.1.8/imap/lib/common.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)    24678 2024-04-13 13:39:03.000000 imap_box-0.1.8/imap/lib/convertor.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     1980 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/convex_hull.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2223 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/draw.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     6642 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/odr_spiral.py
+drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2024-04-13 13:41:46.000000 imap_box-0.1.8/imap/lib/opendrive/
+-rw-rw-r--   0 zero      (1000) zero      (1000)        0 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/__init__.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)      962 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/common.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2450 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/header.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     3302 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/junction.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)    14070 2024-04-13 13:39:03.000000 imap_box-0.1.8/imap/lib/opendrive/lanes.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     4401 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/map.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     8140 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/plan_view.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2681 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/profile.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     6141 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/road.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     4576 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/signals.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)      771 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/opendrive/user_data.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)      988 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/polynoms.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2173 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/proj_helper.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     4528 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/proto_utils.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     1910 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/lib/transform.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     3943 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/main.py
+-rw-rw-r--   0 zero      (1000) zero      (1000)     4800 2023-08-06 03:53:36.000000 imap_box-0.1.8/imap/map.py
+drwxrwxr-x   0 zero      (1000) zero      (1000)        0 2024-04-13 13:41:46.000000 imap_box-0.1.8/imap_box.egg-info/
+-rw-rw-r--   0 zero      (1000) zero      (1000)     2959 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/PKG-INFO
+-rw-rw-r--   0 zero      (1000) zero      (1000)      905 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/SOURCES.txt
+-rw-rw-r--   0 zero      (1000) zero      (1000)        1 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/dependency_links.txt
+-rw-rw-r--   0 zero      (1000) zero      (1000)       40 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/entry_points.txt
+-rw-rw-r--   0 zero      (1000) zero      (1000)       53 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/requires.txt
+-rw-rw-r--   0 zero      (1000) zero      (1000)        5 2024-04-13 13:41:45.000000 imap_box-0.1.8/imap_box.egg-info/top_level.txt
+-rw-rw-r--   0 zero      (1000) zero      (1000)       85 2023-08-06 03:53:36.000000 imap_box-0.1.8/pyproject.toml
+-rw-rw-r--   0 zero      (1000) zero      (1000)       38 2024-04-13 13:41:46.000000 imap_box-0.1.8/setup.cfg
+-rw-rw-r--   0 zero      (1000) zero      (1000)     1045 2024-04-13 13:40:44.000000 imap_box-0.1.8/setup.py
```

### Comparing `imap_box-0.1.7/LICENSE` & `imap_box-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/PKG-INFO` & `imap_box-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap_box
-Version: 0.1.7
+Version: 0.1.8
 Summary: High-resolution map visualization and conversion tool
 Home-page: https://github.com/daohu527/imap
 Author: daohu527
 Author-email: daohu527@gmail.com
 Project-URL: Bug Tracker, https://github.com/daohu527/imap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `imap_box-0.1.7/README.md` & `imap_box-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/editor.py` & `imap_box-0.1.8/imap/editor.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/global_var.py` & `imap_box-0.1.8/imap/global_var.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/common.py` & `imap_box-0.1.8/imap/lib/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,17 @@
 def shift_t(point3d, offset):
   npoint = copy.deepcopy(point3d)
   npoint.shift_t(offset)
 
   return npoint
 
 def calc_length(points):
+  if len(points) < 2:
+    return
+
   length = 0
   if math.fabs(points[0].yaw - points[-1].yaw) < 0.01:
     # straight line
     p, q = points[0], points[-1]
     x = q.x - p.x
     y = q.y - p.y
     z = q.z - p.z
```

### Comparing `imap_box-0.1.7/imap/lib/convertor.py` & `imap_box-0.1.8/imap/lib/convertor.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,19 +152,27 @@
     else:
       # We want just support +proj=tmerc, but some do not contain this parameter
       for p in proj_txt.split():
         if p.startswith('+lat_0'):
           lat = float(p.split('=')[1])
         elif p.startswith('+lon_0'):
           lon = float(p.split('=')[1])
+        elif p.startswith('+x_0'):
+          x_0 = float(p.split('=')[1])
+        elif p.startswith('+y_0'):
+          y_0 = float(p.split('=')[1])
       if lat is None or lon is None:
         self.pb_map.header.projection.proj = "+proj=utm +zone={} +ellps=WGS84 " \
           "+datum=WGS84 +units=m +no_defs".format(0)
       else:
         self.origin_x, self.origin_y, zone_id = latlon2utm(lat, lon)
+        if x_0:
+          self.origin_x = self.origin_x - x_0
+        if y_0:
+          self.origin_y = self.origin_y - y_0
         self.pb_map.header.projection.proj = "+proj=utm +zone={} +ellps=WGS84 " \
           "+datum=WGS84 +units=m +no_defs".format(zone_id)
 
   def convert_header(self):
     if self.xodr_map.header.version:
       self.pb_map.header.version = self.xodr_map.header.version
     if self.xodr_map.header.date:
@@ -579,17 +587,19 @@
 
   def construct_junction_polygon(self, xodr_junction):
     if not self._is_valid_junction(xodr_junction):
       return []
 
     points = []
     for road, relation in xodr_junction.connected_roads:
-      start, end = road.get_cross_section(relation)
-      points.append([start.x, start.y])
-      points.append([end.x, end.y])
+      cross_section = road.get_cross_section(relation)
+      if cross_section:
+        start, end = cross_section
+        points.append([start.x, start.y])
+        points.append([end.x, end.y])
 
     # when point <= 4 convex_hull will not fully covered, so we change to aabb_box
     if len(points) <= 4:
       return aabb_box(points)
     else:
       return convex_hull(points)
```

### Comparing `imap_box-0.1.7/imap/lib/convex_hull.py` & `imap_box-0.1.8/imap/lib/convex_hull.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/draw.py` & `imap_box-0.1.8/imap/lib/draw.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/odr_spiral.py` & `imap_box-0.1.8/imap/lib/odr_spiral.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/common.py` & `imap_box-0.1.8/imap/lib/opendrive/common.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/header.py` & `imap_box-0.1.8/imap/lib/opendrive/header.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/junction.py` & `imap_box-0.1.8/imap/lib/opendrive/junction.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/lanes.py` & `imap_box-0.1.8/imap/lib/opendrive/lanes.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,17 +415,18 @@
 
   def process_lane_sections(self, reference_line):
     for lane_section in self.lane_sections:
       start_s = lane_section.s
       end_s = lane_section.end_s
       reference_line_in_section = []
       for (idx, point3d) in enumerate(reference_line):
-        if start_s <= point3d.s <= end_s or \
-          (point3d.s < start_s and idx + 1 < len(reference_line) and start_s <= reference_line[idx + 1].s <= end_s) or \
-            (end_s < point3d.s and idx - 1 >= 0 and start_s <= reference_line[idx - 1].s <= end_s):
+        # Todo(zero): Remove judgment because there may be exceptions? For example, judge the last 2 points instead of 1
+        # if start_s <= point3d.s <= end_s or \
+        #   (point3d.s < start_s and idx + 1 < len(reference_line) and start_s <= reference_line[idx + 1].s <= end_s) or \
+        #     (end_s < point3d.s and idx - 1 >= 0 and start_s <= reference_line[idx - 1].s <= end_s):
           reference_line_in_section.append(point3d)
       lane_section.process_lane(reference_line_in_section)
 
   def get_cross_section(self, relation):
     if relation == "predecessor":
       return self.lane_sections[0].get_cross_section("start")
     elif relation == "successor":
```

### Comparing `imap_box-0.1.7/imap/lib/opendrive/map.py` & `imap_box-0.1.8/imap/lib/opendrive/map.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/plan_view.py` & `imap_box-0.1.8/imap/lib/opendrive/plan_view.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/profile.py` & `imap_box-0.1.8/imap/lib/opendrive/profile.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/road.py` & `imap_box-0.1.8/imap/lib/opendrive/road.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/signals.py` & `imap_box-0.1.8/imap/lib/opendrive/signals.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/opendrive/user_data.py` & `imap_box-0.1.8/imap/lib/opendrive/user_data.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/polynoms.py` & `imap_box-0.1.8/imap/lib/polynoms.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/proj_helper.py` & `imap_box-0.1.8/imap/lib/proj_helper.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/proto_utils.py` & `imap_box-0.1.8/imap/lib/proto_utils.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/lib/transform.py` & `imap_box-0.1.8/imap/lib/transform.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/main.py` & `imap_box-0.1.8/imap/main.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap/map.py` & `imap_box-0.1.8/imap/map.py`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/imap_box.egg-info/PKG-INFO` & `imap_box-0.1.8/imap_box.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-box
-Version: 0.1.7
+Version: 0.1.8
 Summary: High-resolution map visualization and conversion tool
 Home-page: https://github.com/daohu527/imap
 Author: daohu527
 Author-email: daohu527@gmail.com
 Project-URL: Bug Tracker, https://github.com/daohu527/imap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `imap_box-0.1.7/imap_box.egg-info/SOURCES.txt` & `imap_box-0.1.8/imap_box.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imap_box-0.1.7/setup.py` & `imap_box-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imap_box",
-    version="0.1.7",
+    version="0.1.8",
     author="daohu527",
     author_email="daohu527@gmail.com",
     description="High-resolution map visualization and conversion tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daohu527/imap",
     project_urls={
```

