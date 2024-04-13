# Comparing `tmp/pynovnc-1.0.1.tar.gz` & `tmp/pynovnc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.0.1.tar", last modified: Sat Apr 13 07:01:42 2024, max compression
+gzip compressed data, was "pynovnc-1.0.2.tar", last modified: Sat Apr 13 07:53:17 2024, max compression
```

## Comparing `pynovnc-1.0.1.tar` & `pynovnc-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:01:42.839711 pynovnc-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 07:01:42.839711 pynovnc-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-04-13 07:01:34.000000 pynovnc-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:01:42.837710 pynovnc-1.0.1/pynovnc/
--rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-13 07:01:34.000000 pynovnc-1.0.1/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:01:42.838711 pynovnc-1.0.1/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 07:01:42.000000 pynovnc-1.0.1/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-13 07:01:42.000000 pynovnc-1.0.1/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 07:01:42.000000 pynovnc-1.0.1/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 07:01:42.000000 pynovnc-1.0.1/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 07:01:42.000000 pynovnc-1.0.1/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 07:01:42.839711 pynovnc-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2802 2024-04-13 07:01:34.000000 pynovnc-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:53:17.572260 pynovnc-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 07:53:17.572260 pynovnc-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-04-13 07:53:08.000000 pynovnc-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:53:17.570090 pynovnc-1.0.2/pynovnc/
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-13 07:53:08.000000 pynovnc-1.0.2/pynovnc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:53:17.572260 pynovnc-1.0.2/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 07:53:17.000000 pynovnc-1.0.2/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-13 07:53:17.000000 pynovnc-1.0.2/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 07:53:17.000000 pynovnc-1.0.2/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 07:53:17.000000 pynovnc-1.0.2/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 07:53:17.000000 pynovnc-1.0.2/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 07:53:17.572260 pynovnc-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2882 2024-04-13 07:53:08.000000 pynovnc-1.0.2/setup.py
```

### Comparing `pynovnc-1.0.1/PKG-INFO` & `pynovnc-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.1 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.2 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.0.1/README.md` & `pynovnc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.1/pynovnc/__init__.py` & `pynovnc-1.0.2/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.1/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.0.2/pynovnc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.1 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.2 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.0.1/setup.py` & `pynovnc-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-from setuptools import setup, find_packages
-import os , requests 
-import subprocess
-
-
-class PypiPublisher : 
-    def __init__(self, start_version = "1.0.0") : 
-        self.start_version = start_version
-        self.name = os.path.basename(os.getcwd())
-        print(f"Project name : {self.name}")
-        self.version , self.new_version = self.get_versions()
-        print(f"Project version : {self.version} -> {self.new_version }")
-        #######
-        author= subprocess.check_output(['git', 'config', 'user.name']).decode().strip()  if not os.environ.get("GITLAB_USER_NAME",None ) else os.environ.get("GITLAB_USER_NAME",None )  
-        #######
-        author_email= subprocess.check_output(['git', 'config', 'user.email']).decode().strip() if not  os.environ.get("GITLAB_USER_EMAIL", None ) else os.environ.get("GITLAB_USER_EMAIL", None ) 
-        ######
-        url  = subprocess.check_output(['git', 'remote', 'get-url', 'origin']).decode().strip() if not os.environ.get("CI_PROJECT_URL",None ) else os.environ.get("CI_PROJECT_URL",None )
-        ######
-        description  = 'Python Package made by Mhadhbi Issam . ' if not os.environ.get("CI_PROJECT_DESCRIPTION",None ) else os.environ.get("CI_PROJECT_DESCRIPTION",None )
-        setup(
-            name= os.path.basename(os.getcwd()),
-            version=self.new_version,
-            packages=find_packages(),
-            author= author  ,
-            author_email=author_email   ,
-            description= description,
-            long_description=open("README.md").read(),
-            long_description_content_type="text/markdown",
-            url= url    ,
-            install_requires=["bashi"]  ,
-            classifiers=[
-                'Programming Language :: Python :: 3',
-                'License :: OSI Approved :: MIT License',
-                'Operating System :: OS Independent',
-            ],
-        )
-    def get_versions(self) : 
-        response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
-        version = self.start_version
-        if response.status_code == 200 : 
-            version  = response.json()["info"]["version"]
-
-        new_version = self.upgrade_version(version)
-        return version , new_version
-
-    def upgrade_version(self,version) : 
-        major , minor , patch = map(int, version.split('.'))
-        newversion = str(patch + 10 * minor + 100 * major + 1)
-        a , b , c =  newversion[:-2]  , newversion[-2] , newversion[-1]
-        newer_version = ".".join([str(i) for i in [newversion[:-2]  , newversion[-2] , newversion[-1]]])
-        if newer_version.strip().startswith(".") : 
-            newer_version = "0" + newer_version.strip()
-        return newer_version
-
-
-if __name__ == '__main__':
+from setuptools import setup, find_packages
+import os , requests 
+import subprocess
+import subprocess
+
+
+
+
+
+class PypiPublisher : 
+    def __init__(self, start_version = "1.0.0") : 
+        self.start_version = start_version
+        self.name = subprocess.run(["git", "config", "--get", "remote.origin.url"], capture_output=True, text=True).stdout.strip().split("/")[-1].replace(".git", "")
+        print(f"Project name : {self.name}")
+        self.version , self.new_version = self.get_versions()
+        print(f"Project version : {self.version} -> {self.new_version }")
+        #######
+        author= subprocess.check_output(['git', 'config', 'user.name']).decode().strip()  if not os.environ.get("GITLAB_USER_NAME",None ) else os.environ.get("GITLAB_USER_NAME",None )  
+        #######
+        author_email= subprocess.check_output(['git', 'config', 'user.email']).decode().strip() if not  os.environ.get("GITLAB_USER_EMAIL", None ) else os.environ.get("GITLAB_USER_EMAIL", None ) 
+        ######
+        url  = subprocess.check_output(['git', 'remote', 'get-url', 'origin']).decode().strip() if not os.environ.get("CI_PROJECT_URL",None ) else os.environ.get("CI_PROJECT_URL",None )
+        ######
+        description  = 'Python Package made by Mhadhbi Issam . ' if not os.environ.get("CI_PROJECT_DESCRIPTION",None ) else os.environ.get("CI_PROJECT_DESCRIPTION",None )
+        setup(
+            name= os.path.basename(os.getcwd()),
+            version=self.new_version,
+            packages=find_packages(),
+            author= author  ,
+            author_email=author_email   ,
+            description= description,
+            long_description=open("README.md").read(),
+            long_description_content_type="text/markdown",
+            url= url    ,
+            install_requires=["bashi"]  ,
+            classifiers=[
+                'Programming Language :: Python :: 3',
+                'License :: OSI Approved :: MIT License',
+                'Operating System :: OS Independent',
+            ],
+        )
+    def get_versions(self) : 
+        response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
+        version = self.start_version
+        if response.status_code == 200 : 
+            version  = response.json()["info"]["version"]
+
+        new_version = self.upgrade_version(version)
+        return version , new_version
+
+    def upgrade_version(self,version) : 
+        major , minor , patch = map(int, version.split('.'))
+        newversion = str(patch + 10 * minor + 100 * major + 1)
+        a , b , c =  newversion[:-2]  , newversion[-2] , newversion[-1]
+        newer_version = ".".join([str(i) for i in [newversion[:-2]  , newversion[-2] , newversion[-1]]])
+        if newer_version.strip().startswith(".") : 
+            newer_version = "0" + newer_version.strip()
+        return newer_version
+
+
+if __name__ == '__main__':
     PypiPublisher()
```

