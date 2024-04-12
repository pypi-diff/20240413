# Comparing `tmp/kesslergame-2.1.1.tar.gz` & `tmp/KesslerGame-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kesslergame-2.1.1.tar", last modified: Tue Mar 12 18:10:21 2024, max compression
+gzip compressed data, was "KesslerGame-2.1.2.tar", last modified: Fri Apr 12 22:42:52 2024, max compression
```

## Comparing `kesslergame-2.1.1.tar` & `KesslerGame-2.1.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.033077 kesslergame-2.1.1/
--rw-rw-rw-   0        0        0    11565 2024-03-12 18:09:48.000000 kesslergame-2.1.1/LICENSE
--rw-rw-rw-   0        0        0       73 2024-03-12 18:09:48.000000 kesslergame-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3331 2024-03-12 18:10:21.033077 kesslergame-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2024-03-12 18:09:48.000000 kesslergame-2.1.1/README.md
--rw-rw-rw-   0        0        0      423 2024-03-12 18:09:48.000000 kesslergame-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       23 2024-03-12 18:09:48.000000 kesslergame-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0      882 2024-03-12 18:10:21.033077 kesslergame-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      369 2024-03-12 18:09:48.000000 kesslergame-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.001832 kesslergame-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.017454 kesslergame-2.1.1/src/kesslergame/
--rw-rw-rw-   0        0        0      681 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/asteroid.py
--rw-rw-rw-   0        0        0     1565 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/bullet.py
--rw-rw-rw-   0        0        0     1377 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/collisions.py
--rw-rw-rw-   0        0        0     1426 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/controller.py
--rw-rw-rw-   0        0        0     5949 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/controller_gamepad.py
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.017454 kesslergame-2.1.1/src/kesslergame/graphics/
--rw-rw-rw-   0        0        0      380 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/__init__.py
--rw-rw-rw-   0        0        0      727 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/graphics_base.py
--rw-rw-rw-   0        0        0     2447 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/graphics_handler.py
--rw-rw-rw-   0        0        0     5122 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/graphics_plt.py
--rw-rw-rw-   0        0        0    11977 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/graphics_tk.py
--rw-rw-rw-   0        0        0     3835 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/graphics_ue.py
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.033077 kesslergame-2.1.1/src/kesslergame/graphics/images/
--rw-rw-rw-   0        0        0        0 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/images/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip1_green.png
--rw-rw-rw-   0        0        0     2578 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip1_orange.png
--rw-rw-rw-   0        0        0     3597 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip2_orange.png
--rw-rw-rw-   0        0        0     2725 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip3_orange.png
--rw-rw-rw-   0        0        0    16867 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/kessler_game.py
--rw-rw-rw-   0        0        0     1687 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/mines.py
--rw-rw-rw-   0        0        0     6486 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/scenario.py
--rw-rw-rw-   0        0        0     2285 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/score.py
--rw-rw-rw-   0        0        0    10143 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/ship.py
--rw-rw-rw-   0        0        0     1506 2024-03-12 18:09:48.000000 kesslergame-2.1.1/src/kesslergame/team.py
-drwxrwxrwx   0        0        0        0 2024-03-12 18:10:21.017454 kesslergame-2.1.1/src/kesslergame.egg-info/
--rw-rw-rw-   0        0        0     3331 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-03-12 18:10:20.000000 kesslergame-2.1.1/src/kesslergame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/
+-rw-rw-rw-   0        0        0    11565 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0       73 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3345 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/README.md
+-rw-rw-rw-   0        0        0      477 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      896 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.502638 KesslerGame-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/KesslerGame.egg-info/
+-rw-rw-rw-   0        0        0     3345 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 22:42:52.000000 KesslerGame-2.1.2/src/KesslerGame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/
+-rw-rw-rw-   0        0        0      701 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/_version.py
+-rw-rw-rw-   0        0        0     7086 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/asteroid.py
+-rw-rw-rw-   0        0        0     1886 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/bullet.py
+-rw-rw-rw-   0        0        0     1423 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/collisions.py
+-rw-rw-rw-   0        0        0     1432 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/controller.py
+-rw-rw-rw-   0        0        0     6110 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/controller_gamepad.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/graphics/
+-rw-rw-rw-   0        0        0      380 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_base.py
+-rw-rw-rw-   0        0        0     3034 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_handler.py
+-rw-rw-rw-   0        0        0     5761 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_plt.py
+-rw-rw-rw-   0        0        0    12623 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_tk.py
+-rw-rw-rw-   0        0        0     3912 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/graphics_ue.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:42:52.518264 KesslerGame-2.1.2/src/kesslergame/graphics/images/
+-rw-rw-rw-   0        0        0        0 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_green.png
+-rw-rw-rw-   0        0        0     2578 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_orange.png
+-rw-rw-rw-   0        0        0     3597 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip2_orange.png
+-rw-rw-rw-   0        0        0     2725 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip3_orange.png
+-rw-rw-rw-   0        0        0    17860 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/kessler_game.py
+-rw-rw-rw-   0        0        0     2035 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/mines.py
+-rw-rw-rw-   0        0        0     6571 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/scenario.py
+-rw-rw-rw-   0        0        0     2488 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/score.py
+-rw-rw-rw-   0        0        0    11089 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/ship.py
+-rw-rw-rw-   0        0        0     1881 2024-04-12 22:42:24.000000 KesslerGame-2.1.2/src/kesslergame/team.py
```

### Comparing `kesslergame-2.1.1/LICENSE` & `KesslerGame-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/PKG-INFO` & `KesslerGame-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: kesslergame
-Version: 2.1.1
+Name: KesslerGame
+Version: 2.1.2
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
-Author-email: zachariah.phillips@us.thalesgroup.com
+Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
-Maintainer-email: tim.arnett@psibernetix.com
+Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
 Keywords: artificial intelligence,asteroids,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `kesslergame-2.1.1/README.md` & `KesslerGame-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/src/kesslergame/asteroid.py` & `KesslerGame-2.1.2/src/kesslergame/asteroid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-from typing import Tuple, Dict, List, Any
+from typing import Tuple, Dict, List, Any, Optional, TYPE_CHECKING, Union
 import random
 import math
-from .mines import Mine
 
+if TYPE_CHECKING:
+    from .ship import Ship
+    from .bullet import Bullet
+from .mines import Mine
 
 class Asteroid:
     """ Sprite that represents an asteroid. """
+    __slots__ = ('size', 'max_speed', 'num_children', 'radius', 'mass', 'vx', 'vy', 'velocity', 'position', 'angle', 'turnrate')
     def __init__(self,
-                 position: Tuple[float, float] = None,
-                 speed: float = None,
-                 angle: float = None,
-                 size: float = None):
+                 position: Tuple[float, float],
+                 speed: Optional[float] = None,
+                 angle: Optional[float] = None,
+                 size: Optional[int] = None) -> None:
         """
         Constructor for Asteroid Sprite
 
         :param position:  Optional Starting position (x, y) position
         :param speed: Optional Starting Speed
         :param angle: Optional Starting heading angle (degrees)
         :param size: Optional Starting size (1 to 4 inclusive)
         """
 
         # Set size to 4 if none is specified. Notify if out of size range
         if size:
             if 1 <= size <= 4:
                 self.size = size
             else:
-                raise ValueError("AsteroidSize can only be between 1 and 4")
+                raise ValueError("Asteroid size can only be between 1 and 4")
         else:
             self.size = 4
 
         # Set max speed based off of scaling factor
         speed_scaler = 2.0 + (4.0 - self.size) / 4.0
         self.max_speed = 60.0 * speed_scaler
 
         # Number of child asteroids spawned when this asteroid is destroyed
         self.num_children = 3
 
         # Set collision radius based on size # TODO May need to change once size can be visualized
-        self.radius = self.size * 8
+        self.radius = self.size * 8.0
 
-        self.mass = 0.25*math.pi*self.radius**2
+        self.mass = 0.25*math.pi*self.radius*self.radius
 
         # Use optional angle and speed arguments otherwise generate random angle and speed
         starting_angle = angle if angle is not None else random.random()*360.0
         starting_speed = speed if speed is not None else random.random()*self.max_speed - self.max_speed/2.0
 
         # Set velocity based on starting angle and speed
         # self.velocity = [
         #     -starting_speed * math.sin(math.radians(starting_angle)),
         #     starting_speed * math.cos(math.radians(starting_angle))
         # ]
 
         self.vx = starting_speed*math.cos(math.radians(starting_angle))
         self.vy = starting_speed*math.sin(math.radians(starting_angle))
-        self.velocity = [self.vx, self.vy]
+        self.velocity = (self.vx, self.vy)
 
         # Set position as specified
         self.position = position
 
         # Random rotations for use in display or future use with complex hit box
-        self.angle = random.randint(0, 360)
-        self.turnrate = random.randint(0, 200) - 100
+        self.angle: float = random.uniform(0.0, 360.0)
+        self.turnrate: float = random.uniform(-100, 100)
 
     @property
     def state(self) -> Dict[str, Any]:
         return {
-            "position": tuple(self.position),
-            "velocity": tuple(self.velocity),
-            "size": int(self.size),
-            "mass": float(self.mass),
-            "radius": float(self.radius)
+            "position": self.position,
+            "velocity": self.velocity,
+            "size": self.size,
+            "mass": self.mass,
+            "radius": self.radius
         }
 
-    def update(self, delta_time: float = 1/30):
+    def update(self, delta_time: float = 1/30) -> None:
         """ Move the asteroid based on velocity"""
-        self.position = [pos + v*delta_time for pos, v in zip(self.position, self.velocity)]
+        self.position = (self.position[0] + self.velocity[0] * delta_time, self.position[1] + self.velocity[1] * delta_time)
         self.angle += delta_time * self.turnrate
 
-    def destruct(self, impactor):
+    def destruct(self, impactor: Union['Bullet', 'Mine', 'Ship']) -> list['Asteroid']:
         """ Spawn child asteroids"""
 
         if self.size != 1:
             if isinstance(impactor, Mine):
                 delta_x = impactor.position[0] - self.position[0]
                 delta_y = impactor.position[1] - self.position[1]
                 dist = math.sqrt(delta_x*delta_x + delta_y*delta_y)
@@ -99,25 +103,25 @@
                     vfx = self.vx + a*cos_theta
                     vfy = self.vy + a*sin_theta
 
                     # Calculate speed of resultant asteroid(s) based on velocity vector
                     v = math.sqrt(vfx*vfx + vfy*vfy)
                     # Split angle is the angle off of the new velocity vector for the two asteroids to the sides, the center child
                     # asteroid continues on the new velocity path
-                    split_angle = 15
+                    split_angle = 15.0
                 else:
                     vfx = self.vx
                     vfy = self.vy
                     
                     # Calculate speed of resultant asteroid(s) based on velocity vector
                     # This v calculation matches the speed you would get in the nonzero dist case, if you take the limit as dist -> 0
                     v = math.sqrt(vfx*vfx + vfy*vfy + a*a)
                     # Split angle is the angle off of the new velocity vector for the two asteroids to the sides, the center child
                     # asteroid continues on the new velocity path
-                    split_angle = 120
+                    split_angle = 120.0
             else:
                 # Calculating new velocity vector of asteroid children based on bullet-asteroid collision/momentum
                 # Currently collisions are considered perfectly inelastic i.e. the bullet is absorbed by the asteroid
                 # This assumption doesn't matter much now due to the fact that bullets are "destroyed" by impact with the
                 # asteroid and the bullet mass is significantly smaller than the asteroid. If this changes, these calculations
                 # may need to change
 
@@ -127,15 +131,15 @@
                 vfx = (1/(impactor.mass + self.mass))*(impactor.mass*impactor_vx + self.mass*self.vx)
                 vfy = (1/(impactor.mass + self.mass))*(impactor.mass*impactor_vy + self.mass*self.vy)
 
                 # Calculate speed of resultant asteroid(s) based on velocity vector
                 v = math.sqrt(vfx*vfx + vfy*vfy)
                 # Split angle is the angle off of the new velocity vector for the two asteroids to the sides, the center child
                 # asteroid continues on the new velocity path
-                split_angle = 15
+                split_angle = 15.0
             # Calculate angle of center asteroid for split (degrees)
             theta = math.degrees(math.atan2(vfy, vfx))
             angles = [theta + split_angle, theta, theta - split_angle]
 
             return [Asteroid(position=self.position, size=self.size-1, speed=v, angle=angle) for angle in angles]
 
                 # Old method of doing random splits
```

### Comparing `kesslergame-2.1.1/src/kesslergame/bullet.py` & `KesslerGame-2.1.2/src/kesslergame/bullet.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,39 +2,45 @@
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 from typing import List, Tuple, Dict, Any
 import math
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .ship import Ship
+
 
 class Bullet:
-    def __init__(self, starting_position: List[float], starting_heading: float, owner):
+    __slots__ = ('owner', 'speed', 'length', 'mass', 'position', 'heading', 'rad_heading', 'tail', 'vx', 'vy', 'velocity')
+    def __init__(self, starting_position: Tuple[float, float], starting_heading: float, owner: 'Ship') -> None:
         self.owner = owner
-        self.speed = 800  # m/s
-        self.length = 12
-        self.mass = 1  # mass units - kg?
+        self.speed = 800.0  # m/s
+        self.length = 12.0
+        self.mass = 1.0  # mass units - kg?
         self.position = starting_position
         self.heading = starting_heading
         self.rad_heading = math.radians(starting_heading)
         cos_heading = math.cos(self.rad_heading)
         sin_heading = math.sin(self.rad_heading)
-        self.tail = [self.position[0] - self.length*cos_heading,
-                     self.position[1] - self.length*sin_heading]
+        self.tail = (self.position[0] - self.length*cos_heading,
+                     self.position[1] - self.length*sin_heading)
         self.vx = self.speed*cos_heading
         self.vy = self.speed*sin_heading
         self.velocity = [self.vx, self.vy]
 
-    def update(self, delta_time=1/30):
+    def update(self, delta_time: float = 1/30) -> None:
         # Update the position:
-        self.position = [pos + v * delta_time for pos, v in zip(self.position, self.velocity)]
-        self.tail = [pos + v * delta_time for pos, v in zip(self.tail, self.velocity)]
+        self.position = (self.position[0] + self.velocity[0] * delta_time, self.position[1] + self.velocity[1] * delta_time)
+        self.tail = (self.tail[0] + self.velocity[0] * delta_time, self.tail[1] + self.velocity[1] * delta_time)
 
-    def destruct(self):
-        ...
+    def destruct(self) -> None:
+        pass
 
     @property
     def state(self) -> Dict[str, Any]:
         return {
             "position": tuple(self.position),
             "velocity": tuple(self.velocity),
             "heading": float(self.heading),
```

### Comparing `kesslergame-2.1.1/src/kesslergame/collisions.py` & `KesslerGame-2.1.2/src/kesslergame/collisions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 import math
 
-def circle_line_collision(line_A, line_B, center, radius):
+def circle_line_collision(line_A: tuple[float, float], line_B: tuple[float, float], center: tuple[float, float], radius: float) -> bool:
     # Check if circle edge is within the outer bounds of the line segment (offset for radius)
     # Not 100% accurate (some false positives) but fast and rare inaccuracies
-    x_bounds = [min(line_A[0], line_B[0])-radius, max(line_A[0], line_B[0])+radius]
+    x_bounds = [min(line_A[0], line_B[0]) - radius, max(line_A[0], line_B[0]) + radius]
     if center[0] < x_bounds[0] or center[0] > x_bounds[1]:
         return False
-    y_bounds = [min(line_A[1], line_B[1])-radius, max(line_A[1], line_B[1])+radius]
+    y_bounds = [min(line_A[1], line_B[1]) - radius, max(line_A[1], line_B[1]) + radius]
     if center[1] < y_bounds[0] or center[1] > y_bounds[1]:
         return False
 
     # calculate side lengths of triangle formed from the line segment and circle center point
     a = math.dist(line_A, center)
     b = math.dist(line_B, center)
     c = math.dist(line_A, line_B)
 
     # Heron's formula to calculate area of triangle and resultant height (distance from circle center to line segment)
     s = 0.5 * (a + b + c)
 
-    cen_dist = 2 / c * math.sqrt(max(0.0, s * (s-a) * (s-b) * (s-c)))
+    cen_dist = 2.0 / c * math.sqrt(max(0.0, s * (s-a) * (s-b) * (s-c)))
 
     # If circle distance to line segment is less than circle radius, they are colliding
-    if cen_dist < radius:
-        return True
-    return False
-
-
-
+    return cen_dist < radius
```

### Comparing `kesslergame-2.1.1/src/kesslergame/controller.py` & `KesslerGame-2.1.2/src/kesslergame/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-from typing import Dict, Tuple
-import time
-
-from .ship import Ship
+from typing import Dict, Tuple, Any
 
 
 class KesslerController:
     """
      A ship controller class for Kessler. This can be inherited to create custom controllers that can be passed to the
     game to operate within scenarios. A valid controller contains an actions method that takes in a ship object and ass
     game_state dictionary. This action method then sets the thrust, turn_rate, and fire commands on the ship object.
     """
 
-    def actions(self, ship_state: Dict, game_state: Dict) -> Tuple[float, float, bool, bool]:
+    def actions(self, ship_state: Dict[str, Any], game_state: Dict[str, Any]) -> Tuple[float, float, bool, bool]:
         """
         Method processed each time step by this controller.
         """
 
         raise NotImplementedError('Your derived KesslerController must include an actions method for control input.')
 
 
     # Property to store the ID for the ship this controller is attached to during a scenario
     @property
-    def ship_id(self):
+    def ship_id(self) -> int:
         return self._ship_id if self._ship_id else 0
 
     @ship_id.setter
-    def ship_id(self, value):
+    def ship_id(self, value: int) -> None:
         self._ship_id = value
 
     @property
     def name(self) -> str:
         raise NotImplementedError(f"This controller {self.__class__} needs to have a name() property specified.")
```

### Comparing `kesslergame-2.1.1/src/kesslergame/controller_gamepad.py` & `KesslerGame-2.1.2/src/kesslergame/controller_gamepad.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*-
 
 from .controller import KesslerController
-from typing import Dict, Tuple
-from inputs import get_gamepad
+from typing import Dict, NoReturn, Tuple, Any, Final
+from inputs import get_gamepad  # type: ignore[import-untyped]
 import math
 import threading
 import time
 
 
 class GamepadController(KesslerController):
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.gamepad = XboxController()
         # tracker to determine if human paused game
         self.paused = False
         self.time_last_paused = 0.0
         # can only toggle pausing every 0.5 seconds
         self.pause_time_buffer = 0.5
 
-    def actions(self, ship_state: Dict, game_state: Dict) -> Tuple[float, float, bool, bool]:
+    def actions(self, ship_state: Dict[str, Any], game_state: Dict[str, Any]) -> Tuple[float, float, bool, bool]:
         """
         Read in the current gamepad state, and create the appropriate actions
         """
 
         self.pause_handler()
 
         # deadzones (both left and right using same currently)
         joystick_deadzone = 0.05
         trigger_deadzone = 0.05
 
         # Set thrust control
         if abs(self.gamepad.LeftJoystickY) > joystick_deadzone:
             thrust = self.gamepad.LeftJoystickY * 480.0
         else:
-            thrust = 0
+            thrust = 0.0
 
         # Set turn control
         if abs(self.gamepad.RightJoystickX) > joystick_deadzone:
-            turn_rate = -1 * self.gamepad.RightJoystickX * 180.0
+            turn_rate = -1.0 * self.gamepad.RightJoystickX * 180.0
         else:
-            turn_rate = 0
+            turn_rate = 0.0
 
         # Setfire control
         if self.gamepad.RightTrigger > trigger_deadzone:
             fire = True
         else:
             fire = False
 
@@ -56,19 +56,19 @@
 
         return thrust, turn_rate, fire, drop_mine
 
     @property
     def name(self) -> str:
         return "Gamepad Controller"
 
-    def explanation(self):
-        exp = None
+    def explanation(self) -> None:
+        exp: None = None
         return exp
 
-    def pause_handler(self):
+    def pause_handler(self) -> None:
 
         break_pause = False
         if time.perf_counter() - self.time_last_paused > self.pause_time_buffer and self.gamepad.Back == 1:
             pause_time = time.perf_counter()
             while break_pause is False:
                 if time.perf_counter() - pause_time > self.pause_time_buffer and self.gamepad.Back == 1:
                     break_pause = True
@@ -77,18 +77,18 @@
 class XboxController(object):
     """
     Class for Xbox inputs credit to Kevin Hughes and the TensorCart project.
     Copyright (c) 2017 Kevin Hughes
     MIT License
     """
 
-    MAX_TRIG_VAL = math.pow(2, 8)
-    MAX_JOY_VAL = math.pow(2, 15)
+    MAX_TRIG_VAL: Final[float] = 2.0**8
+    MAX_JOY_VAL: Final[float] = 2.0**15
 
-    def __init__(self):
+    def __init__(self) -> None:
 
         self.LeftJoystickY = 0
         self.LeftJoystickX = 0
         self.RightJoystickY = 0
         self.RightJoystickX = 0
         self.LeftTrigger = 0
         self.RightTrigger = 0
@@ -108,24 +108,24 @@
         self.DownDPad = 0
 
         self._monitor_thread = threading.Thread(target=self._monitor_controller, args=())
         self._monitor_thread.daemon = True
         self._monitor_thread.start()
 
 
-    def read(self):
+    def read(self) -> list[int | Any]:
         x = self.LeftJoystickX
         y = self.LeftJoystickY
         a = self.A
         b = self.X # b=1, x=2
         rb = self.RightBumper
         return [x, y, a, b, rb]
 
 
-    def _monitor_controller(self):
+    def _monitor_controller(self) -> NoReturn:
         while True:
             events = get_gamepad()
             for event in events:
                 if event.code == 'ABS_Y':
                     self.LeftJoystickY = event.state / XboxController.MAX_JOY_VAL # normalize between -1 and 1
                 elif event.code == 'ABS_X':
                     self.LeftJoystickX = event.state / XboxController.MAX_JOY_VAL # normalize between -1 and 1
```

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/graphics_base.py` & `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-import os
+#import os
 from tkinter import *
-from PIL import Image, ImageTk
+from typing import List
+#from PIL import Image, ImageTk  # type: ignore[import-untyped]
 
+from ..ship import Ship
+from ..asteroid import Asteroid
+from ..bullet import Bullet
+from ..mines import Mine
+from ..score import Score
+from ..scenario import Scenario
 
-class KesslerGraphics:
 
-    def start(self, scenario):
+class KesslerGraphics:
+    def start(self, scenario: Scenario) -> None:
         raise NotImplementedError('Your derived KesslerController must include a start() method.')
 
-    def update(self, score, ships, asteroids, bullets, mines):
+    def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet], mines: List[Mine]) -> None:
         raise NotImplementedError('Your derived KesslerController must include an update() method.')
 
-    def close(self):
+    def close(self) -> None:
         raise NotImplementedError('Your derived KesslerController must include a close() method.')
```

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/graphics_handler.py` & `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 from enum import Enum
-import numpy as np
+from typing import Optional, Dict, List
 from .graphics_base import KesslerGraphics
+from ..scenario import Scenario
+from ..ship import Ship
+from ..asteroid import Asteroid
+from ..bullet import Bullet
+from ..mines import Mine
+from ..score import Score
 
 class GraphicsType(Enum):
     NoGraphics = 0
     UnrealEngine = 1
     Tkinter = 2
     Pyplot = 3
     Custom = 4
 
 
 class GraphicsHandler:
-
-    def __init__(self, type: GraphicsType=GraphicsType.NoGraphics, scenario=None, UI_settings=None, graphics_obj=None):
+    def __init__(self, type: GraphicsType = GraphicsType.NoGraphics, scenario: Optional[Scenario] = None, UI_settings: Optional[Dict[str, bool]] = None, graphics_obj: Optional[KesslerGraphics] = None) -> None:
         """
         Create a graphics handler utilizing the assigned graphics engine defined from GraphicsType
         """
         self.type = type
+        self.graphics: Optional[KesslerGraphics]
         if graphics_obj is not None:
             self.graphics = graphics_obj
             if not issubclass(graphics_obj.__class__, KesslerGraphics):
                 raise ValueError('Settings "graphics_obj" must be a child of type "KesslerGraphics"')
         else:
             match self.type:
                 case GraphicsType.NoGraphics:
@@ -36,28 +42,32 @@
                 case GraphicsType.Tkinter:
                     from .graphics_tk import GraphicsTK
                     self.graphics = GraphicsTK(UI_settings)
                 case GraphicsType.Pyplot:
                     from .graphics_plt import GraphicsPLT
                     self.graphics = GraphicsPLT()
                 case GraphicsType.Custom:
-                    if graphics_obj is None:
-                        raise ValueError('"graphics_obj" must be defined in settings when using GraphicsType.Custom')
-                    else:
-                        self.graphics = graphics_obj
+                    #if graphics_obj is None:
+                    raise ValueError('"graphics_obj" must be defined in settings when using GraphicsType.Custom')
+                    #else:
+                    #    self.graphics = graphics_obj
 
         if self.type != GraphicsType.NoGraphics:
+            assert self.graphics is not None
+            assert scenario is not None
             self.graphics.start(scenario)
 
-    def update(self, score, ships, asteroids, bullets, mines):
+    def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet], mines: List[Mine]) -> None:
         """
         Update the graphics draw with new simulation data each simulation time-step
         """
         if self.type != GraphicsType.NoGraphics:
+            assert self.graphics is not None
             self.graphics.update(score, ships, asteroids, bullets, mines)
 
-    def close(self):
+    def close(self) -> None:
         """
         Finalize and close the graphics window
         """
         if self.type != GraphicsType.NoGraphics:
+            assert self.graphics is not None
             self.graphics.close()
```

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/graphics_tk.py` & `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_tk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 import os
-from tkinter import *
-from PIL import Image, ImageTk
+from tkinter import Tk, Canvas, NW
+from PIL import Image, ImageTk  # type: ignore[import-untyped]
 
+from typing import Dict, Optional, List
 from .graphics_base import KesslerGraphics
+from ..ship import Ship
+from ..asteroid import Asteroid
+from ..bullet import Bullet
+from ..mines import Mine
+from ..score import Score
+from ..scenario import Scenario
+from ..team import Team
 
 
 class GraphicsTK(KesslerGraphics):
-    def __init__(self, UI_settings):
+    def __init__(self, UI_settings: Optional[Dict[str, bool]] = None) -> None:
         # UI settings
         # lives, accuracy, asteroids hit, shots taken, bullets left
         # default_ui = {'ships': True, 'lives_remaining': True, 'accuracy': True, 'asteroids_hit': True}
         UI_settings = {} if UI_settings is None else UI_settings
         self.show_ships = UI_settings.get('ships', True)
         self.show_lives = UI_settings.get('lives_remaining', True)
         self.show_accuracy = UI_settings.get('accuracy', True)
         self.show_asteroids_hit = UI_settings.get('asteroids_hit', True)
         self.show_shots_fired = UI_settings.get('shots_fired', False)
         self.show_bullets_remaining = UI_settings.get('bullets_remaining', False)
         self.show_controller_name = UI_settings.get('controller_name', True)
 
-    def start(self, scenario):
+    def start(self, scenario: Scenario) -> None:
         self.game_width = scenario.map_size[0]
         self.game_height = scenario.map_size[1]
         self.max_time = scenario.time_limit
         self.score_width = 385
         self.window_width = self.game_width + self.score_width
-        ship_radius = scenario.ships()[0].radius * 2 - 5
+        ship_radius: int = int(scenario.ships()[0].radius * 2 - 5)
 
         # create and center main window
         self.window = Tk()
         self.window.title('Kessler')
         screen_width = self.window.winfo_screenwidth()
         screen_height = self.window.winfo_screenheight()
         center_x = int(screen_width / 2 - self.window_width / 2)
@@ -54,17 +62,17 @@
                             "images/playerShip3_orange.png"]
         self.num_images = len(self.image_paths)
         self.ship_images = [(Image.open(os.path.join(script_dir, image))).resize((ship_radius, ship_radius)) for image in self.image_paths]
         self.ship_sprites = [ImageTk.PhotoImage(img) for img in self.ship_images]
         self.ship_icons = [ImageTk.PhotoImage((Image.open(os.path.join(script_dir, image))).resize((ship_radius, ship_radius))) for image in self.image_paths]
 
         self.detoantion_time = 0.3
-        self.detonation_timers = []
+        #self.detonation_timers = []
 
-    def update(self, score, ships, asteroids, bullets, mines):
+    def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet], mines: List[Mine]) -> None:
 
         # Delete everything from canvas so we can re-plot
         self.game_canvas.delete("all")
 
         # Plot shields, bullets, ships, and asteroids
         self.plot_shields(ships)
         self.plot_ships(ships)
@@ -74,18 +82,18 @@
 
         # Update score box
         self.update_score(score, ships)
 
         # Push updates to graphics refresh
         self.window.update()
 
-    def close(self):
+    def close(self) -> None:
         self.window.destroy()
 
-    def update_score(self, score, ships):
+    def update_score(self, score: Score, ships: List[Ship]) -> None:
 
         # offsets to deal with cleanliness and window borders covering data
         x_offset = 5
         y_offset = 5
 
         # outline and center line
         self.game_canvas.create_rectangle(self.game_width, 0, self.window_width, self.game_height, outline="white", fill="black",)
@@ -109,46 +117,47 @@
 
             # add each ship to text if enabled
             if self.show_ships:
                 for ship in ships:
                     if ship.team == team.team_id:
                         ships_text += ("Ship " + str(ship.id))
                         if self.show_controller_name:
+                            assert ship.controller is not None
                             ships_text += ": " + str(ship.controller.name)
                         ships_text += '\n'
 
             team_info = self.format_ui(team)
             score_board = title + ships_text + team_info
 
             # determine output location based off order in team list
             if (team_num % 2) == 0:
-                output_location_x = self.game_width + x_offset
+                output_location_x = int(self.game_width + x_offset)
 
                 # y location is based off the number of lines in the previous teams row
                 output_location_y = output_location_y + (17 * max_lines) + y_offset
 
                 # line separating team rows
                 self.game_canvas.create_line(self.game_width, output_location_y - 10, self.window_width, output_location_y - 10, fill="white")
                 max_lines = score_board.count("\n")
             else:
-                output_location_x = self.window_width + x_offset - self.score_width / 2
+                output_location_x = int(self.window_width + x_offset - self.score_width / 2)
 
                 # change max lines in the row if odd team has more lines then even
                 if score_board.count("\n") > max_lines:
                     max_lines = score_board.count("\n")
 
             # display of team information
             self.game_canvas.create_text(output_location_x, output_location_y,
                                     text=score_board, fill="white", font=("Courier New", 10), anchor=NW, )
 
             self.game_canvas.create_image(output_location_x + 120, output_location_y + 15,
                                      image=self.ship_icons[(team.team_id-1) % self.num_images])
             team_num += 1
 
-    def format_ui(self, team):
+    def format_ui(self, team: Team) -> str:
         # lives, accuracy, asteroids hit, shots taken, bullets left
         team_info = "_________\n"
         if self.show_lives:
             team_info += "Lives: " + str(team.lives_remaining) + "\n"
         if self.show_accuracy:
             team_info += "Accuracy: " + str(round(team.accuracy * 100, 1)) + "\n"
         if self.show_asteroids_hit:
@@ -156,29 +165,29 @@
         if self.show_shots_fired:
             team_info += "Shots Fired: " + str(team.shots_fired) + "\n"
         if self.show_bullets_remaining:
             team_info += "Bullets Left: " + str(team.bullets_remaining) + "\n"
 
         return team_info
 
-    def plot_ships(self, ships):
+    def plot_ships(self, ships: List[Ship]) -> None:
         """
         Plots each ship on the game screen using cached sprites and rotating them
         """
         for idx, ship in enumerate(ships):
             if ship.alive:
                 # plot ship image and id text next to it
                 self.ship_sprites[idx] = ImageTk.PhotoImage(self.ship_images[idx].rotate(180 - (-ship.heading - 90)))
                 self.game_canvas.create_image(ship.position[0], self.game_height - ship.position[1],
                                               image=self.ship_sprites[idx])
                 self.game_canvas.create_text(ship.position[0] + ship.radius,
                                              self.game_height - (ship.position[1] + ship.radius), text=str(ship.id),
                                              fill="white")
 
-    def plot_shields(self, ships):
+    def plot_shields(self, ships: List[Ship]) -> None:
         """
         Plots each ship's shield ring
         """
         for ship in ships:
             if ship.alive:
                 # Color shield based on respawn time remaining
                 respawn_scaler = max(min(ship.respawn_time_left, 1), 0)
@@ -189,35 +198,35 @@
                 # Plot shield ring
                 self.game_canvas.create_oval(ship.position[0] - ship.radius,
                                              self.game_height - (ship.position[1] + ship.radius),
                                              ship.position[0] + ship.radius,
                                              self.game_height - (ship.position[1] - ship.radius),
                                              fill="black", outline=color)
 
-    def plot_bullets(self, bullets):
+    def plot_bullets(self, bullets: List[Bullet]) -> None:
         """
         Plots each bullet object on the game screen
         """
         for bullet in bullets:
             self.game_canvas.create_line(bullet.position[0], self.game_height - bullet.position[1],
                                          bullet.tail[0], self.game_height - bullet.tail[1],
                                          fill="#EE2737", width=3)
 
-    def plot_asteroids(self, asteroids):
+    def plot_asteroids(self, asteroids: List[Asteroid]) -> None:
         """
         Plots each asteroid object on the game screen
         """
         for asteroid in asteroids:
             self.game_canvas.create_oval(asteroid.position[0] - asteroid.radius,
                                          self.game_height - (asteroid.position[1] + asteroid.radius),
                                          asteroid.position[0] + asteroid.radius,
                                          self.game_height - (asteroid.position[1] - asteroid.radius),
                                          fill="grey")
 
-    def plot_mines(self, mines):
+    def plot_mines(self, mines: List[Mine]) -> None:
         """
         Plots and animates each mine object on the game screen and their detonations
         """
         for mine in mines:
             self.game_canvas.create_oval(mine.position[0] - mine.radius,
                                          self.game_height - (mine.position[1] + mine.radius),
                                          mine.position[0] + mine.radius,
@@ -236,10 +245,7 @@
                 explosion_radius = mine.blast_radius * (1 - mine.countdown_timer / mine.detonation_time)**2
                 self.game_canvas.create_oval(mine.position[0] - explosion_radius,
                                              self.game_height - (mine.position[1] + explosion_radius),
                                              mine.position[0] + explosion_radius,
                                              self.game_height - (mine.position[1] - explosion_radius),
                                              # fill="#fa441b",
                                              fill="", outline="white", width=10)
-
-
-
```

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/graphics_ue.py` & `KesslerGame-2.1.2/src/kesslergame/graphics/graphics_ue.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 import socket
 import numpy as np
 from typing import List
 
 from ..ship import Ship
 from ..asteroid import Asteroid
 from ..bullet import Bullet
+from ..mines import Mine
 from ..score import Score
 from ..scenario import Scenario
 from .graphics_base import KesslerGraphics
 
 
 class GraphicsUE(KesslerGraphics):
-    def __init__(self):
+    def __init__(self) -> None:
         # Create udp senders/receivers
         udp_host = 'localhost'
         udp_port = 12345
         self.udp_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.udp_recvr = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.udp_recvr.bind(('localhost', 12346))
         self.udp_addr = (udp_host, udp_port)
 
-    def start(self, scenario: Scenario):
+    def start(self, scenario: Scenario) -> None:
         self.map_size = scenario.map_size
         ship_count = len(scenario.ships())
         team_count = len(np.unique([ship.team for ship in scenario.ships()]))
 
         # TODO Launch game
 
         # Wait for graphics engine to be fully initialized before sending scenario initialization message
@@ -42,15 +43,15 @@
 
         start_str = '::start::'
         start_str += 'map:' + str(self.map_size[0]) + ',' + str(self.map_size[1]) + ';'
         start_str += 'ships:' + str(ship_count) + ';'
         start_str += 'teams:' + str(team_count)
         self.udp_sock.sendto(start_str.encode('utf-8'), self.udp_addr)
 
-    def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet]):
+    def update(self, score: Score, ships: List[Ship], asteroids: List[Asteroid], bullets: List[Bullet], mines: List[Mine]) -> None:
         update_parts = ['::frame::']
 
         for ship in ships:
             ship_part = 's({},{},{},{},{},{});'.format(
                 round(self.map_size[0] - ship.position[0]),
                 round(ship.position[1]),
                 round(180 - ship.heading),
@@ -96,9 +97,9 @@
             )
             update_parts.append(team_part)
 
         update_str = ''.join(update_parts)
 
         self.udp_sock.sendto(update_str.encode('utf-8'), self.udp_addr)
 
-    def close(self):
+    def close(self) -> None:
         self.udp_sock.close()
```

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip1_green.png` & `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_green.png`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip1_orange.png` & `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip1_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip2_orange.png` & `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip2_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/src/kesslergame/graphics/images/playerShip3_orange.png` & `KesslerGame-2.1.2/src/kesslergame/graphics/images/playerShip3_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-2.1.1/src/kesslergame/kessler_game.py` & `KesslerGame-2.1.2/src/kesslergame/kessler_game.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,99 +2,118 @@
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 import time
 
 import math
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Tuple, TypedDict, Optional
 from enum import Enum
 from collections import OrderedDict
 
 from .scenario import Scenario
 from .score import Score
 from .controller import KesslerController
 from .collisions import circle_line_collision
 from .graphics import GraphicsType, GraphicsHandler
+from .mines import Mine
+from .asteroid import Asteroid
+from .ship import Ship
+from .bullet import Bullet
+from .graphics import KesslerGraphics
 
 
 class StopReason(Enum):
     not_stopped = 0
     no_ships = 1
     no_asteroids = 2
     time_expired = 3
     out_of_bullets = 4
 
 
+class PerfDict(TypedDict, total=False):
+    controller_times: List[float]
+    total_controller_time: float
+    physics_update: float
+    collisions_check: float
+    score_update: float
+    graphics_draw: float
+    total_frame_time: float
+
+
 class KesslerGame:
-    def __init__(self, settings: Dict[str, Any] = None):
+    def __init__(self, settings: Optional[Dict[str, Any]] = None) -> None:
 
         if settings is None:
             settings = {}
         # Game settings
-        self.frequency = settings.get("frequency", 30.0)
-        self.time_step = 1 / settings.get("frequency", 30.0)
-        self.perf_tracker = settings.get("perf_tracker", True)
-        self.prints_on = settings.get("prints_on", True)
-        self.graphics_type = settings.get("graphics_type", GraphicsType.Tkinter)
-        self.graphics_obj = settings.get("graphics_obj", None)
-        self.realtime_multiplier = settings.get("realtime_multiplier", 0 if self.graphics_type==GraphicsType.NoGraphics else 1)
-        self.time_limit = settings.get("time_limit", None)
+        self.frequency: float = settings.get("frequency", 30.0)
+        self.time_step: float = 1 / settings.get("frequency", 30.0)
+        self.perf_tracker: bool = settings.get("perf_tracker", True)
+        self.prints_on: bool = settings.get("prints_on", True)
+        self.graphics_type: GraphicsType = settings.get("graphics_type", GraphicsType.Tkinter)
+        self.graphics_obj: Optional[KesslerGraphics] = settings.get("graphics_obj", None)
+        self.realtime_multiplier: float = settings.get("realtime_multiplier", 0 if self.graphics_type==GraphicsType.NoGraphics else 1)
+        self.time_limit: float = settings.get("time_limit", float("inf"))
 
         # UI settings
         default_ui = {'ships': True, 'lives_remaining': True, 'accuracy': True,
                       'asteroids_hit': True, 'bullets_remaining': True, 'controller_name': True}
         self.UI_settings = settings.get("UI_settings", default_ui)
         if self.UI_settings == 'all':
             self.UI_settings = {'ships': True, 'lives_remaining': True, 'accuracy': True,
                                 'asteroids_hit': True, 'shots_fired': True, 'bullets_remaining': True,
                                 'controller_name': True}
         
-    def run(self, scenario: Scenario, controllers: List[KesslerController]) -> (Score, OrderedDict):
+    def run(self, scenario: Scenario, controllers: List[KesslerController]) -> Tuple[Score, List[PerfDict]]:
         """
         Run an entire scenario from start to finish and return score and stop reason
         """
 
         ##################
         # INITIALIZATION #
         ##################
         # Initialize objects lists from scenario
-        asteroids = scenario.asteroids()
-        ships = scenario.ships()
-        bullets = []
-        mines = []
+        asteroids: List[Asteroid] = scenario.asteroids()
+        ships: List[Ship] = scenario.ships()
+        bullets: List[Bullet] = []
+        mines: List[Mine] = []
 
         # Initialize Scoring class
         score = Score(scenario)
 
         # Initialize environment parameters
         stop_reason = StopReason.not_stopped
-        sim_time = 0
-        step = 0
+        sim_time: float = 0.0
+        step: int = 0
         time_limit = scenario.time_limit if scenario.time_limit else self.time_limit
 
         # Assign controllers to each ship
         for controller, ship in zip(controllers, ships):
             controller.ship_id = ship.id
             ship.controller = controller
 
         # Initialize graphics display
         graphics = GraphicsHandler(type=self.graphics_type, scenario=scenario, UI_settings=self.UI_settings, graphics_obj=self.graphics_obj)
 
         # Initialize list of dictionary for performance tracking (will remain empty if perf_tracker is false
-        perf_list = []
+        perf_list: List[PerfDict] = []
 
         ######################
         # MAIN SCENARIO LOOP #
         ######################
+        bullet_remove_idxs: list[int] = []
+        asteroid_remove_idxs: set[int] = set()
+        mine_remove_idxs: list[int] = []
+        new_asteroids: list[Asteroid] = []
         while stop_reason == StopReason.not_stopped:
 
             # Get perf time at the start of time step evaluation and initialize performance tracker
             step_start = time.perf_counter()
-            perf_dict = OrderedDict()
+            perf_dict: PerfDict = {}
 
             # --- CALL CONTROLLER FOR EACH SHIP ------------------------------------------------------------------------
             # Get all live ships
             liveships = [ship for ship in ships if ship.alive]
 
             # Generate game_state info to send to controllers
             game_state = {
@@ -114,16 +133,16 @@
                 perf_dict['controller_times'] = []
                 t_start = time.perf_counter()
 
             # Loop through each controller/ship combo and apply their actions
             for idx, ship in enumerate(ships):
                 if ship.alive:
                     # Reset controls on ship to defaults
-                    ship.thrust = 0
-                    ship.turn_rate = 0
+                    ship.thrust = 0.0
+                    ship.turn_rate = 0.0
                     ship.fire = False
                     # Evaluate each controller letting control be applied
                     if controllers[idx].ship_id != ship.id:
                         raise RuntimeError("Controller and ship ID do not match")
                     ship.thrust, ship.turn_rate, ship.fire, ship.drop_mine = controllers[idx].actions(ship.ownstate, game_state)
 
                 # Update controller evaluation time if performance tracking
@@ -153,39 +172,33 @@
                     if new_mine is not None:
                         mines.append(new_mine)
 
             # Cull any bullets past the map edge
             bullets = [bullet
                        for bullet
                        in bullets
-                       if 0 <= bullet.position[0] <= scenario.map_size[0]
-                       and 0 <= bullet.position[1] <= scenario.map_size[1]]
+                       if 0.0 <= bullet.position[0] <= scenario.map_size[0]
+                       and 0.0 <= bullet.position[1] <= scenario.map_size[1]]
 
             # Wrap ships and asteroids to other side of map
             for ship in liveships:
-                for idx, pos in enumerate(ship.position):
-                    bound = scenario.map_size[idx]
-                    ship.position[idx] = pos % bound
+                ship.position = (ship.position[0] % scenario.map_size[0], ship.position[1] % scenario.map_size[1])
 
             for asteroid in asteroids:
-                for idx, pos in enumerate(asteroid.position):
-                    bound = scenario.map_size[idx]
-                    asteroid.position[idx] = pos % bound
+                asteroid.position = (asteroid.position[0] % scenario.map_size[0], asteroid.position[1] % scenario.map_size[1])
 
             # Update performance tracker with
             if self.perf_tracker:
                 perf_dict['physics_update'] = time.perf_counter() - prev
                 prev = time.perf_counter()
 
             # --- CHECK FOR COLLISIONS ---------------------------------------------------------------------------------
 
 
             # --- Check asteroid-bullet collisions ---
-            bullet_remove_idxs = []
-            asteroid_remove_idxs = set() # Keep track of deleted asteroids, and cull all at once at the end
             for idx_bul, bullet in enumerate(bullets):
                 for idx_ast, asteroid in enumerate(asteroids):
                     if idx_ast in asteroid_remove_idxs:
                         continue
                     # If collision occurs
                     if circle_line_collision(bullet.position, bullet.tail, asteroid.position, asteroid.radius):
                         # Increment hit values on ship that fired bullet then destruct bullet and mark for removal
@@ -197,18 +210,17 @@
                         asteroids.extend(asteroid.destruct(impactor=bullet))
                         asteroid_remove_idxs.add(idx_ast)
                         # Stop checking this bullet
                         break
             # Cull bullets and asteroids that are marked for removal
             if bullet_remove_idxs:
                 bullets = [bullet for idx, bullet in enumerate(bullets) if idx not in bullet_remove_idxs]
+                bullet_remove_idxs.clear()
 
             # --- Check mine-asteroid and mine-ship effects ---
-            mine_remove_idxs = []
-            new_asteroids = []
             for idx_mine, mine in enumerate(mines):
                 if mine.detonating:
                     for idx_ast, asteroid in enumerate(asteroids):
                         if idx_ast in asteroid_remove_idxs:
                             continue
                         dx = asteroid.position[0] - mine.position[0]
                         dy = asteroid.position[1] - mine.position[1]
@@ -227,49 +239,54 @@
                                 # Ship destruct function.
                                 ship.destruct(map_size=scenario.map_size)
                     if idx_mine not in mine_remove_idxs:
                         mine_remove_idxs.append(idx_mine)
                     mine.destruct()
             if mine_remove_idxs:
                 mines = [mine for idx, mine in enumerate(mines) if idx not in mine_remove_idxs]
-            asteroids.extend(new_asteroids)
+                mine_remove_idxs.clear()
+            if new_asteroids:
+                asteroids.extend(new_asteroids)
+                new_asteroids.clear()
 
 
             # --- Check asteroid-ship collisions ---
-            for idx_ship, ship in enumerate(liveships):
+            for ship in liveships:
                 if not ship.is_respawning:
                     for idx_ast, asteroid in enumerate(asteroids):
                         if idx_ast in asteroid_remove_idxs:
                             continue
                         dx = ship.position[0] - asteroid.position[0]
                         dy = ship.position[1] - asteroid.position[1]
                         radius_sum = ship.radius + asteroid.radius
-                        # If collision occurs
-                        if dx * dx + dy * dy <= radius_sum * radius_sum:
+                        # Most of the time no collision occurs, so use early exit to optimize collision check
+                        if abs(dx) <= radius_sum and abs(dy) <= radius_sum and dx * dx + dy * dy <= radius_sum * radius_sum:
                             # Asteroid destruct function and mark for removal
                             asteroids.extend(asteroid.destruct(impactor=ship))
                             asteroid_remove_idxs.add(idx_ast)
                             # Ship destruct function. Add one to asteroids_hit
                             ship.asteroids_hit += 1
                             ship.destruct(map_size=scenario.map_size)
                             # Stop checking this ship's collisions
                             break
             # Cull ships if not alive and asteroids that are marked for removal
             liveships = [ship for ship in liveships if ship.alive]
             if asteroid_remove_idxs:
                 asteroids = [asteroid for idx, asteroid in enumerate(asteroids) if idx not in asteroid_remove_idxs]
+                asteroid_remove_idxs.clear()
 
             # --- Check ship-ship collisions ---
             for i, ship1 in enumerate(liveships):
                 for ship2 in liveships[i + 1:]:
                     if not ship2.is_respawning and not ship1.is_respawning:
                         dx = ship1.position[0] - ship2.position[0]
                         dy = ship1.position[1] - ship2.position[1]
                         radius_sum = ship1.radius + ship2.radius
-                        if dx * dx + dy * dy <= radius_sum * radius_sum:
+                        # Most of the time no collision occurs, so use early exit to optimize collision check
+                        if abs(dx) <= radius_sum and abs(dy) <= radius_sum and dx * dx + dy * dy <= radius_sum * radius_sum:
                             ship1.destruct(map_size=scenario.map_size)
                             ship2.destruct(map_size=scenario.map_size)
             # Cull ships that are not alive
             liveships = [ship for ship in liveships if ship.alive]
 
             # Update performance tracker with collisions timing
             if self.perf_tracker:
@@ -336,22 +353,22 @@
         score.finalize(sim_time, stop_reason, ships)
 
         # Return the score and stop condition
         return score, perf_list
 
 
 class TrainerEnvironment(KesslerGame):
-    def __init__(self, settings: Dict[str, Any] = None):
+    def __init__(self, settings: Optional[Dict[str, Any]] = None) -> None:
         """
         Instantiates a KesslerGame object with settings to optimize training time
         """
         if settings is None:
             settings = {}
         trainer_settings = {
             'frequency': settings.get("frequency", 30.0),
             'perf_tracker': settings.get("perf_tracker", False),
             'prints_on': settings.get("prints_on", False),
             'graphics_type': GraphicsType.NoGraphics,
             'realtime_multiplier': 0,
-            'time_limit': settings.get("time_limit", None)
+            'time_limit': settings.get("time_limit", float("inf"))
         }
         super().__init__(trainer_settings)
```

### Comparing `kesslergame-2.1.1/src/kesslergame/mines.py` & `KesslerGame-2.1.2/src/kesslergame/mines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-from typing import List, Tuple, Dict, Any
+from typing import List, Tuple, Dict, Any, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .ship import Ship
+    from .asteroid import Asteroid
 
 
 class Mine:
-    def __init__(self, starting_position: List[float], owner):
-        self.fuse_time = 3
+    __slots__ = ('fuse_time', 'detonation_time', 'mass', 'radius', 'blast_radius', 'blast_pressure', 'owner', 'countdown_timer', 'detonating', 'position')
+    def __init__(self, starting_position: List[float], owner: 'Ship') -> None:
+        self.fuse_time = 3.0
         self.detonation_time = 0.25
-        self.mass = 25  # mass units - kg?
-        self.radius = 12
-        self.blast_radius = 150
-        self.blast_pressure = 2000
+        self.mass = 25.0  # mass units - kg?
+        self.radius = 12.0
+        self.blast_radius = 150.0
+        self.blast_pressure = 2000.0
 
         self.owner = owner
         self.countdown_timer = self.fuse_time
         self.detonating = False
         self.position = starting_position
 
-    def update(self, delta_time=1/30):
+    def update(self, delta_time: float = 1/30) -> None:
         self.countdown_timer -= delta_time
         if self.countdown_timer <= 1e-15:
             self.detonate()
 
-    def detonate(self):
+    def detonate(self) -> None:
         # perform any detonation stuff here
         self.detonating = True
 
-    def destruct(self):
-        ...
+    def destruct(self) -> None:
+        pass
 
     @property
     def state(self) -> Dict[str, Any]:
         return {
             "position": tuple(self.position),
             "mass": float(self.mass),
             "fuse_time": float(self.fuse_time),
             "remaining_time": float(self.countdown_timer)
         }
 
-    def calculate_blast_force(self, dist, obj):
+    def calculate_blast_force(self, dist: float, obj: 'Asteroid') -> float:
         """
         Calculates the blast force based on the blast radius, blast pressure, and a linear decrease in intensity from the mine location to the blast radius
         Also takes into account asteroid diameter to resolve total acceleration based on size/mass
         """
-        return (-dist/self.blast_radius + 1) * self.blast_pressure * 2 * obj.radius
+        return (-dist/self.blast_radius + 1) * self.blast_pressure * 2.0 * obj.radius
```

### Comparing `kesslergame-2.1.1/src/kesslergame/scenario.py` & `KesslerGame-2.1.2/src/kesslergame/scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2018-2020 Thales Avionics USA
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-import math
-from typing import List, Tuple, Dict, Any
+from typing import List, Tuple, Dict, Any, Optional
 import random
 
 from .ship import Ship
 from .asteroid import Asteroid
 
 
 class Scenario:
-    def __init__(self, name: str = "Unnamed", num_asteroids: int = 0, asteroid_states: List[Dict[str, Any]] = None,
-                 ship_states: List[Dict[str, Any]] = None, map_size: Tuple[int, int] = None, seed: int = None,
-                 time_limit: float = float("inf"), ammo_limit_multiplier: float = 0.0, stop_if_no_ammo: bool = False):
+    def __init__(self, name: str = "Unnamed", num_asteroids: int = 0, asteroid_states: Optional[List[Dict[str, Any]]] = None,
+                 ship_states: Optional[List[Dict[str, Any]]] = None, map_size: Optional[Tuple[int, int]] = None, seed: Optional[int] = None,
+                 time_limit: float = float("inf"), ammo_limit_multiplier: float = 0.0, stop_if_no_ammo: bool = False) -> None:
         """
         Specify the starting state of the environment, including map dimensions and optional features
 
         Make sure to only set either ``num_asteroids`` or ``asteroid_states``. If neither are set, the
         Scenario defaults to 3 randomly placed asteroids
 
         :param name: Optional, name of the scenario
@@ -28,15 +27,15 @@
         :param game_map: Game Map using ``Map`` object
         :param seed: Optional seeding value to pass to random.seed() which is called before asteroid creation
         :param time_limit: Optional seeding value to pass to random.seed() which is called before asteroid creation
         :param ammo_limit_multiplier: Optional value for limiting the number of bullets each ship will have
         :param stop_if_no_ammo: Optional flag for stopping the scenario if all ships run out of ammo
         """
         # Protected variable for managing the name, through getter/setter interface
-        self._name = None
+        self._name: Optional[str] = None
 
         # Store name as string using setter
         self.name = name
 
         # Store map size
         self.map_size = map_size if map_size else (1000, 800)
 
@@ -79,19 +78,19 @@
         elif num_asteroids:
             self.asteroid_states = [dict() for _ in range(num_asteroids)]
         else:
             raise (ValueError("User should define `num_asteroids` or `asteroid_states` to create "
                               "valid custom starting states for the environment"))
 
     @property
-    def name(self):
+    def name(self) -> None | str:
         return self._name
 
     @name.setter
-    def name(self, name: str):
+    def name(self, name: str) -> None:
         # Raises error if the name cannot be converted to string
         self._name = str(name)
 
     @property
     def num_starting_asteroids(self) -> float:
         return len(self.asteroid_states)
 
@@ -112,15 +111,15 @@
             else:
                 return temp
 
         else:
             return -1
 
     @staticmethod
-    def count_asteroids(asteroid_size) -> float:
+    def count_asteroids(asteroid_size: int) -> int:
         # Counting based off of each asteroid making 3 children when destroyed
         return sum([3 ** (size - 1) for size in range(1, asteroid_size + 1)])
 
     def asteroids(self) -> List[Asteroid]:
         """
         Create asteroid sprites
         :param frequency: Operating frequency of the game
```

### Comparing `kesslergame-2.1.1/src/kesslergame/score.py` & `KesslerGame-2.1.2/src/kesslergame/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
-from typing import List
+from typing import List, Optional, TYPE_CHECKING
 
 import numpy as np
 
 from .ship import Ship
 from .asteroid import Asteroid
 from .scenario import Scenario
 from .team import Team
+if TYPE_CHECKING:
+    from .kessler_game import StopReason
 
 
 class Score:
-    def __init__(self, scenario: Scenario):
-        self.sim_time = 0
-        self.stop_reason = None
+    def __init__(self, scenario: Scenario) -> None:
+        self.sim_time: float = 0.0
+        self.stop_reason: Optional['StopReason'] = None
 
 
         # Initialize team classes to score team-specific scores
         team_ids = [ship.team for ship in scenario.ships()]
         team_names = [ship.team_name for ship in scenario.ships()]
-        self.teams = [Team(team_id, team_name) for team_id, team_name in zip(np.unique(team_ids), np.unique(team_names))]
+        self.teams = [Team(int(team_id), str(team_name)) for team_id, team_name in zip(np.unique(team_ids), np.unique(team_names))]
 
         # Populate scenario initial conditions into score parameters
         for team in self.teams:
             team.total_asteroids = scenario.max_asteroids
             for ship in scenario.ships():
                 if team.team_id == ship.team:
                     team.total_bullets += scenario.bullet_limit
 
-    def update(self, ships: List[Ship], sim_time, controller_perf: List[float] = None):
+    def update(self, ships: List[Ship], sim_time: float, controller_perf: Optional[List[float]] = None) -> None:
         self.sim_time = sim_time
         for team in self.teams:
             ast_hit, bul_hit, shots, bullets, deaths, lives = (0, 0, 0, 0, 0, 0)
             for idx, ship in enumerate(ships):
                 if team.team_id == ship.team:
                     ast_hit += ship.asteroids_hit
                     bul_hit += ship.bullets_hit
@@ -43,11 +45,11 @@
                     bullets += ship.bullets_remaining
                     deaths += ship.deaths
                     lives += ship.lives
                     if controller_perf is not None and controller_perf[idx] > 0:
                         team.eval_times.append(controller_perf[idx])
             team.asteroids_hit, team.bullets_hit, team.shots_fired, team.bullets_remaining, team.deaths, team.lives_remaining = (ast_hit, bul_hit, shots, bullets, deaths, lives)
 
-    def finalize(self, sim_time, stop_reason, ships):
+    def finalize(self, sim_time: float, stop_reason: 'StopReason', ships: List[Ship]) -> None:
         self.sim_time = sim_time
         self.stop_reason = stop_reason
         self.final_controllers = [ship.controller for ship in ships]
```

### Comparing `kesslergame-2.1.1/src/kesslergame/ship.py` & `KesslerGame-2.1.2/src/kesslergame/ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,66 +2,76 @@
 # Copyright © 2022 Thales. All Rights Reserved.
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 import math
 import warnings
 import numpy as np
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Tuple, Optional
 
 from .bullet import Bullet
 from .mines import Mine
+from .controller import KesslerController
 
 
 class Ship:
-    def __init__(self, ship_id,
-                 position: List[float],
-                 angle: float = 90,
+    __slots__ = (
+        'controller', 'thrust', 'turn_rate', 'id', 'speed', 'position',
+        'velocity', 'heading', 'lives', 'deaths', 'team', 'team_name',
+        'fire', 'drop_mine', 'thrust_range', 'turn_rate_range', 'max_speed',
+        'drag', 'radius', 'mass', '_respawning', '_respawn_time', '_fire_limiter',
+        '_fire_time', '_mine_limiter', '_mine_deploy_time', 'mines_remaining',
+        'bullets_remaining', 'bullets_shot', 'mines_dropped', 'bullets_hit',
+        'mines_hit', 'asteroids_hit'
+    )
+    def __init__(self, ship_id: int,
+                 position: Tuple[float, float],
+                 angle: float = 90.0,
                  lives: int = 3,
                  team: int = 1,
-                 team_name: str = None,
+                 team_name: Optional[str] = None,
                  bullets_remaining: int = -1,
-                 mines_remaining: int = 0):
+                 mines_remaining: int = 0) -> None:
         """
         Instantiate a ship with default parameters and infinite bullets if not specified
         """
 
         # Control information
-        self.controller = None
-        self.thrust = 0.0     # speed defaults to minimum
-        self.turn_rate = 0.0
+        self.controller: Optional[KesslerController] = None
+        self.thrust: float = 0.0  # speed defaults to minimum
+        self.turn_rate: float = 0.0
 
         # State info
-        self.id = ship_id
-        self.speed = 0.0
-        self.position = position
-        self.velocity = [0.0, 0.0]
-        self.heading = angle
-        self.lives = lives
-        self.deaths = 0
-        self.team = team
-        self.team_name = team_name if team_name is not None else 'Team ' + str(self.team)
+        self.id: int = ship_id
+        self.speed: float = 0.0
+        self.position: tuple[float, float] = position
+        self.velocity: tuple[float, float] = (0.0, 0.0)
+        self.heading: float = angle
+        self.lives: int = lives
+        self.deaths: int = 0
+        self.team: int = team
+        self.team_name: str = team_name if team_name is not None else 'Team ' + str(self.team)
 
         # Controller inputs
         self.fire = False
-        self.thrust = 0
-        self.turn_rate = 0
+        self.thrust = 0.0
+        self.turn_rate = 0.0
         self.drop_mine = False
 
         # Physical model constants/params
         self.thrust_range = (-480.0, 480.0)  # m/s^2
         self.turn_rate_range = (-180.0, 180.0)  # Degrees per second
-        self.max_speed = 240  # Meters per second
+        self.max_speed = 240.0  # Meters per second
         self.drag = 80.0  # m/s^2
-        self.radius = 20  # meters TODO verify radius size
-        self.mass = 300  # kg - reasonable? max asteroid mass currently is ~490 kg
+        self.radius = 20.0  # meters TODO verify radius size
+        self.mass = 300.0  # kg - reasonable? max asteroid mass currently is ~490 kg
 
         # Manage respawns/firing via timers
-        self._respawning = 0
-        self._respawn_time = 3  # seconds
+        self._respawning = 0.0
+        self._respawn_time = 3.0  # seconds
         self._fire_limiter = 0.0 # seconds
         self._fire_time = 1 / 10  # seconds
         self._mine_limiter = 0.0 # second
         self._mine_deploy_time = 1.0 # seconds
 
         # Track bullet/mine statistics
         self.mines_remaining = mines_remaining
@@ -100,15 +110,15 @@
                 "thrust_range": self.thrust_range,
                 "turn_rate_range": self.turn_rate_range,
                 "max_speed": self.max_speed,
                 "drag": self.drag,
         }
 
     @property
-    def alive(self):
+    def alive(self) -> bool:
         return True if self.lives > 0 else False
 
     @property
     def is_respawning(self) -> bool:
         return True if self._respawning else False
 
     @property
@@ -139,18 +149,18 @@
     def fire_wait_time(self) -> float:
         return self._fire_limiter
 
     @property
     def mine_wait_time(self) -> float:
         return self._mine_limiter
 
-    def shoot(self):
+    def shoot(self) -> None:
         self.fire = True
 
-    def update(self, delta_time: float = 1 / 30) -> tuple[Bullet, Mine]:
+    def update(self, delta_time: float = 1 / 30) -> tuple[Optional[Bullet], Optional[Mine]]:
         """
         Update our position and other particulars.
         """
 
         # Fire a bullet if instructed to
         if self.fire:
             new_bullet = self.fire_bullet()
@@ -159,16 +169,16 @@
 
         if self.drop_mine:
             new_mine = self.deploy_mine()
         else:
             new_mine = None
 
         # Decrement respawn timer (if necessary)
-        if self._respawning <= 0:
-            self._respawning = 0
+        if self._respawning <= 0.0:
+            self._respawning = 0.0
         else:
             self._respawning -= delta_time
 
         # Decrement fire limit timer (if necessary)
         if self._fire_limiter != 0.0:
             self._fire_limiter -= delta_time
             if self._fire_limiter <= 0.00000000001:
@@ -206,81 +216,83 @@
             self.turn_rate = min(max(self.turn_rate_range[0], self.turn_rate), self.turn_rate_range[1])
             warnings.warn('Ship ' + str(self.id) + ' turn rate command outside of allowable range', RuntimeWarning)
 
         # Update the angle based on turning rate
         self.heading += self.turn_rate * delta_time
 
         # Keep the angle within (0, 360)
-        self.heading %= 360
+        self.heading %= 360.0
 
         # Use speed magnitude to get velocity vector
-        self.velocity = [math.cos(math.radians(self.heading)) * self.speed,
-                         math.sin(math.radians(self.heading)) * self.speed]
+        rad_heading = math.radians(self.heading)
+        self.velocity = (math.cos(rad_heading) * self.speed,
+                         math.sin(rad_heading) * self.speed)
 
         # Update the position based off the velocities
-        self.position = [pos + v * delta_time for pos, v in zip(self.position, self.velocity)]
+        self.position = (self.position[0] + self.velocity[0] * delta_time, self.position[1] + self.velocity[1] * delta_time)
 
         return new_bullet, new_mine
 
-    def destruct(self, map_size):
+    def destruct(self, map_size: tuple[float, float]) -> None:
         """
         Called by the game when a ship collides with something and dies. Handles life decrementing and triggers respawn
         """
         self.lives -= 1
         self.deaths +=1
         # spawn_position = [map_size[0] / 2,
         #                   map_size[1] / 2]
         spawn_position = self.position
         spawn_heading = self.heading
         self.respawn(spawn_position, spawn_heading)
 
-    def respawn(self, position: List[float], heading: float = 90.0) -> None:
+    def respawn(self, position: Tuple[float, float], heading: float = 90.0) -> None:
         """
         Called when we die and need to make a new ship.
         'respawning' is an invulnerability timer.
         """
         # If we are in the middle of respawning, this is non-zero.
         self._respawning = self._respawn_time
 
         # Set location and physical parameters
         self.position = position
         self.speed = 0.0
-        self.velocity = [0.0, 0.0]
+        self.velocity = (0.0, 0.0)
         self.heading = heading
 
-    def deploy_mine(self):
+    def deploy_mine(self) -> Mine | None:
         # if self.mines_remaining != 0 and not self._mine_limiter:
         if self.can_deploy_mine:
 
             # Remove respawn invincibility. Mine deployment limiter
-            self._respawning = 0
+            self._respawning = 0.0
             self._mine_limiter = self._mine_deploy_time
 
             if self.mines_remaining > 0:
                 self.mines_remaining -= 1
             self.mines_dropped += 1
             mine_x = self.position[0]
             mine_y = self.position[1]
             return Mine([mine_x, mine_y], owner=self)
         else:
             return None
 
-    def fire_bullet(self):
+    def fire_bullet(self) -> Bullet | None:
         # if self.bullets_remaining != 0 and not self._fire_limiter:
         if self.can_fire:
 
             # Remove respawn invincibility. Trigger fire limiter
-            self._respawning = 0
+            self._respawning = 0.0
             self._fire_limiter = self._fire_time
 
             # Bullet counters
             if self.bullets_remaining > 0:
                 self.bullets_remaining -= 1
             self.bullets_shot += 1
 
             # Return the bullet object that was fired
-            bullet_x = self.position[0] + self.radius * math.cos(math.radians(self.heading))
-            bullet_y = self.position[1] + self.radius * math.sin(math.radians(self.heading))
-            return Bullet([bullet_x, bullet_y], self.heading, owner=self)
+            rad_heading = math.radians(self.heading)
+            bullet_x = self.position[0] + self.radius * math.cos(rad_heading)
+            bullet_y = self.position[1] + self.radius * math.sin(rad_heading)
+            return Bullet((bullet_x, bullet_y), self.heading, owner=self)
 
         # Return nothing if we can't fire a bullet right now
         return None
```

### Comparing `kesslergame-2.1.1/src/kesslergame/team.py` & `KesslerGame-2.1.2/src/kesslergame/team.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 # NOTICE: This file is subject to the license agreement defined in file 'LICENSE', which is part of
 # this source code package.
 
 import numpy as np
 
 
 class Team:
-    def __init__(self, id, name):
+    def __init__(self, id: int, name: str) -> None:
         self.team_id = id
         self.team_name = name
 
-        self.total_bullets = 0
-        self.total_asteroids = 0
+        self.total_bullets: int = 0
+        self.total_asteroids: int = 0
 
-        self.asteroids_hit = 0
-        self.bullets_hit = 0
-        self.shots_fired = 0
-        self.bullets_remaining = 0
-        self.deaths = 0
-        self.eval_times = []
-        self.lives_remaining = 0
+        self.asteroids_hit: int = 0
+        self.bullets_hit: int = 0
+        self.shots_fired: int = 0
+        self.bullets_remaining: int = 0
+        self.deaths: int = 0
+        self.eval_times: list[float] = []
+        self.lives_remaining: int = 0
 
     @property
     def accuracy(self) -> float:
-        return self.bullets_hit / self.shots_fired if self.shots_fired else 0
+        return self.bullets_hit / self.shots_fired if self.shots_fired else 0.0
 
     @property
     def fraction_total_asteroids_hit(self) -> float:
         return self.asteroids_hit / self.total_asteroids
 
     @property
     def fraction_bullets_used(self) -> float:
@@ -36,20 +36,32 @@
 
     @property
     def ratio_bullets_needed(self) -> float:
         return self.shots_fired / self.total_asteroids
 
     @property
     def mean_eval_time(self) -> float:
-        return np.mean(self.eval_times)
+        if self.eval_times:
+            return float(np.mean(self.eval_times))
+        else:
+            return 0.0
 
     @property
     def median_eval_time(self) -> float:
-        return np.median(self.eval_times)
+        if self.eval_times:
+            return float(np.median(self.eval_times))
+        else:
+            return 0.0
 
     @property
     def min_eval_time(self) -> float:
-        return min(self.eval_times)
+        if self.eval_times:
+            return min(self.eval_times)
+        else:
+            return 0.0
 
     @property
     def max_eval_time(self) -> float:
-        return max(self.eval_times)
+        if self.eval_times:
+            return max(self.eval_times)
+        else:
+            return 0.0
```

### Comparing `kesslergame-2.1.1/src/kesslergame.egg-info/PKG-INFO` & `KesslerGame-2.1.2/src/KesslerGame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: kesslergame
-Version: 2.1.1
+Name: KesslerGame
+Version: 2.1.2
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
-Author-email: zachariah.phillips@us.thalesgroup.com
+Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
-Maintainer-email: tim.arnett@psibernetix.com
+Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
 Keywords: artificial intelligence,asteroids,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `kesslergame-2.1.1/src/kesslergame.egg-info/SOURCES.txt` & `KesslerGame-2.1.2/src/KesslerGame.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
+src/KesslerGame.egg-info/PKG-INFO
+src/KesslerGame.egg-info/SOURCES.txt
+src/KesslerGame.egg-info/dependency_links.txt
+src/KesslerGame.egg-info/requires.txt
+src/KesslerGame.egg-info/top_level.txt
+src/KesslerGame.egg-info/zip-safe
 src/kesslergame/__init__.py
+src/kesslergame/_version.py
 src/kesslergame/asteroid.py
 src/kesslergame/bullet.py
 src/kesslergame/collisions.py
 src/kesslergame/controller.py
 src/kesslergame/controller_gamepad.py
 src/kesslergame/kessler_game.py
 src/kesslergame/mines.py
 src/kesslergame/scenario.py
 src/kesslergame/score.py
 src/kesslergame/ship.py
 src/kesslergame/team.py
-src/kesslergame.egg-info/PKG-INFO
-src/kesslergame.egg-info/SOURCES.txt
-src/kesslergame.egg-info/dependency_links.txt
-src/kesslergame.egg-info/requires.txt
-src/kesslergame.egg-info/top_level.txt
-src/kesslergame.egg-info/zip-safe
 src/kesslergame/graphics/__init__.py
 src/kesslergame/graphics/graphics_base.py
 src/kesslergame/graphics/graphics_handler.py
 src/kesslergame/graphics/graphics_plt.py
 src/kesslergame/graphics/graphics_tk.py
 src/kesslergame/graphics/graphics_ue.py
 src/kesslergame/graphics/images/__init__.py
```

