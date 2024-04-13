# Comparing `tmp/sindapi-0.0.5.tar.gz` & `tmp/sindapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sindapi-0.0.5.tar", last modified: Tue Apr  9 10:26:33 2024, max compression
+gzip compressed data, was "sindapi-0.0.6.tar", last modified: Sat Apr 13 07:58:00 2024, max compression
```

## Comparing `sindapi-0.0.5.tar` & `sindapi-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.819225 sindapi-0.0.5/
--rw-rw-rw-   0        0        0      334 2024-04-09 10:26:33.818226 sindapi-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 10:26:33.819225 sindapi-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-04-09 10:26:22.000000 sindapi-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.787226 sindapi-0.0.5/sindapi/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.5/sindapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.810225 sindapi-0.0.5/sindapi/sindmap/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.5/sindapi/sindmap/__init__.py
--rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.5/sindapi/sindmap/drivable_area.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.812225 sindapi-0.0.5/sindapi/sindmap/intersection/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.5/sindapi/sindmap/intersection/__init__.py
--rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.5/sindapi/sindmap/intersection/intersection.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.814252 sindapi-0.0.5/sindapi/sindmap/lane/
--rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.5/sindapi/sindmap/lane/__init__.py
--rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.5/sindapi/sindmap/lane/lane_segment.py
--rw-rw-rw-   0        0        0     4222 2024-04-09 10:26:07.000000 sindapi-0.0.5/sindapi/sindmap/map_api.py
--rw-rw-rw-   0        0        0     1483 2024-04-09 10:04:14.000000 sindapi-0.0.5/sindapi/sindmap/pedestrian_crossing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.815245 sindapi-0.0.5/sindapi/sindmap/stretch/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.5/sindapi/sindmap/stretch/__init__.py
--rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.5/sindapi/sindmap/stretch/stretch.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.817240 sindapi-0.0.5/sindapi/sindmap/utils/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.5/sindapi/sindmap/utils/__init__.py
--rw-rw-rw-   0        0        0     1948 2024-04-07 10:30:37.000000 sindapi-0.0.5/sindapi/sindmap/utils/map_primitives.py
--rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.5/sindapi/sindmap/utils/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:26:33.807244 sindapi-0.0.5/sindapi.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-09 10:26:33.000000 sindapi-0.0.5/sindapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-09 10:26:33.000000 sindapi-0.0.5/sindapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:26:33.000000 sindapi-0.0.5/sindapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-09 10:26:33.000000 sindapi-0.0.5/sindapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 10:26:33.000000 sindapi-0.0.5/sindapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/
+-rw-rw-rw-   0        0        0      334 2024-04-13 07:58:00.776350 sindapi-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 07:58:00.776350 sindapi-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      440 2024-04-13 07:55:30.000000 sindapi-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.586369 sindapi-0.0.6/sindapi/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.6/sindapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.649392 sindapi-0.0.6/sindapi/sindmap/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.6/sindapi/sindmap/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.6/sindapi/sindmap/drivable_area.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.665419 sindapi-0.0.6/sindapi/sindmap/intersection/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.6/sindapi/sindmap/intersection/__init__.py
+-rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.6/sindapi/sindmap/intersection/intersection.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.696906 sindapi-0.0.6/sindapi/sindmap/lane/
+-rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.6/sindapi/sindmap/lane/__init__.py
+-rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.6/sindapi/sindmap/lane/lane_segment.py
+-rw-rw-rw-   0        0        0     4503 2024-04-10 14:52:17.000000 sindapi-0.0.6/sindapi/sindmap/map_api.py
+-rw-rw-rw-   0        0        0     1483 2024-04-09 12:32:07.000000 sindapi-0.0.6/sindapi/sindmap/pedestrian_crossing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.697662 sindapi-0.0.6/sindapi/sindmap/stretch/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.6/sindapi/sindmap/stretch/__init__.py
+-rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.6/sindapi/sindmap/stretch/stretch.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.712631 sindapi-0.0.6/sindapi/sindmap/traffic_light/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:05:17.000000 sindapi-0.0.6/sindapi/sindmap/traffic_light/__init__.py
+-rw-rw-rw-   0        0        0     1498 2024-04-11 09:39:33.000000 sindapi-0.0.6/sindapi/sindmap/traffic_light/traffic_light.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.729865 sindapi-0.0.6/sindapi/sindmap/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.6/sindapi/sindmap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1955 2024-04-09 12:32:07.000000 sindapi-0.0.6/sindapi/sindmap/utils/map_primitives.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.744409 sindapi-0.0.6/sindapi/sindtrack/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.6/sindapi/sindtrack/__init__.py
+-rw-rw-rw-   0        0        0     4563 2024-04-11 08:15:22.000000 sindapi-0.0.6/sindapi/sindtrack/data_schema.py
+-rw-rw-rw-   0        0        0    12114 2024-04-11 09:45:26.000000 sindapi-0.0.6/sindapi/sindtrack/process_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.762508 sindapi-0.0.6/sindapi/sindtrack/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.6/sindapi/sindtrack/utils/__init__.py
+-rw-rw-rw-   0        0        0      561 2024-04-11 08:39:35.000000 sindapi-0.0.6/sindapi/sindtrack/utils/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/sindapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.6/sindapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.6/sindapi/utils/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/sindapi.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/top_level.txt
```

### Comparing `sindapi-0.0.5/sindapi/sindmap/intersection/intersection.py` & `sindapi-0.0.6/sindapi/sindmap/intersection/intersection.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.5/sindapi/sindmap/lane/lane_segment.py` & `sindapi-0.0.6/sindapi/sindmap/lane/lane_segment.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.5/sindapi/sindmap/map_api.py` & `sindapi-0.0.6/sindapi/sindmap/map_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 
 from .drivable_area import DrivableArea
 from .pedestrian_crossing import PedestrianCrossing
 from .stretch.stretch import Stretch
 from .intersection.intersection import Intersection
 from .lane.lane_segment import Lane, LaneSegment
+from .traffic_light.traffic_light import TrafficLight
 
 
 @dataclass
 class SinDStaticMap:
     city_name: str
     vector_drivable_areas: Dict[int, DrivableArea]
     vector_pedestrian_crossings: Dict[int, PedestrianCrossing]
     vector_stretches: Dict[int, Stretch]
     vector_intersections: Dict[int, Intersection]
     vector_lane_segments: Dict[int, LaneSegment]
+    map_id: Optional[str]
     split_distance: float = None
     segment_point_num: int = None
 
     @classmethod
     def from_cfg(cls, config_path):
         with config_path.open('r') as file:
             config = yaml.safe_load(file)
@@ -37,15 +39,15 @@
             map_data = json.load(file)
         return map_data
 
     @classmethod
     def build(cls, sind_path: Path) -> 'SinDStaticMap':
         sind_map_path = sind_path / 'map'
         cls.from_cfg(sind_map_path / 'config.yaml')
-        map_data = cls.from_json(sind_map_path / 'map.json')
+        map_data = cls.from_json(sind_map_path / 'static_map.json')
 
         vector_stretches = cls.build_stretches(map_data['stretch'])
         vector_intersections, vector_stretches = cls.build_intersections(map_data['intersection'], vector_stretches)
         vector_drivable_areas = cls.build_drivable_areas()
         vector_pedestrian_crossings = cls.build_pedestrian_crossings()
         vector_lane_segments = cls.get_lane_segments(vector_stretches, vector_intersections)
 
@@ -105,7 +107,18 @@
         for _, intersection in vector_intersections.items():
             for _, lane in intersection.vector_lanes.items():
                 for _, segment in lane.vector_lane_segments.items():
                     lane_segments[segment.unique_id] = segment
 
         return lane_segments
 
+
+@dataclass
+class SinDDynamicMap:
+    city_name: str
+    traffic_lights: Dict[int, TrafficLight]
+    map_id: Optional[str]
+
+
+    @classmethod
+    def from_pt(cls):
+        return cls
```

### Comparing `sindapi-0.0.5/sindapi/sindmap/pedestrian_crossing.py` & `sindapi-0.0.6/sindapi/sindmap/pedestrian_crossing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from typing import Tuple
 
-from .utils.map_primitives import Polyline, Point
-from .utils.typing import NDArrayFloat
+from .utils.map_primitives import Polyline
+from sindapi.utils.typing import NDArrayFloat
 
 class PedestrianCrossing:
     id: int
     edge1: Polyline
     edge2: Polyline
 
     @classmethod
```

### Comparing `sindapi-0.0.5/sindapi/sindmap/stretch/stretch.py` & `sindapi-0.0.6/sindapi/sindmap/stretch/stretch.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.5/sindapi/sindmap/utils/map_primitives.py` & `sindapi-0.0.6/sindapi/sindmap/utils/map_primitives.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # <Copyright 2022, Argo AI, LLC. Released under the MIT license.>
 
 """Primitive types for vector maps (point, polyline)."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import List
 import numpy as np
 
-from .typing import NDArrayFloat
+from sindapi.utils.typing import NDArrayFloat
 
 
 @dataclass
 class Point:
     """Represents a single 2-d point."""
 
     x: float
```

### Comparing `sindapi-0.0.5/sindapi.egg-info/SOURCES.txt` & `sindapi-0.0.6/sindapi.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -11,10 +11,18 @@
 sindapi/sindmap/pedestrian_crossing.py
 sindapi/sindmap/intersection/__init__.py
 sindapi/sindmap/intersection/intersection.py
 sindapi/sindmap/lane/__init__.py
 sindapi/sindmap/lane/lane_segment.py
 sindapi/sindmap/stretch/__init__.py
 sindapi/sindmap/stretch/stretch.py
+sindapi/sindmap/traffic_light/__init__.py
+sindapi/sindmap/traffic_light/traffic_light.py
 sindapi/sindmap/utils/__init__.py
 sindapi/sindmap/utils/map_primitives.py
-sindapi/sindmap/utils/typing.py
+sindapi/sindtrack/__init__.py
+sindapi/sindtrack/data_schema.py
+sindapi/sindtrack/process_raw_data.py
+sindapi/sindtrack/utils/__init__.py
+sindapi/sindtrack/utils/constants.py
+sindapi/utils/__init__.py
+sindapi/utils/typing.py
```

