# Comparing `tmp/snake_environment-0.2.2.tar.gz` & `tmp/snake_environment-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.2.2.tar", last modified: Fri Apr 12 18:35:25 2024, max compression
+gzip compressed data, was "snake_environment-0.2.4.tar", last modified: Sat Apr 13 12:33:46 2024, max compression
```

## Comparing `snake_environment-0.2.2.tar` & `snake_environment-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.470678 snake_environment-0.2.2/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2695 2024-04-12 18:35:25.470678 snake_environment-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2024-04-12 18:33:25.000000 snake_environment-0.2.2/README.md
--rw-rw-rw-   0        0        0      708 2024-04-12 18:34:58.000000 snake_environment-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 18:35:25.470678 snake_environment-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.458447 snake_environment-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.461733 snake_environment-0.2.2/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.2/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.467987 snake_environment-0.2.2/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.2/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.2/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     6681 2024-04-12 18:31:06.000000 snake_environment-0.2.2/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.469027 snake_environment-0.2.2/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.2/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      763 2024-04-12 18:11:57.000000 snake_environment-0.2.2/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:35:25.470174 snake_environment-0.2.2/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     2695 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 18:35:25.000000 snake_environment-0.2.2/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.398669 snake_environment-0.2.4/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2695 2024-04-13 12:33:46.397621 snake_environment-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2024-04-12 18:33:25.000000 snake_environment-0.2.4/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-13 12:33:34.000000 snake_environment-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 12:33:46.398669 snake_environment-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.366885 snake_environment-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.374660 snake_environment-0.2.4/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.4/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.391014 snake_environment-0.2.4/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.4/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.4/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     7668 2024-04-12 18:55:57.000000 snake_environment-0.2.4/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.394346 snake_environment-0.2.4/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.4/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.2.4/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.396584 snake_environment-0.2.4/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     2695 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.2.2/LICENSE` & `snake_environment-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.2/PKG-INFO` & `snake_environment-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.2
+Version: 0.2.4
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snake_environment-0.2.2/README.md` & `snake_environment-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.2/pyproject.toml` & `snake_environment-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.2.2"
+version = "0.2.4"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.2.2/src/snake_environment/game/objects.py` & `snake_environment-0.2.4/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.2/src/snake_environment/game/snake_game.py` & `snake_environment-0.2.4/src/snake_environment/game/snake_game.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,14 +118,29 @@
 
         return False
 
     def respawn_food(self):
         self.food.x, self.food.y = self.get_random_position()
 
     def get_game_state(self):
+        """
+        Generates the current game state as a numpy array, which includes information about the direction and distance of dangers,
+        the normalized distance to the food, and the normalized angle to the food. This state representation is used as input for
+        decision-making algorithms (e.g., neural networks in reinforcement learning).
+
+        The state includes:
+        - Danger indicators for each of the four directions (right, left, up, down) up to 4 steps away.
+        - The normalized Euclidean distance between the snake's head and the food.
+        - The normalized angle from the snake's head to the food, where 0 represents directly to the right, and values increase
+          counterclockwise.
+
+        Returns:
+            np.array: A numpy array representing the current state of the game, which includes danger indicators, distance to food,
+                      and angle to food, all normalized to be between 0 and 1.
+        """
         head = self.snake.body[0]
         size = self.snake.size
         directions = {
             'right': (size, 0),
             'left': (-size, 0),
             'up': (0, -size),
             'down': (0, size)
```

### Comparing `snake_environment-0.2.2/src/snake_environment/helpers/helpers.py` & `snake_environment-0.2.4/src/snake_environment/helpers/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 if event.key == pygame.K_DOWN:
                     action = 1
                 if event.key == pygame.K_LEFT:
                     action = 2
                 if event.key == pygame.K_UP:
                     action = 3
 
-        done, reward, score, next_state = game.step(action)
+        next_state, done, reward, score = game.step(action)
```

### Comparing `snake_environment-0.2.2/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.2.4/src/snake_environment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.2
+Version: 0.2.4
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

