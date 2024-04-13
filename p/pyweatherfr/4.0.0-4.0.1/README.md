# Comparing `tmp/pyweatherfr-4.0.0.tar.gz` & `tmp/pyweatherfr-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.0.0.tar", last modified: Thu Apr 11 04:51:14 2024, max compression
+gzip compressed data, was "pyweatherfr-4.0.1.tar", last modified: Fri Apr 12 19:20:44 2024, max compression
```

## Comparing `pyweatherfr-4.0.0.tar` & `pyweatherfr-4.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:20:44.000000 pyweatherfr-4.0.1/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:20:44.521202 pyweatherfr-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 19:20:41.000000 pyweatherfr-4.0.1/setup.py
```

### Comparing `pyweatherfr-4.0.0/LICENSE.txt` & `pyweatherfr-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.0.0/PKG-INFO` & `pyweatherfr-4.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.0.0
+Version: 4.0.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -18,9 +18,10 @@
 Requires-Dist: columnar
 Requires-Dist: termcolor
 Requires-Dist: colorama
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
 Requires-Dist: retry_requests
 Requires-Dist: geopy
+Requires-Dist: numpy
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-4.0.0/README.md` & `pyweatherfr-4.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ## Autres options
 
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
-  - ``-C/--cache``  met à jour le cache du nom des villes (cache par défaut 30j)
+  - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
   
 # Démo
 
 ![image](./demo_01.png)
 
 ![image](./demo_02.png)
```

### Comparing `pyweatherfr-4.0.0/pyweatherfr/args.py` & `pyweatherfr-4.0.1/pyweatherfr/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,25 +56,25 @@
     my_parser.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
         default=1000,
-        choices=range(-100, 4),
+        choices=range(-101, 4),
         help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ..., -1 pour J-1, ...)",
     )
     my_parser.add_argument(
         "-p",
         "--past",
         metavar="JOUR PASSE",
         action="store",
         type=int,
         default=0,
-        choices=range(1, 100),
+        choices=range(1, 101),
         help="affichage des données météo génériques depuis [JOUR PASSE] (-10 pour J-10 à J-1, ...)",
     )         
     my_group.add_argument(
         "-g",
         "--gps",
         metavar=("LATITUDE", "LONGITUDE"),
         action="store",
@@ -90,18 +90,17 @@
     my_parser.add_argument(
         "-c",
         "--condensate",
         action="store_true",
         help="condenser la sortie",
     )
     my_parser.add_argument(
-        "-C",
-        "--cache",
+        "--nocache",
         action="store_true",
-        help="rafraichit le cache des villes",
+        help="supprime le cache de l'api meteo france",
     )    
     my_parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="mode verbeux",
     )
```

### Comparing `pyweatherfr-4.0.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.0.1/pyweatherfr/pyweatherfr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 pyweatherfr use case
 """
 
 
 from pyweatherfr.args import compute_args
 
-import geopy,certifi,ssl
+import unicodedata
+import geopy
+import certifi
+import ssl
 import datetime
 import sys
 import json
 import urllib.request
 import os
 import openmeteo_requests
 import requests_cache
@@ -88,19 +91,19 @@
     pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
     return ze_path
 
 
 def find():
 
     if compute_args().town:
-        ville, dpt, lat, long = obtain_url_and_town_from_cp()
+        ville, dpt, lat, long = obtain_city_data()
     elif compute_args().gps:
-        ville, dpt, lat, long = obtain_url_and_town_from_gps()
+        ville, dpt, lat, long = obtain_city_data_from_gps()
     else:
-        ville, dpt, lat, long = obtain_url_and_town_from_ip()
+        ville, dpt, lat, long = obtain_city_data_from_ip()
 
     if compute_args().now:
         previsions_courantes(ville, dpt, lat, long)
     elif compute_args().jour == 1000:
         previsions_generiques(ville, dpt, lat, long)
     else:
         previsions_detaillees(ville, dpt, lat, long)
@@ -544,20 +547,30 @@
 
 
 def print_generic_data_town(ville, dpt, lat, long):
     print("")
 
     data = []
     if compute_args().nocolor:
-        data.append(ville + " (" + dpt + ")")
-        data.append("lat.: " + lat + " / long.: " +long)
+        if (ville is None or ville == "") and (dpt is None or dpt == ""):
+            print_debug("pas de data pour ville/dpt/cp")
+        elif dpt is None or dpt == "":
+            data.append(ville)
+        else:    
+            data.append(ville + " (" + dpt + ")")
+        data.append(f"lat.:  {float(lat):.4f}° / long.: {float(long):.4f}° ")
         data.append([datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
     else:
-        data.append([HOME, ville + " (" + dpt + ")"])
-        data.append([BOUSSOLE, "lat.: " + lat + " / long.: " +long])
+        if (ville is None or ville == "") and (dpt is None or dpt == ""):
+            print_debug("pas de data pour ville/dpt/cp")
+        elif dpt is None or dpt == "":
+            data.append([HOME, ville])
+        else:    
+            data.append([HOME, ville + " (" + dpt + ")"])
+        data.append([BOUSSOLE, f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° "])
         data.append([CLOCK, datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
 
     if compute_args().condensate:
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
 
@@ -584,15 +597,15 @@
                 'essayez avec le lancement classique "pyweatherfr [VILLE]"',
                 "yellow",
             )
         )
     exit(1)
 
 
-def obtain_url_and_town_from_ip():
+def obtain_city_data_from_ip():
 
     with urllib.request.urlopen("https://geolocation-db.com/json") as url:
         print_debug(
             "recherche de la localisation depuis https://geolocation-db.com/json"
         )
         data = json.loads(url.read().decode())
         print_debug(str(data))
@@ -600,26 +613,26 @@
         lat = str(data["latitude"])
         long = str(data["longitude"])
         dpt = str(data["postal"])
         return ville, dpt, lat, long 
     
 
 
-def obtain_url_and_town_from_gps():
+def obtain_city_data_from_gps():
     print_debug(
         "COORDONNEES_GPS :"
         + "latitude="
         + str(compute_args().gps[0])
         + " longitude="
         + str(compute_args().gps[1])
     )
     return "", "", str(compute_args().gps[0]), str(compute_args().gps[1])
 
 
-def obtain_url_and_town_from_cp():
+def obtain_city_data():
 
     town = compute_args().town
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     
     # Création d'un objet géocodeur Nominatim
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
@@ -630,29 +643,31 @@
     # Affichage des informations de localisation
     choix = []
     if locations == None:
         print(my_colored("erreur : aucune ville trouvée", "red")) 
         exit(1)    
     for location in locations:
         print_debug(str(location.raw))
-        ville = location.raw.get("address").get("village")
-        if ville == None:
+        ville = clean_string(location.raw.get("address").get("village"))
+        if ville == None or (location.raw.get("address").get("municipality") != None and clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower())):
             ville = location.raw.get("address").get("municipality")
-        if ville == None:
+        if ville == None or (location.raw.get("address").get("town") != None and clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower())):
+            ville = location.raw.get("address").get("town")               
+        if ville == None or (location.raw.get("address").get("city") != None and clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower())):
             ville = location.raw.get("address").get("city")
         dpt = location.raw.get("address").get("county")
         if dpt ==None:
             dpt=""
         cp = location.raw.get("address").get("postcode")
         if cp == None:
             cp = ""
         lat = location.raw.get("lat")
         long = location.raw.get("lon")
         print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
-        if ville.lower() == town.lower() or cp.lower() == town.lower(): 
+        if clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower(): 
             if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
                 choix.append([ville+"-"+dpt, ville, dpt, lat, long])
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         lat = choice[3]
@@ -661,16 +676,16 @@
     if len(choix)==0:
         print(my_colored("erreur : aucune ville trouvée", "red")) 
         exit(1)
     i=0    
     for choice in choix:
         i=i+1
         print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
-    toto = input("Quelle ville?")
-    choice = choix[int(toto)]
+    toto = input("Quelle ville? ")
+    choice = choix[int(toto)-1]
     ville = choice[1]
     dpt = choice[2]
     lat = choice[3]
     long = choice[4]
     return ville, dpt, lat, long
 
 
@@ -684,23 +699,16 @@
     if compute_args().verbose:
         print("debug : " + message)
 
 
 
 
 def resume(latitude, longitude):
-    # Setup the Open-Meteo API client with cache and retry on error
-    cache_session = requests_cache.CachedSession(
-        get_user_config_directory_pyweather() + ".cache", expire_after=3600
-    )
-    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
+    retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
-
-    # Make sure all required weather variables are listed here
-    # The order of variables in hourly or daily is important to assign them correctly below
     url = "https://api.open-meteo.com/v1/meteofrance"
     date_debut = (datetime.datetime.now() + datetime.timedelta(days=-1*compute_args().past)).strftime("%Y-%m-%d")
     date_fin = (datetime.datetime.now() + datetime.timedelta(days=3)).strftime("%Y-%m-%d")
     if compute_args().past!=0:
         date_fin = (datetime.datetime.now() + datetime.timedelta(days=-1)).strftime("%Y-%m-%d")    
     params = {
         "timezone": "Europe/Paris",
@@ -721,19 +729,15 @@
             "snowfall_sum",
             "precipitation_hours",
             "sunshine_duration"
         ],
     }
     print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
-
-    # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
-
-    # Process daily data. The order of variables needs to be the same as requested.
     daily = response.Daily()
     daily_temperature_2m_max = daily.Variables(0).ValuesAsNumpy()
     daily_temperature_2m_min = daily.Variables(1).ValuesAsNumpy()
     daily_apparent_temperature_max = daily.Variables(2).ValuesAsNumpy()
     daily_apparent_temperature_min = daily.Variables(3).ValuesAsNumpy()
     daily_precipitation_sum = daily.Variables(4).ValuesAsNumpy()
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
@@ -756,18 +760,15 @@
         snowfall,
         precipitation_hours,
         sunshine_duration
     )
 
 
 def specific_day(latitude, longitude, day):
-    cache_session = requests_cache.CachedSession(
-        get_user_config_directory_pyweather() + ".cache", expire_after=3600
-    )
-    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
+    retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
         "hourly": [
@@ -789,19 +790,15 @@
         ),
         "end_date": (
             datetime.datetime.now() + datetime.timedelta(days=day + 1)
         ).strftime("%Y-%m-%d"),
     }
     print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
-
-    # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
-
-    # Process daily data. The order of variables needs to be the same as requested.
     hourly = response.Hourly()
     hourly_temperature_2m = hourly.Variables(0).ValuesAsNumpy()
     hourly_apparent_temperature = hourly.Variables(1).ValuesAsNumpy()
     hourly_precipitation = hourly.Variables(2).ValuesAsNumpy()
     hourly_wind_speed_10m = hourly.Variables(3).ValuesAsNumpy()
     hourly_wind_gusts_10m = hourly.Variables(4).ValuesAsNumpy()
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
@@ -822,20 +819,30 @@
         weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
         cloud_cover
                 )
 
-
-def current(latitude, longitude):
-    cache_session = requests_cache.CachedSession(
+def cache_session():
+    if compute_args().nocache:
+        directory = get_user_config_directory_pyweather()
+        file_path = os.path.join(directory, ".cache.sqlite")
+        if os.path.exists(file_path):
+            os.remove(file_path)
+            print_debug("Le cache a été supprimé avec succès.")
+        else:
+            print_debug("Le cache n'existe pas.")
+    return requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
-    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
+
+
+def current(latitude, longitude):
+    retry_session = retry_requests.retry(cache_session(), retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
 
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "latitude": latitude,
         "longitude": longitude,
         "current": [
@@ -877,7 +884,18 @@
         current_surface_pressure,
         current_wind_speed_10m,
         current_wind_gusts_10m,
         current_wind_direction_10m,
         current_weather_code,
         snowfall
     )
+
+def clean_string(mystring):
+    if mystring is None:
+        return None
+    retour =""
+    nfkd_form = unicodedata.normalize('NFKD', mystring)
+    retour = ''.join([c for c in nfkd_form if not unicodedata.combining(c)])
+    retour = retour.replace(' ', '-').replace("'", '-').replace('"', '-')
+    if mystring!=retour:
+        print_debug(mystring + " modifié en " + retour)
+    return retour
```

### Comparing `pyweatherfr-4.0.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.0.1/pyweatherfr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.0.0
+Version: 4.0.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -18,9 +18,10 @@
 Requires-Dist: columnar
 Requires-Dist: termcolor
 Requires-Dist: colorama
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
 Requires-Dist: retry_requests
 Requires-Dist: geopy
+Requires-Dist: numpy
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-4.0.0/setup.py` & `pyweatherfr-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.0.0",
+    version="4.0.1",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
-    install_requires=["columnar","termcolor", "colorama","openmeteo_requests","requests_cache","retry_requests","geopy"],
+    install_requires=["columnar","termcolor", "colorama","openmeteo_requests","requests_cache","retry_requests","geopy","numpy"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "pyweatherfr=pyweatherfr.__init__:pyweatherfr"
         ],
     },
     classifiers=[
```

