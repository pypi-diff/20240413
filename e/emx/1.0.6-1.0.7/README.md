# Comparing `tmp/emx-1.0.6-py3-none-any.whl.zip` & `tmp/emx-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7458 bytes, number of entries: 8
--rw-r--r--  2.0 unx    20128 b- defN 24-Apr-11 00:49 emx/__init__.py
+Zip file size: 7585 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    20387 b- defN 24-Apr-12 16:25 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
--rw-r--r--  2.0 unx     2320 b- defN 24-Apr-10 08:57 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-11 00:52 emx-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 00:52 emx-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-11 00:52 emx-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-11 00:52 emx-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-11 00:52 emx-1.0.6.dist-info/RECORD
-8 files, 23743 bytes uncompressed, 6450 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx     2470 b- defN 24-Apr-12 16:28 emx/http.py
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/RECORD
+8 files, 24152 bytes uncompressed, 6577 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.6.dist-info/METADATA
+Filename: emx-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.6.dist-info/WHEEL
+Filename: emx-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.6.dist-info/entry_points.txt
+Filename: emx-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.6.dist-info/top_level.txt
+Filename: emx-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.6.dist-info/RECORD
+Filename: emx-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -240,28 +240,15 @@
             if desc:
                 print(f"{i}. {path} [{format_size(size)}]: {desc}")
             else:
                 print(f"{i}. {path} [{format_size(size)}]")
 
     def info(self, args : argparse.Namespace):
         name = args.name
-        isid = args.id
-
-        try:
-            n = int(name)
-            if str(n) == name:
-                isid = True
-        except:
-            pass
-
-        if isid:
-            req_args = urlencode({"name": name, "type": "id"})
-        else:
-            req_args = urlencode({"name": name, "type": "name"})
-
+        req_args = urlencode({"name": name, "type": "name"})
         resp = http.request_info(f"{self.cfg.SERVER}/detail?{req_args}")
         if resp is None:
             return False
         
         idd = resp["id"]
         name = resp["name"]
         path = resp["path"]
@@ -269,28 +256,30 @@
         size = resp["size"]
         raw_size = resp["raw_size"]
         num_files = resp["num_files"]
         user_name = resp["user_name"]
         is_directory = resp["is_directory"]
         create_time = resp["create_time"]
         update_time = resp["update_time"]
+        delete_time = resp["delete_time"]
         zipped = resp["zipped"]
         file_type = resp["file_type"]
         download_counter = resp["download_counter"]
         print(f"Found file {name}:")
         print(f"  id:          {idd}")
         print(f"  size:        {format_size(int(size))}")
         print(f"  rawsize:     {format_size(int(raw_size))}")
         print(f"  path:        {path}")
         print(f"  num_files:   {num_files}")
         print(f"  directory:   {is_directory}")
         print(f"  zipped:      {zipped}")
         print(f"  type:        {file_type}")
         print(f"  create_time: {create_time}")
         print(f"  update_time: {update_time}")
+        print(f"  delete_time: {delete_time}")
         print(f"  user_name:   {user_name}")
         print(f"  download:    {download_counter}")
         print(f"  descript:    {descript}")
 
 
     def get(self, args : argparse.Namespace):
         name = args.name
@@ -387,14 +376,20 @@
             if not value.encode("utf-8").isalnum():
                 print(f"An invalid username is entered. Only [a-zA-Z0-9] can be passed.")
                 return False
 
             self.cfg.set_cfg("UserName", value)
             print(f"Set UserName to {value}")
 
+    def delete(self, args : argparse.Namespace):
+        path = args.path
+        req_args = urlencode({"path": path, "user_name": self.cfg.get_cfg("UserName"), "user_token": self.cfg.get_cfg("UserToken")})
+        if http.request_info(f"{self.cfg.SERVER}/delete?{req_args}") is not None:
+            print(f"Delete file [{path}] success.")
+
     def put(self, args : argparse.Namespace):
         
         local = args.local
         file_type = args.type
         if not os.path.exists(local):
             print(f"File not found: {local}")
             return False
@@ -540,28 +535,30 @@
         c = cmd.add_cmd("put", "Put to server")
         c.add_argument("local", type=str, help="")
         c.add_argument("--remote", type=str, required=False, help="local 'whoami/local_name' if it is None")
         c.add_argument("--zip", action="store_true", help="Do zip file")
         c.add_argument("--desc", type=str, default="", help="Save folder")
         c.add_argument("--type", type=str, default="archive", help="put file to server")
 
-        c = cmd.add_cmd("list", "Search file")
+        c = cmd.add_cmd("list", "Search the file by keyword.")
         c.add_argument("key", nargs="?", type=str, default="%", help="search name/path")
         c.add_argument("--name", action="store_true", help="search by name, [default is path]")
         c.add_argument("--count", type=int, default=20, help="show count")
         c.add_argument("--skip", type=int, default=0, help="show skip")
 
-        c = cmd.add_cmd("cmds", "Search file")
+        c = cmd.add_cmd("cmds", "List all command lines.")
         c.add_argument("key", nargs="?", type=str, default="%", help="search name/path")
         c.add_argument("--count", type=int, default=20, help="show count")
         c.add_argument("--skip", type=int, default=0, help="show skip")
+        
+        c = cmd.add_cmd("delete", "Remove a file by path.")
+        c.add_argument("path", type=str, help="file path.")
 
         c = cmd.add_cmd("config", "Config")
         c.add_argument("name", type=str, help="key")
         c.add_argument("value", type=str, help="value")
 
         c = cmd.add_cmd("login", "Login")
         c = cmd.add_cmd("user", "Print the current logined user name.")
         c = cmd.add_cmd("info", "Detail file")
         c.add_argument("name", type=str, help="search name")
-        c.add_argument("--id", action="store_true", help="use id to get")
         return cmd.run(args, remargs)
```

## emx/http.py

```diff
@@ -3,17 +3,23 @@
 import traceback
 from tqdm import tqdm
 import json
 
 
 def request_info(url):
     response   = requests.get(url)
-    data = json.loads(str(response.content, encoding="utf-8"))
+    try:
+        resp_str = str(response.content, encoding="utf-8")
+        data = json.loads(resp_str)
+    except json.decoder.JSONDecodeError as e:
+        print(f"Server error: {resp_str}")
+        return None
+
     if response.status_code != 200:
-        print(f"Download failed, {data['detail']}")
+        print(f"Request failed, {data['detail']}")
         return None
     
     return data
 
 
 def upload_file(url, file, headers, title, chunk_size=4096*100):
```

