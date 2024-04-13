# Comparing `tmp/gearpy-0.7.2.tar.gz` & `tmp/gearpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearpy-0.7.2.tar", last modified: Thu Apr 11 09:13:05 2024, max compression
+gzip compressed data, was "gearpy-1.0.0.tar", last modified: Sat Apr 13 15:25:23 2024, max compression
```

## Comparing `gearpy-0.7.2.tar` & `gearpy-1.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.142059 gearpy-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 09:12:57.000000 gearpy-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-04-11 09:13:05.142059 gearpy-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-11 09:12:57.000000 gearpy-0.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.134059 gearpy-0.7.2/gearpy/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.134059 gearpy-0.7.2/gearpy/mechanical_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31114 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/dc_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/flywheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.138059 gearpy-0.7.2/gearpy/mechanical_objects/gear_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/gear_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/gear_data/lewis_factor_table.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/gear_data/worm_gear_and_wheel_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    44175 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/helical_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/mating_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/mechanical_object_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/spur_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    34268 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/worm_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    37366 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/mechanical_objects/worm_wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.138059 gearpy-0.7.2/gearpy/motor_control/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/motor_control_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/pwm_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.138059 gearpy-0.7.2/gearpy/motor_control/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/constant_pwm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/reach_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/rules_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/start_limit_current.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/start_proportional_to_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/motor_control/rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55457 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/powertrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.138059 gearpy-0.7.2/gearpy/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/absolute_rotary_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/amperometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/sensor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/tachometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/sensors/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.138059 gearpy-0.7.2/gearpy/units/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/units/unit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    89149 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/units/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.142059 gearpy-0.7.2/gearpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20109 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.142059 gearpy-0.7.2/gearpy/utils/stop_condition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/stop_condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/stop_condition/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/stop_condition/operator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-11 09:12:57.000000 gearpy-0.7.2/gearpy/utils/stop_condition/stop_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:13:05.142059 gearpy-0.7.2/gearpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-04-11 09:13:05.000000 gearpy-0.7.2/gearpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-11 09:13:05.000000 gearpy-0.7.2/gearpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:13:05.000000 gearpy-0.7.2/gearpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 09:13:05.000000 gearpy-0.7.2/gearpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 09:13:05.000000 gearpy-0.7.2/gearpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-11 09:12:57.000000 gearpy-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:13:05.142059 gearpy-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 09:12:57.000000 gearpy-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.219824 gearpy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 15:25:11.000000 gearpy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-04-13 15:25:23.215824 gearpy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-13 15:25:11.000000 gearpy-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.207825 gearpy-1.0.0/gearpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.207825 gearpy-1.0.0/gearpy/mechanical_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31114 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/dc_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/flywheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.211825 gearpy-1.0.0/gearpy/mechanical_objects/gear_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/gear_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/gear_data/lewis_factor_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/gear_data/worm_gear_and_wheel_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    44175 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/helical_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/mating_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/mechanical_object_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/spur_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34268 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/worm_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37366 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/mechanical_objects/worm_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.211825 gearpy-1.0.0/gearpy/motor_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/motor_control_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/pwm_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.211825 gearpy-1.0.0/gearpy/motor_control/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/constant_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/reach_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/rules_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/start_limit_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/motor_control/rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55441 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/powertrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.211825 gearpy-1.0.0/gearpy/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/absolute_rotary_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/amperometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/sensor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/tachometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/sensors/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.215824 gearpy-1.0.0/gearpy/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/units/unit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89149 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.215824 gearpy-1.0.0/gearpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20109 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.215824 gearpy-1.0.0/gearpy/utils/stop_condition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/stop_condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/stop_condition/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/stop_condition/operator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-13 15:25:11.000000 gearpy-1.0.0/gearpy/utils/stop_condition/stop_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:25:23.215824 gearpy-1.0.0/gearpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-04-13 15:25:23.000000 gearpy-1.0.0/gearpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-13 15:25:23.000000 gearpy-1.0.0/gearpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:25:23.000000 gearpy-1.0.0/gearpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-13 15:25:23.000000 gearpy-1.0.0/gearpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 15:25:23.000000 gearpy-1.0.0/gearpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-13 15:25:11.000000 gearpy-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:25:23.219824 gearpy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 15:25:11.000000 gearpy-1.0.0/setup.py
```

### Comparing `gearpy-0.7.2/LICENSE` & `gearpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/PKG-INFO` & `gearpy-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearpy
-Version: 0.7.2
+Version: 1.0.0
 Summary: Python library for mechanical transmission analysis
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,31 +679,32 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/gearpy
 Project-URL: Documentation, https://gearpy.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/gearpy/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/gearpy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: matplotlib==3.8.0
-Requires-Dist: numpy==1.26.0
-Requires-Dist: pandas==2.1.1
-Requires-Dist: scipy==1.11.3
+Requires-Dist: matplotlib>=3.5
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=1.2
+Requires-Dist: scipy!=1.11.0,>=1.6
 Provides-Extra: doc
 Requires-Dist: furo==2023.9.10; extra == "doc"
 Requires-Dist: m2r2==0.3.3.post2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.1; extra == "test"
@@ -721,15 +722,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -743,15 +744,19 @@
    :target: https://pypi.org/project/gearpy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `gearpy-0.7.2/README.rst` & `gearpy-1.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -30,15 +30,19 @@
    :target: https://pypi.org/project/gearpy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/dc_motor.py` & `gearpy-1.0.0/gearpy/mechanical_objects/dc_motor.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/flywheel.py` & `gearpy-1.0.0/gearpy/mechanical_objects/flywheel.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/helical_gear.py` & `gearpy-1.0.0/gearpy/mechanical_objects/helical_gear.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/mechanical_object_base.py` & `gearpy-1.0.0/gearpy/mechanical_objects/mechanical_object_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/spur_gear.py` & `gearpy-1.0.0/gearpy/mechanical_objects/spur_gear.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/worm_gear.py` & `gearpy-1.0.0/gearpy/mechanical_objects/worm_gear.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/mechanical_objects/worm_wheel.py` & `gearpy-1.0.0/gearpy/mechanical_objects/worm_wheel.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/motor_control_base.py` & `gearpy-1.0.0/gearpy/motor_control/motor_control_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/pwm_control.py` & `gearpy-1.0.0/gearpy/motor_control/pwm_control.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/constant_pwm.py` & `gearpy-1.0.0/gearpy/motor_control/rules/constant_pwm.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/reach_angular_position.py` & `gearpy-1.0.0/gearpy/motor_control/rules/reach_angular_position.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/rules_base.py` & `gearpy-1.0.0/gearpy/motor_control/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/start_limit_current.py` & `gearpy-1.0.0/gearpy/motor_control/rules/start_limit_current.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/start_proportional_to_angular_position.py` & `gearpy-1.0.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/motor_control/rules/utils.py` & `gearpy-1.0.0/gearpy/motor_control/rules/utils.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/powertrain.py` & `gearpy-1.0.0/gearpy/powertrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,19 +438,17 @@
                 for variable, unit in zip(variable_list, unit_list):
                     interpolation_function = interp1d(x = [instant.to('sec').value for instant in self.time],
                                                       y = [value.to(unit).value
                                                            for value in element.time_variables[variable]])
                     data.loc[element.name, f'{variable} ({unit})'] = \
                         interpolation_function(target_time.to('sec').value).take(0)
 
-        data.fillna(value = '', inplace = True)
-
         if print_data:
             print(f'Mechanical Powertrain Status at Time = {target_time}')
-            print(data.to_string())
+            print(data.astype(float).fillna(value = '').to_string())
 
         return data
 
     def plot(self,
              elements: Optional[list[RotatingObject | str]] = None,
              variables: Optional[list[str]] = None,
              angular_position_unit: Optional[str] = 'rad',
```

### Comparing `gearpy-0.7.2/gearpy/sensors/absolute_rotary_encoder.py` & `gearpy-1.0.0/gearpy/sensors/absolute_rotary_encoder.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/sensors/amperometer.py` & `gearpy-1.0.0/gearpy/sensors/amperometer.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/sensors/sensor_base.py` & `gearpy-1.0.0/gearpy/sensors/sensor_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/sensors/tachometer.py` & `gearpy-1.0.0/gearpy/sensors/tachometer.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/sensors/timer.py` & `gearpy-1.0.0/gearpy/sensors/timer.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/solver.py` & `gearpy-1.0.0/gearpy/solver.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/units/unit_base.py` & `gearpy-1.0.0/gearpy/units/unit_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/units/units.py` & `gearpy-1.0.0/gearpy/units/units.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/animate.py` & `gearpy-1.0.0/gearpy/utils/animate.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/export.py` & `gearpy-1.0.0/gearpy/utils/export.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/relations.py` & `gearpy-1.0.0/gearpy/utils/relations.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/stop_condition/operator.py` & `gearpy-1.0.0/gearpy/utils/stop_condition/operator.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/stop_condition/operator_base.py` & `gearpy-1.0.0/gearpy/utils/stop_condition/operator_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy/utils/stop_condition/stop_condition.py` & `gearpy-1.0.0/gearpy/utils/stop_condition/stop_condition.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/gearpy.egg-info/PKG-INFO` & `gearpy-1.0.0/gearpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearpy
-Version: 0.7.2
+Version: 1.0.0
 Summary: Python library for mechanical transmission analysis
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,31 +679,32 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/gearpy
 Project-URL: Documentation, https://gearpy.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/gearpy/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/gearpy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: matplotlib==3.8.0
-Requires-Dist: numpy==1.26.0
-Requires-Dist: pandas==2.1.1
-Requires-Dist: scipy==1.11.3
+Requires-Dist: matplotlib>=3.5
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=1.2
+Requires-Dist: scipy!=1.11.0,>=1.6
 Provides-Extra: doc
 Requires-Dist: furo==2023.9.10; extra == "doc"
 Requires-Dist: m2r2==0.3.3.post2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.1; extra == "test"
@@ -721,15 +722,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -743,15 +744,19 @@
    :target: https://pypi.org/project/gearpy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/gearpy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/gearpy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/gearpy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `gearpy-0.7.2/gearpy.egg-info/SOURCES.txt` & `gearpy-1.0.0/gearpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.2/pyproject.toml` & `gearpy-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gearpy"
 dynamic = ["version"]
-requires-python = ">=3.9,<3.13"
+requires-python = ">=3.9"
 dependencies = [
-  "matplotlib==3.8.0",
-  "numpy==1.26.0",
-  "pandas==2.1.1",
-  "scipy==1.11.3",
+  "matplotlib>=3.5",
+  "numpy>=1.20",
+  "pandas>=1.2",
+  "scipy>=1.6,!=1.11.0",
 ]
 authors = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 maintainers = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 description = "Python library for mechanical transmission analysis"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Education",
   "Intended Audience :: Manufacturing",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

