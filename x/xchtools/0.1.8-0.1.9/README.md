# Comparing `tmp/xchtools-0.1.8-py3-none-any.whl.zip` & `tmp/xchtools-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8535 bytes, number of entries: 10
+Zip file size: 9436 bytes, number of entries: 10
 -rw-r--r--  2.0 fat       69 b- defN 80-Jan-01 00:00 xchtools/.env.example
 -rw-r--r--  2.0 fat      111 b- defN 80-Jan-01 00:00 xchtools/__init__.py
--rw-r--r--  2.0 fat     9824 b- defN 80-Jan-01 00:00 xchtools/common.py
--rw-r--r--  2.0 fat     5876 b- defN 80-Jan-01 00:00 xchtools/connections.py
+-rw-r--r--  2.0 fat    12523 b- defN 80-Jan-01 00:00 xchtools/common.py
+-rw-r--r--  2.0 fat     5894 b- defN 80-Jan-01 00:00 xchtools/connections.py
 -rw-r--r--  2.0 fat     1619 b- defN 80-Jan-01 00:00 xchtools/funcflow.py
 -rw-r--r--  2.0 fat     1308 b- defN 80-Jan-01 00:00 xchtools/logger.py
 -rw-r--r--  2.0 fat      173 b- defN 80-Jan-01 00:00 xchtools/settings.toml.example
--rw-r--r--  2.0 fat     1277 b- defN 80-Jan-01 00:00 xchtools-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 xchtools-0.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 fat      754 b- defN 16-Jan-01 00:00 xchtools-0.1.8.dist-info/RECORD
-10 files, 21099 bytes uncompressed, 7265 bytes compressed:  65.6%
+-rw-r--r--  2.0 fat     1319 b- defN 80-Jan-01 00:00 xchtools-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 xchtools-0.1.9.dist-info/WHEEL
+?rw-r--r--  2.0 fat      755 b- defN 16-Jan-01 00:00 xchtools-0.1.9.dist-info/RECORD
+10 files, 23859 bytes uncompressed, 8166 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -15,17 +15,17 @@
 
 Filename: xchtools/logger.py
 Comment: 
 
 Filename: xchtools/settings.toml.example
 Comment: 
 
-Filename: xchtools-0.1.8.dist-info/METADATA
+Filename: xchtools-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xchtools-0.1.8.dist-info/WHEEL
+Filename: xchtools-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xchtools-0.1.8.dist-info/RECORD
+Filename: xchtools-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xchtools/common.py

```diff
@@ -1,13 +1,16 @@
 """This file is compatible with ljqpy, use import xchtools.commons as ljqpy"""
-
+# %%
 import os, re, sys, random, urllib.parse, json
+import requests
+from tqdm import tqdm
 from collections import defaultdict
 
 
+# --------- from ljqpy -------------
 def WriteLine(fout, lst):
     fout.write("\t".join([str(x) for x in lst]) + "\n")
 
 
 def RM(patt, sr):
     mat = re.search(patt, sr, re.DOTALL | re.MULTILINE)
     return mat.group(1) if mat else ""
@@ -335,7 +338,79 @@
     print("completed, " + str(total) + " records")
 
 
 def cmd():
     while True:
         cmd = input("> ")
         sql(cmd)
+
+
+# ----------------------------------------------------------------
+
+
+# %%
+def batch_url_request(url: str, li: list, retry: int = 2) -> list:
+    """
+    Makes a batch of HTTP GET requests to a specified URL with each query parameter from the list,
+    with a specified number of retries for each request.
+
+    Parameters:
+    url (str): The base URL with a placeholder for the query parameter, e.g., 'http://xxxxxx/?p={q}'.
+    li (list): A list of query parameters to be used in the URL.
+    retry (int): The number of times to retry a request if it fails. Default is 2.
+
+    Returns:
+    list: A list of responses from the server for each request.
+    """
+
+    responses = []
+
+    # Loop through each query parameter in the list
+    for q in tqdm(li, desc="Processing requests"):
+        attempt = 0
+        success = False
+
+        while attempt < retry and not success:
+            try:
+                # Construct the full URL by replacing the placeholder with the actual query parameter
+                full_url = url.format(q=q)
+
+                # Make the HTTP GET request
+                response = requests.get(full_url)
+
+                # Check if the request was successful
+                if response.status_code == 200:
+                    # Append the response to the list and set success to True
+                    responses.append(response.text)
+                    success = True
+                else:
+                    # Increment the attempt counter and log the failed status code
+                    attempt += 1
+                    print(
+                        f"Attempt {attempt} failed with status code {response.status_code}"
+                    )
+
+            except requests.RequestException as e:
+                # Increment the attempt counter and log the exception
+                attempt += 1
+                print(f"Attempt {attempt} resulted in RequestException: {e}")
+
+        # If all attempts fail, append an error message
+        if not success:
+            responses.append(
+                f"Failed to retrieve data for query parameter '{q}' after {retry} attempts."
+            )
+
+    return responses
+
+
+if __name__ == "__main__":
+    # %%
+
+    # Example usage:
+    # Assuming you have a list of query parameters and a base URL
+    query_params = ["param1", "param2", "param3"]
+    base_url = "http://example.com/?p={q}"
+
+    # Call the function with the base URL, the list of query parameters, and the number of retries
+    results = batch_url_request(base_url, query_params, retry=3)
+    results
```

## xchtools/connections.py

```diff
@@ -145,15 +145,15 @@
         xc.sql2li("show tables in information_schema")
         xc.sql2li("show databases")
     # %%
     # xc.sql2li("show tables in fundresearch")
     # xc.sql2li("select * from fundresearch.fund_information")
     xc.sql2li("select * from information_schema.TABLES")
     # %%
-
+    # 批量建表
     path = r"C:\Users\o0oii\Downloads\fundresearch_fundresearch_20231115205701\fundresearch\TABLE"
     xc.create_tables(path, "fundresearch")
 
     # %%
     xc.sql2df("show columns in fundresearch.fund_awards ")
 
     # %%
```

## Comparing `xchtools-0.1.8.dist-info/METADATA` & `xchtools-0.1.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xchtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: remy
 Author-email: redreamality@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.2.4,<4.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 
 
 
 # Config
```

## Comparing `xchtools-0.1.8.dist-info/RECORD` & `xchtools-0.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xchtools/.env.example,sha256=dL_r3BtfQvA1FXK4INrcEleBSSsER7nJFPE2g-Ir-Ic,69
 xchtools/__init__.py,sha256=CfbS64So2Ua9vwMzyb0gE_LgiSJAJ3rqAxJ3oKMS3NQ,111
-xchtools/common.py,sha256=TcZznpyKOSAyjy-EVJouqSP9cKAf480GK9G1CfvX9gw,9824
-xchtools/connections.py,sha256=EBJIvLim6uhOr65R5NpjcB4j7501YRPQGb61QOQm4Kw,5876
+xchtools/common.py,sha256=uvoayere6LAYgAmYnvaLuaNE2v25lpvUsPX0QwF1yos,12523
+xchtools/connections.py,sha256=dxDuklNfX_9nRePoohT16ULA3VBTH7XJBDVHex0u6Vg,5894
 xchtools/funcflow.py,sha256=zfLYy20yK0kFVe3mQDcrGd2gQnfKgY9bCA9wRmWJvgY,1619
 xchtools/logger.py,sha256=vroVmYLMt3LZWXRLWSchnDlQnNhIB6zQ03VLU25VHaM,1308
 xchtools/settings.toml.example,sha256=KAAMfVNYyyH4G4weBmrbZd2ptG-9mWlGMaZVx28J5IE,173
-xchtools-0.1.8.dist-info/METADATA,sha256=avwZSaYvf1fN5a5TdK1Ml9PmsPDQqPdukzO-T_-PNZY,1277
-xchtools-0.1.8.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-xchtools-0.1.8.dist-info/RECORD,,
+xchtools-0.1.9.dist-info/METADATA,sha256=y7eMb20Do6uYPhMG0P-fRMIciDlwpD8hvUrItRrO09U,1319
+xchtools-0.1.9.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+xchtools-0.1.9.dist-info/RECORD,,
```

