# Comparing `tmp/ansar-connect-0.1.139.tar.gz` & `tmp/ansar-connect-0.1.140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.139.tar", last modified: Fri Apr 12 03:16:29 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.140.tar", last modified: Fri Apr 12 05:34:39 2024, max compression
```

## Comparing `ansar-connect-0.1.139.tar` & `ansar-connect-0.1.140.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.080689 ansar-connect-0.1.139/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.139/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 03:16:29.080689 ansar-connect-0.1.139/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.139/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.139/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 03:16:29.080689 ansar-connect-0.1.139/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.139/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.076689 ansar-connect-0.1.139/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.076689 ansar-connect-0.1.139/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.076689 ansar-connect-0.1.139/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.139/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3641 2024-04-12 03:15:07.000000 ansar-connect-0.1.139/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.139/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9228 2024-04-12 02:39:03.000000 ansar-connect-0.1.139/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.080689 ansar-connect-0.1.139/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 03:16:25.000000 ansar-connect-0.1.139/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14046 2024-04-12 02:39:06.000000 ansar-connect-0.1.139/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78172 2024-04-12 02:39:12.000000 ansar-connect-0.1.139/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.139/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.139/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.139/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.139/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.139/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.139/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.139/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.139/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.139/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37539 2024-04-12 02:39:15.000000 ansar-connect-0.1.139/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.139/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.139/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.139/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.139/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6465 2024-04-12 01:38:18.000000 ansar-connect-0.1.139/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:16:29.080689 ansar-connect-0.1.139/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 03:16:29.000000 ansar-connect-0.1.139/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.140/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.140/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.140/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.140/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.840294 ansar-connect-0.1.140/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14476 2024-04-12 05:31:08.000000 ansar-connect-0.1.140/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3641 2024-04-12 03:15:07.000000 ansar-connect-0.1.140/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.140/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9228 2024-04-12 02:39:03.000000 ansar-connect-0.1.140/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 05:34:36.000000 ansar-connect-0.1.140/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14046 2024-04-12 02:39:06.000000 ansar-connect-0.1.140/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78172 2024-04-12 02:39:12.000000 ansar-connect-0.1.140/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.140/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.140/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.140/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.140/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.140/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.140/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.140/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.140/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.140/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37979 2024-04-12 05:33:51.000000 ansar-connect-0.1.140/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.140/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.140/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.140/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.140/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6465 2024-04-12 01:38:18.000000 ansar-connect-0.1.140/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 05:34:39.844293 ansar-connect-0.1.140/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 05:34:39.000000 ansar-connect-0.1.140/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.139/LICENSE` & `ansar-connect-0.1.140/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/PKG-INFO` & `ansar-connect-0.1.140/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.139
+Version: 0.1.140
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.139/README.md` & `ansar-connect-0.1.140/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/pyproject.toml` & `ansar-connect-0.1.140/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/setup.py` & `ansar-connect-0.1.140/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.140/src/ansar/command/ansar_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,29 +327,31 @@
 	(directory, directory_settings),
 )
 
 
 #
 #
 class Settings(object):
-	def __init__(self, force=False, cloud_ip=None, login_token=None):
+	def __init__(self, force=False, cloud_ip=None, SNI=None, login_token=None):
 		'''
 		* force
 		Override cautionary behaviour, mostly relating to the unintended termination
 		or running processes.
 		* cloud_ip
 		Domain name or dotted IP address.
 		'''
 		self.force = force
 		self.cloud_ip = cloud_ip
+		self.SNI = SNI
 		self.login_token = login_token
 
 SETTINGS_SCHEMA = {
 	'force': ar.Boolean(),
 	'cloud_ip': ar.Unicode(),
+	'SNI': ar.Unicode(),
 	'login_token': ar.UUID(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
```

### Comparing `ansar-connect-0.1.139/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.140/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.140/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.140/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/__init__.py` & `ansar-connect-0.1.140/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 74df350198045880de22622f3d12abce45ba05e3
-Version: 0.1.138 (2024-04-12@15:16:25+NZST)
+Commit: 1e2e39f043f911cfabb25a9eb409e07f526553d6
+Version: 0.1.139 (2024-04-12@17:34:36+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.139/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.140/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/directory.py` & `ansar-connect-0.1.140/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.140/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.140/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/group_if.py` & `ansar-connect-0.1.140/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/grouping.py` & `ansar-connect-0.1.140/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/moving.py` & `ansar-connect-0.1.140/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/networking.py` & `ansar-connect-0.1.140/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.140/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/node.py` & `ansar-connect-0.1.140/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.140/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/procedure.py` & `ansar-connect-0.1.140/src/ansar/connect/procedure.py`

 * *Files 3% similar despite different names*

```diff
@@ -664,15 +664,19 @@
 	settings = ar.object_custom_settings()
 	cloud_ip = settings.cloud_ip
 
 	f = crud_address_and_token(1, cloud_ip, uuid.uuid4())
 	if f:
 		return f
 
-	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT))
+	if settings.SNI:
+		encrypted = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encrypted = None
+	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
 		return ar.Aborted()
@@ -689,15 +693,19 @@
 	cloud_ip = settings.cloud_ip
 	login_token = settings.login_token
 
 	f = crud_address_and_token(1, cloud_ip, login_token)
 	if f:
 		return f
 
-	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT))
+	if settings.SNI:
+		encrypted = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encrypted = None
+	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
 		return ar.Aborted()
@@ -736,15 +744,19 @@
 
 	crud = sum([account.read, account.update, account.delete, account.add_login, account.add_directory])
 
 	f = crud_address_and_token(crud, cloud_ip, login_token)
 	if f:
 		return f
 
-	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT))
+	if settings.SNI:
+		encrypted = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encrypted = None
+	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
 		return ar.Aborted()
@@ -954,15 +966,19 @@
 
 	crud = sum([directory.read, directory.update, directory.export])
 
 	f = crud_address_and_token(crud, cloud_ip, login_token)
 	if f:
 		return f
 
-	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT))
+	if settings.SNI:
+		encrypted = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encrypted = None
+	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
 		return ar.Aborted()
```

### Comparing `ansar-connect-0.1.139/src/ansar/connect/product.py` & `ansar-connect-0.1.140/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/socketry.py` & `ansar-connect-0.1.140/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/standard.py` & `ansar-connect-0.1.140/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/transporting.py` & `ansar-connect-0.1.140/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar/connect/wan.py` & `ansar-connect-0.1.140/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.139/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.140/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.139
+Version: 0.1.140
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.139/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.140/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

