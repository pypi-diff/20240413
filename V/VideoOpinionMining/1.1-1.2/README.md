# Comparing `tmp/VideoOpinionMining-1.1.tar.gz` & `tmp/videoopinionmining-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VideoOpinionMining-1.1.tar", last modified: Sun Apr  7 12:32:32 2024, max compression
+gzip compressed data, was "videoopinionmining-1.2.tar", last modified: Sat Apr 13 21:24:22 2024, max compression
```

## Comparing `VideoOpinionMining-1.1.tar` & `videoopinionmining-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.024619 VideoOpinionMining-1.1/
--rw-r--r--   0 art       (1000) art       (1000)     1081 2024-04-06 12:43:21.000000 VideoOpinionMining-1.1/LICENSE
--rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)     1598 2024-04-06 12:41:33.000000 VideoOpinionMining-1.1/README.md
--rw-r--r--   0 art       (1000) art       (1000)      710 2024-04-07 12:22:07.000000 VideoOpinionMining-1.1/pyproject.toml
--rw-r--r--   0 art       (1000) art       (1000)       38 2024-04-07 12:32:32.024619 VideoOpinionMining-1.1/setup.cfg
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/VideoOpinionMining/
--rw-r--r--   0 art       (1000) art       (1000)       29 2024-04-06 13:38:23.000000 VideoOpinionMining-1.1/src/VideoOpinionMining/__init__.py
--rw-r--r--   0 art       (1000) art       (1000)    28874 2024-04-07 12:21:55.000000 VideoOpinionMining-1.1/src/VideoOpinionMining/vem.py
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-07 12:32:32.014619 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/
--rw-r--r--   0 art       (1000) art       (1000)     2236 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)      281 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/SOURCES.txt
--rw-r--r--   0 art       (1000) art       (1000)        1 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/dependency_links.txt
--rw-r--r--   0 art       (1000) art       (1000)       19 2024-04-07 12:32:32.000000 VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/top_level.txt
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-13 21:24:22.461228 videoopinionmining-1.2/
+-rw-r--r--   0 art       (1000) art       (1000)     1081 2024-04-06 12:43:21.000000 videoopinionmining-1.2/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)     2214 2024-04-13 21:24:22.461228 videoopinionmining-1.2/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)     1598 2024-04-06 12:41:33.000000 videoopinionmining-1.2/README.md
+-rw-r--r--   0 art       (1000) art       (1000)      688 2024-04-13 21:23:35.000000 videoopinionmining-1.2/pyproject.toml
+-rw-r--r--   0 art       (1000) art       (1000)       38 2024-04-13 21:24:22.461228 videoopinionmining-1.2/setup.cfg
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-13 21:24:22.451228 videoopinionmining-1.2/src/
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-13 21:24:22.461228 videoopinionmining-1.2/src/VideoOpinionMining/
+-rw-r--r--   0 art       (1000) art       (1000)       29 2024-04-06 13:38:23.000000 videoopinionmining-1.2/src/VideoOpinionMining/__init__.py
+-rw-r--r--   0 art       (1000) art       (1000)    29265 2024-04-13 21:20:05.000000 videoopinionmining-1.2/src/VideoOpinionMining/vem.py
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2024-04-13 21:24:22.461228 videoopinionmining-1.2/src/VideoOpinionMining.egg-info/
+-rw-r--r--   0 art       (1000) art       (1000)     2214 2024-04-13 21:24:22.000000 videoopinionmining-1.2/src/VideoOpinionMining.egg-info/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)      281 2024-04-13 21:24:22.000000 videoopinionmining-1.2/src/VideoOpinionMining.egg-info/SOURCES.txt
+-rw-r--r--   0 art       (1000) art       (1000)        1 2024-04-13 21:24:22.000000 videoopinionmining-1.2/src/VideoOpinionMining.egg-info/dependency_links.txt
+-rw-r--r--   0 art       (1000) art       (1000)       19 2024-04-13 21:24:22.000000 videoopinionmining-1.2/src/VideoOpinionMining.egg-info/top_level.txt
```

### Comparing `VideoOpinionMining-1.1/LICENSE` & `videoopinionmining-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VideoOpinionMining-1.1/PKG-INFO` & `videoopinionmining-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: VideoOpinionMining
-Version: 1.1
+Version: 1.2
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Labic-ICMC-USP/VEM
-Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
+Project-URL: Example, https://colab.research.google.com/drive/1sYAYRxFdpa86Huxm-KVkEvQo6x8ZmgS6?authuser=1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VideoOpinionMining-1.1/README.md` & `videoopinionmining-1.2/README.md`

 * *Files identical despite different names*

### Comparing `VideoOpinionMining-1.1/pyproject.toml` & `videoopinionmining-1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VideoOpinionMining"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Artur Lima", email="vligmart@gmail.com" },
 ]
 description = "This package receives an mp4 file classfying it according to its emotions and generating a heat map"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Labic-ICMC-USP/VEM"
-"Example" = "https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB"
+"Example" = "https://colab.research.google.com/drive/1sYAYRxFdpa86Huxm-KVkEvQo6x8ZmgS6?authuser=1"
```

### Comparing `VideoOpinionMining-1.1/src/VideoOpinionMining/vem.py` & `videoopinionmining-1.2/src/VideoOpinionMining/vem.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
     def process_video(self, video_file, segment_block_size = 10):
         """
           Use this to run the models for all the modalities(transcript, audio, video and multimodal) and generate the heatmaps.
 
           Args:
             **video_file (mp4)**: video to be analized.
+
             **segment_block_size (int)**: size of the block used in each frame of the heatmap.
 
           Return:
             Nothing.
 
           In case you also want the dataframes generated with all the emotions, object_of_class.segmented_video contains it.
 
@@ -83,27 +84,33 @@
         self.opinion_extractor_audio.segmenter_result = self.segmented_video
         self.opinion_extractor_video.segmenter_result = self.segmented_video
         
         self.opinion_extractor_transc.extract_opinions()
         self.opinion_extractor_audio.extract_opinions()
         self.opinion_extractor_video.extract_opinions()
         
+        try:
+           self.segmented_video = self.segmented_video.drop('video_embeddings', axis=1)
+        except:
+           pass
+        
         # Step 3: Extract multimodal opinions
         self.multimodal_extractor.segmented_with_emotion = self.segmented_video
         self.multimodal_extractor.extract_multimodal_opinions()
 
         # Step 4: Generate emotion map
         self.emotion_map_generator.segments_with_emotion = self.segmented_video
         self.emotion_map_generator.graph = self.multimodal_extractor.G_multimodal
 
         self.emotion_map_generator.generate_emotion_map("transcript",segment_block_size)
         self.emotion_map_generator.generate_emotion_map("audio",segment_block_size)
         self.emotion_map_generator.generate_emotion_map("video",segment_block_size)
         self.emotion_map_generator.generate_emotion_map("multimodal",segment_block_size)
 
+
 class VideoSegmenter:
     """
         Class responsible for extracting the transcription from the video, segmenting it in phrases with the
         timestamps and name of the parts contained in a dataframe
     """
     def __init__(self):
         logging.basicConfig(filename="newfile.log",
@@ -327,18 +334,22 @@
 
           return emot, scor, None
 
 #uso dos modelos acima
 class OpinionExtractor:
     """
         Class responsible for applying the models to all the segments of the video
+
         Args:
             **segmenter_result (dataframe)**: sentences to be analyzed.
 
             **opinion_model (OpinionExtractionModel)**: Model responsible for the analysis.
+        
+        Return:
+            Nothing.
     """
     def __init__(self, segmenter_result, opinion_model):
         self.segmenter_result = segmenter_result
         self.opinion_model = opinion_model
 
         logging.basicConfig(filename="newfile.log",
         format='%(asctime)s %(message)s',filemode='w')
@@ -366,17 +377,21 @@
         self.segmenter_result[self.opinion_model.modality + '_prob'] = scor
         self.segmenter_result[self.opinion_model.modality + '_embeddings'] = embeddings
 
 class MultimodalOpinionExtractor:
     """
         Class responsible for applying the multimodal model to all the segments of the video after
         the audio and transcript classification have already been done
+
         Args:
             **segmented_with_emotion (dataframe)**: sentences to be analyzed with the audio and 
             transcript classification already been done.
+
+        Return:
+            Nothing.
             
     """
     def __init__(self, segmented_with_emotion):
         self.segmented_with_emotion = segmented_with_emotion
         url1 = 'https://drive.google.com/uc?id=1yJBHU8Zl4MuoQfJqkPgVDwJfYRJDPUAH'
         output = 'emotions_coord.xlsx'
         gdown.download(url1, output, quiet=False)
@@ -411,19 +426,23 @@
 
         for index,row in self.segmented_with_emotion.iterrows():
           self.G_multimodal.nodes[index]['pseudolabeling'] = 1.0 - (t[index]/np.max(t))
 
 class EmotionMapGenerator:
     """
         Class responsible for generating the heatmaps visualization of the classifications.
+
         Args:
             **segmented_with_emotion (dataframe)**: sentences to be analyzed with the audio and 
             transcript classification already been done.
 
             **graph (networkx graph)**: graph generated by the multimodal model
+
+        Return:
+            Nothing.
             
     """
     def __init__(self, segments_with_emotion, graph = None):
         self.segments_with_emotion = segments_with_emotion
         self.graph = graph
 
         url1 = 'https://drive.google.com/uc?id=1yJBHU8Zl4MuoQfJqkPgVDwJfYRJDPUAH'
@@ -439,19 +458,23 @@
     def generate_emotion_map(self, modality, segment_block_size = 5):
         # Divide segments into blocks
         # Calculate emotion distribution for each block
         # Generate emotion wheel for each block
         # Create a video showing the evolution of emotion map over time
         """
         Generate an emotion wheel for each block of segments in the format of mp4 and png.
+
         Args:
             **modality (string)**: for which modality is the heatmap to be created (the opinion excration of the
             respective modality have to be done befor)
 
             **segment_block_size (int)**: how many phrases are shown in the same frame of the heatmap.
+
+        Return:
+            Nothing.
         """
         if modality == 'multimodal':
           x = []
           y = []
           x_img = []
           y_img = []
           GCP(self.graph,mi=1,audio_weight=0.4, text_weight=0.6,max_iter=30)
@@ -508,14 +531,15 @@
             if all(val == 0 for val in x_temp) and all(val == 0 for val in y_temp):
               x_temp = np.array([0])
               y_temp = np.array([0])
             else:
               x_temp = [i for i,j in zip(x_temp,y_temp) if (i != 0 and j != 0)]
               y_temp = [j for i,j in zip(x[id_ini: id_fim],y_temp) if (i != 0 and j != 0)]
 
+            plot_heatmap(x_temp, y_temp, self.emotions_coord, "animated", vid_name)
             plt.title("Emotions from " + str(id_ini) + " to " + str(id_fim-1) + " block")
             plt.savefig("tempjpgs/output" + str(atual) + ".jpg")
             plt.close()
 
             id_ini += segment_block_size
             id_fim += segment_block_size
             atual += 1
@@ -775,8 +799,8 @@
 
 #Funcoes uteis
 def to_seconds(horario):
 
   horario_separado = horario.split(":")
   seconds = 3600*int(horario_separado[0]) + 60*int(horario_separado[1]) + float(horario_separado[2])
 
-  return seconds
+  return seconds
```

### Comparing `VideoOpinionMining-1.1/src/VideoOpinionMining.egg-info/PKG-INFO` & `videoopinionmining-1.2/src/VideoOpinionMining.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: VideoOpinionMining
-Version: 1.1
+Version: 1.2
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Labic-ICMC-USP/VEM
-Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
+Project-URL: Example, https://colab.research.google.com/drive/1sYAYRxFdpa86Huxm-KVkEvQo6x8ZmgS6?authuser=1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

