# Comparing `tmp/partitionpi-0.0.1.tar.gz` & `tmp/partitionpi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partitionpi-0.0.1.tar", last modified: Mon Mar 25 22:05:58 2024, max compression
+gzip compressed data, was "partitionpi-0.0.2.tar", last modified: Sat Apr 13 21:37:10 2024, max compression
```

## Comparing `partitionpi-0.0.1.tar` & `partitionpi-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 22:05:58.785949 partitionpi-0.0.1/
--rw-rw-rw-   0        0        0     5160 2024-03-25 22:05:58.782951 partitionpi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3687 2024-03-25 21:58:45.000000 partitionpi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 22:05:58.665068 partitionpi-0.0.1/partitionpi/
--rw-rw-rw-   0        0        0       53 2024-03-25 19:03:35.000000 partitionpi-0.0.1/partitionpi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:05:58.781952 partitionpi-0.0.1/partitionpi/domain/
--rw-rw-rw-   0        0        0       69 2024-03-25 00:35:28.000000 partitionpi-0.0.1/partitionpi/domain/__init__.py
--rw-rw-rw-   0        0        0     1669 2024-03-25 19:32:35.000000 partitionpi-0.0.1/partitionpi/domain/base.py
--rw-rw-rw-   0        0        0      322 2024-03-25 02:36:27.000000 partitionpi-0.0.1/partitionpi/domain/math_utils.py
--rw-rw-rw-   0        0        0     4166 2024-03-25 02:33:50.000000 partitionpi-0.0.1/partitionpi/domain/methods.py
--rw-rw-rw-   0        0        0     1431 2024-03-25 00:29:38.000000 partitionpi-0.0.1/partitionpi/domain/operators.py
--rw-rw-rw-   0        0        0     2337 2024-03-25 21:46:58.000000 partitionpi-0.0.1/partitionpi/partition_graph.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:05:58.732981 partitionpi-0.0.1/partitionpi.egg-info/
--rw-rw-rw-   0        0        0     5160 2024-03-25 22:05:58.000000 partitionpi-0.0.1/partitionpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-03-25 22:05:58.000000 partitionpi-0.0.1/partitionpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 22:05:58.000000 partitionpi-0.0.1/partitionpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-25 22:05:58.000000 partitionpi-0.0.1/partitionpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-25 22:05:58.000000 partitionpi-0.0.1/partitionpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 22:05:58.786949 partitionpi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-03-25 20:39:50.000000 partitionpi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:37:10.153661 partitionpi-0.0.2/
+-rw-rw-rw-   0        0        0     5160 2024-04-13 21:37:10.150662 partitionpi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3687 2024-04-13 21:08:03.000000 partitionpi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 21:37:10.015740 partitionpi-0.0.2/partitionpi/
+-rw-rw-rw-   0        0        0       53 2024-03-25 19:03:35.000000 partitionpi-0.0.2/partitionpi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:37:10.149663 partitionpi-0.0.2/partitionpi/domain/
+-rw-rw-rw-   0        0        0       69 2024-03-25 00:35:28.000000 partitionpi-0.0.2/partitionpi/domain/__init__.py
+-rw-rw-rw-   0        0        0     1669 2024-03-25 19:32:35.000000 partitionpi-0.0.2/partitionpi/domain/base.py
+-rw-rw-rw-   0        0        0      322 2024-03-25 02:36:27.000000 partitionpi-0.0.2/partitionpi/domain/math_utils.py
+-rw-rw-rw-   0        0        0     4166 2024-03-25 02:33:50.000000 partitionpi-0.0.2/partitionpi/domain/methods.py
+-rw-rw-rw-   0        0        0     1431 2024-03-25 00:29:38.000000 partitionpi-0.0.2/partitionpi/domain/operators.py
+-rw-rw-rw-   0        0        0     3844 2024-04-13 21:18:52.000000 partitionpi-0.0.2/partitionpi/partition_graph.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:37:10.082702 partitionpi-0.0.2/partitionpi.egg-info/
+-rw-rw-rw-   0        0        0     5160 2024-04-13 21:37:08.000000 partitionpi-0.0.2/partitionpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-04-13 21:37:09.000000 partitionpi-0.0.2/partitionpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 21:37:08.000000 partitionpi-0.0.2/partitionpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-13 21:37:08.000000 partitionpi-0.0.2/partitionpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 21:37:08.000000 partitionpi-0.0.2/partitionpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 21:37:10.154660 partitionpi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      695 2024-04-13 21:29:47.000000 partitionpi-0.0.2/setup.py
```

### Comparing `partitionpi-0.0.1/PKG-INFO` & `partitionpi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partitionpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to handle integer partitions and compute partitional analysis metrics.
 Home-page: https://github.com/luansimoes/partitionpi
 Author: Luan Simões
 Author-email: luansimoes@cos.ufrj.br
 License: MIT License
 Description: # Partition&pi;
         Partition&pi; is a Python library to handle integer partitions as lists and compute partitional analysis metrics.
```

### Comparing `partitionpi-0.0.1/README.md` & `partitionpi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `partitionpi-0.0.1/partitionpi/domain/base.py` & `partitionpi-0.0.2/partitionpi/domain/base.py`

 * *Files identical despite different names*

### Comparing `partitionpi-0.0.1/partitionpi/domain/methods.py` & `partitionpi-0.0.2/partitionpi/domain/methods.py`

 * *Files identical despite different names*

### Comparing `partitionpi-0.0.1/partitionpi/domain/operators.py` & `partitionpi-0.0.2/partitionpi/domain/operators.py`

 * *Files identical despite different names*

### Comparing `partitionpi-0.0.1/partitionpi/partition_graph.py` & `partitionpi-0.0.2/partitionpi/partition_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,48 +30,77 @@
 
         g.nodes[tuple(partition)]['pos'] = (agg(partition), disp(partition))
         g.nodes[tuple(partition)]['label'] = as_tex_str(partition)
         
     return g
 
 
-def draw_complex(obj_to_draw, colors = {'M':'red', 'J':'black'}):
-    '''Plot the partitional complex of the object.'''
+def draw_complex(obj_to_draw, 
+                 colors = {'M':'red', 'J':'black'}, 
+                 styles = {'M':'solid', 'J':'solid'}):
+    '''Plot the partitional complex of the object with custom colors and edge styles.'''
 
     fig, ax = plt.subplots()
 
     if isinstance(obj_to_draw, list):
         obj_to_draw = graph_complex(obj_to_draw)
     
     assert isinstance(obj_to_draw, nx.Graph), 'Object must be a networkx.Graph or a partition.'
 
     pos = nx.get_node_attributes(obj_to_draw, 'pos')
     node_labels = {node : as_tex_str(node) for node in obj_to_draw.nodes}
-    edge_colors = [colors[obj_to_draw[p1][p2]['kinship']] for p1,p2 in obj_to_draw.edges()]
+
+    edges = {'M':[], 'J':[]}
+    [edges[obj_to_draw[e[0]][e[1]]['kinship']].append(e) for e in obj_to_draw.edges()]
+
+
 
     if obj_to_draw.number_of_nodes() < 25:
-        nx.draw(obj_to_draw, 
-            pos=pos, 
-            edge_color=edge_colors, 
-            with_labels=True, 
-            labels=node_labels,
-            ax = ax,
-            node_shape = 'o',
-            node_color = 'white',
-            node_size = 300,
-            font_size = 8)
+        nx.draw_networkx_nodes(obj_to_draw,
+                               pos=pos,
+                               ax=ax,
+                               node_shape='o',
+                               node_color='white',
+                               node_size=300)
+        nx.draw_networkx_labels(obj_to_draw,
+                                pos=pos,
+                                labels=node_labels,
+                                ax=ax,
+                                font_size=8)
+        nx.draw_networkx_edges(obj_to_draw,
+                               pos=pos,
+                               edgelist=edges['M'],
+                               style=styles['M'],
+                               edge_color=colors['M'],
+                               ax=ax)
+        nx.draw_networkx_edges(obj_to_draw,
+                               pos=pos,
+                               edgelist=edges['J'],
+                               style=styles['J'],
+                               edge_color=colors['J'],
+                               ax=ax)
     else:
-        nx.draw(obj_to_draw, 
-            pos=pos, 
-            edge_color=edge_colors, 
-            with_labels=False,
-            ax = ax,
-            node_shape = '.',
-            node_size = 100,
-            node_color = 'green')
+        nx.draw_networkx_nodes(obj_to_draw,
+                               pos=pos,
+                               ax=ax,
+                               node_shape='.',
+                               node_color='green',
+                               node_size=100)
+        nx.draw_networkx_edges(obj_to_draw,
+                               pos=pos,
+                               edgelist=edges['M'],
+                               style=styles['M'],
+                               edge_color=colors['M'],
+                               ax=ax)
+        nx.draw_networkx_edges(obj_to_draw,
+                               pos=pos,
+                               edgelist=edges['J'],
+                               style=styles['J'],
+                               edge_color=colors['J'],
+                               ax=ax)
 
     ax.tick_params(left=True, bottom=True, labelleft=True, labelbottom=True)
     ax.set_xlabel('Agglomeration')
     ax.set_ylabel('Dispersion')
     ax.set_axis_on()
 
     plt.show()
```

### Comparing `partitionpi-0.0.1/partitionpi.egg-info/PKG-INFO` & `partitionpi-0.0.2/partitionpi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partitionpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to handle integer partitions and compute partitional analysis metrics.
 Home-page: https://github.com/luansimoes/partitionpi
 Author: Luan Simões
 Author-email: luansimoes@cos.ufrj.br
 License: MIT License
 Description: # Partition&pi;
         Partition&pi; is a Python library to handle integer partitions as lists and compute partitional analysis metrics.
```

### Comparing `partitionpi-0.0.1/setup.py` & `partitionpi-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(name='partitionpi',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/luansimoes/partitionpi',
     license='MIT License',
     author='Luan Simões',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='luansimoes@cos.ufrj.br',
     keywords='integer-partition texture music partitional analysis',
     description='Python library to handle integer partitions and compute partitional analysis metrics.',
     packages=find_packages(include=['partitionpi', 'partitionpi.*']),
-    install_requires=['networkx','matplotlib'],)
+    install_requires=['networkx>=3','matplotlib>=3'],)
```

