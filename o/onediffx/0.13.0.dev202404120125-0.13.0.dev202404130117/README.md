# Comparing `tmp/onediffx-0.13.0.dev202404120125.tar.gz` & `tmp/onediffx-0.13.0.dev202404130117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-0.13.0.dev202404120125.tar", last modified: Fri Apr 12 01:25:38 2024, max compression
+gzip compressed data, was "onediffx-0.13.0.dev202404130117.tar", last modified: Sat Apr 13 01:17:43 2024, max compression
```

## Comparing `onediffx-0.13.0.dev202404120125.tar` & `onediffx-0.13.0.dev202404130117.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.638832 onediffx-0.13.0.dev202404120125/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 01:25:17.000000 onediffx-0.13.0.dev202404120125/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.638832 onediffx-0.13.0.dev202404120125/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.638832 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-12 01:25:38.000000 onediffx-0.13.0.dev202404120125/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-12 01:25:38.000000 onediffx-0.13.0.dev202404120125/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:25:38.000000 onediffx-0.13.0.dev202404120125/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 01:25:38.000000 onediffx-0.13.0.dev202404120125/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:25:38.000000 onediffx-0.13.0.dev202404120125/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:25:38.642832 onediffx-0.13.0.dev202404120125/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-12 01:25:16.000000 onediffx-0.13.0.dev202404120125/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.723283 onediffx-0.13.0.dev202404130117/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.723283 onediffx-0.13.0.dev202404130117/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-13 01:17:43.000000 onediffx-0.13.0.dev202404130117/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 01:17:43.000000 onediffx-0.13.0.dev202404130117/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:17:43.000000 onediffx-0.13.0.dev202404130117/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 01:17:43.000000 onediffx-0.13.0.dev202404130117/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 01:17:43.000000 onediffx-0.13.0.dev202404130117/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:17:43.727283 onediffx-0.13.0.dev202404130117/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-13 01:17:20.000000 onediffx-0.13.0.dev202404130117/tests/test_lora.py
```

### Comparing `onediffx-0.13.0.dev202404120125/PKG-INFO` & `onediffx-0.13.0.dev202404130117/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 0.13.0.dev202404120125
+Version: 0.13.0.dev202404130117
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-0.13.0.dev202404120125/README.md` & `onediffx-0.13.0.dev202404130117/README.md`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-0.13.0.dev202404130117/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/__init__.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-0.13.0.dev202404130117/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/lora/lora.py` & `onediffx-0.13.0.dev202404130117/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/lora/state_dict_utils.py` & `onediffx-0.13.0.dev202404130117/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/lora/text_encoder.py` & `onediffx-0.13.0.dev202404130117/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/lora/unet.py` & `onediffx-0.13.0.dev202404130117/onediffx/lora/unet.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/lora/utils.py` & `onediffx-0.13.0.dev202404130117/onediffx/lora/utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx/utils/patch_image_processor.py` & `onediffx-0.13.0.dev202404130117/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/onediffx.egg-info/PKG-INFO` & `onediffx-0.13.0.dev202404130117/onediffx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 0.13.0.dev202404120125
+Version: 0.13.0.dev202404130117
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-0.13.0.dev202404120125/onediffx.egg-info/SOURCES.txt` & `onediffx-0.13.0.dev202404130117/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/setup.py` & `onediffx-0.13.0.dev202404130117/setup.py`

 * *Files identical despite different names*

### Comparing `onediffx-0.13.0.dev202404120125/tests/test_lora.py` & `onediffx-0.13.0.dev202404130117/tests/test_lora.py`

 * *Files identical despite different names*

