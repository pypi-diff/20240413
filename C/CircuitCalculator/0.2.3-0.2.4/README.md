# Comparing `tmp/CircuitCalculator-0.2.3.tar.gz` & `tmp/circuitcalculator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircuitCalculator-0.2.3.tar", last modified: Mon Mar  4 17:24:03 2024, max compression
+gzip compressed data, was "circuitcalculator-0.2.4.tar", last modified: Sat Apr 13 15:13:23 2024, max compression
```

## Comparing `CircuitCalculator-0.2.3.tar` & `circuitcalculator-0.2.4.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.092474 CircuitCalculator-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.092474 CircuitCalculator-0.2.3/src/CircuitCalculator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.096474 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/impedance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.096474 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/NodalAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/equivalent_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/labelmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/supernodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Network/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/PlottingTemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.096474 CircuitCalculator-0.2.3/src/CircuitCalculator/SignalProcessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SignalProcessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SignalProcessing/periodic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SignalProcessing/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.096474 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/plot_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/Display.py
--rw-r--r--   0 runner    (1001) docker     (127)    26080 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/Elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/DIN/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/styling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/src/CircuitCalculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-04 17:24:03.000000 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-04 17:24:03.000000 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 17:24:03.000000 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-04 17:24:03.000000 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 17:24:03.000000 CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 17:24:03.100474 CircuitCalculator-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2024-03-04 17:23:57.000000 CircuitCalculator-0.2.3/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.768934 circuitcalculator-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.768934 circuitcalculator-0.2.4/src/CircuitCalculator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.772934 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/impedance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.772934 circuitcalculator-0.2.4/src/CircuitCalculator/Network/
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/NodalAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/equivalent_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/labelmapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/supernodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Network/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/PlottingTemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SignalProcessing/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/plot_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27291 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/LampLighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.776934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/styling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/src/CircuitCalculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 15:13:23.000000 circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:13:23.780934 circuitcalculator-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-04-13 15:13:15.000000 circuitcalculator-0.2.4/tests/test_integration.py
```

### Comparing `CircuitCalculator-0.2.3/LICENSE` & `circuitcalculator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/PKG-INFO` & `circuitcalculator-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: matplotlib==3.5.2
-Requires-Dist: schemdraw==0.17
+Requires-Dist: schemdraw==0.18
 
 # CircuitCalculator
 
 This project is a simple calculator for electrical circuits. It allows users to input the values of various components in a circuit (such as resistors, capacitors, and voltage sources) and will then calculate various properties of the circuit, such as the current and voltage at different points.
 
 ## Usage
```

### Comparing `CircuitCalculator-0.2.3/README.md` & `circuitcalculator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/circuit.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/circuit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .components import Component, is_active
 from .transformers import transformers
 from ..Network.network import Network
 import numpy as np
 from dataclasses import dataclass, field
 
 class MultipleGroundNodes(Exception): pass
+class AmbiguousComponentID(Exception): pass
 
 @dataclass
 class Circuit:
     components : list[Component]
     ground_node : str = field(init=False, default='')
 
     def __post_init__(self) -> None:
@@ -18,14 +19,20 @@
         ground_nodes = [component.nodes[0] for component in self.components if component.type == 'ground']
         if len(ground_nodes) > 1:
             raise MultipleGroundNodes(f'Component list contains multiple ground nodes: {str(ground_nodes)}')
         if len(ground_nodes) == 0:
             self.ground_node = self.components[0].nodes[0]
         else:
             self.ground_node = ground_nodes[0]
+        if len(set([component.id for component in self.components])) != len(self.components):
+            raise AmbiguousComponentID(f'Component list contains multiple components with the same ID.')
+
+    def __getitem__(self, key: str) -> Component:
+        index = [component.id for component in self.components].index(key)
+        return self.components[index]
 
 def w(f: float) -> float:
     return 2*np.pi*f
 
 def transform_circuit(circuit: Circuit, w: float, w_resolution: float = 1e-3) -> Network:
     return Network(
         branches=[transformers[component.type](component, w, w_resolution) for component in circuit.components if component.type in transformers.keys()],
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/components.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/components.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from dataclasses import dataclass, field
 
 @dataclass(frozen=True)
 class Component:
     type : str
     id : str = field(default='0')
     nodes : tuple[str, ...] = field(default=('0',))
@@ -76,15 +75,15 @@
     return Component(
         type='complex_voltage_source',
         id=id,
         value={'V_real': V.real, 'V_imag': V.imag, 'R': Z.real, 'X': Z.imag},
         nodes=nodes
         )
 
-def periodic_voltage_source(id: str, nodes: tuple[str, str], wavetype: str, V: float, w: float, phi: float, R: float = 0) ->Component:
+def periodic_voltage_source(id: str, nodes: tuple[str, str], wavetype: str, V: float, w: float, phi: float = 0, R: float = 0) ->Component:
     return Component(
         type='periodic_voltage_source',
         id=id,
         value={'wavetype': wavetype,
                'V': V,
                'w': w,
                'phi': phi,
@@ -112,26 +111,49 @@
     return Component(
         type='complex_current_source',
         id=id,
         value={'I_real': I.real, 'I_imag': I.imag, 'G': Y.real, 'B': Y.imag},
         nodes=nodes
         )
 
-def periodic_current_source(id: str, nodes: tuple[str, str], wavetype: str, I: float, w: float, phi: float, G: float = 0) ->Component:
+def periodic_current_source(id: str, nodes: tuple[str, str], wavetype: str, I: float, w: float, phi: float, G: float = 0) -> Component:
     return Component(
         type='periodic_current_source',
         id=id,
         value={'wavetype': wavetype,
                'I': I,
                'w': w,
                'phi': phi,
                'G': G},
         nodes=nodes
         )
 
+def lamp(id: str, nodes: tuple[str, str], P: float, V_ref: float) -> Component:
+    return Component(
+        type='lamp',
+        id=id,
+        value={'P': P, 'V_ref': V_ref},
+        nodes=nodes
+        )
+
+def resistive_load(id: str, nodes: tuple[str, str], P: float, V_ref: float) -> Component:
+    return Component(
+        type='resistive_load',
+        id=id,
+        value={'P': P, 'V_ref': V_ref},
+        nodes=nodes
+        )
+
+def short_circuit(id: str, nodes: tuple[str, str]) -> Component:
+    return Component(
+        type='short_circuit',
+        id=id,
+        nodes=nodes
+    )        
+
 def ground(id: str='gnd', nodes: tuple[str]=('0',)) -> Component:
     return Component(
         type='ground',
         id=id,
         nodes=nodes
     )
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/impedance.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/impedance.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/serializers.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/serializers.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/solution.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/solution.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Circuit/transformers.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Circuit/transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -157,21 +157,38 @@
         nodes=(source.nodes[0], source.nodes[1]),
         w=w,
         phi=frequency_properties.phase(n),
         I=frequency_properties.amplitude(n)
     )
     return ac_current_source(single_frequency_source, w, w_resolution)
 
+def short_circuit(short_circuit: ccp.Component, *_) -> ntw.Branch:
+    return ntw.Branch(
+        short_circuit.nodes[0],
+        short_circuit.nodes[1],
+        elm.short_circuit(short_circuit.id)
+    )
+
+def resistive_load(load: ccp.Component, *_) -> ntw.Branch:
+    return ntw.Branch(
+        load.nodes[0],
+        load.nodes[1],
+        elm.load(load.id, float(load.value['P']), float(load.value['V_ref']))
+    )
+
 transformers : dict[str, CircuitComponentTranslator] = {
     'resistor' : resistor,
     'impedance' : impedance,
     'capacitor' : capacitor,
     'inductance' : inductance,
     'dc_voltage_source' : dc_voltage_source,
     'ac_voltage_source' : ac_voltage_source,
     'complex_voltage_source' : complex_voltage_source,
     'dc_current_source' : dc_current_source,
     'ac_current_source' : ac_current_source,
     'complex_current_source' : complex_current_source,
     'periodic_voltage_source' : periodic_voltage_source,
-    'periodic_current_source' : periodic_current_source
+    'periodic_current_source' : periodic_current_source,
+    'short_circuit' : short_circuit,
+    'resistive_load' : resistive_load,
+    'lamp' : resistive_load
 }
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/NodalAnalysis.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/NodalAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .network import Network
+from .network import Network, Branch
 from .elements import is_ideal_current_source, is_ideal_voltage_source, is_current_source, is_voltage_source
 from .supernodes import SuperNodes
 from . import labelmapper as map
 from . import transformers as trf
 from .solution import NetworkSolution
 import itertools
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/elements.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/elements.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 class NortenTheveninElement(Protocol):
     @property
     def name(self) -> str:
         """Name of element"""
         ...
     @property
+    def type(self) -> str:
+        """Specific element type"""
+        ...
+    @property
     def Z(self) -> complex:
         """Impedance value of element"""
         ...
     @property
     def Y(self) -> complex:
         """Admittance value of element"""
         ...
@@ -66,22 +70,35 @@
         except ZeroDivisionError:
             return np.nan
 
 def impedance(name : str, Z : complex) -> NortenTheveninElement:
     return NortenElement(Z=Z, V=0, name=name, type='impedance')
 
 def admittance(name : str, Y : complex) -> NortenTheveninElement:
-    return TheveninElement( Y=Y, I=0, name=name, type='admittance')
+    return TheveninElement(Y=Y, I=0, name=name, type='admittance')
 
 def resistor(name : str, R : float) -> NortenTheveninElement:
     return NortenElement(Z=R, V=0, name=name, type='resistor')
 
 def conductor(name : str, G : float) -> NortenTheveninElement:
     return TheveninElement(Y=G, I=0, name=name, type='conductor')
 
+def load(name : str, P : float, V_ref: float = -1, I_ref: float = -1, Q : float = 0) -> NortenTheveninElement:
+    if V_ref < 0 and I_ref < 0:
+        raise AttributeError('A reference voltage or reference current has to be defined for a load.')
+    if V_ref > 0 and I_ref > 0:
+        raise AttributeError('You can only define a reference voltage or a reference current for a load.')
+    if V_ref == 0 and I_ref < 0:
+        raise ValueError('Reference voltage must be greater than zero.')
+    if I_ref <= 0 and V_ref < 0:
+        raise ValueError('Reference current must be greater than zero.')
+    if V_ref > 0:
+        return TheveninElement(Y=complex(P, Q)/V_ref**2, I=0, name=name, type='load')
+    return NortenElement(Z=complex(P, Q)/I_ref**2, V=0, name=name, type='load')
+
 def voltage_source(name : str, V : complex, Z : complex = 0) -> NortenTheveninElement:
     return NortenElement(V=V, Z=Z, name=name, type='voltage_source')
 
 def current_source(name : str, I : complex, Y : complex = 0) -> NortenTheveninElement:
     return TheveninElement(I=I, Y=Y, name=name, type='current_source')
 
 def open_circuit(name : str) -> NortenTheveninElement:
@@ -116,15 +133,21 @@
 def is_voltage_source(element: NortenTheveninElement) -> bool:
     return np.abs(element.V) > 0
 
 def is_current_source(element: NortenTheveninElement) -> bool:
     return np.abs(element.I) > 0
 
 def is_ideal_voltage_source(element: NortenTheveninElement) -> bool:
-    return is_voltage_source(element) and element.Z==0
+    return np.abs(element.V) >= 0 and element.Z==0
 
 def is_ideal_current_source(element: NortenTheveninElement) -> bool:
-    return is_current_source(element)and element.Y==0
+    return np.abs(element.I) >= 0 and element.Y==0
 
 def is_active(element: NortenTheveninElement) -> bool:
     return is_voltage_source(element) or is_current_source(element)
 
+def is_short_circuit(element: NortenTheveninElement) -> bool:
+    return element.V == 0 and element.Z == 0
+
+def is_open_circuit(element: NortenTheveninElement) -> bool:
+    return element.I == 0 and element.Y == 0
+
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/equivalent_sources.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/equivalent_sources.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/loaders.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     "admittance" : lambda **kwargs: elm.admittance(Y=to_complex(kwargs['Y']), **kwargs),
     "linear_current_source" : lambda **kwargs: elm.current_source(**translate_to_complex(keys=['I', 'Y'], **kwargs)),
     "current_source" : lambda **kwargs: elm.current_source(I=to_complex(kwargs.pop('I')), **kwargs),
     "real_current_source" : elm.current_source,
     "linear_voltage_source" : lambda **kwargs: elm.voltage_source(V=to_complex(kwargs.pop('V')), Z=to_complex(kwargs.pop('Z')), **kwargs),
     "voltage_source" : lambda **kwargs: elm.voltage_source(V=to_complex(kwargs.pop('V')), **kwargs),
     "real_voltage_source" : elm.voltage_source,
+    "short_circuit" : elm.short_circuit,
+    "open_circuit" : elm.open_circuit,
 }
 
 def load_network(network_dict: list[dict[str, Any]]) -> Network:
     def entry_to_branch(entry: dict[str, Any]) -> Branch:
         n1 = entry.pop('N1')
         n2 = entry.pop('N2')
         entry['name'] = entry.pop('id')
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/network.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/network.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Network/supernodes.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Network/supernodes.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/PlottingTemplates.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/PlottingTemplates.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/FrequencyDomain.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/NyquistDiagram.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/layout.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/layout.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleAnalysis/plot_elements.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleAnalysis/plot_elements.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def capacitor_translator(element: elm.Capacitor, nodes: tuple[str, ...]) -> ccp.Component:
     return ccp.capacitor(nodes=(nodes[0], nodes[1]), id=element.name, C=element.C)
 
 def inductance_translator(element: elm.Inductance, nodes: tuple[str, ...]) -> ccp.Component:
     return ccp.inductance(nodes=(nodes[0], nodes[1]), id=element.name, L=element.L)
 
+def lamp_translator(element: elm.Lamp, nodes: tuple[str, ...]) -> ccp.Component:
+    return ccp.lamp(nodes=(nodes[0], nodes[1]), id=element.name, P=element.P_ref, V_ref=element.V_ref)
+
 def ground_translator(element: elm.Ground, nodes: tuple[str, ...]) -> ccp.Component:
     return ccp.ground(nodes=(nodes[0],), id=element.name)
 
 def dc_voltage_source_translator(element: elm.VoltageSource, nodes: tuple[str, ...]) -> ccp.Component:
     return ccp.dc_voltage_source(
         nodes=(nodes[0], nodes[1]) if not element.is_reverse else (nodes[1], nodes[0]),
         id=element.name,
@@ -103,14 +106,20 @@
     return ccp.dc_voltage_source(
         nodes=(nodes[0], nodes[1]) if not element.is_reverse else (nodes[1], nodes[0]),
         id=element.name,
         V=element.V.real if not element.is_reverse else -element.V.real,
         R=element.R
     )
 
+def short_circuit_translator(element: elm.LabeledLine, nodes: tuple[str, ...]) -> ccp.Component:
+    return ccp.short_circuit(
+        nodes=(nodes[0], nodes[1]) if not element.is_reverse else (nodes[1], nodes[0]),
+        id=element.name,
+    )
+
 def switch_translator(element: elm.Switch, nodes: tuple[str, ...]) -> ccp.Component | None:
     if element.state == element.state.OPEN:
         return ccp.resistor(nodes=(nodes[0], nodes[1]), id=element.name, R=inf)
     return ccp.resistor(nodes=(nodes[0], nodes[1]), id=element.name, R=1e-12)
 
 def none_translator(*_) -> None:
     return None
@@ -125,16 +134,18 @@
     elm.ComplexCurrentSource : complex_current_source_translator,
     elm.ACVoltageSource : ac_voltage_source_translator,
     elm.ACCurrentSource : ac_current_source_translator,
     elm.RectVoltageSource : rect_voltage_source_translator,
     elm.RectCurrentSource : rect_current_source_translator,
     elm.Capacitor : capacitor_translator,
     elm.Inductance : inductance_translator,
+    elm.Lamp : lamp_translator,
     elm.Ground : ground_translator,
     elm.Line: none_translator,
+    elm.LabeledLine: short_circuit_translator,
     elm.Node: none_translator,
     elm.LabelNode: none_translator,
     elm.RealCurrentSource: linear_current_source_translator,
     elm.RealVoltageSource: linear_voltage_source_translator,
     elm.Switch: switch_translator,
     elm.VoltageLabel: none_translator,
     elm.CurrentLabel: none_translator,
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramParser.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 node_mapping.update({n: current_unique_node.pop()})
             else:
                 node_mapping.update({n: n})
         return node_mapping
 
     @property
     def ground(self) -> schemdraw.util.Point:
-        ground_nodes = [n for n in self.node_elements if type(n) == elm.Ground]
+        ground_nodes = [n for n in self.node_elements if isinstance(n, elm.Ground)]
         if len(ground_nodes) > 1:
             raise MultipleGroundNodes
         if len(ground_nodes) == 0:
             return list(self.unique_nodes)[0]
         else:
             return elm.get_nodes(ground_nodes[0])[0]
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramSolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,29 +23,29 @@
     power_display: Callable[[complex], str]
 
     def draw_voltage(self, name: str, reverse: bool = False) -> elm.VoltageLabel:
         element = self.diagram_parser.get_element(name)
         V_branch = self.solution.get_voltage(name)
         if reverse:
             V_branch *= -1
-        return elm.VoltageLabel(element, label=self.voltage_display(V_branch), reverse=reverse if not element.is_reverse else not reverse, color=dsp.blue)
+        return elm.VoltageLabel(element, vlabel=self.voltage_display(V_branch), reverse=reverse if not element.is_reverse else not reverse, color=dsp.blue)
 
     def draw_current(self, name: str, reverse: bool = False, end: bool = False) -> elm.CurrentLabel:
         element = self.diagram_parser.get_element(name)
         I_branch = self.solution.get_current(name)
         if reverse:
             I_branch *= -1
         if end:
             reverse = not reverse
-        return elm.CurrentLabel(element, label=self.current_display(I_branch), reverse=reverse if not element.is_reverse else not reverse, start=not end, color=dsp.red)
+        return elm.CurrentLabel(element, ilabel=self.current_display(I_branch), reverse=reverse if not element.is_reverse else not reverse, start=not end, color=dsp.red)
 
     def draw_power(self, name: str, reverse: bool = False) -> elm.PowerLabel:
         element = self.diagram_parser.get_element(name)
         P_branch = self.solution.get_power(name)
-        return elm.PowerLabel(element, label=self.power_display(P_branch), color=dsp.green)
+        return elm.PowerLabel(element, plabel=self.power_display(P_branch), color=dsp.green)
 
     def draw_potential(self, node: str, loc:str = '') -> elm.LabelNode:
         element = self.diagram_parser.get_element(node)
         node_potential = self.solution.get_potential(node_id=node)
         return elm.LabelNode(id_loc=loc, name=self.voltage_display(node_potential), at=element.absdrop[0], color=dsp.blue)
 
 def time_domain_steady_state_solution(schematic: elm.Schematic, solver: NetworkSolver = nodal_analysis_solver, w: float = 0, sin: bool = False, deg: bool = False, hertz: bool = False) -> SchematicDiagramSolution:
@@ -85,9 +85,9 @@
     diagram_parser = SchematicDiagramParser(schematic)
     solution = ComplexSolution(circuit=circuit_translator(schematic), solver=solver)
     return SchematicDiagramSolution(
         diagram_parser=diagram_parser,
         solution=solution,
         voltage_display=partial(dsp.print_real, unit='V', precision=precision),
         current_display=partial(dsp.print_real, unit='A', precision=precision),
-        power_display=partial(dsp.print_active_power, unit='W', precision=precision)
+        power_display=lambda x: dsp.print_active_power(x.real, precision=precision)
     )
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 import schemdraw.elements
-from ..Network.network import Network, Branch
+from ..Network.network import Network
 from ..Circuit.circuit import Circuit, Component
 
 from . import Elements as elm
 from .CircuitComponentTranslators import circuit_translator_map
 from .NetworkBranchTranslators import network_translator_map
 from .SchemdrawTranslatorTypes import ElementTranslatorMap
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/Display.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Display.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     label+= '·t'
     if abs(phase_value) > 1e-4:
         label+= '+' if phase_value > 0 else '-'
         label+= str(abs_phase_value)
     label+= ')'
     return label
 
-def print_active_power(value: float, unit='W', precision: int = 3) -> str:
+def print_active_power(value: float, precision: int = 3) -> str:
     P = ScientificFloat(value=abs(value), unit='W', precision=precision, use_exp_prefix=True)
     P_sign = '↓' if value > 0 else '↑'
     label = f'{P}{P_sign}'
     return label
 
 def print_active_reactive_power(value: complex, precision: int = 3) -> str:
     P = ScientificFloat(value=abs(value.real), unit='W', precision=precision, use_exp_prefix=True)
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/Elements.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/Elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,14 +543,52 @@
     def name(self) -> str:
         return ''
 
     @property
     def type(self) -> str:
         return 'line'
 
+@extension.lamp
+@simple_circuit_element
+class Lamp(schemdraw.elements.Lamp2):
+    def __init__(self, V_ref: float, P_ref: float, name: str, *args, show_name: bool = True, show_value: bool = True, reverse: bool = False, precision: int = 3, **kwargs):
+        super().__init__(*args, reverse=reverse, **kwargs)
+        self._V_ref = V_ref
+        self._P_ref = P_ref
+        label = ''
+        label += f'{name}' if show_name else ''
+        label += '=' if  show_name and show_value else ''
+        label += dsp.print_real(P_ref, unit='W', precision=precision) if show_value else ''
+        self.label(label, rotate=show_value, loc='value_label', halign='center', valign='center')
+
+    @property
+    def V_ref(self) -> float:
+        return self._V_ref
+
+    @property
+    def P_ref(self) -> float:
+        return self._P_ref
+
+    @property
+    def R(self) -> float:
+        return self._V_ref**2/self._P_ref
+
+class LabeledLine(Line):
+    def __init__(self, *args, name: str, **kwargs):
+        super().__init__(*args, name=name, **kwargs)
+        self._name = name
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def type(self) -> str:
+        return 'labeled_line'
+
 @simple_circuit_element
 class Node(schemdraw.elements.Element):
     def __init__(self, *args, name: str = '', **kwargs):
         super().__init__(*args, name=name, **kwargs)
         self.node_id = name
         self.params['theta'] = 0
         self.params['drop'] = (0, 0)
@@ -666,61 +704,61 @@
     def left(self) -> schemdraw.elements.Element:
         return super().down()
 
     def right(self) -> schemdraw.elements.Element:
         return super().up()
 
 class VoltageLabel(schemdraw.elements.CurrentLabel):
-    def __init__(self, at: schemdraw.elements.Element, label: str = '', label_loc: str = 'bottom', reverse: bool = False, **kwargs):
+    def __init__(self, at: schemdraw.elements.Element, vlabel: str = '', label_loc: str = 'bottom', reverse: bool = False, **kwargs):
         kwargs.update({'color': kwargs.get('color', dsp.blue)})
         kwargs.update({'headlength': kwargs.get('headlength', 0.4)})
         kwargs.update({'headwidth': kwargs.get('headwidth', 0.3)})
         if isinstance(at, RealVoltageSource):
             kwargs.update({'length': kwargs.get('length', 4)})
         super().__init__(reverse=reverse, **kwargs)
         try:
             self.at(at.v_label)
             self.theta(at.transform.theta)
         except AttributeError:
             self.at(at)
         rotate = kwargs.get('rotate', True)
         if rotate == True and at.transform.theta == 270:
             rotate = 90
-        self.label(label, rotate=rotate, loc=label_loc, ofst=(0, -0.1))
+        self.label(vlabel, rotate=rotate, loc=label_loc, ofst=(0, -0.1))
 
 class CurrentLabel(schemdraw.elements.CurrentLabelInline):
-    def __init__(self, at: schemdraw.elements.Element, label: str = '', **kwargs):
+    def __init__(self, at: schemdraw.elements.Element, ilabel: str = '', **kwargs):
         kwargs.update(i_label_args.get(type(at), {}))
         kwargs.update({'color': kwargs.get('color', dsp.red)})
         kwargs.update({'headlength': kwargs.get('headlength', 0.4)})
         kwargs.update({'headwidth': kwargs.get('headwidth', 0.3)})
         totlen = at._userparams.get('l', at._userparams.get('unit', 3))
         kwargs.update({'ofst': totlen/4-0.15+kwargs.get('ofst', 0)})
         start = kwargs.get('start', True)
         reverse = kwargs.get('reverse', False)
         if isinstance(at, RealVoltageSource) or isinstance(at, RealCurrentSource): # when replacing CurrentLabelInline this dependency may be removed
             reverse = not reverse
         kwargs.update({'start' : start, 'reverse' : reverse})
         super().__init__(**kwargs)
         self.at(at)
-        self.label(label)
+        self.label(ilabel)
 
 class PowerLabel(schemdraw.elements.Label):
-    def __init__(self, at: schemdraw.elements.Element, label: str = '', **kwargs):
+    def __init__(self, at: schemdraw.elements.Element, plabel: str = '', **kwargs):
         kwargs.update({'color': kwargs.get('color', dsp.green)})
         super().__init__(**kwargs)
         try:
             self.at(at.s_label)
             self.theta(at.transform.theta)
         except AttributeError:
             self.at(at.center)
         rotate = kwargs.get('rotate', True)
         if rotate == True and at.transform.theta == 270:
             rotate = 90
-        self.label(label, rotate=rotate, halign='center')
+        self.label(plabel, rotate=rotate, halign='center')
 
 i_label_args : dict[Any, dict[str, float]] = {
     Resistor : {'ofst' : 1.4},
     Conductance : {'ofst' : 1.4},
     Impedance : {'ofst' : 1.4},
     Admittance : {'ofst' : 1.4},
     Capacitor : {'ofst' : 1.4},
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
         def left(self) -> schemdraw.elements.Element:
             self.anchors['value_label'] = (0.5, -0.9)
             self.anchors['v_label'] = (0.5, 0.3)
             self.anchors['s_label'] = (0.5, -1.2)
             return super().left()
 
-        def _place_label(self, *args, **kwargs):
+        def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
             if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
                 if delta[1] < 0:
-                    kwargs.update({'rotation': 90})
-            super()._place_label(*args, **kwargs)
+                    theta = 90
+            super()._place_label(label=label, theta=theta)
     
     return extended_resistor
 
 def source(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
     class extended_source(element):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
@@ -67,20 +67,20 @@
 
         def left(self) -> schemdraw.elements.Element:
             self.anchors['value_label'] = (0.0, -0.6)
             self.anchors['s_label'] = (0.0, -1.1)
             self.anchors['v_label'] = (0.0, 0.3)
             return super().left()
 
-        def _place_label(self, *args, **kwargs):
+        def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
             if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
                 if delta[1] < 0:
-                    kwargs.update({'rotation': 90})
-            super()._place_label(*args, **kwargs)
+                    theta = 90
+            super()._place_label(label=label, theta=theta)
 
     return extended_inductor
 
 def inductor(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
     class extended_inductor(element):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
@@ -96,21 +96,36 @@
 
         def left(self) -> schemdraw.elements.Element:
             self.anchors['value_label'] = (0.5, -0.6)
             self.anchors['v_label'] = (0.5, 0.2)
             self.anchors['s_label'] = (0.5, -1.2)
             return super().left()
 
-        def _place_label(self, *args, **kwargs):
+        def _place_label(self, label: schemdraw.elements.elements.Label, theta: float = 0):
             delta = self.end-self.start
             if abs(delta[1]) > abs(delta[0]): # portrait placing of resistor
                 if delta[1] < 0:
-                    kwargs.update({'rotation': 90})
-            super()._place_label(*args, **kwargs)
+                    theta = 90
+            super()._place_label(label=label, theta=theta)
 
     return extended_inductor
 
+def lamp(element: Type[schemdraw.elements.Element]) -> Type[schemdraw.elements.Element]:
+    class extended_lamp(element):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.anchors['value_label'] = (0.5, 0.8)
+            self.anchors['v_label'] = (0.5, -1.1)
+            self.anchors['i_label'] = (1.2, 0.3)
+            self.anchors['s_label'] = (0.5, 1.5)
+
+        def down(self) -> schemdraw.elements.Element:
+            self.anchors['s_label'] = (0.5, -0.7)
+            return super().down()
+
+    return extended_lamp
+
 def voltage_arrow(start: tuple[float, float] = (1.5, 0.7), end: tuple[float, float] = (-0.5, 0.7), arrowwidth: float = 0.3, arrowlength: float = 0.4, color=dsp.blue) -> schemdraw.Segment:
     return schemdraw.Segment((start, end), arrow='->', arrowwidth=arrowwidth, arrowlength=arrowlength, color=color)
 
 def current_arrow(start: tuple[float, float] = (1.2, 0.3), end: tuple[float, float] = (1.8, 0.3), arrowwidth: float = 0.3, arrowlength: float = 0.4, color=dsp.red) -> schemdraw.Segment:
     return schemdraw.Segment((start, end), arrow='->', arrowwidth=arrowwidth, arrowlength=arrowlength, color=color)
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/serializer.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .DiagramTranslator import circuit_translator
 from . import Elements as simple_circuit_elements
 import schemdraw.elements
 import schemdraw.util
 import schemdraw.transform
 import json
 from typing import Any, TypedDict, Callable, TypeVar
+from collections import ChainMap
 
 class SchemdrawObjectProperties(TypedDict):
     type: str
     values: dict[str, Any] | list
 
 class SimpleCircuitObjectProperties(SchemdrawObjectProperties):
     name: str
@@ -84,14 +85,15 @@
     str: lambda x: x,
     int: lambda x: x,
     float: lambda x: x,
     bool: lambda x: x,
     dict: lambda x: {k: serialize_schemdraw_element(v) for k, v in x.items()},
     list: lambda x: [serialize_schemdraw_element(e) for e in x],
     tuple: lambda x: [serialize_schemdraw_element(e) for e in x],
+    ChainMap: lambda x: dict(x),
     schemdraw.util.Point: lambda x: schemdraw_object_properties(x, listify_point),
     schemdraw.segments.Segment: lambda x: schemdraw_object_properties(x, dictify_segment),
     schemdraw.segments.SegmentText: lambda x: schemdraw_object_properties(x, dictify_segment_text),
     schemdraw.segments.SegmentCircle: lambda x: schemdraw_object_properties(x, dictify_segment_circle),
     schemdraw.transform.Transform: lambda x: schemdraw_object_properties(x, dictify_transform)
 }
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/SimpleCircuit/styles/DIN/elements.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator/Utils.py` & `circuitcalculator-0.2.4/src/CircuitCalculator/Utils.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/PKG-INFO` & `circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: matplotlib==3.5.2
-Requires-Dist: schemdraw==0.17
+Requires-Dist: schemdraw==0.18
 
 # CircuitCalculator
 
 This project is a simple calculator for electrical circuits. It allows users to input the values of various components in a circuit (such as resistors, capacitors, and voltage sources) and will then calculate various properties of the circuit, such as the current and voltage at different points.
 
 ## Usage
```

### Comparing `CircuitCalculator-0.2.3/src/CircuitCalculator.egg-info/SOURCES.txt` & `circuitcalculator-0.2.4/src/CircuitCalculator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/CircuitCalculator/SimpleAnalysis/plot_elements.py
 src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
 src/CircuitCalculator/SimpleCircuit/DiagramParser.py
 src/CircuitCalculator/SimpleCircuit/DiagramSolution.py
 src/CircuitCalculator/SimpleCircuit/DiagramTranslator.py
 src/CircuitCalculator/SimpleCircuit/Display.py
 src/CircuitCalculator/SimpleCircuit/Elements.py
+src/CircuitCalculator/SimpleCircuit/LampLighter.py
 src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
 src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
 src/CircuitCalculator/SimpleCircuit/__init__.py
 src/CircuitCalculator/SimpleCircuit/schemdraw_element_extension.py
 src/CircuitCalculator/SimpleCircuit/serializer.py
 src/CircuitCalculator/SimpleCircuit/styles/__init__.py
 src/CircuitCalculator/SimpleCircuit/styles/styling.py
```

### Comparing `CircuitCalculator-0.2.3/tests/test_integration.py` & `circuitcalculator-0.2.4/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,8 +224,22 @@
     np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.4, decimal=3)
     np.testing.assert_almost_equal(solution.get_voltage('R2'), 0.4, decimal=3)
     np.testing.assert_almost_equal(solution.get_voltage('Vs'), -0.4, decimal=2)
     np.testing.assert_almost_equal(solution.get_current('R1'), 0.04, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('R2'), 0.02, decimal=3)
     np.testing.assert_almost_equal(solution.get_current('Vs'), -0.06, decimal=3)
     np.testing.assert_almost_equal(solution.get_potential('0'), 0.00, decimal=2)
-    np.testing.assert_almost_equal(solution.get_potential('1'), 0.40, decimal=2)
+    np.testing.assert_almost_equal(solution.get_potential('1'), 0.40, decimal=2)
+
+def test_network_15_with_advanced_nodal_analysis() -> None:
+    network = load_network_from_json(str(json_root / 'example_network_15.json'))
+    solution = nodal_analysis_solver(network)
+    np.testing.assert_almost_equal(solution.get_voltage('R1'), 0.36, decimal=3)
+    np.testing.assert_almost_equal(solution.get_voltage('Vs'), 1.0, decimal=2)
+    np.testing.assert_almost_equal(solution.get_voltage('sc'), 0.0, decimal=2)
+    np.testing.assert_almost_equal(solution.get_current('R1'), 0.036, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('Vs'), -0.048, decimal=3)
+    np.testing.assert_almost_equal(solution.get_current('sc'), 0.004, decimal=3)
+    np.testing.assert_almost_equal(solution.get_potential('0'), 0.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_potential('1'), 1.00, decimal=2)
+    np.testing.assert_almost_equal(solution.get_potential('2'), 0.64, decimal=2)
+    np.testing.assert_almost_equal(solution.get_potential('3'), 0.64, decimal=2)
```

