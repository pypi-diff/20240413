# Comparing `tmp/spotidex-0.0.6.tar.gz` & `tmp/spotidex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.6.tar", max compression
+gzip compressed data, was "spotidex-0.0.7.tar", max compression
```

## Comparing `spotidex-0.0.6.tar` & `spotidex-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      553 2024-04-10 09:43:59.673109 spotidex-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.6/README.md
--rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.6/spotidex/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.6/spotidex/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.6/spotidex/cli/app_screens/__init__.py
--rw-r--r--   0        0        0     6912 2024-04-10 18:01:30.463082 spotidex-0.0.6/spotidex/cli/app_screens/DownloadInterface.py
--rw-r--r--   0        0        0     4675 2024-04-10 14:00:34.257827 spotidex-0.0.6/spotidex/cli/app_screens/MainMenuInterface.py
--rw-r--r--   0        0        0     5137 2024-04-10 14:45:17.645923 spotidex-0.0.6/spotidex/cli/app_screens/SearchInterface.py
--rw-r--r--   0        0        0     4025 2024-04-06 10:25:55.937694 spotidex-0.0.6/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-r--r--   0        0        0     2450 2024-04-10 18:25:24.740301 spotidex-0.0.6/spotidex/cli/app_screens/SettingsInterface.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.6/spotidex/cli/custom_widgets/__init__.py
--rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
--rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
--rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
--rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
--rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
--rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
--rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
--rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
--rw-r--r--   0        0        0     4510 2024-04-10 14:45:36.699352 spotidex-0.0.6/spotidex/cli/custom_widgets/AppInterface.py
--rw-r--r--   0        0        0     1467 2024-04-10 18:25:15.239179 spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-r--r--   0        0        0     1933 2024-03-26 10:25:59.101131 spotidex-0.0.6/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.6/spotidex/cli/popup_screens/__init__.py
--rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
--rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
--rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
--rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
--rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
--rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
--rw-r--r--   0        0        0     4303 2024-04-10 15:10:02.743220 spotidex-0.0.6/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-r--r--   0        0        0     1135 2024-04-10 14:45:53.954177 spotidex-0.0.6/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.6/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.6/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-r--r--   0        0        0      700 2024-04-10 18:25:42.766710 spotidex-0.0.6/spotidex/cli/SpotidexApp.py
--rw-r--r--   0        0        0     4196 2024-04-09 16:52:32.143307 spotidex-0.0.6/spotidex/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.6/spotidex/src/__init__.py
--rw-r--r--   0        0        0     3043 2024-04-07 05:31:37.359930 spotidex-0.0.6/spotidex/src/content.py
--rw-r--r--   0        0        0     6712 2024-04-09 17:18:55.031801 spotidex-0.0.6/spotidex/src/download.py
--rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.6/spotidex/src/static.py
--rw-r--r--   0        0        0     5991 2024-04-10 18:07:50.938740 spotidex-0.0.6/spotidex/src/utils.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 spotidex-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      552 2024-04-13 17:30:43.922225 spotidex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.7/README.md
+-rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.7/spotidex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.7/spotidex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.7/spotidex/cli/app_screens/__init__.py
+-rw-r--r--   0        0        0     6908 2024-04-12 11:27:13.657978 spotidex-0.0.7/spotidex/cli/app_screens/DownloadInterface.py
+-rw-r--r--   0        0        0     4674 2024-04-12 12:43:31.490186 spotidex-0.0.7/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-r--r--   0        0        0     5719 2024-04-13 12:46:07.764636 spotidex-0.0.7/spotidex/cli/app_screens/SearchInterface.py
+-rw-r--r--   0        0        0     4053 2024-04-13 05:48:36.635880 spotidex-0.0.7/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-r--r--   0        0        0     2450 2024-04-13 05:23:06.441432 spotidex-0.0.7/spotidex/cli/app_screens/SettingsInterface.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.7/spotidex/cli/custom_widgets/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
+-rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
+-rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
+-rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
+-rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
+-rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
+-rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
+-rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
+-rw-r--r--   0        0        0     4510 2024-04-10 14:45:36.699352 spotidex-0.0.7/spotidex/cli/custom_widgets/AppInterface.py
+-rw-r--r--   0        0        0     1467 2024-04-10 18:25:15.239179 spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-r--r--   0        0        0     1854 2024-04-12 10:43:16.844163 spotidex-0.0.7/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.7/spotidex/cli/popup_screens/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
+-rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
+-rw-r--r--   0        0        0     4303 2024-04-13 05:59:34.299624 spotidex-0.0.7/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-r--r--   0        0        0     1135 2024-04-10 14:45:53.954177 spotidex-0.0.7/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.7/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.7/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-r--r--   0        0        0      700 2024-04-10 18:25:42.766710 spotidex-0.0.7/spotidex/cli/SpotidexApp.py
+-rw-r--r--   0        0        0     4619 2024-04-13 17:10:46.966551 spotidex-0.0.7/spotidex/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.7/spotidex/src/__init__.py
+-rw-r--r--   0        0        0     5841 2024-04-13 16:54:40.790363 spotidex-0.0.7/spotidex/src/content.py
+-rw-r--r--   0        0        0     6847 2024-04-13 17:27:05.680218 spotidex-0.0.7/spotidex/src/download.py
+-rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.7/spotidex/src/static.py
+-rw-r--r--   0        0        0     5057 2024-04-13 16:42:59.190419 spotidex-0.0.7/spotidex/src/utils.py
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 spotidex-0.0.7/PKG-INFO
```

### Comparing `spotidex-0.0.6/pyproject.toml` & `spotidex-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotidex"
-version = "0.0.6"
+version = "0.0.7"
 description = "Spotify Downloader TUI"
 authors = ["Libin Lalu <libinlalu000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,15 +12,15 @@
 requests = "2.31.0"
 rich = "13.7.1"
 spotipy = "2.23.0"
 textual = "0.56.4"
 tqdm = "4.66.1"
 yt-dlp = "2024.3.10"
 ytmusicapi = "1.3.2"
-pyperclip = "^1.8.2"
+pyperclip = "1.8.2"
 
 [tool.poetry.scripts]
 spotidex = "spotidex:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spotidex-0.0.6/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-0.0.7/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         if "track" in self.app.spotify_link:
             link_type = "TRACK"
         elif "playlist" in self.app.spotify_link:
             link_type = "PLAYLIST"
         elif "album" in self.app.spotify_link:
             link_type = "ALBUM"
 
-        self.query_one("#info-container").border_title = f"{link_type} INFO"
+        self.query_one("#info-container").border_title = "DOWNLOAD INFO"
         name = self.app.link_details[0][f"{link_type} NAME"]
 
         if "track" in self.app.spotify_link:
             full_track_info = f"{name} by {self.app.link_details[0]['ARTIST']}"
             track_info = (
                 full_track_info[:57] + "..."
                 if len(full_track_info) > 57
```

### Comparing `spotidex-0.0.6/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-0.0.7/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,28 +37,28 @@
 
 #link-info{
     width: 86;
     background:transparent;
 }
 
 #download-button{
-    width:100%;
+    width:98%;
     column-span:1;
 }
 
 #download-all-button{
-    width:100%
+    width:98%
 }
 
 #select-download-button{
     width:100%;
 }
 
 #settings-button{
-    width:98%;
+    width:100%;
     column-span:1;
 }
 
 
 """
 
 
@@ -83,22 +83,22 @@
                 ),
                 id="link-info-container",
             ),
             Button("SETTINGS", "primary", id="settings-button"),
         ]
         if "track" not in self.spotify_link:
             childrens.insert(
-                1, Button("DOWNLOAD ALL TRACK", "success", id="download-all-button")
+                3, Button("DOWNLOAD ALL TRACK", "success", id="download-all-button")
             )
             childrens.insert(
-                2, Button("SELECT TO DOWNLOAD", "success", id="select-download-button")
+                2, Button("SELECT TO DOWNLOAD", "warning", id="select-download-button")
             )
         else:
             childrens.insert(
-                1, Button("DOWNLOAD TRACK", "success", id="download-button")
+                2, Button("DOWNLOAD TRACK", "success", id="download-button")
             )
 
         yield AppInterface(*childrens, id="main-menu-interface")
   
     def on_mount(self):
         link_info = self.link_details[0]
         text_log = self.query_one("#link-info")
```

### Comparing `spotidex-0.0.6/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-0.0.7/spotidex/cli/app_screens/SearchInterface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from textual.widgets import Input, Button, Label
 from textual.screen import Screen
 from textual.containers import Horizontal
 
 from spotidex.cli.custom_widgets.AppInterface import AppInterface
 from spotidex.cli.app_screens.MainMenuInterface import MainMenuInterface
+from spotidex.src.utils import SpotidexError
 from spotidex.cli.utils import input_validator, app_description
 from spotidex.cli.utils import get_link_details
 
 from textual.worker import Worker, get_current_worker
 from textual.binding import Binding
 from textual import work
 import pyperclip
@@ -33,16 +34,17 @@
 #search-button{
     column-span:1;
     width: 23%;
     margin-left:1;
 }
 
 #app-description{
-    border: round ansi_bright_cyan;
+    border:heavy ansi_bright_blue 80%;
     border-title-align: center;
+    padding-left:1;
 
 }
 
 #search-input:blur{
     border:tall black
 }
 """
@@ -78,27 +80,38 @@
 
 
     @work(exclusive=True, thread=True)
     def get_link_info(self):
         self.app.query_one("LoadingIndicator").styles.background = "#1c1c1c"
         try:
             self.app.link_details = get_link_details(self.app.spotify_link)
+            if int(self.app.link_details[0]['TOTAL TRACKS']) > 100:
+                raise SpotidexError("Maxlimit")
+                
         except Exception as spotidex_error:
             if spotidex_error.message == "NetworkError":
                 self.app.notify(
                     "Please check you internet connection and try again",
                     title="Network Error",
                     severity="error",
                 )
             elif spotidex_error.message == "InvalidSpotifyLink":
                 self.app.notify(
                     "The link provided is not valid, please check the link and try again",
                     title="INVALID LINK",
                     severity="error",
                 )
+            elif spotidex_error.message == "Maxlimit":
+                self.query_one("#search-input").value = ""
+                self.app.notify(
+                    "The total track of playlist/album has exceeded the maximum limit which is 100",
+                    title="MAX LIMIT REACHED",
+                    severity="error",
+                )
+                
             get_current_worker().cancel()
         self.app.query_one("#interface").loading = False
         self.app.query_one("#exit-button").disabled = False
         self.app.query_one("#interface").styles.padding = (2, 3, 0, 3)
 
     def on_worker_state_changed(self, event: Worker.StateChanged) -> None:
         if str(event.state) == "WorkerState.CANCELLED":
```

### Comparing `spotidex-0.0.6/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-0.0.7/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,233 +20,235 @@
 00000130: 220d 0a53 656c 6563 7444 6f77 6e6c 6f61  "..SelectDownloa
 00000140: 647b 0d0a 2020 2020 616c 6967 6e3a 6365  d{..    align:ce
 00000150: 6e74 6572 206d 6964 646c 653b 0d0a 0d0a  nter middle;....
 00000160: 0d0a 7d0d 0a23 696e 7465 7266 6163 657b  ..}..#interface{
 00000170: 0d0a 2020 2020 7061 6464 696e 673a 3120  ..    padding:1 
 00000180: 313b 0d0a 7d0d 0a0d 0a23 616c 6c2d 7472  1;..}....#all-tr
 00000190: 6163 6b73 207b 0d0a 2020 2020 626f 7264  acks {..    bord
-000001a0: 6572 3a74 616c 6c20 6772 6579 2034 3025  er:tall grey 40%
-000001b0: 3b0d 0a20 2020 2077 6964 7468 3a20 3634  ;..    width: 64
-000001c0: 3b0d 0a20 2020 2068 6569 6768 743a 2031  ;..    height: 1
-000001d0: 3030 253b 0d0a 2020 2020 6261 636b 6772  00%;..    backgr
-000001e0: 6f75 6e64 3a20 2462 6f6f 7374 3b0d 0a20  ound: $boost;.. 
-000001f0: 2020 2070 6164 6469 6e67 2d6c 6566 743a     padding-left:
-00000200: 313b 0d0a 2020 2020 7061 6464 696e 672d  1;..    padding-
-00000210: 7269 6768 743a 313b 0d0a 2020 2020 6d61  right:1;..    ma
-00000220: 7267 696e 2d6c 6566 743a 313b 0d0a 7d0d  rgin-left:1;..}.
-00000230: 0a0d 0a0d 0a23 7365 6c65 6374 736f 6e67  .....#selectsong
-00000240: 732d 6c61 6265 6c7b 0d0a 2020 2020 646f  s-label{..    do
-00000250: 636b 3a72 6967 6874 3b0d 0a20 2020 206d  ck:right;..    m
-00000260: 6172 6769 6e2d 7269 6768 743a 2031 353b  argin-right: 15;
-00000270: 0d0a 7d0d 0a0d 0a23 7365 6c65 6374 6564  ..}....#selected
-00000280: 2d74 7261 636b 732d 6275 7474 6f6e 732d  -tracks-buttons-
-00000290: 636f 6e74 6169 6e65 727b 0d0a 2020 2020  container{..    
-000002a0: 646f 636b 3a72 6967 6874 3b0d 0a20 2020  dock:right;..   
-000002b0: 2077 6964 7468 3a20 3237 3b0d 0a7d 0d0a   width: 27;..}..
-000002c0: 0d0a 2364 6573 656c 6563 742d 616c 6c2d  ..#deselect-all-
-000002d0: 6275 7474 6f6e 7b0d 0a0d 0a20 2020 206d  button{....    m
-000002e0: 6172 6769 6e2d 746f 703a 2031 3b0d 0a20  argin-top: 1;.. 
-000002f0: 2020 2077 6964 7468 3a20 3235 3b0d 0a20     width: 25;.. 
-00000300: 2020 206d 6172 6769 6e2d 6c65 6674 3a20     margin-left: 
-00000310: 313b 0d0a 7d0d 0a0d 0a23 7365 6c65 6374  1;..}....#select
-00000320: 2d61 6c6c 2d62 7574 746f 6e7b 0d0a 2020  -all-button{..  
-00000330: 2020 7769 6474 683a 2032 353b 0d0a 2020    width: 25;..  
-00000340: 2020 6d61 7267 696e 2d74 6f70 3a20 313b    margin-top: 1;
-00000350: 0d0a 2020 2020 6d61 7267 696e 2d6c 6566  ..    margin-lef
-00000360: 743a 2031 3b0d 0a7d 0d0a 0d0a 2364 6f77  t: 1;..}....#dow
-00000370: 6e6c 6f61 642d 7365 6c65 6374 6564 2d62  nload-selected-b
-00000380: 7574 746f 6e7b 0d0a 2020 2020 7769 6474  utton{..    widt
-00000390: 683a 2032 353b 0d0a 2020 2020 6d61 7267  h: 25;..    marg
-000003a0: 696e 2d74 6f70 3a20 313b 0d0a 2020 2020  in-top: 1;..    
-000003b0: 6d61 7267 696e 2d6c 6566 743a 2031 3b0d  margin-left: 1;.
-000003c0: 0a7d 0d0a 0d0a 2373 656c 6563 7465 642d  .}....#selected-
-000003d0: 7472 6163 6b73 2d6c 6162 656c 7b0d 0a20  tracks-label{.. 
-000003e0: 2020 2077 6964 7468 3a32 373b 0d0a 2020     width:27;..  
-000003f0: 2020 6865 6967 6874 3a20 333b 0d0a 2020    height: 3;..  
-00000400: 2020 626f 7264 6572 3a74 616c 6c20 6772    border:tall gr
-00000410: 6565 6e20 3430 253b 0d0a 2020 2020 6261  een 40%;..    ba
-00000420: 636b 6772 6f75 6e64 3a24 626f 6f73 743b  ckground:$boost;
-00000430: 0d0a 2020 2020 636f 6e74 656e 742d 616c  ..    content-al
-00000440: 6967 6e3a 6365 6e74 6572 206d 6964 646c  ign:center middl
-00000450: 653b 0d0a 2020 2020 6d61 7267 696e 2d62  e;..    margin-b
-00000460: 6f74 746f 6d3a 323b 0d0a 0d0a 7d0d 0a0d  ottom:2;....}...
-00000470: 0a0d 0a0d 0a2e 616c 6c2d 736f 6e67 732d  ......all-songs-
-00000480: 6368 6563 6b62 6f78 207b 0d0a 2020 2020  checkbox {..    
-00000490: 7769 6474 683a 3536 3b0d 0a20 2020 2070  width:56;..    p
-000004a0: 6164 6469 6e67 2d72 6967 6874 3a33 3b0d  adding-right:3;.
-000004b0: 0a7d 0d0a 2e61 6c6c 2d73 6f6e 6773 2d63  .}...all-songs-c
-000004c0: 6865 636b 626f 783a 686f 7665 7220 7b0d  heckbox:hover {.
-000004d0: 0a20 2020 2074 6578 742d 7374 796c 653a  .    text-style:
-000004e0: 6e6f 6e65 3b0d 0a20 2020 206f 7061 6369  none;..    opaci
-000004f0: 7479 3a30 2e38 3b0d 0a7d 0d0a 2e61 6c6c  ty:0.8;..}...all
-00000500: 2d73 6f6e 6773 2d63 6865 636b 626f 782e  -songs-checkbox.
-00000510: 2d6f 6e7b 0d0a 2020 2020 626f 7264 6572  -on{..    border
-00000520: 3a20 7461 6c6c 2074 7261 6e73 7061 7265  : tall transpare
-00000530: 6e74 3b0d 0a20 2020 2062 6163 6b67 726f  nt;..    backgro
-00000540: 756e 643a 2333 3243 4433 323b 0d0a 2020  und:#32CD32;..  
-00000550: 2020 6f70 6163 6974 793a 302e 353b 0d0a    opacity:0.5;..
-00000560: 7d0d 0a0d 0a2e 616c 6c2d 736f 6e67 732d  }.....all-songs-
-00000570: 6368 6563 6b62 6f78 3a66 6f63 7573 203e  checkbox:focus >
-00000580: 202e 746f 6767 6c65 2d2d 6c61 6265 6c20   .toggle--label 
-00000590: 7b0d 0a20 2020 2074 6578 742d 7374 796c  {..    text-styl
-000005a0: 653a 206e 6f6e 653b 0d0a 2020 2020 6d61  e: none;..    ma
-000005b0: 7267 696e 2d6c 6566 743a 303b 0d0a 7d0d  rgin-left:0;..}.
-000005c0: 0a0d 0a2e 616c 6c2d 736f 6e67 732d 6368  ....all-songs-ch
-000005d0: 6563 6b62 6f78 3a66 6f63 7573 207b 0d0a  eckbox:focus {..
-000005e0: 2020 2020 626f 7264 6572 3a74 616c 6c20      border:tall 
-000005f0: 7472 616e 7370 6172 656e 740d 0a7d 0d0a  transparent..}..
-00000600: 0d0a 2222 220d 0a0d 0a0d 0a63 6c61 7373  .."""......class
-00000610: 2053 656c 6563 7444 6f77 6e6c 6f61 6428   SelectDownload(
-00000620: 5363 7265 656e 293a 0d0a 2020 2020 4445  Screen):..    DE
-00000630: 4641 554c 545f 4353 5320 3d20 4353 530d  FAULT_CSS = CSS.
-00000640: 0a20 2020 2073 656c 6563 7465 645f 7472  .    selected_tr
-00000650: 6163 6b73 203d 205b 5d0d 0a0d 0a20 2020  acks = []....   
-00000660: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000670: 6c66 293a 0d0a 2020 2020 2020 2020 7365  lf):..        se
-00000680: 6c66 2e74 7261 636b 7320 3d20 7365 6c66  lf.tracks = self
-00000690: 2e61 7070 2e6c 696e 6b5f 6465 7461 696c  .app.link_detail
-000006a0: 735b 315d 0d0a 2020 2020 2020 2020 7375  s[1]..        su
-000006b0: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
-000006c0: 0d0a 0d0a 2020 2020 6465 6620 636f 6d70  ....    def comp
-000006d0: 6f73 6528 7365 6c66 293a 0d0a 2020 2020  ose(self):..    
-000006e0: 2020 2020 7969 656c 6420 4170 7049 6e74      yield AppInt
-000006f0: 6572 6661 6365 280d 0a20 2020 2020 2020  erface(..       
-00000700: 2020 2020 2048 6f72 697a 6f6e 7461 6c28       Horizontal(
-00000710: 5665 7274 6963 616c 5363 726f 6c6c 2869  VerticalScroll(i
-00000720: 643d 2261 6c6c 2d74 7261 636b 7322 292c  d="all-tracks"),
-00000730: 2069 643d 2261 6c6c 2d74 7261 636b 732d   id="all-tracks-
-00000740: 636f 6e74 6169 6e65 7222 292c 0d0a 2020  container"),..  
-00000750: 2020 2020 2020 2020 2020 5665 7274 6963            Vertic
-00000760: 616c 280d 0a20 2020 2020 2020 2020 2020  al(..           
-00000770: 2020 2020 2053 7461 7469 6328 2253 454c       Static("SEL
-00000780: 4543 5445 4420 5452 4143 4b53 203a 2030  ECTED TRACKS : 0
-00000790: 222c 2069 643d 2273 656c 6563 7465 642d  ", id="selected-
-000007a0: 7472 6163 6b73 2d6c 6162 656c 2229 2c0d  tracks-label"),.
-000007b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007c0: 2042 7574 746f 6e28 2244 4553 454c 4543   Button("DESELEC
-000007d0: 5420 414c 4c22 2c20 2265 7272 6f72 222c  T ALL", "error",
-000007e0: 2069 643d 2264 6573 656c 6563 742d 616c   id="deselect-al
-000007f0: 6c2d 6275 7474 6f6e 2229 2c0d 0a20 2020  l-button"),..   
-00000800: 2020 2020 2020 2020 2020 2020 2042 7574               But
-00000810: 746f 6e28 2253 454c 4543 5420 414c 4c22  ton("SELECT ALL"
-00000820: 2c20 2270 7269 6d61 7279 222c 2069 643d  , "primary", id=
-00000830: 2273 656c 6563 742d 616c 6c2d 6275 7474  "select-all-butt
-00000840: 6f6e 2229 2c0d 0a20 2020 2020 2020 2020  on"),..         
-00000850: 2020 2020 2020 2042 7574 746f 6e28 2244         Button("D
-00000860: 4f57 4e4c 4f41 4420 5345 4c45 4354 4544  OWNLOAD SELECTED
-00000870: 2022 2c20 2273 7563 6365 7373 222c 2069   ", "success", i
-00000880: 643d 2264 6f77 6e6c 6f61 642d 7365 6c65  d="download-sele
-00000890: 6374 6564 2d62 7574 746f 6e22 2c64 6973  cted-button",dis
-000008a0: 6162 6c65 643d 5472 7565 292c 0d0a 2020  abled=True),..  
-000008b0: 2020 2020 2020 2020 2020 2020 2020 6964                id
-000008c0: 3d22 7365 6c65 6374 6564 2d74 7261 636b  ="selected-track
-000008d0: 732d 6275 7474 6f6e 732d 636f 6e74 6169  s-buttons-contai
-000008e0: 6e65 7222 2c0d 0a20 2020 2020 2020 2020  ner",..         
-000008f0: 2020 2029 2c0d 0a20 2020 2020 2020 2029     ),..        )
-00000900: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f63  ....    def on_c
-00000910: 6865 636b 626f 785f 6368 616e 6765 6428  heckbox_changed(
-00000920: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
-00000930: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00000940: 5f73 6f6e 6773 203d 205b 5d0d 0a20 2020  _songs = []..   
-00000950: 2020 2020 2066 6f72 2063 6865 636b 626f       for checkbo
-00000960: 7820 696e 2073 656c 662e 6170 702e 7175  x in self.app.qu
-00000970: 6572 7928 222e 616c 6c2d 736f 6e67 732d  ery(".all-songs-
-00000980: 6368 6563 6b62 6f78 2229 3a0d 0a20 2020  checkbox"):..   
-00000990: 2020 2020 2020 2020 2069 6620 6368 6563           if chec
-000009a0: 6b62 6f78 2e76 616c 7565 203d 3d20 5472  kbox.value == Tr
-000009b0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-000009c0: 2020 2020 2073 656c 6563 7465 645f 736f       selected_so
-000009d0: 6e67 732e 6170 7065 6e64 2873 7472 2863  ngs.append(str(c
-000009e0: 6865 636b 626f 782e 6c61 6265 6c29 2e73  heckbox.label).s
-000009f0: 706c 6974 2822 2e20 222c 6d61 7873 706c  plit(". ",maxspl
-00000a00: 6974 3d31 295b 315d 290d 0a20 2020 2020  it=1)[1])..     
-00000a10: 2020 2073 656c 662e 6170 702e 7175 6572     self.app.quer
-00000a20: 795f 6f6e 6528 2223 7365 6c65 6374 6564  y_one("#selected
-00000a30: 2d74 7261 636b 732d 6c61 6265 6c22 292e  -tracks-label").
-00000a40: 7570 6461 7465 280d 0a20 2020 2020 2020  update(..       
-00000a50: 2020 2020 2066 2253 454c 4543 5445 4420       f"SELECTED 
-00000a60: 5452 4143 4b53 203a 207b 6c65 6e28 7365  TRACKS : {len(se
-00000a70: 6c65 6374 6564 5f73 6f6e 6773 297d 220d  lected_songs)}".
-00000a80: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-00000a90: 2020 2020 7365 6c66 2e61 7070 2e73 656c      self.app.sel
-00000aa0: 6563 7465 645f 7472 6163 6b73 203d 205b  ected_tracks = [
-00000ab0: 7365 6c66 2e74 7261 636b 735b 736f 6e67  self.tracks[song
-00000ac0: 5d20 666f 7220 736f 6e67 2069 6e20 7365  ] for song in se
-00000ad0: 6c65 6374 6564 5f73 6f6e 6773 5d0d 0a20  lected_songs].. 
-00000ae0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-00000af0: 6c66 2e61 7070 2e73 656c 6563 7465 645f  lf.app.selected_
-00000b00: 7472 6163 6b73 2920 213d 2030 203a 0d0a  tracks) != 0 :..
-00000b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000b20: 2e71 7565 7279 5f6f 6e65 2827 2364 6f77  .query_one('#dow
-00000b30: 6e6c 6f61 642d 7365 6c65 6374 6564 2d62  nload-selected-b
-00000b40: 7574 746f 6e27 292e 6469 7361 626c 6564  utton').disabled
-00000b50: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-00000b60: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000b70: 2020 2020 2073 656c 662e 7175 6572 795f       self.query_
-00000b80: 6f6e 6528 2723 646f 776e 6c6f 6164 2d73  one('#download-s
-00000b90: 656c 6563 7465 642d 6275 7474 6f6e 2729  elected-button')
-00000ba0: 2e64 6973 6162 6c65 6420 3d20 5472 7565  .disabled = True
-00000bb0: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f6d  ....    def on_m
-00000bc0: 6f75 6e74 2873 656c 6629 3a0d 0a20 2020  ount(self):..   
-00000bd0: 2020 2020 2073 656c 662e 6170 702e 7175       self.app.qu
-00000be0: 6572 795f 6f6e 6528 2223 6e61 762d 6c61  ery_one("#nav-la
-00000bf0: 6265 6c22 292e 7570 6461 7465 2822 5b62  bel").update("[b
-00000c00: 6f6c 645d 5345 4c45 4354 2054 5241 434b  old]SELECT TRACK
-00000c10: 5320 544f 2044 4f57 4e4c 4f41 4422 290d  S TO DOWNLOAD").
-00000c20: 0a20 2020 2020 2020 2066 6f72 2073 6f6e  .        for son
-00000c30: 672c 2074 7261 636b 5f6e 6f20 696e 207a  g, track_no in z
-00000c40: 6970 280d 0a20 2020 2020 2020 2020 2020  ip(..           
-00000c50: 2073 656c 662e 7472 6163 6b73 2e6b 6579   self.tracks.key
-00000c60: 7328 292c 2072 616e 6765 2831 2c20 6c65  s(), range(1, le
-00000c70: 6e28 7365 6c66 2e74 7261 636b 732e 6b65  n(self.tracks.ke
-00000c80: 7973 2829 2920 2b20 3129 0d0a 2020 2020  ys()) + 1)..    
-00000c90: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-00000ca0: 2020 2020 7365 6c66 2e61 7070 2e71 7565      self.app.que
-00000cb0: 7279 5f6f 6e65 2822 2361 6c6c 2d74 7261  ry_one("#all-tra
-00000cc0: 636b 7322 292e 6d6f 756e 7428 0d0a 2020  cks").mount(..  
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 4368                Ch
-00000ce0: 6563 6b62 6f78 2866 227b 7472 6163 6b5f  eckbox(f"{track_
-00000cf0: 6e6f 7d2e 2022 202b 2073 6f6e 672c 2063  no}. " + song, c
-00000d00: 6c61 7373 6573 3d22 616c 6c2d 736f 6e67  lasses="all-song
-00000d10: 732d 6368 6563 6b62 6f78 2229 0d0a 2020  s-checkbox")..  
-00000d20: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00000d30: 2020 2020 2066 6f72 2069 2069 6e20 7365       for i in se
-00000d40: 6c66 2e61 7070 2e71 7565 7279 2822 2e61  lf.app.query(".a
-00000d50: 6c6c 2d73 6f6e 6773 2d63 6865 636b 626f  ll-songs-checkbo
-00000d60: 7822 293a 0d0a 2020 2020 2020 2020 2020  x"):..          
-00000d70: 2020 692e 4255 5454 4f4e 5f49 4e4e 4552    i.BUTTON_INNER
-00000d80: 203d 2022 220d 0a20 2020 2020 2020 2020   = ""..         
-00000d90: 2020 2069 2e42 5554 544f 4e5f 4c45 4654     i.BUTTON_LEFT
-00000da0: 203d 2022 220d 0a20 2020 2020 2020 2020   = ""..         
-00000db0: 2020 2069 2e42 5554 544f 4e5f 5249 4748     i.BUTTON_RIGH
-00000dc0: 5420 3d20 2222 0d0a 0d0a 2020 2020 6465  T = ""....    de
-00000dd0: 6620 6f6e 5f62 7574 746f 6e5f 7072 6573  f on_button_pres
-00000de0: 7365 6428 7365 6c66 2c20 6576 656e 743a  sed(self, event:
-00000df0: 2042 7574 746f 6e2e 5072 6573 7365 6429   Button.Pressed)
-00000e00: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-00000e10: 2020 2069 6620 6576 656e 742e 6275 7474     if event.butt
-00000e20: 6f6e 2e69 6420 3d3d 2022 6465 7365 6c65  on.id == "desele
-00000e30: 6374 2d61 6c6c 2d62 7574 746f 6e22 3a0d  ct-all-button":.
-00000e40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00000e50: 2063 6865 636b 626f 7820 696e 2073 656c   checkbox in sel
-00000e60: 662e 6170 702e 7175 6572 7928 222e 616c  f.app.query(".al
-00000e70: 6c2d 736f 6e67 732d 6368 6563 6b62 6f78  l-songs-checkbox
-00000e80: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00000e90: 2020 2020 2063 6865 636b 626f 782e 7661       checkbox.va
-00000ea0: 6c75 6520 3d20 4661 6c73 650d 0a20 2020  lue = False..   
-00000eb0: 2020 2020 2065 6c69 6620 6576 656e 742e       elif event.
-00000ec0: 6275 7474 6f6e 2e69 6420 3d3d 2022 7365  button.id == "se
-00000ed0: 6c65 6374 2d61 6c6c 2d62 7574 746f 6e22  lect-all-button"
-00000ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00000ef0: 6f72 2063 6865 636b 626f 7820 696e 2073  or checkbox in s
-00000f00: 656c 662e 6170 702e 7175 6572 7928 222e  elf.app.query(".
-00000f10: 616c 6c2d 736f 6e67 732d 6368 6563 6b62  all-songs-checkb
-00000f20: 6f78 2229 3a0d 0a20 2020 2020 2020 2020  ox"):..         
-00000f30: 2020 2020 2020 2063 6865 636b 626f 782e         checkbox.
-00000f40: 7661 6c75 6520 3d20 5472 7565 0d0a 2020  value = True..  
-00000f50: 2020 2020 2020 656c 6966 2065 7665 6e74        elif event
-00000f60: 2e62 7574 746f 6e2e 6964 203d 3d20 2264  .button.id == "d
-00000f70: 6f77 6e6c 6f61 642d 7365 6c65 6374 6564  ownload-selected
-00000f80: 2d62 7574 746f 6e22 3a0d 0a20 2020 2020  -button":..     
-00000f90: 2020 2020 2020 2073 656c 662e 6170 702e         self.app.
-00000fa0: 7075 7368 5f73 6372 6565 6e28 446f 776e  push_screen(Down
-00000fb0: 6c6f 6164 2829 290d 0a                   load())..
+000001a0: 6572 3a74 616c 6c20 2462 6f6f 7374 3b0d  er:tall $boost;.
+000001b0: 0a20 2020 2062 6f72 6465 722d 7469 746c  .    border-titl
+000001c0: 652d 616c 6967 6e3a 2063 656e 7465 723b  e-align: center;
+000001d0: 0d0a 2020 2020 7769 6474 683a 2036 333b  ..    width: 63;
+000001e0: 0d0a 2020 2020 6865 6967 6874 3a20 3130  ..    height: 10
+000001f0: 3025 3b0d 0a20 2020 2062 6163 6b67 726f  0%;..    backgro
+00000200: 756e 643a 2024 626f 6f73 743b 0d0a 2020  und: $boost;..  
+00000210: 2020 7061 6464 696e 672d 6c65 6674 3a31    padding-left:1
+00000220: 3b0d 0a20 2020 2070 6164 6469 6e67 2d72  ;..    padding-r
+00000230: 6967 6874 3a31 3b0d 0a20 2020 206d 6172  ight:1;..    mar
+00000240: 6769 6e2d 6c65 6674 3a31 3b0d 0a7d 0d0a  gin-left:1;..}..
+00000250: 0d0a 0d0a 2373 656c 6563 7473 6f6e 6773  ....#selectsongs
+00000260: 2d6c 6162 656c 7b0d 0a20 2020 2064 6f63  -label{..    doc
+00000270: 6b3a 7269 6768 743b 0d0a 2020 2020 6d61  k:right;..    ma
+00000280: 7267 696e 2d72 6967 6874 3a20 3135 3b0d  rgin-right: 15;.
+00000290: 0a7d 0d0a 0d0a 2373 656c 6563 7465 642d  .}....#selected-
+000002a0: 7472 6163 6b73 2d62 7574 746f 6e73 2d63  tracks-buttons-c
+000002b0: 6f6e 7461 696e 6572 7b0d 0a20 2020 2064  ontainer{..    d
+000002c0: 6f63 6b3a 7269 6768 743b 0d0a 2020 2020  ock:right;..    
+000002d0: 7769 6474 683a 2032 373b 0d0a 7d0d 0a0d  width: 27;..}...
+000002e0: 0a23 6465 7365 6c65 6374 2d61 6c6c 2d62  .#deselect-all-b
+000002f0: 7574 746f 6e7b 0d0a 0d0a 2020 2020 6d61  utton{....    ma
+00000300: 7267 696e 2d74 6f70 3a20 313b 0d0a 2020  rgin-top: 1;..  
+00000310: 2020 7769 6474 683a 2032 353b 0d0a 2020    width: 25;..  
+00000320: 2020 6d61 7267 696e 2d6c 6566 743a 2031    margin-left: 1
+00000330: 3b0d 0a7d 0d0a 0d0a 2373 656c 6563 742d  ;..}....#select-
+00000340: 616c 6c2d 6275 7474 6f6e 7b0d 0a20 2020  all-button{..   
+00000350: 2077 6964 7468 3a20 3235 3b0d 0a20 2020   width: 25;..   
+00000360: 206d 6172 6769 6e2d 746f 703a 2031 3b0d   margin-top: 1;.
+00000370: 0a20 2020 206d 6172 6769 6e2d 6c65 6674  .    margin-left
+00000380: 3a20 313b 0d0a 7d0d 0a0d 0a23 646f 776e  : 1;..}....#down
+00000390: 6c6f 6164 2d73 656c 6563 7465 642d 6275  load-selected-bu
+000003a0: 7474 6f6e 7b0d 0a20 2020 2077 6964 7468  tton{..    width
+000003b0: 3a20 3235 3b0d 0a20 2020 206d 6172 6769  : 25;..    margi
+000003c0: 6e2d 746f 703a 2031 3b0d 0a20 2020 206d  n-top: 1;..    m
+000003d0: 6172 6769 6e2d 6c65 6674 3a20 313b 0d0a  argin-left: 1;..
+000003e0: 7d0d 0a0d 0a23 7365 6c65 6374 6564 2d74  }....#selected-t
+000003f0: 7261 636b 732d 6c61 6265 6c7b 0d0a 2020  racks-label{..  
+00000400: 2020 7769 6474 683a 3237 3b0d 0a20 2020    width:27;..   
+00000410: 2068 6569 6768 743a 2033 3b0d 0a20 2020   height: 3;..   
+00000420: 2062 6f72 6465 723a 7461 6c6c 2024 626f   border:tall $bo
+00000430: 6f73 743b 0d0a 2020 2020 6261 636b 6772  ost;..    backgr
+00000440: 6f75 6e64 3a24 626f 6f73 743b 0d0a 2020  ound:$boost;..  
+00000450: 2020 636f 6e74 656e 742d 616c 6967 6e3a    content-align:
+00000460: 6365 6e74 6572 206d 6964 646c 653b 0d0a  center middle;..
+00000470: 2020 2020 6d61 7267 696e 2d62 6f74 746f      margin-botto
+00000480: 6d3a 323b 0d0a 0d0a 7d0d 0a0d 0a0d 0a0d  m:2;....}.......
+00000490: 0a2e 616c 6c2d 736f 6e67 732d 6368 6563  ..all-songs-chec
+000004a0: 6b62 6f78 207b 0d0a 2020 2020 7769 6474  kbox {..    widt
+000004b0: 683a 3536 3b0d 0a20 2020 2070 6164 6469  h:56;..    paddi
+000004c0: 6e67 2d72 6967 6874 3a33 3b0d 0a7d 0d0a  ng-right:3;..}..
+000004d0: 2e61 6c6c 2d73 6f6e 6773 2d63 6865 636b  .all-songs-check
+000004e0: 626f 783a 686f 7665 7220 7b0d 0a20 2020  box:hover {..   
+000004f0: 2074 6578 742d 7374 796c 653a 6e6f 6e65   text-style:none
+00000500: 3b0d 0a20 2020 206f 7061 6369 7479 3a30  ;..    opacity:0
+00000510: 2e38 3b0d 0a7d 0d0a 2e61 6c6c 2d73 6f6e  .8;..}...all-son
+00000520: 6773 2d63 6865 636b 626f 782e 2d6f 6e7b  gs-checkbox.-on{
+00000530: 0d0a 2020 2020 626f 7264 6572 3a20 7461  ..    border: ta
+00000540: 6c6c 2074 7261 6e73 7061 7265 6e74 3b0d  ll transparent;.
+00000550: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+00000560: 2333 3243 4433 323b 0d0a 2020 2020 6f70  #32CD32;..    op
+00000570: 6163 6974 793a 302e 353b 0d0a 7d0d 0a0d  acity:0.5;..}...
+00000580: 0a2e 616c 6c2d 736f 6e67 732d 6368 6563  ..all-songs-chec
+00000590: 6b62 6f78 3a66 6f63 7573 203e 202e 746f  kbox:focus > .to
+000005a0: 6767 6c65 2d2d 6c61 6265 6c20 7b0d 0a20  ggle--label {.. 
+000005b0: 2020 2074 6578 742d 7374 796c 653a 206e     text-style: n
+000005c0: 6f6e 653b 0d0a 2020 2020 6d61 7267 696e  one;..    margin
+000005d0: 2d6c 6566 743a 303b 0d0a 7d0d 0a0d 0a2e  -left:0;..}.....
+000005e0: 616c 6c2d 736f 6e67 732d 6368 6563 6b62  all-songs-checkb
+000005f0: 6f78 3a66 6f63 7573 207b 0d0a 2020 2020  ox:focus {..    
+00000600: 626f 7264 6572 3a74 616c 6c20 7472 616e  border:tall tran
+00000610: 7370 6172 656e 740d 0a7d 0d0a 0d0a 2222  sparent..}....""
+00000620: 220d 0a0d 0a0d 0a63 6c61 7373 2053 656c  "......class Sel
+00000630: 6563 7444 6f77 6e6c 6f61 6428 5363 7265  ectDownload(Scre
+00000640: 656e 293a 0d0a 2020 2020 4445 4641 554c  en):..    DEFAUL
+00000650: 545f 4353 5320 3d20 4353 530d 0a20 2020  T_CSS = CSS..   
+00000660: 2073 656c 6563 7465 645f 7472 6163 6b73   selected_tracks
+00000670: 203d 205b 5d0d 0a0d 0a20 2020 2064 6566   = []....    def
+00000680: 205f 5f69 6e69 745f 5f28 7365 6c66 293a   __init__(self):
+00000690: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+000006a0: 7261 636b 7320 3d20 7365 6c66 2e61 7070  racks = self.app
+000006b0: 2e6c 696e 6b5f 6465 7461 696c 735b 315d  .link_details[1]
+000006c0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+000006d0: 292e 5f5f 696e 6974 5f5f 2829 0d0a 0d0a  ).__init__()....
+000006e0: 2020 2020 6465 6620 636f 6d70 6f73 6528      def compose(
+000006f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000700: 7969 656c 6420 4170 7049 6e74 6572 6661  yield AppInterfa
+00000710: 6365 280d 0a20 2020 2020 2020 2020 2020  ce(..           
+00000720: 2048 6f72 697a 6f6e 7461 6c28 5665 7274   Horizontal(Vert
+00000730: 6963 616c 5363 726f 6c6c 2869 643d 2261  icalScroll(id="a
+00000740: 6c6c 2d74 7261 636b 7322 292c 2069 643d  ll-tracks"), id=
+00000750: 2261 6c6c 2d74 7261 636b 732d 636f 6e74  "all-tracks-cont
+00000760: 6169 6e65 7222 292c 0d0a 2020 2020 2020  ainer"),..      
+00000770: 2020 2020 2020 5665 7274 6963 616c 280d        Vertical(.
+00000780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000790: 2053 7461 7469 6328 2253 454c 4543 5445   Static("SELECTE
+000007a0: 4420 5452 4143 4b53 203a 2030 222c 2069  D TRACKS : 0", i
+000007b0: 643d 2273 656c 6563 7465 642d 7472 6163  d="selected-trac
+000007c0: 6b73 2d6c 6162 656c 2229 2c0d 0a20 2020  ks-label"),..   
+000007d0: 2020 2020 2020 2020 2020 2020 2042 7574               But
+000007e0: 746f 6e28 2244 4553 454c 4543 5420 414c  ton("DESELECT AL
+000007f0: 4c22 2c20 2265 7272 6f72 222c 2069 643d  L", "error", id=
+00000800: 2264 6573 656c 6563 742d 616c 6c2d 6275  "deselect-all-bu
+00000810: 7474 6f6e 2229 2c0d 0a20 2020 2020 2020  tton"),..       
+00000820: 2020 2020 2020 2020 2042 7574 746f 6e28           Button(
+00000830: 2253 454c 4543 5420 414c 4c22 2c20 2270  "SELECT ALL", "p
+00000840: 7269 6d61 7279 222c 2069 643d 2273 656c  rimary", id="sel
+00000850: 6563 742d 616c 6c2d 6275 7474 6f6e 2229  ect-all-button")
+00000860: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000870: 2020 2042 7574 746f 6e28 2244 4f57 4e4c     Button("DOWNL
+00000880: 4f41 4420 5345 4c45 4354 4544 2022 2c20  OAD SELECTED ", 
+00000890: 2273 7563 6365 7373 222c 2069 643d 2264  "success", id="d
+000008a0: 6f77 6e6c 6f61 642d 7365 6c65 6374 6564  ownload-selected
+000008b0: 2d62 7574 746f 6e22 2c64 6973 6162 6c65  -button",disable
+000008c0: 643d 5472 7565 292c 0d0a 2020 2020 2020  d=True),..      
+000008d0: 2020 2020 2020 2020 2020 6964 3d22 7365            id="se
+000008e0: 6c65 6374 6564 2d74 7261 636b 732d 6275  lected-tracks-bu
+000008f0: 7474 6f6e 732d 636f 6e74 6169 6e65 7222  ttons-container"
+00000900: 2c0d 0a20 2020 2020 2020 2020 2020 2029  ,..            )
+00000910: 2c0d 0a20 2020 2020 2020 2029 0d0a 0d0a  ,..        )....
+00000920: 2020 2020 6465 6620 6f6e 5f63 6865 636b      def on_check
+00000930: 626f 785f 6368 616e 6765 6428 7365 6c66  box_changed(self
+00000940: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00000950: 2020 2020 7365 6c65 6374 6564 5f73 6f6e      selected_son
+00000960: 6773 203d 205b 5d0d 0a20 2020 2020 2020  gs = []..       
+00000970: 2066 6f72 2063 6865 636b 626f 7820 696e   for checkbox in
+00000980: 2073 656c 662e 6170 702e 7175 6572 7928   self.app.query(
+00000990: 222e 616c 6c2d 736f 6e67 732d 6368 6563  ".all-songs-chec
+000009a0: 6b62 6f78 2229 3a0d 0a20 2020 2020 2020  kbox"):..       
+000009b0: 2020 2020 2069 6620 6368 6563 6b62 6f78       if checkbox
+000009c0: 2e76 616c 7565 203d 3d20 5472 7565 3a0d  .value == True:.
+000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009e0: 2073 656c 6563 7465 645f 736f 6e67 732e   selected_songs.
+000009f0: 6170 7065 6e64 2873 7472 2863 6865 636b  append(str(check
+00000a00: 626f 782e 6c61 6265 6c29 2e73 706c 6974  box.label).split
+00000a10: 2822 2e20 222c 6d61 7873 706c 6974 3d31  (". ",maxsplit=1
+00000a20: 295b 315d 290d 0a20 2020 2020 2020 2073  )[1])..        s
+00000a30: 656c 662e 6170 702e 7175 6572 795f 6f6e  elf.app.query_on
+00000a40: 6528 2223 7365 6c65 6374 6564 2d74 7261  e("#selected-tra
+00000a50: 636b 732d 6c61 6265 6c22 292e 7570 6461  cks-label").upda
+00000a60: 7465 280d 0a20 2020 2020 2020 2020 2020  te(..           
+00000a70: 2066 2253 454c 4543 5445 4420 5452 4143   f"SELECTED TRAC
+00000a80: 4b53 203a 207b 6c65 6e28 7365 6c65 6374  KS : {len(select
+00000a90: 6564 5f73 6f6e 6773 297d 220d 0a20 2020  ed_songs)}"..   
+00000aa0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00000ab0: 7365 6c66 2e61 7070 2e73 656c 6563 7465  self.app.selecte
+00000ac0: 645f 7472 6163 6b73 203d 205b 7365 6c66  d_tracks = [self
+00000ad0: 2e74 7261 636b 735b 736f 6e67 5d20 666f  .tracks[song] fo
+00000ae0: 7220 736f 6e67 2069 6e20 7365 6c65 6374  r song in select
+00000af0: 6564 5f73 6f6e 6773 5d0d 0a20 2020 2020  ed_songs]..     
+00000b00: 2020 2069 6620 6c65 6e28 7365 6c66 2e61     if len(self.a
+00000b10: 7070 2e73 656c 6563 7465 645f 7472 6163  pp.selected_trac
+00000b20: 6b73 2920 213d 2030 203a 0d0a 2020 2020  ks) != 0 :..    
+00000b30: 2020 2020 2020 2020 7365 6c66 2e71 7565          self.que
+00000b40: 7279 5f6f 6e65 2827 2364 6f77 6e6c 6f61  ry_one('#downloa
+00000b50: 642d 7365 6c65 6374 6564 2d62 7574 746f  d-selected-butto
+00000b60: 6e27 292e 6469 7361 626c 6564 203d 2046  n').disabled = F
+00000b70: 616c 7365 0d0a 2020 2020 2020 2020 656c  alse..        el
+00000b80: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000b90: 2073 656c 662e 7175 6572 795f 6f6e 6528   self.query_one(
+00000ba0: 2723 646f 776e 6c6f 6164 2d73 656c 6563  '#download-selec
+00000bb0: 7465 642d 6275 7474 6f6e 2729 2e64 6973  ted-button').dis
+00000bc0: 6162 6c65 6420 3d20 5472 7565 0d0a 0d0a  abled = True....
+00000bd0: 2020 2020 6465 6620 6f6e 5f6d 6f75 6e74      def on_mount
+00000be0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000bf0: 2073 656c 662e 6170 702e 7175 6572 795f   self.app.query_
+00000c00: 6f6e 6528 2223 6e61 762d 6c61 6265 6c22  one("#nav-label"
+00000c10: 292e 7570 6461 7465 2822 5b62 6f6c 645d  ).update("[bold]
+00000c20: 5345 4c45 4354 2054 5241 434b 5320 544f  SELECT TRACKS TO
+00000c30: 2044 4f57 4e4c 4f41 4422 290d 0a20 2020   DOWNLOAD")..   
+00000c40: 2020 2020 2066 6f72 2073 6f6e 672c 2074       for song, t
+00000c50: 7261 636b 5f6e 6f20 696e 207a 6970 280d  rack_no in zip(.
+00000c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000c70: 662e 7472 6163 6b73 2e6b 6579 7328 292c  f.tracks.keys(),
+00000c80: 2072 616e 6765 2831 2c20 6c65 6e28 7365   range(1, len(se
+00000c90: 6c66 2e74 7261 636b 732e 6b65 7973 2829  lf.tracks.keys()
+00000ca0: 2920 2b20 3129 0d0a 2020 2020 2020 2020  ) + 1)..        
+00000cb0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000cc0: 7365 6c66 2e61 7070 2e71 7565 7279 5f6f  self.app.query_o
+00000cd0: 6e65 2822 2361 6c6c 2d74 7261 636b 7322  ne("#all-tracks"
+00000ce0: 292e 6d6f 756e 7428 0d0a 2020 2020 2020  ).mount(..      
+00000cf0: 2020 2020 2020 2020 2020 4368 6563 6b62            Checkb
+00000d00: 6f78 2866 227b 7472 6163 6b5f 6e6f 7d2e  ox(f"{track_no}.
+00000d10: 2022 202b 2073 6f6e 672c 2063 6c61 7373   " + song, class
+00000d20: 6573 3d22 616c 6c2d 736f 6e67 732d 6368  es="all-songs-ch
+00000d30: 6563 6b62 6f78 2229 0d0a 2020 2020 2020  eckbox")..      
+00000d40: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00000d50: 2066 6f72 2069 2069 6e20 7365 6c66 2e61   for i in self.a
+00000d60: 7070 2e71 7565 7279 2822 2e61 6c6c 2d73  pp.query(".all-s
+00000d70: 6f6e 6773 2d63 6865 636b 626f 7822 293a  ongs-checkbox"):
+00000d80: 0d0a 2020 2020 2020 2020 2020 2020 692e  ..            i.
+00000d90: 4255 5454 4f4e 5f49 4e4e 4552 203d 2022  BUTTON_INNER = "
+00000da0: 220d 0a20 2020 2020 2020 2020 2020 2069  "..            i
+00000db0: 2e42 5554 544f 4e5f 4c45 4654 203d 2022  .BUTTON_LEFT = "
+00000dc0: 220d 0a20 2020 2020 2020 2020 2020 2069  "..            i
+00000dd0: 2e42 5554 544f 4e5f 5249 4748 5420 3d20  .BUTTON_RIGHT = 
+00000de0: 2222 0d0a 0d0a 2020 2020 6465 6620 6f6e  ""....    def on
+00000df0: 5f62 7574 746f 6e5f 7072 6573 7365 6428  _button_pressed(
+00000e00: 7365 6c66 2c20 6576 656e 743a 2042 7574  self, event: But
+00000e10: 746f 6e2e 5072 6573 7365 6429 202d 3e20  ton.Pressed) -> 
+00000e20: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
+00000e30: 6620 6576 656e 742e 6275 7474 6f6e 2e69  f event.button.i
+00000e40: 6420 3d3d 2022 6465 7365 6c65 6374 2d61  d == "deselect-a
+00000e50: 6c6c 2d62 7574 746f 6e22 3a0d 0a20 2020  ll-button":..   
+00000e60: 2020 2020 2020 2020 2066 6f72 2063 6865           for che
+00000e70: 636b 626f 7820 696e 2073 656c 662e 6170  ckbox in self.ap
+00000e80: 702e 7175 6572 7928 222e 616c 6c2d 736f  p.query(".all-so
+00000e90: 6e67 732d 6368 6563 6b62 6f78 2229 3a0d  ngs-checkbox"):.
+00000ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000eb0: 2063 6865 636b 626f 782e 7661 6c75 6520   checkbox.value 
+00000ec0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
+00000ed0: 2065 6c69 6620 6576 656e 742e 6275 7474   elif event.butt
+00000ee0: 6f6e 2e69 6420 3d3d 2022 7365 6c65 6374  on.id == "select
+00000ef0: 2d61 6c6c 2d62 7574 746f 6e22 3a0d 0a20  -all-button":.. 
+00000f00: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00000f10: 6865 636b 626f 7820 696e 2073 656c 662e  heckbox in self.
+00000f20: 6170 702e 7175 6572 7928 222e 616c 6c2d  app.query(".all-
+00000f30: 736f 6e67 732d 6368 6563 6b62 6f78 2229  songs-checkbox")
+00000f40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000f50: 2020 2063 6865 636b 626f 782e 7661 6c75     checkbox.valu
+00000f60: 6520 3d20 5472 7565 0d0a 2020 2020 2020  e = True..      
+00000f70: 2020 656c 6966 2065 7665 6e74 2e62 7574    elif event.but
+00000f80: 746f 6e2e 6964 203d 3d20 2264 6f77 6e6c  ton.id == "downl
+00000f90: 6f61 642d 7365 6c65 6374 6564 2d62 7574  oad-selected-but
+00000fa0: 746f 6e22 3a0d 0a20 2020 2020 2020 2020  ton":..         
+00000fb0: 2020 2073 656c 662e 6170 702e 7075 7368     self.app.push
+00000fc0: 5f73 6372 6565 6e28 446f 776e 6c6f 6164  _screen(Download
+00000fd0: 2829 290d 0a                             ())..
```

### Comparing `spotidex-0.0.6/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-0.0.7/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-0.0.7/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-0.0.7/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,30 +37,25 @@
     height:3;
     dock:right;
     padding-left:1;
     margin-left:1;
   
 }
 
-#metadata-checkbox:hover.inactive{
-    opacity:0.6;
+#metadata-checkbox:hover{
+    opacity:0.8;
 
 }
 
-#metadata-checkbox:hover.active{
-    opacity:1;
-
-}
 
 .inactive{
-    background:#787878;
-    opacity:0.5;
+    background:$error 8%;
 }
 .active{
-    background:$success 90%;
+    background:$success 8%;
 }
 
 """
 
 
 class MetadataCheckBox(Widget):
     DEFAULT_CSS = CSS
@@ -71,19 +66,19 @@
         with Container(id="main-container"):
             with Container(id="metadata-checkbox-container"):
                 yield Static("INCLUDE METADATA", id="metadata-checkbox-label")
                 yield Static(id="metadata-checkbox")
 
     def watch_value(self, value):
         if value == True:
-            self.query_one("#metadata-checkbox").update("✔️")
+            self.query_one("#metadata-checkbox").update("🟢")
             self.query_one("#metadata-checkbox").remove_class("inactive")
             self.query_one("#metadata-checkbox").add_class("active")
         else:
-            self.query_one("#metadata-checkbox").update("")
+            self.query_one("#metadata-checkbox").update("🔴")
             self.query_one("#metadata-checkbox").remove_class("active")
             self.query_one("#metadata-checkbox").add_class("inactive")
  
 
     def on_click(self) -> None:
         if self.value == True:
             self.value = False
```

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc` & `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-0.0.7/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     width:71;
     margin-top:1;
     align:center middle;
 }
 
 #download-path-confirm-button{
     width:23;
-    dock:left;
+    dock:right;
 
 }
 
 #download-path-reset-button{
     width:22;
     
 }
@@ -75,16 +75,16 @@
     dock:right;
     border:gray;
     background:transparent;
 
 }
 
 #downloads-folder-button{
-    dock:right;
     width:22;
+    dock:left;
 }
 
 #download-path-back-button:hover {
    tint: $background 20%;
 }
 
 """
@@ -108,23 +108,23 @@
                     highlight=True, markup=True, id="download-path-log"
                 ).write(shorten_path(self.current_path, 60))
             yield Button("BACK", id="download-path-back-button", variant="primary")
             with Container(id="select-download-path-container"):
                 yield self.FilteredDirectoryTree(self.current_path, id="filteredtree")
             with Container(id="download-path-button-container"):
                 yield Button(
-                    "CONFIRM", id="download-path-confirm-button", variant="success"
+                    "DOWNLOADS FOLDER", id="downloads-folder-button", variant="warning"
                 )
                 yield Button(
                     "CURRENT DIRECTORY",
                     id="download-path-reset-button",
                     variant="error",
                 )
                 yield Button(
-                    "DOWNLOADS FOLDER", id="downloads-folder-button", variant="warning"
+                    "CONFIRM", id="download-path-confirm-button", variant="success"
                 )
 
     def refresh_tree(self):
         self.app.query_one("#select-download-path-container").remove_children()
         self.app.query_one("#select-download-path-container").mount(
             self.FilteredDirectoryTree(self.current_path, id="filteredtree")
         )
```

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-0.0.7/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-0.0.7/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-0.0.7/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/SpotidexApp.py` & `spotidex-0.0.7/spotidex/cli/SpotidexApp.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/cli/utils.py` & `spotidex-0.0.7/spotidex/cli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from spotidex import SpotifyContent
 from spotidex import SpotifyDownloader
 from pathlib import Path
 import os
 import shutil
 
 scraper = SpotifyContent()
@@ -17,14 +16,15 @@
 
 Spotidex supports a wide range of Spotify links, enabling \
 users to download playlists, individual tracks, and entire albums effortlessly.
 
 App's GitHub repository is available at [link=https://github.com/libin-codes/spotidex]https://github.com/libin-codes/spotidex[/link][/italic]
 """
 
+
 def get_link_details(link):
     if "track" in link:
         track_details = scraper.track_details(link)
         return (
             {
                 "TRACK ID": link.split("/")[-1].split("?")[0],
                 "TRACK NAME": track_details["track_name"],
@@ -85,29 +85,64 @@
 input_validator = lambda value: (
     True
     if ("spotify" in value)
     and (any(keyword in value for keyword in ["track", "playlist", "album"]))
     else False
 )
 
+
 def get_data_drive_path():
-    if os.name == 'nt':  # Windows
-        system_drive = os.environ['SYSTEMDRIVE'] if 'SYSTEMDRIVE' in os.environ else 'C:'
-        drives = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
-        available_drives = [drive + ':\\' for drive in drives if os.path.exists(drive + ':\\') and drive + ':' != system_drive]
+    if os.name == "nt":  # Windows
+        system_drive = (
+            os.environ["SYSTEMDRIVE"] if "SYSTEMDRIVE" in os.environ else "C:"
+        )
+        drives = [
+            "A",
+            "B",
+            "C",
+            "D",
+            "E",
+            "F",
+            "G",
+            "H",
+            "I",
+            "J",
+            "K",
+            "L",
+            "M",
+            "N",
+            "O",
+            "P",
+            "Q",
+            "R",
+            "S",
+            "T",
+            "U",
+            "V",
+            "W",
+            "X",
+            "Y",
+            "Z",
+        ]
+        available_drives = [
+            drive + ":\\"
+            for drive in drives
+            if os.path.exists(drive + ":\\") and drive + ":" != system_drive
+        ]
         return available_drives[0] if available_drives else None
     else:  # Unix-like systems
         # Filter out root directory ('/') from mounted drives
-        mounted_drives = [root for root, dirs, files in os.walk('/') if dirs or files]
+        mounted_drives = [root for root, dirs, files in os.walk("/") if dirs or files]
         return mounted_drives[0] if mounted_drives else None
 
+
 def get_downloads_folder():
     # Get the user's home directory
     home_dir = os.path.expanduser("~")
-    
+
     # Operating system specific logic to get the Downloads folder
-    if os.name == 'posix':  # Unix-like OS (Linux, macOS)
-        downloads_folder = os.path.join(home_dir, 'Downloads')
-    elif os.name == 'nt':   # Windows
-        downloads_folder = os.path.join(home_dir, 'Downloads')
-    
-    return downloads_folder
+    if os.name == "posix":  # Unix-like OS (Linux, macOS)
+        downloads_folder = os.path.join(home_dir, "Downloads")
+    elif os.name == "nt":  # Windows
+        downloads_folder = os.path.join(home_dir, "Downloads")
+
+    return downloads_folder
```

### Comparing `spotidex-0.0.6/spotidex/src/download.py` & `spotidex-0.0.7/spotidex/src/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tempfile import TemporaryDirectory
 import shutil
 import yt_dlp.YoutubeDL
 import spotipy
 from spotipy.oauth2 import SpotifyClientCredentials
 from spotipy import SpotifyException
 from requests import ConnectionError,ReadTimeout
-
+from spotidex.src.content import SpotifyContent
 
 
 class SpotifyDownloader:
     def __init__(self) -> None:
         self.spotidex_path = get_spotidex_data_directory()
         self.ffmpeg_path = get_ffmpeg()
         self.total_tracks = None
@@ -64,15 +64,14 @@
     ):
         try:
             data = self.sp.track(link.split("/")[-1].split("?")[0])
         except SpotifyException:
             raise SpotidexError("InvalidSpotifyLink")
         except (ConnectionError,ReadTimeout):
             raise SpotidexError("NetworkError")
-
         
         track_artist = ",".join([artist["name"] for artist in data["artists"]])
         query = data["name"]+f" song by {track_artist} official lyrics "
         file_name = get_valid_name(download_path,data["name"]+".mp3")
     
         with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
             options = {
@@ -119,22 +118,22 @@
         download_path=Path.cwd(),
         quality="high",
         metadata=True,
         make_folder=True,
     ):
         playlist_id = link.split("/")[-1].split("?")[0]
         try:
-            playlist_data = self.sp.playlist(playlist_id)
-            track_links = extract_track_links(self.sp, link)
+            playlist_data = SpotifyContent().playlist_details(playlist_id)
+            track_links = [track["link"] for track in playlist_data['track_details']]
         except SpotifyException:
             raise SpotidexError("InvalidSpotifyLink")
         except (ConnectionError,ReadTimeout):
             raise SpotidexError("NetworkError")
         
-        folder_name = get_valid_name(download_path,playlist_data['name'])
+        folder_name = get_valid_name(download_path,playlist_data['playlist_name'])
 
         self._download_with_temp_directory(
                 track_links,
                 folder_name,
                 custom_hook,
                 download_path,
                 quality,
@@ -149,16 +148,16 @@
         download_path=Path.cwd(),
         quality="high",
         metadata=True,
         make_folder=True,
     ):
         album_id = link.split("/")[-1].split("?")[0]
         try:
-            album_data = self.sp.album(album_id)
-            track_links = extract_track_links(self.sp, link)
+            album_data = SpotifyContent().album_details(album_id)
+            track_links = [track["link"] for track in album_data['track_details']]
         except SpotifyException:
             raise SpotidexError("InvalidSpotifyLink")
         except (ConnectionError,ReadTimeout):
             raise SpotidexError("NetworkError")
         
         
         folder_name = get_valid_name(download_path,album_data['name'])
```

### Comparing `spotidex-0.0.6/spotidex/src/static.py` & `spotidex-0.0.7/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.6/spotidex/src/utils.py` & `spotidex-0.0.7/spotidex/src/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,22 @@
-import os,re,stat,platform,requests,subprocess
+import os, re, stat, platform, requests, subprocess
 from mutagen.id3 import ID3, APIC, TPE1, TIT2, TALB
 import concurrent.futures
 from pathlib import Path
-from tqdm import tqdm
 from rich.progress import Progress, SpinnerColumn
-from rich.console import Console
 
 from spotidex.src.static import FFMPEG_URLS
 
 progress_dict = {}
+
 class SpotidexError(Exception):
-    def __init__(self,message):
+    def __init__(self, message):
         self.message = message
         super().__init__(message)
 
-def extract_track_links(sp, link):
-    id = link.split("/")[-1].split("?")[0]
-    is_playlist = "playlist" in link
-    data = sp.playlist(id) if is_playlist else sp.album(id)
-    total_tracks = data["tracks"]["total"]
-    offset, limit = 0, 100 if is_playlist else 40
-    track_links = []
-
-    while offset < total_tracks:
-        results = (
-            sp.playlist_items(id, offset=offset, limit=limit)
-            if is_playlist
-            else sp.album_tracks(id, offset=offset, limit=limit)
-        )
-        for track in results["items"]:
-            track_links.append(track["track"]["href"] if is_playlist else track["href"])
-        offset += limit
-    return track_links
-
-
 def add_metadata(data, path):
     audio = ID3(path)
     audio.add(TIT2(encoding=3, text=data["name"]))
     audio.add(
         TPE1(encoding=3, text=",".join([artist["name"] for artist in data["artists"]]))
     )
     audio.add(TALB(encoding=3, text=data["album"]["name"]))
@@ -84,83 +63,77 @@
     if custom_hook is None:
         return
     if d["status"] == "downloading":
         percent = "".join(
             char for char in d["_percent_str"] if char.isdigit() or char == "."
         )
         if self.total_tracks != None:
-            progress_dict.update(
-                {d["info_dict"]["id"]: float(percent[3:]) * 0.943}
-            )
+            progress_dict.update({d["info_dict"]["id"]: float(percent[3:]) * 0.943})
             progress = sum(progress_dict.values()) / self.total_tracks
             custom_hook(str(round(progress, 1)))
         else:
             custom_hook(str(round(float(percent[3:]) * 0.943, 1)))
     elif d["status"] == "downloaded":
         custom_hook("97.8")
     elif d["status"] == "transfered":
         custom_hook("100")
         progress_dict = {}
         self.total_tracks = None
 
-
-def parallel_searches(self, track_links):
-    with concurrent.futures.ThreadPoolExecutor(max_workers=6) as executor:
-        tasks = [executor.submit(self.track_details, link) for link in track_links]
-        concurrent.futures.wait(tasks)
-    return [task.result() for task in tasks]
-
-
 def get_spotidex_data_directory():
     spotidex_path = Path(os.path.expanduser("~"), ".spotidex")
     spotidex_path.mkdir(parents=True, exist_ok=True)
     return spotidex_path
 
+
 def get_ffmpeg():
     os_name = platform.system().lower()
     os_arch = platform.machine().lower()
 
     ffmpeg_url = FFMPEG_URLS.get(os_name, {}).get(os_arch)
     ffmpeg_path = get_ffmpeg_path(os_name)
 
     if ffmpeg_path.exists():
-        if not run_ffmpeg(ffmpeg_path) :
+        if not run_ffmpeg(ffmpeg_path):
             download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name)
         return ffmpeg_path
 
     download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name)
     return ffmpeg_path
 
+
 def get_ffmpeg_path(os_name):
     executable_extension = ".exe" if os_name == "windows" else ""
     return get_spotidex_data_directory() / f"ffmpeg{executable_extension}"
 
+
 def run_ffmpeg(ffmpeg_path):
     current_path = Path().cwd()
     os.chdir(get_spotidex_data_directory())
     try:
         subprocess.run(
             [ffmpeg_path], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
     except Exception:
         return False
     os.chdir(current_path)
     return True
 
+
 def download_ffmpeg(ffmpeg_url, ffmpeg_path, os_name):
     try:
         ffmpeg_binary = requests.get(ffmpeg_url, stream=True, timeout=10)
     except Exception:
         print("Network Error: Please check your internet connection and try later")
         exit()
     with open(ffmpeg_path, "wb") as ffmpeg_file:
         try:
             total_length = int(ffmpeg_binary.headers.get("content-length", 0))
             with Progress(
-                SpinnerColumn('arc'),
+                SpinnerColumn("arc"),
                 " INITIALIZING{task.percentage:>3.0f}%",
             ) as progress:
                 task = progress.add_task("Downloading", total=total_length)
                 for data in ffmpeg_binary.iter_content(chunk_size=1024):
                     ffmpeg_file.write(data)
                     progress.update(task, advance=len(data), total_bytes=total_length)
         except Exception as e:
@@ -170,9 +143,14 @@
     if os_name in ["linux", "darwin"]:
         ffmpeg_path.chmod(ffmpeg_path.stat().st_mode | stat.S_IEXEC)
 
 def get_valid_name(path, name):
     name, i = re.sub(r"[^\w\d(),.\-\[\] ]", "", name), 1
     add_mp3 = ".mp3" if ".mp3" in name else ""
     while Path(path, name).exists():
-        name, i = name.replace('.mp3',"").split(" (")[-1] + f" ({i})" + add_mp3, i + 1
-    return name.replace('.mp3',"")
+        name, i = (
+            (name.replace(".mp3", "") + f" ({i})" + add_mp3, i + 1)
+            if i == 1
+            else (name.replace('.mp3',"")[::-1].split("(",1)[-1][::-1] + f"({i})" + add_mp3, i + 1)
+        )
+
+    return name.replace(".mp3", "")
```

### Comparing `spotidex-0.0.6/PKG-INFO` & `spotidex-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spotify Downloader TUI
 License: MIT
 Author: Libin Lalu
 Author-email: libinlalu000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mutagen (==1.47.0)
-Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: pyperclip (==1.8.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.1)
 Requires-Dist: spotipy (==2.23.0)
 Requires-Dist: textual (==0.56.4)
 Requires-Dist: tqdm (==4.66.1)
 Requires-Dist: yt-dlp (==2024.3.10)
 Requires-Dist: ytmusicapi (==1.3.2)
```

