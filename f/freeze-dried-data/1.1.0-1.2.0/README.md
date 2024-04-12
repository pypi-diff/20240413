# Comparing `tmp/freeze_dried_data-1.1.0.tar.gz` & `tmp/freeze_dried_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-1.1.0.tar", last modified: Fri Apr 12 06:59:36 2024, max compression
+gzip compressed data, was "freeze_dried_data-1.2.0.tar", last modified: Fri Apr 12 20:50:06 2024, max compression
```

## Comparing `freeze_dried_data-1.1.0.tar` & `freeze_dried_data-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/LICENSE
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      825 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     3474 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/README.md
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/freeze_dried_data/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/__init__.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     6946 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/freeze_dried_data.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     5277 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/test_freeze_dried_data.py
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      825 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      303 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/SOURCES.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/dependency_links.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/top_level.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/setup.cfg
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      910 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 20:50:06.451779 freeze_dried_data-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      825 2024-04-12 20:50:06.451779 freeze_dried_data-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5786 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 20:50:06.451779 freeze_dried_data-1.2.0/freeze_dried_data/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/freeze_dried_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10243 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/freeze_dried_data/freeze_dried_data.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/freeze_dried_data/test_freeze_dried_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 20:50:06.451779 freeze_dried_data-1.2.0/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      825 2024-04-12 20:50:06.000000 freeze_dried_data-1.2.0/freeze_dried_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-12 20:50:06.000000 freeze_dried_data-1.2.0/freeze_dried_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 20:50:06.000000 freeze_dried_data-1.2.0/freeze_dried_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-12 20:50:06.000000 freeze_dried_data-1.2.0/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 20:50:06.451779 freeze_dried_data-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      910 2024-04-12 20:49:05.000000 freeze_dried_data-1.2.0/setup.py
```

### Comparing `freeze_dried_data-1.1.0/LICENSE` & `freeze_dried_data-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.1.0/PKG-INFO` & `freeze_dried_data-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-1.1.0/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-1.2.0/freeze_dried_data/freeze_dried_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,61 +3,59 @@
 import os
 from typing import Any, Dict, Iterator, Tuple
 import zlib
 import bz2
 import gzip
 # files are stored as: record,record,record,...,last record,index,index_length
 
+def none_compress(data):
+    return data
+
+def none_decompress(data):
+    return data
+
 class FDD:
     """
     A very simple format for machine learning datasets.
     FDD is a simple way to treat datasets on disk like python dictionaries. FDD is built for speed and simplicity.
     Keys can be any objects that are picklable and valid dictionary keys and are stored in memory until the file is closed. Values can be any picklable object, and are stored on disk.
     FDD files can be in either read mode or write mode. Once the file is finalized, it can no longer be modified (i.e., it is "freeze-dried").
     Values are written to disk immediately upon insertion. Keys are written as part of the index when the FDD file is closed.
     """
+
+    CUSTOM_ATTRIBUTE_TAG = 'FDD_CUSTOM_ATTRIBUTES'
+
     def __init__(self, filename: str, write_or_overwrite: bool = False, read_only: bool = False, compression: str = 'none') -> None:
         """
         Initialize a new or existing data file.
 
         :param filename: The file path used for storing data.
         :param write_or_overwrite: If True, any existing file will be overwritten.
         :param read_only: If True, opens the file in read-only mode and raises FileNotFoundError if the file does not exist.
         """
+        self.__dict__['_initializing'] = True # Use self.__dict__ to bypass __setattr__
 
         self.is_open = False
         self.filename = filename
         self.write_or_overwrite = write_or_overwrite
         self.read_only = read_only
         self.compression = compression
+        self.custom_properties = {}
         
-        # Compression functions dictionary
-        compressors = {
-            'zlib': (zlib.compress, zlib.decompress),
-            'bz2': (bz2.compress, bz2.decompress),
-            'gzip': (gzip.compress, gzip.decompress),
-            'none': (lambda x: x, lambda x: x)
-        }
-
-        # if compression is a pair of functions
-        if isinstance(compression, tuple) and len(compression) == 2 and callable(compression[0]) and callable(compression[1]):
-            compressors['custom'] = compression
-            compression = 'custom'
-
-        if compression not in compressors:
-            raise ValueError(f"Unsupported compression type: {compression}")
         
-        self.compressor = compressors[compression][0]
-        self.decompressor = compressors[compression][1]
+        # Compression functions dictionary
+        self.initialize_compression(compression)
 
         # Detects when something like PyTorch DataLoader clones the object.
         os.register_at_fork(after_in_child=self._after_fork)
 
         self._open_file()
 
+        self._initializing = False # now we can use __setattr__
+
     def _open_file(self) -> None:
         """
         Open the file and load the index if in read mode.
         """
         if self.write_or_overwrite and os.path.exists(self.filename):
             os.remove(self.filename)
 
@@ -68,32 +66,111 @@
         self.file = open(self.filename, 'wb+' if self.mode == 'create_mode' else 'rb+')
         
         self.is_open = True
         self.index = self.get_existing_index() if self.mode == 'read_mode' else {}
         if self.mode == 'create_mode':
             self.current_offset = 0
 
+    def initialize_compression(self, compression):
+        # Then use these in your compressors dictionary
+        compressors = {
+            'zlib': (zlib.compress, zlib.decompress),
+            'bz2': (bz2.compress, bz2.decompress),
+            'gzip': (gzip.compress, gzip.decompress),
+            'none': (none_compress, none_decompress)
+        }
+        if isinstance(compression, tuple) and len(compression) == 2 and callable(compression[0]) and callable(compression[1]):
+            compressors['custom'] = compression
+            compression = 'custom'
+        if compression not in compressors:
+            raise ValueError(f"Unsupported compression type: {compression}")
+        self.compressor = compressors[compression][0]
+        self.decompressor = compressors[compression][1]
+
+    def __getattr__(self, name: str) -> Any:
+        """
+        Get an attribute of the FDD instance.
+
+        This method is called when the requested attribute is not found in the normal
+        places (i.e., it's not an instance attribute nor is it found in the class tree).
+        If the attribute is found in the custom_properties dictionary, it is returned.
+        Otherwise, an AttributeError is raised.
+
+        :param name: Name of the attribute being accessed.
+        :return: The value from the custom_properties dictionary.
+        :raises AttributeError: If the attribute is not found.
+        """
+        if name in self.custom_properties:
+            return self.custom_properties[name]
+        raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        """
+        Set an attribute on the FDD instance.
+
+        This method allows setting of attributes directly on the instance. During initialization,
+        attributes are set directly using the standard mechanism. Post-initialization, if the attribute
+        name is not recognized as an existing instance or class attribute, it is added to the custom_properties
+        dictionary, allowing for dynamic attribute assignment.
+
+        :param name: Name of the attribute to set.
+        :param value: Value to assign to the attribute.
+        """
+        if self._initializing:
+            # Use standard attribute setting mechanism during initialization
+            super().__setattr__(name, value)
+        elif name in self.__dict__ or name in type(self).__dict__:
+            # If it's a known attribute, use the standard mechanism
+            super().__setattr__(name, value)
+        else:
+            # Otherwise, store it in custom_properties
+            self.custom_properties[name] = value
+
+    def __delattr__(self, name: str) -> None:
+        """
+        Delete an attribute from the FDD instance.
+
+        If the attribute is part of custom_properties, it is removed. If it's a regular attribute,
+        it is deleted using the standard mechanism. This allows for dynamic management of both
+        built-in and custom attributes.
+
+        :param name: Name of the attribute to delete.
+        """
+        if name in self.custom_properties:
+            # Remove the attribute from custom_properties if it exists there
+            del self.custom_properties[name]
+        else:
+            # Otherwise, delete the attribute using the standard way
+            super().__delattr__(name)
+
+
+
     def get_existing_index(self) -> Dict[Any, Tuple[int, int]]:
         """
         Retrieve the index map from the end of the file.
 
         :return: The index dictionary.
         """
         self.file.seek(-8, 2)  # Move to the last 8 bytes for index size
         index_size = int.from_bytes(self.file.read(8), 'little')
         self.file.seek(-(8 + index_size), 2)
         index_data = self.file.read(index_size)
         index = pkl.loads(self.decompressor(index_data))
+        if self.CUSTOM_ATTRIBUTE_TAG in index:
+            self.custom_properties = index[self.CUSTOM_ATTRIBUTE_TAG]
+            del index[self.CUSTOM_ATTRIBUTE_TAG]
         return index
 
     def close(self) -> None:
         """
         Close the file and save the index if in create mode.
         """
         if self.mode == 'create_mode':
+            if len(self.custom_properties) > 0:
+                self.index[self.CUSTOM_ATTRIBUTE_TAG] = self.custom_properties
             index_data = self.compressor(pkl.dumps(self.index))
             index_data_length = len(index_data)
             self.file.write(index_data)
             self.file.write(index_data_length.to_bytes(8, 'little'))
         
         self.file.close()
         self.is_open = False
```

### Comparing `freeze_dried_data-1.1.0/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-1.2.0/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import unittest
-from freeze_dried_data_with_compression import FDD
+from freeze_dried_data import FDD
 import torch
 from torch.utils.data import DataLoader, Dataset
 import random
 
 class FDDDataset(Dataset):
     def __init__(self, filename):
         self.fdd = FDD(filename, read_only=True)
@@ -99,14 +99,56 @@
         with FDD(self.test_file, write_or_overwrite=True) as fdd:
             fdd['exists'] = 'yes'
         
         with FDD(self.test_file) as fdd:
             with self.assertRaises(KeyError):
                 _ = fdd['does_not_exist']
 
+    def test_custom_attributes(self):
+        # Test setting and getting custom attributes
+        with FDD(self.test_file, write_or_overwrite=True) as fdd:
+            fdd.property_one = 'initial'
+            fdd.property_two = 123
+            fdd.property_one = 'changed'
+            
+            self.assertEqual(fdd.property_one, 'changed')
+            self.assertEqual(fdd.property_two, 123)
+            # add three records
+            fdd['key1'] = 'value1'
+            fdd['key2'] = 'value2'
+            fdd['key3'] = 'value3'
+
+            self.assertEqual(len(fdd), 3)
+
+        with FDD(self.test_file, read_only=True) as fdd:
+            self.assertEqual(fdd.property_one, 'changed')
+            self.assertEqual(fdd.property_two, 123)
+            for k,v in fdd.items():
+                self.assertTrue(k in ['key1', 'key2', 'key3'])
+                self.assertTrue(v in ['value1', 'value2', 'value3'])
+    
+    def test_delete_custom_attributes(self):
+        with FDD(self.test_file, write_or_overwrite=True) as fdd:
+            fdd.some_property = 'value'
+            self.assertEqual(fdd.some_property, 'value')
+
+            # Now delete the property
+            del fdd.some_property
+
+            # Attempting to access it should raise AttributeError
+            with self.assertRaises(AttributeError):
+                _ = fdd.some_property
+
+        # Re-open to check persistence of deletion
+        with FDD(self.test_file, read_only=True) as fdd:
+            # The property should not exist anymore, hence an AttributeError should be raised
+            with self.assertRaises(AttributeError):
+                _ = fdd.some_property
+
+
     def test_dataloader(self):
         # Test DataLoader functionality with multiple workers
         
         # Create a large dataset
         num_records = 100000
         data = {f'key{i}': (f'value{random.random()}', random.random()) for i in range(num_records)}
         with FDD(self.test_file, write_or_overwrite=True) as fdd:
```

### Comparing `freeze_dried_data-1.1.0/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-1.2.0/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-1.1.0/setup.py` & `freeze_dried_data-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='freeze_dried_data',
-    version='1.1.0',
+    version='1.2.0',
     description='A simple format for machine learning datasets',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
     packages=['freeze_dried_data'],
     classifiers=[
```

