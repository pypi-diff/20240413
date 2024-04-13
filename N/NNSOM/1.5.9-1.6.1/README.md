# Comparing `tmp/nnsom-1.5.9.tar.gz` & `tmp/nnsom-1.6.1.tar.gz`

## Comparing `nnsom-1.5.9.tar` & `nnsom-1.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    77247 2020-02-02 00:00:00.000000 nnsom-1.5.9/src/NNSOM/plots.py
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.9/src/NNSOM/som.py
--rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.5.9/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.9/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.9/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.9/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.9/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0    77155 2020-02-02 00:00:00.000000 nnsom-1.6.1/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.6.1/src/NNSOM/som.py
+-rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 nnsom-1.6.1/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.6.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.1/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.1/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.1/PKG-INFO
```

### Comparing `nnsom-1.5.9/src/NNSOM/plots.py` & `nnsom-1.6.1/src/NNSOM/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, pathces
         """
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
@@ -120,15 +120,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, pathces, text
         """
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
@@ -186,15 +186,15 @@
             If true, the interactive plot and sub-clustering functionalities to be activated
         connect_pick_event
             If true, the pick event is connected to the plot
         kwargs: dict
             Additional arguments to be passed to the on_pick function
             Possible keys includes:
             'data', 'labels', 'clust', 'target', 'num1', 'num2',
-            'cat', 'align', 'height' and 'topn'
+            'cat', and 'topn'
 
         Returns
         -------
             fig, ax, patches, text
         """
 
         pos = self.pos
@@ -425,15 +425,15 @@
             len(edge_width) must be equal to the number of neurons
         mouse_click: bool
             If true, the interactive plot and sub-clustering functionalities to be activated
         kwargs: dict
             Additional arguments to be passed to the onpick function
             Possible keys include:
             'data', 'clust', 'target', 'num1', 'num2',
-            'cat', 'align', 'height' and 'topn'
+            'cat', and 'topn'
 
         Returns:
             fig, ax, patches, text
         """
         numNeurons = self.numNeurons
 
         x = np.asarray(x, np.float32)
@@ -493,15 +493,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, pathces
         """
         # Neighborhood Connection Map. The gray hexagons represent cluster centers.
         pos = self.pos
         numNeurons = self.numNeurons
@@ -570,15 +570,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
         Returns:
             fig, ax, pathces, text
         """
 
         pos = self.pos
         numNeurons = self.numNeurons
 
@@ -683,15 +683,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, pathces, cbar
         """
 
         w = self.w
         pos = self.pos
@@ -887,15 +887,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
 
         numNeurons = self.numNeurons
 
@@ -904,16 +904,15 @@
 
         # Draw stem plot
         for neuron in range(numNeurons):
             # Make graph
             h_axes[neuron].stem(x, y[neuron])
 
         if mouse_click and connect_pick_event:
-            kwargs['align'] = x
-            kwargs['height'] = y
+            kwargs['cat'] = y
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_wgts(self, mouse_click=False, connect_pick_event=True, **kwargs):
@@ -923,15 +922,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
 
         numNeurons = self.numNeurons
         w = self.w
@@ -963,15 +962,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
         # Validate the length of x (array or sequence of vectors)
         if len(x) != self.numNeurons:
             raise ValueError("The length of x must be equal to the number of neurons.")
@@ -1031,15 +1030,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
 
         numNeurons = self.numNeurons
 
@@ -1082,15 +1081,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
 
         numNeurons = self.numNeurons
 
@@ -1128,15 +1127,15 @@
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
+                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
 
         numNeurons = self.numNeurons
 
@@ -1742,39 +1741,50 @@
         neuron_ind = hexagon_to_neuron[thishex]
 
         if len(kwargs["clust"][neuron_ind]) <= 0:
             print('No data in this cluster')
             return
 
         # Create a new window
-        fig, ax1 = plt.subplots(figsize=(6, 6))
+        fig, ax = plt.subplots(figsize=(6, 6))
         fig.subplots_adjust(right=0.8)
-        ax1.set_aspect('equal')
+        ax.set_aspect('equal')
 
         # Button Configuration
         button_types = self.determine_button_types(**kwargs)
         buttons = create_buttons(fig, button_types)
 
         # Set up button click events
         for button_type, button in buttons.items():
-            button.on_clicked(lambda event, b=button_type:
-                              self.button_click_event(b, ax1, neuron_ind, **kwargs))
+            button.on_clicked(self.create_click_handler(button_type, ax, neuron_ind, **kwargs))
 
+        # Show up the 2nd window
         plt.show()
 
+    def create_click_handler(self, button_type, ax, neuron_ind, **kwargs):
+        def handler(event):
+            self.button_click_event(button_type, ax, neuron_ind, **kwargs)
+
+        return handler
+
     def button_click_event(self, button_type, ax, neuron_ind, **kwargs):
 
         # Handle button click event by calling the appropriate plot function
         if button_type == 'pie':
             # Pre-process categorical variables
             sizes = kwargs['cat']
             sizes = sizes[neuron_ind][:kwargs['topn']]
             self.plot_pie(ax, sizes, neuron_ind)
+
         elif button_type == 'stem':
-            self.plot_stem(ax, kwargs['align'], kwargs['height'], neuron_ind)
+            sizes = kwargs['cat']
+            # Generate the align array: 0, 1, 2, ..., number of unique item -1
+            align = np.arange(len(sizes[0]))
+
+            self.plot_stem(ax, align, sizes, neuron_ind)
 
         elif button_type == 'hist':
             num1 = kwargs['num1'][neuron_ind][:kwargs['topn']]
             self.plot_hist(ax, num1, neuron_ind)
 
         elif button_type == 'box':
             # Pre-process continuous variables
@@ -1797,45 +1807,42 @@
             nums = []
             for key in kwargs:
                 if key.startswith('num'):
                     nums.append(kwargs[key][neuron_ind][:kwargs['topn']])
             self.plot_scatter(ax, nums[0], nums[1], neuron_ind)
 
         elif button_type == 'sub_cluster':
-            cluster_data = get_cluster_data(np.transpose(kwargs['input_data']), kwargs['clust'])
+            cluster_data = get_cluster_data(kwargs['data'], kwargs['clust'])
             sub_clust_data = cluster_data[neuron_ind]  # Get the data for the
             self.sub_clustering(sub_clust_data, neuron_ind)
 
         else:
             print(f"Unknown button type: {button_type}")
 
     def determine_button_types(self, **kwargs):
         button_types = []
 
         # Check for categorical data for pie charts
         if 'cat' in kwargs and kwargs['cat'] is not None:
             button_types.append('pie')
-
-        # Check for alignment and height data for stem plots
-        if 'align' in kwargs and 'height' in kwargs:
             button_types.append('stem')
 
         # Check for numerical data and decide which buttons to add
         num_keys = [key for key in kwargs if
                     key.startswith('num') and isinstance(kwargs[key], (list, np.ndarray)) and len(kwargs[key]) > 0]
 
         if num_keys:
             button_types.extend(['hist', 'box', 'violin'])
 
             # Add 'scatter' button only if there are at least two numerical columns
             if len(num_keys) >= 2:
                 button_types.append('scatter')
 
         # Assuming sub-clustering is always an option
-        if 'input_data' in kwargs:
+        if 'data' in kwargs:
             button_types.append('sub_cluster')
 
         return button_types
 
     # Helper function to create charts
     def plot_pie(self, ax, data, neuronNum):
         """
@@ -1937,25 +1944,22 @@
         Returns:
 
         """
         if len(data) <= 1:
             print("There is no enough data to create sub-cluster")
             return
 
-        # Data Prep
-        sub_x = np.transpose(data)
-
         if neuron_ind in self.sub_som:
             print('Sub clustering already done')
             sub_clust = self.sub_som[neuron_ind]
         else:
             # Training Sub Cluster
             sub_clust = SOMPlots((2, 2))
-            sub_clust.init_w(sub_x)
-            sub_clust.train(sub_x, 3, 500, 100)
+            sub_clust.init_w(data, norm_func=self.norm_func)
+            sub_clust.train(data, 3, 500, 100, norm_func=self.norm_func)
 
             self.sub_som[neuron_ind] = sub_clust
 
         # Plot the sub cluster <- Can we h
-        fig, ax, patches, text = sub_clust.hit_hist(sub_x, True, connect_pick_event=False)
+        fig, ax, patches, text = sub_clust.hit_hist(data, True, connect_pick_event=False)
 
         plt.show()
```

### Comparing `nnsom-1.5.9/src/NNSOM/som.py` & `nnsom-1.6.1/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.9/src/NNSOM/utils.py` & `nnsom-1.6.1/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.9/.gitignore` & `nnsom-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.9/pyproject.toml` & `nnsom-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.9"
+version = "1.6.1"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.9/PKG-INFO` & `nnsom-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.9
+Version: 1.6.1
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

