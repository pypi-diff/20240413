# Comparing `tmp/curvey-0.0.2.tar.gz` & `tmp/curvey-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  2 21:23:34 2024, max compression
+gzip compressed data, last modified: Sat Apr 13 14:04:30 2024, max compression
```

## Comparing `curvey-0.0.2.tar` & `curvey-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,57 @@
--rw-r--r--   0        0        0     1102 2024-04-02 21:23:34.000000 curvey-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      335 2024-04-02 21:23:34.000000 curvey-0.0.2/environment.yml
--rw-r--r--   0        0        0     3023 2024-04-02 21:23:34.000000 curvey-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0       47 2024-04-02 21:23:34.000000 curvey-0.0.2/requirements.txt
--rw-r--r--   0        0        0      588 2024-04-02 21:23:34.000000 curvey-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      801 2024-04-02 21:23:34.000000 curvey-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1203 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/bibliography.md
--rw-r--r--   0        0        0      358 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/index.md
--rw-r--r--   0        0        0       36 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/blend.md
--rw-r--r--   0        0        0     3177 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/curve.md
--rw-r--r--   0        0        0       38 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/curves.md
--rw-r--r--   0        0        0       34 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/flow.md
--rw-r--r--   0        0        0      410 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/index.md
--rw-r--r--   0        0        0       69 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/shape_structure_dataset.md
--rw-r--r--   0        0        0       18 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/util.md
--rw-r--r--   0        0        0      308 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/javascripts/katex.js
--rw-r--r--   0        0        0      384 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0     9221 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/blend.ipynb
--rw-r--r--   0        0        0    10269 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/flow.ipynb
--rw-r--r--   0        0        0      625 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/index.md
--rw-r--r--   0        0        0    10970 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/introduction.ipynb
--rw-r--r--   0        0        0     3307 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/shape_structure_dataset.ipynb
--rw-r--r--   0        0        0      296 2024-04-02 21:23:34.000000 curvey-0.0.2/src/conftest.py
--rw-r--r--   0        0        0      119 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/__init__.py
--rw-r--r--   0        0        0    12306 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/blend.py
--rw-r--r--   0        0        0    54814 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/curve.py
--rw-r--r--   0        0        0    20807 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/curves.py
--rw-r--r--   0        0        0    27476 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/flow.py
--rw-r--r--   0        0        0     6498 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/plot.py
--rw-r--r--   0        0        0        0 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/py.typed
--rw-r--r--   0        0        0     5633 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/shape_structure_dataset.py
--rw-r--r--   0        0        0     5818 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/util.py
--rw-r--r--   0        0        0    23917 2024-04-02 21:23:34.000000 curvey-0.0.2/static/curv_interp.png
--rw-r--r--   0        0        0    39468 2024-04-02 21:23:34.000000 curvey-0.0.2/static/curve_plot.png
--rw-r--r--   0        0        0    40234 2024-04-02 21:23:34.000000 curvey-0.0.2/static/willmore_flow.png
--rw-r--r--   0        0        0     1164 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_blend.py
--rw-r--r--   0        0        0     6207 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_curve.py
--rw-r--r--   0        0        0      968 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_curves.py
--rw-r--r--   0        0        0     1092 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_flow.py
--rw-r--r--   0        0        0      739 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_shape_structure_dataset.py
--rw-r--r--   0        0        0       62 2024-04-02 21:23:34.000000 curvey-0.0.2/.gitignore
--rw-r--r--   0        0        0     7651 2024-04-02 21:23:34.000000 curvey-0.0.2/LICENSE
--rw-r--r--   0        0        0     1105 2024-04-02 21:23:34.000000 curvey-0.0.2/README.md
--rw-r--r--   0        0        0     3555 2024-04-02 21:23:34.000000 curvey-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    12089 2024-04-02 21:23:34.000000 curvey-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-13 14:04:30.000000 curvey-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      335 2024-04-13 14:04:30.000000 curvey-0.0.3/environment.yml
+-rw-r--r--   0        0        0     3197 2024-04-13 14:04:30.000000 curvey-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0       47 2024-04-13 14:04:30.000000 curvey-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      588 2024-04-13 14:04:30.000000 curvey-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      801 2024-04-13 14:04:30.000000 curvey-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1615 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/bibliography.md
+-rw-r--r--   0        0        0      358 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/index.md
+-rw-r--r--   0        0        0       36 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/blend.md
+-rw-r--r--   0        0        0     3288 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/curve.md
+-rw-r--r--   0        0        0       38 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/curves.md
+-rw-r--r--   0        0        0       36 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/edges.md
+-rw-r--r--   0        0        0       34 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/flow.md
+-rw-r--r--   0        0        0      578 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/index.md
+-rw-r--r--   0        0        0       40 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/polygon.md
+-rw-r--r--   0        0        0       69 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/shape_structure_dataset.md
+-rw-r--r--   0        0        0       52 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/triangulation.md
+-rw-r--r--   0        0        0       18 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/util.md
+-rw-r--r--   0        0        0      308 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/javascripts/katex.js
+-rw-r--r--   0        0        0      384 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0     9221 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/blend.ipynb
+-rw-r--r--   0        0        0    10269 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/flow.ipynb
+-rw-r--r--   0        0        0      794 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/index.md
+-rw-r--r--   0        0        0    10970 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/introduction.ipynb
+-rw-r--r--   0        0        0     9638 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/polygon.ipynb
+-rw-r--r--   0        0        0     3307 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/shape_structure_dataset.ipynb
+-rw-r--r--   0        0        0      296 2024-04-13 14:04:30.000000 curvey-0.0.3/src/conftest.py
+-rw-r--r--   0        0        0      193 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/_typing.py
+-rw-r--r--   0        0        0    11191 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/approx_medial_axis.py
+-rw-r--r--   0        0        0    12306 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/blend.py
+-rw-r--r--   0        0        0    54874 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/curve.py
+-rw-r--r--   0        0        0    20807 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/curves.py
+-rw-r--r--   0        0        0    16366 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/edges.py
+-rw-r--r--   0        0        0    27476 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/flow.py
+-rw-r--r--   0        0        0     7913 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/plot.py
+-rw-r--r--   0        0        0    12657 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/polygon.py
+-rw-r--r--   0        0        0        0 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/py.typed
+-rw-r--r--   0        0        0     5136 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/shape_structure_dataset.py
+-rw-r--r--   0        0        0     5651 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/triangulation.py
+-rw-r--r--   0        0        0     5818 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/util.py
+-rw-r--r--   0        0        0    28332 2024-04-13 14:04:30.000000 curvey-0.0.3/static/ama.png
+-rw-r--r--   0        0        0    23917 2024-04-13 14:04:30.000000 curvey-0.0.3/static/curv_interp.png
+-rw-r--r--   0        0        0    39468 2024-04-13 14:04:30.000000 curvey-0.0.3/static/curve_plot.png
+-rw-r--r--   0        0        0    40234 2024-04-13 14:04:30.000000 curvey-0.0.3/static/willmore_flow.png
+-rw-r--r--   0        0        0     1164 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_blend.py
+-rw-r--r--   0        0        0     6218 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_curve.py
+-rw-r--r--   0        0        0      968 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_curves.py
+-rw-r--r--   0        0        0     1211 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_edges.py
+-rw-r--r--   0        0        0     1092 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_flow.py
+-rw-r--r--   0        0        0      851 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_shape_structure_dataset.py
+-rw-r--r--   0        0        0     1352 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_triangulation.py
+-rw-r--r--   0        0        0       62 2024-04-13 14:04:30.000000 curvey-0.0.3/.gitignore
+-rw-r--r--   0        0        0     7651 2024-04-13 14:04:30.000000 curvey-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1415 2024-04-13 14:04:30.000000 curvey-0.0.3/README.md
+-rw-r--r--   0        0        0     3587 2024-04-13 14:04:30.000000 curvey-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    12447 2024-04-13 14:04:30.000000 curvey-0.0.3/PKG-INFO
```

### Comparing `curvey-0.0.2/.pre-commit-config.yaml` & `curvey-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/mkdocs.yml` & `curvey-0.0.3/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 repo_url: https://github.com/darikg/curvey
 
 nav:
   - Home: index.md
   - Tutorials:
     - tutorial/index.md
     - Introduction: tutorial/introduction.ipynb
+    - Polygons, triangulations, and the medial axis: tutorial/polygon.ipynb
     - Shape structure dataset: tutorial/shape_structure_dataset.ipynb
     - Flows: tutorial/flow.ipynb
     - Blends: tutorial/blend.ipynb
   - API:
     - api/index.md
+    - Blend: api/blend.md
     - Curve: api/curve.md
     - Curves: api/curves.md
+    - Edges: api/edges.md
     - Flow: api/flow.md
-    - Blend: api/blend.md
+    - Polygon: api/polygon.md
     - Shape structure dataset: api/shape_structure_dataset.md
+    - Triangulation: api/triangulation.md
     - Util: api/util.md
   - Bibliography: bibliography.md
 
 # TO tweak notebook widths
 # https://squidfunk.github.io/mkdocs-material/customization/#overriding-template-blocks
 # See https://pypi.org/project/mkdocs-jupyter/
 # Adjusting width https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#content-area-width
```

### Comparing `curvey-0.0.2/.github/workflows/release.yml` & `curvey-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/.github/workflows/test.yml` & `curvey-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/docs/bibliography.md` & `curvey-0.0.3/docs/bibliography.md`

 * *Files 20% similar despite different names*

```diff
@@ -14,7 +14,13 @@
 http://sibgrapi.sid.inpe.br/col/sid.inpe.br/sibgrapi/2017/09.04.18.39/doc/Mean%20Curvature%20Flow%20and%20Applications.pdf)
 
   - [*Robust Fairing via Conformal Curvature Flow.* Keenan Crane, Ulrich Pinkall, and Peter Schröder. 2014](
 https://www.cs.cmu.edu/~kmcrane/Projects/ConformalWillmoreFlow/paper.pdf)
 
   - [*Rapid blending of closed curves based on curvature flow.* Masahiro Hirano, Yoshihiro Watanabe, and
 Masatoshi Ishikawa. 2017.](https://www.sciencedirect.com/science/article/pii/S016783961730016X)
+
+  - [*Efficient and Robust Computation of an Approximated Medial Axis.* Yuandong Yang, Oliver Brock, and Robert
+N. Moll. 2004.](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=cfc187181ce85d983843c4a184651dbd2a07e7e5)
+
+  - [Triangle: Engineering a 2D Quality Mesh Generator and Delaunay Triangulator.* Jonathan Richard Shewchuk. 1996.](
+https://people.eecs.berkeley.edu/~jrs/papers/triangle.pdf)
```

### Comparing `curvey-0.0.2/docs/api/curve.md` & `curvey-0.0.3/docs/api/curve.md`

 * *Files 6% similar despite different names*

```diff
@@ -94,11 +94,14 @@
 ### ::: curvey.curve.Curve.plot_vectors
 
 ## Special
 ### ::: curvey.curve.Curve.check_same_n_vertices
 ### ::: curvey.curve.Curve.deriv
 ### ::: curvey.curve.Curve.edge_intersections
 ### ::: curvey.curve.Curve.interpolator
+### ::: curvey.curve.Curve.to_edges
 
-## Library interface
+## Type conversion
 ### ::: curvey.curve.Curve.from_shapely
+### ::: curvey.curve.Curve.to_edges
+### ::: curvey.curve.Curve.to_matplotlib
 ### ::: curvey.curve.Curve.to_shapely
```

### Comparing `curvey-0.0.2/docs/tutorial/blend.ipynb` & `curvey-0.0.3/docs/tutorial/blend.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/docs/tutorial/flow.ipynb` & `curvey-0.0.3/docs/tutorial/flow.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/docs/tutorial/introduction.ipynb` & `curvey-0.0.3/docs/tutorial/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/docs/tutorial/shape_structure_dataset.ipynb` & `curvey-0.0.3/docs/tutorial/shape_structure_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/src/curvey/blend.py` & `curvey-0.0.3/src/curvey/blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/src/curvey/curve.py` & `curvey-0.0.3/src/curvey/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """A curve"""
 
 from __future__ import annotations
 
-import collections.abc
 import itertools
 import warnings
 from collections.abc import Sequence
 from functools import cached_property
 from types import MappingProxyType
 from typing import Any, Callable, Literal, NamedTuple, cast, overload
 
+import matplotlib.path
 import numpy as np
 import scipy
 import shapely
 import sortedcontainers
 from matplotlib.axes import Axes
 from matplotlib.collections import LineCollection, PathCollection
 from matplotlib.lines import Line2D
@@ -45,17 +45,18 @@
     sin,
     sqrt,
     stack,
     where,
     zeros,
 )
 from numpy.linalg import norm
-from numpy.typing import ArrayLike
 from typing_extensions import Self
 
+from ._typing import PointsLike
+from .edges import Edges
 from .plot import _get_ax, _VariableColorSpec, quiver, segments
 from .util import (
     InterpType,
     _rescale,
     align_edges,
     angle_to_points,
     periodic_interpolator,
@@ -74,15 +75,15 @@
 
     **kwargs
         Metadata parameters in key=value format.
     """
 
     def __init__(
         self,
-        pts: ndarray | Sequence[Sequence[float] | tuple[float, float]] | ArrayLike,
+        pts: PointsLike,
         _data: dict[str, Any] | None = None,
         **kwargs,
     ):
         # Use `asanyarray` here to allow the user to pass in whatever they want as long as it obeys
         # the numpy array protocol; in particular thinking of arrays of dual numbers for automatic
         # differentiation
         pts = asanyarray(pts)
@@ -583,15 +584,15 @@
 
     def to_orientation(self, orientation: int) -> Curve:
         """A curve with the specified orientation
 
         Parameters
         ----------
         orientation
-            Must be either 1 or -1.
+            Must be either `+1` or `-1`. `+1' is counterclockwise.
         """
         if orientation not in (1, -1):
             msg = f"orientation must be either 1 or -1, got {orientation}"
             raise ValueError(msg)
 
         return self.reverse() if self.orientation != orientation else self
 
@@ -864,37 +865,24 @@
         : matplotlib.quiver.Quiver
             If `directed` is True.
 
         : matplotlib.collections.LineCollection
             If `directed` is False.
         """
 
-        if directed:
-            if isinstance(width, (collections.abc.Sequence, ndarray)):
-                msg = (
-                    "`width` was supplied as a sequence but "
-                    "matplotlib.pyplot.Quiver doesn't support scaling individual arrows. "
-                    "Use directed=False to scale edge width."
-                )
-                raise ValueError(msg)
-
-            return quiver(
-                points=self._pts,
-                vectors=self.edge,
-                color=color,
-                ax=ax,
-                **kwargs,
-            )
+        if color is None:
+            color = self.cum_edge_length
 
         return segments(
             points=self._pts,
             edges=self.edges,
             color=color,
             width=width,
             scale_width=scale_width,
+            directed=directed,
             ax=ax,
             **kwargs,
         )
 
     def plot_vectors(
         self,
         vectors: ndarray | None = None,
@@ -1135,22 +1123,22 @@
                 prev=(i - 1) % self.n,
                 next=(i + 1) % self.n,
                 edge_length=edge_length,
             )
             for i, edge_length in enumerate(self.edge_length)
         }
 
-        # Priority queue by edge length
+        # Priority queue by edge length (shortest last)
         queue = sortedcontainers.SortedSet(verts.values(), key=lambda v: -v.edge_length)
 
         for n_removed in itertools.count(1):
             shortest = queue.pop(-1)
             del verts[shortest.idx]
 
-            if (n_removed == n) or (queue[-1] >= min_edge_length):
+            if (n_removed == n) or (queue[-1].edge_length >= min_edge_length):
                 break
 
             # Remove previous and next vertices so we can update them
             queue.discard(v_prev := verts[shortest.prev])
             queue.discard(v_next := verts[shortest.next])
             updated_prev_edge_length = norm(self._pts[v_next.idx] - self._pts[v_prev.idx])
 
@@ -1214,14 +1202,18 @@
         pts = array(ring.coords)
         if array_equal(pts[0], pts[-1]):
             # Shapely likes to explicitly close points
             pts = pts[:-1]
 
         return cls(pts)
 
+    def to_edges(self) -> Edges:
+        """Representation of the curve as an 'edge soup' in `curvey.edge.Edges` format"""
+        return Edges(points=self.points, edges=self.edges)
+
     @classmethod
     def from_curvature(
         cls,
         curvature: ndarray,
         edge_lengths: ndarray,
         solve_vertices: bool = True,
         theta0: float | None = None,
@@ -1642,14 +1634,24 @@
         )
         if not opt.success:
             msg = "Optimization failed: " + opt.message
             warnings.warn(msg, OptimizationFailed, stacklevel=2)
 
         return self.with_points(_resample(opt.x)._pts)
 
+    def to_matplotlib(self) -> matplotlib.path.Path:
+        """Convert to a `matplotlib.path.Path` object"""
+        from matplotlib.path import Path
+
+        pts = self.closed_points
+        codes = np.full(self.n + 1, Path.LINETO)
+        codes[0] = Path.MOVETO
+        codes[-1] = Path.CLOSEPOLY
+        return Path(pts, codes)
+
 
 class NotEnoughPoints(Exception):
     """Raised if fewer than 3 points are passed to the `Curve` constructor"""
 
 
 class WrongDimensions(Exception):
     """Raised if the points array is not 2d"""
```

### Comparing `curvey-0.0.2/src/curvey/curves.py` & `curvey-0.0.3/src/curvey/curves.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/src/curvey/flow.py` & `curvey-0.0.3/src/curvey/flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/src/curvey/plot.py` & `curvey-0.0.3/src/curvey/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
+import collections
+from collections.abc import Iterable
 from typing import Any, NamedTuple, cast
 
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.collections import LineCollection
 from matplotlib.quiver import Quiver
+from matplotlib.text import Text
 from numpy import asarray, ndarray, newaxis
 from numpy.linalg import norm
 from numpy.typing import ArrayLike
 
 from curvey.util import _rescale
 
 
@@ -160,15 +163,15 @@
         **kwargs,
     )
 
 
 def segments(
     points: ndarray,
     edges: ndarray,
-    directed: bool = False,
+    directed: bool = True,
     color=None,
     width: float | ndarray | None = None,
     scale_width: tuple[float, float] | None = None,
     ax: Axes | None = None,
     **kwargs,
 ) -> LineCollection | Quiver:
     """Plot line segments supplied as separate points and edge arrays
@@ -178,15 +181,15 @@
     points
         `(m, 2)` array of vertex coordinates
 
     edges
         `(n, 2)` integer array of indices into `points` defining the start and end of each segment.
 
     directed
-        If true, plot as a quiver plot.
+        If true, plot as a quiver plot, otherwise a line plot.
 
     color
         The color to plot each edge. Can be a constant color or vector of length `n` specifying
         a color for each edge.
 
     width
         The thickness of each edge segment, scalar or edge quantity vector.
@@ -199,14 +202,22 @@
 
     **kwargs
         Aadditional kwargs passed to `matplotlib.collections.LineCollection`.
     """
     ax = _get_ax(ax)
 
     if directed:
+        if isinstance(width, (collections.abc.Sequence, ndarray)):
+            msg = (
+                "`width` was supplied as a sequence but "
+                "matplotlib.pyplot.Quiver doesn't support scaling individual arrows widths. "
+                "Use directed=False to scale edge width."
+            )
+            raise ValueError(msg)
+
         return quiver(
             points=points[edges[:, 0]],
             vectors=points[edges[:, 1]] - points[edges[:, 0]],
             color=color,
             ax=ax,
             width=width,
             **kwargs,
@@ -229,7 +240,50 @@
 
     ax.add_collection(lc)
 
     # Adding a line collection doesn't update limits so do it here
     ax.update_datalim(points)
     ax.autoscale_view()
     return lc
+
+
+def text(
+    points: ndarray,
+    labels: Iterable[str] | None = None,
+    clip: bool = True,
+    ax: Axes | None = None,
+    **kwargs,
+) -> list[Text]:
+    """Draw text at the points
+
+    Parameters
+    ----------
+    points
+        `(n, 2)` array of points.
+
+    labels
+        `(n,)` sequence of string labels. If not supplied, defaults to the indices
+        `0, 1, ..., n-1`.
+
+    clip
+        By default matplotlib doesn't restrict clip labels by axes limits -- it's the default here.
+
+    ax
+        Matplotlib axes to draw in. Defaults to current axes.
+
+    **kwargs
+        Remaining kwargs passed to `matplotlib.pyplot.text`.
+
+    """
+    ax = _get_ax(ax)
+    txts: list[Text] = []
+
+    if labels is None:
+        labels = (str(i) for i in range(len(points)))
+
+    for (x, y), label in zip(points, labels):
+        txt = ax.text(x, y, label, **kwargs)
+        txts.append(txt)
+        if clip:
+            txt.set_clip_on(True)
+
+    return txts
```

### Comparing `curvey-0.0.2/src/curvey/shape_structure_dataset.py` & `curvey-0.0.3/src/curvey/shape_structure_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 import re
 from collections.abc import Iterator
 from functools import cached_property
 from pathlib import Path
 from typing import TypedDict
 from zipfile import ZipFile
 
-from numpy import array, ndarray
+from numpy import array
 
 from .curve import Curve
+from .polygon import Polygon
+from .triangulation import Triangulation
 
 
 class _JsonPoint(TypedDict):
     x: float
     y: float
 
 
@@ -68,63 +70,51 @@
     """
 
     # regex to match e.g. 'Shapes/Bone-13.json'
     _shape_file_regex = re.compile(r"Shapes/([^.]+)\.json")
 
     def __init__(self, dataset: str | Path):
         self.dataset = ZipFile(Path(dataset).expanduser())
-        self.cache: dict[str, ndarray] = {}
+        self.cache: dict[str, Triangulation] = {}
 
-    def _load_json(self, name: str, idx: int | None = True) -> _JsonShape:
+    def _load_json(self, name: str, idx: int | None = None) -> _JsonShape:
         name = self._canonical_name(name, idx)
         shape_bytes = self.dataset.read(f"Shapes/{name}.json")
         return json.loads(shape_bytes)
 
-    def load_shape(
+    def load_triangulation(
         self,
         name: str,
         idx: int | None = None,
-        load_triangles: bool = True,
-    ) -> tuple[ndarray, ndarray | None]:
-        """A `(n_verts, 2)` array of points and a `(n_faces, 3)` array of triangles"""
-        data = self._load_json(name, idx)
-        pts = array([[d["x"], d["y"]] for d in data["points"]])
-        if load_triangles:
-            tris = array([[d["p1"], d["p2"], d["p3"]] for d in data["triangles"]])
-        else:
-            tris = None
-        return pts, tris
-
-    def load_points(self, name: str, idx: int | None = None) -> ndarray:
-        """Load the points from the specified dataset
-
-        Note
-        ----
-        Some shapes in the dataset include repeated points. This method returns point-sets
-        as-is, without any further processing.
-
-        The dataset also includes triangulations. Use method `load_shape` to load those as well.
-        """
+    ) -> Triangulation:
+        """The triangulated shape"""
         name = self._canonical_name(name, idx)
         if name in self.cache:
             return self.cache[name]
-        pts, _ = self.load_shape(name, load_triangles=False)
-        self.cache[name] = pts
-        return pts
+
+        data = self._load_json(name)
+        pts = array([[d["x"], d["y"]] for d in data["points"]])
+        faces = array([[d["p1"], d["p2"], d["p3"]] for d in data["triangles"]])
+        tris = self.cache[name] = Triangulation(pts, faces)
+        return tris
+
+    def load_polygon(self, name: str, idx: int | None = None) -> Polygon:
+        tris = self.load_triangulation(name, idx)
+        loops = list(tris.boundary_loops())
+        return Polygon(loops[0], loops[1:])
 
     def load_curve(self, name: str, idx: int | None = None) -> Curve:
         """Construct a `Curve` from the named shape in the dataset
 
         Can load curves by explicit name, e.g. `dataset.load_curve('Bone-13')`,
         or a class name and an index, e.g. `dataset.load_curve('Bone', 1)`.
-        Names are case-insensitive. Curves have `drop_repeated_points` applied automatically.
+        Names are case-insensitive.
         """
-        name = self._canonical_name(name, idx)
-        pts = self.load_points(name).copy()
-        return Curve(pts).drop_repeated_points().with_data(ssd_name=name)
+        poly = self.load_polygon(name, idx)
+        return poly.exterior
 
     def _canonical_name(self, name: str, idx: int | None = None) -> str:
         if idx is None:
             return name
 
         return self.names_by_class[name][idx]
```

### Comparing `curvey-0.0.2/src/curvey/util.py` & `curvey-0.0.3/src/curvey/util.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/static/curv_interp.png` & `curvey-0.0.3/static/curv_interp.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/static/curve_plot.png` & `curvey-0.0.3/static/curve_plot.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/static/willmore_flow.png` & `curvey-0.0.3/static/willmore_flow.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/tests/test_blend.py` & `curvey-0.0.3/tests/test_blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/tests/test_curve.py` & `curvey-0.0.3/tests/test_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,17 +134,17 @@
 
 
 def test_subdivide(tri: Curve):
     tri2 = tri.subdivide(1)
     assert tri2.n == tri.n * 2
 
 
-@pytest.mark.parametrize("kwargs", [{"n": 1}, {"min_edge_length": 0.1}])
+@pytest.mark.parametrize("kwargs", [{"n": 2}, {"min_edge_length": 0.1}])
 def test_collapse_shortest_edges(kwargs):
-    c = Curve([[0, 0], [0.98, 0], [1, 0], [1, 1]]).collapse_shortest_edges(**kwargs)
+    c = Curve([[0, 0], [0.97, 0], [0.98, 0], [1, 0], [1, 1]]).collapse_shortest_edges(**kwargs)
     assert_array_equal(c.points, [[0, 0], [1, 0], [1, 1]])
 
 
 def test_is_simple():
     assert Curve([(0, 0), (2, 0), (1, 1)]).is_simple
     assert not Curve([(0, 0), (2, 0), (1, 1), (1, -1)]).is_simple
```

### Comparing `curvey-0.0.2/tests/test_curves.py` & `curvey-0.0.3/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/tests/test_flow.py` & `curvey-0.0.3/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/tests/test_shape_structure_dataset.py` & `curvey-0.0.3/tests/test_shape_structure_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 from curvey import Curve
 from curvey.shape_structure_dataset import ShapeStructureDataset
 
 _DATASET_FILE = Path("~/Downloads/ShapesJSON.zip").expanduser()
 _DATASET_MISSING = not _DATASET_FILE.exists()
 _DATASET_MISSING_REASON = "Dataset file could not be found"
 
+requires_ssd = pytest.mark.skipif(_DATASET_MISSING, reason=_DATASET_MISSING_REASON)
+
 
 def test_missing_zip_file_raises():
     with pytest.raises(FileNotFoundError):
         _ = ShapeStructureDataset("doesnt_exist.zip")
 
 
 @pytest.fixture()
 def dataset():
     return ShapeStructureDataset(_DATASET_FILE)
 
 
-@pytest.mark.skipif(_DATASET_MISSING, reason=_DATASET_MISSING_REASON)
+@requires_ssd
 def test_load_curve(dataset):
     curve = dataset.load_curve("elephant-1")
     assert isinstance(curve, Curve)
+
+    curve = dataset.load_curve("elephant", 0)
+    assert isinstance(curve, Curve)
```

### Comparing `curvey-0.0.2/LICENSE` & `curvey-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curvey-0.0.2/README.md` & `curvey-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,7 +27,15 @@
 
 ### Shape blending
 
 <img src="https://raw.githubusercontent.com/darikg/curvey/main/static/curv_interp.png" alt="curvature based shape interpolation" width="500"/>
 
 Implementations of linear shape blending and [curvature flow shape blending](
 https://www.sciencedirect.com/science/article/pii/S016783961730016X).
+
+
+### Approximate medial axis
+
+<img src="https://raw.githubusercontent.com/darikg/curvey/main/static/ama.png" alt="approximate medial axis" width="150"/>
+
+Implementation of the [approximate medial axis](
+https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=cfc187181ce85d983843c4a184651dbd2a07e7e5).
```

### Comparing `curvey-0.0.2/pyproject.toml` & `curvey-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curvey"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"},
 ]
 maintainers = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"}
 ]
 description = "Pythonic geometric processing of discrete planar closed curves"
@@ -41,18 +41,20 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 dependencies = [
     "matplotlib",
+    "networkx",
     "numpy",
     "scipy",
     "shapely",
     "sortedcontainers",
+    "triangle",
     "typing_extensions",
 ]
 
 [project.optional-dependencies]
 dev = [
     "precommit",
     "mypy",
```

### Comparing `curvey-0.0.2/PKG-INFO` & `curvey-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: curvey
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pythonic geometric processing of discrete planar closed curves
 Project-URL: Homepage, https://github.com/darikg/curvey/
 Project-URL: Documentation, https://darikg.github.io/curvey/
 Project-URL: Source Code, https://github.com/darikg/curvey/
 Author-email: Darik Gamble <darik.gamble@gmail.com>
 Maintainer-email: Darik Gamble <darik.gamble@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
@@ -185,18 +185,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Requires-Dist: matplotlib
+Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: sortedcontainers
+Requires-Dist: triangle
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: precommit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: sortedcontainers-stubs; extra == 'dev'
 Requires-Dist: sybil; extra == 'dev'
@@ -239,7 +241,15 @@
 
 ### Shape blending
 
 <img src="https://raw.githubusercontent.com/darikg/curvey/main/static/curv_interp.png" alt="curvature based shape interpolation" width="500"/>
 
 Implementations of linear shape blending and [curvature flow shape blending](
 https://www.sciencedirect.com/science/article/pii/S016783961730016X).
+
+
+### Approximate medial axis
+
+<img src="https://raw.githubusercontent.com/darikg/curvey/main/static/ama.png" alt="approximate medial axis" width="150"/>
+
+Implementation of the [approximate medial axis](
+https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=cfc187181ce85d983843c4a184651dbd2a07e7e5).
```

