# Comparing `tmp/tck-0.4.2.tar.gz` & `tmp/tck-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tck-0.4.2.tar", last modified: Sat Apr 13 00:44:39 2024, max compression
+gzip compressed data, was "tck-0.4.3.tar", last modified: Sat Apr 13 00:55:25 2024, max compression
```

## Comparing `tck-0.4.2.tar` & `tck-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-03-21 23:02:41.000000 tck-0.4.2/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:44:39.748548 tck-0.4.2/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     5740 2024-03-25 11:34:48.000000 tck-0.4.2/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-13 00:44:39.748548 tck-0.4.2/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      820 2024-04-13 00:43:31.000000 tck-0.4.2/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/tck/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     6429 2024-03-21 23:18:31.000000 tck-0.4.2/tck/GMM_MAP_EM.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     2138 2024-03-21 23:23:22.000000 tck-0.4.2/tck/GMMposterior.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     4748 2024-04-13 00:42:59.000000 tck-0.4.2/tck/TCK.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-03-21 23:08:34.000000 tck-0.4.2/tck/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     5498 2024-03-23 19:06:23.000000 tck-0.4.2/tck/datasets.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/tck.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      241 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       51 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        4 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:55:25.344533 tck-0.4.3/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-03-21 23:02:41.000000 tck-0.4.3/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:55:25.344533 tck-0.4.3/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     5740 2024-03-25 11:34:48.000000 tck-0.4.3/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-13 00:55:25.344533 tck-0.4.3/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      820 2024-04-13 00:54:23.000000 tck-0.4.3/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:55:25.344533 tck-0.4.3/tck/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     6429 2024-03-21 23:18:31.000000 tck-0.4.3/tck/GMM_MAP_EM.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     2138 2024-03-21 23:23:22.000000 tck-0.4.3/tck/GMMposterior.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     4738 2024-04-13 00:53:46.000000 tck-0.4.3/tck/TCK.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-03-21 23:08:34.000000 tck-0.4.3/tck/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     5498 2024-03-23 19:06:23.000000 tck-0.4.3/tck/datasets.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:55:25.344533 tck-0.4.3/tck.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:55:25.000000 tck-0.4.3/tck.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      241 2024-04-13 00:55:25.000000 tck-0.4.3/tck.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-13 00:55:25.000000 tck-0.4.3/tck.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       51 2024-04-13 00:55:25.000000 tck-0.4.3/tck.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        4 2024-04-13 00:55:25.000000 tck-0.4.3/tck.egg-info/top_level.txt
```

### Comparing `tck-0.4.2/LICENSE` & `tck-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tck-0.4.2/PKG-INFO` & `tck-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tck
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kernel similarity for classification and clustering of multi-variate time series with missing values.
 Home-page: https://github.com/FilippoMB/Time-Series-Cluster-Kernel
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tck-0.4.2/README.md` & `tck-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tck-0.4.2/setup.py` & `tck-0.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tck",
-    version="0.4.2",
+    version="0.4.3",
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'numpy>1.19.5',
         'scikit_learn>=1.4',
         'scipy',
         'requests',
```

### Comparing `tck-0.4.2/tck/GMM_MAP_EM.py` & `tck-0.4.3/tck/GMM_MAP_EM.py`

 * *Files identical despite different names*

### Comparing `tck-0.4.2/tck/GMMposterior.py` & `tck-0.4.3/tck/GMMposterior.py`

 * *Files identical despite different names*

### Comparing `tck-0.4.2/tck/TCK.py` & `tck-0.4.3/tck/TCK.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         training_msg += f"\tLength of time segments sampled from [{minT}, {maxT}]\n\n"
         print(training_msg)
         
         # Parallel processing
         with ProcessPoolExecutor() as executor:
             # Pass additional arguments required by process_gmm
             futures = [executor.submit(self.process_gmm, X, self.G, minN, minT, maxT, minV, maxV, I, missing, i) for i in range(self.G * (self.C - 1))]
-            for future in tqdm.tqdm(futures, desc='Fitting GMMs'):
+            for future in tqdm(futures, desc='Fitting GMMs'):
                 self.GMM.append(future.result())
       
         return self
 
     
     def predict(self, mode, Xte=None):
         """
@@ -107,11 +107,11 @@
         elif mode == 'tr-te':
             K = np.zeros((self.GMM[0][0].shape[0], Xte.shape[0]))
         elif mode == 'te-te':
             K = np.zeros((Xte.shape[0], Xte.shape[0]))
 
         with ProcessPoolExecutor() as executor:
             futures = [executor.submit(self.update_matrix, i, mode, Xte) for i in range(self.G * (self.C - 1))]
-            for future in tqdm.tqdm(futures, desc=f"Computing TCK ({mode})"):
+            for future in tqdm(futures, desc=f"Computing TCK ({mode})"):
                 K += future.result()
         
         return K
```

### Comparing `tck-0.4.2/tck/datasets.py` & `tck-0.4.3/tck/datasets.py`

 * *Files identical despite different names*

### Comparing `tck-0.4.2/tck.egg-info/PKG-INFO` & `tck-0.4.3/tck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tck
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kernel similarity for classification and clustering of multi-variate time series with missing values.
 Home-page: https://github.com/FilippoMB/Time-Series-Cluster-Kernel
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

