# Comparing `tmp/flycraft-0.0.7.tar.gz` & `tmp/flycraft-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flycraft-0.0.7.tar", last modified: Sun Mar 31 03:39:28 2024, max compression
+gzip compressed data, was "dist/flycraft-0.0.8.tar", last modified: Sat Apr 13 14:28:44 2024, max compression
```

## Comparing `flycraft-0.0.7.tar` & `flycraft-0.0.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.904433 flycraft-0.0.7/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1066 2024-03-09 07:32:53.000000 flycraft-0.0.7/LICENSE
--rw-rw-r--   0 ucav      (1000) ucav      (1000)       55 2024-03-09 13:10:22.000000 flycraft-0.0.7/MANIFEST.in
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2290 2024-03-31 03:39:28.904433 flycraft-0.0.7/PKG-INFO
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1283 2024-03-10 08:36:27.000000 flycraft-0.0.7/README.md
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.892433 flycraft-0.0.7/build/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.892433 flycraft-0.0.7/build/lib/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/build/lib/flycraft/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        5 2024-03-12 08:31:34.000000 flycraft-0.0.7/build/lib/flycraft/version.txt
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)      272 2024-03-04 11:58:58.000000 flycraft-0.0.7/flycraft/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     9532 2024-03-12 10:37:50.000000 flycraft-0.0.7/flycraft/env.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/planes/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:04:45.000000 flycraft-0.0.7/flycraft/planes/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     4714 2024-03-07 08:10:24.000000 flycraft-0.0.7/flycraft/planes/f16_plane.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/planes/utils/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:04:27.000000 flycraft-0.0.7/flycraft/planes/utils/__init__.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/f16/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/f16/lib/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/
--rw-r--r--   0 ucav      (1000) ucav      (1000)      359 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/nz_ka.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)      407 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/nz_kd.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)      287 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/nz_ki.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)       81 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/nz_max.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)      457 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/p_ka.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)      427 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/p_ki.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)      102 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/p_max.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)        0 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/r_kp.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)       45 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/rud_kp.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)       45 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/cl/rud_kpias.dat
--rw-r--r--   0 ucav      (1000) ucav      (1000)    65504 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/f16_air.lib
--rw-r--r--   0 ucav      (1000) ucav      (1000)        4 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/f16/lib/max_thrust_to_weight_ratio.dat
--rw-rw-r--   0 ucav      (1000) ucav      (1000)    10651 2024-03-01 09:42:55.000000 flycraft-0.0.7/flycraft/planes/utils/f16Classes.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/planes/utils/f16_utils/
--rw-r--r--   0 ucav      (1000) ucav      (1000)      425 2023-04-03 07:32:04.000000 flycraft-0.0.7/flycraft/planes/utils/f16_utils/__init__.py
--rw-r--r--   0 ucav      (1000) ucav      (1000)     1000 2023-04-03 07:32:04.000000 flycraft-0.0.7/flycraft/planes/utils/f16_utils/configLoader.py
--rw-r--r--   0 ucav      (1000) ucav      (1000)     1195 2023-04-03 07:32:04.000000 flycraft-0.0.7/flycraft/planes/utils/f16_utils/loggerOld.py
--rw-r--r--   0 ucav      (1000) ucav      (1000)      436 2023-04-03 07:32:04.000000 flycraft-0.0.7/flycraft/planes/utils/f16_utils/util.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/libs/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/libs/plane/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.896433 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/
--rw-r--r--   0 ucav      (1000) ucav      (1000)    31408 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/Guide1.so
--rw-r--r--   0 ucav      (1000) ucav      (1000)    69064 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/f16cl.so
--rw-r--r--   0 ucav      (1000) ucav      (1000)   131608 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/f16model.so
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/
--rw-r--r--   0 ucav      (1000) ucav      (1000)   624640 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/Guide1.dll
--rw-r--r--   0 ucav      (1000) ucav      (1000)    40448 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/f16cl.dll
--rw-r--r--   0 ucav      (1000) ucav      (1000)   192000 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/f16model.dll
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/libs/
--rw-r--r--   0 ucav      (1000) ucav      (1000)    65504 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/libs/f16_air.lib
--rw-r--r--   0 ucav      (1000) ucav      (1000)        4 2023-04-03 07:32:02.000000 flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/libs/max_thrust_to_weight_ratio.dat
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3404 2024-03-10 08:36:27.000000 flycraft-0.0.7/flycraft/planes/utils/testGuide.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/rewards/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2023-04-12 14:04:46.000000 flycraft-0.0.7/flycraft/rewards/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2715 2024-03-05 02:31:38.000000 flycraft-0.0.7/flycraft/rewards/dense_reward.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3415 2024-03-31 03:17:37.000000 flycraft-0.0.7/flycraft/rewards/dense_reward_based_on_angle_and_velocity.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     6563 2024-03-03 07:46:09.000000 flycraft-0.0.7/flycraft/rewards/ponential_reward.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3153 2024-03-05 02:31:47.000000 flycraft-0.0.7/flycraft/rewards/ponential_reward_based_on_angle.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1699 2024-03-03 07:56:19.000000 flycraft-0.0.7/flycraft/rewards/ponential_reward_based_on_velocity.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3712 2024-03-03 08:00:55.000000 flycraft-0.0.7/flycraft/rewards/reach_target_reward.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1342 2023-04-12 14:04:46.000000 flycraft-0.0.7/flycraft/rewards/reward_base.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/tasks/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:05:01.000000 flycraft-0.0.7/flycraft/tasks/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)    18603 2024-03-31 03:21:53.000000 flycraft-0.0.7/flycraft/tasks/attitude_control_task.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     4795 2024-03-12 08:15:34.000000 flycraft-0.0.7/flycraft/tasks/goal_sampler.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1452 2024-03-05 08:44:22.000000 flycraft-0.0.7/flycraft/tasks/task_base.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft/terminations/
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2023-04-12 14:04:46.000000 flycraft-0.0.7/flycraft/terminations/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     6612 2024-03-03 06:49:33.000000 flycraft-0.0.7/flycraft/terminations/continuousely_move_away_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     6599 2024-03-05 02:32:57.000000 flycraft-0.0.7/flycraft/terminations/continuousely_move_away_termination2.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3488 2024-03-05 02:32:55.000000 flycraft-0.0.7/flycraft/terminations/continuousely_roll_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1959 2024-03-01 01:51:09.000000 flycraft-0.0.7/flycraft/terminations/crash_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2488 2024-03-01 01:51:01.000000 flycraft-0.0.7/flycraft/terminations/extreme_state_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2787 2024-03-01 01:50:55.000000 flycraft-0.0.7/flycraft/terminations/negative_overload_and_big_phi_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     5047 2024-03-03 07:16:31.000000 flycraft-0.0.7/flycraft/terminations/reach_target_termination.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     4706 2024-03-05 02:32:53.000000 flycraft-0.0.7/flycraft/terminations/reach_target_termination2.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3036 2024-03-05 02:32:51.000000 flycraft-0.0.7/flycraft/terminations/reach_target_termination_single_step.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     3602 2024-03-03 06:53:45.000000 flycraft-0.0.7/flycraft/terminations/termination_base.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1849 2024-03-01 01:50:25.000000 flycraft-0.0.7/flycraft/terminations/timeout_termination.py
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.904433 flycraft-0.0.7/flycraft/utils/
--rw-r--r--   0 ucav      (1000) ucav      (1000)        0 2023-04-04 03:39:16.000000 flycraft-0.0.7/flycraft/utils/__init__.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2144 2023-04-12 14:04:46.000000 flycraft-0.0.7/flycraft/utils/attitude_angle_calc_utils.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1916 2024-03-10 01:35:34.000000 flycraft-0.0.7/flycraft/utils/csv2acmi.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)      234 2024-03-02 13:29:49.000000 flycraft-0.0.7/flycraft/utils/dict_utils.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     2790 2024-03-04 02:21:18.000000 flycraft-0.0.7/flycraft/utils/geometry_utils.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)      123 2024-03-01 07:45:32.000000 flycraft-0.0.7/flycraft/utils/load_config.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1393 2024-03-12 08:15:34.000000 flycraft-0.0.7/flycraft/utils/my_log.py
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        5 2024-03-31 03:24:00.000000 flycraft-0.0.7/flycraft/version.txt
-drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-03-31 03:39:28.900433 flycraft-0.0.7/flycraft.egg-info/
--rw-r--r--   0 ucav      (1000) ucav      (1000)     2290 2024-03-31 03:39:28.000000 flycraft-0.0.7/flycraft.egg-info/PKG-INFO
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     4116 2024-03-31 03:39:28.000000 flycraft-0.0.7/flycraft.egg-info/SOURCES.txt
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        1 2024-03-31 03:39:28.000000 flycraft-0.0.7/flycraft.egg-info/dependency_links.txt
--rw-rw-r--   0 ucav      (1000) ucav      (1000)       94 2024-03-31 03:39:28.000000 flycraft-0.0.7/flycraft.egg-info/requires.txt
--rw-rw-r--   0 ucav      (1000) ucav      (1000)        9 2024-03-31 03:39:28.000000 flycraft-0.0.7/flycraft.egg-info/top_level.txt
--rw-rw-r--   0 ucav      (1000) ucav      (1000)       38 2024-03-31 03:39:28.904433 flycraft-0.0.7/setup.cfg
--rw-rw-r--   0 ucav      (1000) ucav      (1000)     1094 2024-03-09 13:10:22.000000 flycraft-0.0.7/setup.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.843651 flycraft-0.0.8/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1066 2024-03-09 07:32:53.000000 flycraft-0.0.8/LICENSE
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)       55 2024-03-09 13:10:22.000000 flycraft-0.0.8/MANIFEST.in
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2290 2024-04-13 14:28:44.843651 flycraft-0.0.8/PKG-INFO
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1283 2024-03-10 08:36:27.000000 flycraft-0.0.8/README.md
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.831648 flycraft-0.0.8/build/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.831648 flycraft-0.0.8/build/lib/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.835649 flycraft-0.0.8/build/lib/flycraft/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        5 2024-03-12 08:31:34.000000 flycraft-0.0.8/build/lib/flycraft/version.txt
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)      272 2024-03-04 11:58:58.000000 flycraft-0.0.8/flycraft/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     9532 2024-03-12 10:37:50.000000 flycraft-0.0.8/flycraft/env.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/planes/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:04:45.000000 flycraft-0.0.8/flycraft/planes/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     4714 2024-03-07 08:10:24.000000 flycraft-0.0.8/flycraft/planes/f16_plane.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/planes/utils/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:04:27.000000 flycraft-0.0.8/flycraft/planes/utils/__init__.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.831648 flycraft-0.0.8/flycraft/planes/utils/f16/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.835649 flycraft-0.0.8/flycraft/planes/utils/f16/lib/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.835649 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      359 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/nz_ka.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      407 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/nz_kd.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      287 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/nz_ki.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)       81 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/nz_max.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      457 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/p_ka.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      427 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/p_ki.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      102 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/p_max.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)        0 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/r_kp.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)       45 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/rud_kp.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)       45 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/cl/rud_kpias.dat
+-rw-r--r--   0 ucav      (1000) ucav      (1000)    65504 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/f16_air.lib
+-rw-r--r--   0 ucav      (1000) ucav      (1000)        4 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/f16/lib/max_thrust_to_weight_ratio.dat
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)    10651 2024-03-01 09:42:55.000000 flycraft-0.0.8/flycraft/planes/utils/f16Classes.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/planes/utils/f16_utils/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      425 2023-04-03 07:32:04.000000 flycraft-0.0.8/flycraft/planes/utils/f16_utils/__init__.py
+-rw-r--r--   0 ucav      (1000) ucav      (1000)     1000 2023-04-03 07:32:04.000000 flycraft-0.0.8/flycraft/planes/utils/f16_utils/configLoader.py
+-rw-r--r--   0 ucav      (1000) ucav      (1000)     1195 2023-04-03 07:32:04.000000 flycraft-0.0.8/flycraft/planes/utils/f16_utils/loggerOld.py
+-rw-r--r--   0 ucav      (1000) ucav      (1000)      436 2023-04-03 07:32:04.000000 flycraft-0.0.8/flycraft/planes/utils/f16_utils/util.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.831648 flycraft-0.0.8/flycraft/planes/utils/libs/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.831648 flycraft-0.0.8/flycraft/planes/utils/libs/plane/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.835649 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.835649 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)    31408 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/Guide1.so
+-rw-r--r--   0 ucav      (1000) ucav      (1000)    69064 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/f16cl.so
+-rw-r--r--   0 ucav      (1000) ucav      (1000)   131608 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/f16model.so
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)   624640 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/Guide1.dll
+-rw-r--r--   0 ucav      (1000) ucav      (1000)    40448 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/f16cl.dll
+-rw-r--r--   0 ucav      (1000) ucav      (1000)   192000 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/f16model.dll
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/libs/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)    65504 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/libs/f16_air.lib
+-rw-r--r--   0 ucav      (1000) ucav      (1000)        4 2023-04-03 07:32:02.000000 flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/libs/max_thrust_to_weight_ratio.dat
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3404 2024-03-10 08:36:27.000000 flycraft-0.0.8/flycraft/planes/utils/testGuide.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.843651 flycraft-0.0.8/flycraft/rewards/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2023-04-12 14:04:46.000000 flycraft-0.0.8/flycraft/rewards/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2715 2024-03-05 02:31:38.000000 flycraft-0.0.8/flycraft/rewards/dense_reward.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3415 2024-03-31 03:17:37.000000 flycraft-0.0.8/flycraft/rewards/dense_reward_based_on_angle_and_velocity.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     6563 2024-03-03 07:46:09.000000 flycraft-0.0.8/flycraft/rewards/ponential_reward.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3153 2024-03-05 02:31:47.000000 flycraft-0.0.8/flycraft/rewards/ponential_reward_based_on_angle.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1699 2024-03-03 07:56:19.000000 flycraft-0.0.8/flycraft/rewards/ponential_reward_based_on_velocity.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1342 2023-04-12 14:04:46.000000 flycraft-0.0.8/flycraft/rewards/reward_base.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3934 2024-04-13 07:25:51.000000 flycraft-0.0.8/flycraft/rewards/sparse_reward.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.843651 flycraft-0.0.8/flycraft/tasks/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2024-03-05 01:05:01.000000 flycraft-0.0.8/flycraft/tasks/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)    18982 2024-04-13 13:51:40.000000 flycraft-0.0.8/flycraft/tasks/attitude_control_task.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     4795 2024-03-12 08:15:34.000000 flycraft-0.0.8/flycraft/tasks/goal_sampler.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1452 2024-03-05 08:44:22.000000 flycraft-0.0.8/flycraft/tasks/task_base.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.843651 flycraft-0.0.8/flycraft/terminations/
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        0 2023-04-12 14:04:46.000000 flycraft-0.0.8/flycraft/terminations/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     6612 2024-03-03 06:49:33.000000 flycraft-0.0.8/flycraft/terminations/continuousely_move_away_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     6599 2024-03-05 02:32:57.000000 flycraft-0.0.8/flycraft/terminations/continuousely_move_away_termination2.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3488 2024-03-05 02:32:55.000000 flycraft-0.0.8/flycraft/terminations/continuousely_roll_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1959 2024-03-01 01:51:09.000000 flycraft-0.0.8/flycraft/terminations/crash_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2488 2024-03-01 01:51:01.000000 flycraft-0.0.8/flycraft/terminations/extreme_state_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2787 2024-03-01 01:50:55.000000 flycraft-0.0.8/flycraft/terminations/negative_overload_and_big_phi_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     5047 2024-03-03 07:16:31.000000 flycraft-0.0.8/flycraft/terminations/reach_target_termination.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     4706 2024-03-05 02:32:53.000000 flycraft-0.0.8/flycraft/terminations/reach_target_termination2.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3036 2024-03-05 02:32:51.000000 flycraft-0.0.8/flycraft/terminations/reach_target_termination_single_step.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     3602 2024-03-03 06:53:45.000000 flycraft-0.0.8/flycraft/terminations/termination_base.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1849 2024-03-01 01:50:25.000000 flycraft-0.0.8/flycraft/terminations/timeout_termination.py
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.843651 flycraft-0.0.8/flycraft/utils/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)        0 2023-04-04 03:39:16.000000 flycraft-0.0.8/flycraft/utils/__init__.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2144 2023-04-12 14:04:46.000000 flycraft-0.0.8/flycraft/utils/attitude_angle_calc_utils.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1916 2024-03-10 01:35:34.000000 flycraft-0.0.8/flycraft/utils/csv2acmi.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)      234 2024-03-02 13:29:49.000000 flycraft-0.0.8/flycraft/utils/dict_utils.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     2790 2024-03-04 02:21:18.000000 flycraft-0.0.8/flycraft/utils/geometry_utils.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)      123 2024-03-01 07:45:32.000000 flycraft-0.0.8/flycraft/utils/load_config.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1393 2024-03-12 08:15:34.000000 flycraft-0.0.8/flycraft/utils/my_log.py
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        5 2024-04-13 13:51:47.000000 flycraft-0.0.8/flycraft/version.txt
+drwxrwxr-x   0 ucav      (1000) ucav      (1000)        0 2024-04-13 14:28:44.839650 flycraft-0.0.8/flycraft.egg-info/
+-rw-r--r--   0 ucav      (1000) ucav      (1000)     2290 2024-04-13 14:28:44.000000 flycraft-0.0.8/flycraft.egg-info/PKG-INFO
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     4110 2024-04-13 14:28:44.000000 flycraft-0.0.8/flycraft.egg-info/SOURCES.txt
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        1 2024-04-13 14:28:44.000000 flycraft-0.0.8/flycraft.egg-info/dependency_links.txt
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)       94 2024-04-13 14:28:44.000000 flycraft-0.0.8/flycraft.egg-info/requires.txt
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)        9 2024-04-13 14:28:44.000000 flycraft-0.0.8/flycraft.egg-info/top_level.txt
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)       38 2024-04-13 14:28:44.843651 flycraft-0.0.8/setup.cfg
+-rw-rw-r--   0 ucav      (1000) ucav      (1000)     1094 2024-03-09 13:10:22.000000 flycraft-0.0.8/setup.py
```

### Comparing `flycraft-0.0.7/LICENSE` & `flycraft-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/PKG-INFO` & `flycraft-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flycraft
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fixed-wing UAV environment based on gymnasium.
 Home-page: https://github.com/gongxudong/fly-craft
 Author: Xudong Gong
 Author-email: gongxudong_cs@aliyun.com
 License: UNKNOWN
 Description: # fly-craft
```

### Comparing `flycraft-0.0.7/README.md` & `flycraft-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/env.py` & `flycraft-0.0.8/flycraft/env.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/f16_plane.py` & `flycraft-0.0.8/flycraft/planes/f16_plane.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/f16/lib/f16_air.lib` & `flycraft-0.0.8/flycraft/planes/utils/f16/lib/f16_air.lib`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/f16Classes.py` & `flycraft-0.0.8/flycraft/planes/utils/f16Classes.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/f16_utils/configLoader.py` & `flycraft-0.0.8/flycraft/planes/utils/f16_utils/configLoader.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/f16_utils/loggerOld.py` & `flycraft-0.0.8/flycraft/planes/utils/f16_utils/loggerOld.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/Guide1.so` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/Guide1.so`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/f16cl.so` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/f16cl.so`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/ubuntu/f16model.so` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/ubuntu/f16model.so`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/Guide1.dll` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/Guide1.dll`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/f16cl.dll` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/f16cl.dll`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/f16model.dll` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/f16model.dll`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/libs/plane/f16/x64/libs/f16_air.lib` & `flycraft-0.0.8/flycraft/planes/utils/libs/plane/f16/x64/libs/f16_air.lib`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/planes/utils/testGuide.py` & `flycraft-0.0.8/flycraft/planes/utils/testGuide.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/dense_reward.py` & `flycraft-0.0.8/flycraft/rewards/dense_reward.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/dense_reward_based_on_angle_and_velocity.py` & `flycraft-0.0.8/flycraft/rewards/dense_reward_based_on_angle_and_velocity.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/ponential_reward.py` & `flycraft-0.0.8/flycraft/rewards/ponential_reward.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/ponential_reward_based_on_angle.py` & `flycraft-0.0.8/flycraft/rewards/ponential_reward_based_on_angle.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/ponential_reward_based_on_velocity.py` & `flycraft-0.0.8/flycraft/rewards/ponential_reward_based_on_velocity.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/rewards/reach_target_reward.py` & `flycraft-0.0.8/flycraft/rewards/sparse_reward.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,55 +8,59 @@
 PROJECT_ROOT_DIR = Path(__file__).parent.parent
 if str(PROJECT_ROOT_DIR.absolute()) not in sys.path:
     sys.path.append(str(PROJECT_ROOT_DIR.absolute()))
     
 from rewards.reward_base import RewardBase
 
 
-class ReachTargetReward(RewardBase):
+class SparseReward(RewardBase):
 
     def __init__(self, 
         is_potential: bool = False, log_history_reward: bool=False,
         step_frequence: int=100, integral_time_length: float=1.,
-        v_threshold=10., mu_threshold=1., chi_threshold=1., 
+        v_threshold: float=10., mu_threshold: float=1., chi_threshold: float=1.,
+        reach_target_reward: float=0., else_reward: float=0. 
     ) -> None:
         super().__init__(is_potential=is_potential, log_history_reward=log_history_reward)
 
         self.is_potential = is_potential
         
         self.step_frequence = step_frequence
         self.integral_time_length = integral_time_length
         
         self.v_threshold = v_threshold
         self.mu_threshold = mu_threshold
         self.chi_threshold = chi_threshold
 
+        self.reach_target_reward = reach_target_reward
+        self.else_reward = else_reward
+
     def get_reward(self, state: Union[namedtuple, np.ndarray], **kwargs) -> float:
         assert "goal_v" in kwargs, "参数中需要包括goal_v，再调用get_termination方法"
         assert "goal_mu" in kwargs, "参数中需要包括goal_mu，再调用get_termination方法"
         assert "goal_chi" in kwargs, "参数中需要包括goal_chi，再调用get_termination方法"
         assert "state_list" in kwargs, "参数中需要包括state_list（list[namedtuple]类型，所有历史观测），再调用get_reward方法"
         assert type(kwargs["state_list"]) is list, "state_list参数的类型应该是list[namedtuple]"
 
         state_list = kwargs["state_list"]  # list[namedtuple], GuideEnv.get_state_vars()返回的namedtuple
 
         if len(state_list) < self.integral_window_length:
-            return 0.
+            return self.else_reward
         else:
             v_flag, mu_flag, chi_flag = False, False, False
             if sum([abs(kwargs["goal_v"] - item.v) for item in state_list[-self.integral_window_length:]]) < self.v_integral_threshold:
                 v_flag = True
             if sum([abs(kwargs["goal_mu"] - item.mu) for item in state_list[-self.integral_window_length:]]) < self.mu_integral_threshold:
                 mu_flag = True
             if sum([abs(kwargs["goal_chi"] - item.chi) for item in state_list[-self.integral_window_length:]]) < self.chi_integral_threshold:
                 chi_flag = True
             if v_flag and mu_flag and chi_flag:
-                return 1.
+                return self.reach_target_reward
             else:
-                return 0.
+                return self.else_reward
     
     def reset(self):
         super().reset()
 
     @property
     def integral_window_length(self):
         """v, mu, chi的积分窗口长度
```

### Comparing `flycraft-0.0.7/flycraft/rewards/reward_base.py` & `flycraft-0.0.8/flycraft/rewards/reward_base.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/tasks/attitude_control_task.py` & `flycraft-0.0.8/flycraft/tasks/attitude_control_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from planes.f16_plane import F16Plane
 from tasks.task_base import Task
 from tasks.goal_sampler import GoalSampler
 
 from rewards.reward_base import RewardBase
 from rewards.dense_reward_based_on_angle_and_velocity import DenseRewardBasedOnAngleAndVelocity
+from rewards.sparse_reward import SparseReward
 
 from terminations.termination_base import TerminationBase
 from terminations.reach_target_termination2 import ReachTargetTermination2
 from terminations.reach_target_termination_single_step import ReachTargetTerminationSingleStep
 from terminations.crash_termination import CrashTermination
 from terminations.extreme_state_termination import ExtremeStateTermination
 from terminations.timeout_termination import TimeoutTermination
@@ -148,14 +149,21 @@
                         DenseRewardBasedOnAngleAndVelocity(
                             b=tmp_cfg.get("b", 0.5),
                             angle_scale=tmp_cfg.get("angle_scale", 180),
                             velocity_scale=tmp_cfg.get("velocity_scale", 100),
                             angle_weight=tmp_cfg.get("angle_weight", 0.5),
                         )
                     )
+                elif rwd == "sparse":
+                    self.reward_funcs.append(
+                        SparseReward(
+                            reach_target_reward=tmp_cfg.get("reach_target_reward", 0.0),
+                            else_reward=tmp_cfg.get("else_reward", 0.0),
+                        )
+                    )
                 # TODO: other rewards
 
     def _prep_termination_funcs(self):
         # TODO: 如何设置优先级？？？
         self.termination_funcs = []
 
         for tmnt in self.config["terminations"]:
```

### Comparing `flycraft-0.0.7/flycraft/tasks/goal_sampler.py` & `flycraft-0.0.8/flycraft/tasks/goal_sampler.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/tasks/task_base.py` & `flycraft-0.0.8/flycraft/tasks/task_base.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/continuousely_move_away_termination.py` & `flycraft-0.0.8/flycraft/terminations/continuousely_move_away_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/continuousely_move_away_termination2.py` & `flycraft-0.0.8/flycraft/terminations/continuousely_move_away_termination2.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/continuousely_roll_termination.py` & `flycraft-0.0.8/flycraft/terminations/continuousely_roll_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/crash_termination.py` & `flycraft-0.0.8/flycraft/terminations/crash_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/extreme_state_termination.py` & `flycraft-0.0.8/flycraft/terminations/extreme_state_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/negative_overload_and_big_phi_termination.py` & `flycraft-0.0.8/flycraft/terminations/negative_overload_and_big_phi_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/reach_target_termination.py` & `flycraft-0.0.8/flycraft/terminations/reach_target_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/reach_target_termination2.py` & `flycraft-0.0.8/flycraft/terminations/reach_target_termination2.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/reach_target_termination_single_step.py` & `flycraft-0.0.8/flycraft/terminations/reach_target_termination_single_step.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/termination_base.py` & `flycraft-0.0.8/flycraft/terminations/termination_base.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/terminations/timeout_termination.py` & `flycraft-0.0.8/flycraft/terminations/timeout_termination.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/utils/attitude_angle_calc_utils.py` & `flycraft-0.0.8/flycraft/utils/attitude_angle_calc_utils.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/utils/csv2acmi.py` & `flycraft-0.0.8/flycraft/utils/csv2acmi.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/utils/geometry_utils.py` & `flycraft-0.0.8/flycraft/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft/utils/my_log.py` & `flycraft-0.0.8/flycraft/utils/my_log.py`

 * *Files identical despite different names*

### Comparing `flycraft-0.0.7/flycraft.egg-info/PKG-INFO` & `flycraft-0.0.8/flycraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flycraft
-Version: 0.0.7
+Version: 0.0.8
 Summary: A fixed-wing UAV environment based on gymnasium.
 Home-page: https://github.com/gongxudong/fly-craft
 Author: Xudong Gong
 Author-email: gongxudong_cs@aliyun.com
 License: UNKNOWN
 Description: # fly-craft
```

### Comparing `flycraft-0.0.7/flycraft.egg-info/SOURCES.txt` & `flycraft-0.0.8/flycraft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 flycraft/planes/utils/libs/plane/f16/x64/libs/max_thrust_to_weight_ratio.dat
 flycraft/rewards/__init__.py
 flycraft/rewards/dense_reward.py
 flycraft/rewards/dense_reward_based_on_angle_and_velocity.py
 flycraft/rewards/ponential_reward.py
 flycraft/rewards/ponential_reward_based_on_angle.py
 flycraft/rewards/ponential_reward_based_on_velocity.py
-flycraft/rewards/reach_target_reward.py
 flycraft/rewards/reward_base.py
+flycraft/rewards/sparse_reward.py
 flycraft/tasks/__init__.py
 flycraft/tasks/attitude_control_task.py
 flycraft/tasks/goal_sampler.py
 flycraft/tasks/task_base.py
 flycraft/terminations/__init__.py
 flycraft/terminations/continuousely_move_away_termination.py
 flycraft/terminations/continuousely_move_away_termination2.py
```

### Comparing `flycraft-0.0.7/setup.py` & `flycraft-0.0.8/setup.py`

 * *Files identical despite different names*

