# Comparing `tmp/celeb_detector-0.0.24.tar.gz` & `tmp/celeb_detector-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celeb_detector-0.0.24.tar", last modified: Tue Nov  9 16:05:40 2021, max compression
+gzip compressed data, was "celeb_detector-0.0.25.tar", last modified: Sat Apr 13 19:27:24 2024, max compression
```

## Comparing `celeb_detector-0.0.24.tar` & `celeb_detector-0.0.25.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 shobhitg   (502) staff       (20)        0 2021-11-09 16:05:40.388734 celeb_detector-0.0.24/
--rw-r--r--   0 shobhitg   (502) staff       (20)     7930 2021-11-09 16:05:40.387975 celeb_detector-0.0.24/PKG-INFO
--rw-r--r--   0 shobhitg   (502) staff       (20)     6646 2021-11-09 15:28:41.000000 celeb_detector-0.0.24/README.md
-drwxr-xr-x   0 shobhitg   (502) staff       (20)        0 2021-11-09 16:05:40.381352 celeb_detector-0.0.24/celeb_detector/
--rw-r--r--   0 shobhitg   (502) staff       (20)      128 2021-04-23 16:19:43.000000 celeb_detector-0.0.24/celeb_detector/__init__.py
--rw-r--r--   0 shobhitg   (502) staff       (20)     2741 2021-11-09 16:04:59.000000 celeb_detector-0.0.24/celeb_detector/celeb_recognition.py
--rw-r--r--   0 shobhitg   (502) staff       (20)     3763 2021-04-23 16:19:43.000000 celeb_detector-0.0.24/celeb_detector/celeb_utils.py
--rw-r--r--   0 shobhitg   (502) staff       (20)     1560 2021-04-23 16:19:43.000000 celeb_detector-0.0.24/celeb_detector/create_celeb_model.py
--rw-r--r--   0 shobhitg   (502) staff       (20)     2334 2021-04-23 16:19:43.000000 celeb_detector-0.0.24/celeb_detector/create_model_utils.py
--rw-r--r--   0 shobhitg   (502) staff       (20)      927 2021-04-23 16:19:43.000000 celeb_detector-0.0.24/celeb_detector/download_gdrive.py
-drwxr-xr-x   0 shobhitg   (502) staff       (20)        0 2021-11-09 16:05:40.386669 celeb_detector-0.0.24/celeb_detector.egg-info/
--rw-r--r--   0 shobhitg   (502) staff       (20)     7930 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/PKG-INFO
--rw-r--r--   0 shobhitg   (502) staff       (20)      449 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/SOURCES.txt
--rw-r--r--   0 shobhitg   (502) staff       (20)        1 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/dependency_links.txt
--rw-r--r--   0 shobhitg   (502) staff       (20)       74 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/entry_points.txt
--rw-r--r--   0 shobhitg   (502) staff       (20)       79 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/requires.txt
--rw-r--r--   0 shobhitg   (502) staff       (20)       15 2021-11-09 16:05:40.000000 celeb_detector-0.0.24/celeb_detector.egg-info/top_level.txt
--rw-r--r--   0 shobhitg   (502) staff       (20)       38 2021-11-09 16:05:40.389028 celeb_detector-0.0.24/setup.cfg
--rw-r--r--   0 shobhitg   (502) staff       (20)     1158 2021-11-09 16:05:10.000000 celeb_detector-0.0.24/setup.py
+drwxr-xr-x   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)        0 2024-04-13 19:27:24.725800 celeb_detector-0.0.25/
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     1070 2024-04-13 18:38:24.000000 celeb_detector-0.0.25/LICENSE
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     7281 2024-04-13 19:27:24.722471 celeb_detector-0.0.25/PKG-INFO
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     6646 2024-04-13 15:43:29.000000 celeb_detector-0.0.25/README.md
+drwxr-xr-x   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)        0 2024-04-13 19:27:24.714792 celeb_detector-0.0.25/celeb_detector/
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)        0 2024-04-13 19:16:03.000000 celeb_detector-0.0.25/celeb_detector/__init__.py
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     3861 2024-04-13 19:10:33.000000 celeb_detector-0.0.25/celeb_detector/celeb_prediction_main.py
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     1365 2024-04-13 19:03:49.000000 celeb_detector-0.0.25/celeb_detector/celeb_recognition.py
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     1792 2024-04-13 18:33:32.000000 celeb_detector-0.0.25/celeb_detector/create_celeb_model.py
+drwxr-xr-x   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)        0 2024-04-13 19:27:24.721499 celeb_detector-0.0.25/celeb_detector.egg-info/
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     7281 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/PKG-INFO
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)      396 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)        1 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)       73 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/entry_points.txt
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)      100 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/requires.txt
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)       15 2024-04-13 19:27:24.000000 celeb_detector-0.0.25/celeb_detector.egg-info/top_level.txt
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)       38 2024-04-13 19:27:24.725913 celeb_detector-0.0.25/setup.cfg
+-rw-r--r--   0 shobhit2.gupta (309353949) IN\Domain Users (826136866)     1263 2024-04-13 19:18:34.000000 celeb_detector-0.0.25/setup.py
```

### Comparing `celeb_detector-0.0.24/PKG-INFO` & `celeb_detector-0.0.25/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,126 +1,136 @@
 Metadata-Version: 2.1
 Name: celeb_detector
-Version: 0.0.24
+Version: 0.0.25
 Summary: Model to recognize celebrities using a face matching algorithm
 Home-page: https://github.com/shobhit9618/celeb_recognition
 Author: Shobhit Gupta
 Author-email: shobhit9618@gmail.com
-License: UNKNOWN
-Description: # Celebrity Recognition [![PyPI version](https://badge.fury.io/py/celeb-detector.svg)](https://badge.fury.io/py/celeb-detector) [![Documentation Status](https://readthedocs.org/projects/celeb-recognition/badge/?version=main)](https://celeb-recognition.readthedocs.io/en/main/) [![Anaconda-Server Badge](https://anaconda.org/shobhit9618/celeb-detector/badges/installer/env.svg)](https://anaconda.org/shobhit9618/celeb-detector)
-        Model to recognize celebrities using a face matching algorithm.
-        
-        Refer [this](https://celeb-recognition.readthedocs.io/en/main/) for detailed documentation.
-        
-        You can also read my article on medium [here](https://medium.com/@shobhitgupta/celebrity-recognition-using-vggface-and-annoy-363c5df31f1e). 
-        
-        ## Basic working of the algorithm includes the following:
-        - Face detection is done using MTCNN face detection model.
-        
-        - Face encodings are created using [VGGFace](https://github.com/rcmalli/keras-vggface) model in keras.
-        
-        - Face matching is done using [annoy](https://github.com/spotify/annoy) library (spotify).
-        
-        ## Installing dependencies
-        - Run `pip install -r requirements.txt` to install all the dependencies (preferably in a virtual environment).
-        
-        ## PyPI package
-        ### Installation
-        - To ensure you have all the required additional packages, run `pip install -r requirements.txt` first.
-        - To install pip package, run:
-            ```bash
-            # pip release version
-            pip install celeb-detector
-            # also install additional dependencies with this (if not installed via requirements.txt file)
-            pip install annoy keras-vggface keras-applications
-            # Directly from repo
-            pip install git+https://github.com/shobhit9618/celeb_recognition.git
-            ```
-        - If you are using conda on linux or ubuntu, you can use the following commands to create and use a new environment called celeb-detector:
-            ```bash
-            conda env create shobhit9618/celeb-detector
-            conda activate celeb-detector
-            ```
-            This will install all the required dependencies. To ensure you are using the latest version of the package, also run (inside the environment):
-            ```bash
-            pip install --upgrade celeb-detector
-            ```
-        
-        ### Using pip pakcage
-        - For using my model for predictions, use the following lines of code after installation:
-            ```python
-            import celeb_detector # on running for the first time, this will download vggface model
-            img_path = 'sample_image.jpg' # this supports both local path and web url like https://sample/sample_image_url.jpg
-            celeb_detector.celeb_recognition(img_path) # on running for the first time, 2 files (celeb_mapping.json and celeb_index_60.ann) will downloaded to your home directory
-            ```
-            This returns a list of dictionaries, each dictionary contains bbox coordinates, celeb name and confidence for each face detected in the image (celeb name will be unknown if no matching face detected).
-        
-        - For using your own custom model, also provide path to json and ann files as shown below:
-            ```python
-            import celeb_detector
-            img_path = 'sample_image.jpg'
-            ann_path = 'sample_index.ann'
-            celeb_map = 'sample_mapping.json'
-            celeb_detector.celeb_recognition(img_path, ann_path, celeb_map)
-            ```
-        
-        - For creating your own model (refer [this](#create-your-own-celeb-model) for more details on usage) and run as follows:
-            ```python
-            import celeb_detector
-            folder_path = 'celeb_images'
-            celeb_detector.create_celeb_model(folder_path)
-            ```
-        
-        ## Create your own celeb model
-        - Create a dataset of celebs in the following directory structure:
-            ```bash
-            celeb_images/
-                celeb-a/
-                    celeb-a_1.jpg
-                    celeb-a_2.jpg
-                    ...
-                celeb-b/
-                    celeb-b_1.jpg
-                    celeb-b_1.jpg
-                    ...
-                ...
-            ```
-        - Each folder name will be considered as the corresponding celeb name for the model (WARNING: Do not provide any special characters or spaces in the names).
-        - Make sure each image has only 1 face (of the desired celebrity), if there are multiple faces, only the first detected face will be considered.
-        - Provide path to the dataset folder (for example, `celeb_images` folder) in the [create_celeb_model.py](create_celeb_model.py) file.
-        - Run [create_celeb_model.py](create_celeb_model.py) file.
-        - Upon successful completion of the code, we get `celeb_mapping.json` (for storing indexes vs celeb names), `celeb_index.ann` (ann file for searching encodings) and `celeb_name_encoding.pkl` files (for storing encodings vs indexes for each celeb).
-        (WARNING: You need to provide paths for storing each of these files, default is to store in the current directory)
-        
-        ## Model predictions in jupyter
-        - Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.ipynb](celeb_recognition.ipynb) file. If you want to try my model, ignore this step.
-        - Run all the cells in the [celeb_recognition.ipynb](celeb_recognition.ipynb) file, the final cell will provide widgets for uploading images and making predictions
-        (this will also download the necessary model files).
-        - NOTE: [celeb_recognition.ipynb](celeb_recognition.ipynb) is a standalone file and does not require any other files from the repo for running.
-        
-        ## Model predictions in python
-        - Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.py](celeb_recognition.py) and [celeb_utils.py](celeb_utils/celeb_utils.py) files. If you want to try my model, ignore this step.
-        - Run [celeb_recognition.py](celeb_recognition.py) file, provide path to image in the file.
-        - Output includes a list of the identified faces, bounding boxes and the predicted celeb name (unknown if not found).
-        - It also displays the output with bounding boxes.
-        
-        ## Sample image output
-        ![Image](https://drive.google.com/uc?export=view&id=1W4P0PPLjr0BHDkj2CzLgFGpOYn4MF1Ck)
-        
-        ## Binder
-        You can run a binder application by clicking the following link:
-        
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main)
-        
-        You can also launch a voila binder application (which only has widgets for image upload and celeb prediction) by clicking [here](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main?urlpath=%2Fvoila%2Frender%2Fceleb_recognition.ipynb).
-        
-        ## Google Colab
-        To open and run [celeb_recognition.ipynb](celeb_recognition.ipynb) file in google colab, click the following link:
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shobhit9618/celeb_recognition/blob/main/celeb_recognition.ipynb)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: annoy
+Requires-Dist: face_recognition
+Requires-Dist: imutils
+Requires-Dist: opencv-python
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: pillow
+Requires-Dist: torch
+Requires-Dist: onnx2torch
+Requires-Dist: requests
+
+# Celebrity Recognition [![PyPI version](https://badge.fury.io/py/celeb-detector.svg)](https://badge.fury.io/py/celeb-detector) [![Documentation Status](https://readthedocs.org/projects/celeb-recognition/badge/?version=main)](https://celeb-recognition.readthedocs.io/en/main/) [![Anaconda-Server Badge](https://anaconda.org/shobhit9618/celeb-detector/badges/installer/env.svg)](https://anaconda.org/shobhit9618/celeb-detector)
+Model to recognize celebrities using a face matching algorithm.
+
+Refer [this](https://celeb-recognition.readthedocs.io/en/main/) for detailed documentation.
+
+You can also read my article on medium [here](https://medium.com/@shobhitgupta/celebrity-recognition-using-vggface-and-annoy-363c5df31f1e). 
+
+## Basic working of the algorithm includes the following:
+- Face detection is done using MTCNN face detection model.
+
+- Face encodings are created using [VGGFace](https://github.com/rcmalli/keras-vggface) model in keras.
+
+- Face matching is done using [annoy](https://github.com/spotify/annoy) library (spotify).
+
+## Installing dependencies
+- Run `pip install -r requirements.txt` to install all the dependencies (preferably in a virtual environment).
+
+## PyPI package
+### Installation
+- To ensure you have all the required additional packages, run `pip install -r requirements.txt` first.
+- To install pip package, run:
+    ```bash
+    # pip release version
+    pip install celeb-detector
+    # also install additional dependencies with this (if not installed via requirements.txt file)
+    pip install annoy keras-vggface keras-applications
+    # Directly from repo
+    pip install git+https://github.com/shobhit9618/celeb_recognition.git
+    ```
+- If you are using conda on linux or ubuntu, you can use the following commands to create and use a new environment called celeb-detector:
+    ```bash
+    conda env create shobhit9618/celeb-detector
+    conda activate celeb-detector
+    ```
+    This will install all the required dependencies. To ensure you are using the latest version of the package, also run (inside the environment):
+    ```bash
+    pip install --upgrade celeb-detector
+    ```
+
+### Using pip pakcage
+- For using my model for predictions, use the following lines of code after installation:
+    ```python
+    import celeb_detector # on running for the first time, this will download vggface model
+    img_path = 'sample_image.jpg' # this supports both local path and web url like https://sample/sample_image_url.jpg
+    celeb_detector.celeb_recognition(img_path) # on running for the first time, 2 files (celeb_mapping.json and celeb_index_60.ann) will downloaded to your home directory
+    ```
+    This returns a list of dictionaries, each dictionary contains bbox coordinates, celeb name and confidence for each face detected in the image (celeb name will be unknown if no matching face detected).
+
+- For using your own custom model, also provide path to json and ann files as shown below:
+    ```python
+    import celeb_detector
+    img_path = 'sample_image.jpg'
+    ann_path = 'sample_index.ann'
+    celeb_map = 'sample_mapping.json'
+    celeb_detector.celeb_recognition(img_path, ann_path, celeb_map)
+    ```
+
+- For creating your own model (refer [this](#create-your-own-celeb-model) for more details on usage) and run as follows:
+    ```python
+    import celeb_detector
+    folder_path = 'celeb_images'
+    celeb_detector.create_celeb_model(folder_path)
+    ```
+
+## Create your own celeb model
+- Create a dataset of celebs in the following directory structure:
+    ```bash
+    celeb_images/
+        celeb-a/
+            celeb-a_1.jpg
+            celeb-a_2.jpg
+            ...
+        celeb-b/
+            celeb-b_1.jpg
+            celeb-b_1.jpg
+            ...
+        ...
+    ```
+- Each folder name will be considered as the corresponding celeb name for the model (WARNING: Do not provide any special characters or spaces in the names).
+- Make sure each image has only 1 face (of the desired celebrity), if there are multiple faces, only the first detected face will be considered.
+- Provide path to the dataset folder (for example, `celeb_images` folder) in the [create_celeb_model.py](create_celeb_model.py) file.
+- Run [create_celeb_model.py](create_celeb_model.py) file.
+- Upon successful completion of the code, we get `celeb_mapping.json` (for storing indexes vs celeb names), `celeb_index.ann` (ann file for searching encodings) and `celeb_name_encoding.pkl` files (for storing encodings vs indexes for each celeb).
+(WARNING: You need to provide paths for storing each of these files, default is to store in the current directory)
+
+## Model predictions in jupyter
+- Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.ipynb](celeb_recognition.ipynb) file. If you want to try my model, ignore this step.
+- Run all the cells in the [celeb_recognition.ipynb](celeb_recognition.ipynb) file, the final cell will provide widgets for uploading images and making predictions
+(this will also download the necessary model files).
+- NOTE: [celeb_recognition.ipynb](celeb_recognition.ipynb) is a standalone file and does not require any other files from the repo for running.
+
+## Model predictions in python
+- Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.py](celeb_recognition.py) and [celeb_utils.py](celeb_utils/celeb_utils.py) files. If you want to try my model, ignore this step.
+- Run [celeb_recognition.py](celeb_recognition.py) file, provide path to image in the file.
+- Output includes a list of the identified faces, bounding boxes and the predicted celeb name (unknown if not found).
+- It also displays the output with bounding boxes.
+
+## Sample image output
+![Image](https://drive.google.com/uc?export=view&id=1W4P0PPLjr0BHDkj2CzLgFGpOYn4MF1Ck)
+
+## Binder
+You can run a binder application by clicking the following link:
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main)
+
+You can also launch a voila binder application (which only has widgets for image upload and celeb prediction) by clicking [here](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main?urlpath=%2Fvoila%2Frender%2Fceleb_recognition.ipynb).
+
+## Google Colab
+To open and run [celeb_recognition.ipynb](celeb_recognition.ipynb) file in google colab, click the following link:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shobhit9618/celeb_recognition/blob/main/celeb_recognition.ipynb)
```

### Comparing `celeb_detector-0.0.24/README.md` & `celeb_detector-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `celeb_detector-0.0.24/celeb_detector/celeb_utils.py` & `celeb_detector-0.0.25/celeb_detector/celeb_prediction_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,109 @@
-import os
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3' 
-import tensorflow as tf
-import matplotlib.pyplot as plt
+import pathlib
+import torch
 import json
 import math
 from annoy import AnnoyIndex
-from mtcnn.mtcnn import MTCNN
-from keras_vggface.vggface import VGGFace
-from keras_vggface.utils import preprocess_input
+import face_recognition
 from PIL import Image
-from numpy import asarray
 import numpy as np
 import cv2
-# import ipywidgets as widgets
-# from IPython.display import display
-import io
-import matplotlib.pyplot as plt
 import imutils
 
-face_detector = MTCNN()
-encoder_model = VGGFace(model='resnet50', include_top=False, input_shape=(224, 224, 3), pooling='avg')
-# ann_index = AnnoyIndex(2048, 'angular')
-# _ = ann_index.load("celeb_index_60.ann")
-
-def celeb_mapping(celeb_mapping_path):
-	with open(celeb_mapping_path) as json_file:
-		celeb_mapping_1_temp = json.load(json_file)
-	celeb_mapping_1 = {}
-	for key, value_list in celeb_mapping_1_temp.items():
-		for each_id in value_list:
-			celeb_mapping_1[each_id] = str(key)
-	return celeb_mapping_1
-
-def get_celeb_name_from_id(result_list, celeb_mapping_path, dist_threshold=0.9):
-	id_list = result_list[0]
-	dist_list = result_list[1]
-	celeb_mapping_dict = celeb_mapping(celeb_mapping_path)
-	counts = dict()
-	for each_id, each_dist in zip(id_list, dist_list):
-		if each_dist < dist_threshold:
-			output = celeb_mapping_dict.get(each_id)
-			counts[output] = counts.get(output, 0) + 1
-	return counts
-
-def face_distance_to_conf(face_distance, face_match_threshold=0.34):
-	if face_distance > face_match_threshold:
-		range = (1.0 - face_match_threshold)
-		linear_val = (1.0 - face_distance) / (range * 2.0)
-		return linear_val
-	else:
-		range = face_match_threshold
-		linear_val = 1.0 - (face_distance / (range * 2.0))
-		return linear_val + ((1.0 - linear_val) * math.pow((linear_val - 0.5) * 2, 0.2))
-
-def get_encoding_new(img):
-	results = face_detector.detect_faces(img)
-	if len(results)>0:
-		encodings = []
-		bbox = []
-		for result in results:
-			x1, y1, width, height = result['box']
-			if x1 <0:
-				x1 = 0
-			if y1 <0:
-				y1 = 0
-			x2, y2 = x1 + width, y1 + height
-			face = img[y1:y2, x1:x2]
-			image = Image.fromarray(face)
-			image = image.resize((224,224))
-			face_array = asarray(image)
-
-			samples = asarray(face_array, 'float32')
-			samples = preprocess_input(samples, version=2)
-			samples = np.expand_dims(samples, axis=0)
-			encoding = encoder_model.predict(samples)
-			encodings.append(encoding)
-			bbox.append((x1, y1, width, height))
-		return encodings, bbox
-	else:
-		return None, None
-
-def get_celeb_prediction(img, ann_filepath, celeb_mapping_path):
-	ann_index = AnnoyIndex(2048, 'angular')
-	_ = ann_index.load(ann_filepath)
-	encs, bbox = get_encoding_new(img)
-	data = []
-	if encs is not None:
+class CelebRecognition:
+	def __init__(self):
+		file_path = pathlib.Path(__file__).parent.absolute()
+		self.celeb_mapping_filepath = f"{file_path}/models/celeb_mapping_117.json"
+		celeb_index_annpath = f"{file_path}/models/celeb_index_117.ann"
+		vggface_modelpath = f"{file_path}/models/vggface_resnet50.pt"
+
+		self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+		if torch.backends.mps.is_available():
+			self.device = torch.device('mps')
+
+		self.encoder_model = torch.load(vggface_modelpath).to(self.device).eval()
+		self.ann_index = AnnoyIndex(2048, 'angular')
+		_ = self.ann_index.load(celeb_index_annpath)
+
+	def get_celeb_mapping(self):
+		with open(self.celeb_mapping_filepath) as json_file:
+			celeb_mapping_temp = json.load(json_file)
+		celeb_mapping = {}
+		for key, value_list in celeb_mapping_temp.items():
+			for each_id in value_list:
+				celeb_mapping[each_id] = str(key)
+		return celeb_mapping
+
+	def get_celeb_name_from_id(self, result_list, dist_threshold=0.9):
+		id_list = result_list[0]
+		dist_list = result_list[1]
+		celeb_mapping_dict = self.get_celeb_mapping()
+		counts = dict()
+		for each_id, each_dist in zip(id_list, dist_list):
+			if each_dist < dist_threshold:
+				output = celeb_mapping_dict.get(each_id)
+				counts[output] = counts.get(output, 0) + 1
+		return counts
+
+	def face_distance_to_conf(self, face_distance, face_match_threshold=0.34):
+		if face_distance > face_match_threshold:
+			range = (1.0 - face_match_threshold)
+			linear_val = (1.0 - face_distance) / (range * 2.0)
+			return linear_val
+		else:
+			range = face_match_threshold
+			linear_val = 1.0 - (face_distance / (range * 2.0))
+			return linear_val + ((1.0 - linear_val) * math.pow((linear_val - 0.5) * 2, 0.2))
+
+	def get_encoding(self, img):
+		results = face_recognition.face_locations(img)
+		if len(results)>0:
+			encodings = []
+			bbox = []
+			for result in results:
+				y1, x2, y2, x1 = result
+				if x1 <0:
+					x1 = 0
+				if y1 <0:
+					y1 = 0
+				face = img[y1:y2, x1:x2]
+				image = Image.fromarray(face)
+				image = image.resize((224,224))
+				face_array = np.asarray(image)
+
+				samples = np.asarray(face_array, 'float32')
+				samples = np.expand_dims(samples, axis=0)
+				encoding = self.encoder_model(torch.Tensor(samples).to(self.device))
+				encodings.append(encoding)
+				bbox.append((x1, y1, x2-x1, y2-y1))
+			return encodings, bbox
+		else:
+			return None, None
+
+	def get_celeb_prediction(self, img):
+		img = imutils.resize(img, height=1080)
+		encs, bbox = self.get_encoding(img)
+		data = []
 		for index, enc in enumerate(encs):
 			cv2.rectangle(img, bbox[index], (255,0,0), 2)
 			temp_data = {}
-			temp_data["bbox"] = bbox[index]
-			results = ann_index.get_nns_by_vector(enc[0], 10, search_k=-1, include_distances=True)
+			temp_data["face_bbox"] = bbox[index]
+			results = self.ann_index.get_nns_by_vector(enc[0], 10, search_k=-1, include_distances=True)
 			dist_threshold = 0.9
-			celeb_count_dict = get_celeb_name_from_id(results, celeb_mapping_path, dist_threshold)
+			celeb_count_dict = self.get_celeb_name_from_id(results, dist_threshold)
 			distance = results[1][0]
 			if len(celeb_count_dict)!=0 and max(celeb_count_dict.values()) > 3:
 				celeb_name = max(celeb_count_dict, key=celeb_count_dict.get)
 				cv2.putText(img, celeb_name.upper(), (bbox[index][0]-5, bbox[index][1] - 5), cv2.FONT_HERSHEY_DUPLEX, 1, (0,0,255), 1)
 				temp_data["celeb_name"] = celeb_name
-				temp_data["confidence"] = face_distance_to_conf(distance)
+				temp_data["confidence"] = round(self.face_distance_to_conf(distance),2)
 			else:
 				temp_data["celeb_name"] = "unknown"
 				temp_data["confidence"] = 0.0
 			data.append(temp_data)
-		img = imutils.resize(img, width=400)
-		# display(img)
 		return data, img
-
-	else:
-		return None, None
+	
+if __name__=="__main__":
+	det = CelebRecognition()
+	img = cv2.imread("/Users/shobhit2.gupta/Downloads/test_images/bolly3.jpg")
+	output = det.get_celeb_prediction(img)
+	print(output[0])
```

### Comparing `celeb_detector-0.0.24/celeb_detector.egg-info/PKG-INFO` & `celeb_detector-0.0.25/celeb_detector.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,136 @@
 Metadata-Version: 2.1
 Name: celeb-detector
-Version: 0.0.24
+Version: 0.0.25
 Summary: Model to recognize celebrities using a face matching algorithm
 Home-page: https://github.com/shobhit9618/celeb_recognition
 Author: Shobhit Gupta
 Author-email: shobhit9618@gmail.com
-License: UNKNOWN
-Description: # Celebrity Recognition [![PyPI version](https://badge.fury.io/py/celeb-detector.svg)](https://badge.fury.io/py/celeb-detector) [![Documentation Status](https://readthedocs.org/projects/celeb-recognition/badge/?version=main)](https://celeb-recognition.readthedocs.io/en/main/) [![Anaconda-Server Badge](https://anaconda.org/shobhit9618/celeb-detector/badges/installer/env.svg)](https://anaconda.org/shobhit9618/celeb-detector)
-        Model to recognize celebrities using a face matching algorithm.
-        
-        Refer [this](https://celeb-recognition.readthedocs.io/en/main/) for detailed documentation.
-        
-        You can also read my article on medium [here](https://medium.com/@shobhitgupta/celebrity-recognition-using-vggface-and-annoy-363c5df31f1e). 
-        
-        ## Basic working of the algorithm includes the following:
-        - Face detection is done using MTCNN face detection model.
-        
-        - Face encodings are created using [VGGFace](https://github.com/rcmalli/keras-vggface) model in keras.
-        
-        - Face matching is done using [annoy](https://github.com/spotify/annoy) library (spotify).
-        
-        ## Installing dependencies
-        - Run `pip install -r requirements.txt` to install all the dependencies (preferably in a virtual environment).
-        
-        ## PyPI package
-        ### Installation
-        - To ensure you have all the required additional packages, run `pip install -r requirements.txt` first.
-        - To install pip package, run:
-            ```bash
-            # pip release version
-            pip install celeb-detector
-            # also install additional dependencies with this (if not installed via requirements.txt file)
-            pip install annoy keras-vggface keras-applications
-            # Directly from repo
-            pip install git+https://github.com/shobhit9618/celeb_recognition.git
-            ```
-        - If you are using conda on linux or ubuntu, you can use the following commands to create and use a new environment called celeb-detector:
-            ```bash
-            conda env create shobhit9618/celeb-detector
-            conda activate celeb-detector
-            ```
-            This will install all the required dependencies. To ensure you are using the latest version of the package, also run (inside the environment):
-            ```bash
-            pip install --upgrade celeb-detector
-            ```
-        
-        ### Using pip pakcage
-        - For using my model for predictions, use the following lines of code after installation:
-            ```python
-            import celeb_detector # on running for the first time, this will download vggface model
-            img_path = 'sample_image.jpg' # this supports both local path and web url like https://sample/sample_image_url.jpg
-            celeb_detector.celeb_recognition(img_path) # on running for the first time, 2 files (celeb_mapping.json and celeb_index_60.ann) will downloaded to your home directory
-            ```
-            This returns a list of dictionaries, each dictionary contains bbox coordinates, celeb name and confidence for each face detected in the image (celeb name will be unknown if no matching face detected).
-        
-        - For using your own custom model, also provide path to json and ann files as shown below:
-            ```python
-            import celeb_detector
-            img_path = 'sample_image.jpg'
-            ann_path = 'sample_index.ann'
-            celeb_map = 'sample_mapping.json'
-            celeb_detector.celeb_recognition(img_path, ann_path, celeb_map)
-            ```
-        
-        - For creating your own model (refer [this](#create-your-own-celeb-model) for more details on usage) and run as follows:
-            ```python
-            import celeb_detector
-            folder_path = 'celeb_images'
-            celeb_detector.create_celeb_model(folder_path)
-            ```
-        
-        ## Create your own celeb model
-        - Create a dataset of celebs in the following directory structure:
-            ```bash
-            celeb_images/
-                celeb-a/
-                    celeb-a_1.jpg
-                    celeb-a_2.jpg
-                    ...
-                celeb-b/
-                    celeb-b_1.jpg
-                    celeb-b_1.jpg
-                    ...
-                ...
-            ```
-        - Each folder name will be considered as the corresponding celeb name for the model (WARNING: Do not provide any special characters or spaces in the names).
-        - Make sure each image has only 1 face (of the desired celebrity), if there are multiple faces, only the first detected face will be considered.
-        - Provide path to the dataset folder (for example, `celeb_images` folder) in the [create_celeb_model.py](create_celeb_model.py) file.
-        - Run [create_celeb_model.py](create_celeb_model.py) file.
-        - Upon successful completion of the code, we get `celeb_mapping.json` (for storing indexes vs celeb names), `celeb_index.ann` (ann file for searching encodings) and `celeb_name_encoding.pkl` files (for storing encodings vs indexes for each celeb).
-        (WARNING: You need to provide paths for storing each of these files, default is to store in the current directory)
-        
-        ## Model predictions in jupyter
-        - Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.ipynb](celeb_recognition.ipynb) file. If you want to try my model, ignore this step.
-        - Run all the cells in the [celeb_recognition.ipynb](celeb_recognition.ipynb) file, the final cell will provide widgets for uploading images and making predictions
-        (this will also download the necessary model files).
-        - NOTE: [celeb_recognition.ipynb](celeb_recognition.ipynb) is a standalone file and does not require any other files from the repo for running.
-        
-        ## Model predictions in python
-        - Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.py](celeb_recognition.py) and [celeb_utils.py](celeb_utils/celeb_utils.py) files. If you want to try my model, ignore this step.
-        - Run [celeb_recognition.py](celeb_recognition.py) file, provide path to image in the file.
-        - Output includes a list of the identified faces, bounding boxes and the predicted celeb name (unknown if not found).
-        - It also displays the output with bounding boxes.
-        
-        ## Sample image output
-        ![Image](https://drive.google.com/uc?export=view&id=1W4P0PPLjr0BHDkj2CzLgFGpOYn4MF1Ck)
-        
-        ## Binder
-        You can run a binder application by clicking the following link:
-        
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main)
-        
-        You can also launch a voila binder application (which only has widgets for image upload and celeb prediction) by clicking [here](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main?urlpath=%2Fvoila%2Frender%2Fceleb_recognition.ipynb).
-        
-        ## Google Colab
-        To open and run [celeb_recognition.ipynb](celeb_recognition.ipynb) file in google colab, click the following link:
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shobhit9618/celeb_recognition/blob/main/celeb_recognition.ipynb)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: annoy
+Requires-Dist: face_recognition
+Requires-Dist: imutils
+Requires-Dist: opencv-python
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: pillow
+Requires-Dist: torch
+Requires-Dist: onnx2torch
+Requires-Dist: requests
+
+# Celebrity Recognition [![PyPI version](https://badge.fury.io/py/celeb-detector.svg)](https://badge.fury.io/py/celeb-detector) [![Documentation Status](https://readthedocs.org/projects/celeb-recognition/badge/?version=main)](https://celeb-recognition.readthedocs.io/en/main/) [![Anaconda-Server Badge](https://anaconda.org/shobhit9618/celeb-detector/badges/installer/env.svg)](https://anaconda.org/shobhit9618/celeb-detector)
+Model to recognize celebrities using a face matching algorithm.
+
+Refer [this](https://celeb-recognition.readthedocs.io/en/main/) for detailed documentation.
+
+You can also read my article on medium [here](https://medium.com/@shobhitgupta/celebrity-recognition-using-vggface-and-annoy-363c5df31f1e). 
+
+## Basic working of the algorithm includes the following:
+- Face detection is done using MTCNN face detection model.
+
+- Face encodings are created using [VGGFace](https://github.com/rcmalli/keras-vggface) model in keras.
+
+- Face matching is done using [annoy](https://github.com/spotify/annoy) library (spotify).
+
+## Installing dependencies
+- Run `pip install -r requirements.txt` to install all the dependencies (preferably in a virtual environment).
+
+## PyPI package
+### Installation
+- To ensure you have all the required additional packages, run `pip install -r requirements.txt` first.
+- To install pip package, run:
+    ```bash
+    # pip release version
+    pip install celeb-detector
+    # also install additional dependencies with this (if not installed via requirements.txt file)
+    pip install annoy keras-vggface keras-applications
+    # Directly from repo
+    pip install git+https://github.com/shobhit9618/celeb_recognition.git
+    ```
+- If you are using conda on linux or ubuntu, you can use the following commands to create and use a new environment called celeb-detector:
+    ```bash
+    conda env create shobhit9618/celeb-detector
+    conda activate celeb-detector
+    ```
+    This will install all the required dependencies. To ensure you are using the latest version of the package, also run (inside the environment):
+    ```bash
+    pip install --upgrade celeb-detector
+    ```
+
+### Using pip pakcage
+- For using my model for predictions, use the following lines of code after installation:
+    ```python
+    import celeb_detector # on running for the first time, this will download vggface model
+    img_path = 'sample_image.jpg' # this supports both local path and web url like https://sample/sample_image_url.jpg
+    celeb_detector.celeb_recognition(img_path) # on running for the first time, 2 files (celeb_mapping.json and celeb_index_60.ann) will downloaded to your home directory
+    ```
+    This returns a list of dictionaries, each dictionary contains bbox coordinates, celeb name and confidence for each face detected in the image (celeb name will be unknown if no matching face detected).
+
+- For using your own custom model, also provide path to json and ann files as shown below:
+    ```python
+    import celeb_detector
+    img_path = 'sample_image.jpg'
+    ann_path = 'sample_index.ann'
+    celeb_map = 'sample_mapping.json'
+    celeb_detector.celeb_recognition(img_path, ann_path, celeb_map)
+    ```
+
+- For creating your own model (refer [this](#create-your-own-celeb-model) for more details on usage) and run as follows:
+    ```python
+    import celeb_detector
+    folder_path = 'celeb_images'
+    celeb_detector.create_celeb_model(folder_path)
+    ```
+
+## Create your own celeb model
+- Create a dataset of celebs in the following directory structure:
+    ```bash
+    celeb_images/
+        celeb-a/
+            celeb-a_1.jpg
+            celeb-a_2.jpg
+            ...
+        celeb-b/
+            celeb-b_1.jpg
+            celeb-b_1.jpg
+            ...
+        ...
+    ```
+- Each folder name will be considered as the corresponding celeb name for the model (WARNING: Do not provide any special characters or spaces in the names).
+- Make sure each image has only 1 face (of the desired celebrity), if there are multiple faces, only the first detected face will be considered.
+- Provide path to the dataset folder (for example, `celeb_images` folder) in the [create_celeb_model.py](create_celeb_model.py) file.
+- Run [create_celeb_model.py](create_celeb_model.py) file.
+- Upon successful completion of the code, we get `celeb_mapping.json` (for storing indexes vs celeb names), `celeb_index.ann` (ann file for searching encodings) and `celeb_name_encoding.pkl` files (for storing encodings vs indexes for each celeb).
+(WARNING: You need to provide paths for storing each of these files, default is to store in the current directory)
+
+## Model predictions in jupyter
+- Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.ipynb](celeb_recognition.ipynb) file. If you want to try my model, ignore this step.
+- Run all the cells in the [celeb_recognition.ipynb](celeb_recognition.ipynb) file, the final cell will provide widgets for uploading images and making predictions
+(this will also download the necessary model files).
+- NOTE: [celeb_recognition.ipynb](celeb_recognition.ipynb) is a standalone file and does not require any other files from the repo for running.
+
+## Model predictions in python
+- Provide paths to `celeb_mapping.json` and `celeb_index.ann` files in [celeb_recognition.py](celeb_recognition.py) and [celeb_utils.py](celeb_utils/celeb_utils.py) files. If you want to try my model, ignore this step.
+- Run [celeb_recognition.py](celeb_recognition.py) file, provide path to image in the file.
+- Output includes a list of the identified faces, bounding boxes and the predicted celeb name (unknown if not found).
+- It also displays the output with bounding boxes.
+
+## Sample image output
+![Image](https://drive.google.com/uc?export=view&id=1W4P0PPLjr0BHDkj2CzLgFGpOYn4MF1Ck)
+
+## Binder
+You can run a binder application by clicking the following link:
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main)
+
+You can also launch a voila binder application (which only has widgets for image upload and celeb prediction) by clicking [here](https://mybinder.org/v2/gh/shobhit9618/celeb_recognition/main?urlpath=%2Fvoila%2Frender%2Fceleb_recognition.ipynb).
+
+## Google Colab
+To open and run [celeb_recognition.ipynb](celeb_recognition.ipynb) file in google colab, click the following link:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shobhit9618/celeb_recognition/blob/main/celeb_recognition.ipynb)
```

### Comparing `celeb_detector-0.0.24/setup.py` & `celeb_detector-0.0.25/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="celeb_detector",
-    version="0.0.24",
+    version="0.0.25",
     author="Shobhit Gupta",
     author_email="shobhit9618@gmail.com",
     description="Model to recognize celebrities using a face matching algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shobhit9618/celeb_recognition",
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'celeb_detector=celeb_detector.celeb_recognition:main'
         ]
     },
-    install_requires = ['tensorflow',
-                        'mtcnn',
-                        'keras>=2.4.3',
+    install_requires = ['annoy',
+                        'face_recognition',
                         'imutils',
-                        'opencv-python>=4.0',
+                        'opencv-python',
                         'matplotlib',
                         'numpy',
-                        'tqdm'],
+                        'tqdm',
+                        'pillow',
+                        'torch',
+                        'onnx2torch',
+                        'requests'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

