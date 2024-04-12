# Comparing `tmp/mgdl-simple-cache-1.2.0.tar.gz` & `tmp/mgdl-simple-cache-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgdl-simple-cache-1.2.0.tar", last modified: Sat Mar 23 23:35:33 2024, max compression
+gzip compressed data, was "mgdl-simple-cache-1.2.1.tar", last modified: Fri Apr 12 23:50:07 2024, max compression
```

## Comparing `mgdl-simple-cache-1.2.0.tar` & `mgdl-simple-cache-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 23:35:33.508483 mgdl-simple-cache-1.2.0/
--rw-rw-rw-   0        0        0     1079 2024-02-14 21:14:34.000000 mgdl-simple-cache-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    11727 2024-03-23 23:35:33.508483 mgdl-simple-cache-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9220 2024-03-20 02:00:58.000000 mgdl-simple-cache-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 23:35:33.508483 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/
--rw-rw-rw-   0        0        0    11727 2024-03-23 23:35:32.000000 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-03-23 23:35:32.000000 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 23:35:32.000000 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-03-23 23:35:32.000000 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-23 23:35:32.000000 mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1429 2024-03-23 23:30:00.000000 mgdl-simple-cache-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-23 23:35:33.524108 mgdl-simple-cache-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-23 23:35:33.376953 mgdl-simple-cache-1.2.0/simple_cache/
--rw-rw-rw-   0        0        0     4273 2024-03-23 23:32:59.000000 mgdl-simple-cache-1.2.0/simple_cache/__init__.py
--rw-rw-rw-   0        0        0      858 2024-03-20 02:00:58.000000 mgdl-simple-cache-1.2.0/simple_cache/cache_data.py
-drwxrwxrwx   0        0        0        0 2024-03-23 23:35:33.423839 mgdl-simple-cache-1.2.0/simple_cache/providers/
--rw-rw-rw-   0        0        0       64 2024-03-23 23:30:00.000000 mgdl-simple-cache-1.2.0/simple_cache/providers/__init__.py
--rw-rw-rw-   0        0        0     6292 2024-03-22 01:00:11.000000 mgdl-simple-cache-1.2.0/simple_cache/providers/deta.py
--rw-rw-rw-   0        0        0     5467 2024-03-23 23:30:00.000000 mgdl-simple-cache-1.2.0/simple_cache/providers/file.py
--rw-rw-rw-   0        0        0     2063 2024-03-23 23:30:00.000000 mgdl-simple-cache-1.2.0/simple_cache/providers/provider.py
-drwxrwxrwx   0        0        0        0 2024-03-23 23:35:33.492858 mgdl-simple-cache-1.2.0/tests/
--rw-rw-rw-   0        0        0      847 2024-03-20 02:00:58.000000 mgdl-simple-cache-1.2.0/tests/test_cache_decorator.py
--rw-rw-rw-   0        0        0     7899 2024-03-20 02:00:58.000000 mgdl-simple-cache-1.2.0/tests/test_deta_provider.py
--rw-rw-rw-   0        0        0     8649 2024-03-23 23:30:00.000000 mgdl-simple-cache-1.2.0/tests/test_file_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:50:07.729924 mgdl-simple-cache-1.2.1/
+-rw-rw-rw-   0        0        0     1079 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    14725 2024-04-12 23:50:07.714283 mgdl-simple-cache-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12218 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 23:50:07.714283 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/
+-rw-rw-rw-   0        0        0    14725 2024-04-12 23:50:07.000000 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-04-12 23:50:07.000000 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 23:50:07.000000 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-12 23:50:07.000000 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 23:50:07.000000 mgdl-simple-cache-1.2.1/mgdl_simple_cache.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1429 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 23:50:07.729924 mgdl-simple-cache-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 23:50:07.645257 mgdl-simple-cache-1.2.1/simple_cache/
+-rw-rw-rw-   0        0        0     4273 2024-04-12 23:44:05.000000 mgdl-simple-cache-1.2.1/simple_cache/__init__.py
+-rw-rw-rw-   0        0        0      858 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/simple_cache/cache_data.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:50:07.676508 mgdl-simple-cache-1.2.1/simple_cache/providers/
+-rw-rw-rw-   0        0        0       64 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/simple_cache/providers/__init__.py
+-rw-rw-rw-   0        0        0     6306 2024-04-12 23:44:05.000000 mgdl-simple-cache-1.2.1/simple_cache/providers/deta.py
+-rw-rw-rw-   0        0        0     5467 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/simple_cache/providers/file.py
+-rw-rw-rw-   0        0        0     2063 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/simple_cache/providers/provider.py
+drwxrwxrwx   0        0        0        0 2024-04-12 23:50:07.714283 mgdl-simple-cache-1.2.1/tests/
+-rw-rw-rw-   0        0        0      847 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/tests/test_cache_decorator.py
+-rw-rw-rw-   0        0        0     7899 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/tests/test_deta_provider.py
+-rw-rw-rw-   0        0        0     8649 2024-04-12 23:34:02.000000 mgdl-simple-cache-1.2.1/tests/test_file_provider.py
```

### Comparing `mgdl-simple-cache-1.2.0/LICENSE` & `mgdl-simple-cache-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/PKG-INFO` & `mgdl-simple-cache-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,54 @@
-Metadata-Version: 2.1
-Name: mgdl-simple-cache
-Version: 1.2.0
-Summary: Simple Cache is a lightweight cache manager designed to simplify caching operations using providers. It offers a convenient way to store and retrieve cached data efficiently in Python applications.
-Author-email: Adaías Magdiel <eu@adaiasmagdiel.com>
-License: Copyright (c) 2024 Adaías Magdiel
-        
-        Permission is hereby granted, free of charge, to any person obtaining
-        a copy of this software and associated documentation files (the
-        "Software"), to deal in the Software without restriction, including
-        without limitation the rights to use, copy, modify, merge, publish,
-        distribute, sublicense, and/or sell copies of the Software, and to
-        permit persons to whom the Software is furnished to do so, subject to
-        the following conditions:
-        
-        The above copyright notice and this permission notice shall be
-        included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-        NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-        LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-        WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/AdaiasMagdiel/simple-cache
-Project-URL: Issues, https://github.com/AdaiasMagdiel/simple-cache/issues
-Keywords: cache,caching,deta,deta space,development,utility,tool
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: deta
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-
 # Simple Cache
 
 [![PyPI version](https://badge.fury.io/py/mgdl-simple-cache.svg)](https://badge.fury.io/py/mgdl-simple-cache)
 ![License](https://img.shields.io/badge/license-MIT-blue)
 
-Simple Cache is a lightweight cache manager designed to simplify caching operations using Deta Base. It offers a convenient way to store and retrieve cached data efficiently in Python applications.
+Simple Cache is a lightweight caching manager crafted to streamline caching operations using various providers. It provides a convenient solution for storing and efficiently retrieving cached data within Python applications. It's highly extensible, allowing you to enhance its functionality with custom providers tailored to your specific use cases. Additionally, creating a new provider is straightforward and seamless.
+
+## Table of Contents
+
+-   [Installation](#installation)
+-   [Purpose](#purpose)
+-   [Available Providers](#available-providers)
+-   [Usage](#usage)
+    -   [Get Data](#get-data)
+    -   [Set Data](#set-data)
+    -   [Set Data Validation](#set-data-validation)
+-   [Documentation](#documentation)
+    -   [SimpleCache](#simplecache)
+    -   [Decorator `attach`](#decorator-attach)
+        -   [How to Use](#how-to-use)
+        -   [Decorator Documentation](#decorator-documentation)
+    -   [Providers](#providers)
+        -   [Provider (ABC)](#provider-abc)
+        -   [DetaProvider](#detaprovider)
+        -   [FileProvider](#fileprovider)
+-   [Testing](#testing)
+    -   [Coverage](#coverage)
+-   [License](#license)
+-   [Contribution](#contribution)
 
 ## Installation
 
 Install Simple Cache via pip:
 
 ```bash
 pip install mgdl-simple-cache
 ```
 
 ## Purpose
 
-In today's data-driven applications, caching plays a crucial role in enhancing performance by reducing the need to repeatedly fetch data from external sources. Simple Cache aims to streamline this process by providing a user-friendly interface for managing cached data, backed by Deta Base, a fast and scalable database service.
+In modern data-driven applications, caching plays a pivotal role in boosting performance by minimizing the necessity to frequently retrieve data from external sources. Simple Cache endeavors to simplify this procedure by offering a user-friendly interface for effectively managing cached data.
+
+## Available Providers
+
+-   **[DetaProvider](#detaprovider)**: Use [Deta Base](https://deta.space/docs/en/build/reference/deta-base/) service to manage the cache.
+
+-   **[FileProvider](#fileprovider)**: Manage the cache in the file system using Python's pickle objects.
 
 ## Usage
 
 To use the Simple Cache library, follow these steps:
 
 1. **Choose a Provider**: Simple Cache provides different providers for storing cache data. See all available providers [here](#providers). Alternatively, you can implement your own provider by subclassing the `Provider` abstract class.
 
@@ -84,15 +66,29 @@
 
 ```python
 from simple_cache import SimpleCache
 
 cache = SimpleCache(provider)
 ```
 
-5. **Usage**:
+It's possible to initialize the Provider with no arguments and initialize the Provider later using the SimpleCache instance:
+
+```python
+from simple_cache import SimpleCache
+from simple_cache.providers import FileProvider
+
+provider = FileProvider()
+cache = SimpleCache(provider=provider)
+
+...
+
+cache.init(cache_dir=Path('path/to/directory')) # This will set the cache directory in FileProvider
+```
+
+4. **Usage**:
 
     - **Get Data**: To retrieve data from the cache, use the `get` method. If the data is not found in the cache or has expired, you can provide a callback function to generate the data and set it in the cache:
 
     ```python
     data = cache.get(key="some_key", action=some_function, expire_in=timedelta(minutes=5))
     ```
 
@@ -134,30 +130,33 @@
 from simple_cache.providers import DetaProvider
 
 # Initialize the cache provider
 provider = DetaProvider(deta_key="your_deta_project_key", table_name="cache_table")
 cache = SimpleCache(provider)
 
 # Define a function that you want to cache
-@cache.attach(key="my_function_result", expire_in=timedelta(minutes=5))
+@cache.attach(key="my_function_result", expire_in=timedelta(minutes=5)) # The expire_in argument is optional
 def my_function():
     # Simulate an operation that is time or resource-intensive
     result = "Result of the function"
     return result
 
 # The first call to the function will store the result in the cache
 print(my_function())
 
 # Subsequent calls within the expiration time will use the cached result
 print(my_function())
+
+# To invalidate the cache just use the set_validate function
+cache.set_validate(key="my_function_result", valid=False)
 ```
 
 In this example, the function `my_function` is decorated with `@cache.attach`, which means that its result will be stored in the cache with the key `"my_function_result"` and will expire after 5 minutes. On the first call to the function, the result is calculated and stored in the cache. On subsequent calls within the expiration time, the cached result is returned, avoiding the need to recalculate the result.
 
-#### Documentation
+#### Decorator Documentation
 
 -   `attach(self, key: str, expire_in: Optional[timedelta] = None)`: Decorator to store the result of a function in the cache.
     -   `key (str)`: The unique key for the cache.
     -   `expire_in (Optional[timedelta])`: The expiration time for the cache.
 
 This decorator is an efficient way to improve the performance of your Python applications, reducing the need for repetitive and resource-intensive operations.
 
@@ -166,26 +165,36 @@
 #### Provider (ABC)
 
 The `Provider` class is an abstract base class defining the interface for cache providers. It includes the following abstract methods:
 
 -   `init(self, **kwargs)`: Initialize the provider with the given parameters. This method should be implemented by subclasses.
 -   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieve data from the cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
 -   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Set data in the cache with the specified key and value. Optionally, you can specify an expiration time for the data.
--   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Mark data in the cache as valid or invalid.
+-   `set_validate(self, key: str, valid: bool, silent: bool = True)
 
 #### DetaProvider
 
-The `DetaProvider` class is a concrete implementation of the `Provider` interface that stores cache data in Deta databases. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
+The `DetaProvider` class is a concrete implementation of the `Provider` interface that stores cache data in Deta Base. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
 
 -   `__init__(self, deta_key: Optional[str] = None, table_name: Optional[str] = None)`: Initialize the Deta provider with the specified Deta project key and table name.
 -   `init(self, **kwargs) -> None`: Initialize the Deta provider with the given parameters. If no table name is provided, a default table name is used.
 -   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieve data from the Deta cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
 -   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Set data in the Deta cache with the specified key and value. Optionally, you can specify an expiration time for the data.
 -   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Mark data in the Deta cache as valid or invalid.
 
+#### FileProvider
+
+The `FileProvider` class is a concrete implementation of the `Provider` interface that stores cache data in files on the local file system using Python's pickle system. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
+
+-   `__init__(self, cache_dir: Optional[PathLike] = None)`: Initializes the FileProvider with the specified cache directory.
+-   `init(self, **kwargs) -> None`: Initializes the FileProvider with the given parameters. The parameters are the same from the constructor.
+-   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieves data from the file-based cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
+-   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Sets data in the file-based cache with the specified key and value. Optionally, you can specify an expiration time for the data.
+-   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Marks data in the file-based cache as valid or invalid.
+
 ## Testing
 
 If you wish to contribute to this project, simply install the development dependencies:
 
 ```bash
 pip install -r requirements.dev.txt
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mgdl-simple-cache-1.2.0/mgdl_simple_cache.egg-info/PKG-INFO` & `mgdl-simple-cache-1.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgdl-simple-cache
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple Cache is a lightweight cache manager designed to simplify caching operations using providers. It offers a convenient way to store and retrieve cached data efficiently in Python applications.
 Author-email: Adaías Magdiel <eu@adaiasmagdiel.com>
 License: Copyright (c) 2024 Adaías Magdiel
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -46,27 +46,56 @@
 Requires-Dist: pytest-cov; extra == "dev"
 
 # Simple Cache
 
 [![PyPI version](https://badge.fury.io/py/mgdl-simple-cache.svg)](https://badge.fury.io/py/mgdl-simple-cache)
 ![License](https://img.shields.io/badge/license-MIT-blue)
 
-Simple Cache is a lightweight cache manager designed to simplify caching operations using Deta Base. It offers a convenient way to store and retrieve cached data efficiently in Python applications.
+Simple Cache is a lightweight caching manager crafted to streamline caching operations using various providers. It provides a convenient solution for storing and efficiently retrieving cached data within Python applications. It's highly extensible, allowing you to enhance its functionality with custom providers tailored to your specific use cases. Additionally, creating a new provider is straightforward and seamless.
+
+## Table of Contents
+
+-   [Installation](#installation)
+-   [Purpose](#purpose)
+-   [Available Providers](#available-providers)
+-   [Usage](#usage)
+    -   [Get Data](#get-data)
+    -   [Set Data](#set-data)
+    -   [Set Data Validation](#set-data-validation)
+-   [Documentation](#documentation)
+    -   [SimpleCache](#simplecache)
+    -   [Decorator `attach`](#decorator-attach)
+        -   [How to Use](#how-to-use)
+        -   [Decorator Documentation](#decorator-documentation)
+    -   [Providers](#providers)
+        -   [Provider (ABC)](#provider-abc)
+        -   [DetaProvider](#detaprovider)
+        -   [FileProvider](#fileprovider)
+-   [Testing](#testing)
+    -   [Coverage](#coverage)
+-   [License](#license)
+-   [Contribution](#contribution)
 
 ## Installation
 
 Install Simple Cache via pip:
 
 ```bash
 pip install mgdl-simple-cache
 ```
 
 ## Purpose
 
-In today's data-driven applications, caching plays a crucial role in enhancing performance by reducing the need to repeatedly fetch data from external sources. Simple Cache aims to streamline this process by providing a user-friendly interface for managing cached data, backed by Deta Base, a fast and scalable database service.
+In modern data-driven applications, caching plays a pivotal role in boosting performance by minimizing the necessity to frequently retrieve data from external sources. Simple Cache endeavors to simplify this procedure by offering a user-friendly interface for effectively managing cached data.
+
+## Available Providers
+
+-   **[DetaProvider](#detaprovider)**: Use [Deta Base](https://deta.space/docs/en/build/reference/deta-base/) service to manage the cache.
+
+-   **[FileProvider](#fileprovider)**: Manage the cache in the file system using Python's pickle objects.
 
 ## Usage
 
 To use the Simple Cache library, follow these steps:
 
 1. **Choose a Provider**: Simple Cache provides different providers for storing cache data. See all available providers [here](#providers). Alternatively, you can implement your own provider by subclassing the `Provider` abstract class.
 
@@ -84,15 +113,29 @@
 
 ```python
 from simple_cache import SimpleCache
 
 cache = SimpleCache(provider)
 ```
 
-5. **Usage**:
+It's possible to initialize the Provider with no arguments and initialize the Provider later using the SimpleCache instance:
+
+```python
+from simple_cache import SimpleCache
+from simple_cache.providers import FileProvider
+
+provider = FileProvider()
+cache = SimpleCache(provider=provider)
+
+...
+
+cache.init(cache_dir=Path('path/to/directory')) # This will set the cache directory in FileProvider
+```
+
+4. **Usage**:
 
     - **Get Data**: To retrieve data from the cache, use the `get` method. If the data is not found in the cache or has expired, you can provide a callback function to generate the data and set it in the cache:
 
     ```python
     data = cache.get(key="some_key", action=some_function, expire_in=timedelta(minutes=5))
     ```
 
@@ -134,30 +177,33 @@
 from simple_cache.providers import DetaProvider
 
 # Initialize the cache provider
 provider = DetaProvider(deta_key="your_deta_project_key", table_name="cache_table")
 cache = SimpleCache(provider)
 
 # Define a function that you want to cache
-@cache.attach(key="my_function_result", expire_in=timedelta(minutes=5))
+@cache.attach(key="my_function_result", expire_in=timedelta(minutes=5)) # The expire_in argument is optional
 def my_function():
     # Simulate an operation that is time or resource-intensive
     result = "Result of the function"
     return result
 
 # The first call to the function will store the result in the cache
 print(my_function())
 
 # Subsequent calls within the expiration time will use the cached result
 print(my_function())
+
+# To invalidate the cache just use the set_validate function
+cache.set_validate(key="my_function_result", valid=False)
 ```
 
 In this example, the function `my_function` is decorated with `@cache.attach`, which means that its result will be stored in the cache with the key `"my_function_result"` and will expire after 5 minutes. On the first call to the function, the result is calculated and stored in the cache. On subsequent calls within the expiration time, the cached result is returned, avoiding the need to recalculate the result.
 
-#### Documentation
+#### Decorator Documentation
 
 -   `attach(self, key: str, expire_in: Optional[timedelta] = None)`: Decorator to store the result of a function in the cache.
     -   `key (str)`: The unique key for the cache.
     -   `expire_in (Optional[timedelta])`: The expiration time for the cache.
 
 This decorator is an efficient way to improve the performance of your Python applications, reducing the need for repetitive and resource-intensive operations.
 
@@ -166,26 +212,36 @@
 #### Provider (ABC)
 
 The `Provider` class is an abstract base class defining the interface for cache providers. It includes the following abstract methods:
 
 -   `init(self, **kwargs)`: Initialize the provider with the given parameters. This method should be implemented by subclasses.
 -   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieve data from the cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
 -   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Set data in the cache with the specified key and value. Optionally, you can specify an expiration time for the data.
--   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Mark data in the cache as valid or invalid.
+-   `set_validate(self, key: str, valid: bool, silent: bool = True)
 
 #### DetaProvider
 
-The `DetaProvider` class is a concrete implementation of the `Provider` interface that stores cache data in Deta databases. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
+The `DetaProvider` class is a concrete implementation of the `Provider` interface that stores cache data in Deta Base. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
 
 -   `__init__(self, deta_key: Optional[str] = None, table_name: Optional[str] = None)`: Initialize the Deta provider with the specified Deta project key and table name.
 -   `init(self, **kwargs) -> None`: Initialize the Deta provider with the given parameters. If no table name is provided, a default table name is used.
 -   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieve data from the Deta cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
 -   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Set data in the Deta cache with the specified key and value. Optionally, you can specify an expiration time for the data.
 -   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Mark data in the Deta cache as valid or invalid.
 
+#### FileProvider
+
+The `FileProvider` class is a concrete implementation of the `Provider` interface that stores cache data in files on the local file system using Python's pickle system. It includes methods to initialize the provider, retrieve data from the cache, set data in the cache, and mark data as valid or invalid.
+
+-   `__init__(self, cache_dir: Optional[PathLike] = None)`: Initializes the FileProvider with the specified cache directory.
+-   `init(self, **kwargs) -> None`: Initializes the FileProvider with the given parameters. The parameters are the same from the constructor.
+-   `get(self, key: str, action: Callable[[], str], expire_in: Optional[timedelta] = None) -> CacheData`: Retrieves data from the file-based cache with the specified key. If the data is not found or has expired, the provided action function is executed to generate the data.
+-   `set(self, key: str, value: Any, expire_in: Optional[timedelta] = None) -> CacheData`: Sets data in the file-based cache with the specified key and value. Optionally, you can specify an expiration time for the data.
+-   `set_validate(self, key: str, valid: bool, silent: bool = True) -> None`: Marks data in the file-based cache as valid or invalid.
+
 ## Testing
 
 If you wish to contribute to this project, simply install the development dependencies:
 
 ```bash
 pip install -r requirements.dev.txt
 ```
```

### Comparing `mgdl-simple-cache-1.2.0/pyproject.toml` & `mgdl-simple-cache-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/simple_cache/__init__.py` & `mgdl-simple-cache-1.2.1/simple_cache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 from functools import wraps
 from typing import Any, Callable, Optional
 
 from simple_cache.cache_data import CacheData
 from .providers.provider import Provider
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 class SimpleCache(Provider):
     """
     A class that provides caching functionality for a given provider.
 
     Attributes:
```

### Comparing `mgdl-simple-cache-1.2.0/simple_cache/cache_data.py` & `mgdl-simple-cache-1.2.1/simple_cache/cache_data.py`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/simple_cache/providers/deta.py` & `mgdl-simple-cache-1.2.1/simple_cache/providers/deta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import UTC, datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Any, Callable, Optional
 from deta import Deta, _Base
 from simple_cache.cache_data import CacheData
 from simple_cache.providers.provider import Provider
 
 
 class DetaProvider(Provider):
@@ -160,15 +160,15 @@
 
         if not key:
             raise ValueError("Key can not be None or empty")
 
         data = {
             "value": value,
             "valid": True,
-            "created_at": datetime.now(UTC).isoformat(),
+            "created_at": datetime.now(timezone.utc).isoformat(),
         }
 
         if expire_in:
             if not isinstance(expire_in, timedelta):
                 raise TypeError(
                     "'expire_in' must be a 'timedelta' with the expire time"
                 )
```

### Comparing `mgdl-simple-cache-1.2.0/simple_cache/providers/file.py` & `mgdl-simple-cache-1.2.1/simple_cache/providers/file.py`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/simple_cache/providers/provider.py` & `mgdl-simple-cache-1.2.1/simple_cache/providers/provider.py`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/tests/test_cache_decorator.py` & `mgdl-simple-cache-1.2.1/tests/test_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/tests/test_deta_provider.py` & `mgdl-simple-cache-1.2.1/tests/test_deta_provider.py`

 * *Files identical despite different names*

### Comparing `mgdl-simple-cache-1.2.0/tests/test_file_provider.py` & `mgdl-simple-cache-1.2.1/tests/test_file_provider.py`

 * *Files identical despite different names*

