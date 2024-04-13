# Comparing `tmp/openjsoncanvas-2.0.2.tar.gz` & `tmp/openjsoncanvas-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-2.0.2.tar` & `openjsoncanvas-2.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.2/LICENSE
--rw-r--r--   0        0        0     1772 2024-04-12 17:30:37.673160 openjsoncanvas-2.0.2/README
--rw-r--r--   0        0        0     4189 2024-04-12 17:31:25.353722 openjsoncanvas-2.0.2/openjsoncanvas.py
--rw-r--r--   0        0        0      468 2024-04-12 16:39:57.422261 openjsoncanvas-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.3/LICENSE
+-rw-r--r--   0        0        0     1772 2024-04-12 23:27:55.463768 openjsoncanvas-2.0.3/README.md
+-rw-r--r--   0        0        0     4934 2024-04-12 23:27:49.988628 openjsoncanvas-2.0.3/openjsoncanvas.py
+-rw-r--r--   0        0        0      471 2024-04-12 23:28:41.108195 openjsoncanvas-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.3/PKG-INFO
```

### Comparing `openjsoncanvas-2.0.2/LICENSE` & `openjsoncanvas-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-2.0.2/README` & `openjsoncanvas-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-2.0.2/openjsoncanvas.py` & `openjsoncanvas-2.0.3/openjsoncanvas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 It allows you to read and write JsonCanvas files in Python, as well as create them from scratch.
 """
 
 import pydantic, pydantic.alias_generators, typing, pprint, functools, collections.abc
 
-__version__: str = '2.0.2'
+__version__: str = '2.0.3'
 __spec_version__: str = '1.0'
 
 class CanvasData(pydantic.BaseModel, collections.abc.MutableMapping):
     
     """Base class for all canvas data classes."""
     
     def __len__(self) -> int:
@@ -93,28 +93,54 @@
 class Canvas(CanvasData):
     nodes: list[Node] = pydantic.Field(default_factory=list)
     edges: list[Edge] = pydantic.Field(default_factory=list)
     
     def _add(self, prop, obj):
         getattr(self, prop).append(obj)
         return self
+    
+    def _add_many(self, prop, objs):
+        getattr(self, prop).extend(objs)
+        return self
 
     def _create(self, type, prop, **kwargs):
         self._add(prop, type(**kwargs))
         
+    def _delete(self, prop, obj):
+        getattr(self, prop).remove(obj)
+        return self
+    
+    def _delete_many(self, prop, objs):
+        for obj in objs:
+            self._delete(prop, obj)
+        return self
+        
     add_node = functools.partialmethod(_add, 'nodes')
+    add_nodes = functools.partialmethod(_add_many, 'nodes')
     add_edge = functools.partialmethod(_add, 'edges')
+    add_edges = functools.partialmethod(_add_many, 'edges')
 
     create_text_node = functools.partialmethod(_create, TextNode, 'nodes')
     create_file_node = functools.partialmethod(_create, FileNode, 'nodes')
     create_link_node = functools.partialmethod(_create, LinkNode, 'nodes')
     create_group_node = functools.partialmethod(_create, GroupNode, 'nodes')
     
     create_edge = functools.partialmethod(_create, Edge, 'edges')
     
+    delete_node = functools.partialmethod(_delete, 'nodes')
+    delete_edge = functools.partialmethod(_delete, 'edges')
+    
+    delete_nodes = functools.partialmethod(_delete_many, 'nodes')
+    delete_edges = functools.partialmethod(_delete_many, 'edges')
+    
+    def clear_canvas(self):
+        self.nodes.clear()
+        self.edges.clear()
+        return self
+    
     def to_file(self, path: str):
         with open(path, 'w') as f:
             f.write(self.model_dump_json())
             
     @classmethod
     def from_file(cls, path: str):
         return cls.parse_file(path)
@@ -123,10 +149,8 @@
 if __name__ == '__main__':
     canvas = Canvas()
     canvas.create_text_node(id='1', x=0, y=0, width=100, height=100, text='Hello, World!')
     canvas.create_file_node(id='2', x=100, y=100, width=100, height=100, file='example.md')
     canvas.create_link_node(id='3', x=200, y=200, width=100, height=100, url='https://example.com')
     canvas.create_group_node(id='4', x=300, y=300, width=100, height=100)
     canvas.create_edge(id='5', fromNode='1', toNode='2', fromEnd='arrow', toEnd='arrow', color='red', label='Edge')
-    
-    canvas.to_file('example.canvas')
-    pprint.pprint(Canvas.from_file('example.canvas').dict())
+
```

### Comparing `openjsoncanvas-2.0.2/PKG-INFO` & `openjsoncanvas-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openjsoncanvas
-Version: 2.0.2
+Version: 2.0.3
 Summary: A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 Author: Alyce Osbourne
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Project-URL: Home, https://github.com/AlyceOsbourne/openjsoncanvas
```

