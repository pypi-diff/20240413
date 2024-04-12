# Comparing `tmp/vulcan_utils-1.11.7.tar.gz` & `tmp/vulcan-utils-1.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.7.tar", last modified: Fri Apr 12 21:59:45 2024, max compression
+gzip compressed data, was "vulcan-utils-1.12.0.tar", last modified: Fri Apr 12 23:30:33 2024, max compression
```

## Comparing `vulcan_utils-1.11.7.tar` & `vulcan-utils-1.12.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.398424 vulcan_utils-1.11.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 21:59:37.000000 vulcan_utils-1.11.7/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:59:45.402424 vulcan_utils-1.11.7/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 21:59:45.000000 vulcan_utils-1.11.7/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11.7/LICENSE` & `vulcan-utils-1.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/PKG-INFO` & `vulcan-utils-1.12.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.7
+Version: 1.12.0
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
@@ -24,14 +24,15 @@
 - **Customizable Log Levels**: Flexibility is key with Vulcan Utils, allowing developers to configure log levels to match the operational needs of their applications, from DEBUG for thorough diagnostics to CRITICAL for monitoring urgent issues.
 - **Colored Logs**: To enhance readability and facilitate quicker log analysis, Vulcan Utils supports colored logging, distinguishing log levels with different colors.
 - **Conditional Logging**: This feature offers advanced control over logging operations, enabling logs to be generated based on dynamic runtime conditions, thereby keeping log files concise and focused.
 - **Function Decorators**: Vulcan Utils introduces function decorators for logging, retrying, JSON serialization, and rate limiting, each adding a layer of functionality that enhances method executions with minimal code intrusion.
 - **Advanced Retry Mechanisms**: The retry decorators provide robust error handling by allowing repeated execution of functions upon failure, customizable by attempts and delays, which is invaluable for dealing with transient system or network issues.
 - **Automatic JSON Serialization**: Simplify data interchange in API services and other integrations with automatic JSON serialization of function outputs, streamlining responses and reducing boilerplate code.
 - **Rate Limiting Controls**: Enforce execution limits on functions with the rate limit decorator to manage resource utilization effectively and prevent system overload, which is essential for maintaining service availability and performance under high load.
+- **Caching**: Easy to use interface to connect with a Redis database, store, and retrieve data.
 
 
 ## Installation
 You can install Vulcan Utils via PIP:
 
 ```bash
 pip install vulcan-logger
@@ -123,14 +124,66 @@
 
 @Decorator.rate_limit(limit=3, interval=60)
 def example_rate_limit():
     """A function that is rate limited."""
     return "This function is rate-limited."
 ```
 
+### Caching
+The `Cache` class provides a straightforward way to interact with a Redis server for caching data. It handles connections, as well as setting, getting, deleting, and clearing cache data with exception management to ensure robust operation.
+
+You must have Redis installed and running on the machine to utilize this functionality. You can install Redis with the following command:
+
+```bash
+sudo apt install redis-server
+```
+
+It is also optional, but recommend, to install the Redis CLI package to interact with the Redis database directly. You can install Redis CLI with the following command:
+
+```bash
+sudo apt install redis-tools
+```
+
+#### Initialization
+Create an instance of the `Cache` class by specifying the Redis server's hostname, port, and database index. The instance will attempt to establish a connection immediately. By default if not otherwise specified a `Cache` object will use `localhost` as a host, port `6379`, and `0` db.
+
+```python
+from vulcan_utils.cache import Cache
+
+cache = Cache(host="localhost", port=6379, db=0)
+```
+
+#### Setting Values
+Store values in the cache with an optional expiration time. The value must be JSON-serializable as it will be serialized using the custom Encoder. By default there is no expire time.
+
+```python
+cache.set("user:1", {"name": "John Doe", "age": 30}, expire=3600)
+```
+
+#### Getting Values
+Retrieve values from the cache using a key. If the key exists, the value is returned after being deserialized from JSON; otherwise, `None` is returned.
+
+```python
+user = cache.get("user:1")
+```
+
+#### Deleting Values
+Remove a specific key and its associated value from the cache.
+
+```python
+cache.delete("user:1")
+```
+
+#### Clearing the Cache
+Clear all keys and values in the currently selected Redis database.
+
+```python
+cache.clear()
+```
+
 ### Advanced Configuration
 Vulcan Utils offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
 #### Setting Global Log Level
 Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
 
 _bash_
```

### Comparing `vulcan_utils-1.11.7/tests/test_decorator.py` & `vulcan-utils-1.12.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/tests/test_encoder.py` & `vulcan-utils-1.12.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/tests/test_formatter.py` & `vulcan-utils-1.12.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/tests/test_logger.py` & `vulcan-utils-1.12.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/tests/test_printable.py` & `vulcan-utils-1.12.0/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils/decorator.py` & `vulcan-utils-1.12.0/vulcan_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils/encoder.py` & `vulcan-utils-1.12.0/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils/formatter.py` & `vulcan-utils-1.12.0/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils/logger.py` & `vulcan-utils-1.12.0/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils/printable.py` & `vulcan-utils-1.12.0/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.7/vulcan_utils.egg-info/PKG-INFO` & `vulcan-utils-1.12.0/vulcan_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.7
+Version: 1.12.0
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
@@ -24,14 +24,15 @@
 - **Customizable Log Levels**: Flexibility is key with Vulcan Utils, allowing developers to configure log levels to match the operational needs of their applications, from DEBUG for thorough diagnostics to CRITICAL for monitoring urgent issues.
 - **Colored Logs**: To enhance readability and facilitate quicker log analysis, Vulcan Utils supports colored logging, distinguishing log levels with different colors.
 - **Conditional Logging**: This feature offers advanced control over logging operations, enabling logs to be generated based on dynamic runtime conditions, thereby keeping log files concise and focused.
 - **Function Decorators**: Vulcan Utils introduces function decorators for logging, retrying, JSON serialization, and rate limiting, each adding a layer of functionality that enhances method executions with minimal code intrusion.
 - **Advanced Retry Mechanisms**: The retry decorators provide robust error handling by allowing repeated execution of functions upon failure, customizable by attempts and delays, which is invaluable for dealing with transient system or network issues.
 - **Automatic JSON Serialization**: Simplify data interchange in API services and other integrations with automatic JSON serialization of function outputs, streamlining responses and reducing boilerplate code.
 - **Rate Limiting Controls**: Enforce execution limits on functions with the rate limit decorator to manage resource utilization effectively and prevent system overload, which is essential for maintaining service availability and performance under high load.
+- **Caching**: Easy to use interface to connect with a Redis database, store, and retrieve data.
 
 
 ## Installation
 You can install Vulcan Utils via PIP:
 
 ```bash
 pip install vulcan-logger
@@ -123,14 +124,66 @@
 
 @Decorator.rate_limit(limit=3, interval=60)
 def example_rate_limit():
     """A function that is rate limited."""
     return "This function is rate-limited."
 ```
 
+### Caching
+The `Cache` class provides a straightforward way to interact with a Redis server for caching data. It handles connections, as well as setting, getting, deleting, and clearing cache data with exception management to ensure robust operation.
+
+You must have Redis installed and running on the machine to utilize this functionality. You can install Redis with the following command:
+
+```bash
+sudo apt install redis-server
+```
+
+It is also optional, but recommend, to install the Redis CLI package to interact with the Redis database directly. You can install Redis CLI with the following command:
+
+```bash
+sudo apt install redis-tools
+```
+
+#### Initialization
+Create an instance of the `Cache` class by specifying the Redis server's hostname, port, and database index. The instance will attempt to establish a connection immediately. By default if not otherwise specified a `Cache` object will use `localhost` as a host, port `6379`, and `0` db.
+
+```python
+from vulcan_utils.cache import Cache
+
+cache = Cache(host="localhost", port=6379, db=0)
+```
+
+#### Setting Values
+Store values in the cache with an optional expiration time. The value must be JSON-serializable as it will be serialized using the custom Encoder. By default there is no expire time.
+
+```python
+cache.set("user:1", {"name": "John Doe", "age": 30}, expire=3600)
+```
+
+#### Getting Values
+Retrieve values from the cache using a key. If the key exists, the value is returned after being deserialized from JSON; otherwise, `None` is returned.
+
+```python
+user = cache.get("user:1")
+```
+
+#### Deleting Values
+Remove a specific key and its associated value from the cache.
+
+```python
+cache.delete("user:1")
+```
+
+#### Clearing the Cache
+Clear all keys and values in the currently selected Redis database.
+
+```python
+cache.clear()
+```
+
 ### Advanced Configuration
 Vulcan Utils offers several environment variables to fine-tune logging behavior for your application. You can set these variables before initializing your logger to customize logging output, destination, and file naming.
 
 #### Setting Global Log Level
 Control the log level globally across your application by setting the `VULCAN_LOG_LEVEL` environment variable. This determines the minimum level of messages that will be logged. Available levels are `DEBUG`, `INFO`, `WARNING`, `ERROR`, and `CRITICAL`.
 
 _bash_
```

