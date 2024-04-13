# Comparing `tmp/ansar-connect-0.1.140.tar.gz` & `tmp/ansar-connect-0.1.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.140.tar", last modified: Fri Apr 12 05:34:39 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.141.tar", last modified: Sat Apr 13 00:30:15 2024, max compression
```

## Comparing `ansar-connect-0.1.140.tar` & `ansar-connect-0.1.141.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.140/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.140/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.140/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.140/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14476 2024-04-12 05:31:08.000000 ansar-connect-0.1.140/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3641 2024-04-12 03:15:07.000000 ansar-connect-0.1.140/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.140/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9228 2024-04-12 02:39:03.000000 ansar-connect-0.1.140/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 05:34:36.000000 ansar-connect-0.1.140/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14046 2024-04-12 02:39:06.000000 ansar-connect-0.1.140/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78172 2024-04-12 02:39:12.000000 ansar-connect-0.1.140/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.140/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.140/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.140/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.140/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.140/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.140/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.140/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.140/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.140/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37979 2024-04-12 05:33:51.000000 ansar-connect-0.1.140/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.140/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.140/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.140/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.140/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6465 2024-04-12 01:38:18.000000 ansar-connect-0.1.140/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.141/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.141/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.141/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.141/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar-connect-0.1.141/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar-connect-0.1.141/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.141/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar-connect-0.1.141/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-13 00:30:11.000000 ansar-connect-0.1.141/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14145 2024-04-12 23:59:12.000000 ansar-connect-0.1.141/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78053 2024-04-12 14:58:30.000000 ansar-connect-0.1.141/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.141/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.141/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.141/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.141/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.141/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.141/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.141/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.141/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.141/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33283 2024-04-13 00:13:16.000000 ansar-connect-0.1.141/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar-connect-0.1.141/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.141/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.141/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.141/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar-connect-0.1.141/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-13 00:30:15.015938 ansar-connect-0.1.141/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-13 00:30:15.000000 ansar-connect-0.1.141/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.140/LICENSE` & `ansar-connect-0.1.141/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/PKG-INFO` & `ansar-connect-0.1.141/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.140
+Version: 0.1.141
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.140/README.md` & `ansar-connect-0.1.141/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/pyproject.toml` & `ansar-connect-0.1.141/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/setup.py` & `ansar-connect-0.1.141/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.141/src/ansar/command/ansar_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 	'main',
 ]
 
 import sys
 
 import ansar.connect as ar
 from ansar.connect.procedure import *
+from ansar.connect.wan import FOH_HOST
 
 # Shims between command-line and library procedures.
 # Provide access to ansar-encode.
 versioning_settings = ar.VersioningSettings()
 compare_settings = ar.CompareSettings()
 release_settings = ar.ReleaseSettings()
 
@@ -442,15 +443,15 @@
 		return e.value
 	return output
 
 ar.bind(ansar)
 
 #
 #
-factory_settings = Settings(cloud_ip='52.53.115.135')
+factory_settings = Settings(cloud_ip=FOH_HOST, SNI=FOH_HOST)
 
 def main():
 	ar.create_object(ansar, factory_settings=factory_settings, parameter_passing=ar.sub_object_passing, parameter_table=table)
 
 # The standard entry point. Needed for IDEs
 # and debugger sessions.
 if __name__ == '__main__':
```

### Comparing `ansar-connect-0.1.140/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.141/src/ansar/command/ansar_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,47 +31,41 @@
 	'main',
 ]
 
 #
 #
 class Settings(object):
 	def __init__(self, directory_scope=None, connect_above=None, accept_below=None,
-			certificate_file=None, key_file=None, SNI=None):
+			certificate_file=None, key_file=None):
 		self.directory_scope = directory_scope or ar.ScopeOfService.HOST
 		self.connect_above = connect_above or ar.HostPort()
 		self.accept_below = accept_below or ar.HostPort()
 		self.certificate_file = certificate_file
 		self.key_file = key_file
-		self.SNI = SNI
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'connect_above': ar.Any(),
 	'accept_below': ar.UserDefined(ar.HostPort),
 	'certificate_file': ar.Unicode(),
 	'key_file': ar.Unicode(),
-	'SNI': ar.Unicode(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 # Just need an object to stay "on duty" while the 
 # global ServiceDirectory does its work.
 def directory(self, settings):
-	encrypted_above = None
-	encrypted_below = None
-
-	if settings.SNI:
-		encrypted_above = ar.TlsClient(SNI=settings.SNI)
+	encrypted = None
 	if settings.certificate_file and settings.key_file:
-		encrypted_below = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
+		encrypted = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
 
 	a = self.create(ar.ServiceDirectory, settings.directory_scope,
 		settings.connect_above, settings.accept_below,
-		encrypted_above=encrypted_above, encrypted_below=encrypted_below)
+		encrypted=encrypted)
 	m = self.select(ar.HostPort, ar.Completed, ar.Stop)
 	if isinstance(m, ar.Completed):
 		return m.value
 	elif isinstance(m, ar.Stop):
 		self.send(m, a)
 		self.select(ar.Completed)
 		return ar.Aborted()
```

### Comparing `ansar-connect-0.1.140/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.141/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.141/src/ansar/command/shared_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,39 +157,34 @@
 	return READY
 
 def ProductDirectory_READY_ProductLookup(self, message):
 	r = self.return_address[-1]
 
 	settings = self.settings
 
-	product_name = message.product_name or 'acme'
-	product_instance = message.product_instance or InstanceOfProduct.DEVELOPMENT
+	product_name = message.product_name or 'Ansar Networking'
+	product_instance = message.product_instance or InstanceOfProduct.TESTING
 	k = f'{product_name}:{product_instance}'
 
 	d = self.directory.get(k)
 	if d is None:
 		self.trace(f'Unknown directory key "{k}" for child [{r}]')
 		c = self.connect_above.get(k)
 		if c is None:
 			self.trace(f'Unknown upward key "{k}" for child [{r}]')
 			# Default upward access is disabled but a hint that it
 			# should adopt the same nature.
 			c = ProductAccess(product_name=product_name, product_instance=product_instance)
 			self.connect_above[k] = c
 			self.store()
 
-		encrypted_above = None
-		if settings.SNI:
-			encrypted_above = ar.TlsClient(SNI=settings.SNI)
-
 		d = self.create(ar.ServiceDirectory,
 			scope=settings.directory_scope,			# All at same scope.
 			connect_above=c,
-			accept_below=ar.HostPort(),				# Disabled.
-			encrypted_above=encrypted_above)
+			accept_below=ar.HostPort())				# Disabled.
 
 		self.assign(d, k)
 		self.directory[k] = d
 
 	self.child_of[r] = d
 	accepted = self.accepted.get(r)
 	if accepted:
@@ -280,27 +275,25 @@
 
 ar.bind(ProductDirectory, PRODUCT_DIRECTORY_DISPATCH)
 
 
 # Allow configuration of network details.
 #
 class Settings(object):
-	def __init__(self, directory_scope=None, public_access=None, certificate_file=None, key_file=None, SNI=None):
+	def __init__(self, directory_scope=None, public_access=None, certificate_file=None, key_file=None):
 		self.directory_scope = directory_scope
 		self.public_access = public_access or ar.HostPort()
 		self.certificate_file = certificate_file
 		self.key_file = key_file
-		self.SNI = SNI
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'public_access': ar.UserDefined(ar.HostPort),
 	'certificate_file': ar.Unicode(),
 	'key_file': ar.Unicode(),
-	'SNI': ar.Unicode(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
 factory_settings = Settings(directory_scope=ar.ScopeOfService.HOST,
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/__init__.py` & `ansar-connect-0.1.141/src/ansar/connect/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 1e2e39f043f911cfabb25a9eb409e07f526553d6
-Version: 0.1.139 (2024-04-12@17:34:36+NZST)
+Commit: 136b4a4baf8dcb69e113a01b3b2df9d25a267dac
+Version: 0.1.140 (2024-04-13@12:30:11+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.141/src/ansar/connect/connect_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,50 +48,54 @@
 class GLARING: pass
 class CONNECTING: pass
 class REDIRECTING: pass
 class ASSIGNING: pass
 class CLOSING: pass
 
 class ConnectToDirectory(ar.Point, ar.StateMachine):
-	def __init__(self, connect_above, session=None, group_address=None, encrypted=None):
+	def __init__(self, connect_above, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.connect_above = connect_above
 		self.session = session
 		self.group_address = group_address
-		self.encrypted = encrypted
 
 		self.started = None
 		self.attempts = 0
 
 		self.connected = None
 		self.remote = None
 		self.redirect = None
 
 		self.closing = None
 		self.intervals = None
 		self.retry = None
 
 	def connect(self):
 		c = self.connect_above
+		encrypted = None
 		if isinstance(c, HostPort):
 			ipp = c
 			next = PENDING
 		elif isinstance(c, ProductAccess):
 			ipp = c.access_ipp
+			if c.SNI:
+				encrypted = TlsClient(SNI=c.SNI)
 			next = PRODUCING
 		elif isinstance(c, WideAreaAccess):
 			ipp = c.access_ipp
+			if c.SNI:
+				encrypted = TlsClient(SNI=c.SNI)
 			next = CLOUDY
 		else:
 			return DISABLED
 
 		if ipp.host is None:
 			return DISABLED
-		connect(self, ipp, session=self.session, encrypted=self.encrypted)
+		connect(self, ipp, session=self.session, encrypted=encrypted)
 		self.start(ar.T1, seconds=8.0)
 		return next
 
 	def reschedule(self):
 		if self.intervals is None:
 			c = self.connect_above
 			if isinstance(c, HostPort):
@@ -182,15 +186,15 @@
 # Waiting for results of connect.
 # Transport established.
 def ConnectToDirectory_PRODUCING_Connected(self, message):
 	self.cancel(ar.T1)
 	self.connected = message
 
 	c = self.connect_above
-	lookup = ProductLookup(c.product_name, c.product_instance)
+	lookup = ProductLookup(product_name=c.product_name, product_instance=c.product_instance)
 	self.reply(lookup)
 	return GLANCING
 
 def ConnectToDirectory_PRODUCING_NotConnected(self, message):
 	self.send(message, self.parent_address)
 	self.cancel(ar.T1)
 	# Attempt failed.
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/directory.py` & `ansar-connect-0.1.141/src/ansar/connect/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,22 +500,21 @@
 			return False
 	return True
 
 CONNECT_ABOVE = 'connect-above'
 ACCEPT_BELOW = 'accept-below'
 
 class ServiceDirectory(ar.Threaded, ar.StateMachine):
-	def __init__(self, scope=None, connect_above=None, accept_below=None, encrypted_above=None, encrypted_below=None):
+	def __init__(self, scope=None, connect_above=None, accept_below=None, encrypted=None):
 		ar.Threaded.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.scope = scope or ScopeOfService.PROCESS
 		self.connect_above = connect_above
 		self.accept_below = accept_below or HostPort()
-		self.encrypted_above = encrypted_above
-		self.encrypted_below = encrypted_below
+		self.encrypted = encrypted
 		self.ctd = None
 		self.directory = {}
 		self.find = {}
 		self.matched = {}
 		self.connected_up = None
 		self.not_connected = None
 		self.connected = None
@@ -775,23 +774,23 @@
 def ServiceDirectory_INITIAL_Start(self, message):
 	self.started = ar.world_now()
 
 	self.trace(f'Scope of {ScopeOfService.to_name(self.scope)}')
 	self.trace(f'Connecting up to "{ar.tof(self.connect_above)}"')
 	self.trace(f'Listening below at "{ar.tof(self.accept_below)}"')
 
-	self.ctd = self.create(ConnectToDirectory, self.connect_above, encrypted=self.encrypted_above)
+	self.ctd = self.create(ConnectToDirectory, self.connect_above)
 	self.assign(self.ctd, CONNECT_ABOVE)
 
 	# Acceptance of connections from lower directories.
 	if isinstance(self.accept_below, HostPort):
 		if self.accept_below.host is None:
 			self.send(HostPort(host=None), self.parent_address)
 		else:
-			listen(self, self.accept_below, tag='directory-accept', encrypted=self.encrypted_below)
+			listen(self, self.accept_below, tag='directory-accept', encrypted=self.encrypted)
 			return OPENING
 	else:
 		pass	# Acceptance arranged externally. May be a
 				# Listening object for diagnosis.
 
 	return NORMAL
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.141/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.141/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/group_if.py` & `ansar-connect-0.1.141/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/grouping.py` & `ansar-connect-0.1.141/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/moving.py` & `ansar-connect-0.1.141/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/networking.py` & `ansar-connect-0.1.141/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.141/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/node.py` & `ansar-connect-0.1.141/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.141/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/procedure.py` & `ansar-connect-0.1.141/src/ansar/connect/procedure.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,25 +59,27 @@
 
 # Per-command arguments as required.
 # e.g. command-line parameters specific to create.
 class NetworkSettings(object):
 	def __init__(self, group_name=None, home_path=None,
 			connect_scope=None, to_scope=None,
 			product_name=None, product_instance=None,
+			SNI=None,
 			custom_host=None, custom_port=None,
 			reserved=False,
 			connect_file=None, connect_disable=False,
 			published_services=False, subscribed_searches=False, routed_matches=False, accepted_processes=False,
 			host_and_port=False, start_time=False):
 		self.group_name = group_name
 		self.home_path = home_path
 		self.connect_scope = connect_scope
 		self.to_scope = to_scope
 		self.product_name = product_name
 		self.product_instance = product_instance
+		self.SNI = SNI
 		self.custom_host = custom_host
 		self.custom_port = custom_port
 		self.reserved = reserved
 		self.connect_file = connect_file
 		self.connect_disable = connect_disable
 		self.published_services = published_services
 		self.subscribed_searches = subscribed_searches
@@ -89,14 +91,15 @@
 NETWORK_SETTINGS_SCHEMA = {
 	'group_name': ar.Unicode(),
 	'home_path': ar.Unicode(),
 	'connect_scope': ScopeOfService,
 	'to_scope': ScopeOfService,
 	'product_name': ar.Unicode(),
 	'product_instance': InstanceOfProduct,
+	'SNI': ar.Unicode(),
 	'custom_host': ar.Unicode(),
 	'custom_port': ar.Integer8(),
 	'reserved': ar.Boolean(),
 	'connect_file': ar.Unicode(),
 	'connect_disable': ar.Boolean(),
 	'published_services': ar.Boolean(),
 	'subscribed_searches': ar.Boolean(),
@@ -228,18 +231,20 @@
 			connect_scope = network.connect_scope
 			to_scope = network.to_scope
 			if network.product_name and network.product_instance:		# ProductAccess
 				shared_host = network.custom_host or scope_host(to_scope)
 				shared_port = network.custom_port or ANSAR_SHARED_PORT
 				access_ipp = ar.HostPort(shared_host, shared_port)
 				connect_above= ProductAccess(access_ipp=access_ipp,
+					SNI=network.SNI,
 					product_name=network.product_name,
 					product_instance=network.product_instance)
 			elif network.product_name or network.product_instance:		# Error
-				pass
+				e = ar.Faulted('need both product name and product instance')
+				raise ar.Incomplete(e)
 			elif network.reserved:										# Reserved space.
 				reserved_host = network.custom_host or scope_host(to_scope)
 				reserved_port = network.custom_port or ANSAR_RESERVED_PORT
 				connect_above = ar.HostPort(reserved_host, reserved_port)
 			else:														# HostPort for connect_scope -> to_scope
 				dedicated_host = network.custom_host or scope_host(to_scope)
 				dedicated_port = network.custom_port or ANSAR_DEDICATED_PORT
@@ -296,169 +301,20 @@
 		elif isinstance(m, ar.Faulted):		# Failure in the hierarchy.
 			return m
 		else:
 			return None
 		# Now the response to the actual
 		# NetworkConnect request.
 		m = self.select(ar.Ack, ar.Stop)
-		return None
 
 	finally:
 		self.send(ar.Stop(), self.directory)
 		self.select(ar.Completed, ar.Stop)
 
 	return None
-'''
-	if self.settings.connect_scope:
-		#self.settings.connect_above = message
-		self.start(ar.T2, seconds=1.5)
-		return RECONNECTING
-
-def Group_RECONNECTING_T2(self, message):
-	try:
-		f = ar.File(self.settings.connect_file, ar.Any(), decorate_names=False)
-		connect_above, _ = f.recover()
-	except (ar.FileFailure, ar.CodecError) as e:
-		s = str(e)
-		f = ar.Failed(connect_file=(s, None))
-		self.complete(f)
-	a = ar.NetworkConnect(scope=self.settings.connect_scope, connect_above=connect_above)
-	self.send(a, self.directory)
-	return RECONNECTING
-
-def Group_RECONNECTING_Anything(self, message):
-	# The DirectoryConnect sent above has been routed to this
-	# directory owner, i.e. the scope was set to GROUP.
-	hr = ar.object_role()
-
-	settings = hr.role_settings[2]
-	settings.connect_above = message.thing
-	try:
-		decoration_store(hr.role_settings, settings)
-	except (ar.FileFailure, ar.CodecFailed) as e:
-		r = ar.Failed(group_reconnect=(e, None))
-		self.warning(str(r))
-	self.reply(ar.Ack())
-	return RECONNECTING
-
-def Group_RECONNECTING_Ack(self, message):
-	# This is the Ack sent by the ServiceDirectory after the
-	# activity above, i.e. its the final "reply" to the
-	# original sending of a NetworkConnect.
-	self.complete(message)
-
-	settings = []
-	if network.connect_scope:	# Assignment of new connection.
-		if not network.connect_file:
-			e = ar.Rejected(connect_with_no_file=('missing connection details', None))
-			raise ar.Incomplete(e)
-		s = ScopeOfService.to_name(network.connect_scope)
-		p = os.path.abspath(network.connect_file)
-		settings.append(f'--connect-scope={s}')
-		settings.append(f'--connect-file={p}')
-
-	else:
-		settings.append(f'--show-scopes')
-
-	try:
-		a = self.create(ar.Process, 'ansar-group',	
-					origin=ar.POINT_OF_ORIGIN.RUN_ORIGIN,
-					home_path=hb.home_path, role_name=group_role, subrole=False,
-					settings=settings)
-
-		# Wait for Ack from new process to verify that
-		# framework is operational.
-		m = self.select(ar.Completed, ar.Stop)
-		if isinstance(m, ar.Stop):
-			# Honor the slim chance of a control-c before
-			# the framework can respond.
-			self.send(m, a)
-			m = self.select(ar.Completed)
-
-		# Process.
-		def lfa_text(lfa):
-			f, l, a = len(d.listing), len(d.find), len(d.accepted)
-			s = f'{f}/{l}/{a}'
-			return s
-
-		value = m.value
-		if isinstance(value, ar.Ack):	   # New instance established itself.
-			pass
-		elif isinstance(value, DirectoryAncestry):
-			for d in reversed(value.lineage):
-
-				scope = ScopeOfService.to_name(d.scope) if d.scope else '?'
-				if isinstance(d.connect_above, ar.HostPort):
-					connecting_ipp = d.connect_above
-					display_name = str(connecting_ipp)
-				elif isinstance(d.connect_above, ProductAccess):
-					connecting_ipp = d.connect_above.access_ipp
-					e = InstanceOfProduct.to_name(d.connect_above.product_instance)
-					display_name = f'{d.connect_above.product_name}/{e}'
-				elif isinstance(d.connect_above, WideAreaAccess):
-					connecting_ipp = d.connect_above.access_ipp
-					display_name = f'{d.connect_above.directory_id}'
-				else:
-					continue
-
-				if connecting_ipp.host is None:
-					continue
-
-				started = ar.world_to_text(d.started) if d.started else '-'
-				connected = ar.world_to_text(d.connected) if d.connected else '-'
-				lfa = lfa_text(d)
-
-				note = []
-				if network.host_and_port:
-					note.append(str(connecting_ipp))
-				if network.start_time:
-					note.append(started)
-
-				if connecting_ipp.host is None:
-					note.append('DISABLED')
-				elif d.not_connected:
-					note.append(d.not_connected)
-
-				key_name = {k: r.search_or_listing for r in d.listing for k in r.route_key}
-				if note:
-					s = ', '.join(note)
-					ar.output_line(f'{scope} {display_name} ({s})')
-				else:
-					ar.output_line(f'{scope} {display_name}')
-				if network.published_services:
-					ar.output_line(f'Published services ({len(d.listing)})', tab=1)
-					for r in d.listing:
-						ar.output_line(f'{r.search_or_listing} ({len(r.route_key)})', tab=2)
-				if network.subscribed_searches:
-					ar.output_line(f'Subscribed searches ({len(d.find)})', tab=1)
-					if network.routed_matches:
-						for r in d.find:
-							ar.output_line(f'{r.search_or_listing} ({len(r.route_key)})', tab=2)
-							for k in r.route_key:
-								ar.output_line(f'"{key_name[k]}"', tab=3)
-				if network.accepted_processes:
-					ar.output_line(f'Accepted processes ({len(d.accepted)})', tab=1)
-					for a in d.accepted:
-						ar.output_line(f'{a}', tab=2)
-
-		elif isinstance(value, NetworkConnect):
-			return value
-		elif isinstance(value, ar.Faulted):
-			raise ar.Incomplete(value)
-		elif isinstance(value, ar.LockedOut):
-			e = ar.Failed(role_lock=(None, f'"{group_role}" already running as <{value.pid}>'))
-			raise ar.Incomplete(e)
-		else:
-			e = ar.Failed(role_execute=(value, f'unexpected response from "{group_role}" (ansar-group)'))
-			raise ar.Incomplete(e)
-	finally:
-		pass
-
-	return None
-'''
 
 class PingSettings(object):
 	def __init__(self, service_name=None, group_name=None, home_path=None, ping_count=None):
 		self.service_name = service_name
 		self.group_name = group_name
 		self.home_path = home_path
 		self.ping_count = ping_count
@@ -1066,15 +922,16 @@
 	if not export.access_name:
 		f = ar.Faulted('access name not specified', 'use --access-name=<uuid>')
 		return f
 	self.send(export, session)
 	m = self.select(DirectoryExported, ar.Faulted, ar.Abandoned, ar.Stop)
 	if isinstance(m, DirectoryExported):
 		cloud_ipp = ar.HostPort(cloud_ip, FOH_PORT)
-		w = WideAreaAccess(access_ipp=cloud_ipp, access_token=m.access_token,
+		SNI = settings.SNI
+		w = WideAreaAccess(access_ipp=cloud_ipp, SNI=SNI, access_token=m.access_token,
 			account_id=m.account_id, directory_id=m.directory_id,
 			product_name=m.product_name, product_instance=m.product_instance)
 		f = output_access(w, directory.export_file)
 		if f:
 			return f
 		return None
 	elif isinstance(m, ar.Faulted):
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/product.py` & `ansar-connect-0.1.141/src/ansar/connect/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,32 @@
 	QA=4, STAGING=5, PRODUCTION=6,
 	DEMONSTRATION=7, TRAINING=8, SALES=9,
 	EVALUATION=10, OTHER=11)
 
 #
 #
 class ProductAccess(object):
-	def __init__(self, access_ipp=None, product_name=None, product_instance=None):
+	def __init__(self, access_ipp=None, SNI=None, product_name=None, product_instance=None):
 		self.access_ipp = access_ipp or ar.HostPort()
+		self.SNI = SNI
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class ProductLookup(object):
 	def __init__(self, product_name=None, product_instance=None):
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class YourProduct(object):
 	def __init__(self, address=None):
 		self.address = address
 
 INSTANT_SCHEMA = {
 	"access_ipp": ar.UserDefined(ar.HostPort),
+	"SNI": ar.Unicode(),
 	"product_name": ar.Unicode(),
 	"product_instance": InstanceOfProduct,
 	"address": ar.Address(),
 }
 
 ar.bind(ProductAccess, object_schema=INSTANT_SCHEMA)
 ar.bind(ProductLookup, object_schema=INSTANT_SCHEMA)
```

### Comparing `ansar-connect-0.1.140/src/ansar/connect/socketry.py` & `ansar-connect-0.1.141/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/standard.py` & `ansar-connect-0.1.141/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/transporting.py` & `ansar-connect-0.1.141/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.140/src/ansar/connect/wan.py` & `ansar-connect-0.1.141/src/ansar/connect/wan.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 	'WideAreaAssignment',
 	'YourWideArea',
 	'RelayLookup',			# Node to WAN relay.
 	'RelayRedirect',
 	'RelayAssignment',
 	'YourRelay',
 	'CloseRelay',
+	'FOH_HOST',
 ]
 
 # Contact details.
 CONTACT_TYPE = ar.Enumeration(PERSONAL=0, BUSINESS=1, HOME=2, OTHER=3)
 CONTACT_DEVICE = ar.Enumeration(MOBILE=0, FIXED_LINE=1)
 
 class EmailAddress(object):
@@ -86,17 +87,18 @@
 
 ar.bind(EmailAddress, object_schema=CONTACT_SCHEMA)
 ar.bind(PhoneNumber, object_schema=CONTACT_SCHEMA)
 
 # Protocol between a connecting directory and
 # a cloud directory.
 class WideAreaAccess(object):
-	def __init__(self, access_ipp=None, access_token=None, account_id=None, directory_id=None,
+	def __init__(self, access_ipp=None, SNI=None, access_token=None, account_id=None, directory_id=None,
 			product_name=None, product_instance=None):
 		self.access_ipp = access_ipp or HostPort()	# Manifestly required.
+		self.SNI = SNI
 		self.access_token = access_token
 		self.account_id = account_id				# Speed up processing.
 		self.directory_id = directory_id
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 	def __str__(self):
@@ -110,19 +112,19 @@
 		self.account_id = account_id
 		self.directory_id = directory_id
 		self.access_token = access_token
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class WideAreaRedirect(object):
-	def __init__(self, redirect_ipp=None, directory_id=None, assignment_token=None, SNI=None):
+	def __init__(self, redirect_ipp=None, SNI=None, directory_id=None, assignment_token=None):
 		self.redirect_ipp = redirect_ipp or HostPort()
+		self.SNI = SNI
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
-		self.SNI = SNI
 
 class WideAreaAssignment(object):
 	def __init__(self, directory_id=None, assignment_token=None):
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
 
 class YourWideArea(object):
@@ -197,7 +199,9 @@
 		self.redirect = redirect or RelayRedirect()
 
 CLOSE_SCHEMA = {
 	"redirect": ar.UserDefined(RelayRedirect),
 }
 
 ar.bind(CloseRelay, object_schema=CLOSE_SCHEMA)
+
+FOH_HOST = 'ansar-mx.net'
```

### Comparing `ansar-connect-0.1.140/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.141/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.140
+Version: 0.1.141
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.140/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.141/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

