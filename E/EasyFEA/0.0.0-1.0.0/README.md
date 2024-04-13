# Comparing `tmp/EasyFEA-0.0.0.tar.gz` & `tmp/EasyFEA-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyFEA-0.0.0.tar", last modified: Sat Feb 10 16:58:01 2024, max compression
+gzip compressed data, was "EasyFEA-1.0.0.tar", last modified: Sat Apr 13 16:20:06 2024, max compression
```

## Comparing `EasyFEA-0.0.0.tar` & `EasyFEA-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,130 @@
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-02-10 16:58:01.182829 EasyFEA-0.0.0/
--rw-r--r--   0 matnoel    (501) staff       (20)     1057 2024-02-10 13:44:49.000000 EasyFEA-0.0.0/LICENSE
--rw-r--r--   0 matnoel    (501) staff       (20)      207 2024-02-10 16:58:01.182653 EasyFEA-0.0.0/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)     2555 2024-02-10 14:00:52.000000 EasyFEA-0.0.0/README.md
--rw-r--r--   0 matnoel    (501) staff       (20)      299 2024-02-10 16:26:55.000000 EasyFEA-0.0.0/pyproject.toml
--rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-02-10 16:58:01.182870 EasyFEA-0.0.0/setup.cfg
--rw-r--r--   0 matnoel    (501) staff       (20)       36 2024-02-10 16:57:49.000000 EasyFEA-0.0.0/setup.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-02-10 16:58:01.181259 EasyFEA-0.0.0/src/
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-02-10 16:58:01.181869 EasyFEA-0.0.0/src/EasyFEA/
--rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-02-10 16:25:47.000000 EasyFEA-0.0.0/src/EasyFEA/__init__.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-02-10 16:58:01.182475 EasyFEA-0.0.0/src/EasyFEA.egg-info/
--rw-r--r--   0 matnoel    (501) staff       (20)      207 2024-02-10 16:58:01.000000 EasyFEA-0.0.0/src/EasyFEA.egg-info/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)      205 2024-02-10 16:58:01.000000 EasyFEA-0.0.0/src/EasyFEA.egg-info/SOURCES.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-02-10 16:58:01.000000 EasyFEA-0.0.0/src/EasyFEA.egg-info/dependency_links.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-02-10 16:58:01.000000 EasyFEA-0.0.0/src/EasyFEA.egg-info/top_level.txt
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.325507 EasyFEA-1.0.0/
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.310731 EasyFEA-1.0.0/EasyFEA/
+-rw-r--r--   0 matnoel    (501) staff       (20)    35934 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/Geoms.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      807 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/Materials.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1065 2024-04-13 15:37:09.000000 EasyFEA-1.0.0/EasyFEA/Simulations.py
+-rw-r--r--   0 matnoel    (501) staff       (20)       21 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/__about__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      942 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/__init__.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.312361 EasyFEA-1.0.0/EasyFEA/fem/
+-rw-r--r--   0 matnoel    (501) staff       (20)      260 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6176 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/_boundary_conditions.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11030 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/_gauss.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    65546 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/_gmsh_interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    68300 2024-04-13 14:42:08.000000 EasyFEA-1.0.0/EasyFEA/fem/_group_elems.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    37173 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/_mesh.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1592 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.313345 EasyFEA-1.0.0/EasyFEA/fem/elems/
+-rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    23110 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_hexa.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      783 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_point.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    13576 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_prism.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4833 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_quad.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    12816 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_seg.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7200 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_tetra.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11843 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/fem/elems/_tri.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.314198 EasyFEA-1.0.0/EasyFEA/materials/
+-rw-r--r--   0 matnoel    (501) staff       (20)      293 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    10778 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    24303 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    49708 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2239 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    17138 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/materials/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.315422 EasyFEA-1.0.0/EasyFEA/simulations/
+-rw-r--r--   0 matnoel    (501) staff       (20)    14044 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/Solvers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    30212 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19526 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_dic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19227 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    30902 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    58113 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_simu.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6780 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/simulations/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2471 2024-04-13 14:48:04.000000 EasyFEA-1.0.0/EasyFEA/simulations/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.316472 EasyFEA-1.0.0/EasyFEA/utilities/
+-rw-r--r--   0 matnoel    (501) staff       (20)    46023 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/Display.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3151 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/Folder.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7771 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/Numba_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9432 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/Paraview_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    27270 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/PyVista_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)       21 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1348 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/_observers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6856 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/EasyFEA/utilities/_tic.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.311408 EasyFEA-1.0.0/EasyFEA.egg-info/
+-rw-r--r--   0 matnoel    (501) staff       (20)    47275 2024-04-13 16:20:06.000000 EasyFEA-1.0.0/EasyFEA.egg-info/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     3129 2024-04-13 16:20:06.000000 EasyFEA-1.0.0/EasyFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-04-13 16:20:06.000000 EasyFEA-1.0.0/EasyFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)      132 2024-04-13 16:20:06.000000 EasyFEA-1.0.0/EasyFEA.egg-info/requires.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-04-13 16:20:06.000000 EasyFEA-1.0.0/EasyFEA.egg-info/top_level.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    35149 2024-04-10 14:50:23.000000 EasyFEA-1.0.0/LICENSE.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    47275 2024-04-13 16:20:06.325340 EasyFEA-1.0.0/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     5803 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/README.md
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.316707 EasyFEA-1.0.0/examples/
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.317328 EasyFEA-1.0.0/examples/Beam/
+-rw-r--r--   0 matnoel    (501) staff       (20)     2825 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Beam/Beam1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3388 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Beam/Beam2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3083 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Beam/Beam3.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2199 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Beam/Beam4.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3167 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Beam/Beam5.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.317988 EasyFEA-1.0.0/examples/Contact/
+-rw-r--r--   0 matnoel    (501) staff       (20)     6027 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Contact/Contact1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5964 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Contact/Contact2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4137 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Contact/Contact3.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.318737 EasyFEA-1.0.0/examples/Dynamic/
+-rw-r--r--   0 matnoel    (501) staff       (20)     4119 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Dynamic/Dyna1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3307 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Dynamic/Dyna2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2759 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Dynamic/Modal1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5547 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Dynamic/Modal2.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.319707 EasyFEA-1.0.0/examples/Elastic/
+-rw-r--r--   0 matnoel    (501) staff       (20)     2194 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/Elas1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2441 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/Elas2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2252 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/Elas3.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3833 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/Elas4.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4133 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/HyperElasticity.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2642 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/PlateWithHole.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3463 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Elastic/PressurizedTube.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1139 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/HelloWorld.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.320830 EasyFEA-1.0.0/examples/Identification/
+-rw-r--r--   0 matnoel    (501) staff       (20)     9219 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/FEMU1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    12098 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/FEMU2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5860 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/Homog1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9673 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/Homog2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6388 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/HomogFullField.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    25437 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/VFM1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5357 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Identification/VFM2.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.320976 EasyFEA-1.0.0/examples/Machine learning/
+-rw-r--r--   0 matnoel    (501) staff       (20)     1257 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Machine learning/k_means.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.323209 EasyFEA-1.0.0/examples/Meshes/
+-rw-r--r--   0 matnoel    (501) staff       (20)      664 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1287 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh10.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      575 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh11.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      731 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1223 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh3.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1321 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh4.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2571 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh5.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1092 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh6.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2937 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh7.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3299 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh8.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9918 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/Mesh9.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7540 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/MeshConvergence.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3074 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/MeshOptim0.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4779 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/MeshOptim1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4735 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/MeshOptim2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5424 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Meshes/MeshOptim3.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.324310 EasyFEA-1.0.0/examples/Phasefield/
+-rw-r--r--   0 matnoel    (501) staff       (20)     5970 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/L_Shape.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.324771 EasyFEA-1.0.0/examples/Phasefield/PlateWithHole/
+-rw-r--r--   0 matnoel    (501) staff       (20)     4521 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/PlateWithHole/Dimension.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9930 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/PlateWithHole/Energy.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     4135 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/PlateWithHole/Loading.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    10441 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/PlateWithHole.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6450 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/PostProcess.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9352 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/Shear.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11176 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/Tension.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3601 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/Tension_Inclusions.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5941 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Phasefield/Traction_Wood.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:20:06.325057 EasyFEA-1.0.0/examples/Thermal/
+-rw-r--r--   0 matnoel    (501) staff       (20)     3424 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Thermal/Thermal1.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3091 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/Thermal/Thermal2.py
+-rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.0/examples/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1336 2024-04-13 16:18:55.000000 EasyFEA-1.0.0/pyproject.toml
+-rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-04-13 16:20:06.325553 EasyFEA-1.0.0/setup.cfg
+-rw-r--r--   0 matnoel    (501) staff       (20)       61 2024-03-19 17:45:45.000000 EasyFEA-1.0.0/setup.py
```

