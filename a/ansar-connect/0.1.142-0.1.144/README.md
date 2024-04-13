# Comparing `tmp/ansar-connect-0.1.142.tar.gz` & `tmp/ansar-connect-0.1.144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.142.tar", last modified: Sat Apr 13 00:36:32 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.144.tar", last modified: Sat Apr 13 03:18:51 2024, max compression
```

## Comparing `ansar-connect-0.1.142.tar` & `ansar-connect-0.1.144.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.142/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.142/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.142/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.142/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar-connect-0.1.142/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar-connect-0.1.142/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar-connect-0.1.142/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar-connect-0.1.142/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-13 00:36:29.000000 ansar-connect-0.1.142/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14145 2024-04-12 23:59:12.000000 ansar-connect-0.1.142/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78053 2024-04-12 14:58:30.000000 ansar-connect-0.1.142/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.142/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.142/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.142/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.142/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.142/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.142/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.142/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.142/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.142/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar-connect-0.1.142/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar-connect-0.1.142/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.142/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.142/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.142/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar-connect-0.1.142/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.482549 ansar-connect-0.1.144/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.144/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 03:18:51.482549 ansar-connect-0.1.144/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.144/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.144/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-13 03:18:51.482549 ansar-connect-0.1.144/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.144/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.478549 ansar-connect-0.1.144/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.478549 ansar-connect-0.1.144/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.478549 ansar-connect-0.1.144/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar-connect-0.1.144/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar-connect-0.1.144/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar-connect-0.1.144/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar-connect-0.1.144/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.482549 ansar-connect-0.1.144/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-13 03:18:48.000000 ansar-connect-0.1.144/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14145 2024-04-12 23:59:12.000000 ansar-connect-0.1.144/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar-connect-0.1.144/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.144/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.144/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.144/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.144/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.144/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.144/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.144/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.144/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.144/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar-connect-0.1.144/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar-connect-0.1.144/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38274 2024-04-13 01:53:06.000000 ansar-connect-0.1.144/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.144/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.144/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar-connect-0.1.144/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 03:18:51.482549 ansar-connect-0.1.144/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-13 03:18:51.000000 ansar-connect-0.1.144/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.142/LICENSE` & `ansar-connect-0.1.144/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/PKG-INFO` & `ansar-connect-0.1.144/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.142
+Version: 0.1.144
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.142/README.md` & `ansar-connect-0.1.144/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/pyproject.toml` & `ansar-connect-0.1.144/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/setup.py` & `ansar-connect-0.1.144/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.144/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.144/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.144/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.144/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/__init__.py` & `ansar-connect-0.1.144/src/ansar/connect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 2c4006fba4c8bd897b18d26d3860290eab631df7
-Version: 0.1.141 (2024-04-13@12:36:29+NZST)
+Commit: d1f798431e1b56d68d566a69d76e11f27e4ade50
+Version: 0.1.143 (2024-04-13@15:18:48+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.142/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.144/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/directory.py` & `ansar-connect-0.1.144/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1808,15 +1808,15 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_PEERING_T2(self, message):
-	key = self.opened_route.key
+	key = self.route.key
 	name = key_service(key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot loop to {name} ({reason})')
 	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
@@ -1836,15 +1836,15 @@
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return CONNECTION_LATCHING
 
 def SubscriberLoop_CONNECTION_LOOPING_T1(self, message):
-	key = self.opened_route.key
+	key = self.route.key
 	name = key_service(key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot loop to {name} ({reason})')
 	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_peer()
@@ -1948,15 +1948,15 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_RELAY_PEERING_T2(self, message):
-	key = self.opened_route.key
+	key = self.route.key
 	name = key_service(key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
@@ -1976,15 +1976,15 @@
 	self.complete(True)
 
 def SubscriberLoop_RELAY_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return RELAY_LATCHING
 
 def SubscriberLoop_RELAY_LOOPING_T1(self, message):
-	key = self.opened_route.key
+	key = self.route.key
 	name = key_service(key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_relay()
```

### Comparing `ansar-connect-0.1.142/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.144/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.144/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/group_if.py` & `ansar-connect-0.1.144/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/grouping.py` & `ansar-connect-0.1.144/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/moving.py` & `ansar-connect-0.1.144/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/networking.py` & `ansar-connect-0.1.144/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.144/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/node.py` & `ansar-connect-0.1.144/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.144/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/procedure.py` & `ansar-connect-0.1.144/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/product.py` & `ansar-connect-0.1.144/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/socketry.py` & `ansar-connect-0.1.144/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 #
 #
 # server_context = ssl.create_default_context()
 #server_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
 #erver_context.load_cert_chain(CERTIFICATE_FILE, keyfile=KEY_FILE)
 
-#tls_client_context = ssl.create_default_context()
+TLS_CLIENT_CONTEXT = ssl.create_default_context()
 #tls_client_context.load_verify_locations(CERT)
 #
 #
 LOCAL_HOST = '127.0.0.1'
 
 class HostPort(object):
 	def __init__(self, host=None, port=None):
@@ -767,16 +767,16 @@
 		client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 		client.setblocking(False)
 	except socket.error as e:
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 		return
 
 	if isinstance(m.encrypted, TlsClient):
-		context = ssl.create_default_context()
-		client = context.wrap_socket(client, server_side=False, do_handshake_on_connect=False, server_hostname=m.encrypted.SNI)
+		# context = ssl.create_default_context()
+		client = TLS_CLIENT_CONTEXT.wrap_socket(client, server_side=False, do_handshake_on_connect=False, server_hostname=m.encrypted.SNI)
 		self.trace(f'Encrypting as TLS client "{m.encrypted.SNI}"')
 
 	def client_not_connected(e):
 		client.close()
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 
 	try:
```

### Comparing `ansar-connect-0.1.142/src/ansar/connect/standard.py` & `ansar-connect-0.1.144/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/transporting.py` & `ansar-connect-0.1.144/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar/connect/wan.py` & `ansar-connect-0.1.144/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.142/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.144/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.142
+Version: 0.1.144
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.142/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.144/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

