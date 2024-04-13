# Comparing `tmp/pogema-1.2.2.tar.gz` & `tmp/pogema-1.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema-1.2.2.tar", last modified: Fri Sep 22 09:45:50 2023, max compression
+gzip compressed data, was "pogema-1.2.3a0.tar", last modified: Sat Apr 13 20:36:40 2024, max compression
```

## Comparing `pogema-1.2.2.tar` & `pogema-1.2.3a0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.311834 pogema-1.2.2/
--rw-r--r--   0 skrynnik   (503) staff       (20)     1073 2023-08-30 09:49:20.000000 pogema-1.2.2/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)     6853 2023-09-22 09:45:50.310940 pogema-1.2.2/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)     6472 2023-08-31 15:07:00.000000 pogema-1.2.2/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.280598 pogema-1.2.2/pogema/
--rw-r--r--   0 skrynnik   (503) staff       (20)      965 2023-09-22 09:45:14.000000 pogema-1.2.2/pogema/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4029 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/a_star_policy.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    26027 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/animation.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    16259 2023-09-22 09:44:42.000000 pogema-1.2.2/pogema/envs.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4800 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11642 2023-09-22 09:44:42.000000 pogema-1.2.2/pogema/grid.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     8150 2023-09-22 09:44:42.000000 pogema-1.2.2/pogema/grid_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3187 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/grid_registry.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.299994 pogema-1.2.2/pogema/integrations/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/integrations/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2522 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/integrations/make_pogema.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2607 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/integrations/pettingzoo.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2610 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/integrations/pymarl.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      936 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/integrations/sample_factory.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3254 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.306487 pogema-1.2.2/pogema/wrappers/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/wrappers/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3912 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/wrappers/metrics.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      656 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/wrappers/multi_time_limit.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3080 2023-08-30 09:49:20.000000 pogema-1.2.2/pogema/wrappers/persistence.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.287294 pogema-1.2.2/pogema.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)     6853 2023-09-22 09:45:50.000000 pogema-1.2.2/pogema.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      793 2023-09-22 09:45:50.000000 pogema-1.2.2/pogema.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2023-09-22 09:45:50.000000 pogema-1.2.2/pogema.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       65 2023-09-22 09:45:50.000000 pogema-1.2.2/pogema.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        7 2023-09-22 09:45:50.000000 pogema-1.2.2/pogema.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2023-09-22 09:45:50.311932 pogema-1.2.2/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1409 2023-08-30 09:49:20.000000 pogema-1.2.2/setup.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2023-09-22 09:45:50.310129 pogema-1.2.2/tests/
--rw-r--r--   0 skrynnik   (503) staff       (20)     7234 2023-08-31 15:07:00.000000 pogema-1.2.2/tests/test_deterministic_policy.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     8065 2023-08-30 09:49:20.000000 pogema-1.2.2/tests/test_grid.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4693 2023-08-30 09:49:20.000000 pogema-1.2.2/tests/test_integrations.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     9497 2023-08-30 09:49:20.000000 pogema-1.2.2/tests/test_pogema_env.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.374878 pogema-1.2.3a0/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1073 2023-08-30 09:49:20.000000 pogema-1.2.3a0/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 20:36:40.373587 pogema-1.2.3a0/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6472 2023-08-31 15:07:00.000000 pogema-1.2.3a0/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.355409 pogema-1.2.3a0/pogema/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      967 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4029 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/a_star_policy.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    23996 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/animation.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    16259 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/envs.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4800 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11642 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/grid.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     8150 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/grid_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3187 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/grid_registry.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.364682 pogema-1.2.3a0/pogema/integrations/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2522 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/make_pogema.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2607 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/pettingzoo.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2603 2024-04-13 20:35:39.000000 pogema-1.2.3a0/pogema/integrations/pymarl.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      936 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/sample_factory.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1975 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/svg_objects.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3254 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.367926 pogema-1.2.3a0/pogema/wrappers/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3912 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/metrics.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      656 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/multi_time_limit.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3080 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/persistence.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.373016 pogema-1.2.3a0/pogema.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      817 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       65 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        7 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-13 20:36:40.375004 pogema-1.2.3a0/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1409 2023-08-30 09:49:20.000000 pogema-1.2.3a0/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.372093 pogema-1.2.3a0/tests/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     7234 2023-08-31 15:07:00.000000 pogema-1.2.3a0/tests/test_deterministic_policy.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     8065 2023-11-28 11:12:00.000000 pogema-1.2.3a0/tests/test_grid.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4693 2023-08-30 09:49:20.000000 pogema-1.2.3a0/tests/test_integrations.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     9497 2023-08-30 09:49:20.000000 pogema-1.2.3a0/tests/test_pogema_env.py
```

### Comparing `pogema-1.2.2/LICENSE` & `pogema-1.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/PKG-INFO` & `pogema-1.2.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema
-Version: 1.2.2
+Version: 1.2.3a0
 Summary: Partially Observable Grid Environment for Multiple Agents
 Home-page: https://github.com/AIRI-Institute/pogema
 Author: Alexey Skrynnik
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-1.2.2/README.md` & `pogema-1.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/__init__.py` & `pogema-1.2.3a0/pogema/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pogema.a_star_policy import AStarAgent, BatchAStarAgent
 
 from pogema.grid_config import Easy8x8, Normal8x8, Hard8x8, ExtraHard8x8
 from pogema.grid_config import Easy16x16, Normal16x16, Hard16x16, ExtraHard16x16
 from pogema.grid_config import Easy32x32, Normal32x32, Hard32x32, ExtraHard32x32
 from pogema.grid_config import Easy64x64, Normal64x64, Hard64x64, ExtraHard64x64
 
-__version__ = '1.2.2'
+__version__ = '1.2.3a0'
 
 __all__ = [
     'GridConfig',
     'pogema_v0',
     'AStarAgent', 'BatchAStarAgent',
     'Easy8x8', 'Normal8x8', 'Hard8x8', 'ExtraHard8x8',
     'Easy16x16', 'Normal16x16', 'Hard16x16', 'ExtraHard16x16',
```

### Comparing `pogema-1.2.2/pogema/a_star_policy.py` & `pogema-1.2.3a0/pogema/a_star_policy.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/animation.py` & `pogema-1.2.3a0/pogema/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,164 +1,114 @@
+import math
 import os
 import typing
+from dataclasses import dataclass
 from itertools import cycle
 from gymnasium import logger, Wrapper
 
-from pydantic import BaseModel
-
-from pogema import GridConfig, pogema_v0
+from pogema import GridConfig, pogema_v0, BatchAStarAgent
+from pogema.svg_objects import Line, RectangleHref, Animation, Circle, Rectangle
 from pogema.grid import Grid
 from pogema.wrappers.persistence import PersistentWrapper, AgentState
 
 
-class AnimationSettings(BaseModel):
+@dataclass
+class AnimationSettings:
     """
     Settings for the animation.
     """
     r: int = 35
     stroke_width: int = 10
     scale_size: int = 100
-    time_scale: float = 0.28
+    time_scale: float = 0.25
     draw_start: int = 100
     rx: int = 15
 
     obstacle_color: str = '#84A1AE'
     ego_color: str = '#c1433c'
-    ego_other_color: str = '#72D5C8'
+    ego_other_color: str = '#6e81af'
     shaded_opacity: float = 0.2
     egocentric_shaded: bool = True
     stroke_dasharray: int = 25
 
-    colors: list = [
+    colors: tuple = (
         '#c1433c',
         '#2e6f9e',
         '#6e81af',
         '#00b9c8',
         '#72D5C8',
         '#0ea08c',
         '#8F7B66',
-    ]
+    )
 
 
-class AnimationConfig(BaseModel):
+@dataclass
+class AnimationConfig:
     """
     Configuration for the animation.
     """
     directory: str = 'renders/'
     static: bool = False
     show_agents: bool = True
     egocentric_idx: typing.Optional[int] = None
     uid: typing.Optional[str] = None
     save_every_idx_episode: typing.Optional[int] = 1
-    show_border: bool = True
-    show_lines: bool = False
+    show_lines: bool = True
 
 
-class GridHolder(BaseModel):
+@dataclass
+class GridHolder:
     """
     Holds the grid and the history.
     """
     obstacles: typing.Any = None
     episode_length: int = None
     height: int = None
     width: int = None
     colors: dict = None
     history: list = None
 
 
-class SvgObject:
-    """
-    Main class for the SVG.
-    """
-    tag = None
-
-    def __init__(self, **kwargs):
-        self.attributes = kwargs
-        self.animations = []
-
-    def add_animation(self, animation):
-        self.animations.append(animation)
-
-    @staticmethod
-    def render_attributes(attributes):
-        result = " ".join([f'{x.replace("_", "-")}="{y}"' for x, y in sorted(attributes.items())])
-        return result
-
-    def render(self):
-        animations = '\n'.join([a.render() for a in self.animations]) if self.animations else None
-        if animations:
-            return f"<{self.tag} {self.render_attributes(self.attributes)}> {animations} </{self.tag}>"
-        return f"<{self.tag} {self.render_attributes(self.attributes)} />"
-
-
-class Rectangle(SvgObject):
-    """
-    Rectangle class for the SVG.
-    """
-    tag = 'rect'
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.attributes['y'] = -self.attributes['y'] - self.attributes['height']
-
-
-class Circle(SvgObject):
-    """
-    Circle class for the SVG.
-    """
-    tag = 'circle'
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.attributes['cy'] = -self.attributes['cy']
-
-
-class Line(SvgObject):
-    """
-    Line class for the SVG.
-    """
-    tag = 'line'
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.attributes['y1'] = -self.attributes['y1']
-        self.attributes['y2'] = -self.attributes['y2']
-
-
-class Animation(SvgObject):
-    """
-    Animation class for the SVG.
-    """
-    tag = 'animate'
-
-    def render(self):
-        return f"<{self.tag} {self.render_attributes(self.attributes)}/>"
-
-
 class Drawing:
     """
     Drawing, analog of the DrawSvg class in the pogema package.
     """
 
-    def __init__(self, height, width, display_inline=False, origin=(0, 0)):
+    def __init__(self, height, width, svg_settings, display_inline=False, origin=(0, 0)):
         self.height = height
         self.width = width
         self.display_inline = display_inline
         self.origin = origin
         self.elements = []
+        self.svg_settings = svg_settings
 
     def add_element(self, element):
         self.elements.append(element)
 
     def render(self):
         view_box = (0, -self.height, self.width, self.height)
+        width = self.width
+        height = self.height
+        t = max(height, width) / 512
+        width = math.ceil(width / t)
+        height = math.ceil(height / t)
+
         results = [f'''<?xml version="1.0" encoding="UTF-8"?>
         <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
-             width="{self.width // 10}" height="{self.height // 10}" viewBox="{" ".join(map(str, view_box))}">''',
-                   '\n<defs>\n', '</defs>\n']
+             width="{width}" height="{height}" viewBox="{" ".join(map(str, view_box))}">''',
+                   '\n<defs>\n',
+                   f'<rect id="obstacle" width="{self.svg_settings.r * 2}" height="{self.svg_settings.r * 2}" fill="{self.svg_settings.obstacle_color}" rx="{self.svg_settings.rx}"/>',
+                   '',
+                   '<style>',
+                   '.line {' + f'stroke: {self.svg_settings.obstacle_color}; stroke-width: {self.svg_settings.stroke_width};' + '}',
+                   '.agent {' + f'r: {self.svg_settings.r}' + '}',
+                   '.target {' + f'fill: none; stroke-width: {self.svg_settings.stroke_width}; r: {self.svg_settings.r}' + '}',
+                   # '.rect { fill: #84A1AE; rx: 15;}',
+                   '</style>',
+                   '</defs>\n']
         for element in self.elements:
             results.append(element.render())
         results.append('</svg>')
         return "\n".join(results)
 
 
 class AnimationMonitor(Wrapper):
@@ -281,73 +231,57 @@
                         obstacles=grid.obstacles,
                         colors=agents_colors,
                         episode_length=episode_length,
                         history=decompressed_history, )
 
         render_width, render_height = gh.height * cfg.scale_size + cfg.scale_size, gh.width * cfg.scale_size + cfg.scale_size
 
-        drawing = Drawing(width=render_width, height=render_height, display_inline=False, origin=(0, 0))
+        drawing = Drawing(width=render_width, height=render_height, svg_settings=self.svg_settings)
         obstacles = self.create_obstacles(gh, anim_cfg)
 
         agents = []
         targets = []
 
         if anim_cfg.show_agents:
             agents = self.create_agents(gh, anim_cfg)
             targets = self.create_targets(gh, anim_cfg)
 
             if not anim_cfg.static:
                 self.animate_agents(agents, anim_cfg.egocentric_idx, gh)
                 self.animate_targets(targets, gh, anim_cfg)
         if anim_cfg.show_lines:
-            grid_lines = self.create_grid_lines(gh, anim_cfg, render_width, render_height)
+            grid_lines = self.create_grid_lines(gh, render_width, render_height)
             for line in grid_lines:
                 drawing.add_element(line)
         for obj in [*obstacles, *agents, *targets, ]:
             drawing.add_element(obj)
 
         if anim_cfg.egocentric_idx is not None:
             field_of_view = self.create_field_of_view(grid_holder=gh, animation_config=anim_cfg)
             if not anim_cfg.static:
                 self.animate_obstacles(obstacles=obstacles, grid_holder=gh, animation_config=anim_cfg)
                 self.animate_field_of_view(field_of_view, anim_cfg.egocentric_idx, gh)
             drawing.add_element(field_of_view)
 
         return drawing
 
-    def create_grid_lines(self, grid_holder: GridHolder, animation_config: AnimationConfig, render_width,
-                          render_height):
-        """
-        Creates the grid lines.
-        :param grid_holder: grid holder
-        :param animation_config: animation configuration
-        :return: grid_lines: list of grid lines
-        """
-        cfg = self.svg_settings
+    def create_grid_lines(self, grid_holder: GridHolder, render_width, render_height):
+        cfg, r = self.svg_settings, self.grid_config.obs_radius
+        offset = (r - 1) * cfg.scale_size
+        stroke_settings = {'class': 'line'}
         grid_lines = []
-        for i in range(-1, grid_holder.height + 1):
-            # vertical lines
-            x0 = x1 = i * cfg.scale_size + cfg.scale_size / 2
-            y0 = 0
-            y1 = render_height
-            grid_lines.append(
-                Line(x1=x0, y1=y0, x2=x1, y2=y1, stroke=cfg.obstacle_color, stroke_width=cfg.stroke_width // 1.5))
-        for i in range(-1, grid_holder.width + 1):
-            # continue
-            # horizontal lines
-            x0 = 0
-            y0 = y1 = i * cfg.scale_size + cfg.scale_size / 2
-            x1 = render_width
-            grid_lines.append(
-                Line(x1=x0, y1=y0, x2=x1, y2=y1, stroke=cfg.obstacle_color, stroke_width=cfg.stroke_width // 1.5))
-
-        # for i in range(grid_holder.width):
-        #     grid_lines.append(Line(start=(0, i * cfg.scale_size),
-        #                            end=(grid_holder.height * cfg.scale_size, i * cfg.scale_size),
-        #                            stroke=cfg.grid_color, stroke_width=cfg.grid_width))
+
+        for i in range(-1 + r, grid_holder.height + 2 - r):
+            x = i * cfg.scale_size + cfg.scale_size / 2
+            grid_lines.append(Line(x1=x, y1=offset, x2=x, y2=render_height - offset, **stroke_settings))
+
+        for i in range(-1 + r, grid_holder.width + 2 - r):
+            y = i * cfg.scale_size + cfg.scale_size / 2
+            grid_lines.append(Line(x1=offset, y1=y, x2=render_width - offset, y2=y, **stroke_settings))
+
         return grid_lines
 
     def save_animation(self, name='render.svg', animation_config: typing.Optional[AnimationConfig] = None):
         """
         Saves the animation.
         :param name: name of the file
         :param animation_config: animation configuration
@@ -355,34 +289,18 @@
         """
         animation = self.create_animation(animation_config)
         with open(name, "w") as f:
             f.write(animation.render())
 
     @staticmethod
     def fix_point(x, y, length):
-        """
-        Fixes the point to the grid.
-        :param x: coordinate x
-        :param y: coordinate y
-        :param length: size of the grid
-        :return: x, y: fixed coordinates
-        """
         return length - y - 1, x
 
     @staticmethod
     def check_in_radius(x1, y1, x2, y2, r) -> bool:
-        """
-        Checks if the point is in the radius.
-        :param x1: coordinate x1
-        :param y1: coordinate y1
-        :param x2: coordinate x2
-        :param y2: coordinate y2
-        :param r: radius
-        :return:
-        """
         return x2 - r <= x1 <= x2 + r and y2 - r <= y1 <= y2 + r
 
     def create_field_of_view(self, grid_holder, animation_config):
         """
         Creates the field of view for the egocentric agent.
         :param grid_holder:
         :param animation_config:
@@ -448,15 +366,15 @@
             for agent_state in gh.history[agent_idx]:
                 x, y = agent_state.get_xy()
 
                 x_path.append(str(cfg.draw_start + y * cfg.scale_size))
                 y_path.append(str(-cfg.draw_start + -(gh.width - x - 1) * cfg.scale_size))
 
                 if egocentric_idx is not None:
-                    ego_x, ego_y = agent_state.get_xy()
+                    ego_x, ego_y = gh.history[egocentric_idx][idx].get_xy()
                     if self.check_in_radius(x, y, ego_x, ego_y, self.grid_config.obs_radius):
                         opacity.append('1.0')
                     else:
                         opacity.append(str(cfg.shaded_opacity))
 
             visibility = ['visible' if state.is_active() else 'hidden' for state in gh.history[agent_idx]]
 
@@ -567,37 +485,33 @@
         :param animation_config:
         :return:
         """
         gh = grid_holder
         cfg = self.svg_settings
 
         result = []
-        r = self.grid_config.obs_radius
+
         for i in range(gh.height):
             for j in range(gh.width):
                 x, y = self.fix_point(i, j, gh.width)
-                if not animation_config.show_border:
-                    if i == r - 1 or j == r - 1 or j == gh.width - r or i == gh.height - r:
-                        continue
+
                 if gh.obstacles[x][y] != self.grid_config.FREE:
                     obs_settings = {}
                     obs_settings.update(x=cfg.draw_start + i * cfg.scale_size - cfg.r,
                                         y=cfg.draw_start + j * cfg.scale_size - cfg.r,
-                                        width=cfg.r * 2,
                                         height=cfg.r * 2,
-                                        rx=cfg.rx,
-                                        fill=self.svg_settings.obstacle_color)
+                                        )
 
                     if animation_config.egocentric_idx is not None and cfg.egocentric_shaded:
                         initial_positions = [agent_states[0].get_xy() for agent_states in gh.history]
                         ego_x, ego_y = initial_positions[animation_config.egocentric_idx]
                         if not self.check_in_radius(x, y, ego_x, ego_y, self.grid_config.obs_radius):
                             obs_settings.update(opacity=cfg.shaded_opacity)
 
-                    result.append(Rectangle(**obs_settings))
+                    result.append(RectangleHref(**obs_settings))
 
         return result
 
     def animate_obstacles(self, obstacles, grid_holder, animation_config):
         """
 
         :param obstacles:
@@ -627,45 +541,37 @@
 
                 obstacle = obstacles[obstacle_idx]
                 obstacle.add_animation(self.compressed_anim('opacity', opacity, cfg.time_scale))
 
                 obstacle_idx += 1
 
     def create_agents(self, grid_holder, animation_config):
-        """
-        Creates the agents.
-        :param grid_holder:
-        :param animation_config:
-        :return:
-        """
-        gh: GridHolder = grid_holder
-        cfg = self.svg_settings
-
+        initial_positions = [state[0].get_xy() for state in grid_holder.history if state[0].is_active()]
+        ego_idx = animation_config.egocentric_idx
         agents = []
-        initial_positions = [agent_states[0].get_xy() for agent_states in gh.history]
-        for idx, (x, y) in enumerate(initial_positions):
 
-            if not any([agent_state.is_active() for agent_state in gh.history[idx]]):
-                continue
+        for idx, (x, y) in enumerate(initial_positions):
+            circle_settings = {
+                'cx': self.svg_settings.draw_start + y * self.svg_settings.scale_size,
+                'cy': self.svg_settings.draw_start + (grid_holder.width - x - 1) * self.svg_settings.scale_size,
+                # 'r': self.svg_settings.r,
+                'fill': grid_holder.colors[idx],
+                'class': 'agent',
+            }
 
-            circle_settings = {}
-            circle_settings.update(cx=cfg.draw_start + y * cfg.scale_size,
-                                   cy=cfg.draw_start + (gh.width - x - 1) * cfg.scale_size,
-                                   r=cfg.r, fill=gh.colors[idx])
-            ego_idx = animation_config.egocentric_idx
             if ego_idx is not None:
                 ego_x, ego_y = initial_positions[ego_idx]
-                if not self.check_in_radius(x, y, ego_x, ego_y, self.grid_config.obs_radius) and cfg.egocentric_shaded:
-                    circle_settings.update(opacity=cfg.shaded_opacity)
-                if ego_idx == idx:
-                    circle_settings.update(fill=self.svg_settings.ego_color)
-                else:
-                    circle_settings.update(fill=self.svg_settings.ego_other_color)
-            agent = Circle(**circle_settings)
-            agents.append(agent)
+                is_out_of_radius = not self.check_in_radius(x, y, ego_x, ego_y, self.grid_config.obs_radius)
+                circle_settings['fill'] = self.svg_settings.ego_other_color
+                if idx == ego_idx:
+                    circle_settings['fill'] = self.svg_settings.ego_color
+                elif is_out_of_radius and self.svg_settings.egocentric_shaded:
+                    circle_settings['opacity'] = self.svg_settings.shaded_opacity
+
+            agents.append(Circle(**circle_settings))
 
         return agents
 
     def create_targets(self, grid_holder, animation_config):
         """
         Creates the targets.
         :param grid_holder:
@@ -679,39 +585,50 @@
 
             tx, ty = agent_states[0].get_target_xy()
             x, y = ty, gh.width - tx - 1
 
             if not any([agent_state.is_active() for agent_state in gh.history[agent_idx]]):
                 continue
 
-            circle_settings = {}
+            circle_settings = {"class": 'target'}
             circle_settings.update(cx=cfg.draw_start + x * cfg.scale_size,
                                    cy=cfg.draw_start + y * cfg.scale_size,
-                                   r=cfg.r,
-                                   stroke=gh.colors[agent_idx], stroke_width=cfg.stroke_width, fill='none')
+                                   # r=cfg.r,
+                                   stroke=gh.colors[agent_idx],
+                                   # stroke_width=cfg.stroke_width,
+                                   # fill='none'
+                                   )
             if animation_config.egocentric_idx is not None:
                 if animation_config.egocentric_idx != agent_idx:
                     continue
 
                 circle_settings.update(stroke=cfg.ego_color)
             target = Circle(**circle_settings)
             targets.append(target)
         return targets
 
 
 def main():
-    grid_config = GridConfig(size=8, num_agents=5, obs_radius=2, seed=9, on_target='finish', max_episode_steps=128)
+    grid = """
+    ...#.
+    .#...
+    .....
+    ##.#.
+    """
+    grid_config = GridConfig(size=32, num_agents=2, obs_radius=2, seed=9, on_target='restart', max_episode_steps=16,
+                             density=0.1, map=grid, observation_type="POMAPF")
     env = pogema_v0(grid_config=grid_config)
     env = AnimationMonitor(env)
 
-    env.reset()
-    done = [False]
+    obs, _ = env.reset()
+    truncated = terminated = [False]
 
-    while not all(done):
-        _, _, done, _ = env.step(env.sample_actions())
+    agent = BatchAStarAgent()
+    while not all(terminated) and not all(truncated):
+        obs, _, terminated, truncated, _ = env.step(agent.act(obs))
 
     env.save_animation('out-static.svg', AnimationConfig(static=True, save_every_idx_episode=None))
     env.save_animation('out-static-ego.svg', AnimationConfig(egocentric_idx=0, static=True))
     env.save_animation('out-static-no-agents.svg', AnimationConfig(show_agents=False, static=True))
     env.save_animation("out.svg")
     env.save_animation("out-ego.svg", AnimationConfig(egocentric_idx=0))
```

### Comparing `pogema-1.2.2/pogema/envs.py` & `pogema-1.2.3a0/pogema/envs.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/generator.py` & `pogema-1.2.3a0/pogema/generator.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/grid.py` & `pogema-1.2.3a0/pogema/grid.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/grid_config.py` & `pogema-1.2.3a0/pogema/grid_config.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/grid_registry.py` & `pogema-1.2.3a0/pogema/grid_registry.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/integrations/make_pogema.py` & `pogema-1.2.3a0/pogema/integrations/make_pogema.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/integrations/pettingzoo.py` & `pogema-1.2.3a0/pogema/integrations/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/integrations/pymarl.py` & `pogema-1.2.3a0/pogema/integrations/pymarl.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         return self
 
     def step(self, actions):
         self._observations, rewards, terminated, truncated, infos = self.env.step(actions)
         info = {}
         done = all(terminated) or all(truncated)
         if done:
-            info.update(CSR=infos[0]['metrics']['CSR'])
-            info.update(ISR=infos[0]['metrics']['ISR'])
-
+            for key, value in infos[0]['metrics'].items():
+                info[key] = value
+            
         return sum(rewards), done, info
 
     def get_obs(self):
         return np.array([self.get_obs_agent(agent_id) for agent_id in range(self.n_agents)])
 
     def get_obs_agent(self, agent_id):
         return np.array(self._observations[agent_id]).flatten()
```

### Comparing `pogema-1.2.2/pogema/integrations/sample_factory.py` & `pogema-1.2.3a0/pogema/integrations/sample_factory.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/utils.py` & `pogema-1.2.3a0/pogema/utils.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/wrappers/metrics.py` & `pogema-1.2.3a0/pogema/wrappers/metrics.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/wrappers/multi_time_limit.py` & `pogema-1.2.3a0/pogema/wrappers/multi_time_limit.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema/wrappers/persistence.py` & `pogema-1.2.3a0/pogema/wrappers/persistence.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/pogema.egg-info/PKG-INFO` & `pogema-1.2.3a0/pogema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema
-Version: 1.2.2
+Version: 1.2.3a0
 Summary: Partially Observable Grid Environment for Multiple Agents
 Home-page: https://github.com/AIRI-Institute/pogema
 Author: Alexey Skrynnik
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-1.2.2/pogema.egg-info/SOURCES.txt` & `pogema-1.2.3a0/pogema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ./pogema/a_star_policy.py
 ./pogema/animation.py
 ./pogema/envs.py
 ./pogema/generator.py
 ./pogema/grid.py
 ./pogema/grid_config.py
 ./pogema/grid_registry.py
+./pogema/svg_objects.py
 ./pogema/utils.py
 ./pogema.egg-info/PKG-INFO
 ./pogema.egg-info/SOURCES.txt
 ./pogema.egg-info/dependency_links.txt
 ./pogema.egg-info/requires.txt
 ./pogema.egg-info/top_level.txt
 ./pogema/integrations/__init__.py
```

### Comparing `pogema-1.2.2/setup.py` & `pogema-1.2.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/tests/test_deterministic_policy.py` & `pogema-1.2.3a0/tests/test_deterministic_policy.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/tests/test_grid.py` & `pogema-1.2.3a0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/tests/test_integrations.py` & `pogema-1.2.3a0/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.2/tests/test_pogema_env.py` & `pogema-1.2.3a0/tests/test_pogema_env.py`

 * *Files identical despite different names*

