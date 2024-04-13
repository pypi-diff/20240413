# Comparing `tmp/pyweatherfr-4.1.0.tar.gz` & `tmp/pyweatherfr-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.1.0.tar", last modified: Sat Apr 13 13:15:55 2024, max compression
+gzip compressed data, was "pyweatherfr-4.1.1.tar", last modified: Sat Apr 13 13:50:21 2024, max compression
```

## Comparing `pyweatherfr-4.1.0.tar` & `pyweatherfr-4.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.052854 pyweatherfr-4.1.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36532 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:15:28.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.808243 pyweatherfr-4.1.1/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36527 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:50:21.808243 pyweatherfr-4.1.1/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:51.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:50:21.000000 pyweatherfr-4.1.1/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:50:21.812243 pyweatherfr-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:49:44.000000 pyweatherfr-4.1.1/setup.py
```

### Comparing `pyweatherfr-4.1.0/LICENSE.txt` & `pyweatherfr-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.0/PKG-INFO` & `pyweatherfr-4.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.0
+Version: 4.1.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.0/README.md` & `pyweatherfr-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.0/pyweatherfr/args.py` & `pyweatherfr-4.1.1/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.1.1/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,28 @@
     ze_path = os.path.join(
         os.path.expanduser("~"), ".config", DOSSIER_CONFIG_PYWEATHER, ""
     )
     pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
     return ze_path
 
 
+def diff_jour(long,lat):
+    tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
+    if not compute_args().date == None:
+        if not est_format_date(compute_args().date):
+            print(my_colored("erreur : format date invalide, format attendu yyyy-mm-dd", "red"))
+            exit(1)
+        diff = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days +1
+        print_debug(str(diff) + " jours")
+        if diff>=4 or diff<-100:
+            print(my_colored("erreur : date invalide (-100 à +4 jour de la date actuelle)", "red"))
+            exit(1)
+        return diff     
+    return compute_args().jour
+
 def est_format_date(chaine):
     try:
         datetime.datetime.strptime(chaine, '%Y-%m-%d')
         return True
     except ValueError:
         return False
 
@@ -109,46 +123,34 @@
     if compute_args().town:
         ville, dpt, lat, long = obtain_city_data()
     elif compute_args().gps:
         ville, dpt, lat, long = obtain_city_data_from_gps()
     else:
         ville, dpt, lat, long = obtain_city_data_from_ip()
     tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
-    if not compute_args().date == None:
-        if not est_format_date(compute_args().date):
-            print(my_colored("erreur : format date invalide, format attendu yyyy-mm-dd", "red"))
-            exit(1)
-        diff = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days
-        if diff>=4 or diff<100:
-            print(my_colored("erreur : date invalide (-100 à +4 jour de la date actuelle)", "red"))
-            exit(1)    
     if compute_args().pc:
         tz=str(tzlocal.get_localzone())
     if compute_args().utc:
         tz=str(pytz.utc)              
     print_debug(tz)
     if compute_args().now:
         previsions_courantes(ville, dpt, lat, long,tz)
     elif not compute_args().date == None:
         previsions_detaillees(ville, dpt, lat, long,tz)        
-    elif compute_args().jour == 1000:
+    elif diff_jour(long,lat) == 1000:
         previsions_generiques(ville, dpt, lat, long,tz)
     else:
         previsions_detaillees(ville, dpt, lat, long,tz)
 
 
 
 def previsions_detaillees(ville, dpt, lat, long, tz):
 
 
-    if compute_args().date:
-        day = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days
-    else:    
-        day = compute_args().jour
-
+    
     (
         hourly_temperature_2m,
         hourly_apparent_temperature,
         hourly_precipitation,
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
@@ -156,32 +158,33 @@
         current_weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
         cloud_cover,
         alt,
         isday   
-    ) = specific_day(lat, long, day, tz)
-    recap ="Prévisions détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+    ) = specific_day(lat, long, diff_jour(long,lat), tz)
+    recap ="Prévisions détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=diff_jour(long,lat))).strftime(
             "%Y-%m-%d")
     if compute_args().pc:
         recap = recap + " (pc)"
     elif compute_args().utc:
         recap = recap + " (utc.)"        
     else:
         recap = recap + " (loc.)"    
-    if compute_args().jour<0:
-        recap ="Données détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+    if diff_jour(long,lat)<0:
+        recap ="Données détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=diff_jour(long,lat))).strftime(
                 "%Y-%m-%d")        
     print_generic_data_town(ville, dpt, lat, long, alt, recap)
     data = []
+    new_var = diff_jour(long,lat)
     for h in range(0, 24):
         warning = ""
         if (
-            (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+            (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=new_var)).strftime(
             "%Y-%m-%d") == datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%Y-%m-%d")
             and 0 < h - int(datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%H")) <= 1
         ):
             warning = warning + " " + CLOCK
         temp = (
             f"{hourly_temperature_2m[h]:.1f}°C ({hourly_apparent_temperature[h]:.1f}°C)"
         )
@@ -216,15 +219,15 @@
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
-                        + datetime.timedelta(days=compute_args().jour)
+                        + datetime.timedelta(days=new_var)
                         + datetime.timedelta(hours=h),
                         "%Y-%m-%d %H:%M",
                     ),
                     weather,
                     temp,
                     pluie,
                     vent,
@@ -238,15 +241,15 @@
         else:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
-                        + datetime.timedelta(days=compute_args().jour)
+                        + datetime.timedelta(days=new_var)
                         + datetime.timedelta(hours=h),
                         "%Y-%m-%d %H:%M",
                     ),
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
```

### Comparing `pyweatherfr-4.1.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.1.1/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.0
+Version: 4.1.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.0/setup.py` & `pyweatherfr-4.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.1.0",
+    version="4.1.1",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

