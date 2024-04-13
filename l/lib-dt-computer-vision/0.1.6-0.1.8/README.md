# Comparing `tmp/lib-dt-computer-vision-0.1.6.tar.gz` & `tmp/lib-dt-computer-vision-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-computer-vision-0.1.6.tar", last modified: Sun Feb 18 05:06:26 2024, max compression
+gzip compressed data, was "lib-dt-computer-vision-0.1.8.tar", last modified: Sat Apr 13 03:41:32 2024, max compression
```

## Comparing `lib-dt-computer-vision-0.1.6.tar` & `lib-dt-computer-vision-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.453268 lib-dt-computer-vision-0.1.6/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      565 2024-02-18 05:06:26.453268 lib-dt-computer-vision-0.1.6/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-02-18 05:06:26.453268 lib-dt-computer-vision-0.1.6/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2005 2024-01-17 23:11:17.000000 lib-dt-computer-vision-0.1.6/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.445268 lib-dt-computer-vision-0.1.6/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.445268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-02-18 05:06:18.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.445268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/anti_instagram/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/anti_instagram/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3477 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/anti_instagram/anti_instagram.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       80 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    46015 2023-12-07 06:12:28.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_active.png
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    45581 2023-12-07 06:12:15.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_inactive.png
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    55277 2023-12-07 06:26:45.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/validation_gui.png
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1357 2023-12-07 05:26:32.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6163 2023-12-07 06:51:27.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       51 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2697 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9130 2023-12-07 06:14:46.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7652 2024-01-17 23:09:51.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/homography.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10183 2024-02-18 05:03:51.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/types.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1997 2023-12-11 22:35:39.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       77 2023-07-12 04:43:08.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/__init__.py
--rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     5254 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/ground_projector.py
--rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     8634 2023-12-05 03:19:19.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       70 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      884 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12570 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/line_detector.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2586 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/rendering.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4817 2023-04-23 19:53:33.000000 lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-02-18 05:06:26.449268 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      565 2024-02-18 05:06:26.000000 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1659 2024-02-18 05:06:26.000000 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-02-18 05:06:26.000000 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       64 2024-02-18 05:06:26.000000 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       19 2024-02-18 05:06:26.000000 lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.714541 lib-dt-computer-vision-0.1.8/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      565 2024-04-13 03:41:32.714541 lib-dt-computer-vision-0.1.8/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-13 03:41:32.714541 lib-dt-computer-vision-0.1.8/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2005 2024-01-18 22:04:53.000000 lib-dt-computer-vision-0.1.8/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.706540 lib-dt-computer-vision-0.1.8/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.706540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-05 13:24:21.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.706540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/anti_instagram/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/anti_instagram/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3477 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/anti_instagram/anti_instagram.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.706540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       80 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.706540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.710540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.710540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    46015 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_active.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    45581 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_inactive.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    55277 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/validation_gui.png
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1357 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/boards.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6162 2024-04-05 13:24:21.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       51 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2697 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9130 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7652 2024-01-18 22:04:53.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/homography.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10736 2024-04-05 13:24:21.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1997 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.710540 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       77 2023-07-11 19:47:10.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/__init__.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     5254 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/ground_projector.py
+-rwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)     8634 2023-12-17 16:44:42.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       70 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.714541 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      884 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12570 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/line_detector.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2586 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/rendering.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4817 2023-04-19 19:49:17.000000 lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-13 03:41:32.714541 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      565 2024-04-13 03:41:32.000000 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1659 2024-04-13 03:41:32.000000 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-13 03:41:32.000000 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       64 2024-04-13 03:41:32.000000 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       19 2024-04-13 03:41:32.000000 lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/top_level.txt
```

### Comparing `lib-dt-computer-vision-0.1.6/PKG-INFO` & `lib-dt-computer-vision-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dt-computer-vision
-Version: 0.1.6
+Version: 0.1.8
 Home-page: http://github.com/duckietown/lib-dt-computer-vision
 Author: Andrea F. Daniele
 Author-email: afdaniele@duckietown.com
 Requires-Dist: opencv-python-headless<=4.8.1.78
 Requires-Dist: numpy<=1.26.2
 Requires-Dist: requests<=2.31.0
```

### Comparing `lib-dt-computer-vision-0.1.6/setup.py` & `lib-dt-computer-vision-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/anti_instagram/anti_instagram.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/anti_instagram/anti_instagram.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_active.png` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_active.png`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_inactive.png` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/gui_inactive.png`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/assets/validation_gui.png` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/assets/validation_gui.png`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/boards.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/boards.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/chessboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         RuntimeError: If no corners were found in image, or the corners couldn't be rearranged
 
     """
     grayscale = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     corners_num = (board.columns - 1, board.rows - 1)
 
     # find corners in the image
-    ret, corners = cv2.findChessboardCorners(grayscale, corners_num, cv2.CALIB_CB_ADAPTIVE_THRESH)
+    ret, corners = cv2.findChessboardCornersSB(image, corners_num, flags=cv2.CALIB_CB_EXHAUSTIVE)
     if not ret:
         raise NoCornersFoundException(
             "No corners found in image, or the corners couldn't be "
             "rearranged. Make sure the camera is positioned correctly."
         )
 
     # refine corners' position
```

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/ransac.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/calibration/extrinsics/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/homography.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/homography.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/types.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -275,14 +275,28 @@
         sy = 1.0 / (br.y - tl.y)
         # ---
         return np.array([
             [sx, 0, -tl.x * sx],
             [0, sy, -tl.y * sy],
             [0,  0,          1]
         ])
+        
+    def homography_pixel2vector(self) -> np.ndarray:
+        """
+        Homography converting a ``[0,W] X [0,H]`` representation to ``[0, 1] X [0, 1]``
+        (from image to normalized coordinates).
+
+        Returns:
+            :py:class:`np.ndarray` : A 3-by-3 matrix implementing the coordinate transformation operation.
+        """        
+        return np.array([
+            [1/self.fx,         0, -self.cx/self.fx],
+            [0,         1/self.fy, -self.cy/self.fy],
+            [0,                 0,                1]
+        ])
 
     def homography_independent2vector(self) -> np.ndarray:
         """
         Homography converting resolution-independent coordinates ``[0, 1] X [0, 1]`` to normalized
         coordinates ``[-∞,+∞] X [-∞,+∞]``.
 
         Returns:
```

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/camera/utils.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/camera/utils.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/ground_projector.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/ground_projector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/ground_projection/rendering.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/ground_projection/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/__init__.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/line_detector.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/line_detector.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/rendering.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/rendering.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/dt_computer_vision/line_detection/types.py` & `lib-dt-computer-vision-0.1.8/src/dt_computer_vision/line_detection/types.py`

 * *Files identical despite different names*

### Comparing `lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/PKG-INFO` & `lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dt-computer-vision
-Version: 0.1.6
+Version: 0.1.8
 Home-page: http://github.com/duckietown/lib-dt-computer-vision
 Author: Andrea F. Daniele
 Author-email: afdaniele@duckietown.com
 Requires-Dist: opencv-python-headless<=4.8.1.78
 Requires-Dist: numpy<=1.26.2
 Requires-Dist: requests<=2.31.0
```

### Comparing `lib-dt-computer-vision-0.1.6/src/lib_dt_computer_vision.egg-info/SOURCES.txt` & `lib-dt-computer-vision-0.1.8/src/lib_dt_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

