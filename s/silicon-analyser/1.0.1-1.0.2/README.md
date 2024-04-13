# Comparing `tmp/silicon-analyser-1.0.1.tar.gz` & `tmp/silicon-analyser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon-analyser-1.0.1.tar", last modified: Thu Apr 11 18:11:30 2024, max compression
+gzip compressed data, was "silicon-analyser-1.0.2.tar", last modified: Sat Apr 13 08:16:48 2024, max compression
```

## Comparing `silicon-analyser-1.0.1.tar` & `silicon-analyser-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon-analyser-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2478 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2024-04-11 18:08:08.000000 silicon-analyser-1.0.1/README.md
--rw-rw-rw-   0        0        0     1141 2024-04-11 16:55:06.000000 silicon-analyser-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3444 2024-04-10 15:06:41.000000 silicon-analyser-1.0.1/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon-analyser-1.0.1/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     2950 2024-04-11 17:04:32.000000 silicon-analyser-1.0.1/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2305 2024-04-11 17:08:12.000000 silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2599 2024-04-11 17:41:51.000000 silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0      940 2024-04-11 17:18:04.000000 silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      716 2024-04-08 18:23:54.000000 silicon-analyser-1.0.1/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon-analyser-1.0.1/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1293 2024-04-11 17:15:09.000000 silicon-analyser-1.0.1/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    14281 2024-04-11 17:16:10.000000 silicon-analyser-1.0.1/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    18801 2024-04-10 16:16:48.000000 silicon-analyser-1.0.1/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1510 2024-04-08 17:17:01.000000 silicon-analyser-1.0.1/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3353 2024-04-08 17:17:18.000000 silicon-analyser-1.0.1/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    15998 2024-04-11 18:05:59.000000 silicon-analyser-1.0.1/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon-analyser-1.0.1/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     6523 2024-04-11 17:42:11.000000 silicon-analyser-1.0.1/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0     7401 2024-04-11 17:42:00.000000 silicon-analyser-1.0.1/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon-analyser-1.0.1/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     1973 2024-04-08 17:15:56.000000 silicon-analyser-1.0.1/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1279 2024-04-05 16:48:05.000000 silicon-analyser-1.0.1/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:11:29.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     2478 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-11 18:11:30.000000 silicon-analyser-1.0.1/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon-analyser-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2622 2024-04-13 08:16:48.000000 silicon-analyser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1841 2024-04-13 07:40:59.000000 silicon-analyser-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1141 2024-04-13 06:22:40.000000 silicon-analyser-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 08:16:48.000000 silicon-analyser-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3444 2024-04-10 15:06:41.000000 silicon-analyser-1.0.2/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon-analyser-1.0.2/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     2950 2024-04-11 17:04:32.000000 silicon-analyser-1.0.2/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2305 2024-04-11 17:08:12.000000 silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     2693 2024-04-13 07:27:03.000000 silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon-analyser-1.0.2/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon-analyser-1.0.2/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1310 2024-04-13 08:15:14.000000 silicon-analyser-1.0.2/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    14281 2024-04-11 17:16:10.000000 silicon-analyser-1.0.2/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    19901 2024-04-13 07:26:44.000000 silicon-analyser-1.0.2/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1520 2024-04-13 07:43:17.000000 silicon-analyser-1.0.2/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     3353 2024-04-08 17:17:18.000000 silicon-analyser-1.0.2/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    16134 2024-04-13 07:03:47.000000 silicon-analyser-1.0.2/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon-analyser-1.0.2/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     6523 2024-04-11 17:42:11.000000 silicon-analyser-1.0.2/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0     8618 2024-04-13 07:34:30.000000 silicon-analyser-1.0.2/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon-analyser-1.0.2/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2043 2024-04-13 06:38:05.000000 silicon-analyser-1.0.2/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1279 2024-04-05 16:48:05.000000 silicon-analyser-1.0.2/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     2622 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-13 08:16:47.000000 silicon-analyser-1.0.2/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon-analyser-1.0.1/LICENSE` & `silicon-analyser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/PKG-INFO` & `silicon-analyser-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.1
+Version: 1.0.2
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,22 @@
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
 Requires-Dist: scikit-learn
 Requires-Dist: packaging
 
 # Installation
 
+Install from source:
+
 `pip install .`
 
+Install from pip:
+
+`pip install silicon-analyser`
+
 # Information
 
 Code will use your graphic card for acceleration.
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
@@ -55,15 +61,15 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
-![image](docs/small_tutorial.gif)
+![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.1/README.md` & `silicon-analyser-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Installation
 
+Install from source:
+
 `pip install .`
 
+Install from pip:
+
+`pip install silicon-analyser`
+
 # Information
 
 Code will use your graphic card for acceleration.
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
@@ -34,15 +40,15 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
-![image](docs/small_tutorial.gif)
+![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.1/pyproject.toml` & `silicon-analyser-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/dialogs/compute_stats.py` & `silicon-analyser-1.0.2/silicon_analyser/dialogs/compute_stats.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/dialogs/compute_stats.ui` & `silicon-analyser-1.0.2/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/grid.py` & `silicon-analyser-1.0.2/silicon_analyser/grid.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstractimage.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QMainWindow
+from PyQt5.QtWidgets import QMainWindow, QPushButton
 from PyQt5.QtGui import QStandardItem
 from PyQt5.QtWidgets import QAction
 
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 
 class AbstractMyWindow(QMainWindow):
@@ -11,15 +11,15 @@
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     autosave: bool
     def __init__(self):
         QMainWindow.__init__(self)
-    
+        
     def getManualItem(self) -> QStandardItem:
         raise NotImplementedError()
     
     def getScale(self):
         raise NotImplementedError()
     
     def getPos(self):
@@ -89,7 +89,10 @@
         raise NotImplementedError()
     
     def getModel(self, name):
         raise NotImplementedError()
     
     def hasModel(self, name) -> bool:
         raise NotImplementedError()
+    
+    def drawImgAndMinimap(self):
+        raise NotImplementedError()
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtGui import QStandardItem
 from PyQt5.QtWidgets import QTreeView
 
 from silicon_analyser.grid import Grid
 from silicon_analyser.treeitem import TreeItem
 
 class AbstractTreeHelper(QTreeView):
+    evtTreeSelectionChanged: pyqtSignal
+    
     def selectedType(self) -> str:
         raise NotImplementedError()
     
     def selectedLabel(self) -> str:
         raise NotImplementedError()
 
     def getSelectedItem(self) -> QStandardItem:
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/addgridbtn.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/addlabelbtn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from PyQt5.QtWidgets import QInputDialog, QPushButton
 from PyQt5.QtGui import QMouseEvent
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
-from silicon_analyser.treeitem import TreeItem
 
-class AddGridBtn(QPushButton):
+class AddLabelBtn(QPushButton):
     def __init__(self, text: str):
         QPushButton.__init__(self, text)
         self.clicked.connect(self.buttonClicked)
-        self.gridIdx = 0
 
     def buttonClicked(self, event: QMouseEvent):
-        print("AddGridBtn: buttonClicked")
-        self._myWindow.getTree().addTreeItem("grid_%d" % self.gridIdx,TreeItem.TYPE_GRID)
-        self.gridIdx += 1
-    
+        print("AddLabelBtn: buttonClicked")
+        text, ok = QInputDialog.getText(self, 'Label Input Dialog', 'Enter your label:')
+        if ok:
+            self._myWindow.getTree().addTreeItem(text)
+            
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/ai.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/ai.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from grid import Grid, getAllCellRects
 import numpy as np
 import keras
+from silicon_analyser.grid import Grid, getAllCellRects
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 
 def getDefaultMaxWMaxH(grid: Grid):
     maxW = grid.width//grid.cols
     maxH = grid.height//grid.rows
     MP = 5
     if maxW % MP != 0:
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/computebtn.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/computebtn.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/fullimage.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/fullimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtCore import Qt, QRect, QSize
+from PyQt5.QtCore import Qt, QRect, QSize, QTimer
 from PyQt5.QtWidgets import QLabel, QSizePolicy
 from PyQt5.QtGui import QImage, QPixmap, QColor, QMouseEvent, QPainter, QPen, QBrush
 import numpy as np
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.savefiles import saveGrids,saveRects
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
@@ -12,14 +12,20 @@
     _rects: dict[Rect]
     _aiRects: dict[Rect]
     _rectActive: dict[bool]
     _grids: dict[Grid]
     _aiGrids: dict[Grid]
     _gridsActive: dict[bool]
     _aiGridsActive: dict[bool]
+    _moveStartX: int
+    _moveStartY: int
+    _moveDeltaX: int
+    _moveDeltaY: int
+    _moveTimer: QTimer
+    
     def __init__(self, parent):
         QLabel.__init__(self, parent)
         self._drawRectStart = False
         self._rectStartX = 0
         self._rectStartY = 0
         self._rectEndX = 0
         self._rectEndY = 0
@@ -29,14 +35,25 @@
         self._aiGridsActive = {}
         self._rects = {}
         self._aiRects = {}
         self._rectActive = {}
         self._aiRectActive = {}
         self._aiIgnoreRects = []
         self.setSizePolicy(QSizePolicy.Policy.Expanding,QSizePolicy.Policy.Expanding)
+        self._moveTimer = QTimer()
+        self._moveTimer.timeout.connect(self.moveUpdate)
+        self._moveTimer.setInterval(int(1000 * 0.2))
+    
+    def moveUpdate(self):
+        posX, posY = self._myWindow.getPos()
+        posX += self._moveDeltaX
+        posY += self._moveDeltaY
+        self._myWindow.setPosX(posX)
+        self._myWindow.setPosY(posY)
+        self._myWindow.drawImgAndMinimap()
     
     def initialize(self, myWindow: AbstractMyWindow, pixmap: QPixmap):
         self._myWindow = myWindow
         self._pixmap: QPixmap = pixmap
         self._currentImg = pixmap
     
     def getRects(self) -> list[Rect]:
@@ -71,27 +88,38 @@
                         grid.setRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
                     if button == Qt.RightButton:
                         grid.unsetRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
                     if self._myWindow.autosave:
                         saveGrids(self._grids)
                     
     def mousePressEvent(self, event: QMouseEvent):
+        if event.button() == Qt.MiddleButton:
+            self._moveStart = True
+            self._moveStartX = event.x()
+            self._moveStartY = event.y()
+            self._moveDeltaX = 0
+            self._moveDeltaY = 0
         tree = self._myWindow.getTree()
         if tree.selectedType() == TreeItem.TYPE_GRID_ITEM:
             self.markGridItem(event.x(),event.y(),event.button())
             return
         if event.button() == Qt.LeftButton:
             print("FullImage: mousePressEvent",self._drawRectStart)
             if tree.selectedType() is not None:
                 if not self._drawRectStart:
                     self._drawRectStart = True
                     self._rectStartX = self._translateEventToPixel(event.x())
                     self._rectStartY = self._translateEventToPixel(event.y())
     
     def mouseMoveEvent(self, event: QMouseEvent | None) -> None:
+        if self._moveStart:
+            self._moveDeltaX = event.x() - self._moveStartX
+            self._moveDeltaY = event.y() - self._moveStartY
+            self._moveTimer.start()
+
         if self._drawRectStart:
             self._rectEndX = self._translateEventToPixel(event.x())
             self._rectEndY = self._translateEventToPixel(event.y())
             if(self._rectEndX < self._rectStartX):
                 self._rectEndX, self._rectStartX = self._rectStartX, self._rectEndX
             if(self._rectEndY < self._rectStartY):
                 self._rectEndY, self._rectStartY = self._rectStartY, self._rectEndY
@@ -106,14 +134,18 @@
                 self._translatePixelToScaled(self._rectStartY),
                 self._translatePixelToScaled(self._rectEndX)-self._translatePixelToScaled(self._rectStartX),
                 self._translatePixelToScaled(self._rectEndY)-self._translatePixelToScaled(self._rectStartY))
             qp.end()
             self.setPixmap(pixmap)
      
     def mouseReleaseEvent(self, event: QMouseEvent):
+        if event.button() == Qt.MiddleButton:
+            self._moveStart = False
+            self._moveTimer.stop()
+            
         if event.button() == Qt.LeftButton:
             self._drawRectStart = False
             print("mouseReleaseEvent",self._rectStartX,self._rectStartY,self._rectEndX,self._rectEndY)
             selectedKey: str = self._myWindow.getTree().selectedLabel()
             if selectedKey is not None:
                 x = self._rectStartX
                 y = self._rectStartY
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/minimap.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/minimap.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         
     def mouseReleaseEvent(self,event: QMouseEvent):
         print("clicked")
         sc1x = 300/self._pixmap.width()
         sc1y = 300/self._pixmap.height()
         self._myWindow.setPosX(int(event.x()/sc1x))
         self._myWindow.setPosY(int(event.y()/sc1y))
-        self._myWindow.drawImg()
+        self._myWindow.drawImgAndMinimap()
         print(self._myWindow.getPosX(),self._myWindow.getPosY())
 
     def scaleMinimapX(self):
         return 300/self._pixmap.width()
     
     def scaleMinimapY(self):
         return 300/self._pixmap.height()
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/properties.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/properties.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/helper/tree.py` & `silicon-analyser-1.0.2/silicon_analyser/helper/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtCore import QItemSelection
+from PyQt5.QtCore import QItemSelection, pyqtSignal
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog
 from PyQt5.QtGui import QStandardItem
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.grid import Grid
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
@@ -13,14 +13,15 @@
     _myWindow: AbstractMyWindow
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
+    evtTreeSelectionChanged: pyqtSignal = pyqtSignal(QItemSelection)
 
     def __init__(self, parent: QWidget | None = ...) -> None:
         super().__init__(parent)
     
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
         self.selectionModel().selectionChanged.connect(self.treeSelectionChanged)
@@ -176,14 +177,15 @@
             self._actionRemoveLabel.setVisible(True)
         else:
             self._actionRemoveLabel.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID_ITEM):
             myWindow.getImage().drawImage()
         if(selectedType == TreeItem.TYPE_AI_GRID_ITEM):
             myWindow.getImage().drawImage()
+        self.evtTreeSelectionChanged.emit(selection)
             
     def addTreeItem(self, text, type="auto", parent_obj=None, parent_item=None) -> tuple[Grid, TreeItem]:
         obj = None
         myWindow: AbstractMyWindow = self._myWindow
         img = myWindow.getImage()
         tree: Tree = self
         if type == "auto":
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/main_window.ui` & `silicon-analyser-1.0.2/silicon_analyser/main_window.ui`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser/mywindow.py` & `silicon-analyser-1.0.2/silicon_analyser/mywindow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from PyQt5 import QtCore, uic
 from PyQt5.QtCore import Qt, QItemSelection
-from PyQt5.QtWidgets import QFileDialog, QTableView, QStatusBar, QAction
+from PyQt5.QtWidgets import QFileDialog, QTableView, QStatusBar, QAction, QPushButton
 from PyQt5.QtGui import QPixmap, QStandardItem, QStandardItemModel
 from os import path as p
 import sys
+
 import silicon_analyser.savefiles
 from silicon_analyser.savefiles import loadGrids, loadRects
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.helper.minimap import MiniMap
 from silicon_analyser.helper.fullimage import FullImage
@@ -39,76 +40,105 @@
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
     autosave: bool
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
         uic.loadUi(p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui', self)
+        tree: Tree = self._tree
+        properties: QTableView = self._properties
+                
         self._treeModel = QStandardItemModel()
         self._propertiesModel = QStandardItemModel()
-        self._properties.setModel(self._propertiesModel)
+        properties.setModel(self._propertiesModel)
         self._propertiesUtil = PropertiesUtil(self,self._properties)
         
         self._treeManualItem = QStandardItem("Manual")
         self._treeManualItem.setFlags(QtCore.Qt.ItemIsUserCheckable |
                           QtCore.Qt.ItemIsEnabled)
         self._treeManualItem.setCheckState(QtCore.Qt.Unchecked)
         self._treeModel.appendRow(self._treeManualItem)
         self._treeAIItem = QStandardItem("AI")
         self._treeAIItem.setFlags(QtCore.Qt.ItemIsUserCheckable |
                           QtCore.Qt.ItemIsEnabled)
         self._treeAIItem.setCheckState(QtCore.Qt.Unchecked)
         self._treeModel.appendRow(self._treeAIItem)
-        self._tree.setModel(self._treeModel)
+        tree.setModel(self._treeModel)
         self._models = {}
         self._actionUrl.triggered.connect(self.openMainUrl)
 
         if(len(sys.argv) < 2):
             dlg = QFileDialog()
             filenames = dlg.getOpenFileName(caption="Load image",filter="Image (*.png;*.jpg;*.bmp;*.gif)",initialFilter="Trained model (*.h5)")
             if(len(filenames) >= 1):
                 self._pixmap = QPixmap(filenames[0])
         else:
             self._pixmap = QPixmap(sys.argv[1])
         
-        self._tree.initialize(self)
-        self._computeBtn.initialize(self)
-        self._addGridBtn.initialize(self)
-        self._addLabelBtn.initialize(self)
-        self._minimap.initialize(self, self._pixmap)
-        self._image.initialize(self, self._pixmap)
+        computeBtn: ComputeBtn = self._computeBtn
+        addGridBtn: AddGridBtn = self._addGridBtn
+        addLabelBtn: AddLabelBtn = self._addLabelBtn
+        minimap: MiniMap = self._minimap
+        image: FullImage = self._image
+
+        tree.initialize(self)
+        computeBtn.initialize(self)
+        addGridBtn.initialize(self)
+        addLabelBtn.initialize(self)
+        minimap.initialize(self, self._pixmap)
+        image.initialize(self, self._pixmap)
+        
+        computeBtn.setDisabled(True)
+        addLabelBtn.setDisabled(True)
+        tree.evtTreeSelectionChanged.connect(self.treeSelectionChanged)
         
         self._posX = 0
         self._posY = 0
         
         self._scale = 1.0
         self.drawImgAndMinimap()
         
         self.autosave = False
         
         if p.isfile(silicon_analyser.savefiles.SAVE_RECTS):
             with open(silicon_analyser.savefiles.SAVE_RECTS,"r") as f:
                 rects = loadRects()
                 for k in rects.keys():
                     self.getTree().addTreeItem(k)
-                self._image.loadRects(rects)
+                image.loadRects(rects)
         if p.isfile(silicon_analyser.savefiles.SAVE_GRIDS):
-            grids: list[Grid] = loadGrids()
+            grids: dict[Grid] = loadGrids()
             for gridKey in grids.keys():
                 grid, parentTreeItem = self.getTree().addTreeItem(gridKey,TreeItem.TYPE_GRID)
                 for gridItemKey in grids[gridKey].getLabels():
                     _, treeItem = self.getTree().addTreeItem(gridItemKey,TreeItem.TYPE_GRID_ITEM, grid, parentTreeItem)
                     text = treeItem.data(TreeItem.TEXT)
                     if(not grids[gridKey]._rectsActive[text]):
                         treeItem.setCheckState(QtCore.Qt.Unchecked)
-            self._image.loadGrids(grids)
+            image.loadGrids(grids)
         
-        self._image.drawImage()
+        image.drawImage()
         self.autosave = True
         
+    def treeSelectionChanged(self, selection: QItemSelection):
+        tree: Tree = self._tree
+        selectedType: str = tree.selectedType()
+        computeBtn: ComputeBtn = self._computeBtn
+        addLabelBtn: AddLabelBtn = self._addLabelBtn
+        if((selectedType == TreeItem.TYPE_GRID_ITEM)
+           or (selectedType == TreeItem.TYPE_GRID)
+           or (selectedType == TreeItem.TYPE_AI_GRID)
+           or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
+           ):
+            computeBtn.setDisabled(False)
+            addLabelBtn.setDisabled(False)
+        else:
+            computeBtn.setDisabled(True)
+            addLabelBtn.setDisabled(True)
+
     def openMainUrl(self):
         import webbrowser
         return webbrowser.open('https://github.com/TheCrazyT/SiliconAnalyser')
         
     def getModel(self, name):
         if name in self._models:
             return self._models[name]
@@ -120,20 +150,23 @@
         return False
     
     def setLastModel(self, name, model_train):
         self._models[name] = model_train
     
     def getImage(self) -> AbstractImage:
         return self._image
+    
+    def getMinimap(self) -> MiniMap:
+        return self._minimap
 
     def imageWidth(self):
-        return self._image.width()
+        return self.getImage().width()
 
     def imageHeight(self):
-        return self._image.height()
+        return self.getImage().height()
             
     def setStatusText(self, text):
         self._statusBar.showMessage(text)
         
     def getTree(self) -> AbstractTreeHelper:
         return self._tree
     
@@ -158,16 +191,16 @@
     def setPosX(self, x):
         self._posX = x
     
     def setPosY(self, y):
         self._posY = y
     
     def drawImgAndMinimap(self):
-        self._image.drawImage()
-        self._minimap.drawMinimap()
+        self.getImage().drawImage()
+        self.getMinimap().drawMinimap()
     
     def reloadProperyWindowByGrid(self, grid):
         return self._propertiesUtil.reloadProperyWindowByGrid(grid)
     
     def reloadPropertyWindow(self, selection: QItemSelection):
         return self._propertiesUtil.reloadPropertyWindow(selection)
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/savefiles.py` & `silicon-analyser-1.0.2/silicon_analyser/savefiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from json import JSONDecoder, JSONEncoder
+
 from silicon_analyser.grid import Grid
+from silicon_analyser.rect import Rect
 
 SAVE_RECTS = "rects.json"
 SAVE_GRIDS = "grids.json"
 doSaveRects = False
 doSaveGrids = False
 
 class JSONGridDecoder(JSONDecoder):
@@ -30,19 +32,19 @@
             grids[gridName] = g
         return grids
         
 class MyJSONEncoder(JSONEncoder):
         def default(self, o):
             return o.__dict__
 
-def loadRects():
+def loadRects() -> dict[Rect]:
     with open(SAVE_RECTS,"r") as f:
         return json.load(f)
 
-def loadGrids():
+def loadGrids() -> dict[Grid]:
     with open(SAVE_GRIDS,"r") as f:
         return json.load(f, cls=JSONGridDecoder)
     
 def triggerSaveRects():
     global doSaveRects
     print("triggerSaveRects")
     doSaveRects = True
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser/treeitem.py` & `silicon-analyser-1.0.2/silicon_analyser/treeitem.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.1/silicon_analyser.egg-info/PKG-INFO` & `silicon-analyser-1.0.2/silicon_analyser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.1
+Version: 1.0.2
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,22 @@
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
 Requires-Dist: scikit-learn
 Requires-Dist: packaging
 
 # Installation
 
+Install from source:
+
 `pip install .`
 
+Install from pip:
+
+`pip install silicon-analyser`
+
 # Information
 
 Code will use your graphic card for acceleration.
 
 Frameworks/Libraries used:
 * [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 * [PyTorch](https://pytorch.org/)
@@ -55,15 +61,15 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
-![image](docs/small_tutorial.gif)
+![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.1/silicon_analyser.egg-info/SOURCES.txt` & `silicon-analyser-1.0.2/silicon_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

