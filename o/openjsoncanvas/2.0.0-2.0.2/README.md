# Comparing `tmp/openjsoncanvas-2.0.0.tar.gz` & `tmp/openjsoncanvas-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-2.0.0.tar` & `openjsoncanvas-2.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.0/LICENSE
--rw-r--r--   0        0        0     1937 2024-04-12 14:50:57.072592 openjsoncanvas-2.0.0/README
--rw-r--r--   0        0        0     3460 2024-04-12 16:38:06.883788 openjsoncanvas-2.0.0/openjsoncanvas.py
--rw-r--r--   0        0        0      468 2024-04-12 16:39:57.422261 openjsoncanvas-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-12 16:05:15.952512 openjsoncanvas-2.0.0/run.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1772 2024-04-12 17:30:37.673160 openjsoncanvas-2.0.2/README
+-rw-r--r--   0        0        0     4189 2024-04-12 17:31:25.353722 openjsoncanvas-2.0.2/openjsoncanvas.py
+-rw-r--r--   0        0        0      468 2024-04-12 16:39:57.422261 openjsoncanvas-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.2/PKG-INFO
```

### Comparing `openjsoncanvas-2.0.0/LICENSE` & `openjsoncanvas-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-2.0.0/openjsoncanvas.py` & `openjsoncanvas-2.0.2/openjsoncanvas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-"""A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md"""
-
+"""
+A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
+It allows you to read and write JsonCanvas files in Python, as well as create them from scratch.
+"""
 
 import pydantic, pydantic.alias_generators, typing, pprint, functools, collections.abc
 
-__version__: str = '2.0.0'
+__version__: str = '2.0.2'
 __spec_version__: str = '1.0'
 
 class CanvasData(pydantic.BaseModel, collections.abc.MutableMapping):
+    
+    """Base class for all canvas data classes."""
+    
     def __len__(self) -> int:
         return len(self.__dict__)
 
     def __contains__(self, key: str) -> bool:
         return key in self.__dict__
 
     def __iter__(self) -> typing.Iterator[str]:
@@ -28,47 +33,56 @@
     class Config:
         validate_assignment = True
         validate_default = True
         extra = 'allow'
         
 
 class Node(CanvasData):
+
+    """Base class for all node classes."""
+
     id: str
     type: str
     x: int
     y: int
-    width: int
-    height: int
+    width: int = 100
+    height: int = 100
     color: typing.Optional[str] = None
 
 
 class TextNode(Node):
+    """A node that contains text."""
+    
     text: str
     type: str = 'text'
 
 
 class FileNode(Node):
+    """A node that contains a file."""
     file: str
     type: str = 'file'
     subpath: typing.Optional[str] = None
 
 
 class LinkNode(Node):
+    """A node that contains a link."""
     url: str
     type: str = 'link'
 
 
 class GroupNode(Node):
+    """A node that contains other nodes."""
     type: str = 'group'
     label: typing.Optional[str] = None
     background: typing.Optional[str] = None
     backgroundStyle: typing.Optional[str] = None
 
 
 class Edge(CanvasData):
+    """An edge between two nodes."""
     id: str
     fromNode: str
     toNode: str
     fromSide: typing.Optional[typing.Literal['top', 'right', 'bottom', 'left']] = None
     toSide: typing.Optional[typing.Literal['top', 'right', 'bottom', 'left']] = None
     fromEnd: typing.Optional[typing.Literal['none', 'arrow']] = None
     toEnd: typing.Optional[typing.Literal['none', 'arrow']] = None
@@ -93,16 +107,26 @@
     create_text_node = functools.partialmethod(_create, TextNode, 'nodes')
     create_file_node = functools.partialmethod(_create, FileNode, 'nodes')
     create_link_node = functools.partialmethod(_create, LinkNode, 'nodes')
     create_group_node = functools.partialmethod(_create, GroupNode, 'nodes')
     
     create_edge = functools.partialmethod(_create, Edge, 'edges')
     
+    def to_file(self, path: str):
+        with open(path, 'w') as f:
+            f.write(self.model_dump_json())
+            
+    @classmethod
+    def from_file(cls, path: str):
+        return cls.parse_file(path)
+    
     
 if __name__ == '__main__':
     canvas = Canvas()
     canvas.create_text_node(id='1', x=0, y=0, width=100, height=100, text='Hello, World!')
     canvas.create_file_node(id='2', x=100, y=100, width=100, height=100, file='example.md')
     canvas.create_link_node(id='3', x=200, y=200, width=100, height=100, url='https://example.com')
     canvas.create_group_node(id='4', x=300, y=300, width=100, height=100)
     canvas.create_edge(id='5', fromNode='1', toNode='2', fromEnd='arrow', toEnd='arrow', color='red', label='Edge')
-    pprint.pprint(canvas.dict())
+    
+    canvas.to_file('example.canvas')
+    pprint.pprint(Canvas.from_file('example.canvas').dict())
```

### Comparing `openjsoncanvas-2.0.0/PKG-INFO` & `openjsoncanvas-2.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,50 @@
 Metadata-Version: 2.1
 Name: openjsoncanvas
-Version: 2.0.0
+Version: 2.0.2
 Summary: A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 Author: Alyce Osbourne
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Project-URL: Home, https://github.com/AlyceOsbourne/openjsoncanvas
 
+
 # JsonCanvas Python Implementation
 
-This project provides a Python implementation of the [JsonCanvas format](https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md), designed to enable the creation, manipulation, and serialization of a structured canvas representation. It is built using Python's `dataclasses` for easy data management and supports various node types including Text, File, Link, Group, and Edge elements.
+This project provides a Python implementation of the [JsonCanvas format](https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md), designed to facilitate the creation, manipulation, and visualization of a structured canvas using objects and relations. It leverages Python's `pydantic` library to ensure data validation and management, supporting a range of node and edge types for comprehensive canvas construction.
 
 ## Features
 
-- Define and manipulate canvas elements like Nodes and Edges.
-- Serialize and deserialize canvas data to and from JSON.
-- Easy integration with file systems for reading and writing canvas data.
+- Robust model definitions for canvas elements (Nodes and Edges) with comprehensive validation and default settings via `pydantic`.
+- Dynamic addition and manipulation of various node types including Text, File, Link, Group, and Edge elements.
+- Enhanced canvas operations allowing easy addition of nodes and edges with automated type handling.
+- Serialize canvas structures to standard Python dictionaries for easy integration with other systems.
 
 ## Installation
 
-`pip install openjsoncanvas`
+```bash
+pip install openjsoncanvas
+```
 
 ## Usage
 
 ### Creating a Canvas
 
-You can create a canvas programmatically by adding nodes and edges:
+Instantiate and manipulate a canvas with various nodes and edges:
 
 ```python
-from openjsoncanvas import Canvas, TextNode, LinkNode, Edge
+from openjsoncanvas import Canvas
 
-# Create a new canvas
 canvas = Canvas()
 
-# Add nodes
-canvas.add_node(TextNode(id='1', x=100, y=100, width=200, height=100, text='Hello World'))
-canvas.add_node(LinkNode(id='2', x=300, y=100, width=200, height=100, url='https://example.com'))
-
-# Add an edge
-canvas.add_edge(Edge(id='1', fromNode='1', toNode='2'))
-
-# Serialize to JSON
-json_output = canvas.to_json()
-print(json_output)
-
-# Write to file
-canvas.to_file('example.canvas')
+canvas.create_text_node(id='1', x=0, y=0, width=100, height=100, text='Hello, World!')
+canvas.create_file_node(id='2', x=100, y=100, width=100, height=100, file='example.md')
+canvas.create_link_node(id='3', x=200, y=200, width=100, height=100, url='https://example.com')
+canvas.create_group_node(id='4', x=300, y=300, width=100, height=100)
+canvas.create_edge(id='5', fromNode='1', toNode='2', fromEnd='arrow', toEnd='arrow', color='red', label='Edge')
+
+# you can save and load the canvas to/from a file
+canvas.to_file('my_canvas.canvas')
+canvas = Canvas.from_file('my_canvas.canvas')
 ```
 
-### Loading from JSON
-
-You can load a canvas from a JSON string or file:
-
-```python
-# Load from JSON string
-json_str = '{"nodes": [{"id": "1", "type": "text", "x": 100, "y": 100, "width": 200, "height": 100, "text": "Hello World"}]}'
-loaded_canvas = Canvas.from_json(json_str)
-
-# Load from a file
-loaded_canvas = Canvas.from_file('path_to_your_canvas_file.canvas')
-```
-
-## Contributing
-
-Contributions are welcome! Feel free to open issues or submit pull requests to our repository.
-
-## License
-
-This project is licensed under the MIT License - see the LICENSE file for details.
-
```

