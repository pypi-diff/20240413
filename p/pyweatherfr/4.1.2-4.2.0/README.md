# Comparing `tmp/pyweatherfr-4.1.2.tar.gz` & `tmp/pyweatherfr-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.1.2.tar", last modified: Sat Apr 13 13:58:55 2024, max compression
+gzip compressed data, was "pyweatherfr-4.2.0.tar", last modified: Sat Apr 13 15:46:50 2024, max compression
```

## Comparing `pyweatherfr-4.1.2.tar` & `pyweatherfr-4.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36627 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:27.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:58:55.000000 pyweatherfr-4.1.2/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:58:55.234347 pyweatherfr-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:58:22.000000 pyweatherfr-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36797 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:46:18.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/setup.py
```

### Comparing `pyweatherfr-4.1.2/LICENSE.txt` & `pyweatherfr-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.2/PKG-INFO` & `pyweatherfr-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.2
+Version: 4.2.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.2/README.md` & `pyweatherfr-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.2/pyweatherfr/args.py` & `pyweatherfr-4.2.0/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.1.2/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.2.0/pyweatherfr/pyweatherfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         current_weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
-        cloud_cover,
+        shortwave_radiation,
         alt,
         isday   
     ) = specific_day(lat, long, diff_jour(long,lat), tz)
     recap ="Prévisions détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=diff_jour(long,lat))).strftime(
             "%Y-%m-%d")
     if compute_args().pc:
         recap = recap + " (pc)"
@@ -211,15 +211,15 @@
         if surface_pressure[h] >= WARNING_HP:
             warning = warning + " " + ELEPHANT
         if surface_pressure[h] <= WARNING_BP:
             warning = warning + " " + PLUME
         weather, emojiweather = traduction(current_weather_code[h],isday[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
-        couv_nuage = f" {cloud_cover[h]:.0f}%"        
+        rayonnement = f" {shortwave_radiation[h]:.0f}W/m"        
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -230,16 +230,15 @@
                     weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
-                    duree_soleil,
-                    couv_nuage,
+                    rayonnement,
                 ]
             )
         else:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now(tz=pytz.timezone(tz)).replace(
@@ -252,45 +251,42 @@
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
-                    duree_soleil,
-                    couv_nuage,
+                    rayonnement,
                     warning,
                 ]
             )
 
     if compute_args().nocolor:
         headers = [
             "date",
             "temps",
             "température (ressentie)",
             "précipitations",
             "vent (rafales)",
             "direction vent",
             "pression",
             "humidité",
-            "durée soleil",
-            "couverture nuage"            
+            "rayonnement"            
         ]
     else:
         headers = [
             "date",
             "temps",
             "température (ressentie)",
             "précipitations",
             "vent (rafales)",
             "direction vent",
             "pression",
             "humidité",
-            "durée soleil",
-            "couverture nuage",            
+            "rayonnement",            
             "warnings",
         ]
 
     if data != []:
         if compute_args().condensate:
             table = columnar.columnar(data, no_borders=True, wrap_max=0)
         else:
@@ -385,15 +381,16 @@
         current_wind_speed_10m,
         current_wind_gusts_10m,
         current_wind_direction_10m,
         current_weather_code,
         snowfall,
         alt,
         time,
-        isday
+        isday,
+        w_soleil
 
     ) = current(lat, long, tz)
     recap = "Données courantes mesurées à " + datetime.datetime.fromtimestamp(time,tz=pytz.timezone(tz)).strftime('%Y-%m-%d %H:%M') 
     if compute_args().pc:
         recap = recap + " (pc)"
     elif compute_args().utc:
         recap = recap + " (utc.)"        
@@ -417,14 +414,15 @@
         data.append(
             [
                 "vent",
                 f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                 + direction,
             ]
         )
+        data.append(["rayonnement", f"{w_soleil:.0f}W/m"])
         data.append(["temps", current_weather])
 
     else:
         if current_temperature_2m >= WARNING_WARM or current_apparent_temperature >= WARNING_WARM:
             data.append(
                 [
                     "température (ressentie)",
@@ -470,14 +468,15 @@
                 [
                     "vent",
                     f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                     + direction,
                     "",
                 ]
             )
+        data.append(["rayonnement", f"{w_soleil:.0f}W/m",""])    
         data.append(["temps", emojiweather + " " + current_weather, ""])
     if compute_args().condensate:
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         print("")
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
     print(table)
@@ -871,15 +870,15 @@
             "wind_gusts_10m",
             "wind_direction_10m",
             "pressure_msl",
             "weather_code",
             "snowfall",
             "relative_humidity_2m",
             "sunshine_duration",
-            "cloud_cover",
+            "shortwave_radiation",
             "is_day"
         ],
         "start_date": (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=day)).strftime(
             "%Y-%m-%d"
         ),
         "end_date": (
             datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=day + 1)
@@ -896,30 +895,30 @@
     hourly_wind_gusts_10m = hourly.Variables(4).ValuesAsNumpy()
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
     surface_pressure = hourly.Variables(6).ValuesAsNumpy()
     weather_code = hourly.Variables(7).ValuesAsNumpy()
     snowfall = hourly.Variables(8).ValuesAsNumpy()
     relative_humidity_2m = hourly.Variables(9).ValuesAsNumpy()
     sunshine_duration = hourly.Variables(10).ValuesAsNumpy()
-    cloud_cover = hourly.Variables(11).ValuesAsNumpy()
+    shortwave_radiation = hourly.Variables(11).ValuesAsNumpy()
     alt= response.Elevation()
     isday= hourly.Variables(12).ValuesAsNumpy()
     return (
         hourly_temperature_2m,
         hourly_apparent_temperature,
         hourly_precipitation,
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
-        cloud_cover,
+        shortwave_radiation,
         alt,
         isday
                 )
 
 def cache_session():
     if compute_args().nocache:
         directory = get_user_config_directory_pyweather()
@@ -951,15 +950,16 @@
             "rain",
             "snowfall",
             "weather_code",
             "pressure_msl",
             "wind_speed_10m",
             "wind_direction_10m",
             "wind_gusts_10m",
-            "is_day"
+            "is_day",
+            "shortwave_radiation"
         ],
     }
     print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
 
     response = responses[0]
 
@@ -973,29 +973,31 @@
     current_surface_pressure = current.Variables(7).Value()
     current_wind_speed_10m = current.Variables(8).Value()
     current_wind_direction_10m = current.Variables(9).Value()
     current_wind_gusts_10m = current.Variables(10).Value()
     isday= current.Variables(11).Value()
     altitude=response.Elevation()
     time=int(response.Current().Time())
+    shortwave_radiation=current.Variables(12).Value()
 
     return (
         current_temperature_2m,
         current_apparent_temperature,
         current_relative_humidity_2m,
         current_precipitation,
         current_surface_pressure,
         current_wind_speed_10m,
         current_wind_gusts_10m,
         current_wind_direction_10m,
         current_weather_code,
         snowfall,
         altitude,
         time,
-        isday
+        isday,
+        shortwave_radiation
     )
 
 def clean_string(mystring):
     if mystring is None:
         return None
     retour =""
     nfkd_form = unicodedata.normalize('NFKD', mystring)
```

### Comparing `pyweatherfr-4.1.2/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.2.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.1.2
+Version: 4.2.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.1.2/setup.py` & `pyweatherfr-4.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.1.2",
+    version="4.2.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

