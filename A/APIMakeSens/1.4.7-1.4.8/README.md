# Comparing `tmp/APIMakeSens-1.4.7.tar.gz` & `tmp/APIMakeSens-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIMakeSens-1.4.7.tar", last modified: Tue Mar 26 00:09:40 2024, max compression
+gzip compressed data, was "APIMakeSens-1.4.8.tar", last modified: Fri Apr 12 22:14:21 2024, max compression
```

## Comparing `APIMakeSens-1.4.7.tar` & `APIMakeSens-1.4.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 00:09:40.173175 APIMakeSens-1.4.7/
-drwxrwxrwx   0        0        0        0 2024-03-26 00:09:40.125337 APIMakeSens-1.4.7/APIMakeSens.egg-info/
--rw-rw-rw-   0        0        0      525 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-26 00:09:39.000000 APIMakeSens-1.4.7/APIMakeSens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-08-31 12:46:55.000000 APIMakeSens-1.4.7/LICENSE
-drwxrwxrwx   0        0        0        0 2024-03-26 00:09:40.169172 APIMakeSens-1.4.7/MakeSens/
--rw-rw-rw-   0        0        0    13929 2024-03-25 23:57:45.000000 APIMakeSens-1.4.7/MakeSens/MakeSens.py
--rw-rw-rw-   0        0        0       19 2024-03-26 00:09:33.000000 APIMakeSens-1.4.7/MakeSens/__init__.py
--rw-rw-rw-   0        0        0      138 2022-08-31 12:46:55.000000 APIMakeSens-1.4.7/MakeSens/__main__.py
--rw-rw-rw-   0        0        0      311 2024-03-25 19:04:25.000000 APIMakeSens-1.4.7/MakeSens/colors_by_variable.json
--rw-rw-rw-   0        0        0      525 2024-03-26 00:09:40.171172 APIMakeSens-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      117 2022-08-31 12:46:55.000000 APIMakeSens-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 00:09:40.173175 APIMakeSens-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-03-26 00:09:30.000000 APIMakeSens-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:14:20.993966 APIMakeSens-1.4.8/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:14:20.968972 APIMakeSens-1.4.8/APIMakeSens.egg-info/
+-rw-rw-rw-   0        0        0      525 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 22:14:20.000000 APIMakeSens-1.4.8/APIMakeSens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-08-31 12:46:55.000000 APIMakeSens-1.4.8/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-12 22:14:20.987965 APIMakeSens-1.4.8/MakeSens/
+-rw-rw-rw-   0        0        0    13985 2024-04-12 22:09:57.000000 APIMakeSens-1.4.8/MakeSens/MakeSens.py
+-rw-rw-rw-   0        0        0       19 2024-04-12 22:13:50.000000 APIMakeSens-1.4.8/MakeSens/__init__.py
+-rw-rw-rw-   0        0        0      138 2022-08-31 12:46:55.000000 APIMakeSens-1.4.8/MakeSens/__main__.py
+-rw-rw-rw-   0        0        0      311 2024-03-25 19:04:25.000000 APIMakeSens-1.4.8/MakeSens/colors_by_variable.json
+-rw-rw-rw-   0        0        0      525 2024-04-12 22:14:20.991989 APIMakeSens-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2022-08-31 12:46:55.000000 APIMakeSens-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 22:14:20.993966 APIMakeSens-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-04-12 22:12:53.000000 APIMakeSens-1.4.8/setup.py
```

### Comparing `APIMakeSens-1.4.7/APIMakeSens.egg-info/PKG-INFO` & `APIMakeSens-1.4.8/APIMakeSens.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIMakeSens
-Version: 1.4.7
+Version: 1.4.8
 Summary: MakeSense API
 Home-page: https://github.com/MakeSens-Data/MakeSensAPI_Python
 Author: MakeSens
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `APIMakeSens-1.4.7/LICENSE` & `APIMakeSens-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `APIMakeSens-1.4.7/MakeSens/MakeSens.py` & `APIMakeSens-1.4.8/MakeSens/MakeSens.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,16 @@
             "pm10_1_ae" : "pm10_1_AE",
             "pm10_2_ae" : "pm10_2_AE",
             "pm25_1_ae" : "pm25_1_AE",
             "pm25_2_ae" : "pm25_2_AE",
             "pm1_1_ae" : "pm1_1_AE",
             "pm1_2_ae" : "pm1_2_AE",		
         }, inplace=True)
+
+        dataframe_data = dataframe_data.resample(sample_rate).mean()
         if file_format is not None:
             start_datetime_str = start_datetime.strftime("%Y-%m-%d_%H_%M_%S")
             end_datetime_str = end_datetime.strftime("%Y-%m-%d_%H_%M_%S")
             name = f"{id_device}_{start_datetime_str}_{end_datetime_str}_{sample_rate}"
             __save_data(dataframe_data, name, file_format)
         return dataframe_data
 
@@ -262,15 +264,15 @@
 
     grouped = data.groupby([data.index.date, data.index.hour]).mean()
     heatmap_data = grouped.unstack(level=-1)
     heatmap_data = heatmap_data.iloc[:,::-1]
 
     plt.figure(figsize=(10,8))
     sns.heatmap(heatmap_data.T, cmap=newcmp, norm=norm)
-    plt.ylabel(f'{variable} [{units}]', fontsize=14)
+    plt.ylabel('Horas', fontsize=14)
     plt.xlabel('Estampa temporal', fontsize=14)
     plt.show()
 
 def __load_normalized_color_ranges(variable_name: str) -> list:
     """
     Carga y normaliza los rangos de colores para una variable específica desde 
     un archivo JSON.
```

### Comparing `APIMakeSens-1.4.7/PKG-INFO` & `APIMakeSens-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIMakeSens
-Version: 1.4.7
+Version: 1.4.8
 Summary: MakeSense API
 Home-page: https://github.com/MakeSens-Data/MakeSensAPI_Python
 Author: MakeSens
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `APIMakeSens-1.4.7/setup.py` & `APIMakeSens-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="APIMakeSens",
-    version="1.4.7",
+    version="1.4.8",
     description="MakeSense API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MakeSens-Data/MakeSensAPI_Python",
     author="MakeSens",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
```

