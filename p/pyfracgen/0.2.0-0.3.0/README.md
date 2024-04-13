# Comparing `tmp/pyfracgen-0.2.0.tar.gz` & `tmp/pyfracgen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfracgen-0.2.0.tar", max compression
+gzip compressed data, was "pyfracgen-0.3.0.tar", max compression
```

## Comparing `pyfracgen-0.2.0.tar` & `pyfracgen-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2024-01-20 19:02:27.502971 pyfracgen-0.2.0/LICENSE
--rw-r--r--   0        0        0     4494 2024-01-20 19:02:27.502971 pyfracgen-0.2.0/README.md
--rw-r--r--   0        0        0      487 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/__init__.py
--rwxr-xr-x   0        0        0     5346 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/buddhabrot.py
--rw-r--r--   0        0        0     2198 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/common.py
--rw-r--r--   0        0        0        0 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/images/__init__.py
--rw-r--r--   0        0        0     5072 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/images/images.py
--rw-r--r--   0        0        0     1270 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/iterfuncs/funcs.py
--rw-r--r--   0        0        0     1856 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/julia.py
--rw-r--r--   0        0        0     1584 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/lyapunov.py
--rw-r--r--   0        0        0     1724 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/mandelbrot.py
--rw-r--r--   0        0        0     1382 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/randomwalk.py
--rw-r--r--   0        0        0      522 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyfracgen/types.py
--rw-r--r--   0        0        0     1886 2024-01-20 19:02:27.542971 pyfracgen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 pyfracgen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-13 14:24:40.883312 pyfracgen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4371 2024-04-13 14:24:40.883312 pyfracgen-0.3.0/README.md
+-rw-r--r--   0        0        0      447 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/__init__.py
+-rwxr-xr-x   0        0        0     5355 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/buddhabrot.py
+-rw-r--r--   0        0        0     1918 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/common.py
+-rw-r--r--   0        0        0        0 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/images/__init__.py
+-rw-r--r--   0        0        0     4161 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/images/images.py
+-rw-r--r--   0        0        0     1270 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/iterfuncs/funcs.py
+-rw-r--r--   0        0        0     1856 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/julia.py
+-rw-r--r--   0        0        0     1584 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/lyapunov.py
+-rw-r--r--   0        0        0     1724 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/mandelbrot.py
+-rw-r--r--   0        0        0     1016 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/randomwalk.py
+-rw-r--r--   0        0        0      460 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyfracgen/types.py
+-rw-r--r--   0        0        0     1936 2024-04-13 14:24:40.911311 pyfracgen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 pyfracgen-0.3.0/PKG-INFO
```

### Comparing `pyfracgen-0.2.0/LICENSE` & `pyfracgen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfracgen-0.2.0/README.md` & `pyfracgen-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 `pyfracgen` can currently be installed from the following sources (if you want
 to install from GH, probably do so using `poetry`).
 
 ### Git
 ```bash
 git clone https://github.com/rytheranderson/pyfracgen.git
+cd pyfracgen
 poetry install
 ```
 
 ### PyPI
 ```bash
 pip install pyfracgen
 ```
@@ -101,18 +102,17 @@
 
 ### Random Walk
 ![](https://github.com/rytheranderson/pyfracgen/raw/main/example_images/randomwalk_ex.png?raw=true)
 
 Image produced with this code:
 
 ```python
-basis = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-moves = pf.construct_moves(basis)
-res = pf.randomwalk(moves, niter=5000000, width=4, height=3, depth=10, dpi=300)
-pf.images.randomwalk_image(res, cmap=colormaps["gist_yarg"], gamma=1.0)
+moves = pf.construct_moves((1, 0), (0, 1))
+res = pf.randomwalk(moves, niter=1000000, width=4, height=3, dpi=300)
+pf.images.image(res, cmap=colormaps["gnuplot"], gamma=1.0)
 plt.savefig("example_images/randomwalk_ex.png")
 ```
 
 ### Buddhabrot with Nebula Coloring
 ![](https://github.com/rytheranderson/pyfracgen/raw/main/example_images/buddhabrot_ex.png?raw=true)
 
 Image produced with this code:
@@ -135,21 +135,20 @@
 plt.savefig("example_images/buddhabrot_ex.png")
 ```
 ## Fractal "Types" Supported
 * Mandelbrot
 * Julia
 * Buddhabrot
 * Markus-Lyapunov
-* 3D random walks
+* 2D random walks
 
 ## Image Creation
 * Function `image` wrapping `matplotlib.pyplot.imshow`
 * Function `nebula_image` for Buddhabrot ["nebula"](https://en.wikipedia.org/wiki/Buddhabrot#Nuances) coloration
 * Function `markus_lyapunov_image` for [Markus-Lyapunov](https://doi.org/10.1016/0097-8493(89)90019-8) coloration
-* Function `randomwalk_image` for coloring 3D random walks with depth
 * Function `save_animation` for animating a sequence of results
 
 ## More than Quadratic Polynomials
 Mandelbrot, Julia, and Buddhabrot fractal images are almost always created by
 iterating the function $f_c(z) = z^2 + c$. Makes sense, since this function is
 part of the definition of the Mandelbrot set. However, you can iterate lots of
 other functions to produce similarly striking images: see the `iterfuncs` module
```

### Comparing `pyfracgen-0.2.0/pyfracgen/buddhabrot.py` & `pyfracgen-0.3.0/pyfracgen/buddhabrot.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,17 @@
         for _ in range(maxiter):
             az = np.abs(z)
             trial_sequence.append(z)
             if az > horizon:
                 sequence.extend(trial_sequence)
                 break
             z = update_func(z, c)
-        for c in sequence:
-            indx = int((c.real - xmin) / (xmax - xmin) * width)
-            indy = int((c.imag - ymin) / (ymax - ymin) * height)
+        for sval in sequence:
+            indx = int((sval.real - xmin) / (xmax - xmin) * width)
+            indy = int((sval.imag - ymin) / (ymax - ymin) * height)
             if (indx < 0 or indx >= width) or (indy < 0 or indy >= height):
                 continue
             lattice[indy, indx] += 1
 
 
 class Buddhabrot(CanvasBounded):
     @property
```

### Comparing `pyfracgen-0.2.0/pyfracgen/common.py` & `pyfracgen-0.3.0/pyfracgen/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Utility objects and methods used across the library."""
+
 from __future__ import annotations
 
 import pickle
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 
-from pyfracgen.types import Bound, Lattice, Lattice3D
+from pyfracgen.types import Bound, Lattice
 
 RESULT_DEFAULT_SAVE = Path("save.pickle")
 
 
 @dataclass(frozen=True)
 class Result:
     image_array: Lattice
@@ -43,22 +44,14 @@
     def result(self) -> Result:
         return Result(self.lattice, self.width, self.height, self.dpi)
 
     def paint(self, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError
 
 
-class Canvas3D(Canvas):
-    def __init__(self, width: int, height: int, depth: int, dpi: int) -> None:
-        super().__init__(width, height, dpi)
-        self.lattice: Lattice3D = np.dstack(
-            [np.zeros(self.lattice.shape) for _ in range(depth)]
-        )
-
-
 class CanvasBounded(Canvas):
     def __init__(
         self, width: int, height: int, dpi: int, xbound: Bound, ybound: Bound
     ) -> None:
         super().__init__(width, height, dpi)
         ny, nx = self.lattice.shape
         self.xbound = xbound
```

### Comparing `pyfracgen-0.2.0/pyfracgen/images/images.py` & `pyfracgen-0.3.0/pyfracgen/images/images.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Sequence
 
-import matplotlib.animation as animation
+from matplotlib import animation
 import numpy as np
 from matplotlib import colormaps, colors
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure, figaspect
 
 from pyfracgen.common import Result
@@ -74,57 +74,32 @@
     cmap_pos: colors.Colormap,
     gammas: tuple[float, float] = (1.0, 1.0),
     ticks: bool = False,
 ) -> tuple[Figure, Axes]:
     fig, ax0 = plt.subplots(figsize=figaspect(res.image_array), dpi=res.dpi)
     fig.subplots_adjust(0, 0, 1, 1)
     ax0.imshow(
-        np.ma.masked_where(res.image_array > 0.0, res.image_array),  # type: ignore[no-untyped-call] # noqa: E501
+        np.ma.masked_where(res.image_array > 0.0, res.image_array),  # type: ignore[no-untyped-call]
         cmap=cmap_neg,
         origin="lower",
         norm=colors.PowerNorm(gammas[0]),
     )
     ax0.imshow(
-        np.ma.masked_where(res.image_array < 0.0, res.image_array),  # type: ignore[no-untyped-call] # noqa: E501
+        np.ma.masked_where(res.image_array < 0.0, res.image_array),  # type: ignore[no-untyped-call]
         cmap=cmap_pos,
         origin="lower",
         norm=colors.PowerNorm(gammas[1]),
     )
     if not ticks:
         plt.axis(ticks)
     fs = plt.gcf()
     fs.set_size_inches(res.width_inches, res.height_inches)
     return fig, ax0
 
 
-def randomwalk_image(
-    res: Result,
-    cmap: colors.Colormap = DEFAULT_COLORMAP,
-    ticks: bool = False,
-    gamma: float = 0.3,
-    alpha_scale: float = 1.0,
-) -> tuple[Figure, Axes]:
-    fig, ax0 = plt.subplots(figsize=figaspect(res.image_array[:, :, 0]), dpi=res.dpi)
-    fig.subplots_adjust(0, 0, 1, 1)
-    max_ind = float(res.image_array.shape[-1] + 1)
-    for i in range(res.image_array.shape[-1]):
-        im = res.image_array[..., i]
-        im = np.ma.masked_where(im == 0, im)  # type: ignore[no-untyped-call]
-        alpha = alpha_scale * (1 - (i + 1) / max_ind)
-        norm = colors.PowerNorm(gamma)
-        ax0.imshow(
-            im, origin="lower", alpha=alpha, cmap=cmap, norm=norm, interpolation=None
-        )
-    if not ticks:
-        plt.axis(ticks)
-    fs = plt.gcf()
-    fs.set_size_inches(res.width_inches, res.height_inches)
-    return fig, ax0
-
-
 def save_animation(
     series: Sequence[Result],
     cmap: colors.Colormap = DEFAULT_COLORMAP,
     fps: int = 15,
     bitrate: int = 1800,
     file: Path = ANIMATION_DEFAULT_SAVE,
     ticks: bool = True,
```

### Comparing `pyfracgen-0.2.0/pyfracgen/iterfuncs/funcs.py` & `pyfracgen-0.3.0/pyfracgen/iterfuncs/funcs.py`

 * *Files identical despite different names*

### Comparing `pyfracgen-0.2.0/pyfracgen/julia.py` & `pyfracgen-0.3.0/pyfracgen/julia.py`

 * *Files identical despite different names*

### Comparing `pyfracgen-0.2.0/pyfracgen/lyapunov.py` & `pyfracgen-0.3.0/pyfracgen/lyapunov.py`

 * *Files identical despite different names*

### Comparing `pyfracgen-0.2.0/pyfracgen/mandelbrot.py` & `pyfracgen-0.3.0/pyfracgen/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `pyfracgen-0.2.0/pyproject.toml` & `pyfracgen-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pyfracgen"
 
 [tool.poetry]
 name = "pyfracgen"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python Fractal Generation is a package for generating aesthetic fractal images quickly and (hopefully) easily"
 authors = ["Ryther Anderson"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/rytheranderson/pyfracgen"
 include = [
     "README.md",
@@ -21,48 +21,44 @@
 python = "^3.10"
 matplotlib = "^3.8.2"
 numba = ">=0.59.0rc1"
 numpy = "^1.26.2"
 nptyping = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-cruft = "^2.15.0"
-flake8 = "^6.1.0"
-flake8-docstrings = "^1.7.0"
-flake8-bugbear = "^23.5.9"
-hypothesis = "^6.75.6"
-isort = "^5.12.0"
-mypy = "^1.7.1"
-pre-commit = "^3.3.2"
-pytest = "^7.3.1"
-pytest-cov = "^4.1.0"
-pytest-mock = "^3.10.0"
-tbump = "^6.10.0"
-tox = "^3.24"
-tox-gh-actions = "^2.8"
-tox-poetry-installer = "^0.10.0"
-
-[tool.black]
-line-length = 88
-experimental_string_processing = true
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | build
-  | dist
-)/
-'''
+hypothesis = "^6.99.13"
+mypy = "^1.9.0"
+pre-commit = "^3.7.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
+ruff = "^0.3.4"
+tbump = "^6.11.0"
+tox = "^3.28.0"
+tox-gh-actions = "^2.12.0"
+tox-poetry-installer = "^0.10.3"
+
+[tool.ruff.lint]
+# B = flake8-bugbear
+# C9 = mccabe complexity
+# E = pycodestyle error
+# F = pyflakes
+# N = pep8-naming
+# PL = pylint
+# Q = flake8-quotes
+# RUF = ruf
+# W = pycodestyle warning
+select = ["B", "C9", "D", "E", "F", "N", "PL", "Q", "RUF", "W"]
+ignore = ["D10", "PLR0913"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
 
 [tool.tbump.version]
-current = "0.2.0"
+current = "0.3.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -70,19 +66,19 @@
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
-search = 'current = "0.2.0"'
+search = 'current = "0.3.0"'
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
-search = 'version = "0.2.0"'
+search = 'version = "0.3.0"'
 
 [[tool.tbump.file]]
 src = "pyfracgen/__init__.py"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyfracgen-0.2.0/PKG-INFO` & `pyfracgen-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfracgen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Fractal Generation is a package for generating aesthetic fractal images quickly and (hopefully) easily
 Home-page: https://github.com/rytheranderson/pyfracgen
 License: MIT
 Author: Ryther Anderson
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,14 +30,15 @@
 
 `pyfracgen` can currently be installed from the following sources (if you want
 to install from GH, probably do so using `poetry`).
 
 ### Git
 ```bash
 git clone https://github.com/rytheranderson/pyfracgen.git
+cd pyfracgen
 poetry install
 ```
 
 ### PyPI
 ```bash
 pip install pyfracgen
 ```
@@ -121,18 +122,17 @@
 
 ### Random Walk
 ![](https://github.com/rytheranderson/pyfracgen/raw/main/example_images/randomwalk_ex.png?raw=true)
 
 Image produced with this code:
 
 ```python
-basis = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-moves = pf.construct_moves(basis)
-res = pf.randomwalk(moves, niter=5000000, width=4, height=3, depth=10, dpi=300)
-pf.images.randomwalk_image(res, cmap=colormaps["gist_yarg"], gamma=1.0)
+moves = pf.construct_moves((1, 0), (0, 1))
+res = pf.randomwalk(moves, niter=1000000, width=4, height=3, dpi=300)
+pf.images.image(res, cmap=colormaps["gnuplot"], gamma=1.0)
 plt.savefig("example_images/randomwalk_ex.png")
 ```
 
 ### Buddhabrot with Nebula Coloring
 ![](https://github.com/rytheranderson/pyfracgen/raw/main/example_images/buddhabrot_ex.png?raw=true)
 
 Image produced with this code:
@@ -155,21 +155,20 @@
 plt.savefig("example_images/buddhabrot_ex.png")
 ```
 ## Fractal "Types" Supported
 * Mandelbrot
 * Julia
 * Buddhabrot
 * Markus-Lyapunov
-* 3D random walks
+* 2D random walks
 
 ## Image Creation
 * Function `image` wrapping `matplotlib.pyplot.imshow`
 * Function `nebula_image` for Buddhabrot ["nebula"](https://en.wikipedia.org/wiki/Buddhabrot#Nuances) coloration
 * Function `markus_lyapunov_image` for [Markus-Lyapunov](https://doi.org/10.1016/0097-8493(89)90019-8) coloration
-* Function `randomwalk_image` for coloring 3D random walks with depth
 * Function `save_animation` for animating a sequence of results
 
 ## More than Quadratic Polynomials
 Mandelbrot, Julia, and Buddhabrot fractal images are almost always created by
 iterating the function $f_c(z) = z^2 + c$. Makes sense, since this function is
 part of the definition of the Mandelbrot set. However, you can iterate lots of
 other functions to produce similarly striking images: see the `iterfuncs` module
```

