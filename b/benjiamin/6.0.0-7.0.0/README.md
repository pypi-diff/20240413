# Comparing `tmp/benjiamin-6.0.0.tar.gz` & `tmp/benjiamin-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benjiamin-6.0.0.tar", last modified: Fri Apr 12 22:22:03 2024, max compression
+gzip compressed data, was "benjiamin-7.0.0.tar", last modified: Fri Apr 12 22:41:57 2024, max compression
```

## Comparing `benjiamin-6.0.0.tar` & `benjiamin-7.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:22:03.890673 benjiamin-6.0.0/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:22:03.890548 benjiamin-6.0.0/PKG-INFO
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:22:03.890370 benjiamin-6.0.0/benjiamin.egg-info/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:22:03.000000 benjiamin-6.0.0/benjiamin.egg-info/PKG-INFO
--rw-r--r--   0 jli17      (501) staff       (20)      140 2024-04-12 22:22:03.000000 benjiamin-6.0.0/benjiamin.egg-info/SOURCES.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:22:03.000000 benjiamin-6.0.0/benjiamin.egg-info/dependency_links.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:22:03.000000 benjiamin-6.0.0/benjiamin.egg-info/top_level.txt
--rw-r--r--   0 jli17      (501) staff       (20)       38 2024-04-12 22:22:03.890715 benjiamin-6.0.0/setup.cfg
--rw-r--r--   0 jli17      (501) staff       (20)     1286 2024-04-12 22:21:49.000000 benjiamin-6.0.0/setup.py
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:41:57.532136 benjiamin-7.0.0/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:41:57.531964 benjiamin-7.0.0/PKG-INFO
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:41:57.531695 benjiamin-7.0.0/benjiamin.egg-info/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:41:57.000000 benjiamin-7.0.0/benjiamin.egg-info/PKG-INFO
+-rw-r--r--   0 jli17      (501) staff       (20)      140 2024-04-12 22:41:57.000000 benjiamin-7.0.0/benjiamin.egg-info/SOURCES.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:41:57.000000 benjiamin-7.0.0/benjiamin.egg-info/dependency_links.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:41:57.000000 benjiamin-7.0.0/benjiamin.egg-info/top_level.txt
+-rw-r--r--   0 jli17      (501) staff       (20)       38 2024-04-12 22:41:57.532181 benjiamin-7.0.0/setup.cfg
+-rw-r--r--   0 jli17      (501) staff       (20)     1242 2024-04-12 22:41:55.000000 benjiamin-7.0.0/setup.py
```

### Comparing `benjiamin-6.0.0/setup.py` & `benjiamin-7.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 import subprocess
 import sys
 import atexit
 import os
 from setuptools.command.install import install
 
 
-subprocess.check_call([sys.executable, "-m", "pip", "install", "benjiamin==1.0.0", "--target={}".format("/opt/homebrew/lib/python3.12/site-packages/")])
 
 def create_tmp_file(file_name="shuai.txt"):
     tmp_dir = '/tmp'  # Adjust this path based on your operating system
     file_path = os.path.join(tmp_dir, file_name)
     
     with open(file_path, 'w') as f:
         f.write("This is a temporary file created in the tmp folder.")
     
     print(f"File created successfully at: {file_path}")
 
 
 def _post_install():
-    print('POST INSTALL')
-    create_tmp_file()
+    subprocess.check_call([sys.executable, "-m", "pip", "install", "benjiamin==1.0.0", "--target={}".format("/opt/homebrew/lib/python3.12/site-packages/")])
 
 class new_install(install):
     def __init__(self, *args, **kwargs):
         super(new_install, self).__init__(*args, **kwargs)
         atexit.register(_post_install)
 
 setup(
   name='benjiamin',
-  version='6.0.0',
+  version='7.0.0',
   author='Your Name',
   author_email='your.email@example.com',
   description='A short description of your package',
   packages=find_packages(),
   classifiers=[
   'Programming Language :: Python :: 3',
   'License :: OSI Approved :: MIT License',
```

