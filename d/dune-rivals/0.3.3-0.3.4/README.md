# Comparing `tmp/dune_rivals-0.3.3.tar.gz` & `tmp/dune_rivals-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.3.tar", last modified: Sat Apr 13 18:28:19 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.4.tar", last modified: Sat Apr 13 21:49:52 2024, max compression
```

## Comparing `dune_rivals-0.3.3.tar` & `dune_rivals-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:28:19.997154 dune_rivals-0.3.3/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:28:19.996150 dune_rivals-0.3.3/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.3/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:28:19.995554 dune_rivals-0.3.3/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    16222 2024-04-13 18:27:49.000000 dune_rivals-0.3.3/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 18:28:15.000000 dune_rivals-0.3.3/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 18:28:19.997351 dune_rivals-0.3.3/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:49:52.488554 dune_rivals-0.3.4/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:49:52.488136 dune_rivals-0.3.4/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.4/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:49:52.487688 dune_rivals-0.3.4/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23266 2024-04-13 21:49:10.000000 dune_rivals-0.3.4/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:49:43.000000 dune_rivals-0.3.4/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:49:52.488643 dune_rivals-0.3.4/setup.cfg
```

### Comparing `dune_rivals-0.3.3/dune_rivals.py` & `dune_rivals-0.3.4/dune_rivals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ray
 import time
 import numpy as np
+import scipy as sp
 
 # TODO: double check that obj. store read is < 0.1 (S3 read time)
 # DEFINITIONS
 SLEEP_SECONDS_PER_TRAVEL_COORD = 1e-5
 SLEEP_SECONDS_READ_FROM_S3     = 0.100
 SLEEP_SECONDS_NOT_ON_SPICE     = 1.000
 
@@ -266,16 +267,16 @@
         self.order_map = order_map
 
         # confirm that other actors have set variables
         all_ready = False
         while not all_ready:
             all_ready = True
             for id in [2, 3, 4]:
-                goose = ray.get_actor(f"GlossuRabban{id}")
-                loc_map = ray.get(goose.get_spice_loc_map.remote())
+                warrior = ray.get_actor(f"GlossuRabban{id}")
+                loc_map = ray.get(warrior.get_spice_loc_map.remote())
                 all_ready = all_ready and (loc_map is not None)
 
         def destroy_all_spice_of_file_type(file_type):
             # get spice locations and iterate over them to destroy spice
             spice = np.where(spice_file_map==file_type)
             for i, j in zip(spice[0], spice[1]):
                 # move warriors that are needed to location (i,j)
@@ -323,73 +324,245 @@
 
 ##############################################################################################
 ################################         Feyd Rautha          ################################
 ##############################################################################################
 class BaseFeydRautha(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
+        self.id = None
+        self.free = None
+        self.num_singletons = None
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
+
+    def get_num_singletons(self, id):
+        if id == self.id:
+            return self.num_singletons
+        else:
+            warrior = ray.get_actor(f"FeydRautha{id}")
+            return ray.get(warrior.get_num_singletons(id))
+
+    def is_free(self):
+        return self.free
+
+    def destroy_spice_field_with_retry(self):
+        self.free = False
+        destroyed = False
+        while not destroyed:
+            destroyed = self._destroy_spice_field()
+            time.sleep(0.0001)
+        
+        self.free = True
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        self.free = False
+
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
-    def get_spice_loc_map(self):
-        return self.spice_loc_map
+        # construct spice arr w/this warrior's fields for finding nearest points quickly
+        def get_warrior_spice_arr(file_type):
+            locs, singletons = [], []
+            spice = np.where(self.spice_file_map==file_type)
+            idx = 0
+            for i, j in zip(spice[0], spice[1]):
+                warriors = self.order_map[(i, j)]
+                if self.id in warriors:
+                    locs.append((i, j))
+                    if len(warriors) == 1:
+                        singletons.append(idx)
+                    idx += 1
+            return np.array(locs), np.array(singletons)
+
+        obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
+        self.num_singletons = len(obj_singletons)
+
+        # get num_singletons from every warrior to determine who leader will be (later);
+        # everyone will compute the same leader
+        leader, fewest_singletons = -1, np.inf
+        for id in [1, 2, 3, 4]:
+            num_singletons = self.get_num_singletons(id)
+            if num_singletons < fewest_singletons:
+                fewest_singletons = num_singletons
+                leader = id
+
+        print(f"LEADER WILL BE: {leader}")
+
+        # destroy all the obj singletons associated with this warrior
+        for i, j in obj_spice_arr[obj_singletons]:
+            self._ride_sandworm(i, j)
+            self.destroy_block(self.id)
+
+        # remove deleted fields from obj_spice_arr
+        obj_spice_arr = np.delete(obj_spice_arr, obj_singletons, axis=0)
+
+        # once everyone is finished, leader will run the show
+        self.free = True
+        if self.id == leader:
+            # destroy remaining obj spice
+            first_pass, skipped_lst = True, []
+            while first_pass or len(skipped_lst) > 0:
+                first_pass = False
+
+                for loc in obj_spice_arr:
+                    i, j = loc[0], loc[1]
+                    warrior_ids = self.order_map[(i,j)]
+
+                    # if one of warrior_ids isn't free then skip
+                    not_free = False
+                    for warrior_id in warrior_ids:
+                        if not ray.get(ray.get_actor(f"FeydRautha{warrior_id}").is_free.remote()):
+                            skipped_lst.append(loc)
+                            not_free = True
+                            break
+                    
+                    if not_free:
+                        continue
+
+                    # otherwise, move warriors that are needed to location (i,j)
+                    for warrior_id in warrior_ids:
+                        if warrior_id != 1:
+                            warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                            warrior._ride_sandworm.remote(i, j)
+                        else:
+                            self._ride_sandworm(i, j)
+
+                    # destroy spice in asynchronous fashion
+                    for warrior_id in warrior_ids:
+                        if warrior_id != 1:
+                            warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                            warrior.destroy_spice_field_with_retry.remote()
+                        else:
+                            self.destroy_spice_field_with_retry()
+
+            # destroy s3 spice
+            # get spice locations and iterate over them to destroy spice
+            spice = np.where(spice_file_map==S3_FILE)
+            for i, j in zip(spice[0], spice[1]):
+                # move warriors that are needed to location (i,j)
+                warrior_ids = self.order_map[(i,j)]
+                for warrior_id in warrior_ids:
+                    if warrior_id != 1:
+                        warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                        warrior._ride_sandworm.remote(i, j)
+                    else:
+                        self._ride_sandworm(i, j)
+
+                # destroy spice in synchronous fashion
+                for warrior_id in warrior_ids:
+                    if warrior_id != 1:
+                        warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                        ray.get(warrior._destroy_spice_field.remote())
+                    else:
+                        self._destroy_spice_field()
 
 
 @ray.remote(num_cpus=0.8, name="FeydRautha1", resources={"worker3": 1e-4})
 class FeydRautha1(BaseFeydRautha):
     """
-    FeydRautha is an implementation which uses greedy cost estimation to select which
-    spice field to destroy. Each worker computes its easiest spice targt to destroy, with
-    a coarse estimate of the time it would take to destroy fields which require multiple
-    actors. Actors then vote on which field to destroy next. If an actor can destroy a field
-    in parallel to the current easiest field being destroyed, then it may do so.
+    FeydRautha computes the distance from each worker to its top-k nearest spice fields
+    and coordinates which one(s) to destroy. The (k/2)-kth closest fields are selected to be destroyed,
+    and if any actors which are not needed can be used to destroy one of the [k/2, k] fields in parallel
+    then that is done as well.
     """
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
         self.name = "FeydRautha1"
+        self.k = 10
 
-    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        # set these state variables
-        self.spice_loc_map = spice_loc_map
-        self.spice_file_map = spice_file_map
-        self.order_map = order_map
-
-        # confirm that other actors have set variables
-        all_ready = False
-        while not all_ready:
-            all_ready = True
-            for id in [2, 3, 4]:
-                goose = ray.get_actor(f"FeydRautha{id}")
-                loc_map = ray.get(goose.get_spice_loc_map.remote())
-                all_ready = all_ready and (loc_map is not None)
-
-        # get spice locations and iterate over them to destroy spice
-        out = np.where(spice_loc_map==1)
-        for i, j in zip(out[0], out[1]):
-            # move Geese that are needed to location (i,j)
-            geese_ids = self.order_map[(i,j)]
-            for goose_id in geese_ids:
-                if goose_id != 1:
-                    goose = ray.get_actor(f"FeydRautha{goose_id}")
-                    goose._ride_sandworm.remote(i, j)
-                else:
-                    self._ride_sandworm(i, j)
-
-            # destroy spice in synchronous fashion
-            for goose_id in geese_ids:
-                if goose_id != 1:
-                    goose = ray.get_actor(f"FeydRautha{goose_id}")
-                    ray.get(goose._destroy_spice_field.remote())
-                else:
-                    self._destroy_spice_field()
+    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+    #     # set these state variables
+    #     self.spice_loc_map = spice_loc_map
+    #     self.spice_file_map = spice_file_map
+    #     self.order_map = order_map
+
+    #     # construct spice arr w/this warrior's fields for finding nearest points quickly
+    #     def get_warrior_spice_arr(file_type):
+    #         locs, singletons = [], []
+    #         spice = np.where(self.spice_file_map==file_type)
+    #         idx = 0
+    #         for i, j in zip(spice[0], spice[1]):
+    #             warriors = self.order_map[(i, j)]
+    #             if self.id in warriors:
+    #                 locs.append((i, j))
+    #                 if len(warriors) == 1:
+    #                     singletons.append(idx)
+    #                 idx += 1
+    #         return np.array(locs), np.array(singletons)
+
+    #     obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
+
+    #     # destroy all the obj singletons associated with this warrior
+    #     for i, j in obj_spice_arr[obj_singletons]:
+    #         self._ride_sandworm(i, j)
+    #         self.destroy_block(self.id)
+
+    #     # loop forever and destroy spice
+    #     while len(obj_spice_arr) > 0:
+    #         # construct spatial tree
+    #         obj_spatial_tree = sp.spatial.KDTree(obj_spice_arr)
+
+    #         # get location of each warrior
+    #         other_warrior_coords = ray.get([
+    #             ray.get_actor(f"FeydRautha{id}").get_location.remote()
+    #             for id in [2, 3, 4]
+    #         ])
+    #         warrior_coords = [(self.i, self.j)] + other_warrior_coords
+
+    #         # aggregate closest [k/2, k] spice fields for each worker
+    #         close_obj_locs, close_obj_indices = [], []
+    #         for i, j in warrior_coords:
+    #             pt = [i, j]
+    #             close_obj_loc_idxs = obj_spatial_tree.query(pt, k=self.k)[1][int(self.k/2):]
+    #             close_obj_locs.extend(obj_spice_arr[close_obj_loc_idxs])
+    #             close_obj_indices.extend(close_obj_loc_idxs)
+
+    #         # filter for unique set of locations and indices
+    #         close_obj_locs = np.unique(np.array(close_obj_locs), axis=0)
+    #         close_obj_indices = np.unique(np.array(close_obj_indices), axis=0)
+
+    #         # destroy all singletons first
+    #         for loc in close_obj_locs:
+    #             i, j = loc[0], loc[1]
+    #             warriors = self.order_map[(i, j)]
+    #             if len(warriors) == 1:
+    #                 command_field_destroy(warriors[0])
+
+    #         # then destroy all doubles
+
+
+    #         obj_spice_arr = np.delete(obj_spice_arr, close_obj_indices, axis=0)
+
+
+    #     # movement cost for each worker in order map + 1ms * num workers (obj read) [+ 100ms * num workers (s3_file read)]
+
+    #     # 
+
+    #     out = np.where(spice_loc_map==1)
+    #     for i, j in zip(out[0], out[1]):
+    #         # move warriors that are needed to location (i,j)
+    #         warrior_ids = self.order_map[(i,j)]
+    #         for warrior_id in warrior_ids:
+    #             if warrior_id != 1:
+    #                 warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+    #                 warrior._ride_sandworm.remote(i, j)
+    #             else:
+    #                 self._ride_sandworm(i, j)
+
+    #         # destroy spice in synchronous fashion
+    #         for warrior_id in warrior_ids:
+    #             if warrior_id != 1:
+    #                 warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+    #                 ray.get(warrior._destroy_spice_field.remote())
+    #             else:
+    #                 self._destroy_spice_field()
 
 
 @ray.remote(num_cpus=0.8, name="FeydRautha2", resources={"worker3": 1e-4})
 class FeydRautha2(BaseFeydRautha):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
```

