# Comparing `tmp/machineroom-0.45.0.tar.gz` & `tmp/machineroom-0.45.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.45.0.tar", last modified: Sat Apr 13 11:13:59 2024, max compression
+gzip compressed data, was "machineroom-0.45.1.tar", last modified: Sat Apr 13 17:13:32 2024, max compression
```

## Comparing `machineroom-0.45.0.tar` & `machineroom-0.45.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.189813 machineroom-0.45.0/
--rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.0/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 11:13:59.189637 machineroom-0.45.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.180806 machineroom-0.45.0/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.0/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.186111 machineroom-0.45.0/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-13 11:13:58.000000 machineroom-0.45.0/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5260 2024-04-13 11:13:02.000000 machineroom-0.45.0/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.0/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    13315 2024-03-22 10:56:07.000000 machineroom-0.45.0/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    19685 2024-04-13 11:13:02.000000 machineroom-0.45.0/machineroom/taskbase.py
--rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.0/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.0/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 11:13:59.189067 machineroom-0.45.0/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      371 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-13 11:13:59.000000 machineroom-0.45.0/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-13 11:13:59.190412 machineroom-0.45.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.0/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.0/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-13 11:13:46.000000 machineroom-0.45.0/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.539594 machineroom-0.45.1/
+-rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.1/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 17:13:32.539328 machineroom-0.45.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.528636 machineroom-0.45.1/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.1/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.535496 machineroom-0.45.1/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7488 2024-04-13 17:01:00.000000 machineroom-0.45.1/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.1/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    13510 2024-04-13 15:24:08.000000 machineroom-0.45.1/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    22572 2024-04-13 17:12:48.000000 machineroom-0.45.1/machineroom/taskbase.py
+-rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.1/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.1/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.538606 machineroom-0.45.1/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      371 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-13 17:13:32.540535 machineroom-0.45.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.1/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.1/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-13 17:13:20.000000 machineroom-0.45.1/version
```

### Comparing `machineroom-0.45.0/.gitignore` & `machineroom-0.45.1/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/LICENSE` & `machineroom-0.45.1/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/PKG-INFO` & `machineroom-0.45.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.0
+Version: 0.45.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.0/README.md` & `machineroom-0.45.1/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/cmdbin/connect` & `machineroom-0.45.1/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/machineroom/__init__.py` & `machineroom-0.45.1/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.45.0'
+__version__ = '0.45.1'
```

### Comparing `machineroom-0.45.0/machineroom/const.py` & `machineroom-0.45.1/machineroom/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -103,22 +103,21 @@
     echo "推荐的端口如下："
     for port in "${ports[@]}"; do
         echo -e "\033[0;32m$port\033[0m"
     done
 }
 list_recommended_ports;"""
 DOCKER_STOP_REMOVE = """{COMMAND_DOCKER} rm $({COMMAND_DOCKER} stop $(sudo docker ps -a | grep "{CONTAINER_NAME}" | cut -d " " -f 1))"""
-DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d {VOLUME} {NETWORK} --restart unless-stopped --name {NODE_NAME} {IMAGE}:{VERSION} {COMMAND}"""
+DOCKER_LAUNCH_LINE = """{COMMAND_DOCKER} run -d {VOLUME} {NETWORK} --restart unless-stopped --name {NODE_NAME} {IMAGE}{VERSION} {COMMAND}"""
 DOCKER_STOP_ID = """{COMMAND_DOCKER} stop {CID}"""
 DOCKER_STOP_RM = """{COMMAND_DOCKER} rm {CID}"""
 DOCKER_STOP_CONTAIN_NAME = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs {COMMAND_DOCKER} stop"""
 DOCKER_RM_NAME_BASED = """{COMMAND_DOCKER} ps -a | grep '{CONTAINER_NAME}' | awk '{{print $1}}' | xargs -r {COMMAND_DOCKER} rm -f"""
 DOCKER_RM_VOLUME = """{COMMAND_DOCKER} volume ls -qf dangling=true -f name={CONTAINER_NAME} | xargs -r {COMMAND_DOCKER} volume rm"""
 DOCKER_LOG_REVIEW = """COMMAND_DOCKER ps -a --filter "name=__CONTAINER_KEYWORD" --format "{{.ID}}" | shuf -n 1 | xargs docker logs --tail __RECENT_LINES"""
-
 BACKUP_CACHE_FAST = """
 # Define the path to the file
 path_to_file="_CFP_"
 # Check if the file exists
 if [ -f "$path_to_file" ]; then
     # Go to the directory of the file
     cd "$(dirname "$path_to_file")" || exit
@@ -128,7 +127,104 @@
             tar -czvf _FR_ $(basename "$path_to_file")
             if [ $? -eq 0 ]; then
                 break
             fi
         done
     echo "compress file success"
 fi"""
+DOCKER_COMPOSE_XCLASH = """
+version: '3.7'
+services:
+  proxy_service:
+    image: dreamacro/clash
+    container_name: clashmoe
+    ports:
+      - "17890:17890"
+      - "17891:17891"
+    volumes:
+      - ./clash_conf/X_CLASH_CONFIG_YAML_NM:/root/.config/clash/config.yaml:ro
+      - ./clash_conf:/root/.config/clash
+    restart: always
+    # When your system is Linux, you can use `network_mode: "host"` directly.
+    # network_mode: host
+    # clash_docker_default
+    privileged: true
+    expose:
+      - 7890
+      - 7891
+      - 17890
+      - 9090
+    networks:
+      - clsh_octopus_network
+
+  proxy_control_service:
+    image: adriansteward/galxewrok:X_CLASH_GALXE_HELPER_VER
+    container_name: clash_checker
+    restart: "on-failure"
+    command: python clash_runtime.py
+    networks:
+      - clsh_octopus_network
+    depends_on:
+      - proxy_service
+    volumes:
+      - ./config:./cache
+networks:
+  clsh_octopus_network:
+
+
+"""
+CLASH_HELPER_RESOURCE = """{
+  "clash_proxy": {
+    "port": "7890",
+    "secret": "___SECRET___",
+    "conn_file": "/home/clashperfectoctopus/config/proxy_config.json",
+    "selector": "___SELECTOR___",
+    "test_endpoint": "__TEST_ENDPOINT__"
+  }
+}
+"""
+
+CLASH_SETUP_1 = """
+network_name="clsh_octopus_network"
+docker network inspect "$network_name" >/dev/null 2>&1 || docker network create "$network_name"
+
+if [ -d "/home/clashperfectoctopus" ]; then
+  cd /home/clashperfectoctopus
+  git pull https://github.com/ONode/clashperfectoctopus.git
+else
+  echo "Directory does not exist."
+  cd /home
+  git clone https://github.com/ONode/clashperfectoctopus
+  cd clashperfectoctopus
+fi
+
+cat > docker_proxy_compose.yml << 'EOF'
+_CONTENT_DOCKER_COMPOSE
+EOF
+cd /home/clashperfectoctopus/config
+cat > resources.json << 'EOF'
+_RESOURCE_JSON
+EOF
+
+cd /home/clashperfectoctopus
+echo "clean up the containers"
+docker container prune -f
+
+echo "add YAML config file"
+
+
+"""
+CLASH_SETUP_2="""
+configuration_yaml_xsh="_PATH_CLASH"
+
+if [ -f "$configuration_yaml_xsh" ]; then
+    echo "$configuration_yaml_xsh is a file."
+else
+    echo "$configuration_yaml_xsh is not a file."
+    echo "wait until you have the correct configuration file install first."
+    exit;
+fi
+
+echo "start up the service"
+bash clash_up.sh
+
+"""
```

### Comparing `machineroom-0.45.0/machineroom/schema.json` & `machineroom-0.45.1/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/machineroom/sql.py` & `machineroom-0.45.1/machineroom/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,30 +252,38 @@
 
     def docker_ce_install(self):
         self._update_what_installed("docker_installed")
 
     def docker_compose_install(self):
         self._update_what_installed("docker_compose_installed")
 
+    def docker_clash_install(self):
+        return self._update_what_installed("clash_installed")
+
     def docker_yacht_install(self):
         self._update_what_installed("yacht_installed")
 
     def python3_install(self):
         self._update_what_installed("python3_installed")
+
     def dae_install(self):
         self._update_what_installed("daed_installed")
+
     def is_docker_compose_installed(self):
         return self._is_what_installed("docker_compose_installed")
 
     def is_docker_yacht_installed(self):
         return self._is_what_installed("yacht_installed")
 
     def is_dae_installed(self):
         return self._is_what_installed("daed_installed")
 
+    def is_xclash_installed(self):
+        return self._is_what_installed("clash_installed")
+
     def is_docker_ce_installed(self):
         return self._is_what_installed("docker_installed")
 
     def is_python_installed(self):
         return self._is_what_installed("python3_installed")
 
     def is_cert_installed(self):
```

### Comparing `machineroom-0.45.0/machineroom/taskbase.py` & `machineroom-0.45.1/machineroom/taskbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os.path
+
 import pexpect
 from fabric import Connection, Config as FabricConfig, Result
 from machineroom.sql import ServerRoom
 from machineroom.util import *
 
 
 def copy_id(c: Connection, file: str = Config.PUB_KEY):
@@ -255,21 +257,26 @@
         _vol = " -v " + " -v ".join(vol)
 
     if network != "":
         _net = "--net " + network
     else:
         _net = ""
 
+    if ver == "" or ver is None:
+        _ver = ""
+    else:
+        _ver = f":{ver}"
+
     return c.run(DOCKER_LAUNCH_LINE.format(
         COMMAND_DOCKER=Config.DOCKER,
         VOLUME=_vol,
         NETWORK=_net,
         NODE_NAME=container_name,
         IMAGE=image,
-        VERSION=ver,
+        VERSION=_ver,
         COMMAND=command,
     ), pty=True, timeout=4900, warn=True, echo=True)
 
 
 def stop_container_by_name(c: Connection, container_name: str):
     cmd_line_go = DOCKER_STOP_CONTAIN_NAME.format(
         COMMAND_DOCKER=Config.DOCKER,
@@ -404,14 +411,66 @@
 
 def install_docker_compose(c: Connection):
     exec_shell_global(c, DOCKER_COMPOSE.format(
         DOCKER_COMPOSE_VERSION=Config.DOCKER_COMPOSE_VERSION
     ))
 
 
+def docker_launch_solution(c: Connection, node_name: str, pass_file: str):
+    print("use container name", node_name)
+    _command_line = f"python main_exe.py {pass_file}"
+    sentence = docker_launch(
+        c=c,
+        container_name=node_name,
+        vol=[
+            "/home/galxeionetapplication/cache:/home/galxe/cache",
+            "/home/clash_docker/config/proxy_config.json:/home/galxe/cache/proxy_config.json"
+        ],
+        image="adriansteward/galxewrok",
+        ver="",
+        command=_command_line
+    )
+    (issue, hash) = docker_is_container_conflict(sentence)
+    if issue:
+        docker_solve_conflict(c, hash)
+        docker_launch_solution(c, node_name, pass_file)
+
+
+def install_clash_network(
+        c: Connection,
+        network_config_file: str,
+        helper_version: str,
+        external_token_access: str,
+        selector: str,
+        tst_endpoint: str
+):
+    # network config is yaml file format
+    docker_file = DOCKER_COMPOSE_XCLASH \
+        .replace("X_CLASH_CONFIG_YAML_NM", network_config_file) \
+        .replace("X_CLASH_GALXE_HELPER_VER", "1.2.1291" if helper_version == "" else helper_version)
+    resrc = CLASH_HELPER_RESOURCE \
+        .replace("___SECRET___", external_token_access) \
+        .replace("___SELECTOR___", selector).replace(
+        "__TEST_ENDPOINT__", tst_endpoint)
+    network_cfg = os.path.join("home", "clashperfectoctopus", "clash_conf", network_config_file)
+    network_cfg_local = os.path.join(Config.DATAPATH_BASE, "clash_config", network_config_file)
+    content = CLASH_SETUP_1 \
+        .replace("_CONTENT_DOCKER_COMPOSE", docker_file) \
+        .replace("_RESOURCE_JSON", resrc)
+    exec_shell_program(c, "/tmp", content)
+    if os.path.isfile(network_cfg_local) is False:
+        print("aborted the network config file is not found from", network_cfg_local)
+        return
+    ensure_path_exist()
+    c.put(network_cfg_local, network_cfg)
+    content2 = CLASH_SETUP_2 \
+        .replace("_PATH_CLASH", network_cfg)
+    exec_shell_program(c, "/tmp", content2)
+
+
 class DeploymentBotFoundation:
     # the text file servers that recorded the authentications and some basic information
     srv: Servers
     # the local db connection of servers
     db: ServerRoom
 
     def __init__(self, server_room: str):
@@ -535,14 +594,33 @@
         if task == "daed":
             if self.db.is_dae_installed() is False:
                 if detect_program(c, "daed") is False:
                     print("daed will be installed")
                     install_dae_proxy(c)
                     self.db.dae_install()
 
+        if task == "clash":
+            if self.db.is_xclash_installed() is False:
+                if check_docker_ps_specific(c, "dreamacro/clash") is False:
+                    print("dreamacro.clash will be installed")
+                    if self.install_xclash(1) is True:
+                        self.db.docker_clash_install()
+            else:
+                if self.install_xclash_update() is True:
+                    if self.install_xclash(2) is True:
+                        print("xclash is updated.")
+
         if task.startswith("yacht"):
             port = task.replace("yacht", "")
             if port == "":
                 port = "9055"
             if self.db.is_docker_yacht_installed() is False:
                 install_container_management_utility(c, int(port))
                 self.db.docker_yacht_install()
+
+    def install_xclash(self, install_times: int) -> bool:
+        # if check_docker_ps_specific(c, "dreamacro/clash") is False:...
+
+        return False
+
+    def install_xclash_update(self) -> bool:
+        return False
```

### Comparing `machineroom-0.45.0/machineroom/util.py` & `machineroom-0.45.1/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/machineroom/worker.py` & `machineroom-0.45.1/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/machineroom.egg-info/PKG-INFO` & `machineroom-0.45.1/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.0
+Version: 0.45.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.0/setup.py` & `machineroom-0.45.1/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.0/update` & `machineroom-0.45.1/update`

 * *Files identical despite different names*

