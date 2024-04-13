# Comparing `tmp/machineroom-0.44.9.tar.gz` & `tmp/machineroom-0.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.44.9.tar", last modified: Mon Apr  8 17:38:38 2024, max compression
+gzip compressed data, was "machineroom-0.45.0.tar", last modified: Sat Apr 13 11:13:59 2024, max compression
```

## Comparing `machineroom-0.44.9.tar` & `machineroom-0.45.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:38:38.168413 machineroom-0.44.9/
--rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.44.9/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.44.9/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-08 17:38:38.168248 machineroom-0.44.9/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.44.9/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:38:38.155221 machineroom-0.44.9/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.44.9/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:38:38.158183 machineroom-0.44.9/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-08 17:38:37.000000 machineroom-0.44.9/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5253 2024-04-08 17:15:42.000000 machineroom-0.44.9/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.44.9/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    13315 2024-03-22 10:56:07.000000 machineroom-0.44.9/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    19378 2024-04-08 17:37:00.000000 machineroom-0.44.9/machineroom/taskbase.py
--rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.44.9/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.44.9/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-08 17:38:38.167706 machineroom-0.44.9/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-08 17:38:38.000000 machineroom-0.44.9/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      371 2024-04-08 17:38:38.000000 machineroom-0.44.9/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-08 17:38:38.000000 machineroom-0.44.9/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-08 17:38:38.000000 machineroom-0.44.9/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-08 17:38:38.168975 machineroom-0.44.9/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.44.9/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1534 2024-04-08 17:38:24.000000 machineroom-0.44.9/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-08 17:38:31.000000 machineroom-0.44.9/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.189813 machineroom-0.45.0/
+-rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.0/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 11:13:59.189637 machineroom-0.45.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.180806 machineroom-0.45.0/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.0/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.186111 machineroom-0.45.0/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-13 11:13:58.000000 machineroom-0.45.0/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5260 2024-04-13 11:13:02.000000 machineroom-0.45.0/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.0/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    13315 2024-03-22 10:56:07.000000 machineroom-0.45.0/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    19685 2024-04-13 11:13:02.000000 machineroom-0.45.0/machineroom/taskbase.py
+-rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.0/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.0/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.189067 machineroom-0.45.0/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      371 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-13 11:13:59.190412 machineroom-0.45.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.0/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.0/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-13 11:13:46.000000 machineroom-0.45.0/version
```

### Comparing `machineroom-0.44.9/.gitignore` & `machineroom-0.45.0/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/LICENSE` & `machineroom-0.45.0/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/PKG-INFO` & `machineroom-0.45.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.44.9
+Version: 0.45.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.44.9/README.md` & `machineroom-0.45.0/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/cmdbin/connect` & `machineroom-0.45.0/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/machineroom/__init__.py` & `machineroom-0.45.0/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.44.9'
+__version__ = '0.45.0'
```

### Comparing `machineroom-0.44.9/machineroom/const.py` & `machineroom-0.45.0/machineroom/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     echo "推荐的端口如下："
     for port in "${ports[@]}"; do
         echo -e "\033[0;32m$port\033[0m"
     done
 }
 list_recommended_ports;"""
 DOCKER_STOP_REMOVE = """{COMMAND_DOCKER} rm $({COMMAND_DOCKER} stop $(sudo docker ps -a | grep "{CONTAINER_NAME}" | cut -d " " -f 1))"""
-DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d -v {VOLUME} --restart unless-stopped --name {NODE_NAME} {IMAGE}:{VERSION} {COMMAND}"""
+DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d {VOLUME} {NETWORK} --restart unless-stopped --name {NODE_NAME} {IMAGE}:{VERSION} {COMMAND}"""
 DOCKER_STOP_ID = """{COMMAND_DOCKER} stop {CID}"""
 DOCKER_STOP_RM = """{COMMAND_DOCKER} rm {CID}"""
 DOCKER_STOP_CONTAIN_NAME = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs {COMMAND_DOCKER} stop"""
 DOCKER_RM_NAME_BASED = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs -r {COMMAND_DOCKER} rm -f"""
 DOCKER_RM_VOLUME = """{COMMAND_DOCKER} volume ls -qf dangling=true -f name={CONTAINER_NAME} | xargs -r {COMMAND_DOCKER} volume rm"""
 DOCKER_LOG_REVIEW = """COMMAND_DOCKER ps -a --filter "name=__CONTAINER_KEYWORD" --format "{{.ID}}" | shuf -n 1 | xargs docker logs --tail __RECENT_LINES"""
```

### Comparing `machineroom-0.44.9/machineroom/schema.json` & `machineroom-0.45.0/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/machineroom/sql.py` & `machineroom-0.45.0/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/machineroom/taskbase.py` & `machineroom-0.45.0/machineroom/taskbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
     cmd0 = f'cd {working_path} && {Config.BASH} {bash_file}'
     cmd1 = f'cd {working_path} && echo "" > {bash_file}'
     result = c.run(cmd0, pty=True, timeout=3000, warn=True)
     if result.ok and empty_content_after_execution:
         result = c.run(cmd1, pty=True, timeout=3600, warn=True)
     return result
 
+
 # Back up related commands
 def safe_cache_backup(c: Connection, local_file_name: str):
     """
     safely backup the working cache file in the remote server
     download the gz db to local
     """
     original_rm = os.path.join(Config.REMOTE_WS, "cache", "cache.db")
@@ -241,18 +242,31 @@
 
 
 def docker_solve_conflict(c: Connection, hash: str):
     c.run(DOCKER_STOP_ID.format(CID=hash, COMMAND_DOCKER=Config.DOCKER), pty=True, timeout=100, warn=True, echo=True)
     c.run(DOCKER_STOP_RM.format(CID=hash, COMMAND_DOCKER=Config.DOCKER), pty=True, timeout=100, warn=True, echo=True)
 
 
-def docker_launch(c: Connection, vol: str, container_name: str, image: str, ver: str, command: str) -> Result:
+def docker_launch(c: Connection, vol: Union[str, list[str]], container_name: str, image: str, ver: str, command: str,
+                  network: str = "") -> Result:
+    _vol = ""
+    if isinstance(vol, str):
+        _vol = f" -v {vol}"
+    if isinstance(vol, list):
+        _vol = " -v " + " -v ".join(vol)
+
+    if network != "":
+        _net = "--net " + network
+    else:
+        _net = ""
+
     return c.run(DOCKER_LAUNCH_LINE.format(
         COMMAND_DOCKER=Config.DOCKER,
-        VOLUME=vol,
+        VOLUME=_vol,
+        NETWORK=_net,
         NODE_NAME=container_name,
         IMAGE=image,
         VERSION=ver,
         COMMAND=command,
     ), pty=True, timeout=4900, warn=True, echo=True)
```

### Comparing `machineroom-0.44.9/machineroom/util.py` & `machineroom-0.45.0/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/machineroom/worker.py` & `machineroom-0.45.0/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/machineroom.egg-info/PKG-INFO` & `machineroom-0.45.0/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.44.9
+Version: 0.45.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.44.9/setup.py` & `machineroom-0.45.0/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.44.9/update` & `machineroom-0.45.0/update`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 git_update() {
   git add .
   git commit -m "auto patched"
   git push
 }
 
 pub_ver
-# git_update
+git_update
```

