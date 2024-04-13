# Comparing `tmp/facecrop-thumb-1.0.4.tar.gz` & `tmp/facecrop-thumb-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facecrop-thumb-1.0.4.tar", last modified: Fri Apr 12 15:35:24 2024, max compression
+gzip compressed data, was "facecrop-thumb-1.0.5.tar", last modified: Sat Apr 13 05:30:55 2024, max compression
```

## Comparing `facecrop-thumb-1.0.4.tar` & `facecrop-thumb-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:35:24.156547 facecrop-thumb-1.0.4/
--rw-rw-rw-   0        0        0     1092 2024-04-12 11:58:00.000000 facecrop-thumb-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1204 2024-04-12 15:35:24.155608 facecrop-thumb-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2024-04-12 12:03:25.000000 facecrop-thumb-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 15:35:24.146622 facecrop-thumb-1.0.4/facecrop_thumb/
--rw-rw-rw-   0        0        0        0 2024-04-12 15:10:13.000000 facecrop-thumb-1.0.4/facecrop_thumb/__init__.py
--rw-rw-rw-   0        0        0      283 2024-04-12 10:33:36.000000 facecrop-thumb-1.0.4/facecrop_thumb/face_detection.py
--rw-rw-rw-   0        0        0      788 2024-04-12 10:33:30.000000 facecrop-thumb-1.0.4/facecrop_thumb/image_processing.py
--rw-rw-rw-   0        0        0     1042 2024-04-12 12:37:35.000000 facecrop-thumb-1.0.4/facecrop_thumb/main.py
--rw-rw-rw-   0        0        0     2461 2024-04-12 12:37:45.000000 facecrop-thumb-1.0.4/facecrop_thumb/thumbnail_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:35:24.154605 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/
--rw-rw-rw-   0        0        0     1204 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 15:35:24.000000 facecrop-thumb-1.0.4/facecrop_thumb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 15:35:24.157586 facecrop-thumb-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1481 2024-04-12 15:34:53.000000 facecrop-thumb-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/facecrop_thumb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/thumbnail_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/setup.py
```

### Comparing `facecrop-thumb-1.0.4/LICENSE` & `facecrop-thumb-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Vaibhav Shukla
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Vaibhav Shukla
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `facecrop-thumb-1.0.4/README.md` & `facecrop-thumb-1.0.5/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# FaceCropThumb
-
-FaceCropThumb is a Python package for generating thumbnails of detected faces in images. It utilizes the MTCNN (Multi-Task Cascaded Convolutional Neural Network) for accurate face detection and OpenCV for image processing.
-
-## Features
-
-- Detect faces in images using the MTCNN model
-- Crop detected faces with a configurable margin
-- Generate square thumbnails of detected faces
-- Option to resize the entire image if no face is detected or face detection is skipped
-- Command-line utility for easy usage
-
-## Installation
-
-You can install FaceCropThumb via pip:
-
-```pip install facecropthumb```
-
-## Usage
-
-```facecropthumb <image_path> [-d/--dir <output_directory>] [-m/--margin <margin_size>] [-F/--no-face] [-S/--skip-face]```
-
-- `<image_path>`: Path to the input image file.
-- `-d/--dir <output_directory>`: Directory to store the output thumbnail. Default is the current directory.
-- `-m/--margin <margin_size>`: Margin around the detected face. Default is 50 pixels.
-- `-F/--no-face`: Skip face detection and resize the whole image if no face is detected.
-- `-S/--skip-face`: Skip face detection and resize the whole image.
-
-Example:
-
-```facecropthumb input_image.jpg -d output_directory -m 30 -F```
-
-This command will generate a thumbnail of the detected face in `input_image.jpg`, with a margin of 30 pixels, and if no face is detected, it will resize the whole image to a square of 74 x Y pixels (~approx).
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+# FaceCropThumb
+
+FaceCropThumb is a Python package for generating thumbnails of detected faces in images. It utilizes the MTCNN (Multi-Task Cascaded Convolutional Neural Network) for accurate face detection and OpenCV for image processing.
+
+## Features
+
+- Detect faces in images using the MTCNN model
+- Crop detected faces with a configurable margin
+- Generate square thumbnails of detected faces
+- Option to resize the entire image if no face is detected or face detection is skipped
+- Command-line utility for easy usage
+
+## Installation
+
+You can install FaceCropThumb via pip:
+
+```pip install facecropthumb```
+
+## Usage
+
+```facecropthumb <image_path> [-d/--dir <output_directory>] [-m/--margin <margin_size>] [-F/--no-face] [-S/--skip-face]```
+
+- `<image_path>`: Path to the input image file.
+- `-d/--dir <output_directory>`: Directory to store the output thumbnail. Default is the current directory.
+- `-m/--margin <margin_size>`: Margin around the detected face. Default is 50 pixels.
+- `-F/--no-face`: Skip face detection and resize the whole image if no face is detected.
+- `-S/--skip-face`: Skip face detection and resize the whole image.
+
+Example:
+
+```facecropthumb input_image.jpg -d output_directory -m 30 -F```
+
+This command will generate a thumbnail of the detected face in `input_image.jpg`, with a margin of 30 pixels, and if no face is detected, it will resize the whole image to a square of 74 x Y pixels (~approx).
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `facecrop-thumb-1.0.4/facecrop_thumb/image_processing.py` & `facecrop-thumb-1.0.5/facecrop_thumb/image_processing.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# image_processing.py
-import cv2
-
-def crop_face_thumbnail(image, face_coords, margin=50, target_size=(74, 74)):
-    x, y, w, h = face_coords
-    x -= margin
-    y -= margin
-    w += 2 * margin
-    h += 2 * margin
-    x = max(0, x)
-    y = max(0, y)
-    w = min(w, image.shape[1])
-    h = min(h, image.shape[0])
-    aspect_ratio = w / h
-    if w > h:
-        thumbnail_height = int(target_size[1])
-        thumbnail_width = int(thumbnail_height * aspect_ratio)
-    else:
-        thumbnail_width = int(target_size[0])
-        thumbnail_height = int(thumbnail_width / aspect_ratio)
-    face_with_margin = image[y:y+h, x:x+w]
-    face_thumbnail = cv2.resize(face_with_margin, (thumbnail_width, thumbnail_height), interpolation=cv2.INTER_AREA)
-    return face_thumbnail
+# image_processing.py
+import cv2
+
+def crop_face_thumbnail(image, face_coords, margin=50, target_size=(74, 74)):
+    x, y, w, h = face_coords
+    x -= margin
+    y -= margin
+    w += 2 * margin
+    h += 2 * margin
+    x = max(0, x)
+    y = max(0, y)
+    w = min(w, image.shape[1])
+    h = min(h, image.shape[0])
+    aspect_ratio = w / h
+    if w > h:
+        thumbnail_height = int(target_size[1])
+        thumbnail_width = int(thumbnail_height * aspect_ratio)
+    else:
+        thumbnail_width = int(target_size[0])
+        thumbnail_height = int(thumbnail_width / aspect_ratio)
+    face_with_margin = image[y:y+h, x:x+w]
+    face_thumbnail = cv2.resize(face_with_margin, (thumbnail_width, thumbnail_height), interpolation=cv2.INTER_AREA)
+    return face_thumbnail
```

