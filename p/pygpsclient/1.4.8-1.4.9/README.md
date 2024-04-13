# Comparing `tmp/pygpsclient-1.4.8.tar.gz` & `tmp/pygpsclient-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpsclient-1.4.8.tar", last modified: Thu Jan 18 14:24:36 2024, max compression
+gzip compressed data, was "pygpsclient-1.4.9.tar", last modified: Tue Feb  6 07:58:59 2024, max compression
```

## Comparing `pygpsclient-1.4.8.tar` & `pygpsclient-1.4.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.242580 pygpsclient-1.4.8/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)      102 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    55883 2024-01-18 14:24:36.242038 pygpsclient-1.4.8/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    52233 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/README.md
--rw-r--r--   0 steve      (501) staff       (20)     3200 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-01-18 14:24:36.242710 pygpsclient-1.4.8/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.205542 pygpsclient-1.4.8/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.215885 pygpsclient-1.4.8/src/pygpsclient/
--rw-r--r--   0 steve      (501) staff       (20)      222 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     2676 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/__main__.py
--rw-r--r--   0 steve      (501) staff       (20)      166 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     6883 2024-01-07 08:55:16.000000 pygpsclient-1.4.8/src/pygpsclient/about_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)    34343 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/app.py
--rw-r--r--   0 steve      (501) staff       (20)    21610 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/banner_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     6782 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/console_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     1075 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/dialog_state.py
--rw-r--r--   0 steve      (501) staff       (20)    14569 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/file_handler.py
--rw-r--r--   0 steve      (501) staff       (20)    10564 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/globals.py
--rw-r--r--   0 steve      (501) staff       (20)     2051 2024-01-15 14:17:56.000000 pygpsclient-1.4.8/src/pygpsclient/gnss_status.py
--rw-r--r--   0 steve      (501) staff       (20)    20429 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/gpx_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)     6224 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/graphview_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    24213 2024-01-07 08:50:11.000000 pygpsclient-1.4.8/src/pygpsclient/helpers.py
--rw-r--r--   0 steve      (501) staff       (20)    12411 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/map_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     3304 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/mapquest.py
--rw-r--r--   0 steve      (501) staff       (20)     3226 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/menu_bar.py
--rw-r--r--   0 steve      (501) staff       (20)    13078 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/nmea_handler.py
--rw-r--r--   0 steve      (501) staff       (20)    25308 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/ntrip_client_dialog.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.226384 pygpsclient-1.4.8/src/pygpsclient/resources/
--rw-r--r--   0 steve      (501) staff       (20)     9309 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/binary-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)      576 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/blank-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)      575 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/clear-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)     9507 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/ethernet-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)      714 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-antenna-3-24.png
--rw-r--r--   0 steve      (501) staff       (20)      808 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-antenna-4-24.png
--rw-r--r--   0 steve      (501) staff       (20)      269 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-arrow-12-24.png
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-arrow-80-16.png
--rw-r--r--   0 steve      (501) staff       (20)      844 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png
--rw-r--r--   0 steve      (501) staff       (20)      395 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-door-6-24.png
--rw-r--r--   0 steve      (501) staff       (20)      305 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-folder-18-24.png
--rw-r--r--   0 steve      (501) staff       (20)     1037 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-gear-2-24.png
--rw-r--r--   0 steve      (501) staff       (20)      439 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-location-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)     1724 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-location-27-32.png
--rw-r--r--   0 steve      (501) staff       (20)      331 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-media-control-48-24.png
--rw-r--r--   0 steve      (501) staff       (20)      125 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-media-control-50-24.png
--rw-r--r--   0 steve      (501) staff       (20)    10472 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-noclient-10-24.png
--rw-r--r--   0 steve      (501) staff       (20)     8807 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-record-24.png
--rw-r--r--   0 steve      (501) staff       (20)      442 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-refresh-6-16.png
--rw-r--r--   0 steve      (501) staff       (20)      495 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-refresh-lined-24.png
--rw-r--r--   0 steve      (501) staff       (20)      205 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-save-14-24.png
--rw-r--r--   0 steve      (501) staff       (20)      119 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-stop-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)      875 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-time-6-24.png
--rw-r--r--   0 steve      (501) staff       (20)      860 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-transmit-10-24.png
--rw-r--r--   0 steve      (501) staff       (20)      326 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-trash-can-filled-24.png
--rw-r--r--   0 steve      (501) staff       (20)      276 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-triangle-1-16.png
--rw-r--r--   0 steve      (501) staff       (20)     7751 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-undo-24.png
--rw-r--r--   0 steve      (501) staff       (20)      466 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-warning-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)     4286 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/pygpsclient.ico
--rw-r--r--   0 steve      (501) staff       (20)     5424 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/usbport-1-24.png
--rw-r--r--   0 steve      (501) staff       (20)   327167 2023-07-18 14:52:16.000000 pygpsclient-1.4.8/src/pygpsclient/resources/world.png
--rw-r--r--   0 steve      (501) staff       (20)     9537 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/rover_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     1226 2023-08-07 21:45:30.000000 pygpsclient-1.4.8/src/pygpsclient/rtcm3_handler.py
--rw-r--r--   0 steve      (501) staff       (20)     8321 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/scatter_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    18917 2023-10-05 07:26:57.000000 pygpsclient-1.4.8/src/pygpsclient/serialconfig_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    29923 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/serverconfig_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    35372 2024-01-18 14:22:55.000000 pygpsclient-1.4.8/src/pygpsclient/settings_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     5389 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/skyview_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     5451 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/socketconfig_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     9302 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/spartn_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)    17766 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/spartn_gnss_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     3948 2023-08-02 19:03:37.000000 pygpsclient-1.4.8/src/pygpsclient/spartn_json_config.py
--rw-r--r--   0 steve      (501) staff       (20)    25467 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/spartn_lband_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    16321 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/spartn_mqtt_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    14834 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/spectrum_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     3340 2023-08-24 07:28:55.000000 pygpsclient-1.4.8/src/pygpsclient/status_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     8998 2023-12-17 09:31:16.000000 pygpsclient-1.4.8/src/pygpsclient/stream_handler.py
--rw-r--r--   0 steve      (501) staff       (20)     7032 2024-01-18 09:33:37.000000 pygpsclient-1.4.8/src/pygpsclient/strings.py
--rw-r--r--   0 steve      (501) staff       (20)    13025 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/sysmon_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    14995 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_cfgval_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    11646 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_config_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)    16872 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_dynamic_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    18074 2024-01-07 08:55:16.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_handler.py
--rw-r--r--   0 steve      (501) staff       (20)     7170 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_info_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     9448 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_msgrate_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     9123 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_port_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    18624 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_preset_frame.py
--rw-r--r--   0 steve      (501) staff       (20)    15261 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_recorder_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     6980 2023-09-08 07:06:20.000000 pygpsclient-1.4.8/src/pygpsclient/ubx_solrate_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     3847 2023-09-13 16:37:19.000000 pygpsclient-1.4.8/src/pygpsclient/widget_state.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.236971 pygpsclient-1.4.8/src/pygpsclient.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    55883 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     3481 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       58 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      212 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       12 2024-01-18 14:24:36.000000 pygpsclient-1.4.8/src/pygpsclient.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-18 14:24:36.236545 pygpsclient-1.4.8/tests/
--rw-r--r--   0 steve      (501) staff       (20)    14114 2024-01-07 08:55:16.000000 pygpsclient-1.4.8/tests/test_static.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.956967 pygpsclient-1.4.9/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)      102 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    55913 2024-02-06 07:58:59.956709 pygpsclient-1.4.9/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    52233 2024-01-18 14:22:55.000000 pygpsclient-1.4.9/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     3222 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-02-06 07:58:59.957016 pygpsclient-1.4.9/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.942253 pygpsclient-1.4.9/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.950143 pygpsclient-1.4.9/src/pygpsclient/
+-rw-r--r--   0 steve      (501) staff       (20)      224 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     2676 2024-01-18 14:22:55.000000 pygpsclient-1.4.9/src/pygpsclient/__main__.py
+-rw-r--r--   0 steve      (501) staff       (20)      166 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     6883 2024-01-07 08:55:16.000000 pygpsclient-1.4.9/src/pygpsclient/about_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    34345 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/app.py
+-rw-r--r--   0 steve      (501) staff       (20)    21610 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/banner_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     6782 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/console_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     1075 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/dialog_state.py
+-rw-r--r--   0 steve      (501) staff       (20)    14569 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/file_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)    10566 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/globals.py
+-rw-r--r--   0 steve      (501) staff       (20)     2051 2024-01-15 14:17:56.000000 pygpsclient-1.4.9/src/pygpsclient/gnss_status.py
+-rw-r--r--   0 steve      (501) staff       (20)    20430 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/gpx_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)     6224 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/graphview_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    24197 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/helpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    12365 2024-01-22 18:35:39.000000 pygpsclient-1.4.9/src/pygpsclient/map_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3304 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/mapquest.py
+-rw-r--r--   0 steve      (501) staff       (20)     3226 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/menu_bar.py
+-rw-r--r--   0 steve      (501) staff       (20)    13078 2023-12-17 09:31:16.000000 pygpsclient-1.4.9/src/pygpsclient/nmea_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)    25308 2023-12-17 09:31:16.000000 pygpsclient-1.4.9/src/pygpsclient/ntrip_client_dialog.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.955271 pygpsclient-1.4.9/src/pygpsclient/resources/
+-rw-r--r--   0 steve      (501) staff       (20)     9309 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/binary-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      576 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/blank-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      575 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/clear-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     9507 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/ethernet-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      714 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-antenna-3-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      808 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-antenna-4-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      269 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-arrow-12-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-arrow-80-16.png
+-rw-r--r--   0 steve      (501) staff       (20)      844 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      395 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-door-6-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      305 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-folder-18-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     1037 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-gear-2-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      439 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-location-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     1724 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-location-27-32.png
+-rw-r--r--   0 steve      (501) staff       (20)      331 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-media-control-48-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      125 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-media-control-50-24.png
+-rw-r--r--   0 steve      (501) staff       (20)    10472 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-noclient-10-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     8807 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-record-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      442 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-refresh-6-16.png
+-rw-r--r--   0 steve      (501) staff       (20)      495 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-refresh-lined-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      205 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-save-14-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      119 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-stop-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-time-6-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      860 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-transmit-10-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      326 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-trash-can-filled-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      276 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-triangle-1-16.png
+-rw-r--r--   0 steve      (501) staff       (20)     7751 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-undo-24.png
+-rw-r--r--   0 steve      (501) staff       (20)      466 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-warning-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)     4286 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/pygpsclient.ico
+-rw-r--r--   0 steve      (501) staff       (20)     5424 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/usbport-1-24.png
+-rw-r--r--   0 steve      (501) staff       (20)   327167 2023-07-18 14:52:16.000000 pygpsclient-1.4.9/src/pygpsclient/resources/world.png
+-rw-r--r--   0 steve      (501) staff       (20)     9539 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/rover_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     1226 2023-08-07 21:45:30.000000 pygpsclient-1.4.9/src/pygpsclient/rtcm3_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     8321 2024-01-18 14:22:55.000000 pygpsclient-1.4.9/src/pygpsclient/scatter_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    18917 2023-10-05 07:26:57.000000 pygpsclient-1.4.9/src/pygpsclient/serialconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    29925 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/serverconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    35374 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/settings_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     5389 2023-12-17 09:31:16.000000 pygpsclient-1.4.9/src/pygpsclient/skyview_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     5451 2023-12-17 09:31:16.000000 pygpsclient-1.4.9/src/pygpsclient/socketconfig_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9302 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/spartn_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    17766 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/spartn_gnss_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3948 2023-08-02 19:03:37.000000 pygpsclient-1.4.9/src/pygpsclient/spartn_json_config.py
+-rw-r--r--   0 steve      (501) staff       (20)    25467 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/spartn_lband_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    16321 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/spartn_mqtt_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    14834 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/spectrum_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3340 2023-08-24 07:28:55.000000 pygpsclient-1.4.9/src/pygpsclient/status_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     8998 2023-12-17 09:31:16.000000 pygpsclient-1.4.9/src/pygpsclient/stream_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     7034 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/strings.py
+-rw-r--r--   0 steve      (501) staff       (20)    13025 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/sysmon_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    14995 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_cfgval_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    11646 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_config_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    16872 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_dynamic_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    17973 2024-02-06 07:58:12.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_handler.py
+-rw-r--r--   0 steve      (501) staff       (20)     7170 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_info_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9448 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_msgrate_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     9123 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_port_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    18624 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_preset_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)    15261 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_recorder_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     6980 2023-09-08 07:06:20.000000 pygpsclient-1.4.9/src/pygpsclient/ubx_solrate_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     3847 2023-09-13 16:37:19.000000 pygpsclient-1.4.9/src/pygpsclient/widget_state.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.955766 pygpsclient-1.4.9/src/pygpsclient.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    55913 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     3481 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       58 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      227 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       12 2024-02-06 07:58:59.000000 pygpsclient-1.4.9/src/pygpsclient.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-02-06 07:58:59.955573 pygpsclient-1.4.9/tests/
+-rw-r--r--   0 steve      (501) staff       (20)    14114 2024-01-07 08:55:16.000000 pygpsclient-1.4.9/tests/test_static.py
```

### Comparing `pygpsclient-1.4.8/LICENSE` & `pygpsclient-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/PKG-INFO` & `pygpsclient-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpsclient
-Version: 1.4.8
+Version: 1.4.9
 Summary: GNSS Diagnostic and UBX Configuration GUI Application
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
@@ -59,14 +59,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.0
 Requires-Dist: Pillow>=9.0.0
 Requires-Dist: pygnssutils>=1.0.17
 Requires-Dist: pynmeagps>=1.0.33
 Requires-Dist: pyserial>=3.5
+Requires-Dist: pyubx2>=1.2.37
 Provides-Extra: deploy
 Requires-Dist: build; extra == "deploy"
 Requires-Dist: pip; extra == "deploy"
 Requires-Dist: setuptools>=66.0.0; extra == "deploy"
 Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
```

### Comparing `pygpsclient-1.4.8/README.md` & `pygpsclient-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/pyproject.toml` & `pygpsclient-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pygpsclient"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "GNSS Diagnostic and UBX Configuration GUI Application"
-version = "1.4.8"
+version = "1.4.9"
 license = { file = "LICENSE" }
 keywords = [
     "PyGPSClient",
     "GNSS",
     "GPS",
     "GALILEO",
     "GLONASS",
@@ -51,14 +51,15 @@
 
 dependencies = [
     "requests>=2.28.0",
     "Pillow>=9.0.0",
     "pygnssutils>=1.0.17",
     "pynmeagps>=1.0.33",
     "pyserial>=3.5",
+    "pyubx2>=1.2.37",
 ]
 
 [project.scripts]
 pygpsclient = "pygpsclient.__main__:main"
 
 [project.urls]
 homepage = "https://github.com/semuconsulting/PyGPSClient"
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/__main__.py` & `pygpsclient-1.4.9/src/pygpsclient/__main__.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/about_dialog.py` & `pygpsclient-1.4.9/src/pygpsclient/about_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/app.py` & `pygpsclient-1.4.9/src/pygpsclient/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
+
 # pylint: disable=too-many-ancestors, no-member
 
 from datetime import datetime, timedelta
 from os import getenv, path
 from pathlib import Path
 from queue import Empty, Queue
 from socket import AF_INET, AF_INET6
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/banner_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/banner_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/console_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/console_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/dialog_state.py` & `pygpsclient-1.4.9/src/pygpsclient/dialog_state.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/file_handler.py` & `pygpsclient-1.4.9/src/pygpsclient/file_handler.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/globals.py` & `pygpsclient-1.4.9/src/pygpsclient/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Created on 14 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 
 """
+
 # pylint: disable=line-too-long
 
 from collections import namedtuple
 from datetime import datetime
 from os import path
 from pathlib import Path
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/gnss_status.py` & `pygpsclient-1.4.9/src/pygpsclient/gnss_status.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/gpx_dialog.py` & `pygpsclient-1.4.9/src/pygpsclient/gpx_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Created on 10 Jan 2023
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
+
 # pylint: disable=unused-argument
 
 from datetime import datetime
 from http.client import responses
 from io import BytesIO
 from tkinter import (
     BOTH,
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/graphview_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/graphview_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/helpers.py` & `pygpsclient-1.4.9/src/pygpsclient/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,17 +697,15 @@
     :rtype: int
     """
 
     lbb = len(bitfield) * 8
     if position + length > lbb:
         return None
 
-    return (
-        int.from_bytes(bitfield, "big") >> (lbb - position - length) & 2**length - 1
-    )
+    return int.from_bytes(bitfield, "big") >> (lbb - position - length) & 2**length - 1
 
 
 def parse_rxmspartnkey(msg: UBXMessage) -> list:
     """
     Extract dates and keys from RXM-SPARTNKEY message.
 
     :param UBXMessage msg: RXM-SPARTNKEY message
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/map_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/map_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,17 +181,15 @@
 
         OFFSET_X = 0
         OFFSET_Y = 0
 
         self._lastmaptype = "world"
         w, h = self.width, self.height
         self._can_mapview.delete("all")
-        self._img = ImageTk.PhotoImage(
-            Image.open(IMG_WORLD).resize((w, h))  # , Image.ANTIALIAS)
-        )
+        self._img = ImageTk.PhotoImage(Image.open(IMG_WORLD).resize((w, h)))
         self._marker = ImageTk.PhotoImage(Image.open(ICON_POS))
         self._can_mapview.create_image(0, 0, image=self._img, anchor=NW)
         x = (w / 2) + int((lon * (w / 360))) + OFFSET_X
         y = (h / 2) - int((lat * (h / 180))) + OFFSET_Y
         self._can_mapview.create_image(x, y, image=self._marker, anchor=S)
 
     def _draw_web_map(self, lat: float, lon: float, hacc: float, maptype: str = "map"):
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/mapquest.py` & `pygpsclient-1.4.9/src/pygpsclient/mapquest.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/menu_bar.py` & `pygpsclient-1.4.9/src/pygpsclient/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/nmea_handler.py` & `pygpsclient-1.4.9/src/pygpsclient/nmea_handler.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ntrip_client_dialog.py` & `pygpsclient-1.4.9/src/pygpsclient/ntrip_client_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/binary-1-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/binary-1-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/blank-1-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/blank-1-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/clear-1-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/clear-1-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/ethernet-1-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/ethernet-1-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-antenna-3-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-antenna-3-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-antenna-4-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-antenna-4-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-check-mark-8-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-gear-2-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-gear-2-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-location-27-32.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-location-27-32.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-noclient-10-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-noclient-10-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-record-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-record-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-time-6-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-time-6-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-transmit-10-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-transmit-10-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/iconmonstr-undo-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/iconmonstr-undo-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/pygpsclient.ico` & `pygpsclient-1.4.9/src/pygpsclient/resources/pygpsclient.ico`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/usbport-1-24.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/usbport-1-24.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/resources/world.png` & `pygpsclient-1.4.9/src/pygpsclient/resources/world.png`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/rover_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/rover_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Created on 22 Aug 2023
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
+
 # pylint: disable=invalid-name
 
 from math import cos, pi, sin
 from tkinter import BOTH, YES, Frame, font
 
 from pygpsclient.globals import BGCOL, FGCOL, WIDGETU2
 from pygpsclient.helpers import setubxrate
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/rtcm3_handler.py` & `pygpsclient-1.4.9/src/pygpsclient/rtcm3_handler.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/scatter_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/scatter_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/serialconfig_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/serialconfig_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/serverconfig_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/serverconfig_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 Created on 23 Jul 2023
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
+
 # pylint: disable=unused-argument
 
 from tkinter import (
     DISABLED,
     NORMAL,
     Button,
     Checkbutton,
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/settings_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/settings_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
+
 # pylint: disable=unnecessary-lambda
 
 from socket import AF_INET6
 from tkinter import (
     ALL,
     BOTH,
     BOTTOM,
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/skyview_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/skyview_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/socketconfig_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/socketconfig_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spartn_dialog.py` & `pygpsclient-1.4.9/src/pygpsclient/spartn_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spartn_gnss_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/spartn_gnss_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spartn_json_config.py` & `pygpsclient-1.4.9/src/pygpsclient/spartn_json_config.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spartn_lband_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/spartn_lband_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spartn_mqtt_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/spartn_mqtt_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/spectrum_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/spectrum_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/status_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/status_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/stream_handler.py` & `pygpsclient-1.4.9/src/pygpsclient/stream_handler.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/strings.py` & `pygpsclient-1.4.9/src/pygpsclient/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
+
 # pylint: disable=line-too-long
 
 TITLE = "PyGPSClient"
 
 COPYRIGHTTXT = "\u00A9 SEMU Consulting 2020\nBSD-2 License. All Rights Reserved"
 
 INTROTXT = "Welcome to PyGPSClient!"
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/sysmon_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/sysmon_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_cfgval_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_cfgval_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_config_dialog.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_dynamic_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_dynamic_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_handler.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,26 +364,26 @@
         NB: pyubx2 parses relPosHP values as mm, so total relPosN
         in cm = relPosN + (relPosHPN * 1e-1), etc.
 
         :param UBXMessage data: NAV-RELPOSNED parsed message
         """
 
         if data.version == 0x00:
-            n = data.relPosN + data.relPosHPN * 1e-1
-            e = data.relPosE + data.relPosHPE * 1e-1
-            d = data.relPosD + data.relPosHPD * 1e-1
+            n = data.relPosN
+            e = data.relPosE
+            d = data.relPosD
             relPosLength, relPosHeading = ned2vector(n, e, d)
             n = data.accN * 1e-2
             e = data.accE * 1e-2
             d = data.accD * 1e-2
             accLength, _ = ned2vector(n, e, d)
             accHeading = accLength * relPosHeading / relPosLength  # ballpark
         else:
             relPosLength, relPosHeading, accLength, accHeading = (
-                data.relPosLength + data.relPosHPLength * 1e-1,
+                data.relPosLength,
                 data.relPosHeading,
                 data.accLength * 1e-2,
                 data.accHeading,
             )
 
         self.__app.gnss_status.rel_pos_heading = relPosHeading
         self.__app.gnss_status.rel_pos_length = relPosLength
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_info_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_info_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_msgrate_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_msgrate_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_port_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_port_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_preset_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_preset_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_recorder_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_recorder_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/ubx_solrate_frame.py` & `pygpsclient-1.4.9/src/pygpsclient/ubx_solrate_frame.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient/widget_state.py` & `pygpsclient-1.4.9/src/pygpsclient/widget_state.py`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/src/pygpsclient.egg-info/PKG-INFO` & `pygpsclient-1.4.9/src/pygpsclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpsclient
-Version: 1.4.8
+Version: 1.4.9
 Summary: GNSS Diagnostic and UBX Configuration GUI Application
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
@@ -59,14 +59,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.0
 Requires-Dist: Pillow>=9.0.0
 Requires-Dist: pygnssutils>=1.0.17
 Requires-Dist: pynmeagps>=1.0.33
 Requires-Dist: pyserial>=3.5
+Requires-Dist: pyubx2>=1.2.37
 Provides-Extra: deploy
 Requires-Dist: build; extra == "deploy"
 Requires-Dist: pip; extra == "deploy"
 Requires-Dist: setuptools>=66.0.0; extra == "deploy"
 Requires-Dist: wheel; extra == "deploy"
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
```

### Comparing `pygpsclient-1.4.8/src/pygpsclient.egg-info/SOURCES.txt` & `pygpsclient-1.4.9/src/pygpsclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygpsclient-1.4.8/tests/test_static.py` & `pygpsclient-1.4.9/tests/test_static.py`

 * *Files identical despite different names*

