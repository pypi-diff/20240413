# Comparing `tmp/dune_rivals-0.3.1.tar.gz` & `tmp/dune_rivals-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.1.tar", last modified: Sat Apr 13 17:59:41 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.2.tar", last modified: Sat Apr 13 18:24:04 2024, max compression
```

## Comparing `dune_rivals-0.3.1.tar` & `dune_rivals-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 17:59:41.405784 dune_rivals-0.3.1/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 17:59:41.405307 dune_rivals-0.3.1/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.1/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 17:59:41.404875 dune_rivals-0.3.1/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 17:59:41.000000 dune_rivals-0.3.1/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 17:59:41.000000 dune_rivals-0.3.1/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 17:59:41.000000 dune_rivals-0.3.1/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 17:59:41.000000 dune_rivals-0.3.1/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    16240 2024-04-13 17:58:43.000000 dune_rivals-0.3.1/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 17:59:31.000000 dune_rivals-0.3.1/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 17:59:41.405882 dune_rivals-0.3.1/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:24:04.238192 dune_rivals-0.3.2/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:24:04.237602 dune_rivals-0.3.2/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.2/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:24:04.237097 dune_rivals-0.3.2/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    16223 2024-04-13 18:23:32.000000 dune_rivals-0.3.2/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 18:23:59.000000 dune_rivals-0.3.2/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 18:24:04.238327 dune_rivals-0.3.2/setup.cfg
```

### Comparing `dune_rivals-0.3.1/dune_rivals.py` & `dune_rivals-0.3.2/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             print(f"{self.name} fetching spice field object from S3 for {(self.i, self.j)}")
             time.sleep(SLEEP_SECONDS_READ_FROM_S3)
         else:
             print(f"{self.name} fetching spice field object from OBJECT STORE for {(self.i, self.j)}")
 
         # get spice field object
         t0 = time.time()
-        spice_field_refs = ray.get(self.gamestate.get_spice_field_refs.remote("southern"))  # TODO: fix for h2h
+        spice_field_ref = ray.get(self.gamestate.get_spice_field_ref.remote("southern", self.i, self.j))  # TODO: fix for h2h
         t1 = time.time()
-        spice_field = ray.get(spice_field_refs[(self.i, self.j)])
+        spice_field = ray.get(spice_field_ref)
         t2 = time.time()
         print(f"FETCH SPICE FIELD REFS: {t1 - t0}")
         print(f"FETCH SPICE FIELD: {t2 - t1}")
 
         # check if spice field object can be written to
         write_order = self.order_map[(self.i, self.j)]
         try:
@@ -115,15 +115,15 @@
         # sleep for travel duration
         time.sleep(total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD)
 
         # update coordinates
         self.i = new_i
         self.j = new_j
 
-        print(f"movement sleep for: {time.sleep(total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD)}")
+        print(f"movement sleep for: {total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD}")
 
 
 @ray.remote(num_cpus=0.1, resources={"worker3": 1e-4})
 class Noop12(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 12
```

