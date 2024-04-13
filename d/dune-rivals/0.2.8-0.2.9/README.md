# Comparing `tmp/dune_rivals-0.2.8.tar.gz` & `tmp/dune_rivals-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.8.tar", last modified: Fri Apr 12 21:07:12 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.9.tar", last modified: Fri Apr 12 21:11:54 2024, max compression
```

## Comparing `dune_rivals-0.2.8.tar` & `dune_rivals-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:07:12.182103 dune_rivals-0.2.8/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:07:12.181638 dune_rivals-0.2.8/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.8/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:07:12.181193 dune_rivals-0.2.8/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10473 2024-04-12 21:06:32.000000 dune_rivals-0.2.8/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 21:07:06.000000 dune_rivals-0.2.8/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 21:07:12.182222 dune_rivals-0.2.8/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:11:54.210576 dune_rivals-0.2.9/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:11:54.210170 dune_rivals-0.2.9/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.9/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:11:54.209751 dune_rivals-0.2.9/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10823 2024-04-12 21:10:43.000000 dune_rivals-0.2.9/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 21:11:48.000000 dune_rivals-0.2.9/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 21:11:54.210666 dune_rivals-0.2.9/setup.cfg
```

### Comparing `dune_rivals-0.2.8/dune_rivals.py` & `dune_rivals-0.2.9/dune_rivals.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,27 +134,36 @@
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
 
 ##############################################################################################
 ################################         Silly Goose          ################################
 ##############################################################################################
-# class BaseSillyGoose(BaseRivalActor):
-#     def __init__(self, payload: str):
-#         super().__init__(payload)
-
-#     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-#         # set these state variables
-#         self.spice_loc_map = spice_loc_map
-#         self.spice_file_map = spice_file_map
-#         self.order_map = order_map
+class BaseSillyGoose(BaseRivalActor):
+    def __init__(self, payload: str):
+        super().__init__(payload)
+
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
+
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose1", resources={"worker3": 1e-4})
-class SillyGoose1(BaseRivalActor):
+class SillyGoose1(BaseSillyGoose):
     """
     SillyGoose1 is the leader. It picks which spice field to target and moves all
     other Geese to that target. Once the necessary Geese arrive, it instructs the
     Geese to destroy spice in the specified order.
     """
     def __init__(self, payload: str):
         super().__init__(payload)
@@ -190,70 +199,70 @@
 
             # destroy spice in synchronous fashion
             for goose_id in geese_ids:
                 if goose_id != 1:
                     goose = ray.get_actor(f"SillyGoose{goose_id}")
                     ray.get(goose._destroy_spice_field.remote())
                 else:
-                    ray.get(self._destroy_spice_field())
+                    self._destroy_spice_field()
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
-class SillyGoose2(BaseRivalActor):
+class SillyGoose2(BaseSillyGoose):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
         self.name = "SillyGoose2"
     
-    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        print(f"SillyGoose{self.id} starting")
-        # set these state variables
-        self.spice_loc_map = spice_loc_map
-        self.spice_file_map = spice_file_map
-        self.order_map = order_map
-        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+    #     print(f"SillyGoose{self.id} starting")
+    #     # set these state variables
+    #     self.spice_loc_map = spice_loc_map
+    #     self.spice_file_map = spice_file_map
+    #     self.order_map = order_map
+    #     print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
 
-    def get_spice_loc_map(self):
-        return self.spice_loc_map
+    # def get_spice_loc_map(self):
+    #     return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
-class SillyGoose3(BaseRivalActor):
+class SillyGoose3(BaseSillyGoose):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
         self.name = "SillyGoose3"
     
-    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        print(f"SillyGoose{self.id} starting")
-        # set these state variables
-        self.spice_loc_map = spice_loc_map
-        self.spice_file_map = spice_file_map
-        self.order_map = order_map
-        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+    #     print(f"SillyGoose{self.id} starting")
+    #     # set these state variables
+    #     self.spice_loc_map = spice_loc_map
+    #     self.spice_file_map = spice_file_map
+    #     self.order_map = order_map
+    #     print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
 
-    def get_spice_loc_map(self):
-        return self.spice_loc_map
+    # def get_spice_loc_map(self):
+    #     return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
-class SillyGoose4(BaseRivalActor):
+class SillyGoose4(BaseSillyGoose):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
         self.name = "SillyGoose4"
 
-    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        print(f"SillyGoose{self.id} starting")
-        # set these state variables
-        self.spice_loc_map = spice_loc_map
-        self.spice_file_map = spice_file_map
-        self.order_map = order_map
-        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+    # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+    #     print(f"SillyGoose{self.id} starting")
+    #     # set these state variables
+    #     self.spice_loc_map = spice_loc_map
+    #     self.spice_file_map = spice_file_map
+    #     self.order_map = order_map
+    #     print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
 
-    def get_spice_loc_map(self):
-        return self.spice_loc_map
+    # def get_spice_loc_map(self):
+    #     return self.spice_loc_map
 
 ##############################################################################################
 ###############################         Glossu Rabban          ###############################
 ##############################################################################################
 
 
 ##############################################################################################
```

