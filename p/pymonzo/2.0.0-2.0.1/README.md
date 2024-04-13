# Comparing `tmp/pymonzo-2.0.0.tar.gz` & `tmp/pymonzo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonzo-2.0.0.tar", last modified: Thu Mar  7 22:14:21 2024, max compression
+gzip compressed data, was "pymonzo-2.0.1.tar", last modified: Sat Apr 13 15:36:41 2024, max compression
```

## Comparing `pymonzo-2.0.0.tar` & `pymonzo-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    16725 2024-03-07 22:14:21.000000 pymonzo-2.0.0/LICENSE
--rw-r--r--   0        0        0     2669 2024-03-07 22:14:21.000000 pymonzo-2.0.0/README.md
--rw-r--r--   0        0        0     3677 2024-03-07 22:14:21.000000 pymonzo-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      700 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/__init__.py
--rw-r--r--   0        0        0      271 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/accounts/__init__.py
--rw-r--r--   0        0        0      437 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/accounts/enums.py
--rw-r--r--   0        0        0     2216 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/accounts/resources.py
--rw-r--r--   0        0        0     3038 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/accounts/schemas.py
--rw-r--r--   0        0        0      223 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/attachments/__init__.py
--rw-r--r--   0        0        0     3037 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/attachments/resources.py
--rw-r--r--   0        0        0     1144 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/attachments/schemas.py
--rw-r--r--   0        0        0      183 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/balance/__init__.py
--rw-r--r--   0        0        0     1199 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/balance/resources.py
--rw-r--r--   0        0        0     2422 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/balance/schemas.py
--rw-r--r--   0        0        0     7969 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/client.py
--rw-r--r--   0        0        0      514 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/exceptions.py
--rw-r--r--   0        0        0      186 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/feed/__init__.py
--rw-r--r--   0        0        0     1700 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/feed/resources.py
--rw-r--r--   0        0        0     1144 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/feed/schemas.py
--rw-r--r--   0        0        0      170 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/pots/__init__.py
--rw-r--r--   0        0        0     6685 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/pots/resources.py
--rw-r--r--   0        0        0     1769 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/pots/schemas.py
--rw-r--r--   0        0        0        0 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/py.typed
--rw-r--r--   0        0        0     1852 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/resources.py
--rw-r--r--   0        0        0     1594 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/settings.py
--rw-r--r--   0        0        0      361 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/transactions/__init__.py
--rw-r--r--   0        0        0     1324 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/transactions/enums.py
--rw-r--r--   0        0        0     3954 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/transactions/resources.py
--rw-r--r--   0        0        0     7358 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/transactions/schemas.py
--rw-r--r--   0        0        0     2697 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/utils.py
--rw-r--r--   0        0        0      252 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/webhooks/__init__.py
--rw-r--r--   0        0        0     2744 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/webhooks/resources.py
--rw-r--r--   0        0        0     2346 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/webhooks/schemas.py
--rw-r--r--   0        0        0      196 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/whoami/__init__.py
--rw-r--r--   0        0        0      733 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/whoami/resources.py
--rw-r--r--   0        0        0     1028 2024-03-07 22:14:21.000000 pymonzo-2.0.0/src/pymonzo/whoami/schemas.py
--rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 pymonzo-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-13 15:36:41.000000 pymonzo-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2669 2024-04-13 15:36:41.000000 pymonzo-2.0.1/README.md
+-rw-r--r--   0        0        0     3677 2024-04-13 15:36:41.000000 pymonzo-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      700 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/enums.py
+-rw-r--r--   0        0        0     2216 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/resources.py
+-rw-r--r--   0        0        0     3038 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/schemas.py
+-rw-r--r--   0        0        0      223 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/__init__.py
+-rw-r--r--   0        0        0     3037 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/resources.py
+-rw-r--r--   0        0        0     1144 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/schemas.py
+-rw-r--r--   0        0        0      183 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/__init__.py
+-rw-r--r--   0        0        0     1199 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/resources.py
+-rw-r--r--   0        0        0     2422 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/schemas.py
+-rw-r--r--   0        0        0     7970 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/client.py
+-rw-r--r--   0        0        0      514 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/exceptions.py
+-rw-r--r--   0        0        0      186 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/__init__.py
+-rw-r--r--   0        0        0     1700 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/resources.py
+-rw-r--r--   0        0        0     1144 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/schemas.py
+-rw-r--r--   0        0        0      170 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/__init__.py
+-rw-r--r--   0        0        0     6685 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/resources.py
+-rw-r--r--   0        0        0     1786 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/py.typed
+-rw-r--r--   0        0        0     1852 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/resources.py
+-rw-r--r--   0        0        0     1594 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/settings.py
+-rw-r--r--   0        0        0      361 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/__init__.py
+-rw-r--r--   0        0        0     1324 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/enums.py
+-rw-r--r--   0        0        0     3954 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/resources.py
+-rw-r--r--   0        0        0     7358 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/schemas.py
+-rw-r--r--   0        0        0     2697 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/utils.py
+-rw-r--r--   0        0        0      252 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/__init__.py
+-rw-r--r--   0        0        0     2744 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/resources.py
+-rw-r--r--   0        0        0     2346 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/schemas.py
+-rw-r--r--   0        0        0      196 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/resources.py
+-rw-r--r--   0        0        0     1028 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/schemas.py
+-rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 pymonzo-2.0.1/PKG-INFO
```

### Comparing `pymonzo-2.0.0/LICENSE` & `pymonzo-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/README.md` & `pymonzo-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/pyproject.toml` & `pymonzo-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/__init__.py` & `pymonzo-2.0.1/src/pymonzo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 [pydantic]: https://github.com/pydantic/pydantic
 """
 
 from pymonzo.client import MonzoAPI  # noqa
 
 __title__ = "pymonzo"
 __description__ = "Modern Python API client for Monzo public API."
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __url__ = "https://github.com/pawelad/pymonzo"
 __author__ = "Paweł Adamczak"
 __email__ = "pawel.ad@gmail.com"
 __license__ = "MPL-2.0"
```

### Comparing `pymonzo-2.0.0/src/pymonzo/accounts/resources.py` & `pymonzo-2.0.1/src/pymonzo/accounts/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/accounts/schemas.py` & `pymonzo-2.0.1/src/pymonzo/accounts/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/attachments/resources.py` & `pymonzo-2.0.1/src/pymonzo/attachments/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/attachments/schemas.py` & `pymonzo-2.0.1/src/pymonzo/attachments/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/balance/resources.py` & `pymonzo-2.0.1/src/pymonzo/balance/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/balance/schemas.py` & `pymonzo-2.0.1/src/pymonzo/balance/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/client.py` & `pymonzo-2.0.1/src/pymonzo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         else:
             try:
                 self._settings = PyMonzoSettings.load_from_disk(self.settings_path)
             except (FileNotFoundError, JSONDecodeError) as e:
                 raise NoSettingsFile(
                     "No settings file found. You need to either run "
                     "`MonzoAPI.authorize(client_id, client_secret)` "
-                    "to get the authorization token (and save it to disk),"
+                    "to get the authorization token (and save it to disk), "
                     "or explicitly pass the `access_token`."
                 ) from e
 
         self.session = OAuth2Client(
             client_id=self._settings.client_id,
             client_secret=self._settings.client_secret,
             token=self._settings.token,
```

### Comparing `pymonzo-2.0.0/src/pymonzo/exceptions.py` & `pymonzo-2.0.1/src/pymonzo/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/feed/resources.py` & `pymonzo-2.0.1/src/pymonzo/feed/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/feed/schemas.py` & `pymonzo-2.0.1/src/pymonzo/feed/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/pots/resources.py` & `pymonzo-2.0.1/src/pymonzo/pots/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/pots/schemas.py` & `pymonzo-2.0.1/src/pymonzo/pots/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     balance: int
     currency: str
     created: datetime
     updated: datetime
     deleted: bool
 
     # Undocumented in Monzo API docs
-    goal_amount: int
+    goal_amount: Optional[int] = None
     type: str
     product_id: str
     current_account_id: str
     cover_image_url: str
     isa_wrapper: str
     round_up: bool
     round_up_multiplier: Optional[int]
```

### Comparing `pymonzo-2.0.0/src/pymonzo/resources.py` & `pymonzo-2.0.1/src/pymonzo/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/settings.py` & `pymonzo-2.0.1/src/pymonzo/settings.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/transactions/enums.py` & `pymonzo-2.0.1/src/pymonzo/transactions/enums.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/transactions/resources.py` & `pymonzo-2.0.1/src/pymonzo/transactions/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/transactions/schemas.py` & `pymonzo-2.0.1/src/pymonzo/transactions/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/utils.py` & `pymonzo-2.0.1/src/pymonzo/utils.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/webhooks/resources.py` & `pymonzo-2.0.1/src/pymonzo/webhooks/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/webhooks/schemas.py` & `pymonzo-2.0.1/src/pymonzo/webhooks/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/whoami/resources.py` & `pymonzo-2.0.1/src/pymonzo/whoami/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/src/pymonzo/whoami/schemas.py` & `pymonzo-2.0.1/src/pymonzo/whoami/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.0/PKG-INFO` & `pymonzo-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonzo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Modern Python API client for Monzo public API.
 Keywords: monzo,api
 Author-email: Paweł Adamczak <pawel.ad@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

