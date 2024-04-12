# Comparing `tmp/wikiwormhole-0.0.1.tar.gz` & `tmp/wikiwormhole-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiwormhole-0.0.1.tar", last modified: Tue Mar 26 13:52:06 2024, max compression
+gzip compressed data, was "wikiwormhole-0.0.2.tar", last modified: Fri Apr 12 19:08:04 2024, max compression
```

## Comparing `wikiwormhole-0.0.1.tar` & `wikiwormhole-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.155359 wikiwormhole-0.0.1/
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     1072 2024-03-26 13:48:30.000000 wikiwormhole-0.0.1/LICENSE
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     1404 2024-03-26 13:52:06.155288 wikiwormhole-0.0.1/PKG-INFO
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     1004 2024-03-26 13:45:10.000000 wikiwormhole-0.0.1/README.md
--rw-r--r--   0 jspencerpittman   (501) staff       (20)       81 2024-03-25 19:38:05.000000 wikiwormhole-0.0.1/pyproject.toml
--rw-r--r--   0 jspencerpittman   (501) staff       (20)      486 2024-03-26 13:52:06.155636 wikiwormhole-0.0.1/setup.cfg
--rw-r--r--   0 jspencerpittman   (501) staff       (20)       37 2024-03-25 19:15:29.000000 wikiwormhole-0.0.1/setup.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     2007 2024-03-26 13:19:27.000000 wikiwormhole-0.0.1/setup_wormhole.py
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.151685 wikiwormhole-0.0.1/src/
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.153275 wikiwormhole-0.0.1/src/wikiwormhole/
--rw-r--r--   0 jspencerpittman   (501) staff       (20)        0 2024-03-25 18:27:50.000000 wikiwormhole-0.0.1/src/wikiwormhole/__init__.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     3782 2024-03-26 12:53:01.000000 wikiwormhole-0.0.1/src/wikiwormhole/title2vec.py
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.154577 wikiwormhole-0.0.1/src/wikiwormhole/traverse/
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     4500 2024-03-25 21:20:14.000000 wikiwormhole-0.0.1/src/wikiwormhole/traverse/graph.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     4116 2024-03-25 21:20:11.000000 wikiwormhole-0.0.1/src/wikiwormhole/traverse/popular.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     6060 2024-03-26 13:42:55.000000 wikiwormhole-0.0.1/src/wikiwormhole/traverse/similar.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)      532 2024-03-25 19:25:41.000000 wikiwormhole-0.0.1/src/wikiwormhole/traverse/traverse.py
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.154852 wikiwormhole-0.0.1/src/wikiwormhole/util/
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     1117 2024-03-25 18:27:50.000000 wikiwormhole-0.0.1/src/wikiwormhole/util/fixedpq.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)      727 2024-03-25 18:27:50.000000 wikiwormhole-0.0.1/src/wikiwormhole/util/sinkset.py
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     3965 2024-03-25 21:19:21.000000 wikiwormhole-0.0.1/src/wikiwormhole/wikiapi.py
-drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-03-26 13:52:06.155056 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/
--rw-r--r--   0 jspencerpittman   (501) staff       (20)     1404 2024-03-26 13:52:06.000000 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/PKG-INFO
--rw-r--r--   0 jspencerpittman   (501) staff       (20)      568 2024-03-26 13:52:06.000000 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/SOURCES.txt
--rw-r--r--   0 jspencerpittman   (501) staff       (20)        1 2024-03-26 13:52:06.000000 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/dependency_links.txt
--rw-r--r--   0 jspencerpittman   (501) staff       (20)       94 2024-03-26 13:52:06.000000 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/requires.txt
--rw-r--r--   0 jspencerpittman   (501) staff       (20)       13 2024-03-26 13:52:06.000000 wikiwormhole-0.0.1/src/wikiwormhole.egg-info/top_level.txt
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.720354 wikiwormhole-0.0.2/
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     1072 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/LICENSE
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     3445 2024-04-12 19:08:04.720282 wikiwormhole-0.0.2/PKG-INFO
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     4140 2024-04-12 19:01:32.000000 wikiwormhole-0.0.2/README.md
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     2985 2024-04-12 19:07:33.000000 wikiwormhole-0.0.2/README_PYPI.md
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)       81 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/pyproject.toml
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)      537 2024-04-12 19:08:04.720665 wikiwormhole-0.0.2/setup.cfg
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)       37 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/setup.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     2007 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/setup_wormhole.py
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.714483 wikiwormhole-0.0.2/src/
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.717183 wikiwormhole-0.0.2/src/wikiwormhole/
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)        0 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/src/wikiwormhole/__init__.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     3782 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/src/wikiwormhole/title2vec.py
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.718770 wikiwormhole-0.0.2/src/wikiwormhole/traverse/
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     4331 2024-04-11 19:44:23.000000 wikiwormhole-0.0.2/src/wikiwormhole/traverse/popular.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     6772 2024-04-11 20:28:23.000000 wikiwormhole-0.0.2/src/wikiwormhole/traverse/similar.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)      905 2024-04-11 19:44:35.000000 wikiwormhole-0.0.2/src/wikiwormhole/traverse/traverse.py
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.719726 wikiwormhole-0.0.2/src/wikiwormhole/util/
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     1117 2024-04-10 20:35:49.000000 wikiwormhole-0.0.2/src/wikiwormhole/util/fixedpq.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     5766 2024-04-03 22:27:34.000000 wikiwormhole-0.0.2/src/wikiwormhole/util/graph.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)      727 2024-04-10 20:36:18.000000 wikiwormhole-0.0.2/src/wikiwormhole/util/sinkset.py
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     3965 2024-04-03 19:15:26.000000 wikiwormhole-0.0.2/src/wikiwormhole/wikiapi.py
+drwxr-xr-x   0 jspencerpittman   (501) staff       (20)        0 2024-04-12 19:08:04.719971 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)     3445 2024-04-12 19:08:04.000000 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/PKG-INFO
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)      579 2024-04-12 19:08:04.000000 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/SOURCES.txt
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)        1 2024-04-12 19:08:04.000000 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/dependency_links.txt
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)       94 2024-04-12 19:08:04.000000 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/requires.txt
+-rw-r--r--   0 jspencerpittman   (501) staff       (20)       13 2024-04-12 19:08:04.000000 wikiwormhole-0.0.2/src/wikiwormhole.egg-info/top_level.txt
```

### Comparing `wikiwormhole-0.0.1/LICENSE` & `wikiwormhole-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/setup_wormhole.py` & `wikiwormhole-0.0.2/setup_wormhole.py`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/title2vec.py` & `wikiwormhole-0.0.2/src/wikiwormhole/title2vec.py`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/traverse/popular.py` & `wikiwormhole-0.0.2/src/wikiwormhole/traverse/popular.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from wikiwormhole.util.sinkset import SinkSet
 from wikiwormhole.traverse.traverse import Traverse
 from wikiwormhole import wikiapi
-from typing import List
-from datetime import datetime
+from typing import List, cast
+from wikiwormhole.util.graph import AbsorbNode
 
 
 class PopularTraverse(Traverse):
     def __init__(self, start_subject: str, pv_config_path: str, explore_per_traversal=5) -> None:
         """
         Constructor for Popular Traversal.
 
@@ -17,23 +17,23 @@
         Args:
             start_subject (str): The root of our search for which all nodes must stem from.
             pv_config_path (str): path to the .yaml file configurations for pageviews API.
             explore_per_traversal (int): number of nodes to randomly explore on each traversal.
         """
         super(PopularTraverse, self).__init__(start_subject)
 
-        self._active_page = wikiapi.generate_wiki_page_from_title(
-            start_subject)
+        self._pv_config_path = pv_config_path
+
+        # Caching of subjects
         self._frontier = SinkSet()
         self._frontier.fill([start_subject])
 
+        # Hyperparameters
         self._explore_per_traversal = explore_per_traversal
 
-        self._pv_config_path = pv_config_path
-
     def traverse(self) -> None:
         """
         Move to the next most popular node.
 
         Algorithm:
         1. Select k random nodes to explore from the SinkSet.
         2. Record each sampled node's outgoing connections in the graph.
@@ -54,26 +54,28 @@
         # Explore each node
         for node in explore:
             # Add outgoing connections to graph for current node
             page = wikiapi.generate_wiki_page_from_title(node)
             for link in wikiapi.retrieve_outgoing_links(page):
                 if not Traverse.valid_page(link.title()):
                     continue
-                self._graph.new_edge(node, link.title())
+                self._graph.new_connection(node, link.title())
                 self._frontier.fill([link.title()])
 
         # Identify most popular node
         max_refs, pop_node = -1, ""
-        for node in self._graph.target_nodes():
+        for node in self._graph.asorb_nodes():
             # Prevent revisiting nodes.
             if node in self._trace:
                 continue
             # If the node has a higher connectivity set it as the most popular node.
-            if self._graph.total_references(node) > max_refs:
-                max_refs = self._graph.total_references(node)
+            num_cnxs = cast(AbsorbNode, self._graph.node(node)
+                            ).total_connections()
+            if num_cnxs > max_refs:
+                max_refs = num_cnxs
                 pop_node = node
 
         # Update state.
         self._trace.append(pop_node)
         self._active_page = wikiapi.generate_wiki_page_from_title(pop_node)
         self._subject = pop_node
 
@@ -95,16 +97,19 @@
         max_views, pop_page = -1, ""
 
         for page in self._trace:
             page = wikiapi.generate_wiki_page_from_title(page)
             try:
                 views = sum(wikiapi.retreive_pageviews(
                     page, self._pv_config_path))
+            except FileNotFoundError as e:
+                print("Please provide valid path for wikiapi configurations.")
+                continue
             except Exception as e:
                 continue
 
             # Does page have the most views.
             if views > max_views:
                 max_views = views
                 pop_page = page
 
-        return self._graph.unravel(pop_page.title())
+        return cast(List[str], self._graph.unravel(pop_page.title()))
```

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/traverse/similar.py` & `wikiwormhole-0.0.2/src/wikiwormhole/traverse/similar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from wikiwormhole import wikiapi
 from wikiwormhole.title2vec import Title2Vec, EmbeddedTitle
 import numpy as np
 from wikiwormhole.traverse.traverse import Traverse
 from wikiwormhole.util.fixedpq import FixedPriorityQueue
+from typing import List, Union
 
 
 class SimilarTraverse(Traverse):
     def __init__(self, start_subject: str, target_subject: str, t2v: Title2Vec, priority_queue_size=10, decay_factor=0.9) -> None:
         """
         Constructor for SimilarTraverse.
 
@@ -19,38 +20,58 @@
             t2v (Title2Vec): a Word2Vec model for embedding titles.
             priority_queue_size (int): size of fixed priority queue. A smaller size promotoes emphasis on
                 depth over breadth.
             decay_factor (float): the decay factor used for calculating similarity between two titles. 
         """
 
         super(SimilarTraverse, self).__init__(start_subject)
-        self._target = target_subject
 
-        self._active_page = wikiapi.generate_wiki_page_from_title(
-            start_subject)
+        self._target_subject = target_subject
+
+        if not wikiapi.generate_wiki_page_from_title(target_subject).exists():
+            raise Exception(
+                'SimilarTraverse: please provide a target page that exists.')
+
         self._t2v = t2v
 
         self._target_embedded = self._t2v.embed_title(target_subject)
+
+        # Caching of subjects
         self._blacklist = list()
         self._sim_scores = dict()
         self._fixpq = FixedPriorityQueue(priority_queue_size, True)
 
+        # Hyperparameters
         self._decay_factor = decay_factor
 
-    def target_found(self) -> bool:
+    def target_reached(self) -> bool:
         """
         Has the target been reached in the graph?
 
         Returns:
             bool: the target has been reached if true.
         """
 
-        return self._graph.node_exists(self._target)
+        return self._graph.node_exists(self._target_subject)
+
+    def path_to_target(self) -> Union[List[str], None]:
+        """
+        Returns the path from the source node to the target.
+
+        Returns:
+            Union[List[str], None]: The path from the source node to the target, if no such
+                path exists return None.
+        """
+
+        if not self._graph.node_exists(self._target_subject):
+            return None
+        else:
+            return self._graph.unravel(self._target_subject)
 
-    def traverse(self):
+    def traverse(self) -> None:
         """
         This algorithm works as follows:
         1. Loop through all outgoing links for the current page.
         2. For each link do steps 3-6
         3. Add link to the graph.
         4. Embed the link using pre-trained Word2Vec model.
         5. Calculate similarity between link and title.
@@ -67,22 +88,22 @@
                 self._attempt_traverse()
                 success_traverse = True
             except Exception:
                 failed_subject = self._trace.pop()
                 prev_subject = self._trace[-1]
 
                 # Undo traversal.
-                self._subject = prev_subject
+                self._active_subject = prev_subject
                 self._active_page = wikiapi.generate_wiki_page_from_title(
                     prev_subject)
 
                 # Remember the failed page.
                 self._blacklist.append(failed_subject)
 
-    def _attempt_traverse(self):
+    def _attempt_traverse(self) -> None:
         """
         This algorithm works as follows:
         1. Loop through all outgoing links for the current page.
         2. For each link do steps 3-6
         3. Add link to the graph.
         4. Embed the link using pre-trained Word2Vec model.
         5. Calculate similarity between link and title.
@@ -97,15 +118,15 @@
             # Don't vist past, failed, or invalid nodes.
             if (title in self._trace or
                 title in self._blacklist or
                     not Traverse.valid_page(title)):
                 continue
 
             # Inform the graph of this new connection
-            self._graph.new_edge(self._subject, title)
+            self._graph.new_connection(self._active_subject, title)
 
             if title not in self._sim_scores.keys():
 
                 # Embed the title.
                 embedded_title = self._t2v.embed_title(title)
                 if len(embedded_title) == 0:
                     continue
@@ -118,18 +139,18 @@
 
             sim_score = self._sim_scores[title]
 
             self._fixpq.push(sim_score, title)
 
         # Move to the most similar page.
         if len(self._fixpq) > 0:
-            _, self._subject = self._fixpq.pop()
+            _, self._active_subject = self._fixpq.pop()
             self._active_page = wikiapi.generate_wiki_page_from_title(
-                self._subject)
-            self._trace.append(self._subject)
+                self._active_subject)
+            self._trace.append(self._active_subject)
         else:
             raise Exception("SimilarTraverse.traverse: no valid pages found.")
 
     def title_sim_score(self, title1: EmbeddedTitle, title2: EmbeddedTitle) -> float:
         """
         For the NLP domain, this code utilizes the cosine similarity.
```

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/util/fixedpq.py` & `wikiwormhole-0.0.2/src/wikiwormhole/util/fixedpq.py`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/util/sinkset.py` & `wikiwormhole-0.0.2/src/wikiwormhole/util/sinkset.py`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole/wikiapi.py` & `wikiwormhole-0.0.2/src/wikiwormhole/wikiapi.py`

 * *Files identical despite different names*

### Comparing `wikiwormhole-0.0.1/src/wikiwormhole.egg-info/SOURCES.txt` & `wikiwormhole-0.0.2/src/wikiwormhole.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
+README_PYPI.md
 pyproject.toml
 setup.cfg
 setup.py
 setup_wormhole.py
 src/wikiwormhole/__init__.py
 src/wikiwormhole/title2vec.py
 src/wikiwormhole/wikiapi.py
 src/wikiwormhole.egg-info/PKG-INFO
 src/wikiwormhole.egg-info/SOURCES.txt
 src/wikiwormhole.egg-info/dependency_links.txt
 src/wikiwormhole.egg-info/requires.txt
 src/wikiwormhole.egg-info/top_level.txt
-src/wikiwormhole/traverse/graph.py
 src/wikiwormhole/traverse/popular.py
 src/wikiwormhole/traverse/similar.py
 src/wikiwormhole/traverse/traverse.py
 src/wikiwormhole/util/fixedpq.py
+src/wikiwormhole/util/graph.py
 src/wikiwormhole/util/sinkset.py
```

