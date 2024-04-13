# Comparing `tmp/hahomematic-2024.4.6.tar.gz` & `tmp/hahomematic-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.6.tar", last modified: Wed Apr 10 17:57:07 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.7.tar", last modified: Sat Apr 13 16:20:10 2024, max compression
```

## Comparing `hahomematic-2024.4.6.tar` & `hahomematic-2024.4.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    57524 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41426 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.859441 hahomematic-2024.4.6/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.859441 hahomematic-2024.4.6/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33468 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    28733 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.971527 hahomematic-2024.4.7/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.971527 hahomematic-2024.4.7/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    57490 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41418 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28706 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_text.py
```

### Comparing `hahomematic-2024.4.6/LICENSE` & `hahomematic-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/PKG-INFO` & `hahomematic-2024.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.6
+Version: 2024.4.7
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.6/README.md` & `hahomematic-2024.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/__init__.py` & `hahomematic-2024.4.7/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.7/hahomematic/caches/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     NO_CACHE_ENTRY,
     CallSource,
     EventType,
     InterfaceEventType,
     InterfaceName,
 )
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import changed_within_seconds, loop_safe
+from hahomematic.support import changed_within_seconds
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class DeviceDetailsCache:
     """Cache for device/channel details."""
 
@@ -250,30 +250,28 @@
     def clear(self) -> None:
         """Clear the cache."""
         self._pending_pongs.clear()
         self._unknown_pongs.clear()
         self._pending_pong_logged = False
         self._unknown_pong_logged = False
 
-    @loop_safe
     def handle_send_ping(self, ping_ts: datetime) -> None:
         """Handle send ping timestamp."""
         self._pending_pongs.add(ping_ts)
         self._check_and_fire_pong_event(
             event_type=InterfaceEventType.PENDING_PONG,
             pong_mismatch_count=self.pending_pong_count,
         )
         _LOGGER.debug(
             "PING PONG CACHE: Increase pending PING count: %s - %i for ts: %s",
             self._interface_id,
             self.pending_pong_count,
             ping_ts,
         )
 
-    @loop_safe
     def handle_received_pong(self, pong_ts: datetime) -> None:
         """Handle received pong timestamp."""
         if pong_ts in self._pending_pongs:
             self._pending_pongs.remove(pong_ts)
             self._check_and_fire_pong_event(
                 event_type=InterfaceEventType.PENDING_PONG,
                 pong_mismatch_count=self.pending_pong_count,
@@ -322,15 +320,14 @@
                 _LOGGER.debug(
                     "PING PONG CACHE: Removing expired unknown PONG: %s - %i or ts: %s",
                     self._interface_id,
                     self.unknown_pong_count,
                     pong_ts,
                 )
 
-    @loop_safe
     def _check_and_fire_pong_event(
         self, event_type: InterfaceEventType, pong_mismatch_count: int
     ) -> None:
         """Fire an event about the pong status."""
 
         def _fire_event(mismatch_count: int) -> None:
             self._central.fire_ha_event_callback(
```

### Comparing `hahomematic-2024.4.6/hahomematic/caches/persistent.py` & `hahomematic-2024.4.7/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/caches/visibility.py` & `hahomematic-2024.4.7/hahomematic/caches/visibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,15 @@
         )
 
     def _add_line_to_cache(self, line: str) -> None:
         """Add line to from un ignore file to cache."""
 
         # ignore empty line
         if not line.strip():
-            return None
+            return
 
         if line.lower().startswith(_IGNORE_DEVICE_TYPE):
             self._ignore_custom_device_type.append(line.lower().replace(_IGNORE_DEVICE_TYPE, ""))
             return
 
         if line_details := self._get_unignore_line_details(line=line):
             if isinstance(line_details, str):
```

### Comparing `hahomematic-2024.4.6/hahomematic/central/__init__.py` & `hahomematic-2024.4.7/hahomematic/central/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 from hahomematic.platforms.hub import Hub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
 from hahomematic.support import (
     cancelling,
     check_config,
     get_device_address,
-    loop_safe,
+    loop_check,
     reduce_args,
 )
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _R = TypeVar("_R")
 _T = TypeVar("_T")
@@ -316,15 +316,15 @@
         self._stop_connection_checker()
         await self._stop_clients()
         if self.json_rpc_client.is_activated:
             await self.json_rpc_client.logout()
 
         if self._xml_rpc_server:
             # un-register this instance from XmlRPC-Server
-            self._xml_rpc_server.un_register_central(central=self)
+            self._xml_rpc_server.unregister_central(central=self)
             # un-register and stop XmlRPC-Server, if possible
             if self._xml_rpc_server.no_central_registered:
                 self._xml_rpc_server.stop()
             _LOGGER.debug("STOP: XmlRPC-Server stopped")
         else:
             _LOGGER.debug(
                 "STOP: shared XmlRPC-Server NOT stopped. "
@@ -474,15 +474,15 @@
                 _LOGGER.debug("DE_INIT_CLIENTS: Proxy de-initialized: %s", name)
 
     async def _init_hub(self) -> None:
         """Init the hub."""
         await self._hub.fetch_program_data()
         await self._hub.fetch_sysvar_data()
 
-    @loop_safe
+    @loop_check
     def fire_interface_event(
         self,
         interface_id: str,
         interface_event_type: InterfaceEventType,
         data: dict[str, Any] | None = None,
     ) -> None:
         """Fire an event about the interface status."""
@@ -561,20 +561,20 @@
             system_information = SystemInformation()
             for interface_config in self.config.interface_configs:
                 client = await hmcl.create_client(
                     central=self, interface_config=interface_config, local_ip=local_ip
                 )
                 if not system_information.serial:
                     system_information = client.system_information
-            return system_information
         except NoClients:
             raise
         except Exception as ex:
             _LOGGER.warning(ex)
             raise
+        return system_information
 
     def get_client(self, interface_id: str) -> hmcl.Client:
         """Return a client by interface_id."""
         if not self.has_client(interface_id=interface_id):
             raise HaHomematicException(
                 f"get_client: interface_id {interface_id} does not exist on {self._name}"
             )
@@ -961,15 +961,14 @@
         except CancelledError:
             _LOGGER.debug(
                 "create_task: task cancelled for %s",
                 self._name,
             )
             return
 
-    @loop_safe
     def _async_create_task(self, target: Coroutine[Any, Any, _R], name: str) -> asyncio.Task[_R]:
         """Create a task from within the event_loop. This method must be run in the event_loop."""
         task = self._loop.create_task(target, name=name)
         self._tasks.add(task)
         task.add_done_callback(self._tasks.remove)
         return task
 
@@ -980,26 +979,25 @@
         except CancelledError:  # pragma: no cover
             _LOGGER.debug(
                 "run_coroutine: coroutine interrupted for %s",
                 self._name,
             )
             return None
 
-    @loop_safe
     def async_add_executor_job(self, target: Callable[..., _T], *args: Any) -> asyncio.Future[_T]:
         """Add an executor job from within the event_loop."""
         try:
             task = self._loop.run_in_executor(None, target, *args)
             self._tasks.add(task)
             task.add_done_callback(self._tasks.remove)
-            return task
         except (TimeoutError, CancelledError) as err:  # pragma: no cover
             message = f"async_add_executor_job: task cancelled for {self._name} [{reduce_args(args=err.args)}]"
             _LOGGER.debug(message)
             raise HaHomematicException(message) from err
+        return task
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
         if client := self.primary_client:
             return await client.execute_program(pid=pid)
         return False
 
@@ -1102,15 +1100,15 @@
         self._ha_event_callbacks.add(ha_event_callback)
 
     def unregister_ha_event_callback(self, ha_event_callback: Callable) -> None:
         """RUn register ha_event callback in central."""
         if ha_event_callback in self._ha_event_callbacks:
             self._ha_event_callbacks.remove(ha_event_callback)
 
-    @loop_safe
+    @loop_check
     def fire_ha_event_callback(self, event_type: EventType, event_data: dict[str, str]) -> None:
         """
         Fire ha_event callback in central.
 
         # Events like INTERFACE, KEYPRESS, ...
         """
         for callback_handler in self._ha_event_callbacks:
@@ -1126,15 +1124,15 @@
         self._entity_event_callbacks.add(entity_event_callback)
 
     def unregister_entity_event_callback(self, entity_event_callback: Callable) -> None:
         """Un register entity_event callback in central."""
         if entity_event_callback in self._entity_event_callbacks:
             self._entity_event_callbacks.remove(entity_event_callback)
 
-    @loop_safe
+    @loop_check
     def fire_entity_event_callback(
         self, interface_id: str, channel_address: str, parameter: str, value: Any
     ) -> None:
         """
         Fire entity callback in central.
 
         Not used by HA.
@@ -1154,15 +1152,15 @@
         self._system_event_callbacks.add(system_event_callback)
 
     def unregister_system_event_callback(self, system_event_callback: Callable) -> None:
         """Un register system_event callback in central."""
         if system_event_callback in self._system_event_callbacks:
             self._system_event_callbacks.remove(system_event_callback)
 
-    @loop_safe
+    @loop_check
     def fire_system_event_callback(self, system_event: SystemEvent, **kwargs: Any) -> None:
         """
         Fire system_event callback in central.
 
         e.g. DEVICES_CREATED, HUB_REFRESHED
         """
         for callback_handler in self._system_event_callbacks:
```

### Comparing `hahomematic-2024.4.6/hahomematic/central/decorators.py` & `hahomematic-2024.4.7/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.7/hahomematic/central/xml_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         return self._started.is_set() is True  # type: ignore[attr-defined]
 
     def register_central(self, central: hmcu.CentralUnit) -> None:
         """Register a central in the XmlRPC-Server."""
         if not self._centrals.get(central.name):
             self._centrals[central.name] = central
 
-    def un_register_central(self, central: hmcu.CentralUnit) -> None:
+    def unregister_central(self, central: hmcu.CentralUnit) -> None:
         """Unregister a central from XmlRPC-Server."""
         if self._centrals.get(central.name):
             del self._centrals[central.name]
 
     def get_central(self, interface_id: str) -> hmcu.CentralUnit | None:
         """Return a central by interface_id."""
         for central in self._centrals.values():
```

### Comparing `hahomematic-2024.4.6/hahomematic/client/__init__.py` & `hahomematic-2024.4.7/hahomematic/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,15 @@
     ProxyInitState,
     SystemInformation,
     SystemVariableData,
 )
 from hahomematic.exceptions import BaseHomematicException, NoConnection
 from hahomematic.performance import measure_execution_time
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import (
-    build_headers,
-    build_xml_rpc_uri,
-    get_channel_no,
-    loop_safe,
-    reduce_args,
-)
+from hahomematic.support import build_headers, build_xml_rpc_uri, get_channel_no, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _ADDRESS: Final = "address"
 _CHANNELS: Final = "channels"
 _ID: Final = "id"
 _INTERFACE: Final = "interface"
@@ -170,15 +164,14 @@
 
     async def proxy_re_init(self) -> ProxyInitState:
         """Reinit Proxy."""
         if await self.proxy_de_init() != ProxyInitState.DE_INIT_FAILED:
             return await self.proxy_init()
         return ProxyInitState.DE_INIT_FAILED
 
-    @loop_safe
     def _mark_all_devices_forced_availability(
         self, forced_availability: ForcedDeviceAvailability
     ) -> None:
         """Mark device's availability state for this interface."""
         available = forced_availability != ForcedDeviceAvailability.FORCE_FALSE
         if self._available != available:
             for device in self.central.devices:
@@ -245,15 +238,14 @@
             )
             return False
 
         if (datetime.now() - self.last_updated).total_seconds() < CALLBACK_WARN_INTERVAL:
             return True
         return False
 
-    @loop_safe
     def is_callback_alive(self) -> bool:
         """Return if XmlRPC-Server is alive based on received events for this client."""
         if last_events_time := self.central.last_events.get(self.interface_id):
             seconds_since_last_event = (datetime.now() - last_events_time).total_seconds()
             if seconds_since_last_event > CALLBACK_WARN_INTERVAL:
                 if self._is_callback_alive:
                     self.central.fire_interface_event(
@@ -632,21 +624,22 @@
                     else bool(update_result[0])
                 )
                 _LOGGER.info(
                     "UPDATE_DEVICE_FIRMWARE: Executed firmware update for %s with result '%s'",
                     device_address,
                     "success" if result else "failed",
                 )
-                return result
             except BaseHomematicException as ex:
                 _LOGGER.warning(
                     "UPDATE_DEVICE_FIRMWARE failed: %s [%s]",
                     ex.name,
                     reduce_args(args=ex.args),
                 )
+            else:
+                return result
         return False
 
     async def update_paramset_descriptions(self, device_address: str) -> None:
         """Update paramsets descriptions for provided device_address."""
         if not self.central.device_descriptions.get_device_descriptions(
             interface_id=self.interface_id
         ):
@@ -741,21 +734,22 @@
             calllerId = (
                 f"{self.interface_id}#{dt_now.strftime(DATETIME_FORMAT_MILLIS)}"
                 if handle_ping_pong
                 else self.interface_id
             )
             await self._proxy.ping(calllerId)
             self.last_updated = dt_now
-            return True
         except BaseHomematicException as ex:
             _LOGGER.debug(
                 "CHECK_CONNECTION_AVAILABILITY failed: %s [%s]",
                 ex.name,
                 reduce_args(args=ex.args),
             )
+        else:
+            return True
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU."""
         return await self._json_rpc_client.execute_program(pid=pid)
 
@@ -856,21 +850,22 @@
                 )
 
     async def check_connection_availability(self, handle_ping_pong: bool) -> bool:
         """Check if proxy is still initialized."""
         try:
             await self._proxy.clientServerInitialized(self.interface_id)
             self.last_updated = datetime.now()
-            return True
         except BaseHomematicException as ex:
             _LOGGER.debug(
                 "CHECK_CONNECTION_AVAILABILITY failed: %s [%s]",
                 ex.name,
                 reduce_args(args=ex.args),
             )
+        else:
+            return True
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on Homegear."""
         return True
 
@@ -1051,17 +1046,17 @@
         remote_path: str | None = None,
     ) -> None:
         """Init the interface config."""
         self.interface: Final[InterfaceName] = interface
         self.interface_id: Final[str] = f"{central_name}-{self.interface}"
         self.port: Final = port
         self.remote_path: Final = remote_path
-        self.validate()
+        self._init_validate()
 
-    def validate(self) -> None:
+    def _init_validate(self) -> None:
         """Validate the client_config."""
         if self.interface not in list(InterfaceName):
             _LOGGER.warning(
                 "VALIDATE interface config failed: "
                 "Interface names must be within [%s] for production use",
                 ", ".join(list(InterfaceName)),
             )
```

### Comparing `hahomematic-2024.4.6/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.7/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.7/hahomematic/client/xml_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,18 @@
         )
         self._tls: Final[bool] = kwargs.pop(_TLS, False)
         self._verify_tls: Final[bool] = kwargs.pop(_VERIFY_TLS, True)
         self._supported_methods: tuple[str, ...] = ()
         if self._tls:
             kwargs[_CONTEXT] = get_tls_context(self._verify_tls)
         xmlrpc.client.ServerProxy.__init__(  # type: ignore[misc]
-            self, encoding=_ENCODING_ISO_8859_1, *args, **kwargs
+            self,
+            encoding=_ENCODING_ISO_8859_1,
+            *args,  # noqa: B026
+            **kwargs,
         )
 
     async def do_init(self) -> None:
         """Init the xml rpc proxy."""
         if supported_methods := await self.system.listMethods():
             # ping is missing in VirtualDevices interface but can be used.
             supported_methods.append(XmlRpcMethod.PING)
```

### Comparing `hahomematic-2024.4.6/hahomematic/config.py` & `hahomematic-2024.4.7/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/const.py` & `hahomematic-2024.4.7/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/exceptions.py` & `hahomematic-2024.4.7/hahomematic/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,16 +125,14 @@
                     raise
                 return ex_return  # type: ignore[no-any-return]
             return return_value
 
         @wraps(func)
         def wrapper_log_exception(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap sync methods."""
-            return_value = cast(_R, func(*args, **kwargs))
-
-            return return_value
+            return cast(_R, func(*args, **kwargs))
 
         if asyncio.iscoroutinefunction(func):
             return async_wrapper_log_exception
         return wrapper_log_exception
 
     return decorator_log_exception
```

### Comparing `hahomematic-2024.4.6/hahomematic/hmcli.py` & `hahomematic-2024.4.7/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/performance.py` & `hahomematic-2024.4.7/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.7/hahomematic/platforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,18 @@
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import create_custom_entity_and_append_to_device
 from hahomematic.platforms.event import create_event_and_append_to_device
 from hahomematic.platforms.generic import create_entity_and_append_to_device
-from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
-@loop_safe
 def create_entities_and_append_to_device(device: hmd.HmDevice) -> None:
     """Create the entities associated to this device."""
     for channel_address in device.channels:
         channel_no = hms.get_channel_no(channel_address)
 
         if not device.central.paramset_descriptions.get_paramset_keys(
             interface_id=device.interface_id, channel_address=channel_address
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 import importlib
 import logging
 from typing import Final
 
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom.definition import entity_definition_exists, get_entity_configs
 from hahomematic.platforms.custom.support import CustomConfig
-from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
-@loop_safe
 def create_custom_entity_and_append_to_device(
     device: hmd.HmDevice,
 ) -> None:
     """Decides which default platform should be used, and creates the required entities."""
 
     if device.ignore_for_custom_entity:
         _LOGGER.debug(
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.7/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.7/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/device.py` & `hahomematic-2024.4.7/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.support import PayloadMixin, get_device_name
 from hahomematic.platforms.update import HmUpdate
 from hahomematic.support import (
     CacheEntry,
     Channel,
     check_or_create_directory,
-    loop_safe,
+    loop_check,
     reduce_args,
 )
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class HmDevice(PayloadMixin):
@@ -340,15 +340,15 @@
     def add_sub_device_channel(self, channel_no: int, base_channel_no: int) -> None:
         """Assign channel no to base channel no."""
         if base_channel_no not in self._sub_device_channels:
             self._sub_device_channels[base_channel_no] = base_channel_no
         if channel_no not in self._sub_device_channels:
             self._sub_device_channels[channel_no] = base_channel_no
         elif self._sub_device_channels[channel_no] != base_channel_no:
-            return None
+            return
 
     def get_sub_device_channel(self, channel_no: int) -> int | None:
         """Return the sub device channel."""
         return self._sub_device_channels.get(channel_no)
 
     def add_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
@@ -500,15 +500,14 @@
         """Return the list of readable master entities."""
         return tuple(
             ge
             for ge in self._generic_entities.values()
             if ge.is_readable and ge.paramset_key == paramset_key
         )
 
-    @loop_safe
     def set_forced_availability(self, forced_availability: ForcedDeviceAvailability) -> None:
         """Set the availability of the device."""
         if self._forced_availability != forced_availability:
             self._forced_availability = forced_availability
             for entity in self.generic_entities:
                 entity.fire_entity_updated_callback()
 
@@ -578,15 +577,15 @@
                     save_to_file=False,
                 )
         await self.central.paramset_descriptions.save()
         for entity in self.generic_entities:
             entity.update_parameter_data()
         self.fire_device_updated_callback()
 
-    @loop_safe
+    @loop_check
     def fire_device_updated_callback(self, *args: Any) -> None:
         """Do what is needed when the state of the device has been updated."""
         self._set_last_updated()
         for callback_handler in self._device_updated_callbacks:
             try:
                 callback_handler(*args)
             except Exception as ex:
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/entity.py` & `hahomematic-2024.4.7/hahomematic/platforms/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.support import (
     EntityNameData,
     PayloadMixin,
     convert_value,
     generate_channel_unique_id,
 )
-from hahomematic.support import loop_safe, reduce_args
+from hahomematic.support import loop_check, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 
 _CONFIGURABLE_CHANNEL: Final[tuple[str, ...]] = (
     "KEY_TRANSCEIVER",
@@ -225,24 +225,24 @@
             self._device_removed_callbacks.append(device_removed_callback)
 
     def unregister_device_removed_callback(self, device_removed_callback: Callable) -> None:
         """Unregister the device removed callback."""
         if device_removed_callback in self._device_removed_callbacks:
             self._device_removed_callbacks.remove(device_removed_callback)
 
-    @loop_safe
+    @loop_check
     def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated/refreshed."""
         for callback_handler in self._entity_updated_callbacks:
             try:
                 callback_handler(*args, **kwargs)
             except Exception as ex:
                 _LOGGER.warning("FIRE_entity_updated_EVENT failed: %s", reduce_args(args=ex.args))
 
-    @loop_safe
+    @loop_check
     def fire_device_removed_callback(self, *args: Any) -> None:
         """Do what is needed when the entity has been removed."""
         for callback_handler in self._device_removed_callbacks:
             try:
                 callback_handler(*args)
             except Exception as ex:
                 _LOGGER.warning("FIRE_DEVICE_REMOVED_EVENT failed: %s", reduce_args(args=ex.args))
@@ -644,15 +644,14 @@
         """Replace given unit."""
         if not raw_unit:
             return 1
         if multiplier := _MULTIPLIER_UNIT.get(raw_unit):
             return multiplier
         return 1
 
-    @loop_safe
     @abstractmethod
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity data."""
         if direct_call is False and hms.changed_within_seconds(last_change=self._last_refreshed):
@@ -668,15 +667,14 @@
                 paramset_key=self._paramset_key,
                 parameter=self._parameter,
                 call_source=call_source,
                 direct_call=direct_call,
             )
         )
 
-    @loop_safe
     def write_value(self, value: Any) -> tuple[ParameterT | None, ParameterT | None]:
         """Update value of the entity."""
         old_value = self._value
         if value == NO_CACHE_ENTRY:
             if self.last_refreshed != INIT_DATETIME:
                 self._state_uncertain = True
                 self.fire_entity_updated_callback()
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/event.py` & `hahomematic-2024.4.7/hahomematic/platforms/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseParameterEntity
 from hahomematic.platforms.support import EntityNameData, generate_unique_id, get_event_name
-from hahomematic.support import loop_safe
+from hahomematic.support import loop_check
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEvent(BaseParameterEntity[Any, Any]):
     """Base class for events."""
 
@@ -60,23 +60,22 @@
         return EntityUsage.EVENT if force_enabled else EntityUsage.NO_CREATE
 
     @config_property
     def event_type(self) -> EventType:
         """Return the event_type of the event."""
         return self._event_type
 
-    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
         if self.event_type in ENTITY_EVENTS:
             self.fire_entity_updated_callback(parameter=self.parameter.lower())
         self._set_last_updated()
         self.fire_event(value)
 
-    @loop_safe
+    @loop_check
     def fire_event(self, value: Any) -> None:
         """Do what is needed to fire an event."""
         self._central.fire_ha_event_callback(
             event_type=self.event_type, event_data=self.get_event_data(value=value)
         )
 
     def _get_entity_name(self) -> EntityNameData:
@@ -100,15 +99,14 @@
 
 
 class DeviceErrorEvent(GenericEvent):
     """class for handling device error events."""
 
     _event_type = EventType.DEVICE_ERROR
 
-    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
 
         if (
             isinstance(new_value, bool)
@@ -128,15 +126,14 @@
 
 class ImpulseEvent(GenericEvent):
     """class for handling impulse events."""
 
     _event_type = EventType.IMPULSE
 
 
-@loop_safe
 def create_event_and_append_to_device(
     device: hmd.HmDevice, channel_address: str, parameter: str, parameter_data: Mapping[str, Any]
 ) -> None:
     """Create action event entity."""
     if device.central.parameter_visibility.parameter_is_ignored(
         device_type=device.device_type,
         channel_no=hms.get_channel_no(address=channel_address),
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,24 @@
 from hahomematic.platforms.generic.button import HmButton
 from hahomematic.platforms.generic.number import HmFloat, HmInteger
 from hahomematic.platforms.generic.select import HmSelect
 from hahomematic.platforms.generic.sensor import HmSensor
 from hahomematic.platforms.generic.switch import HmSwitch
 from hahomematic.platforms.generic.text import HmText
 from hahomematic.platforms.support import generate_unique_id, is_binary_sensor
-from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 _BUTTON_ACTIONS: Final[tuple[str, ...]] = ("RESET_MOTION", "RESET_PRESENCE")
 
 # Entities that should be wrapped in a new entity on a new platform.
 _SWITCH_ENTITY_TO_SENSOR: Final[Mapping[str | tuple[str, ...], Parameter]] = {
     ("HmIP-eTRV", "HmIP-HEATING"): Parameter.LEVEL,
 }
 
 
-@loop_safe
 def create_entity_and_append_to_device(
     device: hmd.HmDevice,
     channel_address: str,
     paramset_key: str,
     parameter: str,
     parameter_data: dict[str, Any],
 ) -> None:
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 from typing import Any, Final
 
 from hahomematic.const import CallSource, EntityUsage, EventType, Parameter, ParamsetKey
 from hahomematic.platforms import device as hmd, entity as hme
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.support import EntityNameData, get_entity_name
-from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEntity(hme.BaseParameterEntity[hme.ParameterT, hme.InputParameterT]):
     """Base class for generic entities."""
 
@@ -45,15 +44,14 @@
         """Return the entity usage."""
         if self._is_forced_sensor or self._is_un_ignored:
             return EntityUsage.ENTITY
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._usage
         return EntityUsage.ENTITY if force_enabled else EntityUsage.NO_CREATE
 
-    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this entity has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
         if old_value == new_value:
             return
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.7/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from __future__ import annotations
 
 from typing import Final
 
 from hahomematic import central as hmcu
 from hahomematic.const import PROGRAM_ADDRESS, HmPlatform, HubData, ProgramData
 from hahomematic.platforms.hub.entity import GenericHubEntity
-from hahomematic.support import loop_safe
 
 
 class HmProgramButton(GenericHubEntity):
     """Class for a HomeMatic program button."""
 
     _platform = HmPlatform.HUB_BUTTON
 
@@ -43,15 +42,14 @@
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the program button entity."""
         if data.name.lower().startswith(tuple({"p_", "prg_"})):
             return data.name
         return f"P_{data.name}"
 
-    @loop_safe
     def update_data(self, data: ProgramData) -> None:
         """Set variable value on CCU/Homegear."""
         do_update: bool = False
         if self.is_active != data.is_active:
             self.is_active = data.is_active
             do_update = True
         if self.is_internal != data.is_internal:
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from slugify import slugify
 
 from hahomematic import central as hmcu
 from hahomematic.const import SYSVAR_ADDRESS, HubData, SystemVariableData
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.entity import CallbackEntity
 from hahomematic.platforms.support import generate_unique_id
-from hahomematic.support import loop_safe, parse_sys_var
+from hahomematic.support import parse_sys_var
 
 
 class GenericHubEntity(CallbackEntity):
     """Class for a HomeMatic system variable."""
 
     def __init__(
         self,
@@ -112,15 +112,14 @@
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the sysvar entity."""
         if data.name.lower().startswith(tuple({"v_", "sv_", "sv"})):
             return data.name
         return f"Sv_{data.name}"
 
-    @loop_safe
     def write_value(self, value: Any) -> None:
         """Set variable value on CCU/Homegear."""
         old_value = self._value
         if self.data_type:
             value = parse_sys_var(data_type=self.data_type, raw_value=value)
         elif isinstance(old_value, bool):
             value = bool(value)
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.7/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/support.py` & `hahomematic-2024.4.7/hahomematic/platforms/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,17 +330,17 @@
 
 def _check_channel_name_with_channel_no(name: str) -> bool:
     """Check if name contains channel and this is an int."""
     if name.count(":") == 1:
         channel_part = name.split(":")[1]
         try:
             int(channel_part)
-            return True
         except ValueError:
             return False
+        return True
     return False
 
 
 def convert_value(
     value: Any, target_type: ParameterType, value_list: tuple[str, ...] | None
 ) -> Any:
     """Convert a value to target_type."""
```

### Comparing `hahomematic-2024.4.6/hahomematic/platforms/update.py` & `hahomematic-2024.4.7/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.7/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.7/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.7/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic/support.py` & `hahomematic-2024.4.7/hahomematic/support.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 
 import asyncio
 import base64
 from collections.abc import Callable, Collection
 import contextlib
 from dataclasses import dataclass
 from datetime import datetime
-from functools import lru_cache
+from functools import lru_cache, wraps
 import logging
 import os
 import re
 import socket
 import ssl
-from typing import Any, Final, TypeVar
+import sys
+from typing import Any, Final, ParamSpec, TypeVar
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     SysvarType,
 )
 from hahomematic.exceptions import BaseHomematicException, HaHomematicException
 
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 _LOGGER: Final = logging.getLogger(__name__)
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
 
 
 def reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
     """Return the first arg, if there is only one arg."""
     return args[0] if len(args) == 1 else args
 
 
@@ -294,11 +296,50 @@
 
 
 def cancelling(task: asyncio.Future[Any]) -> bool:
     """Return True if task is cancelling."""
     return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
 
 
-def loop_safe(func: _CallableT) -> _CallableT:
+def loop_check(func: Callable[_P, _R]) -> Callable[_P, _R]:
     """Annotation to mark method as safe to call from within the event loop."""
+
+    _with_loop: set = set()
+
+    @wraps(func)
+    def wrapper_loop_safe(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+        """Wrap loop safe."""
+        return_value = func(*args, **kwargs)
+
+        try:
+            asyncio.get_running_loop()
+            loop_running = True
+        except Exception:
+            loop_running = False
+
+        if not loop_running and func not in _with_loop:
+            _with_loop.add(func)
+            _LOGGER.warning(
+                "Method %s must run in the event_loop. No loop detected.", func.__name__
+            )
+
+        return return_value
+
     setattr(func, "_loop_safe", True)
-    return func
+    return wrapper_loop_safe if debug_enabled() else func
+
+
+def debug_enabled() -> bool:
+    """Check if debug mode is enabled."""
+    try:
+        if sys.gettrace() is not None:
+            return True
+    except AttributeError:
+        pass
+
+    try:
+        if sys.monitoring.get_tool(sys.monitoring.DEBUGGER_ID) is not None:
+            return True
+    except AttributeError:
+        pass
+
+    return False
```

### Comparing `hahomematic-2024.4.6/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.7/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.6
+Version: 2024.4.7
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.6/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.7/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/hahomematic_support/client_local.py` & `hahomematic-2024.4.7/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/pyproject.toml` & `hahomematic-2024.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.6"
+version     = "2024.4.7"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
@@ -414,100 +414,129 @@
     "B014", # Exception handler with duplicate exception
     "B015", # Pointless comparison. Did you mean to assign a value? Otherwise, prepend assert or remove it.
     "B018", # Found useless attribute access. Either assign it to a variable or remove it.
     "B023", # Function definition does not bind loop variable {name}
     "B026", # Star-arg unpacking after a keyword argument is strongly discouraged
     "B032", # Possible unintentional type annotation (using :). Did you mean to assign (using =)?
     "B904", # Use raise from to specify exception cause
-    "B905", # zip() without an explicit strict= parameter
-    "C",  # complexity
+    "C", # complexity
     "COM818", # Trailing comma on bare tuple prohibited
-    "D",  # docstrings
-    "DTZ003",  # Use datetime.now(tz=) instead of datetime.utcnow()
-    "DTZ004",  # Use datetime.fromtimestamp(ts, tz=) instead of datetime.utcfromtimestamp(ts)
-    "E",  # pycodestyle
-    "F",  # pyflakes/autoflake
+    "D", # docstrings
+    "DTZ003", # Use datetime.now(tz=) instead of datetime.utcnow()
+    "DTZ004", # Use datetime.fromtimestamp(ts, tz=) instead of datetime.utcfromtimestamp(ts)
+    "E", # pycodestyle
+    "F", # pyflakes/autoflake
     "FLY", # flynt
     "G", # flake8-logging-format
-    "I",  # isort
+    "I", # isort
     "INP", # flake8-no-pep420
+    "ISC", # flake8-implicit-str-concat
     "ICN001", # import concentions; {name} should be imported as {asname}
     "LOG", # flake8-logging
     "N804", # First argument of a class method should be named cls
     "N805", # First argument of a method should be named self
     "N815", # Variable {name} in class scope should not be mixedCase
-    "PERF", # perflint
+    "PERF", # Perflint
     "PGH", # pygrep-hooks
-    "PLC", # pylint
-    "PLC0414", # Useless import alias. Import alias does not rename original package.
-    "PLE", # pylint
-    "PLR", # pylint
-    "PLW", # pylint
+    "PIE", # flake8-pie
+    "PL", # pylint
     "PT", # flake8-pytest-style
     "PYI", # flake8-pyi
-    "Q000", # Double quotes found but single quotes preferred
+    "RET", # flake8-return
     "RSE", # flake8-raise
+    "RUF005", # Consider iterable unpacking instead of concatenation
     "RUF006", # Store a reference to the return value of asyncio.create_task
+    "RUF013", # PEP 484 prohibits implicit Optional
+    "RUF018", # Avoid assignment expressions in assert statements
+    # "RUF100", # Unused `noqa` directive; temporarily every now and then to clean them up
     "S102", # Use of exec detected
-    "S103",  # bad-file-permissions
-    "S108",  # hardcoded-temp-file
-    "S306",  # suspicious-mktemp-usage
-    "S307",  # suspicious-eval-usage
-    "S313",  # suspicious-xmlc-element-tree-usage
-    "S314",  # suspicious-xml-element-tree-usage
-    "S315",  # suspicious-xml-expat-reader-usage
-    "S316",  # suspicious-xml-expat-builder-usage
-    "S317",  # suspicious-xml-sax-usage
-    "S318",  # suspicious-xml-mini-dom-usage
-    "S319",  # suspicious-xml-pull-dom-usage
-    "S320",  # suspicious-xmle-tree-usage
-    "S601",  # paramiko-call
-    "S602",  # subprocess-popen-with-shell-equals-true
-    "S604",  # call-with-shell-equals-true
-    "S608",  # hardcoded-sql-expression
-    "S609",  # unix-command-wildcard-injection
+    "S103", # bad-file-permissions
+    "S108", # hardcoded-temp-file
+    "S306", # suspicious-mktemp-usage
+    "S307", # suspicious-eval-usage
+    "S313", # suspicious-xmlc-element-tree-usage
+    "S314", # suspicious-xml-element-tree-usage
+    "S315", # suspicious-xml-expat-reader-usage
+    "S316", # suspicious-xml-expat-builder-usage
+    "S317", # suspicious-xml-sax-usage
+    "S318", # suspicious-xml-mini-dom-usage
+    "S319", # suspicious-xml-pull-dom-usage
+    "S320", # suspicious-xmle-tree-usage
+    "S601", # paramiko-call
+    "S602", # subprocess-popen-with-shell-equals-true
+    "S604", # call-with-shell-equals-true
+    "S608", # hardcoded-sql-expression
+    "S609", # unix-command-wildcard-injection
     "SIM", # flake8-simplify
     "SLOT", # flake8-slots
     "T100", # Trace found: {name} used
-    "T20",  # flake8-print
+    "T20", # flake8-print
     "TID251", # Banned imports
-    "TRY004", # Prefer TypeError exception for invalid type
-    "TRY302", # Remove exception handler; error is immediately re-raised
-    "UP",  # pyupgrade
-    "W",  # pycodestyle
+    "TRY", # tryceratops
+    "UP", # pyupgrade
+    "W", # pycodestyle
 ]
 
 lint.ignore = [
-    "B026", # Catching too general exception Exception
-    "D202",  # No blank lines allowed after function docstring
-    "D203",  # 1 blank line required before class docstring
+    "D202", # No blank lines allowed after function docstring
+    "D203", # 1 blank line required before class docstring
     "D212",  # Multi-line docstring summary should start at the second line
     #"D213",  # Multi-line docstring summary should start at the second line
-    "D406",  # Section name should end with a newline
-    "D407",  # Section name underlining
-    "E501",  # line too long
-    "E731",  # do not assign a lambda expression, use a def
-    #"PLC1901", # Lots of false positives
-    # False positives https://github.com/astral-sh/ruff/issues/5386
-    "PLC0208", # Use a sequence type instead of a `set` when iterating over values
+    "D406", # Section name should end with a newline
+    "D407", # Section name underlining
+    "E501", # line too long
+    "E731", # do not assign a lambda expression, use a def
+
+    "PLC1901", # {existing} can be simplified to {replacement} as an empty string is falsey; too many false positives
     "PLR0911", # Too many return statements ({returns} > {max_returns})
     "PLR0912", # Too many branches ({branches} > {max_branches})
     "PLR0913", # Too many arguments to function call ({c_args} > {max_args})
-    "PT004", # Fixture {fixture} does not return anything, add leading underscore
-    "PT011", # pytest.raises({exception}) is too broad, set the `match` parameter or use a more specific exception
-    "PYI024", # Use typing.NamedTuple instead of collections.namedtuple
-    "PYI036",
-    "PYI041",
     "PLR0915", # Too many statements ({statements} > {max_statements})
-    "PLR2004",  # Magic value used in comparison, consider replacing {value} with a constant variable
+    "PLR2004", # Magic value used in comparison, consider replacing {value} with a constant variable
     "PLW2901", # Outer {outer_kind} variable {name} overwritten by inner {inner_kind} target
+    "PT004", # Fixture {fixture} does not return anything, add leading underscore
+    "PT011", # pytest.raises({exception}) is too broad, set the `match` parameter or use a more specific exception
+    "PT012", # `pytest.raises()` block should contain a single simple statement
+    "PT018", # Assertion should be broken down into multiple parts
+    #"SIM102", # Use a single if statement instead of nested if statements
+    #"SIM108", # Use ternary operator {contents} instead of if-else-block
+    "SIM115", # Use context handler for opening files
+    "TRY003", # Avoid specifying long messages outside the exception class
+    "TRY400", # Use `logging.exception` instead of `logging.error`
     "UP006", # keep type annotation style as is
     "UP007", # keep type annotation style as is
     # Ignored due to performance: https://github.com/charliermarsh/ruff/issues/2923
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
+    # Ignored due to incompatible with mypy: https://github.com/python/mypy/issues/15238
+    "UP040", # Checks for use of TypeAlias annotation for declaring type aliases.
+
+    # May conflict with the formatter, https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+    "W191",
+    "E111",
+    "E114",
+    "E117",
+    "D206",
+    "D300",
+    "Q",
+    "COM812",
+    "COM819",
+    "ISC001",
+
+    # Disabled because ruff does not understand type of __all__ generated by a function
+    #"PLE0605",
+
+    # temporarily disabled
+    #"PT019",
+    #"PYI024", # Use typing.NamedTuple instead of collections.namedtuple
+    #"RET503",
+    #"RET502",
+    #"RET501",
+    #"TRY002",
+    "TRY301",
+    "PYI041"
 ]
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
 [tool.ruff.lint.flake8-import-conventions.extend-aliases]
 voluptuous = "vol"
```

### Comparing `hahomematic-2024.4.6/tests/test_action.py` & `hahomematic-2024.4.7/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_binary_sensor.py` & `hahomematic-2024.4.7/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_button.py` & `hahomematic-2024.4.7/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_central.py` & `hahomematic-2024.4.7/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_central_pydevccu.py` & `hahomematic-2024.4.7/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_climate.py` & `hahomematic-2024.4.7/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_cover.py` & `hahomematic-2024.4.7/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_decorator.py` & `hahomematic-2024.4.7/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_device.py` & `hahomematic-2024.4.7/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_entity.py` & `hahomematic-2024.4.7/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_event.py` & `hahomematic-2024.4.7/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_json_rpc.py` & `hahomematic-2024.4.7/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_light.py` & `hahomematic-2024.4.7/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_lock.py` & `hahomematic-2024.4.7/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_number.py` & `hahomematic-2024.4.7/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_select.py` & `hahomematic-2024.4.7/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_sensor.py` & `hahomematic-2024.4.7/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_siren.py` & `hahomematic-2024.4.7/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_support.py` & `hahomematic-2024.4.7/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_switch.py` & `hahomematic-2024.4.7/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.6/tests/test_text.py` & `hahomematic-2024.4.7/tests/test_text.py`

 * *Files identical despite different names*

