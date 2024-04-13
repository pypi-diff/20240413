# Comparing `tmp/searchspotify-0.0.7.tar.gz` & `tmp/searchspotify-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchspotify-0.0.7.tar", last modified: Sat Apr 13 00:16:51 2024, max compression
+gzip compressed data, was "searchspotify-0.0.8.tar", last modified: Sat Apr 13 01:28:25 2024, max compression
```

## Comparing `searchspotify-0.0.7.tar` & `searchspotify-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:16:51.250307 searchspotify-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-13 00:16:47.000000 searchspotify-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-13 00:16:51.250307 searchspotify-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-13 00:16:47.000000 searchspotify-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 00:16:47.000000 searchspotify-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-13 00:16:51.254307 searchspotify-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:16:51.250307 searchspotify-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:16:51.250307 searchspotify-0.0.7/src/searchspotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-13 00:16:51.000000 searchspotify-0.0.7/src/searchspotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 00:16:51.000000 searchspotify-0.0.7/src/searchspotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:16:51.000000 searchspotify-0.0.7/src/searchspotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 00:16:51.000000 searchspotify-0.0.7/src/searchspotify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:16:51.250307 searchspotify-0.0.7/src/spotifysearch/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    22741 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-13 00:16:47.000000 searchspotify-0.0.7/src/spotifysearch/urlbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.071377 searchspotify-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-13 01:28:19.000000 searchspotify-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-13 01:28:25.071377 searchspotify-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-13 01:28:19.000000 searchspotify-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 01:28:19.000000 searchspotify-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-13 01:28:25.071377 searchspotify-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.067377 searchspotify-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.067377 searchspotify-0.0.8/src/searchspotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-13 01:28:19.000000 searchspotify-0.0.8/src/searchspotify/urlbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:25.071377 searchspotify-0.0.8/src/searchspotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 01:28:25.000000 searchspotify-0.0.8/src/searchspotify.egg-info/top_level.txt
```

### Comparing `searchspotify-0.0.7/LICENSE` & `searchspotify-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `searchspotify-0.0.7/PKG-INFO` & `searchspotify-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,137 @@
-Metadata-Version: 2.1
-Name: searchspotify
-Version: 0.0.7
-Summary: A complete wrapper for the Search API provided by Spotify written in Python.
-Home-page: https://github.com/ufoptg/SearchSpotify
-Author: True Saiyan
-Project-URL: Bug Tracker, https://github.com/ufoptg/SearchSpotify/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Spotify Search
-<p>
-    <a href="https://choosealicense.com/licenses/mit/" target="_blank">
-        <img src="https://img.shields.io/github/license/ufoptg/SearchSpotify" alt="LICENSE">
-    </a>
-    <a href="https://pypi.org/project/searchspotify/" target="_blank">
-        <img src="https://img.shields.io/pypi/v/searchspotify?color=33BBFF&label=PIP" alt="PIP">
-    </a>
-</p>
-
-SearchSpotify is a complete wrapper for the Search API provided by Spotify written in Python.
-
-It has built-in classes that helps you access the data returned by Spotify, alongside with useful methods for exporting data.
-
-Check the [documentation](https://readthedocs.org/) for more information on classes and methods.
-
-## What you can do
-- Get Spotify catalog information about albums, artists or tracks that match a keyword string.
-- Easily access the information provided by Spotify using specific class attributes and methods, such as **name**, **id**, **url** and many more.
-- Access and export audio and image files, such as album covers for example.
-
-## Installation
-SearchSpotify depends on **[requests](https://pypi.org/project/requests/)**. You can easily install it by using **PIP**
-```bash
-python -m pip install requests
-```
-
-Then, you can safely install SearchSpotify using the following command:
-```bash
-python -m pip install searchspotify
-```
-
-## Testing your installation
-You can test your installation using python interactive shell
-```python
->>> import searchspotify
-```
-
-## Getting access to the API
-To get access to Spotify Search API, you need to have a Spotify account to get an access token, which is required by the API itself. <br>
-You can [register an account](https://www.spotify.com/signup/) if you don't have one.
-
-Then, you need to login into your account in [Spotify for Developers](https://developer.spotify.com/dashboard/login).
-Once you have successfully logged in, go to your **Dashboard**, and create a new application.
-
-You should see something like this: <br>
-<p align="center"><img src="https://i.imgur.com/fWLbWUH.png"></p>
-
-Once you've created your application, you'll receive a **client ID** and a **client secret**. These are your credentials, you should store them in a **safe environment**.
-
-**IMPORTANT: You should not store your credentials inside of your code if you're planning to publish it. You should use Environment Variables instead. Check [this section](https://github.com/ufoptg/SearchSpotify#keeping-your-credentials-safe) to learn how to keep your credentials safe.**
-
-## Making your first call
-So now that you have your **credentials**, you can start making your calls to the API. 
-
-Open your editor and run the following code:
-
-```python
-# First, we import our Client class from searchspotify.client
-from searchspotify.client import Client
-
-# Then, we create an instance of that class passing our credentials as arguments.
-# IMPORTANT: Don't put your credentials inside your code if your planning to publish it.
-myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET")
-
-# Now we can call the method search() from our client and store the results in a new object.
-results = myclient.search("Never gonna give you up")
-
-# Then we call the method get_tracks() from our results object, which returns a list of tracks.
-tracks = results.get_tracks()
-
-# Now, let's access the first track in our list by using index 0.
-track = tracks[0]
-
-# Finally, we can access some information contained in our track.
-print(track.name, "-", track.artists[0].name)
-print(track.url)
-
-```
-
-**This should be your result:**
-```bash
-Never Gonna Give You Up - Rick Astley
-https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT
-```
-<br>
-
-That seems to be a lot of code, but you can simplify it a lot, like so:
-```python
-from searchspotify.client import Client
-
-myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET")
-track = myclient.search("Never gonna give you up").get_tracks()[0]
-
-print(track.name, "-", track.artists[0].name)
-
-```
-In a few lines of code, we got access to the API, retrieved some useful information of the first track in our results and displayed it.
-
-There are a lot of class attributes and methods that you can use to retrieve the information you need, you can check them out in the [documentation](https://readthedocs.org/).
-
-## Keeping your credentials safe
-As mentioned before, you should not store your credentials inside of your code. Specially if you are planning to publish it.
-
-A safer way to store them is by using Environment Variables.
-Here's a complete [tutorial](https://www.twilio.com/blog/environment-variables-python) on how to define and access environment variables using Python.
-
-## License
-This project is under the terms of the [MIT license](https://opensource.org/licenses/MIT).
+# Spotify Search
+<p>
+    <a href="https://choosealicense.com/licenses/mit/" target="_blank">
+        <img src="https://img.shields.io/github/license/ufoptg/SearchSpotify" alt="LICENSE">
+    </a>
+    <a href="https://pypi.org/project/searchspotify/" target="_blank">
+        <img src="https://img.shields.io/pypi/v/searchspotify?color=33BBFF&label=PIP" alt="PIP">
+    </a>
+</p>
+
+SearchSpotify is a complete wrapper for the Search API provided by Spotify written in Python.
+
+It has built-in classes that helps you access the data returned by Spotify, alongside with useful methods for exporting data.
+
+Check the [documentation](https://readthedocs.org/) for more information on classes and methods.
+
+## What you can do
+- Get Spotify catalog information about albums, artists or tracks that match a keyword string.
+- Easily access the information provided by Spotify using specific class attributes and methods, such as **name**, **id**, **url** and many more.
+- Access and export audio and image files, such as album covers for example.
+
+## Installation
+SearchSpotify depends on **[requests](https://pypi.org/project/requests/)**. You can easily install it by using **PIP**
+```bash
+python -m pip install requests
+```
+
+Then, you can safely install SearchSpotify using the following command:
+```bash
+python -m pip install searchspotify
+```
+
+## Testing your installation
+You can test your installation using python interactive shell
+```python
+>>> import searchspotify
+```
+
+## Getting access to the API
+To get access to Spotify Search API, you need to have a Spotify account to get an access token, which is required by the API itself. <br>
+You can [register an account](https://www.spotify.com/signup/) if you don't have one.
+
+Then, you need to login into your account in [Spotify for Developers](https://developer.spotify.com/dashboard/login).
+Once you have successfully logged in, go to your **Dashboard**, and create a new application.
+
+You should see something like this: <br>
+<p align="center"><img src="https://i.imgur.com/fWLbWUH.png"></p>
+
+Once you've created your application, you'll receive a **client ID** and a **client secret**. These are your credentials, you should store them in a **safe environment**.
+
+**IMPORTANT: You should not store your credentials inside of your code if you're planning to publish it. You should use Environment Variables instead. Check [this section](https://github.com/ufoptg/SearchSpotify#keeping-your-credentials-safe) to learn how to keep your credentials safe.**
+
+## Making your first call
+So now that you have your **credentials**, you can start making your calls to the API. 
+
+Open your editor and run the following code:
+
+```python
+# First, we import our Client class from searchspotify.client
+from searchspotify import Client
+
+# Then, we create an instance of that class passing our credentials as arguments.
+# IMPORTANT: Don't put your credentials inside your code if your planning to publish it.
+myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET")
+
+# Now we can call the method search() from our client and store the results in a new object.
+results = myclient.search("Never gonna give you up")
+
+# Then we call the method get_tracks() from our results object, which returns a list of tracks.
+tracks = results.get_tracks()
+
+# Now, let's access the first track in our list by using index 0.
+track = tracks[0]
+
+# Finally, we can access some information contained in our track.
+print(track.name, "-", track.artists[0].name)
+print(track.url)
+
+#Using Album or Playlist links
+playlist = myclient.search("https://open.spotify.com/playlist/37i9dQZEVXbmHwm9TPg9pf?si=fUjIaGonRlW3GfkZ9kuxFg")
+
+p(f"Playlist title: {playlist.playlist_name}")
+p(f"total tracks: {playlist.total_tracks}")
+p(f"description: {playlist.description}")
+p(f"total duration: {playlist.total_duration()}")
+for track in playlist.tracks:
+    print("Track Name:", track.track_name)
+    print("Track URL:", track.spotify_url)
+    print("Duration:", track.get_string_duration())
+
+
+album = myclient.search("https://open.spotify.com/album/5nUuEb92id5CtdQCtOs7a1")
+
+print("Album Name:", album.album_name)
+print("Album Label:", album.label)
+print("Album popularity:", album.popularity)
+print("Album Thumb:", album.thumbnail_url)
+print("Artists:", album.artists)
+print("Release Date:", album.release_date)
+print("Total Tracks:", album.total_tracks)
+print("Total Duration:", album.total_duration_string())
+for track in album.tracks:
+    print("Track Name:", track.track_name)
+    print("Track Number:", track.track_number)
+    print("Track URL:", track.spotify_url)
+    print("Duration:", track.get_string_duration())
+```
+
+**This should be your result:**
+```bash
+Never Gonna Give You Up - Rick Astley
+https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT
+```
+<br>
+
+That seems to be a lot of code, but you can simplify it a lot, like so:
+```python
+from searchspotify.client import Client
+
+myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET")
+track = myclient.search("Never gonna give you up").get_tracks()[0]
+
+print(track.name, "-", track.artists[0].name)
+
+```
+In a few lines of code, we got access to the API, retrieved some useful information of the first track in our results and displayed it.
+
+There are a lot of class attributes and methods that you can use to retrieve the information you need, you can check them out in the [documentation](https://readthedocs.org/).
+
+## Keeping your credentials safe
+As mentioned before, you should not store your credentials inside of your code. Specially if you are planning to publish it.
+
+A safer way to store them is by using Environment Variables.
+Here's a complete [tutorial](https://www.twilio.com/blog/environment-variables-python) on how to define and access environment variables using Python.
+
+## License
+This project is under the terms of the [MIT license](https://opensource.org/licenses/MIT).
```

#### html2text {}

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1 Name: searchspotify Version: 0.0.7 Summary: A complete
-wrapper for the Search API provided by Spotify written in Python. Home-page:
-https://github.com/ufoptg/SearchSpotify Author: True Saiyan Project-URL: Bug
-Tracker, https://github.com/ufoptg/SearchSpotify/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Spotify Search
+# Spotify Search
 _[_L_I_C_E_N_S_E_]_[_P_I_P_]
 SearchSpotify is a complete wrapper for the Search API provided by Spotify
 written in Python. It has built-in classes that helps you access the data
 returned by Spotify, alongside with useful methods for exporting data. Check
 the [documentation](https://readthedocs.org/) for more information on classes
 and methods. ## What you can do - Get Spotify catalog information about albums,
 artists or tracks that match a keyword string. - Easily access the information
@@ -34,26 +28,41 @@
 **safe environment**. **IMPORTANT: You should not store your credentials inside
 of your code if you're planning to publish it. You should use Environment
 Variables instead. Check [this section](https://github.com/ufoptg/
 SearchSpotify#keeping-your-credentials-safe) to learn how to keep your
 credentials safe.** ## Making your first call So now that you have your
 **credentials**, you can start making your calls to the API. Open your editor
 and run the following code: ```python # First, we import our Client class from
-searchspotify.client from searchspotify.client import Client # Then, we create
-an instance of that class passing our credentials as arguments. # IMPORTANT:
-Don't put your credentials inside your code if your planning to publish it.
-myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") # Now we can call the
-method search() from our client and store the results in a new object. results
-= myclient.search("Never gonna give you up") # Then we call the method
-get_tracks() from our results object, which returns a list of tracks. tracks =
+searchspotify.client from searchspotify import Client # Then, we create an
+instance of that class passing our credentials as arguments. # IMPORTANT: Don't
+put your credentials inside your code if your planning to publish it. myclient
+= Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") # Now we can call the method
+search() from our client and store the results in a new object. results =
+myclient.search("Never gonna give you up") # Then we call the method get_tracks
+() from our results object, which returns a list of tracks. tracks =
 results.get_tracks() # Now, let's access the first track in our list by using
 index 0. track = tracks[0] # Finally, we can access some information contained
 in our track. print(track.name, "-", track.artists[0].name) print(track.url)
-``` **This should be your result:** ```bash Never Gonna Give You Up - Rick
-Astley https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT ```
+#Using Album or Playlist links playlist = myclient.search("https://
+open.spotify.com/playlist/37i9dQZEVXbmHwm9TPg9pf?si=fUjIaGonRlW3GfkZ9kuxFg") p
+(f"Playlist title: {playlist.playlist_name}") p(f"total tracks:
+{playlist.total_tracks}") p(f"description: {playlist.description}") p(f"total
+duration: {playlist.total_duration()}") for track in playlist.tracks: print
+("Track Name:", track.track_name) print("Track URL:", track.spotify_url) print
+("Duration:", track.get_string_duration()) album = myclient.search("https://
+open.spotify.com/album/5nUuEb92id5CtdQCtOs7a1") print("Album Name:",
+album.album_name) print("Album Label:", album.label) print("Album popularity:",
+album.popularity) print("Album Thumb:", album.thumbnail_url) print("Artists:",
+album.artists) print("Release Date:", album.release_date) print("Total Tracks:
+", album.total_tracks) print("Total Duration:", album.total_duration_string())
+for track in album.tracks: print("Track Name:", track.track_name) print("Track
+Number:", track.track_number) print("Track URL:", track.spotify_url) print
+("Duration:", track.get_string_duration()) ``` **This should be your result:**
+```bash Never Gonna Give You Up - Rick Astley https://open.spotify.com/track/
+4cOdK2wGLETKBW3PvgPWqT ```
 That seems to be a lot of code, but you can simplify it a lot, like so:
 ```python from searchspotify.client import Client myclient = Client
 ("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") track = myclient.search("Never gonna
 give you up").get_tracks()[0] print(track.name, "-", track.artists[0].name) ```
 In a few lines of code, we got access to the API, retrieved some useful
 information of the first track in our results and displayed it. There are a lot
 of class attributes and methods that you can use to retrieve the information
```

### Comparing `searchspotify-0.0.7/setup.cfg` & `searchspotify-0.0.8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = searchspotify
-version = 0.0.7
+version = 0.0.8
 author = True Saiyan
 description = A complete wrapper for the Search API provided by Spotify written in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ufoptg/SearchSpotify
 project_urls = 
 	Bug Tracker = https://github.com/ufoptg/SearchSpotify/issues
```

### Comparing `searchspotify-0.0.7/src/searchspotify.egg-info/PKG-INFO` & `searchspotify-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchspotify
-Version: 0.0.7
+Version: 0.0.8
 Summary: A complete wrapper for the Search API provided by Spotify written in Python.
 Home-page: https://github.com/ufoptg/SearchSpotify
 Author: True Saiyan
 Project-URL: Bug Tracker, https://github.com/ufoptg/SearchSpotify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,15 +67,15 @@
 ## Making your first call
 So now that you have your **credentials**, you can start making your calls to the API. 
 
 Open your editor and run the following code:
 
 ```python
 # First, we import our Client class from searchspotify.client
-from searchspotify.client import Client
+from searchspotify import Client
 
 # Then, we create an instance of that class passing our credentials as arguments.
 # IMPORTANT: Don't put your credentials inside your code if your planning to publish it.
 myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET")
 
 # Now we can call the method search() from our client and store the results in a new object.
 results = myclient.search("Never gonna give you up")
@@ -86,14 +86,42 @@
 # Now, let's access the first track in our list by using index 0.
 track = tracks[0]
 
 # Finally, we can access some information contained in our track.
 print(track.name, "-", track.artists[0].name)
 print(track.url)
 
+#Using Album or Playlist links
+playlist = myclient.search("https://open.spotify.com/playlist/37i9dQZEVXbmHwm9TPg9pf?si=fUjIaGonRlW3GfkZ9kuxFg")
+
+p(f"Playlist title: {playlist.playlist_name}")
+p(f"total tracks: {playlist.total_tracks}")
+p(f"description: {playlist.description}")
+p(f"total duration: {playlist.total_duration()}")
+for track in playlist.tracks:
+    print("Track Name:", track.track_name)
+    print("Track URL:", track.spotify_url)
+    print("Duration:", track.get_string_duration())
+
+
+album = myclient.search("https://open.spotify.com/album/5nUuEb92id5CtdQCtOs7a1")
+
+print("Album Name:", album.album_name)
+print("Album Label:", album.label)
+print("Album popularity:", album.popularity)
+print("Album Thumb:", album.thumbnail_url)
+print("Artists:", album.artists)
+print("Release Date:", album.release_date)
+print("Total Tracks:", album.total_tracks)
+print("Total Duration:", album.total_duration_string())
+for track in album.tracks:
+    print("Track Name:", track.track_name)
+    print("Track Number:", track.track_number)
+    print("Track URL:", track.spotify_url)
+    print("Duration:", track.get_string_duration())
 ```
 
 **This should be your result:**
 ```bash
 Never Gonna Give You Up - Rick Astley
 https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: searchspotify Version: 0.0.7 Summary: A complete
+Metadata-Version: 2.1 Name: searchspotify Version: 0.0.8 Summary: A complete
 wrapper for the Search API provided by Spotify written in Python. Home-page:
 https://github.com/ufoptg/SearchSpotify Author: True Saiyan Project-URL: Bug
 Tracker, https://github.com/ufoptg/SearchSpotify/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Spotify Search
 _[_L_I_C_E_N_S_E_]_[_P_I_P_]
@@ -34,26 +34,41 @@
 **safe environment**. **IMPORTANT: You should not store your credentials inside
 of your code if you're planning to publish it. You should use Environment
 Variables instead. Check [this section](https://github.com/ufoptg/
 SearchSpotify#keeping-your-credentials-safe) to learn how to keep your
 credentials safe.** ## Making your first call So now that you have your
 **credentials**, you can start making your calls to the API. Open your editor
 and run the following code: ```python # First, we import our Client class from
-searchspotify.client from searchspotify.client import Client # Then, we create
-an instance of that class passing our credentials as arguments. # IMPORTANT:
-Don't put your credentials inside your code if your planning to publish it.
-myclient = Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") # Now we can call the
-method search() from our client and store the results in a new object. results
-= myclient.search("Never gonna give you up") # Then we call the method
-get_tracks() from our results object, which returns a list of tracks. tracks =
+searchspotify.client from searchspotify import Client # Then, we create an
+instance of that class passing our credentials as arguments. # IMPORTANT: Don't
+put your credentials inside your code if your planning to publish it. myclient
+= Client("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") # Now we can call the method
+search() from our client and store the results in a new object. results =
+myclient.search("Never gonna give you up") # Then we call the method get_tracks
+() from our results object, which returns a list of tracks. tracks =
 results.get_tracks() # Now, let's access the first track in our list by using
 index 0. track = tracks[0] # Finally, we can access some information contained
 in our track. print(track.name, "-", track.artists[0].name) print(track.url)
-``` **This should be your result:** ```bash Never Gonna Give You Up - Rick
-Astley https://open.spotify.com/track/4cOdK2wGLETKBW3PvgPWqT ```
+#Using Album or Playlist links playlist = myclient.search("https://
+open.spotify.com/playlist/37i9dQZEVXbmHwm9TPg9pf?si=fUjIaGonRlW3GfkZ9kuxFg") p
+(f"Playlist title: {playlist.playlist_name}") p(f"total tracks:
+{playlist.total_tracks}") p(f"description: {playlist.description}") p(f"total
+duration: {playlist.total_duration()}") for track in playlist.tracks: print
+("Track Name:", track.track_name) print("Track URL:", track.spotify_url) print
+("Duration:", track.get_string_duration()) album = myclient.search("https://
+open.spotify.com/album/5nUuEb92id5CtdQCtOs7a1") print("Album Name:",
+album.album_name) print("Album Label:", album.label) print("Album popularity:",
+album.popularity) print("Album Thumb:", album.thumbnail_url) print("Artists:",
+album.artists) print("Release Date:", album.release_date) print("Total Tracks:
+", album.total_tracks) print("Total Duration:", album.total_duration_string())
+for track in album.tracks: print("Track Name:", track.track_name) print("Track
+Number:", track.track_number) print("Track URL:", track.spotify_url) print
+("Duration:", track.get_string_duration()) ``` **This should be your result:**
+```bash Never Gonna Give You Up - Rick Astley https://open.spotify.com/track/
+4cOdK2wGLETKBW3PvgPWqT ```
 That seems to be a lot of code, but you can simplify it a lot, like so:
 ```python from searchspotify.client import Client myclient = Client
 ("YOUR_CLIENT_ID", "YOUR_CLIENT_SECRET") track = myclient.search("Never gonna
 give you up").get_tracks()[0] print(track.name, "-", track.artists[0].name) ```
 In a few lines of code, we got access to the API, retrieved some useful
 information of the first track in our results and displayed it. There are a lot
 of class attributes and methods that you can use to retrieve the information
```

### Comparing `searchspotify-0.0.7/src/spotifysearch/__init__.py` & `searchspotify-0.0.8/src/searchspotify/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
-# Nimbus ~ UserBot
-# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-# This file is a part of < https://github.com/ufoptg/Nimbus/ >
-# PLease read the GNU Affero General Public License in
-# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
-# If not, see <https://www.gnu.org/licenses/>.
-
-
-from .classes import *
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
+# Nimbus ~ UserBot
+# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# This file is a part of < https://github.com/ufoptg/Nimbus/ >
+# PLease read the GNU Affero General Public License in
+# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
+# If not, see <https://www.gnu.org/licenses/>.
+
+
+from .classes import *
 from .client import Client
```

### Comparing `searchspotify-0.0.7/src/spotifysearch/calls.py` & `searchspotify-0.0.8/src/searchspotify/calls.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
-# Nimbus ~ UserBot
-# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-# This file is a part of < https://github.com/ufoptg/Nimbus/ >
-# PLease read the GNU Affero General Public License in
-# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
-# If not, see <https://www.gnu.org/licenses/>.
-
-# THIS FILE IS RESPONSABLE FOR API CALLS
-
-from requests import get, post
-
-from . import urlbuilder
-
-
-def call_acess_token(credentials):
-    """
-    Calls Spotify API to obtain an access token using client credentials.
-
-    :param credentials: Encoded client credentials.
-    :return: Response object containing the access token.
-    """
-    endpoint = "https://accounts.spotify.com/api/token"
-    data = {"grant_type": "client_credentials"}
-    headers = {"Authorization": f"Basic {credentials}"}
-    return post(url=endpoint, data=data, headers=headers)
-
-
-def call_search(acess_token, args):
-    """
-    Calls Spotify API to search for entities using the provided access token and arguments.
-
-    :param access_token: Access token for authentication.
-    :param args: Tuple of arguments for the search endpoint.
-    :return: Response object containing the search results.
-    """
-    endpoint = urlbuilder.search_endpoint(*args)
-    headers = {"Authorization": f"Bearer {acess_token}"}
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
+# Nimbus ~ UserBot
+# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# This file is a part of < https://github.com/ufoptg/Nimbus/ >
+# PLease read the GNU Affero General Public License in
+# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
+# If not, see <https://www.gnu.org/licenses/>.
+
+# THIS FILE IS RESPONSABLE FOR API CALLS
+
+from requests import get, post
+
+from . import urlbuilder
+
+
+def call_acess_token(credentials):
+    """
+    Calls Spotify API to obtain an access token using client credentials.
+
+    :param credentials: Encoded client credentials.
+    :return: Response object containing the access token.
+    """
+    endpoint = "https://accounts.spotify.com/api/token"
+    data = {"grant_type": "client_credentials"}
+    headers = {"Authorization": f"Basic {credentials}"}
+    return post(url=endpoint, data=data, headers=headers)
+
+
+def call_search(acess_token, args):
+    """
+    Calls Spotify API to search for entities using the provided access token and arguments.
+
+    :param access_token: Access token for authentication.
+    :param args: Tuple of arguments for the search endpoint.
+    :return: Response object containing the search results.
+    """
+    endpoint = urlbuilder.search_endpoint(*args)
+    headers = {"Authorization": f"Bearer {acess_token}"}
     return get(url=endpoint, headers=headers)
```

### Comparing `searchspotify-0.0.7/src/spotifysearch/classes.py` & `searchspotify-0.0.8/src/searchspotify/classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,767 +1,768 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
-# Nimbus ~ UserBot
-# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-# This file is a part of < https://github.com/ufoptg/Nimbus/ >
-# PLease read the GNU Affero General Public License in
-# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
-# If not, see <https://www.gnu.org/licenses/>.
-
-# THIS FILE IS RESPONSABLE FOR MANY CLASS DECLARATIONS
-
-import json
-import math
-from base64 import b64encode
-from urllib.request import urlretrieve
-
-from . import calls, constructor
-
-
-class Authenticator:
-    """
-    Handles authentication and token retrieval for Spotify API.
-    """
-
-    def __init__(self, client_id: str, client_secret: str):
-        """
-        Initializes the Authenticator with client credentials.
-
-        :param client_id: Spotify client ID.
-        :param client_secret: Spotify client secret.
-        """
-        self.credentials = self.encode_credentials(client_id, client_secret)
-
-    def encode_credentials(self, client_id, client_secret):
-        """
-        Encodes client credentials for token retrieval.
-
-        :param client_id: Spotify client ID.
-        :param client_secret: Spotify client secret.
-        :return: Encoded credentials.
-        """
-        credentials = f"{client_id}:{client_secret}"
-        encoded_credentials = b64encode(credentials.encode("utf-8"))
-        return str(encoded_credentials, "utf-8")
-
-    def get_acess_token(self):
-        """
-        Retrieves access token using encoded credentials.
-
-        :return: Access token.
-        """
-        response = calls.call_acess_token(self.credentials)
-        return response.json()["access_token"]
-
-
-# OBJECTS
-# Base class for all classes
-class Base:
-    """
-    Base class for all Spotify API objects.
-    """
-
-    def __init__(self, data, type, name, url, id):
-        """
-        Initializes Base object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the object.
-        :param url: URL of the object.
-        :param id: ID of the object.
-        """
-        self.data = data
-        self.type = type
-        self.name = name
-        self.url = url
-        self.id = id
-
-    def export_json(self, path: str):
-        """
-        Exports object data to JSON file.
-
-        :param path: File path.
-        """
-        file = open(path, "w")
-        json.dump(self.data, file, indent=4)
-        file.close()
-
-
-class TrackBase(Base):
-    """
-    Base class for track-like Spotify API objects.
-    """
-
-    def __init__(self, data, type, name, url, id, explicit, duration_ms):
-        """
-        Initializes TrackBase object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the object.
-        :param url: URL of the object.
-        :param id: ID of the object.
-        :param explicit: Explicit content indicator.
-        :param duration_ms: Duration of the object in milliseconds.
-        """
-        super().__init__(data, type, name, url, id)
-        self.explicit = explicit
-        self.duration_ms = duration_ms
-
-    def get_formatted_duration(self) -> dict:
-        """
-        Gets the formatted duration of the object.
-
-        :return: Dictionary containing hours, minutes, and seconds.
-        """
-        duration_in_seconds = self.duration_ms / 1000
-        hours = 0
-        mins = math.floor(duration_in_seconds // 60)
-
-        if mins >= 60:
-            hours = math.floor(mins // 60)
-            mins = math.floor(mins % 60)
-
-        secs = math.floor(duration_in_seconds % 60)
-
-        return {"hours": hours, "minutes": mins, "seconds": secs}
-
-    def get_string_duration(self) -> str:
-        """
-        Gets the duration of the object as a formatted string.
-
-        :return: Formatted duration string.
-        """
-        duration = self.get_formatted_duration()
-        format = self.__format_duration
-
-        hours = format(str(duration["hours"]))
-        mins = format(str(duration["minutes"]))
-        secs = format(str(duration["seconds"]))
-
-        if int(hours):
-            return f"{hours}:{mins}:{secs}"
-        else:
-            return f"{mins}:{secs}"
-
-    def __format_duration(self, value: str):
-        """
-        Formats duration value.
-
-        :param value: Value to format.
-        :return: Formatted value.
-        """
-        if len(value) < 2:
-            return "0" + value
-        else:
-            return value
-
-
-class Artist(Base):
-    """
-    Represents an artist on Spotify.
-    """
-
-    def __init__(self, data: dict, type: str, name: str, url: str, id: str):
-        """
-        Initializes Artist object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the artist.
-        :param url: URL of the artist.
-        :param id: ID of the artist.
-        """
-        super().__init__(data, type, name, url, id)
-
-
-class AlbumCover:
-    """
-    Represents the cover image of an album.
-    """
-
-    def __init__(self, width, height, url):
-        """
-        Initializes AlbumCover object.
-
-        :param width: Width of the image.
-        :param height: Height of the image.
-        :param url: URL of the image.
-        """
-        self.width = width
-        self.height = height
-        self.url = url
-
-    def export_image(self, path):
-        """
-        Exports the image to a file.
-
-        :param path: File path.
-        """
-        urlretrieve(self.url, path)
-
-
-class Album(Base):
-    """
-    Represents an album on Spotify.
-    """
-
-    def __init__(
-        self,
-        data: dict,
-        type: str,
-        name: str,
-        url: str,
-        id: str,
-        images: list,
-        artists: list,
-        available_markets: list,
-        release_date: str,
-        total_tracks: int,
-    ):
-        """
-        Initializes Album object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the album.
-        :param url: URL of the album.
-        :param id: ID of the album.
-        :param images: List of album cover images.
-        :param artists: List of artists associated with the album.
-        :param available_markets: List of available markets.
-        :param release_date: Release date of the album.
-        :param total_tracks: Total number of tracks in the album.
-        """
-        super().__init__(data, type, name, url, id)
-        self.images = images
-        self.artists = artists
-        self.available_markets = available_markets
-        self.release_date = release_date
-        self.total_tracks = total_tracks
-
-
-class AlbumTrack:
-    """
-    Represents a track in an album.
-    """
-
-    def __init__(self, track_data):
-        """
-        Initializes AlbumTrack object.
-
-        :param track_data: Data dictionary for the track.
-        """
-        self.spotify_url = track_data.get("external_urls", {}).get("spotify")
-        self.track_name = track_data.get("name")
-        self.artists = ", ".join(
-            artist.get("name", "") for artist in track_data.get("artists", [])
-        )
-        self.track_number = track_data.get("track_number")
-        self.duration_ms = track_data.get("duration_ms", 0)
-
-    def get_formatted_duration(self) -> dict:
-        """
-        Gets the formatted duration of the object.
-
-        :return: Dictionary containing hours, minutes, and seconds.
-        """
-        duration_in_seconds = self.duration_ms / 1000
-        hours = 0
-        mins = math.floor(duration_in_seconds // 60)
-
-        if mins >= 60:
-            hours = math.floor(mins // 60)
-            mins = math.floor(mins % 60)
-
-        secs = math.floor(duration_in_seconds % 60)
-
-        return {"hours": hours, "minutes": mins, "seconds": secs}
-
-    def get_string_duration(self) -> str:
-        """
-        Gets the duration of the object as a formatted string.
-
-        :return: Formatted duration string.
-        """
-        duration = self.get_formatted_duration()
-        format = self.__format_duration
-
-        hours = format(str(duration["hours"]))
-        mins = format(str(duration["minutes"]))
-        secs = format(str(duration["seconds"]))
-
-        if int(hours):
-            return f"{hours}:{mins}:{secs}"
-        else:
-            return f"{mins}:{secs}"
-
-    def __format_duration(self, value: str):
-        """
-        Formats duration value.
-
-        :param value: Value to format.
-        :return: Formatted value.
-        """
-        if len(value) < 2:
-            return "0" + value
-        else:
-            return value
-
-
-class Albums:
-    """
-    Represents an album.
-    """
-
-    def __init__(self, album_data):
-        """
-        Initializes Album object.
-
-        :param album_data: Data dictionary for the album.
-        """
-        self.album_name = album_data.get("name", "Unknown Album")
-        self.artists = ", ".join(
-            artist.get("name", "") for artist in album_data.get("artists", [])
-        )
-        self.release_date = album_data.get("release_date")
-        self.total_tracks = album_data.get("total_tracks", 0)
-        self.thumbnail_url = (
-            album_data.get("images", [])[0].get("url")
-            if album_data.get("images")
-            else None
-        )
-        self.label = album_data.get("label")
-        self.popularity = album_data.get("popularity")
-        self.tracks = [
-            AlbumTrack(track) for track in album_data.get("tracks", {}).get("items", [])
-        ]
-
-    def total_duration(self):
-        """
-        Calculate the total duration of all tracks in the album.
-
-        :return: Total duration as a formatted string.
-        """
-        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
-        hours = int(total_seconds // 3600)
-        minutes = int((total_seconds % 3600) // 60)
-        seconds = int(total_seconds % 60)
-        return f"{hours}:{minutes}:{seconds}"
-
-    def total_duration_string(self):
-        """
-        Calculate the total duration of all tracks in the album as a formatted string.
-
-        :return: Total duration as a formatted string.
-        """
-        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
-        total_duration_track = AlbumTrack({"duration_ms": total_seconds * 1000})
-        return total_duration_track.get_string_duration()
-
-
-class TrackPreview:
-    """
-    Represents a preview of a track.
-    """
-
-    def __init__(self, url):
-        """
-        Initializes TrackPreview object.
-
-        :param url: URL of the track preview.
-        """
-        self.url = url
-
-    def export_audio(self, path):
-        """
-        Exports the audio preview to a file.
-
-        :param path: File path.
-        """
-        urlretrieve(self.url, path)
-
-
-class Track(TrackBase):
-    """
-    Represents a track on Spotify.
-    """
-
-    def __init__(
-        self,
-        data: dict,
-        type: str,
-        name: str,
-        url: str,
-        id: str,
-        explicit: bool,
-        duration_ms: int,
-        preview: TrackPreview,
-        artists: list,
-        album: Album,
-        available_markets: list,
-        disc_number: int,
-        popularity: int,
-    ):
-        """
-        Initializes Track object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the track.
-        :param url: URL of the track.
-        :param id: ID of the track.
-        :param explicit: Explicit content indicator.
-        :param duration_ms: Duration of the track in milliseconds.
-        :param preview: Track preview object.
-        :param artists: List of artists associated with the track.
-        :param album: Album object associated with the track.
-        :param available_markets: List of available markets.
-        :param disc_number: Disc number of the track.
-        :param popularity: Popularity of the track.
-        """
-        super().__init__(data, type, name, url, id, explicit, duration_ms)
-        self.preview = preview
-        self.artists = artists
-        self.album = album
-        self.available_markets = available_markets
-        self.disc_number = disc_number
-        self.popularity = popularity
-
-
-class Episode(TrackBase):
-    """
-    Represents an episode on Spotify.
-    """
-
-    def __init__(
-        self,
-        data: dict,
-        type: str,
-        name: str,
-        url: str,
-        id: str,
-        explicit: bool,
-        duration_ms: int,
-        preview: str,
-        description: str,
-        html_description: str,
-        images: list,
-        language: str,
-        languages: list,
-        release_date: str,
-    ):
-        """
-        Initializes Episode object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the episode.
-        :param url: URL of the episode.
-        :param id: ID of the episode.
-        :param explicit: Explicit content indicator.
-        :param duration_ms: Duration of the episode in milliseconds.
-        :param preview: URL of the episode preview.
-        :param description: Description of the episode.
-        :param html_description: HTML description of the episode.
-        :param images: List of images associated with the episode.
-        :param language: Language of the episode.
-        :param languages: List of languages available for the episode.
-        :param release_date: Release date of the episode.
-        """
-        super().__init__(data, type, name, url, id, explicit, duration_ms)
-        self.preview = preview
-        self.description = description
-        self.html_description = html_description
-        self.images = images
-        self.language = language
-        self.languages = languages
-        self.release_date = release_date
-
-
-class Playlist(Base):
-    """
-    Represents a playlist on Spotify.
-    """
-
-    def __init__(
-        self,
-        data: dict,
-        type: str,
-        name: str,
-        url: str,
-        id: str,
-        description: str,
-        images: list,
-        tracks: list,
-        public: bool,
-        total_tracks: int,
-    ):
-        """
-        Initializes Playlist object.
-
-        :param data: Data dictionary.
-        :param type: Object type.
-        :param name: Name of the playlist.
-        :param url: URL of the playlist.
-        :param id: ID of the playlist.
-        :param description: Description of the playlist.
-        :param images: List of images associated with the playlist.
-        :param tracks: List of tracks in the playlist.
-        :param public: Public visibility indicator.
-        """
-        super().__init__(data, type, name, url, id)
-        self.description = description
-        self.images = images
-        self.tracks = tracks
-        self.public = public
-        self.total_tracks = total_tracks
-
-
-class PlaylistTrack:
-    """
-    Represents a track in a playlist.
-    """
-
-    def __init__(self, track_data):
-        """
-        Initializes PlaylistTrack object.
-
-        :param track_data: Data dictionary for the track.
-        """
-        self.spotify_url = track_data.get("external_urls", {}).get("spotify")
-        self.track_name = track_data.get("name")
-        self.artists = ", ".join(
-            artist.get("name", "") for artist in track_data.get("artists", [])
-        )
-        self.album = track_data.get("album", {}).get("name")
-        self.release_date = track_data.get("album", {}).get("release_date")
-        self.preview_url = track_data.get("preview_url")
-        self.thumbnail_url = track_data.get("album", {}).get("images", [])[0].get("url")
-        self.duration_ms = track_data.get("duration_ms", 0)
-
-    def get_formatted_duration(self) -> dict:
-        """
-        Gets the formatted duration of the object.
-
-        :return: Dictionary containing hours, minutes, and seconds.
-        """
-        duration_in_seconds = self.duration_ms / 1000
-        hours = 0
-        mins = math.floor(duration_in_seconds // 60)
-
-        if mins >= 60:
-            hours = math.floor(mins // 60)
-            mins = math.floor(mins % 60)
-
-        secs = math.floor(duration_in_seconds % 60)
-
-        return {"hours": hours, "minutes": mins, "seconds": secs}
-
-    def get_string_duration(self) -> str:
-        """
-        Gets the duration of the object as a formatted string.
-
-        :return: Formatted duration string.
-        """
-        duration = self.get_formatted_duration()
-        format = self.__format_duration
-
-        hours = format(str(duration["hours"]))
-        mins = format(str(duration["minutes"]))
-        secs = format(str(duration["seconds"]))
-
-        if int(hours):
-            return f"{hours}:{mins}:{secs}"
-        else:
-            return f"{mins}:{secs}"
-
-    def __format_duration(self, value: str):
-        """
-        Formats duration value.
-
-        :param value: Value to format.
-        :return: Formatted value.
-        """
-        if len(value) < 2:
-            return "0" + value
-        else:
-            return value
-
-
-class Playlists:
-    """
-    Represents a collection of playlists.
-    """
-
-    def __init__(self, playlist_data):
-        """
-        Initializes Playlists object.
-
-        :param playlist_data: Data dictionary for the playlists.
-        """
-        self.playlist_name = playlist_data.get("name", "Unknown Playlist")
-        self.description = playlist_data.get("description", "")
-        self.total_tracks = playlist_data.get("tracks", {}).get("total", 0)
-        self.tracks = [
-            PlaylistTrack(item.get("track"))
-            for item in playlist_data.get("tracks", {}).get("items", [])
-        ]
-
-    def total_duration(self):
-        """
-        Calculate the total duration of all tracks in the playlist.
-
-        :return: Total duration as a string.
-        """
-        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
-        hours = int(total_seconds // 3600)
-        minutes = int((total_seconds % 3600) // 60)
-        seconds = int(total_seconds % 60)
-        return f"{hours}:{minutes}:{seconds}"
-
-    def total_duration_string(self):
-        """
-        Calculate the total duration of all tracks in the album as a formatted string.
-
-        :return: Total duration as a formatted string.
-        """
-        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
-        total_duration_track = PlaylistTrack({"duration_ms": total_seconds * 1000})
-        return total_duration_track.get_string_duration()
-
-
-# CLIENT OBJECTS
-
-
-class Results(Base):
-    """
-    Represents results obtained from Spotify API.
-    """
-
-    def __init__(self, data):
-        """
-        Initializes Results object.
-
-        :param data: Data dictionary.
-        """
-        self.data = data
-
-    def __get_items(self, type):
-        """
-        Retrieves items from the data dictionary based on the type.
-
-        :param type: Type of items to retrieve.
-        :return: List of items.
-        """
-        if type == "artist":
-            try:
-                data = self.data["artists"]["items"]
-                func = constructor.artist
-            except KeyError:
-                return []
-
-        elif type == "track":
-            try:
-                data = self.data["tracks"]["items"]
-                func = constructor.track
-            except KeyError:
-                return []
-
-        elif type == "album":
-            try:
-                data = [item["album"] for item in self.data["tracks"]["items"]]
-                func = constructor.album
-            except KeyError:
-                return []
-
-        elif type == "episode":
-            try:
-                data = self.data["episodes"]["items"]
-                func = constructor.episode
-            except KeyError:
-                return []
-
-        elif type == "playlist":
-            try:
-                data = self.data["playlists"]["items"]
-                func = constructor.playlist
-            except KeyError:
-                return []
-
-        return [func(item) for item in data]
-
-    def get_playlist(self) -> "Playlists":
-        """
-        Retrieves playlist items from the results.
-
-        :return: Playlists object.
-        """
-        try:
-            playlist_data = self.data
-            return Playlists(playlist_data)
-        except KeyError:
-            return None
-
-    def get_album(self) -> "Albums":
-        """
-        Retrieves album items from the results.
-
-        :return: Albums object.
-        """
-        try:
-            album_data = self.data
-            return Albums(album_data)
-        except KeyError:
-            return None
-
-    def get_tracks(self) -> list:
-        """
-        Retrieves track items from the results.
-
-        :return: List of track items.
-        """
-        return self.__get_items("track")
-
-    def get_artists(self) -> list:
-        """
-        Retrieves artist items from the results.
-
-        :return: List of artist items.
-        """
-        return self.__get_items("artist")
-
-    def get_albums(self) -> list:
-        """
-        Retrieves album items from the results.
-
-        :return: List of album items.
-        """
-        return self.__get_items("album")
-
-    def get_episodes(self) -> list:
-        """
-        Retrieves episode items from the results.
-
-        :return: List of episode items.
-        """
-        return self.__get_items("episode")
-
-    def get_playlists(self) -> list:
-        """
-        Retrieves playlist items from the results.
-
-        :return: List of playlist items.
-        """
-        return self.__get_items("playlist")
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
+# Nimbus ~ UserBot
+# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# This file is a part of < https://github.com/ufoptg/Nimbus/ >
+# PLease read the GNU Affero General Public License in
+# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
+# If not, see <https://www.gnu.org/licenses/>.
+
+# THIS FILE IS RESPONSABLE FOR MANY CLASS DECLARATIONS
+
+import json
+import math
+from base64 import b64encode
+from urllib.request import urlretrieve
+
+from . import calls, constructor
+
+
+class Authenticator:
+    """
+    Handles authentication and token retrieval for Spotify API.
+    """
+
+    def __init__(self, client_id: str, client_secret: str):
+        """
+        Initializes the Authenticator with client credentials.
+
+        :param client_id: Spotify client ID.
+        :param client_secret: Spotify client secret.
+        """
+        self.credentials = self.encode_credentials(client_id, client_secret)
+
+    def encode_credentials(self, client_id, client_secret):
+        """
+        Encodes client credentials for token retrieval.
+
+        :param client_id: Spotify client ID.
+        :param client_secret: Spotify client secret.
+        :return: Encoded credentials.
+        """
+        credentials = f"{client_id}:{client_secret}"
+        encoded_credentials = b64encode(credentials.encode("utf-8"))
+        return str(encoded_credentials, "utf-8")
+
+    def get_acess_token(self):
+        """
+        Retrieves access token using encoded credentials.
+
+        :return: Access token.
+        """
+        response = calls.call_acess_token(self.credentials)
+        return response.json()["access_token"]
+
+
+# OBJECTS
+# Base class for all classes
+class Base:
+    """
+    Base class for all Spotify API objects.
+    """
+
+    def __init__(self, data, type, name, url, id):
+        """
+        Initializes Base object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the object.
+        :param url: URL of the object.
+        :param id: ID of the object.
+        """
+        self.data = data
+        self.type = type
+        self.name = name
+        self.url = url
+        self.id = id
+
+    def export_json(self, path: str):
+        """
+        Exports object data to JSON file.
+
+        :param path: File path.
+        """
+        file = open(path, "w")
+        json.dump(self.data, file, indent=4)
+        file.close()
+
+
+class TrackBase(Base):
+    """
+    Base class for track-like Spotify API objects.
+    """
+
+    def __init__(self, data, type, name, url, id, explicit, duration_ms):
+        """
+        Initializes TrackBase object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the object.
+        :param url: URL of the object.
+        :param id: ID of the object.
+        :param explicit: Explicit content indicator.
+        :param duration_ms: Duration of the object in milliseconds.
+        """
+        super().__init__(data, type, name, url, id)
+        self.explicit = explicit
+        self.duration_ms = duration_ms
+
+    def get_formatted_duration(self) -> dict:
+        """
+        Gets the formatted duration of the object.
+
+        :return: Dictionary containing hours, minutes, and seconds.
+        """
+        duration_in_seconds = self.duration_ms / 1000
+        hours = 0
+        mins = math.floor(duration_in_seconds // 60)
+
+        if mins >= 60:
+            hours = math.floor(mins // 60)
+            mins = math.floor(mins % 60)
+
+        secs = math.floor(duration_in_seconds % 60)
+
+        return {"hours": hours, "minutes": mins, "seconds": secs}
+
+    def get_string_duration(self) -> str:
+        """
+        Gets the duration of the object as a formatted string.
+
+        :return: Formatted duration string.
+        """
+        duration = self.get_formatted_duration()
+        format = self.__format_duration
+
+        hours = format(str(duration["hours"]))
+        mins = format(str(duration["minutes"]))
+        secs = format(str(duration["seconds"]))
+
+        if int(hours):
+            return f"{hours}:{mins}:{secs}"
+        else:
+            return f"{mins}:{secs}"
+
+    def __format_duration(self, value: str):
+        """
+        Formats duration value.
+
+        :param value: Value to format.
+        :return: Formatted value.
+        """
+        if len(value) < 2:
+            return "0" + value
+        else:
+            return value
+
+
+class Artist(Base):
+    """
+    Represents an artist on Spotify.
+    """
+
+    def __init__(self, data: dict, type: str, name: str, url: str, id: str):
+        """
+        Initializes Artist object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the artist.
+        :param url: URL of the artist.
+        :param id: ID of the artist.
+        """
+        super().__init__(data, type, name, url, id)
+
+
+class AlbumCover:
+    """
+    Represents the cover image of an album.
+    """
+
+    def __init__(self, width, height, url):
+        """
+        Initializes AlbumCover object.
+
+        :param width: Width of the image.
+        :param height: Height of the image.
+        :param url: URL of the image.
+        """
+        self.width = width
+        self.height = height
+        self.url = url
+
+    def export_image(self, path):
+        """
+        Exports the image to a file.
+
+        :param path: File path.
+        """
+        urlretrieve(self.url, path)
+
+
+class Album(Base):
+    """
+    Represents an album on Spotify.
+    """
+
+    def __init__(
+        self,
+        data: dict,
+        type: str,
+        name: str,
+        url: str,
+        id: str,
+        images: list,
+        artists: list,
+        available_markets: list,
+        release_date: str,
+        total_tracks: int,
+    ):
+        """
+        Initializes Album object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the album.
+        :param url: URL of the album.
+        :param id: ID of the album.
+        :param images: List of album cover images.
+        :param artists: List of artists associated with the album.
+        :param available_markets: List of available markets.
+        :param release_date: Release date of the album.
+        :param total_tracks: Total number of tracks in the album.
+        """
+        super().__init__(data, type, name, url, id)
+        self.images = images
+        self.artists = artists
+        self.available_markets = available_markets
+        self.release_date = release_date
+        self.total_tracks = total_tracks
+
+
+class AlbumTrack:
+    """
+    Represents a track in an album.
+    """
+
+    def __init__(self, track_data):
+        """
+        Initializes AlbumTrack object.
+
+        :param track_data: Data dictionary for the track.
+        """
+        self.spotify_url = track_data.get("external_urls", {}).get("spotify")
+        self.track_name = track_data.get("name")
+        self.artists = ", ".join(
+            artist.get("name", "") for artist in track_data.get("artists", [])
+        )
+        self.track_number = track_data.get("track_number")
+        self.duration_ms = track_data.get("duration_ms", 0)
+
+    def get_formatted_duration(self) -> dict:
+        """
+        Gets the formatted duration of the object.
+
+        :return: Dictionary containing hours, minutes, and seconds.
+        """
+        duration_in_seconds = self.duration_ms / 1000
+        hours = 0
+        mins = math.floor(duration_in_seconds // 60)
+
+        if mins >= 60:
+            hours = math.floor(mins // 60)
+            mins = math.floor(mins % 60)
+
+        secs = math.floor(duration_in_seconds % 60)
+
+        return {"hours": hours, "minutes": mins, "seconds": secs}
+
+    def get_string_duration(self) -> str:
+        """
+        Gets the duration of the object as a formatted string.
+
+        :return: Formatted duration string.
+        """
+        duration = self.get_formatted_duration()
+        format = self.__format_duration
+
+        hours = format(str(duration["hours"]))
+        mins = format(str(duration["minutes"]))
+        secs = format(str(duration["seconds"]))
+
+        if int(hours):
+            return f"{hours}:{mins}:{secs}"
+        else:
+            return f"{mins}:{secs}"
+
+    def __format_duration(self, value: str):
+        """
+        Formats duration value.
+
+        :param value: Value to format.
+        :return: Formatted value.
+        """
+        if len(value) < 2:
+            return "0" + value
+        else:
+            return value
+
+
+class Albums:
+    """
+    Represents an album.
+    """
+
+    def __init__(self, album_data):
+        """
+        Initializes Album object.
+
+        :param album_data: Data dictionary for the album.
+        """
+        self.album_name = album_data.get("name", "Unknown Album")
+        self.artists = ", ".join(
+            artist.get("name", "") for artist in album_data.get("artists", [])
+        )
+        self.release_date = album_data.get("release_date")
+        self.total_tracks = album_data.get("total_tracks", 0)
+        self.thumbnail_url = (
+            album_data.get("images", [])[0].get("url")
+            if album_data.get("images")
+            else None
+        )
+        self.label = album_data.get("label")
+        self.popularity = album_data.get("popularity")
+        self.tracks = [
+            AlbumTrack(track) for track in album_data.get("tracks", {}).get("items", [])
+        ]
+
+    def total_duration(self):
+        """
+        Calculate the total duration of all tracks in the album.
+
+        :return: Total duration as a formatted string.
+        """
+        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
+        hours = int(total_seconds // 3600)
+        minutes = int((total_seconds % 3600) // 60)
+        seconds = int(total_seconds % 60)
+        return f"{hours}:{minutes}:{seconds}"
+
+    def total_duration_string(self):
+        """
+        Calculate the total duration of all tracks in the album as a formatted string.
+
+        :return: Total duration as a formatted string.
+        """
+        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
+        total_duration_track = AlbumTrack({"duration_ms": total_seconds * 1000})
+        return total_duration_track.get_string_duration()
+
+
+class TrackPreview:
+    """
+    Represents a preview of a track.
+    """
+
+    def __init__(self, url):
+        """
+        Initializes TrackPreview object.
+
+        :param url: URL of the track preview.
+        """
+        self.url = url
+
+    def export_audio(self, path):
+        """
+        Exports the audio preview to a file.
+
+        :param path: File path.
+        """
+        urlretrieve(self.url, path)
+
+
+class Track(TrackBase):
+    """
+    Represents a track on Spotify.
+    """
+
+    def __init__(
+        self,
+        data: dict,
+        type: str,
+        name: str,
+        url: str,
+        id: str,
+        explicit: bool,
+        duration_ms: int,
+        preview: TrackPreview,
+        artists: list,
+        album: Album,
+        available_markets: list,
+        disc_number: int,
+        popularity: int,
+    ):
+        """
+        Initializes Track object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the track.
+        :param url: URL of the track.
+        :param id: ID of the track.
+        :param explicit: Explicit content indicator.
+        :param duration_ms: Duration of the track in milliseconds.
+        :param preview: Track preview object.
+        :param artists: List of artists associated with the track.
+        :param album: Album object associated with the track.
+        :param available_markets: List of available markets.
+        :param disc_number: Disc number of the track.
+        :param popularity: Popularity of the track.
+        """
+        super().__init__(data, type, name, url, id, explicit, duration_ms)
+        self.preview = preview
+        self.artists = artists
+        self.album = album
+        self.available_markets = available_markets
+        self.disc_number = disc_number
+        self.popularity = popularity
+
+
+class Episode(TrackBase):
+    """
+    Represents an episode on Spotify.
+    """
+
+    def __init__(
+        self,
+        data: dict,
+        type: str,
+        name: str,
+        url: str,
+        id: str,
+        explicit: bool,
+        duration_ms: int,
+        preview: str,
+        description: str,
+        html_description: str,
+        images: list,
+        language: str,
+        languages: list,
+        release_date: str,
+    ):
+        """
+        Initializes Episode object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the episode.
+        :param url: URL of the episode.
+        :param id: ID of the episode.
+        :param explicit: Explicit content indicator.
+        :param duration_ms: Duration of the episode in milliseconds.
+        :param preview: URL of the episode preview.
+        :param description: Description of the episode.
+        :param html_description: HTML description of the episode.
+        :param images: List of images associated with the episode.
+        :param language: Language of the episode.
+        :param languages: List of languages available for the episode.
+        :param release_date: Release date of the episode.
+        """
+        super().__init__(data, type, name, url, id, explicit, duration_ms)
+        self.preview = preview
+        self.description = description
+        self.html_description = html_description
+        self.images = images
+        self.language = language
+        self.languages = languages
+        self.release_date = release_date
+
+
+class Playlist(Base):
+    """
+    Represents a playlist on Spotify.
+    """
+
+    def __init__(
+        self,
+        data: dict,
+        type: str,
+        name: str,
+        url: str,
+        id: str,
+        description: str,
+        images: list,
+        tracks: list,
+        public: bool,
+        total_tracks: int,
+    ):
+        """
+        Initializes Playlist object.
+
+        :param data: Data dictionary.
+        :param type: Object type.
+        :param name: Name of the playlist.
+        :param url: URL of the playlist.
+        :param id: ID of the playlist.
+        :param description: Description of the playlist.
+        :param images: List of images associated with the playlist.
+        :param tracks: List of tracks in the playlist.
+        :param public: Public visibility indicator.
+        """
+        super().__init__(data, type, name, url, id)
+        self.description = description
+        self.images = images
+        self.tracks = tracks
+        self.public = public
+        self.total_tracks = total_tracks
+
+
+class PlaylistTrack:
+    """
+    Represents a track in a playlist.
+    """
+
+    def __init__(self, track_data):
+        """
+        Initializes PlaylistTrack object.
+
+        :param track_data: Data dictionary for the track.
+        """
+        self.spotify_url = track_data.get("external_urls", {}).get("spotify")
+        self.track_name = track_data.get("name")
+        self.artists = ", ".join(
+            artist.get("name", "") for artist in track_data.get("artists", [])
+        )
+        self.album = track_data.get("album", {}).get("name")
+        self.release_date = track_data.get("album", {}).get("release_date")
+        self.preview_url = track_data.get("preview_url")
+        self.thumbnail_url = track_data.get("album", {}).get("images", [])[0].get("url")
+        self.duration_ms = track_data.get("duration_ms", 0)
+
+    def get_formatted_duration(self) -> dict:
+        """
+        Gets the formatted duration of the object.
+
+        :return: Dictionary containing hours, minutes, and seconds.
+        """
+        duration_in_seconds = self.duration_ms / 1000
+        hours = 0
+        mins = math.floor(duration_in_seconds // 60)
+
+        if mins >= 60:
+            hours = math.floor(mins // 60)
+            mins = math.floor(mins % 60)
+
+        secs = math.floor(duration_in_seconds % 60)
+
+        return {"hours": hours, "minutes": mins, "seconds": secs}
+
+    def get_string_duration(self) -> str:
+        """
+        Gets the duration of the object as a formatted string.
+
+        :return: Formatted duration string.
+        """
+        duration = self.get_formatted_duration()
+        format = self.__format_duration
+
+        hours = format(str(duration["hours"]))
+        mins = format(str(duration["minutes"]))
+        secs = format(str(duration["seconds"]))
+
+        if int(hours):
+            return f"{hours}:{mins}:{secs}"
+        else:
+            return f"{mins}:{secs}"
+
+    def __format_duration(self, value: str):
+        """
+        Formats duration value.
+
+        :param value: Value to format.
+        :return: Formatted value.
+        """
+        if len(value) < 2:
+            return "0" + value
+        else:
+            return value
+
+
+class Playlists:
+    """
+    Represents a collection of playlists.
+    """
+
+    def __init__(self, playlist_data):
+        """
+        Initializes Playlists object.
+
+        :param playlist_data: Data dictionary for the playlists.
+        """
+        self.playlist_name = playlist_data.get("name", "Unknown Playlist")
+        self.description = playlist_data.get("description", "")
+        self.total_tracks = playlist_data.get("tracks", {}).get("total", 0)
+        self.thumbnail_url = playlist_data.get("images", [])[0].get("url")
+        self.tracks = [
+            PlaylistTrack(item.get("track"))
+            for item in playlist_data.get("tracks", {}).get("items", [])
+        ]
+
+    def total_duration(self):
+        """
+        Calculate the total duration of all tracks in the playlist.
+
+        :return: Total duration as a string.
+        """
+        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
+        hours = int(total_seconds // 3600)
+        minutes = int((total_seconds % 3600) // 60)
+        seconds = int(total_seconds % 60)
+        return f"{hours}:{minutes}:{seconds}"
+
+    def total_duration_string(self):
+        """
+        Calculate the total duration of all tracks in the album as a formatted string.
+
+        :return: Total duration as a formatted string.
+        """
+        total_seconds = sum(track.duration_ms for track in self.tracks) / 1000
+        total_duration_track = PlaylistTrack({"duration_ms": total_seconds * 1000})
+        return total_duration_track.get_string_duration()
+
+
+# CLIENT OBJECTS
+
+
+class Results(Base):
+    """
+    Represents results obtained from Spotify API.
+    """
+
+    def __init__(self, data):
+        """
+        Initializes Results object.
+
+        :param data: Data dictionary.
+        """
+        self.data = data
+
+    def __get_items(self, type):
+        """
+        Retrieves items from the data dictionary based on the type.
+
+        :param type: Type of items to retrieve.
+        :return: List of items.
+        """
+        if type == "artist":
+            try:
+                data = self.data["artists"]["items"]
+                func = constructor.artist
+            except KeyError:
+                return []
+
+        elif type == "track":
+            try:
+                data = self.data["tracks"]["items"]
+                func = constructor.track
+            except KeyError:
+                return []
+
+        elif type == "album":
+            try:
+                data = [item["album"] for item in self.data["tracks"]["items"]]
+                func = constructor.album
+            except KeyError:
+                return []
+
+        elif type == "episode":
+            try:
+                data = self.data["episodes"]["items"]
+                func = constructor.episode
+            except KeyError:
+                return []
+
+        elif type == "playlist":
+            try:
+                data = self.data["playlists"]["items"]
+                func = constructor.playlist
+            except KeyError:
+                return []
+
+        return [func(item) for item in data]
+
+    def get_playlist(self) -> "Playlists":
+        """
+        Retrieves playlist items from the results.
+
+        :return: Playlists object.
+        """
+        try:
+            playlist_data = self.data
+            return Playlists(playlist_data)
+        except KeyError:
+            return None
+
+    def get_album(self) -> "Albums":
+        """
+        Retrieves album items from the results.
+
+        :return: Albums object.
+        """
+        try:
+            album_data = self.data
+            return Albums(album_data)
+        except KeyError:
+            return None
+
+    def get_tracks(self) -> list:
+        """
+        Retrieves track items from the results.
+
+        :return: List of track items.
+        """
+        return self.__get_items("track")
+
+    def get_artists(self) -> list:
+        """
+        Retrieves artist items from the results.
+
+        :return: List of artist items.
+        """
+        return self.__get_items("artist")
+
+    def get_albums(self) -> list:
+        """
+        Retrieves album items from the results.
+
+        :return: List of album items.
+        """
+        return self.__get_items("album")
+
+    def get_episodes(self) -> list:
+        """
+        Retrieves episode items from the results.
+
+        :return: List of episode items.
+        """
+        return self.__get_items("episode")
+
+    def get_playlists(self) -> list:
+        """
+        Retrieves playlist items from the results.
+
+        :return: List of playlist items.
+        """
+        return self.__get_items("playlist")
```

### Comparing `searchspotify-0.0.7/src/spotifysearch/constructor.py` & `searchspotify-0.0.8/src/searchspotify/constructor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
-# Nimbus ~ UserBot
-# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-# This file is a part of < https://github.com/ufoptg/Nimbus/ >
-# PLease read the GNU Affero General Public License in
-# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
-# If not, see <https://www.gnu.org/licenses/>.
-
-# THIS FILE IS RESPONSABLE FOR THE CONSTRUCTION OF MANY OBJECTS
-
-from . import classes
-
-
-def get_available_markets(data):
-    """
-    Extracts available markets from the data.
-
-    :param data: The data containing available markets information.
-    :return: Available markets or None if not found.
-    """
-    try:
-        return data["available_markets"]
-    except KeyError:
-        return None
-
-
-# BASE ARGUMENTS FOR ALL CLASSES
-def base_arguments(data):
-    """
-    Generates base arguments for all classes.
-
-    :param data: The data to generate base arguments from.
-    :return: Dictionary of base arguments.
-    """
-    arguments = dict(
-        data=data,
-        type=data["type"] if "type" in data else "",
-        name=data["name"] if "name" in data else "",
-        url=data["external_urls"]["spotify"] if "external_urls" in data else "",
-        id=data["id"] if "id" in data else "",
-    )
-    return arguments
-
-
-# BASE ARGUMENTS FOR TRACK-LIKE CLASSES
-def track_base_arguments(data):
-    """
-    Generates base arguments for track-like classes.
-
-    :param data: The data to generate base arguments from.
-    :return: Dictionary of base arguments.
-    """
-    arguments = dict(explicit=data["explicit"], duration_ms=data["duration_ms"])
-    return arguments
-
-
-def artist(data):
-    """
-    Creates an Artist object from the provided data.
-
-    :param data: The data to create the Artist object from.
-    :return: An instance of Artist.
-    """
-    return classes.Artist(**base_arguments(data))
-
-
-def track(data):
-    """
-    Creates a Track object from the provided data.
-
-    :param data: The data to create the Track object from.
-    :return: An instance of Track.
-    """
-    base = base_arguments(data)
-    track_base = track_base_arguments(data)
-
-    arguments = dict(
-        preview=data["preview_url"],
-        artists=[artist(artist_data) for artist_data in data["artists"]],
-        album=album(data["album"]),
-        available_markets=get_available_markets(data),
-        disc_number=data["disc_number"],
-        popularity=data["popularity"],
-    )
-    return classes.Track(**{**base, **track_base, **arguments})
-
-
-def album(data):
-    """
-    Creates an Album object from the provided data.
-
-    :param data: The data to create the Album object from.
-    :return: An instance of Album.
-    """
-    base = base_arguments(data)
-
-    arguments = dict(
-        images=[
-            classes.AlbumCover(image["width"], image["height"], image["url"])
-            for image in data["images"]
-        ],
-        artists=[artist(artist_data) for artist_data in data["artists"]],
-        available_markets=get_available_markets(data),
-        release_date=data["release_date"],
-        total_tracks=data["total_tracks"],
-    )
-    return classes.Album(**{**base, **arguments})
-
-
-def episode(data):
-    """
-    Creates an Episode object from the provided data.
-
-    :param data: The data to create the Episode object from.
-    :return: An instance of Episode.
-    """
-    base = base_arguments(data)
-    track_base = track_base_arguments(data)
-
-    arguments = dict(
-        preview=data["audio_preview_url"],
-        description=data["description"],
-        html_description=data["html_description"],
-        images=data["images"],
-        language=data["language"],
-        languages=data["languages"],
-        release_date=data["release_date"],
-    )
-    return classes.Episode(**{**base, **track_base, **arguments})
-
-
-def playlist(data):
-    """
-    Creates a Playlist object from the provided data.
-
-    :param data: The data to create the Playlist object from.
-    :return: An instance of Playlist.
-    """
-    base = base_arguments(data)
-
-    arguments = dict(
-        images=[
-            classes.AlbumCover(image["width"], image["height"], image["url"])
-            for image in data.get("images", [])
-        ],
-        tracks=[
-            track(track_data) for track_data in data.get("tracks", {}).get("items", [])
-        ],
-        description=data.get("description"),
-        public=data.get("public", False),
-        total_tracks=data.get("tracks", {}).get("total", 0),
-    )
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
+# Nimbus ~ UserBot
+# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# This file is a part of < https://github.com/ufoptg/Nimbus/ >
+# PLease read the GNU Affero General Public License in
+# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
+# If not, see <https://www.gnu.org/licenses/>.
+
+# THIS FILE IS RESPONSABLE FOR THE CONSTRUCTION OF MANY OBJECTS
+
+from . import classes
+
+
+def get_available_markets(data):
+    """
+    Extracts available markets from the data.
+
+    :param data: The data containing available markets information.
+    :return: Available markets or None if not found.
+    """
+    try:
+        return data["available_markets"]
+    except KeyError:
+        return None
+
+
+# BASE ARGUMENTS FOR ALL CLASSES
+def base_arguments(data):
+    """
+    Generates base arguments for all classes.
+
+    :param data: The data to generate base arguments from.
+    :return: Dictionary of base arguments.
+    """
+    arguments = dict(
+        data=data,
+        type=data["type"] if "type" in data else "",
+        name=data["name"] if "name" in data else "",
+        url=data["external_urls"]["spotify"] if "external_urls" in data else "",
+        id=data["id"] if "id" in data else "",
+    )
+    return arguments
+
+
+# BASE ARGUMENTS FOR TRACK-LIKE CLASSES
+def track_base_arguments(data):
+    """
+    Generates base arguments for track-like classes.
+
+    :param data: The data to generate base arguments from.
+    :return: Dictionary of base arguments.
+    """
+    arguments = dict(explicit=data["explicit"], duration_ms=data["duration_ms"])
+    return arguments
+
+
+def artist(data):
+    """
+    Creates an Artist object from the provided data.
+
+    :param data: The data to create the Artist object from.
+    :return: An instance of Artist.
+    """
+    return classes.Artist(**base_arguments(data))
+
+
+def track(data):
+    """
+    Creates a Track object from the provided data.
+
+    :param data: The data to create the Track object from.
+    :return: An instance of Track.
+    """
+    base = base_arguments(data)
+    track_base = track_base_arguments(data)
+
+    arguments = dict(
+        preview=data["preview_url"],
+        artists=[artist(artist_data) for artist_data in data["artists"]],
+        album=album(data["album"]),
+        available_markets=get_available_markets(data),
+        disc_number=data["disc_number"],
+        popularity=data["popularity"],
+    )
+    return classes.Track(**{**base, **track_base, **arguments})
+
+
+def album(data):
+    """
+    Creates an Album object from the provided data.
+
+    :param data: The data to create the Album object from.
+    :return: An instance of Album.
+    """
+    base = base_arguments(data)
+
+    arguments = dict(
+        images=[
+            classes.AlbumCover(image["width"], image["height"], image["url"])
+            for image in data["images"]
+        ],
+        artists=[artist(artist_data) for artist_data in data["artists"]],
+        available_markets=get_available_markets(data),
+        release_date=data["release_date"],
+        total_tracks=data["total_tracks"],
+    )
+    return classes.Album(**{**base, **arguments})
+
+
+def episode(data):
+    """
+    Creates an Episode object from the provided data.
+
+    :param data: The data to create the Episode object from.
+    :return: An instance of Episode.
+    """
+    base = base_arguments(data)
+    track_base = track_base_arguments(data)
+
+    arguments = dict(
+        preview=data["audio_preview_url"],
+        description=data["description"],
+        html_description=data["html_description"],
+        images=data["images"],
+        language=data["language"],
+        languages=data["languages"],
+        release_date=data["release_date"],
+    )
+    return classes.Episode(**{**base, **track_base, **arguments})
+
+
+def playlist(data):
+    """
+    Creates a Playlist object from the provided data.
+
+    :param data: The data to create the Playlist object from.
+    :return: An instance of Playlist.
+    """
+    base = base_arguments(data)
+
+    arguments = dict(
+        images=[
+            classes.AlbumCover(image["width"], image["height"], image["url"])
+            for image in data.get("images", [])
+        ],
+        tracks=[
+            track(track_data) for track_data in data.get("tracks", {}).get("items", [])
+        ],
+        description=data.get("description"),
+        public=data.get("public", False),
+        total_tracks=data.get("tracks", {}).get("total", 0),
+    )
     return classes.Playlist(**{**base, **arguments})
```

### Comparing `searchspotify-0.0.7/src/spotifysearch/urlbuilder.py` & `searchspotify-0.0.8/src/searchspotify/urlbuilder.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
-# Nimbus ~ UserBot
-# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-# This file is a part of < https://github.com/ufoptg/Nimbus/ >
-# PLease read the GNU Affero General Public License in
-# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
-# If not, see <https://www.gnu.org/licenses/>.
-
-# THIS FILE IS RESPONSABLE FOR BUILDING DYNAMIC URLS
-
-
-def search_endpoint(
-    keywords: str,
-    allowed_types: list,
-    filters: dict,
-    market: str = None,
-    limit: int = None,
-    offset: int = None,
-):
-    """
-    Constructs the Spotify API search endpoint URL based on provided parameters.
-
-    :param keywords: Keywords for the search.
-    :param allowed_types: List of allowed types to search for.
-    :param filters: Dictionary of filters to apply to the search.
-    :param market: Market to search in (optional).
-    :param limit: Maximum number of items to return (optional).
-    :param offset: Offset for pagination (optional).
-    :return: Constructed search endpoint URL.
-    """
-    endpoint = "https://api.spotify.com/v1/"
-
-    if "::" in keywords:
-        entity_type, entity_id = keywords.split("::")
-        # Construct the endpoint based on the entity type and ID
-        endpoint += f"{entity_type}s/{entity_id}"
-    else:
-        endpoint += "search?"
-
-        # FORMAT QUERY ITEMS AND FILTERS
-        query_items = keywords.split(" ")
-        for filter_name, value in filters.items():
-            value = value.replace(" ", "%20")
-            item = f"{filter_name}:{value}"
-            query_items.append(item)
-
-        # REQUIRED ARGUMENTS
-        query = "q=" + "%20".join(query_items)
-        types = "type=" + ",".join(allowed_types)
-        arguments = [query, types]
-
-        # OPTIONAL ARGUMENTS
-        if market:
-            arguments.append(f"market={market}")
-        if limit:
-            arguments.append(f"limit={limit}")
-        if offset:
-            arguments.append(f"offset={offset}")
-
-        endpoint += "&".join(arguments)
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2020-2023 (c) Randy W @xtdevs, @xtsea
+# Nimbus ~ UserBot
+# Copyright (C) 2023 NimbusTheCloud, ufoptg, @TrueSaiyan
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# This file is a part of < https://github.com/ufoptg/Nimbus/ >
+# PLease read the GNU Affero General Public License in
+# <https://www.github.com/ufoptg/Nimbus/blob/main/LICENSE/>.
+# If not, see <https://www.gnu.org/licenses/>.
+
+# THIS FILE IS RESPONSABLE FOR BUILDING DYNAMIC URLS
+
+
+def search_endpoint(
+    keywords: str,
+    allowed_types: list,
+    filters: dict,
+    market: str = None,
+    limit: int = None,
+    offset: int = None,
+):
+    """
+    Constructs the Spotify API search endpoint URL based on provided parameters.
+
+    :param keywords: Keywords for the search.
+    :param allowed_types: List of allowed types to search for.
+    :param filters: Dictionary of filters to apply to the search.
+    :param market: Market to search in (optional).
+    :param limit: Maximum number of items to return (optional).
+    :param offset: Offset for pagination (optional).
+    :return: Constructed search endpoint URL.
+    """
+    endpoint = "https://api.spotify.com/v1/"
+
+    if "::" in keywords:
+        entity_type, entity_id = keywords.split("::")
+        # Construct the endpoint based on the entity type and ID
+        endpoint += f"{entity_type}s/{entity_id}"
+    else:
+        endpoint += "search?"
+
+        # FORMAT QUERY ITEMS AND FILTERS
+        query_items = keywords.split(" ")
+        for filter_name, value in filters.items():
+            value = value.replace(" ", "%20")
+            item = f"{filter_name}:{value}"
+            query_items.append(item)
+
+        # REQUIRED ARGUMENTS
+        query = "q=" + "%20".join(query_items)
+        types = "type=" + ",".join(allowed_types)
+        arguments = [query, types]
+
+        # OPTIONAL ARGUMENTS
+        if market:
+            arguments.append(f"market={market}")
+        if limit:
+            arguments.append(f"limit={limit}")
+        if offset:
+            arguments.append(f"offset={offset}")
+
+        endpoint += "&".join(arguments)
+
     return endpoint
```

