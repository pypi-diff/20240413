# Comparing `tmp/snake_environment-0.3.0.tar.gz` & `tmp/snake_environment-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.3.0.tar", last modified: Sat Apr 13 15:13:45 2024, max compression
+gzip compressed data, was "snake_environment-0.3.3.tar", last modified: Sat Apr 13 15:17:02 2024, max compression
```

## Comparing `snake_environment-0.3.0.tar` & `snake_environment-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.620955 snake_environment-0.3.0/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     2652 2024-04-13 15:13:45.619797 snake_environment-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2029 2024-04-13 12:35:06.000000 snake_environment-0.3.0/README.md
--rw-rw-rw-   0        0        0      708 2024-04-13 15:13:34.000000 snake_environment-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 15:13:45.620955 snake_environment-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.594419 snake_environment-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.601118 snake_environment-0.3.0/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.3.0/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.614374 snake_environment-0.3.0/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.3.0/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.3.0/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     7886 2024-04-13 15:13:09.000000 snake_environment-0.3.0/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.616696 snake_environment-0.3.0/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.3.0/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.3.0/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:13:45.618487 snake_environment-0.3.0/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     2652 2024-04-13 15:13:45.000000 snake_environment-0.3.0/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-13 15:13:45.000000 snake_environment-0.3.0/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 15:13:45.000000 snake_environment-0.3.0/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 15:13:45.000000 snake_environment-0.3.0/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 15:13:45.000000 snake_environment-0.3.0/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.888909 snake_environment-0.3.3/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:17:02.887911 snake_environment-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2029 2024-04-13 12:35:06.000000 snake_environment-0.3.3/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-13 15:16:53.000000 snake_environment-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:17:02.888909 snake_environment-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.864340 snake_environment-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.871107 snake_environment-0.3.3/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.3.3/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.881624 snake_environment-0.3.3/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.3.3/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.3.3/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     7881 2024-04-13 15:16:28.000000 snake_environment-0.3.3/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.884391 snake_environment-0.3.3/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.3.3/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      814 2024-04-13 15:15:53.000000 snake_environment-0.3.3/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:17:02.886907 snake_environment-0.3.3/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:17:02.000000 snake_environment-0.3.3/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-13 15:17:02.000000 snake_environment-0.3.3/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:17:02.000000 snake_environment-0.3.3/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 15:17:02.000000 snake_environment-0.3.3/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 15:17:02.000000 snake_environment-0.3.3/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.3.0/LICENSE` & `snake_environment-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.3.0/PKG-INFO` & `snake_environment-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.3.0
+Version: 0.3.3
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snake_environment-0.3.0/README.md` & `snake_environment-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `snake_environment-0.3.0/pyproject.toml` & `snake_environment-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.3.0"
+version = "0.3.3"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.3.0/src/snake_environment/game/objects.py` & `snake_environment-0.3.3/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.3.0/src/snake_environment/game/snake_game.py` & `snake_environment-0.3.3/src/snake_environment/game/snake_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         if food_eaten:  # If food was eaten
             self.respawn_food()  # Respawn food at a new location
 
         if self.render:  # If rendering is enabled
             self.update_ui()  # Update the game UI
 
-        if self.num_frames > len(self.snake.body)*self.max_frames == 0:
+        if self.num_frames > len(self.snake.body)*self.max_frames:
             done = True
 
         return state, done, reward, self.score  # Return the step result
 
     def update_ui(self):
         self.screen.fill((0, 0, 0))
```

### Comparing `snake_environment-0.3.0/src/snake_environment/helpers/helpers.py` & `snake_environment-0.3.3/src/snake_environment/helpers/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,7 +21,9 @@
                     action = 1
                 if event.key == pygame.K_LEFT:
                     action = 2
                 if event.key == pygame.K_UP:
                     action = 3
 
         next_state, done, reward, score = game.step(action)
+
+    print(f'Played for {game.num_frames} frames')
```

### Comparing `snake_environment-0.3.0/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.3.3/src/snake_environment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.3.0
+Version: 0.3.3
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

