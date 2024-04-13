# Comparing `tmp/snake_environment-0.2.tar.gz` & `tmp/snake_environment-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.2.tar", last modified: Fri Apr 12 18:16:13 2024, max compression
+gzip compressed data, was "snake_environment-0.2.2.tar", last modified: Fri Apr 12 18:35:25 2024, max compression
```

## Comparing `snake_environment-0.2.tar` & `snake_environment-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.309620 snake_environment-0.2/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2/LICENSE
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:16:13.309620 snake_environment-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-12 17:25:27.000000 snake_environment-0.2/README.md
--rw-rw-rw-   0        0        0      708 2024-04-12 18:15:31.000000 snake_environment-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 18:16:13.309620 snake_environment-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.294069 snake_environment-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.297392 snake_environment-0.2/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.305855 snake_environment-0.2/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     6681 2024-04-12 18:15:21.000000 snake_environment-0.2/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.308293 snake_environment-0.2/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      763 2024-04-12 18:11:57.000000 snake_environment-0.2/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:16:13.308293 snake_environment-0.2/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:16:13.000000 snake_environment-0.2/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-12 18:16:13.000000 snake_environment-0.2/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:16:13.000000 snake_environment-0.2/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 18:16:13.000000 snake_environment-0.2/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 18:16:13.000000 snake_environment-0.2/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.470678 snake_environment-0.2.2/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2695 2024-04-12 18:35:25.470678 snake_environment-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2024-04-12 18:33:25.000000 snake_environment-0.2.2/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-12 18:34:58.000000 snake_environment-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:35:25.470678 snake_environment-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.458447 snake_environment-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.461733 snake_environment-0.2.2/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.2/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.467987 snake_environment-0.2.2/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.2/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.2/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     6681 2024-04-12 18:31:06.000000 snake_environment-0.2.2/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.469027 snake_environment-0.2.2/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.2/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      763 2024-04-12 18:11:57.000000 snake_environment-0.2.2/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.470174 snake_environment-0.2.2/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     2695 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.2/LICENSE` & `snake_environment-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2/pyproject.toml` & `snake_environment-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.2.0"
+version = "0.2.2"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.2/src/snake_environment/game/objects.py` & `snake_environment-0.2.2/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2/src/snake_environment/game/snake_game.py` & `snake_environment-0.2.2/src/snake_environment/game/snake_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         if food_eaten:  # If food was eaten
             self.respawn_food()  # Respawn food at a new location
 
         if self.render:  # If rendering is enabled
             self.update_ui()  # Update the game UI
 
-        return done, reward, self.score, state  # Return the step result
+        return state, done, reward, self.score  # Return the step result
 
     def update_ui(self):
         self.screen.fill((0, 0, 0))
 
         # drawing snake
 
         for segment in self.snake.body:
```

### Comparing `snake_environment-0.2/src/snake_environment/helpers/helpers.py` & `snake_environment-0.2.2/src/snake_environment/helpers/helpers.py`

 * *Files identical despite different names*

