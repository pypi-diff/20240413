# Comparing `tmp/glayout-0.0.1.tar.gz` & `tmp/glayout-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glayout-0.0.1.tar", last modified: Fri Apr 12 19:59:50 2024, max compression
+gzip compressed data, was "glayout-0.0.2.tar", last modified: Fri Apr 12 23:59:52 2024, max compression
```

## Comparing `glayout-0.0.1.tar` & `glayout-0.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.313376 glayout-0.0.1/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-12 19:59:50.313376 glayout-0.0.1/PKG-INFO
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.281376 glayout-0.0.1/glayout/
--rw-r--r--   0 labtob    (1000) labtob    (1000)       18 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/__init__.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.290376 glayout-0.0.1/glayout/components/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10577 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/diff_pair.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     7074 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/diff_pair_cmirrorbias.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10713 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/diff_pair_stackedcmirror.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    12982 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/differential_to_single_ended_converter.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    10212 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/opamp.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    15844 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/opamp_twostage.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4912 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/row_csamplifier_diff_to_single_ended_converter.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     3129 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/components/stacked_current_mirror.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.291376 glayout-0.0.1/glayout/pdk/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/__init__.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.293376 glayout-0.0.1/glayout/pdk/gf180_mapped/
--rw-r--r--   0 labtob    (1000) labtob    (1000)      150 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/gf180_mapped/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/gf180_mapped/gf180_mapped.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    13625 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/gf180_mapped/grules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    14510 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/mappedpdk.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.296376 glayout-0.0.1/glayout/pdk/sky130_mapped/
--rw-r--r--   0 labtob    (1000) labtob    (1000)      155 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/sky130_mapped/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    13642 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/sky130_mapped/grules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2781 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/sky130_mapped/sky130_add_npc.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1303 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/sky130_mapped/sky130_mapped.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.301376 glayout-0.0.1/glayout/pdk/util/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    12926 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/comp_utils.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2350 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/component_array_create.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    15988 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/port_utils.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5190 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/print_rules.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)      480 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/pdk/util/snap_to_grid.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.303376 glayout-0.0.1/glayout/placement/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/placement/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8520 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/placement/two_transistor_interdigitized.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     2241 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/placement/two_transistor_place.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.307376 glayout-0.0.1/glayout/primitives/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/primitives/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    28362 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/primitives/fet.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5503 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/primitives/guardring.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     5182 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/primitives/mimcap.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    14335 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/primitives/via_gen.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.310376 glayout-0.0.1/glayout/routing/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4469 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/routing/L_route.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/routing/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     9611 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/routing/c_route.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4488 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/routing/straight_route.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.311376 glayout-0.0.1/glayout/spice/
--rw-r--r--   0 labtob    (1000) labtob    (1000)       28 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/spice/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)    11224 2024-04-06 16:10:51.000000 glayout-0.0.1/glayout/spice/netlist.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 19:59:50.283376 glayout-0.0.1/glayout.egg-info/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-12 19:59:49.000000 glayout-0.0.1/glayout.egg-info/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1624 2024-04-12 19:59:50.000000 glayout-0.0.1/glayout.egg-info/SOURCES.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-12 19:59:49.000000 glayout-0.0.1/glayout.egg-info/dependency_links.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)       34 2024-04-12 19:59:49.000000 glayout-0.0.1/glayout.egg-info/requires.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        8 2024-04-12 19:59:49.000000 glayout-0.0.1/glayout.egg-info/top_level.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)       38 2024-04-12 19:59:50.314376 glayout-0.0.1/setup.cfg
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1063 2024-04-12 19:59:46.000000 glayout-0.0.1/setup.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.973925 glayout-0.0.2/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-12 23:59:52.973925 glayout-0.0.2/PKG-INFO
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.968925 glayout-0.0.2/glayout/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       18 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.970925 glayout-0.0.2/glayout/components/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10577 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/diff_pair.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     7074 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/diff_pair_cmirrorbias.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10713 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/diff_pair_stackedcmirror.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    12982 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/differential_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10212 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/opamp.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15844 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/opamp_twostage.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4912 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/row_csamplifier_diff_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3129 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/components/stacked_current_mirror.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.970925 glayout-0.0.2/glayout/pdk/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.970925 glayout-0.0.2/glayout/pdk/gf180_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      150 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/gf180_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/gf180_mapped/gf180_mapped.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13625 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/gf180_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14510 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/mappedpdk.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.971925 glayout-0.0.2/glayout/pdk/sky130_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      155 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/sky130_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13642 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/sky130_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2781 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/sky130_mapped/sky130_add_npc.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1303 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/sky130_mapped/sky130_mapped.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.971925 glayout-0.0.2/glayout/pdk/util/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    12926 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/comp_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2350 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/component_array_create.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15988 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/port_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5190 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/print_rules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      480 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/pdk/util/snap_to_grid.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.972925 glayout-0.0.2/glayout/placement/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/placement/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8520 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/placement/two_transistor_interdigitized.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2241 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/placement/two_transistor_place.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.972925 glayout-0.0.2/glayout/primitives/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/primitives/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    28362 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/primitives/fet.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5503 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/primitives/guardring.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5182 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/primitives/mimcap.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14335 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/primitives/via_gen.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.973925 glayout-0.0.2/glayout/routing/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4469 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/routing/L_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/routing/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     9611 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/routing/c_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4488 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/routing/straight_route.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.973925 glayout-0.0.2/glayout/spice/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       28 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/spice/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11224 2024-04-06 16:10:51.000000 glayout-0.0.2/glayout/spice/netlist.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-12 23:59:52.969925 glayout-0.0.2/glayout.egg-info/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    31914 2024-04-12 23:59:52.000000 glayout-0.0.2/glayout.egg-info/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1624 2024-04-12 23:59:52.000000 glayout-0.0.2/glayout.egg-info/SOURCES.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-12 23:59:52.000000 glayout-0.0.2/glayout.egg-info/dependency_links.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       34 2024-04-12 23:59:52.000000 glayout-0.0.2/glayout.egg-info/requires.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        8 2024-04-12 23:59:52.000000 glayout-0.0.2/glayout.egg-info/top_level.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       38 2024-04-12 23:59:52.973925 glayout-0.0.2/setup.cfg
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1128 2024-04-12 23:59:48.000000 glayout-0.0.2/setup.py
```

### Comparing `glayout-0.0.1/PKG-INFO` & `glayout-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glayout
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glayout-0.0.1/glayout/components/diff_pair.py` & `glayout-0.0.2/glayout/components/diff_pair.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/diff_pair_cmirrorbias.py` & `glayout-0.0.2/glayout/components/diff_pair_cmirrorbias.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/diff_pair_stackedcmirror.py` & `glayout-0.0.2/glayout/components/diff_pair_stackedcmirror.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/differential_to_single_ended_converter.py` & `glayout-0.0.2/glayout/components/differential_to_single_ended_converter.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/opamp.py` & `glayout-0.0.2/glayout/components/opamp.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/opamp_twostage.py` & `glayout-0.0.2/glayout/components/opamp_twostage.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/row_csamplifier_diff_to_single_ended_converter.py` & `glayout-0.0.2/glayout/components/row_csamplifier_diff_to_single_ended_converter.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/components/stacked_current_mirror.py` & `glayout-0.0.2/glayout/components/stacked_current_mirror.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/gf180_mapped/gf180_mapped.py` & `glayout-0.0.2/glayout/pdk/gf180_mapped/gf180_mapped.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/gf180_mapped/grules.py` & `glayout-0.0.2/glayout/pdk/gf180_mapped/grules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/mappedpdk.py` & `glayout-0.0.2/glayout/pdk/mappedpdk.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/sky130_mapped/grules.py` & `glayout-0.0.2/glayout/pdk/sky130_mapped/grules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/sky130_mapped/sky130_add_npc.py` & `glayout-0.0.2/glayout/pdk/sky130_mapped/sky130_add_npc.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/sky130_mapped/sky130_mapped.py` & `glayout-0.0.2/glayout/pdk/sky130_mapped/sky130_mapped.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/util/comp_utils.py` & `glayout-0.0.2/glayout/pdk/util/comp_utils.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/util/component_array_create.py` & `glayout-0.0.2/glayout/pdk/util/component_array_create.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/util/port_utils.py` & `glayout-0.0.2/glayout/pdk/util/port_utils.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/pdk/util/print_rules.py` & `glayout-0.0.2/glayout/pdk/util/print_rules.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/placement/two_transistor_interdigitized.py` & `glayout-0.0.2/glayout/placement/two_transistor_interdigitized.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/placement/two_transistor_place.py` & `glayout-0.0.2/glayout/placement/two_transistor_place.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/primitives/fet.py` & `glayout-0.0.2/glayout/primitives/fet.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/primitives/guardring.py` & `glayout-0.0.2/glayout/primitives/guardring.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/primitives/mimcap.py` & `glayout-0.0.2/glayout/primitives/mimcap.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/primitives/via_gen.py` & `glayout-0.0.2/glayout/primitives/via_gen.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/routing/L_route.py` & `glayout-0.0.2/glayout/routing/L_route.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/routing/c_route.py` & `glayout-0.0.2/glayout/routing/c_route.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/routing/straight_route.py` & `glayout-0.0.2/glayout/routing/straight_route.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout/spice/netlist.py` & `glayout-0.0.2/glayout/spice/netlist.py`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/glayout.egg-info/PKG-INFO` & `glayout-0.0.2/glayout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glayout
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glayout-0.0.1/glayout.egg-info/SOURCES.txt` & `glayout-0.0.2/glayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glayout-0.0.1/setup.py` & `glayout-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 def get_install_requires():
     with open("glayout/requirements.txt", "r") as f:
         return [line.strip() for line in f.readlines() if not line.startswith("-")]
 
 
 setup(
     name="glayout",
-    version="0.0.1",
+    version="0.0.2",
     url="https://github.com/idea-fasoc/OpenFASOC",
     license="MIT",
     author=" msaligane",
     author_email="mehdi@umich.edu",
     description="Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
     package_dir={"":"./"},
+    package_data={'glayout' :[]},
+    include_package_data=True,
     install_requires=get_install_requires(),
     python_requires=">=3.10",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.10",
```

