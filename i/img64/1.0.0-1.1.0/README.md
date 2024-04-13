# Comparing `tmp/img64-1.0.0.tar.gz` & `tmp/img64-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img64-1.0.0.tar", last modified: Tue Dec 19 12:50:04 2023, max compression
+gzip compressed data, was "img64-1.1.0.tar", last modified: Sat Apr 13 07:37:39 2024, max compression
```

## Comparing `img64-1.0.0.tar` & `img64-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nkm        (501) staff       (20)        0 2023-12-19 12:50:04.912005 img64-1.0.0/
--rw-r--r--   0 nkm        (501) staff       (20)     1063 2023-12-15 11:22:18.000000 img64-1.0.0/LICENSE
--rw-r--r--   0 nkm        (501) staff       (20)       33 2023-12-15 11:22:18.000000 img64-1.0.0/MANIFEST.in
--rw-r--r--   0 nkm        (501) staff       (20)     2213 2023-12-19 12:50:04.911720 img64-1.0.0/PKG-INFO
--rw-r--r--   0 nkm        (501) staff       (20)     1648 2023-12-15 13:33:08.000000 img64-1.0.0/README.md
-drwxr-xr-x   0 nkm        (501) staff       (20)        0 2023-12-19 12:50:04.910857 img64-1.0.0/img64/
--rw-r--r--   0 nkm        (501) staff       (20)       58 2023-12-15 11:22:18.000000 img64-1.0.0/img64/__init__.py
--rw-r--r--   0 nkm        (501) staff       (20)      936 2023-12-19 12:45:41.000000 img64-1.0.0/img64/convert.py
-drwxr-xr-x   0 nkm        (501) staff       (20)        0 2023-12-19 12:50:04.911504 img64-1.0.0/img64.egg-info/
--rw-r--r--   0 nkm        (501) staff       (20)     2213 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/PKG-INFO
--rw-r--r--   0 nkm        (501) staff       (20)      245 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/SOURCES.txt
--rw-r--r--   0 nkm        (501) staff       (20)        1 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/dependency_links.txt
--rw-r--r--   0 nkm        (501) staff       (20)        1 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/not-zip-safe
--rw-r--r--   0 nkm        (501) staff       (20)       13 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/requires.txt
--rw-r--r--   0 nkm        (501) staff       (20)        6 2023-12-19 12:50:04.000000 img64-1.0.0/img64.egg-info/top_level.txt
--rw-r--r--   0 nkm        (501) staff       (20)       38 2023-12-19 12:50:04.912059 img64-1.0.0/setup.cfg
--rw-r--r--   0 nkm        (501) staff       (20)      857 2023-12-19 12:45:48.000000 img64-1.0.0/setup.py
+drwxr-xr-x   0 nkm        (501) staff       (20)        0 2024-04-13 07:37:39.101173 img64-1.1.0/
+-rw-r--r--   0 nkm        (501) staff       (20)     1063 2024-04-12 12:27:09.000000 img64-1.1.0/LICENSE
+-rw-r--r--   0 nkm        (501) staff       (20)       33 2024-04-12 12:27:09.000000 img64-1.1.0/MANIFEST.in
+-rw-r--r--   0 nkm        (501) staff       (20)     2200 2024-04-13 07:37:39.100919 img64-1.1.0/PKG-INFO
+-rw-r--r--   0 nkm        (501) staff       (20)     1636 2024-04-13 07:23:18.000000 img64-1.1.0/README.md
+drwxr-xr-x   0 nkm        (501) staff       (20)        0 2024-04-13 07:37:39.099527 img64-1.1.0/img64/
+-rw-r--r--   0 nkm        (501) staff       (20)      116 2024-04-13 07:17:16.000000 img64-1.1.0/img64/__init__.py
+-rw-r--r--   0 nkm        (501) staff       (20)     1131 2024-04-13 07:30:17.000000 img64-1.1.0/img64/convert.py
+drwxr-xr-x   0 nkm        (501) staff       (20)        0 2024-04-13 07:37:39.100587 img64-1.1.0/img64.egg-info/
+-rw-r--r--   0 nkm        (501) staff       (20)     2200 2024-04-13 07:37:39.000000 img64-1.1.0/img64.egg-info/PKG-INFO
+-rw-r--r--   0 nkm        (501) staff       (20)      245 2024-04-13 07:37:39.000000 img64-1.1.0/img64.egg-info/SOURCES.txt
+-rw-r--r--   0 nkm        (501) staff       (20)        1 2024-04-13 07:37:39.000000 img64-1.1.0/img64.egg-info/dependency_links.txt
+-rw-r--r--   0 nkm        (501) staff       (20)        1 2024-04-13 07:24:47.000000 img64-1.1.0/img64.egg-info/not-zip-safe
+-rw-r--r--   0 nkm        (501) staff       (20)       13 2024-04-13 07:37:39.000000 img64-1.1.0/img64.egg-info/requires.txt
+-rw-r--r--   0 nkm        (501) staff       (20)        6 2024-04-13 07:37:39.000000 img64-1.1.0/img64.egg-info/top_level.txt
+-rw-r--r--   0 nkm        (501) staff       (20)       38 2024-04-13 07:37:39.101217 img64-1.1.0/setup.cfg
+-rw-r--r--   0 nkm        (501) staff       (20)      857 2024-04-13 07:33:08.000000 img64-1.1.0/setup.py
```

### Comparing `img64-1.0.0/LICENSE` & `img64-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `img64-1.0.0/PKG-INFO` & `img64-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img64
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library is a tool for converting images to base64 encoding and vice versa.
 Home-page: https://github.com/gibiee/img64
 Download-URL: 
 Author: gibiee
 Author-email: gibiee@naver.com
 License: MIT
 Keywords: image,base64,image_base64
@@ -22,60 +22,55 @@
 ![PyPI - License](https://img.shields.io/pypi/l/img64)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/img64)
 
 <p align="center">
   <img src="https://github.com/gibiee/img64/assets/37574274/1e4ba6f4-776d-4e84-b589-09f75d64d175" width="50%" height="50%" />
 </p>
 
-This library is a tool for converting images to base64 encoding and vice versa.
-
-- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
-  - The referenced code didn't ensure data consistency, so this code improves that issue.
-  - This code enhances user convenience in handling both RGB and grayscale images.
+This library converts images to base64 encoding and vice versa.
 
 
 # Installation
 ```sh
 pip install img64
 ```
 
 
 # Quick start
 
-## Convert pil image to base64
+## Convert Image to Base64
 ```py
 from PIL import Image
+import cv2
 import img64
 
+# PIL image to Base64
 image = Image.open('sample.png')
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
-```
-
-## Convert numpy(opencv) image to base64
-```py
-import cv2
-import img64
 
+# Numpy(OpenCV) image to Base64
 image = cv2.imread('sample.png')
 image = cv2.cvtColor(image, cv2.COLOR_BGRA2RGBA)
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 ```
 
-## Convert base64 to pil image
+## Convert Base64 to Image
 ```py
 import img64
 
+# Base64 to PIL image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='pil')
 type(image) # PIL.Image.Image
-```
-
-## Convert base64 to numpy image
-```py
-import img64
 
+# Base64 to Numpy(OpenCV) image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='numpy')
 type(image) # numpy.ndarray
 ```
+
+# Information
+- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
+  - The referenced library doesn't ensure data consistency, so this library addresses that issue.
+  - This library enhances user convenience in handling both RGB and grayscale images.
```

### Comparing `img64-1.0.0/README.md` & `img64-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,60 +3,55 @@
 ![PyPI - License](https://img.shields.io/pypi/l/img64)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/img64)
 
 <p align="center">
   <img src="https://github.com/gibiee/img64/assets/37574274/1e4ba6f4-776d-4e84-b589-09f75d64d175" width="50%" height="50%" />
 </p>
 
-This library is a tool for converting images to base64 encoding and vice versa.
-
-- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
-  - The referenced code didn't ensure data consistency, so this code improves that issue.
-  - This code enhances user convenience in handling both RGB and grayscale images.
+This library converts images to base64 encoding and vice versa.
 
 
 # Installation
 ```sh
 pip install img64
 ```
 
 
 # Quick start
 
-## Convert pil image to base64
+## Convert Image to Base64
 ```py
 from PIL import Image
+import cv2
 import img64
 
+# PIL image to Base64
 image = Image.open('sample.png')
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
-```
-
-## Convert numpy(opencv) image to base64
-```py
-import cv2
-import img64
 
+# Numpy(OpenCV) image to Base64
 image = cv2.imread('sample.png')
 image = cv2.cvtColor(image, cv2.COLOR_BGRA2RGBA)
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 ```
 
-## Convert base64 to pil image
+## Convert Base64 to Image
 ```py
 import img64
 
+# Base64 to PIL image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='pil')
 type(image) # PIL.Image.Image
-```
-
-## Convert base64 to numpy image
-```py
-import img64
 
+# Base64 to Numpy(OpenCV) image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='numpy')
 type(image) # numpy.ndarray
-```
+```
+
+# Information
+- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
+  - The referenced library doesn't ensure data consistency, so this library addresses that issue.
+  - This library enhances user convenience in handling both RGB and grayscale images.
```

### Comparing `img64-1.0.0/img64/convert.py` & `img64-1.1.0/img64/convert.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import io
-import base64 as _base64
+import base64
 import numpy as np
 from PIL import Image
 from typing import Union, Literal
 
-def image_to_base64(image: Union[Image.Image, np.ndarray]) -> str :
-    if isinstance(image, np.ndarray) :
-        image = Image.fromarray(image)
-
+def image_to_bytes(img: Union[Image.Image, np.ndarray]) -> bytes :
+    if isinstance(img, np.ndarray) :
+        img = Image.fromarray(img)
+    
     buffer = io.BytesIO()
-    image.save(buffer, format="PNG")
-
-    image_bytes = buffer.getvalue()
-    image_b64 = _base64.b64encode(image_bytes)
-    image_b64_utf8 = image_b64.decode("utf-8")
-
-    return image_b64_utf8
-
-def base64_to_image(base64: str, type: Literal['pil', 'numpy']='pil') -> Union[Image.Image, np.ndarray] :
+    img.save(buffer, format="PNG")
+    img_bytes = buffer.getvalue()
+    return img_bytes
+
+def image_to_base64(img: Union[Image.Image, np.ndarray]) -> str :
+    img_bytes = image_to_bytes(img)
+    img_b64 = base64.b64encode(img_bytes)
+    img_b64_utf8 = img_b64.decode("utf-8")
+    return img_b64_utf8
+
+def base64_to_bytes(b64: str) -> bytes :
+    img_bytes = base64.b64decode(b64)
+    return img_bytes
+    
+def base64_to_image(b64: str, type: Literal['pil', 'numpy']='pil') -> Union[Image.Image, np.ndarray] :
     assert type in ['pil', 'numpy'], "Expected type 'pil' or 'numpy'"
-    img_bytes = _base64.b64decode(base64)
+    
+    img_bytes = base64_to_bytes(b64)
     buffer = io.BytesIO(img_bytes)
     img = Image.open(buffer)
     img = np.array(img) # RGB 이미지가 PIL.PngImagePlugin.PngImageFile 객체인 현상 방지
 
     if type == 'numpy' : return img
     else : return Image.fromarray(img)
```

### Comparing `img64-1.0.0/img64.egg-info/PKG-INFO` & `img64-1.1.0/img64.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img64
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library is a tool for converting images to base64 encoding and vice versa.
 Home-page: https://github.com/gibiee/img64
 Download-URL: 
 Author: gibiee
 Author-email: gibiee@naver.com
 License: MIT
 Keywords: image,base64,image_base64
@@ -22,60 +22,55 @@
 ![PyPI - License](https://img.shields.io/pypi/l/img64)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/img64)
 
 <p align="center">
   <img src="https://github.com/gibiee/img64/assets/37574274/1e4ba6f4-776d-4e84-b589-09f75d64d175" width="50%" height="50%" />
 </p>
 
-This library is a tool for converting images to base64 encoding and vice versa.
-
-- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
-  - The referenced code didn't ensure data consistency, so this code improves that issue.
-  - This code enhances user convenience in handling both RGB and grayscale images.
+This library converts images to base64 encoding and vice versa.
 
 
 # Installation
 ```sh
 pip install img64
 ```
 
 
 # Quick start
 
-## Convert pil image to base64
+## Convert Image to Base64
 ```py
 from PIL import Image
+import cv2
 import img64
 
+# PIL image to Base64
 image = Image.open('sample.png')
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
-```
-
-## Convert numpy(opencv) image to base64
-```py
-import cv2
-import img64
 
+# Numpy(OpenCV) image to Base64
 image = cv2.imread('sample.png')
 image = cv2.cvtColor(image, cv2.COLOR_BGRA2RGBA)
 base64 = img64.image_to_base64(image)
 base64[:30] # 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 ```
 
-## Convert base64 to pil image
+## Convert Base64 to Image
 ```py
 import img64
 
+# Base64 to PIL image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='pil')
 type(image) # PIL.Image.Image
-```
-
-## Convert base64 to numpy image
-```py
-import img64
 
+# Base64 to Numpy(OpenCV) image
 base64 = 'iVBORw0KGgoAAAANSUhEUgAABAAAAA...'
 image = img64.base64_to_image(base64, type='numpy')
 type(image) # numpy.ndarray
 ```
+
+# Information
+- It was implemented by referencing [ternaus/base64ToImageConverters](https://github.com/ternaus/base64ToImageConverters).
+  - The referenced library doesn't ensure data consistency, so this library addresses that issue.
+  - This library enhances user convenience in handling both RGB and grayscale images.
```

