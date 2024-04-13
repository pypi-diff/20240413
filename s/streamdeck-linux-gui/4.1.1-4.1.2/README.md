# Comparing `tmp/streamdeck_linux_gui-4.1.1.tar.gz` & `tmp/streamdeck_linux_gui-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeck_linux_gui-4.1.1.tar", max compression
+gzip compressed data, was "streamdeck_linux_gui-4.1.2.tar", max compression
```

## Comparing `streamdeck_linux_gui-4.1.1.tar` & `streamdeck_linux_gui-4.1.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1072 2024-03-04 21:48:40.079570 streamdeck_linux_gui-4.1.1/LICENSE
--rw-r--r--   0        0        0     7684 2024-03-04 21:48:40.079570 streamdeck_linux_gui-4.1.1/README.md
--rw-r--r--   0        0        0     1544 2024-03-04 21:49:11.964114 streamdeck_linux_gui-4.1.1/pyproject.toml
--rw-r--r--   0        0        0       98 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/__init__.py
--rw-r--r--   0        0        0    32075 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/api.py
--rw-r--r--   0        0        0    33773 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/button.ui
--rw-r--r--   0        0        0        0 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/cli/__init__.py
--rw-r--r--   0        0        0     7958 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/cli/commands.py
--rw-r--r--   0        0        0     9715 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/cli/server.py
--rw-r--r--   0        0        0     9770 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/config.py
--rw-r--r--   0        0        0     3266 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/dimmer.py
--rw-r--r--   0        0        0        0 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/__init__.py
--rw-r--r--   0        0        0     1222 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/background_color_filter.py
--rw-r--r--   0        0        0    11274 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/display_grid.py
--rw-r--r--   0        0        0     1330 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/empty_filter.py
--rw-r--r--   0        0        0     2441 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/filter.py
--rw-r--r--   0        0        0     5075 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/image_filter.py
--rw-r--r--   0        0        0     1915 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/keypress_filter.py
--rw-r--r--   0        0        0     2807 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/pipeline.py
--rw-r--r--   0        0        0     1581 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/pulse_filter.py
--rw-r--r--   0        0        0     5191 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/display/text_filter.py
--rw-r--r--   0        0        0    11560 2024-03-04 21:48:40.087570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/LICENSE.txt
--rw-r--r--   0        0        0   171072 2024-03-04 21:48:40.091570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   177120 2024-03-04 21:48:40.091570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   170348 2024-03-04 21:48:40.091570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   174520 2024-03-04 21:48:40.091570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   173516 2024-03-04 21:48:40.095570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   170012 2024-03-04 21:48:40.095570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   176184 2024-03-04 21:48:40.095570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   171656 2024-03-04 21:48:40.099570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   176428 2024-03-04 21:48:40.099570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   171272 2024-03-04 21:48:40.099570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   171500 2024-03-04 21:48:40.099570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   175872 2024-03-04 21:48:40.099570 streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0    50598 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/gui.py
--rw-r--r--   0        0        0      372 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/add_page.png
--rw-r--r--   0        0        0     1081 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/cross.png
--rw-r--r--   0        0        0     1341 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/gear.png
--rw-r--r--   0        0        0      533 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/horizontal-align.png
--rw-r--r--   0        0        0      250 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/remove_page.png
--rw-r--r--   0        0        0      236 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/vertical-align.png
--rw-r--r--   0        0        0    24041 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/warning_icon_button.png
--rw-r--r--   0        0        0      306 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/logger.py
--rw-r--r--   0        0        0    17681 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/logo.png
--rw-r--r--   0        0        0    12539 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/main.ui
--rw-r--r--   0        0        0     6301 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/mock_streamdeck.py
--rw-r--r--   0        0        0     2529 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/model.py
--rw-r--r--   0        0        0        0 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/__init__.py
--rw-r--r--   0        0        0     7013 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/fonts.py
--rw-r--r--   0        0        0    11142 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/keyboard.py
--rw-r--r--   0        0        0        0 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/utils/__init__.py
--rw-r--r--   0        0        0      861 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/utils/timers.py
--rw-r--r--   0        0        0      284 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/resources.qrc
--rw-r--r--   0        0        0    13372 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/resources_rc.py
--rw-r--r--   0        0        0     1007 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/semaphore.py
--rw-r--r--   0        0        0     4118 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/settings.ui
--rw-r--r--   0        0        0     6818 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/stream_deck_monitor.py
--rw-r--r--   0        0        0    19864 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_button.py
--rw-r--r--   0        0        0    12301 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_main.py
--rw-r--r--   0        0        0     5184 2024-03-04 21:48:40.103570 streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_settings.py
--rw-r--r--   0        0        0     8686 1970-01-01 00:00:00.000000 streamdeck_linux_gui-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-13 09:08:15.895311 streamdeck_linux_gui-4.1.2/LICENSE
+-rw-r--r--   0        0        0     7684 2024-04-13 09:08:15.895311 streamdeck_linux_gui-4.1.2/README.md
+-rw-r--r--   0        0        0     1544 2024-04-13 09:08:52.971346 streamdeck_linux_gui-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/__init__.py
+-rw-r--r--   0        0        0    32075 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/api.py
+-rw-r--r--   0        0        0    33773 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/button.ui
+-rw-r--r--   0        0        0        0 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/cli/__init__.py
+-rw-r--r--   0        0        0     7958 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/cli/commands.py
+-rw-r--r--   0        0        0     9715 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/cli/server.py
+-rw-r--r--   0        0        0     9770 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/config.py
+-rw-r--r--   0        0        0     3266 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/dimmer.py
+-rw-r--r--   0        0        0        0 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/background_color_filter.py
+-rw-r--r--   0        0        0    11313 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/display_grid.py
+-rw-r--r--   0        0        0     1330 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/empty_filter.py
+-rw-r--r--   0        0        0     2441 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/filter.py
+-rw-r--r--   0        0        0     5200 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/image_filter.py
+-rw-r--r--   0        0        0     1915 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/keypress_filter.py
+-rw-r--r--   0        0        0     2807 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/pipeline.py
+-rw-r--r--   0        0        0     1581 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/pulse_filter.py
+-rw-r--r--   0        0        0     5191 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/display/text_filter.py
+-rw-r--r--   0        0        0    11560 2024-04-13 09:08:15.903311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/LICENSE.txt
+-rw-r--r--   0        0        0   171072 2024-04-13 09:08:15.907311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   177120 2024-04-13 09:08:15.907311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   170348 2024-04-13 09:08:15.907311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   174520 2024-04-13 09:08:15.907311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   173516 2024-04-13 09:08:15.911311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   170012 2024-04-13 09:08:15.911311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   176184 2024-04-13 09:08:15.911311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   171656 2024-04-13 09:08:15.915311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   176428 2024-04-13 09:08:15.915311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   171272 2024-04-13 09:08:15.915311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   171500 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   175872 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0    50643 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/gui.py
+-rw-r--r--   0        0        0      372 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/add_page.png
+-rw-r--r--   0        0        0     1081 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/cross.png
+-rw-r--r--   0        0        0     1341 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/gear.png
+-rw-r--r--   0        0        0      533 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/horizontal-align.png
+-rw-r--r--   0        0        0      250 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/remove_page.png
+-rw-r--r--   0        0        0      236 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/vertical-align.png
+-rw-r--r--   0        0        0    24041 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/warning_icon_button.png
+-rw-r--r--   0        0        0      306 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/logger.py
+-rw-r--r--   0        0        0    17681 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/logo.png
+-rw-r--r--   0        0        0    12539 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/main.ui
+-rw-r--r--   0        0        0     6301 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/mock_streamdeck.py
+-rw-r--r--   0        0        0     2529 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/model.py
+-rw-r--r--   0        0        0        0 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/__init__.py
+-rw-r--r--   0        0        0     7013 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/fonts.py
+-rw-r--r--   0        0        0    13283 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/keyboard.py
+-rw-r--r--   0        0        0        0 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/utils/timers.py
+-rw-r--r--   0        0        0      284 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/resources.qrc
+-rw-r--r--   0        0        0    13372 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/resources_rc.py
+-rw-r--r--   0        0        0     1007 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/semaphore.py
+-rw-r--r--   0        0        0     4118 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/settings.ui
+-rw-r--r--   0        0        0     6818 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/stream_deck_monitor.py
+-rw-r--r--   0        0        0    19864 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_button.py
+-rw-r--r--   0        0        0    12301 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_main.py
+-rw-r--r--   0        0        0     5184 2024-04-13 09:08:15.919311 streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_settings.py
+-rw-r--r--   0        0        0     8686 1970-01-01 00:00:00.000000 streamdeck_linux_gui-4.1.2/PKG-INFO
```

### Comparing `streamdeck_linux_gui-4.1.1/LICENSE` & `streamdeck_linux_gui-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/README.md` & `streamdeck_linux_gui-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/pyproject.toml` & `streamdeck_linux_gui-4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamdeck-linux-gui"
-version = "4.1.1"
+version = "4.1.2"
 description = "A service, Web Interface, and UI for interacting with your computer using a Stream Deck"
 authors = ["Timothy Crosley <timothy.crosley@gmail.com>"]
 maintainers = ["4s3ti <4s3ti@4s3ti.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "streamdeck_ui"}
```

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/api.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/api.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/button.ui` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/button.ui`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/cli/commands.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/cli/commands.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/cli/server.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/cli/server.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/config.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/config.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/dimmer.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/dimmer.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/background_color_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/background_color_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/display_grid.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/display_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 
 class DisplayGrid:
     """
     A DisplayGrid is made up of a collection of pipelines, each processing
     filters for one individual button display.
     """
 
-    _empty_filter: EmptyFilter = EmptyFilter()
-    "Static instance of EmptyFilter shared by all pipelines"
-
     lock: threading.Lock
 
     def __init__(
         self,
         lock: threading.Lock,
         streamdeck: StreamDeck,
         pages: List[int],
@@ -54,14 +51,19 @@
         if streamdeck.is_visual():
             self.size = streamdeck.key_image_format()["size"]
         else:
             self.size = (StreamDeckOriginal.KEY_PIXEL_WIDTH, StreamDeckOriginal.KEY_PIXEL_HEIGHT)
             # Default to original stream deck size - even though we're not actually going to display anything
         self.serial_number = streamdeck.get_serial_number()
 
+        self._empty_filter: EmptyFilter = EmptyFilter()
+        self._empty_filter.initialize(self.size)
+        # Instance of EmptyFilter shared by all pipelines related to this
+        # DisplayGrid instance
+
         self.pages: Dict[int, Dict[int, Pipeline]] = {}
         # A dictionary of lists of pipelines. Each page has
         # a list, corresponding to each button.
 
         self.current_page: int = -1
         self.pipeline_thread: Optional[threading.Thread] = None
         self.quit = threading.Event()
@@ -72,30 +74,29 @@
         self.sync = threading.Event()
         self.cpu_callback = cpu_callback
 
         # Initialize with a pipeline per key for all pages
         for page in pages:
             self.initialize_page(page)
         # The sync event allows a caller to wait until all the buttons have been processed
-        DisplayGrid._empty_filter.initialize(self.size)
 
     def initialize_page(self, page: int):
         self.pages[page] = {}
         for button in range(self.streamdeck.key_count()):
             self.pages[page][button] = Pipeline()
             self.replace(page, button, [])
 
     def remove_page(self, page: int):
         with self.lock:
             del self.pages[page]
 
     def replace(self, page: int, button: int, filters: List[Filter]):
         with self.lock:
             pipeline = Pipeline()
-            pipeline.add(DisplayGrid._empty_filter)
+            pipeline.add(self._empty_filter)
             for pipeline_filter in filters:
                 pipeline_filter.initialize(self.size)
                 pipeline.add(pipeline_filter)
             keypress = KeypressFilter()
             keypress.initialize(self.size)
             pipeline.add(keypress)
             self.pages[page][button] = pipeline
```

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/empty_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/empty_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/image_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/image_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         for frame, milliseconds, hashcode in zip(frames, frame_duration, frame_hash):
             frame = frame.copy()
             if frame.has_transparency_data and frame.mode != "RGBA":
                 try:
                     frame = frame.convert("RGBA")
                 except BaseException:
                     pass
-            frame.thumbnail(size, Image.LANCZOS)
+            scale_factor = min(size[0] / frame.size[0], size[1] / frame.size[1])
+            frame = frame.resize((int(v * scale_factor) for v in frame.size), Image.LANCZOS)
             self.frames.append((frame, milliseconds, hashcode))
 
         self.frame_cycle = itertools.cycle(self.frames)
         self.current_frame = next(self.frame_cycle)
         self.frame_time = Fraction()
 
     def transform(
```

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/keypress_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/keypress_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/pipeline.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/pipeline.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/pulse_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/pulse_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/display/text_filter.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/display/text_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/LICENSE.txt` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Black.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Light.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/gui.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -933,15 +933,17 @@
         column_layout.addStretch(1)
     row_layout.addStretch(1)
 
     # Note that the button click event captures the ui variable, the current button
     #  and all the other buttons
     for button in buttons:
         button.clicked.connect(
-            lambda current_button=button, all_buttons=buttons: button_clicked(current_button, all_buttons)
+            lambda checked=False, current_button=button, all_buttons=buttons: button_clicked(
+                current_button, all_buttons
+            )
         )
 
 
 def export_config(window, api) -> None:
     file_name = QFileDialog.getSaveFileName(
         window, "Export Config", os.path.expanduser("~/streamdeck_ui_export.json"), "JSON (*.json)"
     )[0]
```

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/cross.png` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/cross.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/gear.png` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/gear.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/horizontal-align.png` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/horizontal-align.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/icons/warning_icon_button.png` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/icons/warning_icon_button.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/logo.png` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/logo.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/main.ui` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/main.ui`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/mock_streamdeck.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/mock_streamdeck.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/model.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/model.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/fonts.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/fonts.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/keyboard.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/keyboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import time
-from typing import List
+from typing import Dict, List, Union
 
 from evdev import InputDevice, UInput
 from evdev import ecodes as e
 from evdev import list_devices
-from PySide6.QtCore import QStringListModel
+from PySide6.QtCore import QStringListModel, QThread
 from PySide6.QtWidgets import QCompleter
 
 _DEFAULT_KEY_PRESS_DELAY = 0.05
 _DEFAULT_KEY_SECTION_DELAY = 0.5
 
+# As far as I know all the key syms in linux are integers below 1000
+# use 2000 or above to signify a delay, and add the delay in deciseconds to this keysym value
+# For example, if you would like a delay of 5 seconds --> 50 deciseconds, then the keysym would be 2050
+_DELAY_KEYSYM = 2000
+# Default delay to add when user uses delay keyword in deciseconds (1/10th of a second)
+_DEFAULT_ADDITIONAL_DELAY = 5
+
 # fmt: off
-_SPECIAL_KEYS = {
+_SPECIAL_KEYS: Dict[str, str] = {
     "plus": "+",
-    "comma": ","
+    "comma": ",",
+    "delay": "delay",
 }
-_OLD_NUMPAD_KEYS = {
+_OLD_NUMPAD_KEYS: Dict[str, int] = {
     "numpad_0": e.KEY_KP0,
     "numpad_1": e.KEY_KP1,
     "numpad_2": e.KEY_KP2,
     "numpad_3": e.KEY_KP3,
     "numpad_4": e.KEY_KP4,
     "numpad_5": e.KEY_KP5,
     "numpad_6": e.KEY_KP6,
@@ -29,40 +37,40 @@
     "numpad_enter": e.KEY_ENTER,
     "numpad_decimal": e.KEY_KPDOT,
     "numpad_divide": e.KEY_KPSLASH,
     "numpad_multiply": e.KEY_KPASTERISK,
     "numpad_subtract": e.KEY_KPMINUS,
     "numpad_add": e.KEY_KPPLUS,
 }
-_OLD_PYNPUT_KEYS = {
+_OLD_PYNPUT_KEYS: Dict[str, int] = {
     "media_volume_mute": e.KEY_MUTE,
     "media_volume_down": e.KEY_VOLUMEDOWN,
     "media_volume_up": e.KEY_VOLUMEUP,
     "media_play_pause": e.KEY_PLAYPAUSE,
     "media_previous_track": e.KEY_PREVIOUSSONG,
     "media_previous": e.KEY_PREVIOUSSONG,
     "media_next_track": e.KEY_NEXTSONG,
     "media_next": e.KEY_NEXTSONG,
     "media_stop": e.KEY_STOPCD,
     "num_lock": e.KEY_NUMLOCK,
     "caps_lock": e.KEY_CAPSLOCK,
     "scroll_lock": e.KEY_SCROLLLOCK,
 }
-_MODIFIER_KEYS = {
+_MODIFIER_KEYS: Dict[str, int] = {
     "ctrl": e.KEY_LEFTCTRL,
     "alt": e.KEY_LEFTALT,
     "alt_gr": e.KEY_RIGHTALT,
     "shift": e.KEY_LEFTSHIFT,
     "meta": e.KEY_LEFTMETA,
     "super": e.KEY_LEFTMETA,
     "win": e.KEY_LEFTMETA,
 }
 
 _BAD_ECODES = ['KEY_MAX', 'KEY_CNT']
-_KEY_MAPPING = {
+_KEY_MAPPING: Dict[str, int] = {
     'a': e.KEY_A,
     'b': e.KEY_B,
     'c': e.KEY_C,
     'd': e.KEY_D,
     'e': e.KEY_E,
     'f': e.KEY_F,
     'g': e.KEY_G,
@@ -153,15 +161,15 @@
     ':': e.KEY_SEMICOLON,
     '"': e.KEY_APOSTROPHE,
     '<': e.KEY_COMMA,
     '>': e.KEY_DOT,
     '?': e.KEY_SLASH,
     '~': e.KEY_GRAVE,
 }
-_SHIFT_KEY_MAPPING = {
+_SHIFT_KEY_MAPPING: Dict[str, int] = {
     '!': e.KEY_1,
     '@': e.KEY_2,
     '#': e.KEY_3,
     '$': e.KEY_4,
     '%': e.KEY_5,
     '^': e.KEY_6,
     '&': e.KEY_7,
@@ -224,46 +232,69 @@
             self.device = UInput({e.EV_KEY: _SUPPORTED_KEY_CONSTANTS})
             self.initialized = True
 
 
 _UINPUT = UInputWrapper()
 
 
-def parse_keys_as_keycodes(keys: str) -> List[List[str]]:
+def parse_delay(key: Union[str, int]) -> Union[str, int]:
+    if isinstance(key, int) or not key.startswith("delay"):
+        return key
+    key = key.replace("delay", "")
+    if len(key) == 0:
+        return _DELAY_KEYSYM + _DEFAULT_ADDITIONAL_DELAY
+    delay = _DEFAULT_ADDITIONAL_DELAY
+    try:
+        delay = int(float(key) * 10)
+    except ValueError:
+        print("Cannot parse delay amount, using default delay")
+    return _DELAY_KEYSYM + delay
+
+
+def parse_keys(
+        key: Union[str, int], key_type: Union[Dict[str, int], Dict[str, str]]) -> Union[str, int]:  # fmt: skip
+    if isinstance(key, int):
+        return key
+    return key_type.get(key, key)
+
+
+def parse_keys_as_keycodes(keys: str) -> List[List[Union[str, int]]]:
     stripped = keys.strip().replace(" ", "").lower()
     if not stripped:
         return []
     # split by , for sections
     sections = stripped.split(",")
     parsed_keys = []
     for section in sections:
         # split by + for individual keys
         individual = section.split("+")
         # filter empty strings
         individual = list(filter(None, individual))
         # replace any string with e.KEY_<string>
         individual = [getattr(e, f"KEY_{key.upper()}", key) for key in individual]
+        # check if delay
+        parsed: List[Union[str, int]] = [parse_delay(key) for key in individual]
         # replace special keys
-        individual = [_SPECIAL_KEYS.get(key, key) for key in individual]
+        parsed = [parse_keys(key, _SPECIAL_KEYS) for key in parsed]
         # replace old numpad keys
-        individual = [_OLD_NUMPAD_KEYS.get(key, key) for key in individual]
+        parsed = [parse_keys(key, _OLD_NUMPAD_KEYS) for key in parsed]
         # replace old media keys
-        individual = [_OLD_PYNPUT_KEYS.get(key, key) for key in individual]
+        parsed = [parse_keys(key, _OLD_PYNPUT_KEYS) for key in parsed]
         # replace modifier keys
-        individual = [_MODIFIER_KEYS.get(key, key) for key in individual]
+        parsed = [parse_keys(key, _MODIFIER_KEYS) for key in parsed]
         # replace key names with key codes
-        individual = [_KEY_MAPPING.get(key, key) for key in individual]
+        parsed = [parse_keys(key, _KEY_MAPPING) for key in parsed]
 
         # if any value is not an int, raise an error
-        if not all(isinstance(key, int) for key in individual):
-            invalid_keys = [key for key in individual if not isinstance(key, int)]
+        if not all(isinstance(key, int) for key in parsed):
+            invalid_keys = [key for key in parsed if not isinstance(key, int)]
             raise ValueError(f"Invalid keys: {invalid_keys}")
 
-        if len(individual) > 0:
-            parsed_keys.append(individual)
+        if len(parsed) > 0:
+            parsed_keys.append(parsed)
 
     return parsed_keys
 
 
 def keyboard_write(string: str):
     _UINPUT.initialize()
     _ui = _UINPUT.device
@@ -321,31 +352,57 @@
 
             # send keys
             _ui.syn()
         else:
             print(f"Unsupported character: {char}")
 
 
-def keyboard_press_keys(keys: str):
-    _UINPUT.initialize()
-    _ui = _UINPUT.device
-    sections = parse_keys_as_keycodes(keys)
-    for section_of_keycodes in sections:
-        for keycode in section_of_keycodes:
-            _ui.write(e.EV_KEY, keycode, 1)
-            _ui.syn()
-        time.sleep(_DEFAULT_KEY_PRESS_DELAY)
+_PRESS_KEY_THREADS: List[QThread] = []
 
-        for keycode in reversed(section_of_keycodes):
-            _ui.write(e.EV_KEY, keycode, 0)
-            _ui.syn()
 
-        # add some delay between sections, only if there are more than one
-        if len(section_of_keycodes) > 1:
-            time.sleep(_DEFAULT_KEY_SECTION_DELAY)
+class KeyboardThread(QThread):
+    def __init__(self, keys):
+        super().__init__()
+        self.keys = keys
+
+    def run(self):
+        _UINPUT.initialize()
+        _ui = _UINPUT.device
+        sections = parse_keys_as_keycodes(self.keys)
+        for section_of_keycodes in sections:
+            for keycode in section_of_keycodes:
+                if keycode > _DELAY_KEYSYM:
+                    # if it is a delay, subtract the delay keysym from the keycode to get the delay in seconds
+                    time.sleep((keycode - _DELAY_KEYSYM) / 10.0)
+                    continue
+                _ui.write(e.EV_KEY, keycode, 1)
+                _ui.syn()
+            time.sleep(_DEFAULT_KEY_PRESS_DELAY)
+
+            for keycode in reversed(section_of_keycodes):
+                _ui.write(e.EV_KEY, keycode, 0)
+                _ui.syn()
+
+            # add some delay between sections, only if there are more than one
+            if len(section_of_keycodes) > 1:
+                time.sleep(_DEFAULT_KEY_SECTION_DELAY)
+
+
+def cleanup_keyboard_thread():
+    global _PRESS_KEY_THREADS
+    # Remove threads that are not running anymore
+    _PRESS_KEY_THREADS = [t for t in _PRESS_KEY_THREADS if t.isRunning()]
+
+
+def keyboard_press_keys(keys: str):
+    global _PRESS_KEY_THREADS
+    thread = KeyboardThread(keys)
+    thread.finished.connect(cleanup_keyboard_thread)
+    _PRESS_KEY_THREADS.append(thread)
+    thread.start()
 
 
 def get_valid_key_names() -> List[str]:
     """Returns a list of valid key names."""
     key_names = [key for key in _SUPPORTED_KEYS]
     key_names.extend(_SPECIAL_KEYS.keys())
     key_names.extend(_OLD_NUMPAD_KEYS.keys())
```

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/modules/utils/timers.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/modules/utils/timers.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/resources_rc.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/semaphore.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/semaphore.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/settings.ui` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/settings.ui`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/stream_deck_monitor.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/stream_deck_monitor.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_button.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_button.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_main.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_main.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/streamdeck_ui/ui_settings.py` & `streamdeck_linux_gui-4.1.2/streamdeck_ui/ui_settings.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-4.1.1/PKG-INFO` & `streamdeck_linux_gui-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck-linux-gui
-Version: 4.1.1
+Version: 4.1.2
 Summary: A service, Web Interface, and UI for interacting with your computer using a Stream Deck
 License: MIT
 Author: Timothy Crosley
 Author-email: timothy.crosley@gmail.com
 Maintainer: 4s3ti
 Maintainer-email: 4s3ti@4s3ti.net
 Requires-Python: >=3.8,<3.13
```

