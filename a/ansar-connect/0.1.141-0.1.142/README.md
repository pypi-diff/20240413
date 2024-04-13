# Comparing `tmp/ansar-connect-0.1.141.tar.gz` & `tmp/ansar-connect-0.1.142.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.141.tar", last modified: Sat Apr 13 00:30:15 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.142.tar", last modified: Sat Apr 13 00:36:32 2024, max compression
```

## Comparing `ansar-connect-0.1.141.tar` & `ansar-connect-0.1.142.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.141/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.141/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.141/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.141/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar-connect-0.1.141/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar-connect-0.1.141/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.141/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar-connect-0.1.141/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-13 00:30:11.000000 ansar-connect-0.1.141/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14145 2024-04-12 23:59:12.000000 ansar-connect-0.1.141/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78053 2024-04-12 14:58:30.000000 ansar-connect-0.1.141/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.141/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.141/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.141/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.141/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.141/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.141/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.141/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.141/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.141/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33283 2024-04-13 00:13:16.000000 ansar-connect-0.1.141/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar-connect-0.1.141/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.141/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.141/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.141/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar-connect-0.1.141/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.142/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.142/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.142/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.142/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar-connect-0.1.142/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar-connect-0.1.142/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar-connect-0.1.142/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar-connect-0.1.142/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-13 00:36:29.000000 ansar-connect-0.1.142/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14145 2024-04-12 23:59:12.000000 ansar-connect-0.1.142/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78053 2024-04-12 14:58:30.000000 ansar-connect-0.1.142/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.142/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.142/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.142/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.142/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.142/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.142/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.142/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.142/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.142/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar-connect-0.1.142/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar-connect-0.1.142/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.142/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.142/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.142/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar-connect-0.1.142/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:36:32.180365 ansar-connect-0.1.142/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-13 00:36:32.000000 ansar-connect-0.1.142/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.141/LICENSE` & `ansar-connect-0.1.142/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/PKG-INFO` & `ansar-connect-0.1.142/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.141
+Version: 0.1.142
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.141/README.md` & `ansar-connect-0.1.142/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/pyproject.toml` & `ansar-connect-0.1.142/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/setup.py` & `ansar-connect-0.1.142/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.142/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.142/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.142/src/ansar/command/ansar_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,15 @@
 		hb = hr.home
 		if hb.role_exists(self.main_role):
 			tr = hb.open_role(self.main_role, None, None, ar.NodeProperties())
 			if series(hr.properties.retry) or series(tr.properties.retry):
 				r = ar.Rejected(forwarding_retry=(f'main role "{self.main_role}" is configured to retry', 'not supported'))
 				self.complete(r)
 
-	if self.settings.SNI:
-		encrypted_above = ar.TlsClient(SNI=self.settings.SNI)
-	else:
-		encrypted_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
 	self.assign(a, None)
 	self.directory = a
 	return OPENING
 
 def Group_OPENING_HostPort(self, message):
 	self.directory_ipp = message
 	self.group_start = ar.world_now()
```

### Comparing `ansar-connect-0.1.141/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.142/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/__init__.py` & `ansar-connect-0.1.142/src/ansar/connect/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 136b4a4baf8dcb69e113a01b3b2df9d25a267dac
-Version: 0.1.140 (2024-04-13@12:30:11+NZST)
+Commit: 2c4006fba4c8bd897b18d26d3860290eab631df7
+Version: 0.1.141 (2024-04-13@12:36:29+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.141/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.142/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/directory.py` & `ansar-connect-0.1.142/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.142/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.142/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/group_if.py` & `ansar-connect-0.1.142/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/grouping.py` & `ansar-connect-0.1.142/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/moving.py` & `ansar-connect-0.1.142/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/networking.py` & `ansar-connect-0.1.142/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.142/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/node.py` & `ansar-connect-0.1.142/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.142/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/procedure.py` & `ansar-connect-0.1.142/src/ansar/connect/procedure.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,19 +205,15 @@
 		e = ar.Failed(group_running=(f'group "{group}" is already running', None))
 		raise ar.Incomplete(e)
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Grab an ephemeral for consistency.
 
-	if settings.SNI:
-		encrypted_above = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort.
 		m = self.select(ar.HostPort, ar.Stop)
 		if isinstance(m, ar.HostPort):
 			connect_above = m
@@ -400,19 +396,15 @@
 	settings = GroupSettings()
 	hr = hb.open_role(group_role, settings, None, ar.NodeProperties())
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Disabled.
 
-	if settings.SNI:
-		encrypted_above = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
 	self.assign(a, None)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort
 		# Then wait for a grace period.
 		m = self.select(ar.HostPort, ar.Stop)
```

### Comparing `ansar-connect-0.1.141/src/ansar/connect/product.py` & `ansar-connect-0.1.142/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/socketry.py` & `ansar-connect-0.1.142/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/standard.py` & `ansar-connect-0.1.142/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/transporting.py` & `ansar-connect-0.1.142/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar/connect/wan.py` & `ansar-connect-0.1.142/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.141/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.142/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.141
+Version: 0.1.142
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.141/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.142/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

