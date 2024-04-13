# Comparing `tmp/AgentlyCmd-0.0.0.1a3.tar.gz` & `tmp/AgentlyCmd-0.0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgentlyCmd-0.0.0.1a3.tar", last modified: Sat Apr 13 08:44:32 2024, max compression
+gzip compressed data, was "AgentlyCmd-0.0.0.1a4.tar", last modified: Sat Apr 13 08:45:27 2024, max compression
```

## Comparing `AgentlyCmd-0.0.0.1a3.tar` & `AgentlyCmd-0.0.0.1a4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:44:32.516328 AgentlyCmd-0.0.0.1a3/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:44:32.515179 AgentlyCmd-0.0.0.1a3/AgentlyCmd/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-13 08:27:56.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      975 2024-04-13 08:44:13.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd/cmd.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:44:32.515988 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      414 2024-04-13 08:44:32.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)      222 2024-04-13 08:44:32.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-13 08:44:32.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)       48 2024-04-13 08:44:32.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/entry_points.txt
--rw-r--r--   0 moxin      (501) staff       (20)       11 2024-04-13 08:44:32.000000 AgentlyCmd-0.0.0.1a3/AgentlyCmd.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      414 2024-04-13 08:44:32.516159 AgentlyCmd-0.0.0.1a3/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-13 08:44:32.516386 AgentlyCmd-0.0.0.1a3/setup.cfg
--rw-r--r--   0 moxin      (501) staff       (20)      696 2024-04-13 08:44:22.000000 AgentlyCmd-0.0.0.1a3/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:45:27.775944 AgentlyCmd-0.0.0.1a4/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:45:27.774822 AgentlyCmd-0.0.0.1a4/AgentlyCmd/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-13 08:27:56.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      968 2024-04-13 08:45:20.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd/cmd.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 08:45:27.775599 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      414 2024-04-13 08:45:27.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)      222 2024-04-13 08:45:27.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-13 08:45:27.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)       48 2024-04-13 08:45:27.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/entry_points.txt
+-rw-r--r--   0 moxin      (501) staff       (20)       11 2024-04-13 08:45:27.000000 AgentlyCmd-0.0.0.1a4/AgentlyCmd.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      414 2024-04-13 08:45:27.775781 AgentlyCmd-0.0.0.1a4/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-13 08:45:27.775984 AgentlyCmd-0.0.0.1a4/setup.cfg
+-rw-r--r--   0 moxin      (501) staff       (20)      696 2024-04-13 08:45:23.000000 AgentlyCmd-0.0.0.1a4/setup.py
```

### Comparing `AgentlyCmd-0.0.0.1a3/AgentlyCmd/cmd.py` & `AgentlyCmd-0.0.0.1a4/AgentlyCmd/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         print(f"\033[91m\033[47m\033[3m\033[1m Agent\033[34mly\033[30m.Tech \033[0m Project Creator")
         project_name = "agently_project"
         if len(args) >= 1:
             project_name = "_".join(args)
         else:
             print("No project name is given. Use 'agently_project' by default.")
         print(f"Creating project '{ project_name }'...")
-        subprocess.run(["git", "git", "clone", "https://gitee.com/maplemx/agently-ws.git"])
+        subprocess.run(["git", "clone", "https://gitee.com/maplemx/agently-ws.git"])
         os.rename("agently-ws", project_name)
         print("Done. Happy coding!")
         return
 
 def main():
     command_name = ""
     args = []
```

### Comparing `AgentlyCmd-0.0.0.1a3/setup.py` & `AgentlyCmd-0.0.0.1a4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = "AgentlyCmd",
-    version = "0.0.0.1-alpha-3",
+    version = "0.0.0.1-alpha-4",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently Shell Command.",
     long_description = "Agently Shell Command.",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     packages = setuptools.find_packages(),
```

