# Comparing `tmp/snake_environment-0.2.6.tar.gz` & `tmp/snake_environment-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.2.6.tar", last modified: Sat Apr 13 15:03:22 2024, max compression
+gzip compressed data, was "snake_environment-0.2.8.tar", last modified: Sat Apr 13 15:11:12 2024, max compression
```

## Comparing `snake_environment-0.2.6.tar` & `snake_environment-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.546658 snake_environment-0.2.6/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2652 2024-04-13 15:03:22.545323 snake_environment-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2029 2024-04-13 12:35:06.000000 snake_environment-0.2.6/README.md
--rw-rw-rw-   0        0        0      708 2024-04-13 15:03:00.000000 snake_environment-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 15:03:22.548164 snake_environment-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.518204 snake_environment-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.526313 snake_environment-0.2.6/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.6/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.537923 snake_environment-0.2.6/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.6/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.6/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     7818 2024-04-13 15:02:11.000000 snake_environment-0.2.6/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.541334 snake_environment-0.2.6/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.6/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.2.6/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.544331 snake_environment-0.2.6/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     2652 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.727959 snake_environment-0.2.8/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:11:12.726962 snake_environment-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2029 2024-04-13 12:35:06.000000 snake_environment-0.2.8/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-13 15:10:35.000000 snake_environment-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:11:12.729113 snake_environment-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.696168 snake_environment-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.704628 snake_environment-0.2.8/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.8/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.720978 snake_environment-0.2.8/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.8/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.8/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     7886 2024-04-13 15:10:25.000000 snake_environment-0.2.8/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.723970 snake_environment-0.2.8/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.8/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.2.8/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:11:12.725965 snake_environment-0.2.8/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:11:12.000000 snake_environment-0.2.8/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-13 15:11:12.000000 snake_environment-0.2.8/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:11:12.000000 snake_environment-0.2.8/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 15:11:12.000000 snake_environment-0.2.8/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 15:11:12.000000 snake_environment-0.2.8/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.2.6/LICENSE` & `snake_environment-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.6/PKG-INFO` & `snake_environment-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.6
+Version: 0.2.8
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snake_environment-0.2.6/README.md` & `snake_environment-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.6/pyproject.toml` & `snake_environment-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.2.6"
+version = "0.2.8"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.2.6/src/snake_environment/game/objects.py` & `snake_environment-0.2.8/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.6/src/snake_environment/game/snake_game.py` & `snake_environment-0.2.8/src/snake_environment/game/snake_game.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from .objects import Snake, Food
 
 WINDOW_WIDTH = 800
 WINDOW_HEIGHT = 600
 
 
 class SnakeGame:
-    def __init__(self, render=False):
+    def __init__(self, render=False, max_frames=1000):
         self.render = render
         if self.render:
             pygame.init()
             pygame.font.init()
             self.screen = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
             pygame.display.set_caption("Snake Game")
             self.clock = pygame.time.Clock()
             self.font = pygame.font.Font(None, 30)
 
         self.reset()
+        self.max_frames = max_frames
         self.state_dimensions = len(self.get_game_state())
 
     def reset(self):
         snake_start_x = WINDOW_WIDTH // 2
         snake_start_y = WINDOW_HEIGHT // 2
 
         self.snake = Snake(snake_start_x, snake_start_y)
@@ -48,14 +49,16 @@
 
         Returns:
         - done: A boolean indicating whether the game is over (True if the game is over, otherwise False).
         - reward: An integer representing the reward obtained in this step. Eating food gives a positive reward, hitting a wall or itself gives a negative reward.
         - self.score: The current score of the game.
         - state: The current state of the game, represented as a numpy array.
         """
+        self.num_frames += 1
+
         done = False
         self.snake.change_direction(action)  # Change the direction of the snake based on the action
         self.snake.move()  # Move the snake in the new direction
 
         head = self.snake.body[0]  # Get the new head position after moving
         food_eaten = (head[0] == self.food.x and head[1] == self.food.y)  # Check if the snake has eaten the food
 
@@ -75,18 +78,17 @@
 
         if food_eaten:  # If food was eaten
             self.respawn_food()  # Respawn food at a new location
 
         if self.render:  # If rendering is enabled
             self.update_ui()  # Update the game UI
 
-        if self.num_frames % len(self.snake.body)*1000 == 0:
+        if self.num_frames % len(self.snake.body)*self.max_frames == 0:
             done = True
 
-        self.num_frames += 1
         return state, done, reward, self.score  # Return the step result
 
     def update_ui(self):
         self.screen.fill((0, 0, 0))
 
         # drawing snake
```

### Comparing `snake_environment-0.2.6/src/snake_environment/helpers/helpers.py` & `snake_environment-0.2.8/src/snake_environment/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.6/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.2.8/src/snake_environment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.6
+Version: 0.2.8
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

