# Comparing `tmp/sessionless-0.0.2.tar.gz` & `tmp/sessionless-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessionless-0.0.2.tar", last modified: Tue Apr  9 18:31:46 2024, max compression
+gzip compressed data, was "sessionless-0.0.3.tar", last modified: Sat Apr 13 19:16:45 2024, max compression
```

## Comparing `sessionless-0.0.2.tar` & `sessionless-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-09 18:31:46.180068 sessionless-0.0.2/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3904 2024-04-09 18:31:46.179290 sessionless-0.0.2/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)     3296 2024-04-09 18:20:37.000000 sessionless-0.0.2/README.md
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-09 18:31:46.174134 sessionless-0.0.2/sessionless/
--rw-r--r--   0 habsoomane   (501) staff       (20)      104 2024-04-07 17:58:42.000000 sessionless-0.0.2/sessionless/__init__.py
--rw-r--r--   0 habsoomane   (501) staff       (20)      103 2024-04-07 16:05:50.000000 sessionless-0.0.2/sessionless/core.py
--rw-r--r--   0 habsoomane   (501) staff       (20)     3216 2024-04-09 16:10:18.000000 sessionless-0.0.2/sessionless/modelsecp256k1.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-09 18:31:46.178111 sessionless-0.0.2/sessionless.egg-info/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3904 2024-04-09 18:31:46.000000 sessionless-0.0.2/sessionless.egg-info/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)      295 2024-04-09 18:31:46.000000 sessionless-0.0.2/sessionless.egg-info/SOURCES.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-04-09 18:31:46.000000 sessionless-0.0.2/sessionless.egg-info/dependency_links.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       15 2024-04-09 18:31:46.000000 sessionless-0.0.2/sessionless.egg-info/requires.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       12 2024-04-09 18:31:46.000000 sessionless-0.0.2/sessionless.egg-info/top_level.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-04-09 18:31:46.180251 sessionless-0.0.2/setup.cfg
--rw-r--r--   0 habsoomane   (501) staff       (20)     1126 2024-04-09 18:31:26.000000 sessionless-0.0.2/setup.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-09 18:31:46.177354 sessionless-0.0.2/tests/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3166 2024-04-09 16:16:38.000000 sessionless-0.0.2/tests/test.modelsecp256k1.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.553071 sessionless-0.0.3/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3581 2024-04-13 19:16:45.551816 sessionless-0.0.3/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2973 2024-04-12 23:12:13.000000 sessionless-0.0.3/README.md
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.544859 sessionless-0.0.3/sessionless/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       59 2024-04-12 22:02:34.000000 sessionless-0.0.3/sessionless/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2598 2024-04-12 23:14:33.000000 sessionless-0.0.3/sessionless/modelsecp256k1.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.550673 sessionless-0.0.3/sessionless.egg-info/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3581 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)      294 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/SOURCES.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/dependency_links.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       15 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/requires.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       18 2024-04-13 19:16:45.000000 sessionless-0.0.3/sessionless.egg-info/top_level.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-04-13 19:16:45.553370 sessionless-0.0.3/setup.cfg
+-rw-r--r--   0 habsoomane   (501) staff       (20)     1126 2024-04-13 19:16:30.000000 sessionless-0.0.3/setup.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-13 19:16:45.549566 sessionless-0.0.3/tests/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       63 2024-04-12 22:08:56.000000 sessionless-0.0.3/tests/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2794 2024-04-12 23:11:57.000000 sessionless-0.0.3/tests/modelsecp256k1__test.py
```

### Comparing `sessionless-0.0.2/PKG-INFO` & `sessionless-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessionless
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
 Author: Sessionless Team
 Author-email: zach@planetnine.app
 Keywords: authentication,cryptography,authenticate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -16,65 +16,66 @@
 
 <div align="center">
     <h1> Sessionless : Python</h1>
 </div>
 
 ## About
 
-[Sessionless](https://sessionless.org/) is an open source authentication protocol that uses the cryptography employed by Bitcoin and Ethereum to authenticate messages sent between a client and a server. Within this protocol, you create and store a private key on the client and then use that key to sign messages; those messages are then verified by the server via the public key associated with the client. When you verify a message you also certify its provenance. Because no other secret need be shared between client and server, sessions are wholly unnecessary.
+[Sessionless](https://sessionless.org/) is an open-source authentication protocol that uses the cryptography employed by Bitcoin and Ethereum to authenticate messages sent between a client and a server. Within this protocol, you create and store a private key on the client and then use that key to sign messages; the server then verifies those messages via the public key associated with the client. When you verify a message you also certify its provenance. Sessions are wholly unnecessary because no other secret needs to be shared between client and server.
 
 ## Getting Started 
 
 To install the package, run the following code within your command line interface. More information regarding release history for this package can be found [here](https://pypi.org/project/sessionless/).
 ```
 pip install sessionless
 ```
 
 ## Development 
 
-### Generating a private key
-To use this package, please call a new instance of the SessionlessSecp256k1 class. Users can default to providing a private key within the class constructor. If no key is provided, a key will be randomly generated for the user.
+### Getting started
+To use this package, please call a new instance of the SessionlessSecp256k1 class. Users will need to provide a get key method. This method will be referenced later on to obtain key values.
 
 ```python
-# This will generate a random private key
-# Passing a private key in hex format within the constructor will assign the value as an instance private key
-sessionless = SessionlessSecp256k1()
+# This will create an instance of the SessionlessSecp256k1 class 
+# Users must pass a method to retrieve keys.
+def get_key():
+    pass
+sessionless = SessionlessSecp256k1(get_key)
 ```
 
-### Retrieving the private key
-Users will need to supply methods to retrieve the key. If methods are not supplied, the private key will not be returned. This is to uphold security practices.
+### Generating private and public keys
+The generate keys method will generate a private key and a public key. To use the method, users must provide a method to save the keys. 
 ```python
-sessionless.get_private_key(saveKeys(), getKeys()) # This will return the encrypted private key
-```
-Accessing the private key by calling the parameter will throw an attribute error. 
-
-```python
-sessionless.__private_key # AttributeError: 'SessionlessSecp256k1' object has no attribute '__private_key'. Did you mean: 'get_private_key'?
-```
-### Generating a public key
-Users can easily generate public keys from the private key.
-```python
-public_key = sessionless.get_public_key_from_private_key()
+def save_key():
+    pass
+private_key, public_key = sessionless.generate_keys(save_key) # This will return the encrypted private and public key
 ```
 
 ### Signing messages
-Users can easily sign messages by providing a message to the sign_message() method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
+Users can easily sign messages by providing a message to the sign method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
 ```python
 msg = {
 "message": "The weather is so nice today!"
 }
-signature = sessionless.sign_message(msg)
+signature = sessionless.sign(msg)
 ```
 
 ### Verifying messages
 Users can verify messages and signatures to ensure data integrity, authenticity, and non-repudiation. Users will pass a signature, message, and an encrypted public key as parameters. If public key is not provided, a public key will be generated from the instance's private key.
 ```python
-res = sessionless.verify_signature(signature, msg) # Returns True
-res2 = sessionless.verify_signature(signature, msg, second_primary_key) # Returns False
+res = sessionless.verify_signature(signature, msg, public_key) # Returns True
+res2 = sessionless.verify_signature(first_signature, first_msg, second_primary_key) # Returns False
 ```
 
 ### Associating messages
-Sessionless is a practical implmentation of delegatable anonymous credentials. Users can verify that two messages are able to be associated using the associate_message() method. 
+Users can verify that two messages can be associated using the associate method. 
+```python
+res = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+
+```
+
+### Generating UUIDs [Universally Unique Identifiers]
+Users can generate unique identifiers as needed by calling the generate UUID method.
 ```python
-res = sessionless.associate_message(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+uuid = sessionless.generate_UUID() # Returns UUID
 
 ```
```

### Comparing `sessionless-0.0.2/README.md` & `sessionless-0.0.3/sessionless.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,81 @@
+Metadata-Version: 2.1
+Name: sessionless
+Version: 0.0.3
+Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
+Author: Sessionless Team
+Author-email: zach@planetnine.app
+Keywords: authentication,cryptography,authenticate
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+Requires-Dist: secp256k1
+Requires-Dist: uuid
+
 <div align="center">
     <h1> Sessionless : Python</h1>
 </div>
 
 ## About
 
-[Sessionless](https://sessionless.org/) is an open source authentication protocol that uses the cryptography employed by Bitcoin and Ethereum to authenticate messages sent between a client and a server. Within this protocol, you create and store a private key on the client and then use that key to sign messages; those messages are then verified by the server via the public key associated with the client. When you verify a message you also certify its provenance. Because no other secret need be shared between client and server, sessions are wholly unnecessary.
+[Sessionless](https://sessionless.org/) is an open-source authentication protocol that uses the cryptography employed by Bitcoin and Ethereum to authenticate messages sent between a client and a server. Within this protocol, you create and store a private key on the client and then use that key to sign messages; the server then verifies those messages via the public key associated with the client. When you verify a message you also certify its provenance. Sessions are wholly unnecessary because no other secret needs to be shared between client and server.
 
 ## Getting Started 
 
 To install the package, run the following code within your command line interface. More information regarding release history for this package can be found [here](https://pypi.org/project/sessionless/).
 ```
 pip install sessionless
 ```
 
 ## Development 
 
-### Generating a private key
-To use this package, please call a new instance of the SessionlessSecp256k1 class. Users can default to providing a private key within the class constructor. If no key is provided, a key will be randomly generated for the user.
+### Getting started
+To use this package, please call a new instance of the SessionlessSecp256k1 class. Users will need to provide a get key method. This method will be referenced later on to obtain key values.
 
 ```python
-# This will generate a random private key
-# Passing a private key in hex format within the constructor will assign the value as an instance private key
-sessionless = SessionlessSecp256k1()
+# This will create an instance of the SessionlessSecp256k1 class 
+# Users must pass a method to retrieve keys.
+def get_key():
+    pass
+sessionless = SessionlessSecp256k1(get_key)
 ```
 
-### Retrieving the private key
-Users will need to supply methods to retrieve the key. If methods are not supplied, the private key will not be returned. This is to uphold security practices.
-```python
-sessionless.get_private_key(saveKeys(), getKeys()) # This will return the encrypted private key
-```
-Accessing the private key by calling the parameter will throw an attribute error. 
-
-```python
-sessionless.__private_key # AttributeError: 'SessionlessSecp256k1' object has no attribute '__private_key'. Did you mean: 'get_private_key'?
-```
-### Generating a public key
-Users can easily generate public keys from the private key.
+### Generating private and public keys
+The generate keys method will generate a private key and a public key. To use the method, users must provide a method to save the keys. 
 ```python
-public_key = sessionless.get_public_key_from_private_key()
+def save_key():
+    pass
+private_key, public_key = sessionless.generate_keys(save_key) # This will return the encrypted private and public key
 ```
 
 ### Signing messages
-Users can easily sign messages by providing a message to the sign_message() method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
+Users can easily sign messages by providing a message to the sign method. Messages do not need to be encoded before passing them to the method. The method will return an encrypted signature that users can store as needed.
 ```python
 msg = {
 "message": "The weather is so nice today!"
 }
-signature = sessionless.sign_message(msg)
+signature = sessionless.sign(msg)
 ```
 
 ### Verifying messages
 Users can verify messages and signatures to ensure data integrity, authenticity, and non-repudiation. Users will pass a signature, message, and an encrypted public key as parameters. If public key is not provided, a public key will be generated from the instance's private key.
 ```python
-res = sessionless.verify_signature(signature, msg) # Returns True
-res2 = sessionless.verify_signature(signature, msg, second_primary_key) # Returns False
+res = sessionless.verify_signature(signature, msg, public_key) # Returns True
+res2 = sessionless.verify_signature(first_signature, first_msg, second_primary_key) # Returns False
 ```
 
 ### Associating messages
-Sessionless is a practical implmentation of delegatable anonymous credentials. Users can verify that two messages are able to be associated using the associate_message() method. 
+Users can verify that two messages can be associated using the associate method. 
+```python
+res = sessionless.associate(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+
+```
+
+### Generating UUIDs [Universally Unique Identifiers]
+Users can generate unique identifiers as needed by calling the generate UUID method.
 ```python
-res = sessionless.associate_message(primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key) # Returns either True or False
+uuid = sessionless.generate_UUID() # Returns UUID
 
 ```
```

### Comparing `sessionless-0.0.2/sessionless/modelsecp256k1.py` & `sessionless-0.0.3/sessionless/modelsecp256k1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,58 @@
 import secp256k1
 import pickle
+import uuid
+import inspect
+
+
 class SessionlessSecp256k1():
-    def __init__(self, private_key_hex=secp256k1.PrivateKey().serialize()):
-        private_key = secp256k1.PrivateKey()
-        assert private_key.deserialize(private_key_hex) == private_key.private_key
-        self.__private_key = private_key
     
-    def get_algorithm_name(self):
-        return "secp256k1"
-    
-    def get_private_key(self, saveKeys, getKeys):
-        try: 
-            if callable(saveKeys) and callable(getKeys):
-                return self.__private_key.serialize()
-        except Exception as e:
-            raise TypeError("No default secure storage in python. Please provide a saveKeys and getKeys function to store private key. Internal error message: " + e)
+    def __init__(self, get_keys):
+        self.get_keys = get_keys
         
-    def update_private_key(self, new_private_key_hex):
-        try:
-            private_key = secp256k1.PrivateKey()
-            assert private_key.deserialize(new_private_key_hex) == private_key.private_key
-            self.__private_key = private_key
-            return "Updated private key value."
-        except Exception as e:
-            raise AttributeError("Private key unable to be assigned. Please provide a valid key in hex format and try again. Internal error message: " + e)
+    def generate_UUID(self):
+        return uuid.uuid4().hex
     
-    def get_public_key_from_private_key(self):
-        try:
-            return self.__private_key.pubkey.serialize().hex()
-        except Exception as e:
-            raise ValueError("Value not provided in correct format. Private key expected to be in hex format. Internal error message: " + e)
+    def generate_keys(self, saveKeys):
+        try: 
+            if callable(saveKeys):
+                private_key_obj = secp256k1.PrivateKey()
+                private_key = private_key_obj.serialize()
+                public_key = private_key_obj.pubkey.serialize().hex()
+                return private_key, public_key
+        except Exception:
+            raise TypeError("No default secure storage in python. Please provide a saveKeys and getKeys function to store private key. Internal error message: ")
     
-    def sign_message(self, msg):
+    async def sign(self, msg):
         try:
             if not isinstance(msg, bytes):
                 msg = pickle.dumps(msg)
-            deserializedSig = self.__private_key.ecdsa_sign(msg)
-            sig = self.__private_key.ecdsa_serialize_compact(deserializedSig)
+            if inspect.iscoroutinefunction(self.get_keys):
+                private_key_hex = await self.get_keys()
+            else: 
+                private_key_hex = self.get_keys()
+            private_key = secp256k1.PrivateKey()
+            assert private_key.deserialize(private_key_hex) == private_key.private_key
+            deserializedSig = private_key.ecdsa_sign(msg)
+            sig = private_key.ecdsa_serialize_compact(deserializedSig)
             return sig.hex()
-        except Exception as e:
-            raise ValueError("Value not provided in correct format. Internal error message: " + e)
+        except Exception:
+            raise ValueError("Value not provided in correct format. Internal error message: ")
         
-    def verify_signature(self, signature, msg, public_key_hex=None):
+    def verify_signature(self, signature, msg, public_key_hex):
         try:
             if not isinstance(msg, bytes):
                 msg = pickle.dumps(msg)
             sig = bytes.fromhex(signature)
-            if public_key_hex is not None:
-                public_key = secp256k1.PublicKey()
-                public_key.deserialize(bytes.fromhex(public_key_hex))
-            else:
-                public_key = self.__private_key.pubkey
+            public_key = secp256k1.PublicKey()
+            assert public_key.deserialize(bytes.fromhex(public_key_hex)) == public_key.public_key
+            
             signature = public_key.ecdsa_deserialize_compact(sig)
             return public_key.ecdsa_verify(msg, signature)
-        except Exception as e:
-            raise ValueError("Error with parameters. Please ensure values are provided in correct format. Internal error message: " + e)
+        except Exception:
+            raise ValueError("Error with parameters. Please ensure values are provided in correct format. Internal error message: ")
     
-    def associate_message(self, primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key ):
+    def associate(self, primary_sig, primary_msg, primary_public_key, secondary_sig, secondary_msg, secondary_public_key ):
         try:
-            return (self.verifySignature(primary_sig, primary_msg, primary_public_key) and self.verifySignature(secondary_sig, secondary_msg, secondary_public_key))
-        except Exception as e:
-            raise ValueError("Error with parameters. Please ensure values are provided in correct format. Internal error message: " + e)
-
-
-
-
+            return (self.verify_signature(primary_sig, primary_msg, primary_public_key) and self.verify_signature(secondary_sig, secondary_msg, secondary_public_key))
+        except Exception:
+            raise ValueError("Error with parameters. Please ensure values are provided in correct format. Internal error message: ")
```

### Comparing `sessionless-0.0.2/setup.py` & `sessionless-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 def read_markdown_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as file:
         markdown_content = file.read()
     return markdown_content
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.'
 LONG_DESCRIPTION = read_markdown_file("./README.md")
 
 # Setting up
 setup(
         name="sessionless", 
         version=VERSION,
```

### Comparing `sessionless-0.0.2/tests/test.modelsecp256k1.py` & `sessionless-0.0.3/tests/modelsecp256k1__test.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,57 @@
 def getKey():
         pass
 
 def saveKey():
         pass
 class SessionlessSecp256k1Test(unittest.TestCase):
    
-        def test_private_key_hex(self):
+        def test_generate_keys(self):
                 sl = SessionlessSecp256k1(PRIVATE_KEY_1)
-                result = sl.get_private_key(saveKey, getKey)
-                self.assertEqual(result, PRIVATE_KEY_1)
+                private_key, public_key = sl.generate_keys(saveKey, getKey)
+                self.assertIsNotNone(private_key)
+                self.assertIsNotNone(public_key)
                 
                 sl2 = SessionlessSecp256k1(PRIVATE_KEY_2)
-                result2 = sl2.get_private_key(saveKey, getKey)
-                self.assertEqual(result2, PRIVATE_KEY_2)
-        
-        def test_public_key_from_hex(self):
-                sl = SessionlessSecp256k1(PRIVATE_KEY_1)
-                result = sl.get_public_key_from_private_key()
-                self.assertEqual(result, PUBLIC_KEY_1)
-                
-                sl2 = SessionlessSecp256k1(PRIVATE_KEY_2)
-                result2 = sl2.get_public_key_from_private_key()
-                self.assertEqual(result2, PUBLIC_KEY_2)
+                private_key2, public_key2 = sl2.generate_keys(saveKey, getKey)
+                self.assertIsNotNone(private_key2)
+                self.assertIsNotNone(public_key2)
                 
         
-        def test_signing_message(self):
-                sl = SessionlessSecp256k1(PRIVATE_KEY_1)
-                result = sl.sign_message(MSG)
-                self.assertEqual(result, SIG_1)
-                
-                sl2 = SessionlessSecp256k1(PRIVATE_KEY_2)
-                result2 = sl2.sign_message(MSG)
-                self.assertEqual(result2, SIG_2)
+        async def test_sign(self):
+                sl = SessionlessSecp256k1(getKey)
+                result = await sl.sign(MSG)
+                self.assertIsNotNone(result)
+                
+                sl2 = SessionlessSecp256k1(getKey)
+                result2 = await sl2.sign(MSG)
+                self.assertIsNotNone(result2)
         
-        def test_verifying_signature(self):
-                sl = SessionlessSecp256k1(PRIVATE_KEY_1)
-                sig = sl.sign_message(MSG)
+        async def test_verify_signature(self):
+                sl = SessionlessSecp256k1(getKey)
+                sig = await sl.sign(MSG)
                 
-                sl2 = SessionlessSecp256k1(PRIVATE_KEY_2)
-                sig2 = sl2.sign_message(MSG)
+                sl2 = SessionlessSecp256k1(getKey)
+                sig2 = await sl2.sign(MSG)
                 
                 res1 = sl.verify_signature(sig2, MSG) 
                 res2 = sl.verify_signature(sig, MSG)
                 res3 = sl2.verify_signature(sig2, MSG) 
                 res4 = sl2.verify_signature(sig, MSG)
                 
                 self.assertEqual(res1, False)
                 self.assertEqual(res2, True)
                 self.assertEqual(res3, True)
                 self.assertEqual(res4, False)
         
         
-        def test_associating_message(self):
-                sl = SessionlessSecp256k1(PRIVATE_KEY_1)
-                sig = sl.sign_message(MSG)
-                
-                sl2 = SessionlessSecp256k1(PRIVATE_KEY_2)
-                sig2 = sl2.sign_message(MSG)
-                
-                res = sl.associate_message(sig, MSG, PUBLIC_KEY_1, sig2, MSG, PUBLIC_KEY_2)
+        def test_associate(self):
+                sl = SessionlessSecp256k1(getKey)
+       
+                res = sl.associate(SIG_1, MSG, PUBLIC_KEY_1, SIG_2, MSG, PUBLIC_KEY_2)
 
                 self.assertEqual(res, True)
 
+        def test_generate_UUID(self):
+                sl = SessionlessSecp256k1(getKey)
+                uuid = sl.generate_UUID()
+                self.assertIsNotNone(uuid)
```

