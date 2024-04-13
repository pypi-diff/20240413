# Comparing `tmp/sideseeing-tools-0.1.4.tar.gz` & `tmp/sideseeing_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing-tools-0.1.4.tar", last modified: Thu Apr 11 19:25:00 2024, max compression
+gzip compressed data, was "sideseeing_tools-0.1.5.tar", last modified: Sat Apr 13 16:29:06 2024, max compression
```

## Comparing `sideseeing-tools-0.1.4.tar` & `sideseeing_tools-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:25:00.887998 sideseeing-tools-0.1.4/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing-tools-0.1.4/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:25:00.887998 sideseeing-tools-0.1.4/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3595 2024-04-11 18:55:32.000000 sideseeing-tools-0.1.4/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      881 2024-04-11 19:12:19.000000 sideseeing-tools-0.1.4/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-11 19:25:00.887998 sideseeing-tools-0.1.4/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:25:00.879998 sideseeing-tools-0.1.4/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:25:00.887998 sideseeing-tools-0.1.4/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-11 19:11:31.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2846 2024-04-11 16:52:19.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    22548 2024-04-11 19:16:05.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5577 2024-04-11 18:31:34.000000 sideseeing-tools-0.1.4/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:25:00.887998 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:25:00.000000 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      448 2024-04-11 19:25:00.000000 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-11 19:25:00.000000 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      137 2024-04-11 19:25:00.000000 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-11 19:25:00.000000 sideseeing-tools-0.1.4/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-13 16:29:06.294593 sideseeing_tools-0.1.5/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing_tools-0.1.5/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4380 2024-04-13 16:29:06.294593 sideseeing_tools-0.1.5/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3501 2024-04-13 16:28:27.000000 sideseeing_tools-0.1.5/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      878 2024-04-13 15:57:19.000000 sideseeing_tools-0.1.5/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-13 16:29:06.294593 sideseeing_tools-0.1.5/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-13 16:29:06.286593 sideseeing_tools-0.1.5/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-13 16:29:06.290593 sideseeing_tools-0.1.5/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-11 19:11:31.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2341 2024-04-13 15:55:53.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    13159 2024-04-13 16:11:10.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/plot.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8245 2024-04-13 16:02:12.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     7369 2024-04-13 16:04:14.000000 sideseeing_tools-0.1.5/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-13 16:29:06.294593 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4380 2024-04-13 16:29:06.000000 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      477 2024-04-13 16:29:06.000000 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-13 16:29:06.000000 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      134 2024-04-13 16:29:06.000000 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-13 16:29:06.000000 sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/top_level.txt
```

### Comparing `sideseeing-tools-0.1.4/LICENSE` & `sideseeing_tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.4/PKG-INFO` & `sideseeing_tools-0.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: folium~=0.13.0
 Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
-Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: moviepy~=1.0.3
 Requires-Dist: numpy~=1.25.0
 Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
 
@@ -30,21 +30,17 @@
 pip install sideseeing-tools
 ```
 
 ## Usage
 
 __Creating a dataset__
 ```python
-from sideseeing_tools import sideseeing as side
+from sideseeing_tools import sideseeing
 
-# If your content directories are in /home/user/my-project/data, use this
-ds = side.SideSeeingDS(root_dir='/home/user/my-project', subdir_data='data')
-
-# Otherwise, if your content directories are in /home/user/my-project, use this
-ds = side.SideSeeingDS(root_dir='/home/user/my-project')
+ds = sideseeing.SideSeeingDS(root_dir='/home/user/my-project')
 
 # Available iterators
 #   .instances  // Tip: dictionary of instances (key=instance_name, value=SideSeeingInstance)
 #   .iterator   // Tip: for i in ds.iterator: i.instance_name
 
 # Available attributes and methods
 #   .metadata() // Tip: generates and prints the dataset metadata
@@ -73,15 +69,17 @@
 | `label`               | List of categories and tags representing the taxonomy of sidewalks. |
 | `video_start_time`    | Start time of the video associated with the collected data. |
 | `video_stop_time`     | Stop time of the video associated with the collected data. |
 
 
 __Creating a plotter__
 ```python
-plotter = sst.SideSeeingPlotter(ds, '/home/user/my-project/taxonomy.csv')
+from sideseeing_tools import plot
+
+plotter = plot.SideSeeingPlotter(ds, taxonomy='/home/user/my-project/taxonomy.csv')
 
 # Available methods:
 #   .plot_dataset_cities()
 #   .plot_dataset_map()
 #   .plot_dataset_sensors3()
 #   .plot_dataset_tags_matrix()
 #   .plot_dataset_tags()
@@ -90,39 +88,42 @@
 #   .plot_instance_sensors3_and_audio()
 #   .plot_instance_video_frames_at_times()
 #   .plot_instance_video_frames()
 ```
 
 __Suggested dataset folder structure__
 
-- **my-project/**
-    - metadata.csv (autogenerated)
-    - taxonomy.csv
-    - **data/**
-        - **CityName1-LocationName1/**
-            - **Route01-Timestamp/**
-                - consumption.csv
-                - gps.csv
-                - metadata.json
-                - sensors.one.csv
-                - sensors.three.csv
-                - sensors.three.uncalibrated.csv
-                - video.mp4
-                - video.gif (autoextracted)
-                - video.wav (autoextracted)
-            - **Route02-Timestamp/**
-                - consumption.csv
-                - ...
-        - **CityName1-LocationName2/**
-            - **Route01-Timestamp/**
-                - ...
-            - ...
-        - **CityName2-LocationName1/**
-            - **Route01-Timestamp/**
-                - ...
-            - ...
+`ds = sideseeing.SideSeeingDS('/home/user/my-project', subdir='data', name='MyDataset')`
+
+```text
+my-project/
+├─ data/
+│  ├─ place01/
+│  │  ├─ route01/
+│  │  │  ├─ consumption.csv
+│  │  │  ├─ gps.csv
+│  │  │  ├─ metadata.json
+│  │  │  ├─ sensors.one.csv
+│  │  │  ├─ sensors.three.csv
+│  │  │  ├─ sensors.three.uncalibrated.csv
+│  │  │  ├─ video.gif
+│  │  │  ├─ video.mp4
+│  │  │  ├─ video.wav
+│  │  ├─ route02/
+│  ├─ place02/
+│  ├─ place03/
+├─ metadata.csv
+├─ taxonomy.csv
+```
+
 
 ## Documentation
 Under construction.
 
+## Author
+
+[Rafael J P Damaceno](https://github.com/rafaelpezzuto)
+
+
 ## About us
-Take a look at our [website](https://sites.usp.br/sideseeing).
+
+The SideSeeing Project aims to develop methods based on Computer Vision and Machine Learning for Urban Informatics applications. Our goal is to devise strategies for obtaining and analyzing data related to urban accessibility. Take a look at our [website](https://sites.usp.br/sideseeing).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sideseeing-tools-0.1.4/README.md` & `sideseeing_tools-0.1.5/src/sideseeing_tools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,46 @@
+Metadata-Version: 2.1
+Name: sideseeing-tools
+Version: 0.1.5
+Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
+Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
+Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
+Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: folium~=0.13.0
+Requires-Dist: imageio~=2.5.0
+Requires-Dist: librosa~=0.10.0
+Requires-Dist: moviepy~=1.0.3
+Requires-Dist: numpy~=1.25.0
+Requires-Dist: opencv-python~=4.7.0.68
+Requires-Dist: pandas~=2.0.3
+Requires-Dist: reverse-geocode==1.6
+
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
 
 ```bash
 pip install sideseeing-tools
 ```
 
 ## Usage
 
 __Creating a dataset__
 ```python
-from sideseeing_tools import sideseeing as side
-
-# If your content directories are in /home/user/my-project/data, use this
-ds = side.SideSeeingDS(root_dir='/home/user/my-project', subdir_data='data')
+from sideseeing_tools import sideseeing
 
-# Otherwise, if your content directories are in /home/user/my-project, use this
-ds = side.SideSeeingDS(root_dir='/home/user/my-project')
+ds = sideseeing.SideSeeingDS(root_dir='/home/user/my-project')
 
 # Available iterators
 #   .instances  // Tip: dictionary of instances (key=instance_name, value=SideSeeingInstance)
 #   .iterator   // Tip: for i in ds.iterator: i.instance_name
 
 # Available attributes and methods
 #   .metadata() // Tip: generates and prints the dataset metadata
@@ -51,15 +69,17 @@
 | `label`               | List of categories and tags representing the taxonomy of sidewalks. |
 | `video_start_time`    | Start time of the video associated with the collected data. |
 | `video_stop_time`     | Stop time of the video associated with the collected data. |
 
 
 __Creating a plotter__
 ```python
-plotter = sst.SideSeeingPlotter(ds, '/home/user/my-project/taxonomy.csv')
+from sideseeing_tools import plot
+
+plotter = plot.SideSeeingPlotter(ds, taxonomy='/home/user/my-project/taxonomy.csv')
 
 # Available methods:
 #   .plot_dataset_cities()
 #   .plot_dataset_map()
 #   .plot_dataset_sensors3()
 #   .plot_dataset_tags_matrix()
 #   .plot_dataset_tags()
@@ -68,39 +88,42 @@
 #   .plot_instance_sensors3_and_audio()
 #   .plot_instance_video_frames_at_times()
 #   .plot_instance_video_frames()
 ```
 
 __Suggested dataset folder structure__
 
-- **my-project/**
-    - metadata.csv (autogenerated)
-    - taxonomy.csv
-    - **data/**
-        - **CityName1-LocationName1/**
-            - **Route01-Timestamp/**
-                - consumption.csv
-                - gps.csv
-                - metadata.json
-                - sensors.one.csv
-                - sensors.three.csv
-                - sensors.three.uncalibrated.csv
-                - video.mp4
-                - video.gif (autoextracted)
-                - video.wav (autoextracted)
-            - **Route02-Timestamp/**
-                - consumption.csv
-                - ...
-        - **CityName1-LocationName2/**
-            - **Route01-Timestamp/**
-                - ...
-            - ...
-        - **CityName2-LocationName1/**
-            - **Route01-Timestamp/**
-                - ...
-            - ...
+`ds = sideseeing.SideSeeingDS('/home/user/my-project', subdir='data', name='MyDataset')`
+
+```text
+my-project/
+├─ data/
+│  ├─ place01/
+│  │  ├─ route01/
+│  │  │  ├─ consumption.csv
+│  │  │  ├─ gps.csv
+│  │  │  ├─ metadata.json
+│  │  │  ├─ sensors.one.csv
+│  │  │  ├─ sensors.three.csv
+│  │  │  ├─ sensors.three.uncalibrated.csv
+│  │  │  ├─ video.gif
+│  │  │  ├─ video.mp4
+│  │  │  ├─ video.wav
+│  │  ├─ route02/
+│  ├─ place02/
+│  ├─ place03/
+├─ metadata.csv
+├─ taxonomy.csv
+```
+
 
 ## Documentation
 Under construction.
 
+## Author
+
+[Rafael J P Damaceno](https://github.com/rafaelpezzuto)
+
+
 ## About us
-Take a look at our [website](https://sites.usp.br/sideseeing).
+
+The SideSeeing Project aims to develop methods based on Computer Vision and Machine Learning for Urban Informatics applications. Our goal is to devise strategies for obtaining and analyzing data related to urban accessibility. Take a look at our [website](https://sites.usp.br/sideseeing).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sideseeing-tools-0.1.4/pyproject.toml` & `sideseeing_tools-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "sideseeing-tools"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "folium~=0.13.0",
   "imageio~=2.5.0",
   "librosa~=0.10.0",
-  "matplotlib~=3.7.1",
+  "moviepy~=1.0.3",
   "numpy~=1.25.0",
   "opencv-python~=4.7.0.68",
   "pandas~=2.0.3",
   "reverse-geocode==1.6",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `sideseeing-tools-0.1.4/src/sideseeing_tools/constants.py` & `sideseeing_tools-0.1.5/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.4/src/sideseeing_tools/media.py` & `sideseeing_tools-0.1.5/src/sideseeing_tools/media.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-import base64
 import os
-import subprocess
 
-import cv2
 import imageio
+import cv2
 
-from IPython.display import (
-    Audio, 
-    HTML, 
-    Image,
-)
+from moviepy.editor import VideoFileClip
 
 
-def extract_audio(source_path: str, target_path: str, sample_rate=44100, channels=2, codec='pcm_s16le'):
+def extract_audio(source_path: str, target_path: str, sample_rate=44100, channels=2, codec='pcm_s16le', overwrite=False):
     '''
     Extracts audio in WAV format from a video file.
     '''
     target_dir = os.path.dirname(target_path)
 
     if not os.path.exists(target_dir):
         os.makedirs(target_dir)
 
     mp4_name = os.path.basename(source_path)
     wav_path = os.path.join(target_dir, mp4_name.replace('.mp4', '.wav'))
 
-    if not os.path.exists(wav_path):
+    if not os.path.exists(wav_path) or overwrite:
         print(f'INFO. Extracting WAV from {source_path} to {wav_path}.')
-        subprocess.call(['ffmpeg', '-i', source_path, '-vn', '-acodec', codec, '-ar', f'{sample_rate}', '-ac', f'{channels}', wav_path])
+        clip = VideoFileClip(source_path)
+        clip.audio.write_audiofile(wav_path, fps=sample_rate, nbytes=2, codec=codec, ffmpeg_params=["-ac", str(channels)])
+        clip.close()
 
     return wav_path
 
 
 def extract_gif(source_path: str, target_path: str, target_width=300, target_fps=5):
     '''
     Extracts a tiny video in GIF format from a video file.
@@ -70,31 +66,7 @@
                 break
 
         imageio.mimsave(gif_path, gif_frames_list, fps=target_fps, subrectangles=True)
 
         cap.release()
 
     return gif_path
-
-
-def play_video(path: str):
-    '''
-    Plays the video.
-    '''
-    mp4 = open(path,'rb').read()
-    data_url = "data:video/mp4;base64," + base64.b64encode(mp4).decode()
-    return HTML("""<video width=400 controls><source src="%s" type="video/mp4"></video>""" % data_url)
-
-
-def play_gif(path: str):
-    '''
-    Displays the GIF.
-    '''
-    with open(path, 'rb') as f:
-        display(Image(data=f.read(), format='png'))
-
-
-def play_audio(path: str):
-    '''
-    Plays the audio track.
-    '''
-    return display(Audio(path))
```

### Comparing `sideseeing-tools-0.1.4/src/sideseeing_tools/utils.py` & `sideseeing_tools-0.1.5/src/sideseeing_tools/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,92 @@
 import csv
 import datetime
 import requests
 
+import cv2
 import numpy as np
 import pandas as pd
 import reverse_geocode
 
 
 def load_csv_data(path: str, fieldnames: list, delimiter=','):
-  '''
-  Reads a CSV file using csv.DictReader and a predefined list of fields.
-  '''
-  data = []
+    '''
+    Reads a CSV file using csv.DictReader and a predefined list of fields.
+    '''
+    data = []
+
+    with open(path) as fin:
+        for row in csv.DictReader(fin, fieldnames=fieldnames, delimiter=delimiter):
+          new_row = {}
+          for k, v in row.items():
+            new_row[k.strip().lower()] = v.strip().lower()
+          data.append(new_row)
+
+    return data
+
+
+def load_csv_data_with_pandas(path: str):
+    return pd.read_csv(path)
+
 
-  with open(path) as fin:
-      for row in csv.DictReader(fin, fieldnames=fieldnames, delimiter=delimiter):
-        new_row = {}
-        for k, v in row.items():
-          new_row[k.strip().lower()] = v.strip().lower()
-        data.append(new_row)
+def save_csv_data_with_pandas(data: pd.DataFrame, path: str, index=False):
+    data.to_csv(path, index=index)
 
-  return data
+
+def generate_metadata(iterator, datetime_format: str):
+    items = []
+
+    for i in iterator:
+        cap = cv2.VideoCapture(i.video)
+        v_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        v_fps = cap.get(cv2.CAP_PROP_FPS)
+        v_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        v_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+        cap.release()
+
+        item = {}
+
+        item['name'] = i.instance_name
+        item['video_start_time'] = datetime.datetime.strptime(i.metadata.get('time', {}).get('videoStartDateTime', ''), datetime_format)
+        item['video_end_time'] = datetime.datetime.strptime(i.metadata.get('time', {}).get('videoStopDateTime', ''), datetime_format)
+        item['video_duration'] = round(v_frames / v_fps, 2)
+        item['video_frames'] = v_frames
+        item['video_fps'] = v_fps
+        item['video_resolution'] = f'{v_width}x{v_height}'
+        item['manufacturer'] = i.metadata.get('device', {}).get('manufacturer', '')
+        item['model'] = i.metadata.get('device', {}).get('model', '')
+        item['so_version'] = i.metadata.get('device', {}).get('androidVersion', '')
+
+        items.append(item)
+
+    return pd.DataFrame.from_dict(items)
 
 
 def standardize_sensor_name(sensor_name: str):
   '''
   Obtains an adequately sensor's name
   '''
   sensor_name_lowered = sensor_name.lower()
 
-  if 'accel' in sensor_name_lowered:
+  if 'accel' in sensor_name_lowered or 'acc' in sensor_name_lowered:
     if 'linear' in sensor_name_lowered:
       return 'Linear Accelerometer'
-    else:
-      return 'Accelerometer'
+    return 'Accelerometer'
 
   if 'grav' in sensor_name_lowered:
     return 'Gravity'
 
   if 'gyro' in sensor_name_lowered:
+    if 'uncali' in sensor_name_lowered:
+       return 'Gyroscope Uncalibrated'
     return 'Gyroscope'
 
-  if 'magn' in sensor_name_lowered:
+  if 'mag' in sensor_name_lowered:
+    if 'uncali' in sensor_name_lowered:
+       return 'Magnetometer Uncalibrated'
     return 'Magnetometer'
 
   if 'light' in sensor_name_lowered or 'lux' in sensor_name_lowered:
     if 'uncalibrated' in sensor_name_lowered:
       return 'Light Uncalibrated'
     return 'Light'
 
@@ -102,14 +143,17 @@
       ])
 
     series[sensor_name].append(current_data)
 
   if ignored_lines > 0 and debug:
     print(f'INFO. {ignored_lines} lines has been ignored.')
 
+  if debug:
+    print(f'Converting sensor data to pandas.DataFrame')
+  
   for key, value in series.items():
     series[key] = to_dataframe(value, num_axes, datetime_format)
 
   return series
 
 
 def to_dataframe(data: dict, num_axes: int, datetime_format: str, create_time_column=True):
@@ -132,14 +176,18 @@
   if create_time_column:
       df['Datetime UTC'] = pd.to_datetime(df['Datetime UTC'], format=datetime_format)
       df['Time (s)'] = (df['Datetime UTC'] - df['Datetime UTC'].iloc[0]).dt.total_seconds()
 
   return df
 
 
+def preprocess_gps(data: dict):
+    return np.array([[float(d['latitude']), float(d['longitude'])] for d in data])
+
+
 def resample_sensor_data(data: pd.DataFrame, target_fps=30):
     '''
     Converts the sensor data to match the FPS rate of the video.
     This is necessary because the frequency of sensor data varies.
     At times, there are 100 points in a single second, while at other times, there are only 50 points.
     This variation is controlled by the Android device, and it is crucial to ensure synchronization between the video and sensor data.
     '''
```

