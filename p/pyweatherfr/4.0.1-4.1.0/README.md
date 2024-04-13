# Comparing `tmp/pyweatherfr-4.0.1.tar.gz` & `tmp/pyweatherfr-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.0.1.tar", last modified: Fri Apr 12 19:20:44 2024, max compression
+gzip compressed data, was "pyweatherfr-4.1.0.tar", last modified: Sat Apr 13 13:15:55 2024, max compression
```

## Comparing `pyweatherfr-4.0.1.tar` & `pyweatherfr-4.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.052854 pyweatherfr-4.1.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36532 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:15:28.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 13:15:55.000000 pyweatherfr-4.1.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:15:55.056854 pyweatherfr-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:15:19.000000 pyweatherfr-4.1.0/setup.py
```

### Comparing `pyweatherfr-4.0.1/LICENSE.txt` & `pyweatherfr-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.0.1/PKG-INFO` & `pyweatherfr-4.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.0.1
+Version: 4.1.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -19,9 +19,12 @@
 Requires-Dist: termcolor
 Requires-Dist: colorama
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
 Requires-Dist: retry_requests
 Requires-Dist: geopy
 Requires-Dist: numpy
+Requires-Dist: timezonefinder
+Requires-Dist: tzlocal
+Requires-Dist: pytz
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-4.0.1/README.md` & `pyweatherfr-4.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,24 +29,29 @@
 
 attention : le paramètre peut être compris entre - 100 et 3
 
 pyweatherfr \[TOWN\] -p [INT]
 
 exemple : ``pyweatherfr Grenoble -p 10`` affiche les données météo détaillées pour Grenoble de J-10 à J-1
 
+pyweatherfr \[TOWN\] -d [STR]
+
+exemple : ``pyweatherfr Grenoble -d 2024-03-30`` affiche les données météo détaillées pour Grenoble au 30/03/2024
 
 
 ## Autres options
 
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
+  - ``--utc``    utilise l'heure utc dans les previsions au lieu de l'heure locale de la ville
+  - ``--pc``    utilise l'heure du pc dans les previsions au lieu de l'heure locale de la ville
   
 # Démo
 
 ![image](./demo_01.png)
 
 ![image](./demo_02.png)
```

### Comparing `pyweatherfr-4.0.1/pyweatherfr/args.py` & `pyweatherfr-4.1.0/pyweatherfr/args.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,31 +43,42 @@
     my_group.add_argument(
         "town",
         metavar="VILLE",
         type=str,
         nargs="?",
         help="affichage des données météo par nom de ville ou code postal -si absent, la VILLE est déduite de l'ip-",
     )
-    my_parser.add_argument(
+    my_2group = my_parser.add_mutually_exclusive_group()
+    my_2group.add_argument(
         "-n",
         "--now",
         action="store_true",
         help="affichage des données météo détaillées actuelles",
     )
-    my_parser.add_argument(
+    my_2group.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
         default=1000,
+        nargs='?',
+        const=0,        
         choices=range(-101, 4),
         help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ..., -1 pour J-1, ...)",
     )
-    my_parser.add_argument(
+    my_2group.add_argument(
+        "-d",
+        "--date",
+        metavar="DATE",
+        action="store",
+        type=str,      
+        help="affichage des données météo détaillées pour [DAY] au format yyyy-mm-dd",
+    )    
+    my_2group.add_argument(
         "-p",
         "--past",
         metavar="JOUR PASSE",
         action="store",
         type=int,
         default=0,
         choices=range(1, 101),
@@ -83,14 +94,25 @@
         help="affichage des données météo par coordonnées GPS",
     )      
     my_parser.add_argument(
         "--nocolor",
         action="store_true",
         help="désactiver couleur et emojis en sortie -à utiliser en cas de problème d'affichage-",
     )
+    group = my_parser.add_mutually_exclusive_group()
+    group.add_argument(
+        "--pc",
+        action="store_true",
+        help="utilise l'heure locale du PC indépendamment de la ville cherchée",
+    )
+    group.add_argument(
+        "--utc",
+        action="store_true",
+        help="utilise l'heure UTC",
+    )          
     my_parser.add_argument(
         "-c",
         "--condensate",
         action="store_true",
         help="condenser la sortie",
     )
     my_parser.add_argument(
```

### Comparing `pyweatherfr-4.0.1/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.1.0/pyweatherfr/pyweatherfr.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 import openmeteo_requests
 import requests_cache
 import columnar
 import termcolor
 import pathlib
 import retry_requests
 import geopy
+import timezonefinder
+import pytz
+import tzlocal
 
 
 DOSSIER_CONFIG_PYWEATHER = "pyweatherfr"
 
 SUN = "\U0001F31E"
 MI_SUN = "\U0001F324"
 CLOUD = "\U0001F325"
+NIGHT_CLOUD = "\U0001f319"
 MI_CLOUD_RAIN = "\U0001F326"
 RAIN = "\U0001F327"
 SNOW = "\U0001F328"
-NIGHT_CLEAR = "\U0001F319"
+NIGHT_CLEAR = "\U0001f319"
 ORAGE = "\U0001F329"
 ORAGE_PLUIE = "\U0001F329" + " " + "\U0001F327"
 FOG = "\U0001F32B"
 DROPLET = "\U0001F4A7"
 FLOCON = "\U00002744"
 WIND = "\U0001F6A9"
 COLD = "\U0001F9CA"
@@ -52,14 +56,15 @@
 FLECHE_SW = "\U0000FE0F"
 FLECHE_S = "\U0000FE0F"
 FLECHE_SE = "\U0000FE0F"
 FLECHE_E = "\U0000FE0F"
 FLECHE_NE = "\U0000FE0F"
 ELEPHANT = "\U0001F418"
 PLUME = "\U0001FAB6"
+PC ="\U0001f4bb"
 WARNING_WARM=30
 WARNING_FROID=0
 WARNING_SNOW=0.1
 WARNING_RAIN=0.1
 WARNING_WIND=30
 WARNING_WIND_GUST=50
 WARNING_HP=1030
@@ -88,60 +93,101 @@
     ze_path = os.path.join(
         os.path.expanduser("~"), ".config", DOSSIER_CONFIG_PYWEATHER, ""
     )
     pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
     return ze_path
 
 
+def est_format_date(chaine):
+    try:
+        datetime.datetime.strptime(chaine, '%Y-%m-%d')
+        return True
+    except ValueError:
+        return False
+
 def find():
 
     if compute_args().town:
         ville, dpt, lat, long = obtain_city_data()
     elif compute_args().gps:
         ville, dpt, lat, long = obtain_city_data_from_gps()
     else:
         ville, dpt, lat, long = obtain_city_data_from_ip()
-
+    tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
+    if not compute_args().date == None:
+        if not est_format_date(compute_args().date):
+            print(my_colored("erreur : format date invalide, format attendu yyyy-mm-dd", "red"))
+            exit(1)
+        diff = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days
+        if diff>=4 or diff<100:
+            print(my_colored("erreur : date invalide (-100 à +4 jour de la date actuelle)", "red"))
+            exit(1)    
+    if compute_args().pc:
+        tz=str(tzlocal.get_localzone())
+    if compute_args().utc:
+        tz=str(pytz.utc)              
+    print_debug(tz)
     if compute_args().now:
-        previsions_courantes(ville, dpt, lat, long)
+        previsions_courantes(ville, dpt, lat, long,tz)
+    elif not compute_args().date == None:
+        previsions_detaillees(ville, dpt, lat, long,tz)        
     elif compute_args().jour == 1000:
-        previsions_generiques(ville, dpt, lat, long)
+        previsions_generiques(ville, dpt, lat, long,tz)
     else:
-        previsions_detaillees(ville, dpt, lat, long)
+        previsions_detaillees(ville, dpt, lat, long,tz)
 
 
 
-def previsions_detaillees(ville, dpt, lat, long):
-    print_generic_data_town(ville, dpt, lat, long)
+def previsions_detaillees(ville, dpt, lat, long, tz):
 
 
+    if compute_args().date:
+        day = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days
+    else:    
+        day = compute_args().jour
+
     (
         hourly_temperature_2m,
         hourly_apparent_temperature,
         hourly_precipitation,
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         current_weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
-        cloud_cover       
-    ) = specific_day(lat, long, compute_args().jour)
+        cloud_cover,
+        alt,
+        isday   
+    ) = specific_day(lat, long, day, tz)
+    recap ="Prévisions détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+            "%Y-%m-%d")
+    if compute_args().pc:
+        recap = recap + " (pc)"
+    elif compute_args().utc:
+        recap = recap + " (utc.)"        
+    else:
+        recap = recap + " (loc.)"    
+    if compute_args().jour<0:
+        recap ="Données détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+                "%Y-%m-%d")        
+    print_generic_data_town(ville, dpt, lat, long, alt, recap)
     data = []
     for h in range(0, 24):
         warning = ""
         if (
-            compute_args().jour == 0
-            and 0 < h - int(datetime.datetime.now().strftime("%H")) <= 1
+            (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=compute_args().jour)).strftime(
+            "%Y-%m-%d") == datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%Y-%m-%d")
+            and 0 < h - int(datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%H")) <= 1
         ):
             warning = warning + " " + CLOCK
         temp = (
-            f"{hourly_temperature_2m[h]:.1f}° ({hourly_apparent_temperature[h]:.1f}°)"
+            f"{hourly_temperature_2m[h]:.1f}°C ({hourly_apparent_temperature[h]:.1f}°C)"
         )
         if hourly_temperature_2m[h] <= WARNING_FROID or hourly_apparent_temperature[h] <= WARNING_FROID:
             warning = warning + " " + COLD
         if hourly_temperature_2m[h] >= WARNING_WARM or hourly_apparent_temperature[h] >= WARNING_WARM:
             warning = warning + " " + WARM
         pluie = f"{hourly_precipitation[h]:.1f}mm"
         if snowfall[h] >= WARNING_SNOW:
@@ -159,23 +205,23 @@
             warning = warning + " " + WIND
 
         pression = f"{surface_pressure[h]:.1f}Hpa"
         if surface_pressure[h] >= WARNING_HP:
             warning = warning + " " + ELEPHANT
         if surface_pressure[h] <= WARNING_BP:
             warning = warning + " " + PLUME
-        weather, emojiweather = traduction(current_weather_code[h])
+        weather, emojiweather = traduction(current_weather_code[h],isday[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
         couv_nuage = f" {cloud_cover[h]:.0f}%"        
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
-                        datetime.datetime.now().replace(
+                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
                         + datetime.timedelta(days=compute_args().jour)
                         + datetime.timedelta(hours=h),
                         "%Y-%m-%d %H:%M",
                     ),
                     weather,
@@ -189,15 +235,15 @@
                     couv_nuage,
                 ]
             )
         else:
             data.append(
                 [
                     datetime.datetime.strftime(
-                        datetime.datetime.now().replace(
+                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
                         + datetime.timedelta(days=compute_args().jour)
                         + datetime.timedelta(hours=h),
                         "%Y-%m-%d %H:%M",
                     ),
                     emojiweather + " " + weather,
@@ -289,22 +335,26 @@
             direction_vent_degres <= 360 - 22.5 - 270
             and direction_vent_degres > 360 - 22.5 - 315
         ):
         direction = "NE"
     return direction
 
 
-def traduction(current_weather_code):
+def traduction(current_weather_code,jour):
     if (
         current_weather_code == 0
         or current_weather_code == 1
         or current_weather_code == 2
     ):
-        return ["ciel clair", SUN]
+        if jour==0:
+            return ["nuit claire ", NIGHT_CLEAR]
+        return ["ciel clair ", SUN]
     if current_weather_code >= 3 and current_weather_code <= 12:
+        if jour==0:
+            return ["nuageux ", NIGHT_CLOUD]        
         return ["nuageux", CLOUD]
     if current_weather_code >= 13 and current_weather_code <= 19:
         return ["pluie proche", RAIN]
     if current_weather_code >= 20 and current_weather_code <= 29:
         return ["fin de pluie", RAIN]
     if current_weather_code >= 30 and current_weather_code <= 39:
         return ["tempete de poussière, sable ou neige", FOG]
@@ -316,39 +366,50 @@
         return ["pluie", RAIN]
     if current_weather_code >= 70 and current_weather_code <= 79:
         return ["neige", SNOW]
     if current_weather_code >= 80 and current_weather_code <= 99:
         return ["averse / orage", ORAGE_PLUIE]
 
 
-def previsions_courantes(ville, dpt, lat, long):
-    print_generic_data_town(ville, dpt, lat, long)
+def previsions_courantes(ville, dpt, lat, long, tz):
+    
 
     (
         current_temperature_2m,
         current_apparent_temperature,
         current_relative_humidity_2m,
         current_precipitation,
         current_surface_pressure,
         current_wind_speed_10m,
         current_wind_gusts_10m,
         current_wind_direction_10m,
         current_weather_code,
-        snowfall
-
-    ) = current(lat, long)
-    current_weather, emojiweather = traduction(current_weather_code)
+        snowfall,
+        alt,
+        time,
+        isday
+
+    ) = current(lat, long, tz)
+    recap = "Données courantes mesurées à " + datetime.datetime.fromtimestamp(time,tz=pytz.timezone(tz)).strftime('%Y-%m-%d %H:%M') 
+    if compute_args().pc:
+        recap = recap + " (pc)"
+    elif compute_args().utc:
+        recap = recap + " (utc.)"        
+    else:
+        recap = recap + " (loc.)"
+    print_generic_data_town(ville, dpt, lat, long, alt, recap)
+    current_weather, emojiweather = traduction(current_weather_code,isday)
     data = []
     direction = calculer_direction(current_wind_direction_10m)
 
     if compute_args().nocolor:
         data.append(
             [
                 "température (ressentie)",
-                f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",
+                f"{current_temperature_2m:.1f}°C ({current_apparent_temperature:.1f}°C)",
             ]
         )
         data.append(["humidité", f"{current_relative_humidity_2m:.1f}%"])
         data.append(["precipitation", f"{current_precipitation:.1f}mm"])
         data.append(["pression", f"{current_surface_pressure:.1f}Hp"])
         data.append(
             [
@@ -360,36 +421,36 @@
         data.append(["temps", current_weather])
 
     else:
         if current_temperature_2m >= WARNING_WARM or current_apparent_temperature >= WARNING_WARM:
             data.append(
                 [
                     "température (ressentie)",
-                    f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",
+                    f"{current_temperature_2m:.1f}°C ({current_apparent_temperature:.1f}°C)",
                     WARM,
                 ]
             )
         else:
             data.append(
                 [
                     "température",
-                    f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",
+                    f"{current_temperature_2m:.1f}°C ({current_apparent_temperature:.1f}°C)",
                     "",
                 ]
             )
         if current_relative_humidity_2m >= WARNING_HUMIDITY:
             data.append(["humidité", f"{current_relative_humidity_2m:.1f}%", DROPLET])
         else:
             data.append(["humidité", f"{current_relative_humidity_2m:.1f}%", ""])
         if snowfall >= WARNING_SNOW:
             data.append(["precipitation", f"{current_precipitation:.1f}mm", SNOW])
         elif current_precipitation>=WARNING_RAIN:
             data.append(["precipitation", f"{current_precipitation:.1f}mm", RAIN])
         else:
-            data.append(["precipitation", f"{current_precipitation:.1f}mm", RAIN])
+            data.append(["precipitation", f"{current_precipitation:.1f}mm", ""])
         if current_surface_pressure >= WARNING_HP:
             data.append(["pression", f"{current_surface_pressure:.1f}Hp", ELEPHANT])
         elif current_surface_pressure <= WARNING_BP:
             data.append(["pression", f"{current_surface_pressure:.1f}Hp", PLUME])
         else:
             data.append(["pression", f"{current_surface_pressure:.1f}Hp", ""])
         if current_wind_speed_10m >= WARNING_WIND or current_wind_gusts_10m >= WARNING_WIND_GUST:
@@ -415,75 +476,87 @@
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         print("")
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
     print(table)
 
 
-def previsions_generiques(ville, dpt, lat, long):
-
-    print_generic_data_town(ville, dpt, lat, long)
-
+def previsions_generiques(ville, dpt, lat, long, tz):
 
+    
     (
         daily_temperature_2m_min,
         daily_temperature_2m_max,
         daily_apparent_temperature_min,
         daily_apparent_temperature_max,
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
         daily_wind_direction_10m_dominant,
         weather_code,
         snowfall,
         precipitation_hours,
         sunshine_duration,
-    ) = resume(lat, long)
-    data2 = []
+        alt,
+        debut,
+        fin
+    ) = resume(lat, long, tz)
+    datetime.datetime.fromtimestamp(debut,tz=pytz.timezone(tz)).strftime('%Y-%m-%d')
+    recap = "Prévisions génériques du " + datetime.datetime.fromtimestamp(debut,tz=pytz.timezone(tz)).strftime('%Y-%m-%d') + " au " + (datetime.datetime.fromtimestamp(fin,tz=pytz.timezone(tz))+ datetime.timedelta(days=-1)).strftime('%Y-%m-%d')
+    if compute_args().past!=0:
+        recap = "Données génériques du " + datetime.datetime.fromtimestamp(debut,tz=pytz.timezone(tz)).strftime('%Y-%m-%d') + " au " + (datetime.datetime.fromtimestamp(fin,tz=pytz.timezone(tz))+ datetime.timedelta(days=-1)).strftime('%Y-%m-%d')
+    if compute_args().pc:
+        recap = recap + " (pc)"
+    elif compute_args().utc:
+        recap = recap + " (utc.)"        
+    else:
+        recap = recap + " (loc.)"  
+    print_generic_data_town(ville, dpt, lat, long, alt, recap)
+    data = []
     fin = 3
     if compute_args().past!=0:
         fin=-1
     for i in range(0,len(daily_precipitation_sum)):
         warning = ""
         pluie = f"{daily_precipitation_sum[i]:.1f}mm"
         if snowfall[i] >= WARNING_SNOW:
             warning = warning + " " + SNOW
         elif daily_precipitation_sum[i] >= WARNING_RAIN:
             warning = warning + " " + RAIN
-        temp = f"{daily_temperature_2m_min[i]:.1f}° ({daily_apparent_temperature_min[i]:.1f}°) -> {daily_temperature_2m_max[i]:.1f}° ({daily_apparent_temperature_max[i]:.1f}°)"
+        temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
         if (
             daily_temperature_2m_min[i] <= WARNING_FROID
             or daily_apparent_temperature_min[i] <= WARNING_FROID
             or daily_temperature_2m_max[i] <= WARNING_FROID
             or daily_apparent_temperature_max[i] <= WARNING_FROID
         ):
             warning = warning + " " + COLD
         if (
             daily_temperature_2m_min[i] >= WARNING_WARM
             or daily_apparent_temperature_min[i] >= WARNING_WARM
             or daily_temperature_2m_max[i] >= WARNING_WARM
             or daily_apparent_temperature_max[i] >= WARNING_WARM
         ):
             warning = warning + " " + WARM
-        weather, emojiweather = traduction(weather_code[i])
+        weather, emojiweather = traduction(weather_code[i],1)
 
         vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
         direction=calculer_direction(daily_wind_direction_10m_dominant[i])
 
 
         vent = vent
         if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
             warning = warning + " " + WIND
         duree_pluie = f"{precipitation_hours[i]:.0f}h"
         duree_soleil = f"{sunshine_duration[i]/3600:.1f}h"
         if compute_args().nocolor:
-            data2.append(
+            data.append(
                 [
                     datetime.datetime.strftime(
-                        datetime.datetime.now().replace(
+                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
                         + datetime.timedelta(hours=24 * i),
                         "%Y-%m-%d",
                     ),
                     weather,
                     temp,
@@ -501,18 +574,18 @@
                 "précipitations",
                 "vent (rafales)",
                 "direction",
                 "durée pluie",
                 "durée soleil"
             ]
         else:
-            data2.append(
+            data.append(
                 [
                     datetime.datetime.strftime(
-                        datetime.datetime.now().replace(
+                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
                         + datetime.timedelta(hours=24 * i)
                         + datetime.timedelta(days=-1*compute_args().past),
                         "%Y-%m-%d",
                     ),
                     emojiweather + " " + weather,
@@ -533,46 +606,47 @@
                 "vent (rafales)",
                 "direction vent",
                 "durée pluie",
                 "durée soleil",
                 "warning",
             ]
 
-    if data2 != []:
+    if data != []:
         if compute_args().condensate:
-            table = columnar.columnar(data2, no_borders=True, wrap_max=0)
+            table = columnar.columnar(data, no_borders=True, wrap_max=0)
         else:
             print("")
-            table = columnar.columnar(data2, headers, no_borders=False, wrap_max=0)
+            table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
 
 
-def print_generic_data_town(ville, dpt, lat, long):
+def print_generic_data_town(ville, dpt, lat, long, alt, recap):
     print("")
 
     data = []
     if compute_args().nocolor:
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
             print_debug("pas de data pour ville/dpt/cp")
         elif dpt is None or dpt == "":
-            data.append(ville)
+            data.append([ville])
         else:    
-            data.append(ville + " (" + dpt + ")")
-        data.append(f"lat.:  {float(lat):.4f}° / long.: {float(long):.4f}° ")
-        data.append([datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
+            data.append([ville + " (" + dpt + ")"])
+        data.append([f"lat.:  {float(lat):.4f}° / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m "])
+        #data.append([datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
+        data.append([recap])
     else:
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
             print_debug("pas de data pour ville/dpt/cp")
         elif dpt is None or dpt == "":
             data.append([HOME, ville])
         else:    
             data.append([HOME, ville + " (" + dpt + ")"])
-        data.append([BOUSSOLE, f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° "])
-        data.append([CLOCK, datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
-
+        data.append([BOUSSOLE, f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m "])
+        #data.append([CLOCK, datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
+        data.append([PC,recap])
     if compute_args().condensate:
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
 
     print(table)
 
@@ -604,21 +678,22 @@
 def obtain_city_data_from_ip():
 
     with urllib.request.urlopen("https://geolocation-db.com/json") as url:
         print_debug(
             "recherche de la localisation depuis https://geolocation-db.com/json"
         )
         data = json.loads(url.read().decode())
-        print_debug(str(data))
+        print_debug(str(json.dumps(data, indent=4,ensure_ascii=False)))
         ville = data["city"]
         lat = str(data["latitude"])
         long = str(data["longitude"])
-        dpt = str(data["postal"])
+        dpt = str(data["state"])
         return ville, dpt, lat, long 
-    
+
+
 
 
 def obtain_city_data_from_gps():
     print_debug(
         "COORDONNEES_GPS :"
         + "latitude="
         + str(compute_args().gps[0])
@@ -642,25 +717,29 @@
     
     # Affichage des informations de localisation
     choix = []
     if locations == None:
         print(my_colored("erreur : aucune ville trouvée", "red")) 
         exit(1)    
     for location in locations:
-        print_debug(str(location.raw))
-        ville = clean_string(location.raw.get("address").get("village"))
+        print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
+        ville = clean_string(location.raw.get("address").get("island"))
+        if ville == None or (location.raw.get("address").get("village") != None and clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower())):
+            ville = location.raw.get("address").get("village")
         if ville == None or (location.raw.get("address").get("municipality") != None and clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower())):
             ville = location.raw.get("address").get("municipality")
         if ville == None or (location.raw.get("address").get("town") != None and clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower())):
             ville = location.raw.get("address").get("town")               
         if ville == None or (location.raw.get("address").get("city") != None and clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower())):
             ville = location.raw.get("address").get("city")
         dpt = location.raw.get("address").get("county")
         if dpt ==None:
-            dpt=""
+            dpt=location.raw.get("address").get("state")
+        if dpt ==None:
+            dpt= location.raw.get("address").get("postcode")  
         cp = location.raw.get("address").get("postcode")
         if cp == None:
             cp = ""
         lat = location.raw.get("lat")
         long = location.raw.get("lon")
         print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
         if clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower(): 
@@ -672,19 +751,23 @@
         dpt = choice[2]
         lat = choice[3]
         long = choice[4]
         return ville, dpt, lat, long    
     if len(choix)==0:
         print(my_colored("erreur : aucune ville trouvée", "red")) 
         exit(1)
-    i=0    
-    for choice in choix:
-        i=i+1
-        print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
-    toto = input("Quelle ville? ")
+    while True:    
+        i=0    
+        for choice in choix:
+            i=i+1
+            print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
+        toto = input("Quelle ville? ")
+        if toto.isnumeric() and 1 <= int(toto) <= len(choix):
+            break
+        print(my_colored("erreur : choix incorrect", "red"))       
     choice = choix[int(toto)-1]
     ville = choice[1]
     dpt = choice[2]
     lat = choice[3]
     long = choice[4]
     return ville, dpt, lat, long
 
@@ -698,24 +781,24 @@
 def print_debug(message):
     if compute_args().verbose:
         print("debug : " + message)
 
 
 
 
-def resume(latitude, longitude):
+def resume(latitude, longitude, tz):
     retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     date_debut = (datetime.datetime.now() + datetime.timedelta(days=-1*compute_args().past)).strftime("%Y-%m-%d")
     date_fin = (datetime.datetime.now() + datetime.timedelta(days=3)).strftime("%Y-%m-%d")
     if compute_args().past!=0:
         date_fin = (datetime.datetime.now() + datetime.timedelta(days=-1)).strftime("%Y-%m-%d")    
     params = {
-        "timezone": "Europe/Paris",
+        "timezone": tz,
         "start_date": date_debut,
 	    "end_date": date_fin,
         "latitude": latitude,
         "longitude": longitude,
         "daily": [
             "temperature_2m_max",
             "temperature_2m_min",
@@ -743,51 +826,58 @@
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
     daily_wind_gusts_10m_max = daily.Variables(6).ValuesAsNumpy()
     daily_wind_direction_10m_dominant = daily.Variables(7).ValuesAsNumpy()
     weather_code = daily.Variables(8).ValuesAsNumpy()
     snowfall = daily.Variables(9).ValuesAsNumpy()
     precipitation_hours= daily.Variables(10).ValuesAsNumpy()
     sunshine_duration= daily.Variables(11).ValuesAsNumpy()
+    alt= response.Elevation()
+    debut=daily.Time()
+    fin=(daily.TimeEnd())
     return (
         daily_temperature_2m_min,
         daily_temperature_2m_max,
         daily_apparent_temperature_min,
         daily_apparent_temperature_max,
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
         daily_wind_direction_10m_dominant,
         weather_code,
         snowfall,
         precipitation_hours,
-        sunshine_duration
+        sunshine_duration,
+        alt,
+        debut,
+        fin
     )
 
 
-def specific_day(latitude, longitude, day):
+def specific_day(latitude, longitude, day, tz):
     retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
-        "timezone": "Europe/Paris",
+        "timezone": tz,
         "latitude": latitude,
         "longitude": longitude,
         "hourly": [
             "temperature_2m",
             "apparent_temperature",
             "precipitation",
             "wind_speed_10m",
             "wind_gusts_10m",
             "wind_direction_10m",
             "pressure_msl",
             "weather_code",
             "snowfall",
             "relative_humidity_2m",
             "sunshine_duration",
-            "cloud_cover" 
+            "cloud_cover",
+            "is_day"
         ],
         "start_date": (datetime.datetime.now() + datetime.timedelta(days=day)).strftime(
             "%Y-%m-%d"
         ),
         "end_date": (
             datetime.datetime.now() + datetime.timedelta(days=day + 1)
         ).strftime("%Y-%m-%d"),
@@ -804,27 +894,31 @@
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
     surface_pressure = hourly.Variables(6).ValuesAsNumpy()
     weather_code = hourly.Variables(7).ValuesAsNumpy()
     snowfall = hourly.Variables(8).ValuesAsNumpy()
     relative_humidity_2m = hourly.Variables(9).ValuesAsNumpy()
     sunshine_duration = hourly.Variables(10).ValuesAsNumpy()
     cloud_cover = hourly.Variables(11).ValuesAsNumpy()
+    alt= response.Elevation()
+    isday= hourly.Variables(12).ValuesAsNumpy()
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
-        cloud_cover
+        cloud_cover,
+        alt,
+        isday
                 )
 
 def cache_session():
     if compute_args().nocache:
         directory = get_user_config_directory_pyweather()
         file_path = os.path.join(directory, ".cache.sqlite")
         if os.path.exists(file_path):
@@ -833,34 +927,36 @@
         else:
             print_debug("Le cache n'existe pas.")
     return requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
 
 
-def current(latitude, longitude):
+def current(latitude, longitude, tz):
     retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
 
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "latitude": latitude,
         "longitude": longitude,
+        "timezone": tz,
         "current": [
             "temperature_2m",
             "relative_humidity_2m",
             "apparent_temperature",
             "precipitation",
             "rain",
             "snowfall",
             "weather_code",
             "pressure_msl",
             "wind_speed_10m",
             "wind_direction_10m",
             "wind_gusts_10m",
+            "is_day"
         ],
     }
     print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
 
     response = responses[0]
 
@@ -871,26 +967,32 @@
     current_precipitation = current.Variables(4).Value()
     snowfall=current.Variables(5).Value()
     current_weather_code = current.Variables(6).Value()
     current_surface_pressure = current.Variables(7).Value()
     current_wind_speed_10m = current.Variables(8).Value()
     current_wind_direction_10m = current.Variables(9).Value()
     current_wind_gusts_10m = current.Variables(10).Value()
+    isday= current.Variables(11).Value()
+    altitude=response.Elevation()
+    time=int(response.Current().Time())
 
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
-        snowfall
+        snowfall,
+        altitude,
+        time,
+        isday
     )
 
 def clean_string(mystring):
     if mystring is None:
         return None
     retour =""
     nfkd_form = unicodedata.normalize('NFKD', mystring)
```

### Comparing `pyweatherfr-4.0.1/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.1.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.0.1
+Version: 4.1.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -19,9 +19,12 @@
 Requires-Dist: termcolor
 Requires-Dist: colorama
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
 Requires-Dist: retry_requests
 Requires-Dist: geopy
 Requires-Dist: numpy
+Requires-Dist: timezonefinder
+Requires-Dist: tzlocal
+Requires-Dist: pytz
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-4.0.1/setup.py` & `pyweatherfr-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.0.1",
+    version="4.1.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
-    install_requires=["columnar","termcolor", "colorama","openmeteo_requests","requests_cache","retry_requests","geopy","numpy"],
+    install_requires=["columnar","termcolor", "colorama","openmeteo_requests","requests_cache","retry_requests","geopy","numpy","timezonefinder","tzlocal","pytz"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "pyweatherfr=pyweatherfr.__init__:pyweatherfr"
         ],
     },
     classifiers=[
```

