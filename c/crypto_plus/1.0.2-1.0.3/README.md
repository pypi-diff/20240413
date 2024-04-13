# Comparing `tmp/crypto_plus-1.0.2.tar.gz` & `tmp/crypto_plus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_plus-1.0.2.tar", max compression
+gzip compressed data, was "crypto_plus-1.0.3.tar", max compression
```

## Comparing `crypto_plus-1.0.2.tar` & `crypto_plus-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.2/LICENSE
--rw-r--r--   0        0        0     1608 2024-04-04 13:52:52.933182 crypto_plus-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.2/README.md
--rw-r--r--   0        0        0      143 2024-04-04 13:48:03.170202 crypto_plus-1.0.2/src/crypto_plus/__init__.py
--rw-r--r--   0        0        0     7525 2024-04-04 04:57:32.396140 crypto_plus-1.0.2/src/crypto_plus/asymmetric.py
--rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.2/src/crypto_plus/base.py
--rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.2/src/crypto_plus/compatible.py
--rw-r--r--   0        0        0     5284 2024-04-04 13:45:34.624509 crypto_plus-1.0.2/src/crypto_plus/encrypt.py
--rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.2/src/crypto_plus/key.py
--rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.2/src/crypto_plus/sign.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-13 10:41:02.033305 crypto_plus-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.3/README.md
+-rw-r--r--   0        0        0      143 2024-04-13 10:41:09.260895 crypto_plus-1.0.3/src/crypto_plus/__init__.py
+-rw-r--r--   0        0        0     7586 2024-04-13 10:30:04.946637 crypto_plus-1.0.3/src/crypto_plus/asymmetric.py
+-rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.3/src/crypto_plus/base.py
+-rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.3/src/crypto_plus/compatible.py
+-rw-r--r--   0        0        0     5688 2024-04-13 10:33:43.989796 crypto_plus-1.0.3/src/crypto_plus/encrypt.py
+-rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.3/src/crypto_plus/key.py
+-rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.3/src/crypto_plus/sign.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.3/PKG-INFO
```

### Comparing `crypto_plus-1.0.2/LICENSE` & `crypto_plus-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.2/pyproject.toml` & `crypto_plus-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crypto_plus"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Easy-to-use Crypto Tool"
 readme = "README.md"
 authors = ["wmymz <wmymz@icloud.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.12",
```

### Comparing `crypto_plus-1.0.2/README.md` & `crypto_plus-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.2/src/crypto_plus/asymmetric.py` & `crypto_plus-1.0.3/src/crypto_plus/asymmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,20 +177,22 @@
         builder = builder.public_key(self.raw_public_key)
         certificate = builder.sign(
             private_key=self.raw_private_key, algorithm=hashes.SHA256()
         )
         return certificate.public_bytes(serialization.Encoding.PEM)
 
     # 非常规方法
-    def encrypt_by_private_key(self, message: bytes) -> bytes:
+    def encrypt_by_private_key(
+        self, message: bytes, random_padding=False
+    ) -> bytes:
         if not message:
             return b""
         if not self.private_key:
             raise Exception("私钥缺失")
-        return encrypt_by_key(self.private_key, message)
+        return encrypt_by_key(self.private_key, message, random=random_padding)
 
     def decrypt_by_public_key(self, message: bytes) -> bytes:
         if not message:
             return b""
         return decrypt_by_key(self.public_key, message)
 
     # 常规方法
```

### Comparing `crypto_plus-1.0.2/src/crypto_plus/compatible.py` & `crypto_plus-1.0.3/src/crypto_plus/compatible.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.2/src/crypto_plus/encrypt.py` & `crypto_plus-1.0.3/src/crypto_plus/encrypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,35 +75,46 @@
     raise NotImplementedError(f"Not implemented type: {type(key)}")
 
 
 @encrypt_by_key.register(RsaKey)
 def _(key: RsaKey, message: bytes, **kwargs):
     pad = 8
     max_segment_len = key.size_in_bytes() - pad - 3
+    random_padding = kwargs.get("random", False)
     res = []
     if key.has_private():
         # 私钥加密（不建议）
         _fast_pow = fast_pow_factor(key)
         for i in range(1 + (len(message) - 1) // max_segment_len):
             # 分段加密
             plaintext_part = message[
                 i * max_segment_len : (i + 1) * max_segment_len
             ]
             pad_len = key.size_in_bytes() - len(plaintext_part) - 3
             # 填充后加密
-            # 生成范围在1到255之间的随机数，确保非零字节
-            rand_pads = bytearray(pad_len)
-            for j in range(pad_len):
-                rand_pads[j] = random.randint(1, 255)
+            if random_padding:
+                # 随机填充
+                # 生成范围在1到255之间的随机数，确保非零字节
+                rand_pads = bytearray(pad_len)
+                for j in range(pad_len):
+                    rand_pads[j] = random.randint(1, 255)
 
-            rand_pads = rand_pads[:pad_len]
-            plaintext_part_padding = bytes_to_long(
-                # bytes.fromhex(f'0001{"ff" * pad_len}00{plaintext_part.hex()}')
-                bytes.fromhex(f"0002{rand_pads.hex()}00{plaintext_part.hex()}")
-            )
+                plaintext_part_padding = bytes_to_long(
+                    # bytes.fromhex(f'0001{"ff" * pad_len}00{plaintext_part.hex()}')
+                    bytes.fromhex(
+                        f"0002{rand_pads.hex()}00{plaintext_part.hex()}"
+                    )
+                )
+            else:
+                # ff填充
+                plaintext_part_padding = bytes_to_long(
+                    bytes.fromhex(
+                        f'0001{"ff" * pad_len}00{plaintext_part.hex()}'
+                    )
+                )
             ciphertext_part = _fast_pow(plaintext_part_padding)
 
             # encrypt_data = encrypt_data.to_bytes(1 + encrypt_data.bit_length() // 8)
             ciphertext_part = ciphertext_part.to_bytes(
                 key.public_key().size_in_bytes()
             )
             res.append(ciphertext_part)
```

### Comparing `crypto_plus-1.0.2/src/crypto_plus/key.py` & `crypto_plus-1.0.3/src/crypto_plus/key.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.2/src/crypto_plus/sign.py` & `crypto_plus-1.0.3/src/crypto_plus/sign.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.2/PKG-INFO` & `crypto_plus-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto_plus
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Easy-to-use Crypto Tool
 License: MIT
 Author: wmymz
 Author-email: wmymz@icloud.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

