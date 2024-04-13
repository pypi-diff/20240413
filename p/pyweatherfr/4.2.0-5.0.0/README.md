# Comparing `tmp/pyweatherfr-4.2.0.tar.gz` & `tmp/pyweatherfr-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-4.2.0.tar", last modified: Sat Apr 13 15:46:50 2024, max compression
+gzip compressed data, was "pyweatherfr-5.0.0.tar", last modified: Sat Apr 13 16:49:16 2024, max compression
```

## Comparing `pyweatherfr-4.2.0.tar` & `pyweatherfr-5.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36797 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:46:18.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 15:46:50.000000 pyweatherfr-4.2.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:46:50.868672 pyweatherfr-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 15:46:05.000000 pyweatherfr-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.575111 pyweatherfr-5.0.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37788 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:48:46.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/setup.py
```

### Comparing `pyweatherfr-4.2.0/LICENSE.txt` & `pyweatherfr-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-4.2.0/PKG-INFO` & `pyweatherfr-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.2.0
+Version: 5.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.2.0/README.md` & `pyweatherfr-5.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # :sunny: :umbrella: :cloud: pyweatherfr
 
-pyweatherfr affiche les prévisions méteo pour les communes françaises dans votre terminal. Il utilise l'API de MéteoFrance
+pyweatherfr affiche les prévisions méteo pour les communes françaises (voire mondiales) dans votre terminal. Il utilise l'API de MéteoFrance
 
 
 # 🚀 Comment utiliser **pyweatherfr**
 
 pyweatherfr affiche les prévisions météo sur 4 jours en se basant sur l'ip
 
 pyweatherfr \[VILLE\]
@@ -36,14 +36,15 @@
 pyweatherfr \[TOWN\] -d [STR]
 
 exemple : ``pyweatherfr Grenoble -d 2024-03-30`` affiche les données météo détaillées pour Grenoble au 30/03/2024
 
 
 ## Autres options
 
+  - ``--world``    active la recherche des villes dans le monde entier. Attention, les données sont moins précises.
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
   - ``--utc``    utilise l'heure utc dans les previsions au lieu de l'heure locale de la ville
```

### Comparing `pyweatherfr-4.2.0/pyweatherfr/args.py` & `pyweatherfr-5.0.0/pyweatherfr/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,19 @@
         help="affichage des données météo par coordonnées GPS",
     )      
     my_parser.add_argument(
         "--nocolor",
         action="store_true",
         help="désactiver couleur et emojis en sortie -à utiliser en cas de problème d'affichage-",
     )
+    my_parser.add_argument(
+        "--world",
+        action="store_true",
+        help="activer la recherche hors France",
+    )    
     group = my_parser.add_mutually_exclusive_group()
     group.add_argument(
         "--pc",
         action="store_true",
         help="utilise l'heure locale du PC indépendamment de la ville cherchée",
     )
     group.add_argument(
```

### Comparing `pyweatherfr-4.2.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.0.0/pyweatherfr/pyweatherfr.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             "humidité",
             "rayonnement",            
             "warnings",
         ]
 
     if data != []:
         if compute_args().condensate:
-            table = columnar.columnar(data, no_borders=True, wrap_max=0)
+            table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
 
 def calculer_direction(direction_vent_degres):
     if (
@@ -610,15 +610,15 @@
                 "durée pluie",
                 "durée soleil",
                 "warning",
             ]
 
     if data != []:
         if compute_args().condensate:
-            table = columnar.columnar(data, no_borders=True, wrap_max=0)
+            table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
 
 
 def print_generic_data_town(ville, dpt, lat, long, alt, recap):
@@ -711,46 +711,52 @@
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     
     # Création d'un objet géocodeur Nominatim
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     
     # Géocodage d'une adresse
-    locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True)
+    if compute_args().world:
+        locations = geolocator.geocode(town,exactly_one=False,addressdetails=True)
+    else:
+        locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True)
     
     # Affichage des informations de localisation
     choix = []
     if locations == None:
         print(my_colored("erreur : aucune ville trouvée", "red")) 
         exit(1)    
     for location in locations:
-        print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
-        ville = clean_string(location.raw.get("address").get("island"))
-        if ville == None or (location.raw.get("address").get("village") != None and clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower())):
-            ville = location.raw.get("address").get("village")
-        if ville == None or (location.raw.get("address").get("municipality") != None and clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower())):
-            ville = location.raw.get("address").get("municipality")
-        if ville == None or (location.raw.get("address").get("town") != None and clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower())):
-            ville = location.raw.get("address").get("town")               
-        if ville == None or (location.raw.get("address").get("city") != None and clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower())):
-            ville = location.raw.get("address").get("city")
-        dpt = location.raw.get("address").get("county")
-        if dpt ==None:
-            dpt=location.raw.get("address").get("state")
-        if dpt ==None:
-            dpt= location.raw.get("address").get("postcode")  
-        cp = location.raw.get("address").get("postcode")
-        if cp == None:
-            cp = ""
-        lat = location.raw.get("lat")
-        long = location.raw.get("lon")
-        print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
-        if clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower(): 
-            if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
-                choix.append([ville+"-"+dpt, ville, dpt, lat, long])
+        if (location.raw.get("addresstype")=="postcode" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
+            print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
+            ville = None
+            if ville == None or (location.raw.get("address").get("village") != None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+                ville = location.raw.get("address").get("village")
+            if ville == None or (location.raw.get("address").get("municipality") != None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+                ville = location.raw.get("address").get("municipality")
+            if ville == None or (location.raw.get("address").get("town") != None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+                ville = location.raw.get("address").get("town")               
+            if ville == None or (location.raw.get("address").get("city") != None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+                ville = location.raw.get("address").get("city")        
+            dpt = location.raw.get("address").get("county")
+            if dpt ==None:
+                dpt=location.raw.get("address").get("state")
+            if dpt ==None:
+                dpt= location.raw.get("address").get("postcode") 
+            if dpt ==None or compute_args().world:
+                dpt= location.raw.get("address").get("country")              
+            cp = location.raw.get("address").get("postcode")
+            if cp == None:
+                cp = ""
+            lat = location.raw.get("lat")
+            long = location.raw.get("lon")
+            print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
+            if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower() or (compute_args().world and location.raw.get("address").get("country")!="France")): 
+                if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
+                    choix.append([ville+"-"+dpt, ville, dpt, lat, long])
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         lat = choice[3]
         long = choice[4]
         return ville, dpt, lat, long
```

### Comparing `pyweatherfr-4.2.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.0.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 4.2.0
+Version: 5.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-4.2.0/setup.py` & `pyweatherfr-5.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="4.2.0",
+    version="5.0.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

