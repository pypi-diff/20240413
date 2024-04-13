# Comparing `tmp/snake_environment-0.2.4.tar.gz` & `tmp/snake_environment-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.2.4.tar", last modified: Sat Apr 13 12:33:46 2024, max compression
+gzip compressed data, was "snake_environment-0.2.6.tar", last modified: Sat Apr 13 15:03:22 2024, max compression
```

## Comparing `snake_environment-0.2.4.tar` & `snake_environment-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.398669 snake_environment-0.2.4/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2695 2024-04-13 12:33:46.397621 snake_environment-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2024-04-12 18:33:25.000000 snake_environment-0.2.4/README.md
--rw-rw-rw-   0        0        0      708 2024-04-13 12:33:34.000000 snake_environment-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 12:33:46.398669 snake_environment-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.366885 snake_environment-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.374660 snake_environment-0.2.4/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.4/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.391014 snake_environment-0.2.4/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.4/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.4/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     7668 2024-04-12 18:55:57.000000 snake_environment-0.2.4/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.394346 snake_environment-0.2.4/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.4/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.2.4/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 12:33:46.396584 snake_environment-0.2.4/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     2695 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 12:33:46.000000 snake_environment-0.2.4/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.546658 snake_environment-0.2.6/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:03:22.545323 snake_environment-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2029 2024-04-13 12:35:06.000000 snake_environment-0.2.6/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-13 15:03:00.000000 snake_environment-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:03:22.548164 snake_environment-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.518204 snake_environment-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.526313 snake_environment-0.2.6/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.2.6/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.537923 snake_environment-0.2.6/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.2.6/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.2.6/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     7818 2024-04-13 15:02:11.000000 snake_environment-0.2.6/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.541334 snake_environment-0.2.6/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.2.6/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      763 2024-04-13 12:31:15.000000 snake_environment-0.2.6/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:03:22.544331 snake_environment-0.2.6/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     2652 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 15:03:22.000000 snake_environment-0.2.6/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.2.4/LICENSE` & `snake_environment-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.4/PKG-INFO` & `snake_environment-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.4
+Version: 0.2.6
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,40 +17,40 @@
 # Snake Environment
 
 The Snake Environment is a Python package designed for training machine learning models using reinforcement learning techniques. This environment mimics the OpenAI Gym interface, providing a familiar setup for those who are accustomed to using Gym for developing and testing AI models.
 
 ## Features
 
 - **Game Environment**: Built using Pygame, this environment allows for on-screen rendering of the snake game, which is useful for visual feedback while training models.
-- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (done, reward, score, state), similar to environments found in OpenAI Gym.
+- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (state, done, reward, score), similar to environments found in OpenAI Gym.
 - **State Representation**: The state is represented as a numpy array with 18 dimensions, providing comprehensive information about the game environment at any given step.
 - **Utility Methods**: Includes `reset` and `state_dimensions` methods for resetting the game state and retrieving the dimensions of the state space, respectively.
 
 ## Installation
 
 To install the Snake Environment, you can use pip:
 
 ```bash
 pip install snake_environment
 ```
 
-## Usage
+## Example Usage
 ```python
 from snake_environment import SnakeGame
 
 # Initialize the environment
 env = SnakeGame(render=True)  # Set render=False if you do not need to visualize the training process
 
 # Start a new episode
 state = env.reset()
 
 # Loop until the episode is finished
 done = False
 while not done:
-    action = model.predict(state)  # Replace this with your model's prediction method
+    action = model.predict(state) 
     next_state, done, reward, score = env.step(action)
     state = next_state
 
 # Get the dimensions of the state for input layer configuration or debugging
 state_dim = env.state_dimensions
 print("State dimensions:", state_dim)
```

### Comparing `snake_environment-0.2.4/README.md` & `snake_environment-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # Snake Environment
 
 The Snake Environment is a Python package designed for training machine learning models using reinforcement learning techniques. This environment mimics the OpenAI Gym interface, providing a familiar setup for those who are accustomed to using Gym for developing and testing AI models.
 
 ## Features
 
 - **Game Environment**: Built using Pygame, this environment allows for on-screen rendering of the snake game, which is useful for visual feedback while training models.
-- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (done, reward, score, state), similar to environments found in OpenAI Gym.
+- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (state, done, reward, score), similar to environments found in OpenAI Gym.
 - **State Representation**: The state is represented as a numpy array with 18 dimensions, providing comprehensive information about the game environment at any given step.
 - **Utility Methods**: Includes `reset` and `state_dimensions` methods for resetting the game state and retrieving the dimensions of the state space, respectively.
 
 ## Installation
 
 To install the Snake Environment, you can use pip:
 
 ```bash
 pip install snake_environment
 ```
 
-## Usage
+## Example Usage
 ```python
 from snake_environment import SnakeGame
 
 # Initialize the environment
 env = SnakeGame(render=True)  # Set render=False if you do not need to visualize the training process
 
 # Start a new episode
 state = env.reset()
 
 # Loop until the episode is finished
 done = False
 while not done:
-    action = model.predict(state)  # Replace this with your model's prediction method
+    action = model.predict(state) 
     next_state, done, reward, score = env.step(action)
     state = next_state
 
 # Get the dimensions of the state for input layer configuration or debugging
 state_dim = env.state_dimensions
 print("State dimensions:", state_dim)
 
 ```
 
 ## Contributions
 Contributions are welcome! If you'd like to improve the Snake Environment, please fork this repository and submit a pull request with your proposed changes.
 
 ## License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `snake_environment-0.2.4/pyproject.toml` & `snake_environment-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.2.4"
+version = "0.2.6"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.2.4/src/snake_environment/game/objects.py` & `snake_environment-0.2.6/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.4/src/snake_environment/game/snake_game.py` & `snake_environment-0.2.6/src/snake_environment/game/snake_game.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
         snake_start_y = WINDOW_HEIGHT // 2
 
         self.snake = Snake(snake_start_x, snake_start_y)
         food_start_x, food_start_y = self.get_random_position()
         self.food = Food(food_start_x, food_start_y)
 
         self.score = 0
+        self.num_frames = 0
         return self.get_game_state()
 
+
     def get_random_position(self):
         x = random.randrange(0, WINDOW_WIDTH // self.snake.size) * self.snake.size
         y = random.randrange(0, WINDOW_HEIGHT // self.snake.size) * self.snake.size
         return x, y
 
     def step(self, action):
         """
@@ -73,14 +75,18 @@
 
         if food_eaten:  # If food was eaten
             self.respawn_food()  # Respawn food at a new location
 
         if self.render:  # If rendering is enabled
             self.update_ui()  # Update the game UI
 
+        if self.num_frames % len(self.snake.body)*1000 == 0:
+            done = True
+
+        self.num_frames += 1
         return state, done, reward, self.score  # Return the step result
 
     def update_ui(self):
         self.screen.fill((0, 0, 0))
 
         # drawing snake
```

### Comparing `snake_environment-0.2.4/src/snake_environment/helpers/helpers.py` & `snake_environment-0.2.6/src/snake_environment/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.2.4/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.2.6/src/snake_environment.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.2.4
+Version: 0.2.6
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,40 +17,40 @@
 # Snake Environment
 
 The Snake Environment is a Python package designed for training machine learning models using reinforcement learning techniques. This environment mimics the OpenAI Gym interface, providing a familiar setup for those who are accustomed to using Gym for developing and testing AI models.
 
 ## Features
 
 - **Game Environment**: Built using Pygame, this environment allows for on-screen rendering of the snake game, which is useful for visual feedback while training models.
-- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (done, reward, score, state), similar to environments found in OpenAI Gym.
+- **Compatibility with AI Training Workflows**: The `SnakeGame` class features a `step` function that returns a tuple of (state, done, reward, score), similar to environments found in OpenAI Gym.
 - **State Representation**: The state is represented as a numpy array with 18 dimensions, providing comprehensive information about the game environment at any given step.
 - **Utility Methods**: Includes `reset` and `state_dimensions` methods for resetting the game state and retrieving the dimensions of the state space, respectively.
 
 ## Installation
 
 To install the Snake Environment, you can use pip:
 
 ```bash
 pip install snake_environment
 ```
 
-## Usage
+## Example Usage
 ```python
 from snake_environment import SnakeGame
 
 # Initialize the environment
 env = SnakeGame(render=True)  # Set render=False if you do not need to visualize the training process
 
 # Start a new episode
 state = env.reset()
 
 # Loop until the episode is finished
 done = False
 while not done:
-    action = model.predict(state)  # Replace this with your model's prediction method
+    action = model.predict(state) 
     next_state, done, reward, score = env.step(action)
     state = next_state
 
 # Get the dimensions of the state for input layer configuration or debugging
 state_dim = env.state_dimensions
 print("State dimensions:", state_dim)
```

