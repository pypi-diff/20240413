# Comparing `tmp/anilist-helper-1.42.tar.gz` & `tmp/anilist-helper-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anilist-helper-1.42.tar", last modified: Fri Mar  8 12:11:28 2024, max compression
+gzip compressed data, was "anilist-helper-1.5.tar", last modified: Sat Apr 13 00:51:34 2024, max compression
```

## Comparing `anilist-helper-1.42.tar` & `anilist-helper-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 12:11:28.381489 anilist-helper-1.42/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-08 12:11:20.000000 anilist-helper-1.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-03-08 12:11:28.381489 anilist-helper-1.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-03-08 12:11:20.000000 anilist-helper-1.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 12:11:28.381489 anilist-helper-1.42/anilist_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-03-08 12:11:28.000000 anilist-helper-1.42/anilist_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-08 12:11:28.000000 anilist-helper-1.42/anilist_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 12:11:28.000000 anilist-helper-1.42/anilist_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 12:11:28.000000 anilist-helper-1.42/anilist_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 12:11:28.000000 anilist-helper-1.42/anilist_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 12:11:28.381489 anilist-helper-1.42/anilisthelper/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-08 12:11:20.000000 anilist-helper-1.42/anilisthelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20562 2024-03-08 12:11:20.000000 anilist-helper-1.42/anilisthelper/anilist_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-08 12:11:20.000000 anilist-helper-1.42/anilisthelper/token_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-08 12:11:20.000000 anilist-helper-1.42/anilisthelper/token_getter.html
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-08 12:11:20.000000 anilist-helper-1.42/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 12:11:28.381489 anilist-helper-1.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-08 12:11:20.000000 anilist-helper-1.42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-13 00:51:19.000000 anilist-helper-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-13 00:51:34.167762 anilist-helper-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-13 00:51:19.000000 anilist-helper-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/anilist_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/anilisthelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/anilist_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-13 00:51:19.000000 anilist-helper-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 00:51:34.167762 anilist-helper-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 00:51:19.000000 anilist-helper-1.5/setup.py
```

### Comparing `anilist-helper-1.42/LICENSE` & `anilist-helper-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anilist-helper-1.42/PKG-INFO` & `anilist-helper-1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilist-helper
-Version: 1.42
+Version: 1.5
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/ProchyGaming/anilist-helper
 Project-URL: Documentation, https://github.com/ProchyGaming/anilist-helper/wiki
 Project-URL: Source, https://github.com/ProchyGaming/anilist-helper
 Keywords: python,anilist
@@ -85,17 +85,23 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-
+* [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
+    * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
+    * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
+    * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
+    * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
+    * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
-    * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
+    * [gh-actions: Add action to cache build dependencies](https://github.com/ProchyGaming/anilist-helper/commit/7e02445ec6f5acf0ef7e5fad8634e77c9301164a)
+    * [anilist_helper: Remove debug lines for cache](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
 * [1.041](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.041)
     * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/b0ea061c16c5c147faf651593dd412b5bb92d2bb)
 * [1.04](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.04)
     * [anilist_helper: Break down the setup process](https://github.com/ProchyGaming/anilist-helper/commit/8c3fe5900f4396186b3a7315bf38e73e236e784e)
     * [Remove LICENCE file when using pip show](https://github.com/ProchyGaming/anilist-helper/commit/9b42002dab525a1893c1f31b415c504c8e34c04b)
     * Didn't forget to update the README finally lul xd
 * [1.03](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.03)
```

### Comparing `anilist-helper-1.42/README.md` & `anilist-helper-1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -58,17 +58,23 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-
+* [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
+    * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
+    * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
+    * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
+    * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
+    * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
-    * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
+    * [gh-actions: Add action to cache build dependencies](https://github.com/ProchyGaming/anilist-helper/commit/7e02445ec6f5acf0ef7e5fad8634e77c9301164a)
+    * [anilist_helper: Remove debug lines for cache](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
 * [1.041](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.041)
     * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/b0ea061c16c5c147faf651593dd412b5bb92d2bb)
 * [1.04](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.04)
     * [anilist_helper: Break down the setup process](https://github.com/ProchyGaming/anilist-helper/commit/8c3fe5900f4396186b3a7315bf38e73e236e784e)
     * [Remove LICENCE file when using pip show](https://github.com/ProchyGaming/anilist-helper/commit/9b42002dab525a1893c1f31b415c504c8e34c04b)
     * Didn't forget to update the README finally lul xd
 * [1.03](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.03)
```

### Comparing `anilist-helper-1.42/anilist_helper.egg-info/PKG-INFO` & `anilist-helper-1.5/anilist_helper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilist-helper
-Version: 1.42
+Version: 1.5
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/ProchyGaming/anilist-helper
 Project-URL: Documentation, https://github.com/ProchyGaming/anilist-helper/wiki
 Project-URL: Source, https://github.com/ProchyGaming/anilist-helper
 Keywords: python,anilist
@@ -85,17 +85,23 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-
+* [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
+    * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
+    * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
+    * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
+    * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
+    * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
-    * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
+    * [gh-actions: Add action to cache build dependencies](https://github.com/ProchyGaming/anilist-helper/commit/7e02445ec6f5acf0ef7e5fad8634e77c9301164a)
+    * [anilist_helper: Remove debug lines for cache](https://github.com/ProchyGaming/anilist-helper/commit/acc5b453d8324ef181c549df3bc550d5c46b0b26)
 * [1.041](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.041)
     * [anilist_helper: Fix more oversights](https://github.com/ProchyGaming/anilist-helper/commit/b0ea061c16c5c147faf651593dd412b5bb92d2bb)
 * [1.04](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.04)
     * [anilist_helper: Break down the setup process](https://github.com/ProchyGaming/anilist-helper/commit/8c3fe5900f4396186b3a7315bf38e73e236e784e)
     * [Remove LICENCE file when using pip show](https://github.com/ProchyGaming/anilist-helper/commit/9b42002dab525a1893c1f31b415c504c8e34c04b)
     * Didn't forget to update the README finally lul xd
 * [1.03](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.03)
```

### Comparing `anilist-helper-1.42/anilisthelper/anilist_helper.py` & `anilist-helper-1.5/anilisthelper/anilist_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,191 +1,136 @@
 import requests, time, json, os, webbrowser, copy
-from datetime import datetime
+from datetime import datetime, timedelta
 from flask import Flask, request, jsonify, send_file
 from gevent.pywsgi import WSGIServer
+from .utils import utils_save_json, utils_read_json
+from .config_utils import config_setup
 
-def setup_webserver():
-    app = Flask(__name__)
-
-    # Enable CORS for all routes
-    @app.after_request
-    def add_cors_headers(response):
-        response.headers['Access-Control-Allow-Origin'] = '*'
-        response.headers['Access-Control-Allow-Headers'] = 'Content-Type'
-        response.headers['Access-Control-Allow-Methods'] = 'GET, POST, OPTIONS'
-        return response
-
-    @app.route('/auth') #Host the token processing html page
-    def send_token():
-        return send_file('token_getter.html')
-
-    @app.route('/access_token', methods=["POST"]) #Listen for token webhook
-    def receive_token():
-      json_data = request.get_json()
-      if 'access_token' in json_data:
-        global global_token
-        global_token = json_data['access_token']
-        http_server.stop()
-        print('Token obtained!')
-        return jsonify({'message': 'Token received successfully'})
-      
-    http_server = WSGIServer(('127.0.0.1', 8888), app, log=None)
-
-    def start_webserver():
-        print('Authentificate in the opened tab')
-        webbrowser.open(global_tooltip, 0)
-        http_server.serve_forever()
-
-    return start_webserver, http_server
-
-def setup_anilist():
-  setup_function, _ = setup_webserver()  # Setup the server function here
-  script_path = os.path.dirname(os.path.abspath(__file__))
-  config = os.path.join(script_path, 'data', 'config', 'config.json')
+total_user = {}
+user_entries = {}
+script_path = os.path.dirname(os.path.abspath(__file__))
+anilist_id_cache_path = os.path.join(script_path, 'cache', 'anilist_id_cache.json')
+anilist_search_cache_path = os.path.join(script_path, 'cache', 'anilist_search_cache.json')
+config_path = os.path.join(script_path, 'config', 'config.json')
 
-  def gen_please(name, help):
-      return f'Please input your {name} here ({help}):\n'
-    
-  def get_input(prompt, data_type = str):
-      while True:
-          user_input = input(prompt).lower()
-          try:
-              converted_input = data_type(user_input)
-              return converted_input
-          except ValueError:
-              print("Invalid input. Please enter a valid", data_type.__name__)  
-
-  def anilist_generate_api_key(client_id):
-      global global_tooltip
-      global_tooltip = f"https://anilist.co/api/v2/oauth/authorize?client_id={client_id}&response_type=token" 
-      setup_function()  # Start the server here
-      user_token = global_token
-      return user_token
-
-  config_dict = {}
-  if anilist_env_key:
-    config_dict['anilist_client_token'] = ''
-    config_dict['anilist_user_token'] = anilist_env_key
-  else:
-    webbrowser.open('https://anilist.co/settings/developer', 0)
-    config_dict['anilist_client_token'] = get_input(gen_please('Anilist API Client ID',"Create a new client and copy its ID"))
-    config_dict['anilist_user_token'] = anilist_generate_api_key(config_dict['anilist_client_token'])
-  utils_save_json(config ,config_dict)
-
-def create_data_files(file_path):
-  folder_path = os.path.dirname(file_path)
-  if not os.path.exists(folder_path):
-    os.makedirs(folder_path)
-  does_exist = os.path.exists(file_path)
-  if not does_exist:
-    utils_save_json(file_path, {})  
-
-def setup_cache():
-  script_path = os.path.dirname(os.path.abspath(__file__))
-  anilist_cache = os.path.join(script_path, 'data', 'cache', 'anilist_cache.json')
-  search_cache = os.path.join(script_path, 'data', 'cache', 'search_cache.json')
-  script_files = [anilist_cache, search_cache]
-  for file in script_files:
-    create_data_files(file)
-
-def config_anilist():
-  script_path = os.path.dirname(os.path.abspath(__file__))
-  config = os.path.join(script_path, 'data', 'config', 'config.json')
-  create_data_files(config)
-  if anilist_env_key:
-    print('Config not found! AniList environmental variable detected. Generating....')
-  else:
-    print('Config not found! Please follow the on-screen instructions. Generating....')
-  setup_anilist()
 
-def init_setup():
-  setup_cache()
-  config_anilist()
+# Utils
 
 def clear_cache():
-  cache_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data', 'cache')
+  config = utils_read_json(config_path)
+  try:
+    del config['checked_date']
+  except:
+    pass
+  os.remove(anilist_id_cache_path)
+  os.remove(anilist_search_cache_path)
+
+def check_status_in_cache():
+  og_cache = utils_read_json(anilist_id_cache_path)
+  if not og_cache: return
+  cache = copy.deepcopy(og_cache)
   config_dict = utils_read_json(config_path)
+  current_date = datetime.now().date()
+  try:
+    checked_date = datetime.strptime(config_dict['checked_date'], '%Y-%m-%d').date()
+  except:
+    config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
+    utils_save_json(config_path, config_dict)
+    checked_date = current_date
+  if current_date > checked_date:
+    for anime in og_cache:
+      try:
+        release_date = datetime.strptime(cache[anime]['release_date'], '%Y-%m-%d').date()
+      except:
+        release_date = None
+      try:
+        end_date = datetime.strptime(cache[anime]['end_date'], '%Y-%m-%d').date()
+      except:
+        end_date = None
+      if not release_date and not end_date:
+        continue
+      status = cache[anime]['status']
+      if status == 'RELEASING':
+        next_ep_date = release_date + timedelta(cache[anime]['upcoming_ep'] * 7)
+        if end_date:
+          if current_date > end_date:
+            updated_info = get_anime_info(anime, True)
+            cache.update(updated_info)
+        if current_date > next_ep_date:
+          updated_info = get_anime_info(anime, True)
+          cache.update(updated_info)
+      elif status == 'NOT_YET_RELEASED':
+        if release_date:
+          if current_date > release_date:
+            cache.update(get_anime_info(anime, True))
+    config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
+    utils_save_json(config_path, config_dict)
+    utils_save_json(anilist_id_cache_path, cache, True)
+
+def load_cache():
+  check_status_in_cache()
+  return utils_read_json(anilist_id_cache_path)
+
+def load_config():
+  config = utils_read_json(config_path)
   try:
-    del config_dict['checked_date']
+    return config['anilist_user_token']
   except:
+    return config_setup()['anilist_user_token']
+
+# Functions
+
+def make_graphql_request(query, variables=None, anilist_token=None):
+  if anilist_token:
     pass
-  utils_save_json(config_path, config_dict)
-  files = os.listdir(cache_path)
-  for file in files:
-    utils_save_json(os.path.join(cache_path, file), {})
-
-def utils_save_json(file_path, data, overwrite = True):
-  def update_json():
-    json_copy = utils_read_json(file_path)
-    if json_copy is None:
-      json_copy = {}
-    json_copy.update(data)
-    with open(file_path, "w", encoding="utf-8") as file:
-      json.dump(json_copy, file, indent=4, ensure_ascii=False)
-
-  json_file = utils_read_json(file_path)
-  if json_file != None:
-      if overwrite:
-        with open(file_path, "w", encoding="utf-8") as file:
-          json.dump(data, file, indent=4, ensure_ascii=False)
-      else:
-        update_json()
+  elif 'anilist_key' in os.environ:
+    anilist_token = os.getenv('anilist_key')
   else:
-    update_json() 
+    anilist_token = load_config()
 
-def utils_read_json(file_path):
-  if os.path.exists(file_path):
-    with open(file_path, "r", encoding="utf-8") as json_file:
-      data = json.load(json_file)
-    if data == {}:
-      return None
-    else:
-      return data
-  else:
-    return None
+  # Constants for GraphQL endpoint and headers
+  ANILIST_API_URL = 'https://graphql.anilist.co'
+  HEADERS = {'Content-Type': 'application/json', 'Authorization': f'Bearer {anilist_token}'}
+
+  def make_request():
+      response = requests.post(ANILIST_API_URL, json={'query': query, 'variables': variables}, headers=HEADERS)
+      return response
+
+  retries = 0
+  while True:
+      response = make_request()
+      if response.status_code == 200:
+          return response.json().get('data', {})
+      elif response.status_code == 429:
+          print(f"Rate limit exceeded. Waiting before retrying...")
+          print(query, variables, HEADERS, sep='\n')
+          print(response.json())
+          retry_after = int(response.headers.get('retry-after', 1))
+          time.sleep(retry_after)
+          retries += 1
+      elif response.status_code == 500 or response.status_code == 400:
+          print(f"Unknown error occured, retrying...")
+          print(query, variables, HEADERS, sep='\n')
+          print(response.json())
+          retries += 1
+      elif response.status_code == 404:
+          print(f"Anime not found")
+          return None
+      else:
+          print(f"Error {response.status_code}: {variables}")
+          return {}
 
-# Helper function for making GraphQL requests
-def make_graphql_request(query, variables=None):
-    
-    # Constants for GraphQL endpoint and headers
-    ANILIST_API_URL = 'https://graphql.anilist.co'
-    HEADERS = {'Content-Type': 'application/json', 'Authorization': f'Bearer {anilist_user_token}'}
-
-    def make_request():
-        response = requests.post(ANILIST_API_URL, json={'query': query, 'variables': variables}, headers=HEADERS)
-        return response
-
-    retries = 0
-    while True:
-        response = make_request()
-        if response.status_code == 200:
-            return response.json().get('data', {})
-        elif response.status_code == 429:
-            print(f"Rate limit exceeded. Waiting before retrying...")
-            retry_after = int(response.headers.get('retry-after', 1))
-            time.sleep(retry_after)
-            retries += 1
-        elif response.status_code == 500 or response.status_code == 400:
-            print(f"Unknown error occured, retrying...")
-            retries += 1
-        elif response.status_code == 404:
-            print(f"Anime not found")
-            return None
-        else:
-            print(f"Error {response.status_code}: {variables}")
-            return {}
-
-        # Exponential backoff with a maximum of 5 retries
-        if retries >= 5:
-            print("Maximum retries reached. Exiting.")
-            return {}
-            
-        print(f"Retrying... (Attempt {retries})")
+      # Exponential backoff with a maximum of 5 retries
+      if retries >= 5:
+          print("Maximum retries reached. Exiting.")
+          return {}
+          
+      print(f"Retrying... (Attempt {retries})")
 
-def get_latest_anime_entry_for_user(username, status = 'ALL'):
+def get_latest_anime_entry_for_user(username, status = 'ALL', anilist_token=None):
     status = status.upper()
     status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
     if status != 'ALL':
       if not status in status_options:
         print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
         return
       query = '''
@@ -201,15 +146,21 @@
                 lists {
                   entries {
                     id
                     progress
                     status
                     media {
                       id
+                      idMal
                       episodes
+                      tags {
+                        name
+                      }
+                      genres
+                      isAdult
                       title {
                         romaji
                         english
                         native
                       }
                       synonyms
                       status
@@ -243,15 +194,15 @@
                   }
                 }
               }
             }
             '''
     variables = {'username': username}
 
-    data = make_graphql_request(query, variables)
+    data = make_graphql_request(query, variables, anilist_token)
 
     if not username in user_entries:
       user_entries[username] = {}
       
     if data:
         entries = data.get('MediaListCollection', {}).get('lists', [])[0].get('entries', [])
         if entries:
@@ -265,15 +216,16 @@
               user_entry[anime_id]['watching_status'] = anime['status']
               user_entries[username][anime_id] = user_entry
               return user_entry
 
     print(f"No entries found for {username}'s planned anime list.")
     return None
 
-def get_all_anime_for_user(username, status = 'ALL'):
+def get_all_anime_for_user(username, status_list='ALL', anilist_token=None):
+  def main_function(status):
     status = status.upper()
     status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
     if status != 'ALL':
       if not status in status_options:
         print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
         return
       query = '''
@@ -289,15 +241,21 @@
                 lists {
                   entries {
                     id
                     progress
                     status
                     media {
                       id
+                      idMal
                       episodes
+                      tags {
+                        name
+                      }
+                      genres
+                      isAdult
                       title {
                         romaji
                         english
                         native
                       }
                       synonyms
                       status
@@ -331,19 +289,25 @@
                   }
                 }
               }
             }
             '''
     variables = {'username': username}
 
-    data = make_graphql_request(query, variables)
+    data = make_graphql_request(query, variables, anilist_token)
 
     if not username in user_entries:
       user_entries[username] = {}
 
+    if not username in total_user:
+      total_user[username] = {}
+
+    if not status in user_entries[username]:
+      user_entries[username][status] = {}
+
     user_ids = {}
       
     if data:
         entries = data.get('MediaListCollection', {}).get('lists', [])
         full_entries = {}
         for entry in entries: 
           for list_entry in entry['entries']:
@@ -352,60 +316,89 @@
         if full_entries:
             for anime_entry in full_entries:
               anime = full_entries[anime_entry]
               anime_entry_data = anime['media']
               anime_id = anime_entry_data['id']
               anime_id = str(anime_id)
               anime_info = generate_anime_entry(anime_entry_data)
-              user_ids[anime_id] = {}  # Initialize as a dictionary if not already initialized
+              if not anime_id in user_ids:
+                user_ids[anime_id] = {}  # Initialize as a dictionary if not already initialized
               user_ids[anime_id].update(anime_info)
               user_ids[anime_id]['watched_ep'] = anime['progress']
               user_ids[anime_id]['watching_status'] = anime['status']
-              user_entries[username].update(user_ids)
-            return user_ids
-
+            user_entries[username][status].update(user_ids)
+            return
     print(f"No entries found for {username}'s planned anime list.")
-    return None
+    return None  
+
+  if isinstance(status_list, str):
+    status_list = status_list.upper()
+    main_function(status_list)
+    return user_entries[username][status_list]
+  elif len(status_list) == 1:
+    status_list = status_list[0].upper()
+    main_function(status_list)
+    return user_entries[username][status_list]
+  elif isinstance(status_list, list):
+    for status in status_list:
+      status.upper()
+      main_function(status)
+      total_user[username].update(user_entries[username][status])
+    return total_user[username]
 
-def get_anime_entry_for_user(username, anilist_id):
+def get_anime_entry_for_user(username, anilist_id, anilist_token=None):
   anilist_id = str(anilist_id)
   try:
-    if anilist_id in user_entries[username]:
-          return {anilist_id: user_entries[username][anilist_id]}
+    if anilist_id in user_entries[username]['ALL']:
+          return {anilist_id: user_entries[username]['ALL'][anilist_id]}
   except KeyError:
-    get_all_anime_for_user(username)
-    return get_anime_entry_for_user(username, anilist_id)
+    get_all_anime_for_user(username, anilist_token)
+    return get_anime_entry_for_user(username, anilist_id, anilist_token)
   return None
 
-def get_anime_info(anime_id, force_update = False):
-    anime_cache = utils_read_json(anilist_id_cache_path)
+def reset_user_cache(username):
+  user_entries[username] = {}
+  total_user[username] = {}
+
+def get_anime_info(anime_id, force_update = False, anilist_token=None):
+    if force_update:
+      anime_cache = {}
+    else:
+      anime_cache = load_cache()
     anime_id = str(anime_id)
     if not anime_id:
       return None
     def fetch_from_anilist():
       # Fetch anime info from Anilist API or any other source
-      anime_info = anilist_fetch_anime_info(anime_id)
+      anime_info = anilist_fetch_anime_info(anime_id, anilist_token)
       # Cache the fetched anime info
       utils_save_json(anilist_id_cache_path, anime_info, False)
       return anime_info
     # Check if anime_id exists in cache
     try:
       if anime_id in anime_cache and not force_update:
+          print("Returning cached result for anime_id:", anime_id)
           return {anime_id: anime_cache[anime_id]}
       else:
         return fetch_from_anilist()
     except TypeError:
       return fetch_from_anilist()
 
-def anilist_fetch_anime_info(anilist_id):
+def anilist_fetch_anime_info(anilist_id, anilist_token=None):
     query = '''
     query ($mediaId: Int) {
       Media(id: $mediaId) {
         id
+        idMal
         episodes
+        tags {
+          name
+        }
+        genres
+        isAdult
         title {
           romaji
           english
           native
         }
         synonyms
         status
@@ -437,15 +430,15 @@
         }
       }
     }
     '''
     
     variables = {'mediaId': anilist_id}
 
-    data = make_graphql_request(query, variables)
+    data = make_graphql_request(query, variables, anilist_token)
     anime_data = {}
     if data:
       anime = data.get('Media', {})
       if anime:
         anime_id = str(anime['id'])
         anime_info = anime
         anime_data[anime_id] = {}
@@ -483,20 +476,32 @@
         relations[edge['node']['id']]['main_title'] = edge['node']['title']['romaji']
         relations[edge['node']['id']]['status'] = edge['node']['status']
         relations[edge['node']['id']]['type'] = edge['relationType']
     if not relations:
       relations = None
     return relations
 
-  cache = utils_read_json(anilist_id_cache_path)
+  def is_sus(anime_data):
+    genres = anime_data['genres']
+    tags = [item['name'] for item in anime_data['tags']]
+    adult_status = anime_data['isAdult']
+    sus_tags = ['Nudity', 'Bondage', 'Masochism', 'Sadism', 'Exhibitionism']
+    for sus_tag in sus_tags:
+      if sus_tag in tags:
+        return True
+    if 'Ecchi' in genres or adult_status:
+      return True
+    else:
+      return False
+
   anime_id = str(anime_info['id'])
-  if cache and anime_id in cache:
-    return cache[anime_id]
   anime_data = {}
+  anime_data['mal_id'] = anime_info['idMal']
   anime_data['total_eps'] = anime_info['episodes']
+  anime_data['is_sus'] = is_sus(anime_info)
   anime_data['main_title'] = anime_info['title']['romaji']
   anime_data['synonyms'] = [
       anime_info['title']['romaji'],
       anime_info['title']['english'],
       anime_info['title']['native'],
   ] + anime_info['synonyms']
   anime_data['synonyms'] = [item for item in anime_data['synonyms'] if item is not None]  
@@ -508,104 +513,72 @@
   except:
     anime_data['upcoming_ep'] = None
   anime_data['format'] = anime_info['format']
   anime_data['related'] = getRelated()
   utils_save_json(anilist_id_cache_path, {anime_id: anime_data}, False)
   return anime_data
 
-def get_id(name):
-  search_cache = utils_read_json(search_cache_path)
+def get_id(name, anilist_token=None):
+  search_cache = utils_read_json(anilist_search_cache_path)
   
   def fetch_from_anilist():
     # Fetch anime info from Anilist API or any other source
-    anime_info = anilist_fetch_id(name)
+    anime_info = str(anilist_fetch_id(name))
     if anime_info:
-      ani_dict = get_anime_info(anime_info)
-      status = ani_dict[str(anime_info)]['status']
+      ani_dict = get_anime_info(anime_info, False, anilist_token)
+      status = ani_dict[anime_info]['status']
       if status == 'NOT_YET_RELEASED':
         anime_info = None
     json_out = {name: anime_info}
+    utils_save_json(anilist_search_cache_path, json_out, False)
     return anime_info
   
   # Check if anime_id exists in cache
   try:
     if search_cache and name in search_cache:
-        return search_cache[name]
+        print("Returning cached result for search query:", name)
+        return str(search_cache[name])
     else:
         return fetch_from_anilist()
   except TypeError:
     return fetch_from_anilist()
       
-def anilist_fetch_id(name):
+def anilist_fetch_id(name, anilist_token=None):
     query = '''
     query ($search: String) {
       Media(search: $search, type: ANIME) {
         id
       }
     }
     '''
     variables = {'search': name}
-    data = make_graphql_request(query, variables)
+    data = make_graphql_request(query, variables, anilist_token)
 
     if data:
         anime_list = data['Media']['id']
 
         if anime_list:
             return anime_list
 
     return None
 
-def check_status_in_cache():
-  og_cache = utils_read_json(anilist_id_cache_path)
-  if not og_cache: return
-  cache = copy.deepcopy(og_cache)
-  config_dict = utils_read_json(config_path)
-  current_date = datetime.now().date()
-  try:
-    checked_date = datetime.strptime(config_dict['checked_date'], '%Y-%m-%d').date()
-  except:
-    config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
-    utils_save_json(config_path, config_dict)
-    checked_date = current_date
-  if current_date > checked_date:
-    for anime in og_cache:
-      try:
-        release_date = datetime.strptime(cache[anime]['release_date'], '%Y-%m-%d').date()
-      except:
-        release_date = None
-      try:
-        end_date = datetime.strptime(cache[anime]['end_date'], '%Y-%m-%d').date()
-      except:
-        end_date = None
-      if not release_date and not end_date:
-        continue
-      status = cache[anime]['status']
-      if status == 'RELEASING':
-        if end_date:
-          if current_date > end_date:
-            cache.update(get_anime_info(anime, True))
-      elif status == 'NOT_YET_RELEASED':
-        if release_date:
-          if current_date > release_date:
-            cache.update(get_anime_info(anime, True))
-    config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
-    utils_save_json(config_path, config_dict)
-    utils_save_json(anilist_id_cache_path, cache, True)
-  
+def get_userdata(anilist_token=None):
+    # GraphQL query to get the username of the authenticated user
+    query = """
+    query {
+      Viewer {
+        name
+        avatar {
+          large
+        }
+      }
+    }
+    """
+    
+    variables = {}
+    data = make_graphql_request(query, variables, anilist_token)
 
-data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-anilist_env_key = os.getenv('anilist_key')
-if not os.path.exists(data_path):
-  if os.path.exists(os.path.join(data_path, 'cache')):
-    config_anilist()
-  else:
-    init_setup()
-user_entries = {}
-try:
-  anilist_user_token = utils_read_json(os.path.join(data_path, 'config', 'config.json'))['anilist_user_token']
-except:
-  config_anilist()
-  anilist_user_token = utils_read_json(os.path.join(data_path, 'config', 'config.json'))['anilist_user_token']
-anilist_id_cache_path = os.path.join(data_path, 'cache', 'anilist_cache.json')
-search_cache_path = os.path.join(data_path, 'cache', 'search_cache.json')
-config_path = os.path.join(data_path, 'config', 'config.json')
-check_status_in_cache()
+    if data:
+      # Extract the username from the response data
+      username = data['Viewer']['name']
+      profile_pic = data['Viewer']['avatar']['large']
+      return [username, profile_pic]
```

### Comparing `anilist-helper-1.42/pyproject.toml` & `anilist-helper-1.5/pyproject.toml`

 * *Files identical despite different names*

