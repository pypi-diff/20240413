# Comparing `tmp/rwmapeditor_exgcdwu-1.1.2.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.1.2.tar", last modified: Sun Apr  7 14:27:04 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.2.0.tar", last modified: Sat Apr 13 10:38:07 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.1.2.tar` & `rwmapeditor_exgcdwu-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.601052 rwmapeditor_exgcdwu-1.1.2/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.601052 rwmapeditor_exgcdwu-1.1.2/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_default_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-07 14:27:04.000000 rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 14:27:04.000000 rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:27:04.000000 rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 14:27:04.000000 rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 14:27:04.605052 rwmapeditor_exgcdwu-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-07 14:26:45.000000 rwmapeditor_exgcdwu-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/_object_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/default_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tobject_group_COP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tobject_group_COP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/LICENSE` & `rwmapeditor_exgcdwu-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1.2/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.1.2
+Version: 1.2.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,49 +19,56 @@
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
+地块组框架已完成。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
 
 1.使用地图编辑器(Tiled,notTiled)创建新地图，确定大小。
 
 2.手动载入地块集
 
-3.即可使用python库自动改变地块和宾语
+3.手动创建所需的地块层和宾语层
+
+4.即可使用python库自动改变地块和宾语
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
-map_name = 'example_mission.tmx'
-map_name_out = 'example_mission(1).tmx'
-
+map_name = '[p2]example_skirmish_(2p).tmx'
+map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+print(mygraph)
 
-print(mygraph.output_str())
-
-mygraph.addObject("Triggers", {"id": "100","type": "unitAdd", "x": "1000", "y":"1000", "width": "20", "height": "20"}, {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"20s"})
+mygraph.addObject(
+    "Triggers", 
+    {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
+    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
+mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
+
 mygraph.write_file(map_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/README.md` & `rwmapeditor_exgcdwu-1.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -9,49 +9,56 @@
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
+地块组框架已完成。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
 
 1.使用地图编辑器(Tiled,notTiled)创建新地图，确定大小。
 
 2.手动载入地块集
 
-3.即可使用python库自动改变地块和宾语
+3.手动创建所需的地块层和宾语层
+
+4.即可使用python库自动改变地块和宾语
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
-map_name = 'example_mission.tmx'
-map_name_out = 'example_mission(1).tmx'
-
+map_name = '[p2]example_skirmish_(2p).tmx'
+map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+print(mygraph)
 
-print(mygraph.output_str())
-
-mygraph.addObject("Triggers", {"id": "100","type": "unitAdd", "x": "1000", "y":"1000", "width": "20", "height": "20"}, {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"20s"})
+mygraph.addObject(
+    "Triggers", 
+    {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
+    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
+mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
+
 mygraph.write_file(map_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_objectgroup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 """
 
 import xml.etree.ElementTree as et
 
 import rwmap._util as utility
 import rwmap._frame as frame
+from rwmap._case._object import TObject
 
 class ObjectGroup(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, object_list:list[frame.ElementProperties])->None:
+    def __init__(self, properties:frame.ElementProperties, object_list:list[TObject])->None:
         super().__init__(properties)
         self._object_list = object_list
 
     def __iter__(self):
         return self._object_list
 
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
         properties = frame.ElementProperties.init_etElement(root)
-        _object_list = [frame.ElementProperties.init_etElement(tobject) for tobject in root if tobject.tag == "object"]
-        return cls(properties, _object_list)
+        object_list = [TObject.init_etElement(tobject) for tobject in root if tobject.tag == "object"]
+        return cls(properties, object_list)
     
     def output_str(self, objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, -1)]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
@@ -34,10 +35,10 @@
         self._properties.output_etElement(root)
         for tobject in self._object_list:
             tobject_element = et.Element("object")
             tobject.output_etElement(tobject_element)
             root.append(tobject_element)
         return root
     
-    def addObject(self, default_properties:dict[str, str], optional_properties :dict[str, str])->None:
-        self._object_list.append(frame.ElementProperties("object", default_properties, optional_properties))
+    def addObject(self, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {}, other_properties:list[et.Element] = [])->None:
+        self._object_list.append(TObject("object", default_properties, optional_properties, other_properties))
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_tileset.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 """
 
 """
 import xml.etree.ElementTree as et
 
 import rwmap._util as utility
 import rwmap._frame as frame
+import rwmap._exceptions as exception
 
 class TileSet(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, column:int, image_properties:frame.ElementProperties = None,
+    def __init__(self, properties:frame.ElementProperties, size:frame.Coordinate, image_properties:frame.ElementProperties = None,
                   png_text:str = None, tilelist_properties:list[frame.ElementProperties] = None)->None:
         super().__init__(properties)
-        self._column = column
+        self._size = size
         self._image_properties = image_properties
         self._png_text = png_text
         self._tilelist_properties = tilelist_properties
     @classmethod
     def init_etElement(cls, root:et.Element, rwmaps_dir:str)->None:
         png_text_pro = utility.get_etElement_callable_from_tag(root, "properties")
         png_text = utility.get_etElement_name_to_text_rm(png_text_pro, "embedded_png")
@@ -25,31 +26,37 @@
         tilelist_properties = None if tilelist_properties == [] else tilelist_properties
         
         if properties.returnDefaultProperty("columns") == None:
             source_file = properties.returnDefaultProperty("source")
 
             source = rwmaps_dir + source_file
             root = et.ElementTree(file=source).getroot()
-            if root.attrib.get("columns") == None:
-                tilewidth = int(root.attrib["tilewidth"])
-                image_element = utility.get_etElement_callable_from_tag(root, "image")
-                if image_element.attrib.get("width") == None:
-                    source_fa_dir = "/".join(source_file.split("/")[0:-1]) + "/"
-                    source_fa_dir = "" if source_fa_dir == "/" else source_fa_dir
-                    width = utility.image_width(rwmaps_dir + source_fa_dir + image_element.attrib["source"])
-                else:
-                    width = int(image_element.attrib["width"])
-                column = int(width / tilewidth)
+            #if root.attrib.get("columns") == None:
+            tilewidth = int(root.attrib["tilewidth"])
+            tileheight = int(root.attrib["tileheight"])
+            image_element = utility.get_etElement_callable_from_tag(root, "image")
+            if image_element.attrib.get("width") == None:
+                source_fa_dir = "/".join(source_file.split("/")[0:-1]) + "/"
+                source_fa_dir = "" if source_fa_dir == "/" else source_fa_dir
+                width = utility.image_width(rwmaps_dir + source_fa_dir + image_element.attrib["source"])
+                height = utility.image_height(rwmaps_dir + source_fa_dir + image_element.attrib["source"])
             else:
-                column = int(root.attrib["columns"])
+                width = int(image_element.attrib["width"])
+                height = int(image_element.attrib["height"])
+            column = int(width / tilewidth)
+            row = int(height / tileheight)
+            #else:
+                #column = int(root.attrib["columns"])
+                #row = int(int(root.attrib["tilecount"]) / column)
 
         else:
             column = int(properties.returnDefaultProperty("columns"))
-
-        return cls(properties, column, image_properties, png_text, tilelist_properties)
+            row = int(int(properties.returnDefaultProperty("tilecount")) / column)
+        size = frame.Coordinate(row, column)
+        return cls(properties, size, image_properties, png_text, tilelist_properties)
     
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         if self._image_properties != None:
             str_ans = str_ans + self._image_properties.output_str() + "\n"
         if self._png_text != None:
@@ -83,14 +90,20 @@
         tileset_name = self._properties.returnDefaultProperty("name")
         if tileset_name == None:
             tileset_name = self._properties.returnDefaultProperty("source")
         tileset_name = utility.str_slash_to_dot(tileset_name)
         return tileset_name
     
     def tileid(self, tile_grid:frame.Coordinate)->int:
-        id_now = tile_grid.id(self._column)
-        id_ans = int(self._properties.returnDefaultProperty("firstgid")) + id_now
+        if tile_grid < self._size:
+            id_now = tile_grid.id(self._size.y())
+            id_ans = int(self._properties.returnDefaultProperty("firstgid")) + id_now
+        else:
+            raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.output_name()}")
         return id_ans
+    
+    def isexist(self)->bool:
+        return self._properties.returnDefaultProperty("firstgid") != "0"
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_coordinate.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,25 +37,60 @@
             return Coordinate(self.x() - other.x(), self.y() - other.y())
         else:
             return Coordinate(self.x() - other, self.y() - other)
 
     def __neg__(self):
         return Coordinate(-self.x(), -self.y())
     
+    def _iterator(self):
+        for i in range(0, self.x()):
+            for j in range(0, self.y()):
+                yield Coordinate(i, j)
+
+    def __iter__(self):
+        return self._iterator()
+    
+    def __lt__(self, other)->int:
+        if self.x() < other.x() and self.y() < other.y():
+            return 1
+        elif self.x() > other.x() and self.y() > other.y():
+            return -1
+        else:
+            return 0
+    
 class Rectangle:
     def __init__(self, initialCoordinate:Coordinate, addCoordinate:Coordinate):
         self._initialCoordinate = initialCoordinate
         self._addCoordinate = addCoordinate
     
     def i(self):
         return self._initialCoordinate
 
     def a(self):
         return self._addCoordinate
     
     def e(self):
         return self._initialCoordinate + self._addCoordinate
     
-    def iterator(self):
+    def _iterator(self):
         for i in range(0, self._addCoordinate.x()):
             for j in range(0, self._addCoordinate.y()):
-                yield self._initialCoordinate + Coordinate(i, j)
+                coordinate_now = self._initialCoordinate + Coordinate(i, j)
+                yield Coordinate(coordinate_now.x(), coordinate_now.y())
+
+    def __iter__(self):
+        return self._iterator()
+    
+class TagCoordinate:
+    def __init__(self, tag:str, place:Coordinate):
+        self._place = place
+        self._tag = tag
+
+    @classmethod
+    def init_xy(cls, tag:str, x = 0, y = 0, dtype:str = np.int32):
+        return cls(tag, Coordinate(x, y, dtype))
+
+    def tag(self):
+        return self._tag
+    
+    def place(self):
+        return self._place
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_property.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import xml.etree.ElementTree as et
 import rwmap._util as utility
 
 class ElementProperties:
-    def __init__(self, tag:str, default_properties:dict[str, str], optional_properties:dict[str, str])->None:
+    def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {})->None:
         self.tag = tag
         self._default_properties = default_properties
         self._optional_properties = optional_properties
         
     @classmethod
     def init_etElement(cls, root:et.Element):
         if root == None:
             return None
-        return cls(root.tag, root.attrib, utility.get_etElement_properties(utility.get_etElement_callable_from_tag(root, "properties")))
+        optional_properties = utility.get_etElement_properties(utility.get_etElement_callable_from_tag(root, "properties"))
+        return cls(root.tag, root.attrib, optional_properties)
         
-    def output_etElement(self, root:et.Element)->None:
+    def output_etElement(self, root:et.Element)->et.Element:
         root.tag = self.tag
-        root.attrib = self._default_properties
-        root.append(utility.output_etElement_properties(self._optional_properties))
+        if self._default_properties != {}:
+            root.attrib = self._default_properties
+        if self._optional_properties != {}:
+            root.append(utility.output_etElement_properties(self._optional_properties))
         
     def output_str(self)->str:
         str_ans = ""
         str_ans = str_ans + self.tag + ":\n"
-        str_ans = str_ans + "_default_properties:" + str(self._default_properties) + "\n"
-        str_ans = str_ans + "_optional_properties:" + str(self._optional_properties) + "\n"
+        str_ans = str_ans + "default_properties:" + str(self._default_properties) + "\n"
+        str_ans = str_ans + "optional_properties:" + str(self._optional_properties) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
     
     def assignDefaultProperty(self, name:str, value:str):
         self._default_properties[name] = value
     
     def assignOptionalProperty(self, name:str, value:str):
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,10 +6,14 @@
 from rwmap._util._etElement_process import get_etElement_from_text_packed
 from rwmap._util._etElement_process import output_file_from_etElement
 from rwmap._util._etElement_process import output_etElement_properties
 
 from rwmap._util._str_util import indentstr_Tab
 from rwmap._util._str_util import str_slash_to_dot
 
+from rwmap._util._dict_util import dict_isconflict
+
 from rwmap._util._class_rel import get_ElementOri_from_list_by_name
 
-from rwmap._util._png_rel import image_width
+from rwmap._util._png_rel import image_width, image_height
+
+from rwmap._util._list_util import fill_list_of_list
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.1.2
+Version: 1.2.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,49 +19,56 @@
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
+地块组框架已完成。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
 
 1.使用地图编辑器(Tiled,notTiled)创建新地图，确定大小。
 
 2.手动载入地块集
 
-3.即可使用python库自动改变地块和宾语
+3.手动创建所需的地块层和宾语层
+
+4.即可使用python库自动改变地块和宾语
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
-map_name = 'example_mission.tmx'
-map_name_out = 'example_mission(1).tmx'
-
+map_name = '[p2]example_skirmish_(2p).tmx'
+map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+print(mygraph)
 
-print(mygraph.output_str())
-
-mygraph.addObject("Triggers", {"id": "100","type": "unitAdd", "x": "1000", "y":"1000", "width": "20", "height": "20"}, {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"20s"})
+mygraph.addObject(
+    "Triggers", 
+    {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
+    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
+mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
+
 mygraph.write_file(map_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.1.2/setup.py` & `rwmapeditor_exgcdwu-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 #import os
 from setuptools import setup, find_packages
 
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 #current_dir = os.path.dirname(__file__)
 #requirements = open(current_dir + '/requirements.txt').readlines()
 
 def readme():
     with open('README.md') as file:
         return file.read()
 
@@ -17,11 +17,11 @@
     name = 'rwmapeditor_exgcdwu',
     version = __version__,
     author = 'exgcdwu',
     author_email = '1006605318@qq.com',
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
     long_description = strreadme,
     long_description_content_type = "text/markdown",
-    packages = find_packages(exclude=["tests", "rwmap_data"]),
+    packages = find_packages(exclude=["tests"]),
     python_requires = '>=3.0.0'
     #,install_requires = requirements
 )
```

