# Comparing `tmp/sindapi-0.0.6.tar.gz` & `tmp/sindapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sindapi-0.0.6.tar", last modified: Sat Apr 13 07:58:00 2024, max compression
+gzip compressed data, was "sindapi-0.0.7.tar", last modified: Sat Apr 13 08:44:16 2024, max compression
```

## Comparing `sindapi-0.0.6.tar` & `sindapi-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/
--rw-rw-rw-   0        0        0      334 2024-04-13 07:58:00.776350 sindapi-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 07:58:00.776350 sindapi-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-04-13 07:55:30.000000 sindapi-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.586369 sindapi-0.0.6/sindapi/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.6/sindapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.649392 sindapi-0.0.6/sindapi/sindmap/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.6/sindapi/sindmap/__init__.py
--rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.6/sindapi/sindmap/drivable_area.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.665419 sindapi-0.0.6/sindapi/sindmap/intersection/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.6/sindapi/sindmap/intersection/__init__.py
--rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.6/sindapi/sindmap/intersection/intersection.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.696906 sindapi-0.0.6/sindapi/sindmap/lane/
--rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.6/sindapi/sindmap/lane/__init__.py
--rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.6/sindapi/sindmap/lane/lane_segment.py
--rw-rw-rw-   0        0        0     4503 2024-04-10 14:52:17.000000 sindapi-0.0.6/sindapi/sindmap/map_api.py
--rw-rw-rw-   0        0        0     1483 2024-04-09 12:32:07.000000 sindapi-0.0.6/sindapi/sindmap/pedestrian_crossing.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.697662 sindapi-0.0.6/sindapi/sindmap/stretch/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.6/sindapi/sindmap/stretch/__init__.py
--rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.6/sindapi/sindmap/stretch/stretch.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.712631 sindapi-0.0.6/sindapi/sindmap/traffic_light/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:05:17.000000 sindapi-0.0.6/sindapi/sindmap/traffic_light/__init__.py
--rw-rw-rw-   0        0        0     1498 2024-04-11 09:39:33.000000 sindapi-0.0.6/sindapi/sindmap/traffic_light/traffic_light.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.729865 sindapi-0.0.6/sindapi/sindmap/utils/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.6/sindapi/sindmap/utils/__init__.py
--rw-rw-rw-   0        0        0     1955 2024-04-09 12:32:07.000000 sindapi-0.0.6/sindapi/sindmap/utils/map_primitives.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.744409 sindapi-0.0.6/sindapi/sindtrack/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.6/sindapi/sindtrack/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-04-11 08:15:22.000000 sindapi-0.0.6/sindapi/sindtrack/data_schema.py
--rw-rw-rw-   0        0        0    12114 2024-04-11 09:45:26.000000 sindapi-0.0.6/sindapi/sindtrack/process_raw_data.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.762508 sindapi-0.0.6/sindapi/sindtrack/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.6/sindapi/sindtrack/utils/__init__.py
--rw-rw-rw-   0        0        0      561 2024-04-11 08:39:35.000000 sindapi-0.0.6/sindapi/sindtrack/utils/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/sindapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.6/sindapi/utils/__init__.py
--rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.6/sindapi/utils/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:58:00.776350 sindapi-0.0.6/sindapi.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      923 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 07:58:00.000000 sindapi-0.0.6/sindapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.123781 sindapi-0.0.7/
+-rw-rw-rw-   0        0        0      334 2024-04-13 08:44:16.121762 sindapi-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 08:44:16.123781 sindapi-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      440 2024-04-13 08:43:31.000000 sindapi-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.087255 sindapi-0.0.7/sindapi/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.7/sindapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.106323 sindapi-0.0.7/sindapi/sindmap/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.7/sindapi/sindmap/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.7/sindapi/sindmap/drivable_area.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.108321 sindapi-0.0.7/sindapi/sindmap/intersection/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.7/sindapi/sindmap/intersection/__init__.py
+-rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.7/sindapi/sindmap/intersection/intersection.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.109323 sindapi-0.0.7/sindapi/sindmap/lane/
+-rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.7/sindapi/sindmap/lane/__init__.py
+-rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.7/sindapi/sindmap/lane/lane_segment.py
+-rw-rw-rw-   0        0        0     4503 2024-04-10 14:52:17.000000 sindapi-0.0.7/sindapi/sindmap/map_api.py
+-rw-rw-rw-   0        0        0     1483 2024-04-09 12:32:07.000000 sindapi-0.0.7/sindapi/sindmap/pedestrian_crossing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.111324 sindapi-0.0.7/sindapi/sindmap/stretch/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.7/sindapi/sindmap/stretch/__init__.py
+-rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.7/sindapi/sindmap/stretch/stretch.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.112320 sindapi-0.0.7/sindapi/sindmap/traffic_light/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:05:17.000000 sindapi-0.0.7/sindapi/sindmap/traffic_light/__init__.py
+-rw-rw-rw-   0        0        0     1498 2024-04-11 09:39:33.000000 sindapi-0.0.7/sindapi/sindmap/traffic_light/traffic_light.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.113324 sindapi-0.0.7/sindapi/sindmap/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.7/sindapi/sindmap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1955 2024-04-09 12:32:07.000000 sindapi-0.0.7/sindapi/sindmap/utils/map_primitives.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.116322 sindapi-0.0.7/sindapi/sindtrack/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.7/sindapi/sindtrack/__init__.py
+-rw-rw-rw-   0        0        0     4573 2024-04-13 08:40:22.000000 sindapi-0.0.7/sindapi/sindtrack/data_schema.py
+-rw-rw-rw-   0        0        0    12157 2024-04-13 08:41:42.000000 sindapi-0.0.7/sindapi/sindtrack/process_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.117322 sindapi-0.0.7/sindapi/sindtrack/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.7/sindapi/sindtrack/utils/__init__.py
+-rw-rw-rw-   0        0        0      561 2024-04-11 08:39:35.000000 sindapi-0.0.7/sindapi/sindtrack/utils/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.119814 sindapi-0.0.7/sindapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.7/sindapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.7/sindapi/utils/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:44:16.102323 sindapi-0.0.7/sindapi.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-13 08:44:15.000000 sindapi-0.0.7/sindapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-13 08:44:15.000000 sindapi-0.0.7/sindapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 08:44:15.000000 sindapi-0.0.7/sindapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 08:44:15.000000 sindapi-0.0.7/sindapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 08:44:15.000000 sindapi-0.0.7/sindapi.egg-info/top_level.txt
```

### Comparing `sindapi-0.0.6/sindapi/sindmap/intersection/intersection.py` & `sindapi-0.0.7/sindapi/sindmap/intersection/intersection.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/lane/lane_segment.py` & `sindapi-0.0.7/sindapi/sindmap/lane/lane_segment.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/map_api.py` & `sindapi-0.0.7/sindapi/sindmap/map_api.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/pedestrian_crossing.py` & `sindapi-0.0.7/sindapi/sindmap/pedestrian_crossing.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/stretch/stretch.py` & `sindapi-0.0.7/sindapi/sindmap/stretch/stretch.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/traffic_light/traffic_light.py` & `sindapi-0.0.7/sindapi/sindmap/traffic_light/traffic_light.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindmap/utils/map_primitives.py` & `sindapi-0.0.7/sindapi/sindmap/utils/map_primitives.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi/sindtrack/data_schema.py` & `sindapi-0.0.7/sindapi/sindtrack/data_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,11 +126,11 @@
     """
 
     scenario_id: int
     record_id: str
     timestamps_ms: List[float]
     tracks: Dict[str, Track]
     focal_track_id: str
-    dynamic_map: SinDDynamicMap
     city_name: str
+    dynamic_map: Optional[SinDDynamicMap]
     map_id: Optional[str]
```

### Comparing `sindapi-0.0.6/sindapi/sindtrack/process_raw_data.py` & `sindapi-0.0.7/sindapi/sindtrack/process_raw_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,25 +83,26 @@
 
     focal_track_id = None
     for track in tracks.values():
         if track.category.value >= TrackCategory.SCORED_TRACK.value and track.object_type == ObjectType.CAR:
             focal_track_id = track.track_id
             break
 
+    # TODO: need to debug at line 228
     dynamic_map = get_dynamic_map(record_path, timestamps_ms)
 
     sind_scenario = SinDScenario(
         scenario_id=scenario_id,
         record_id=record_id,
         timestamps_ms=timestamps_ms,
         tracks=tracks,
         focal_track_id=focal_track_id,
-        dynamic_map=dynamic_map,
         city_name=city_name,
-        map_id=dynamic_map.map_id
+        # dynamic_map=dynamic_map,
+        # map_id=dynamic_map.map_id
     )
 
     return sind_scenario
 
 def get_tracks(record_path: Path, start_frame: int, end_frame: int) -> Dict[str, Track]:
     df_vehicle_meta = pd.read_csv(record_path / 'Veh_tracks_meta.csv')
     df_vehicle_meta = df_vehicle_meta[
```

### Comparing `sindapi-0.0.6/sindapi/sindtrack/utils/constants.py` & `sindapi-0.0.7/sindapi/sindtrack/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.6/sindapi.egg-info/SOURCES.txt` & `sindapi-0.0.7/sindapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*
