# Comparing `tmp/argsreq-1.5.tar.gz` & `tmp/argsreq-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsreq-1.5.tar", last modified: Sat Apr 13 09:07:57 2024, max compression
+gzip compressed data, was "argsreq-1.6.tar", last modified: Sat Apr 13 09:13:54 2024, max compression
```

## Comparing `argsreq-1.5.tar` & `argsreq-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.902454 argsreq-1.5/
--rw-rw-rw-   0        0        0      311 2024-04-13 09:07:57.901434 argsreq-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.898553 argsreq-1.5/argsreq.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.901434 argsreq-1.5/reqargs/
--rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:08.000000 argsreq-1.5/reqargs/__init__.py
--rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.5/reqargs/__main__.py
--rw-rw-rw-   0        0        0    15372 2024-04-13 08:50:18.000000 argsreq-1.5/reqargs/colorls.py
--rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:22.000000 argsreq-1.5/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-13 09:07:57.903463 argsreq-1.5/setup.cfg
--rw-rw-rw-   0        0        0      641 2024-04-13 09:07:49.000000 argsreq-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 09:13:54.708358 argsreq-1.6/
+-rw-rw-rw-   0        0        0      311 2024-04-13 09:13:54.708358 argsreq-1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 09:13:54.705357 argsreq-1.6/argsreq.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-13 09:13:54.000000 argsreq-1.6/argsreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-13 09:13:54.000000 argsreq-1.6/argsreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 09:13:54.000000 argsreq-1.6/argsreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 09:13:54.000000 argsreq-1.6/argsreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 09:13:54.707482 argsreq-1.6/reqargs/
+-rw-rw-rw-   0        0        0    15741 2024-04-13 09:13:16.000000 argsreq-1.6/reqargs/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.6/reqargs/__main__.py
+-rw-rw-rw-   0        0        0    15327 2024-04-13 09:13:34.000000 argsreq-1.6/reqargs/colorls.py
+-rw-rw-rw-   0        0        0    15741 2024-04-13 09:13:38.000000 argsreq-1.6/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 09:13:54.709340 argsreq-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      641 2024-04-13 09:13:46.000000 argsreq-1.6/setup.py
```

### Comparing `argsreq-1.5/reqargs/__init__.py` & `argsreq-1.6/reqargs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             print(s1)
         print('\n')
 
 
 def get_config():
     config = ConfigParser()
     config.read([
-                os.path.join(sys.prefix, 'colorls/config/colorls.toml'),
-                os.path.join(site.USER_BASE, 'colorls/config/colorls.toml'),
-                os.path.expanduser('~/.config/colorls.toml'),
+                os.path.join(sys.prefix, 'colorls.toml'),
+                os.path.join(site.USER_BASE, 'colorls.toml'),
+                os.path.expanduser('~/colorls.toml'),
                 os.path.expanduser('~/.colorls.toml'),
-                os.path.join(Path(__file__).parent.absolute(), 'config/colorls.toml'),
+                os.path.join(Path(__file__).parent.absolute(), 'colorls.toml'),
                 ], encoding='utf8')
     return dict(config['FORMATTING']), dict(config['ICONS']), dict(config['ALIASES']), dict(config['SUFFIXES'])
 
 
 ANSI, ICONS, ALIAS, SUFFIX = get_config()
```

### Comparing `argsreq-1.5/reqargs/colorls.py` & `argsreq-1.6/reqargs/colorls.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             print(s1)
         print('\n')
 
 
 def get_config():
     config = ConfigParser()
     config.read([
-                os.path.join(sys.prefix, 'colorls/config/colorls.toml'),
-                os.path.join(site.USER_BASE, 'colorls/config/colorls.toml'),
-                os.path.expanduser('~/.config/colorls.toml'),
+                os.path.join(sys.prefix, 'colorls.toml'),
+                os.path.join(site.USER_BASE, 'colorls.toml'),
+                os.path.expanduser('~/colorls.toml'),
                 os.path.expanduser('~/.colorls.toml'),
-                os.path.join(Path(__file__).parent.absolute(), 'config/colorls.toml'),
+                os.path.join(Path(__file__).parent.absolute(), 'colorls.toml'),
                 ], encoding='utf8')
     return dict(config['FORMATTING']), dict(config['ICONS']), dict(config['ALIASES']), dict(config['SUFFIXES'])
 
 
 ANSI, ICONS, ALIAS, SUFFIX = get_config()
```

### Comparing `argsreq-1.5/reqargs/reqargs.py` & `argsreq-1.6/reqargs/reqargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             print(s1)
         print('\n')
 
 
 def get_config():
     config = ConfigParser()
     config.read([
-                os.path.join(sys.prefix, 'colorls/config/colorls.toml'),
-                os.path.join(site.USER_BASE, 'colorls/config/colorls.toml'),
-                os.path.expanduser('~/.config/colorls.toml'),
+                os.path.join(sys.prefix, 'colorls.toml'),
+                os.path.join(site.USER_BASE, 'colorls.toml'),
+                os.path.expanduser('~/colorls.toml'),
                 os.path.expanduser('~/.colorls.toml'),
-                os.path.join(Path(__file__).parent.absolute(), 'config/colorls.toml'),
+                os.path.join(Path(__file__).parent.absolute(), 'colorls.toml'),
                 ], encoding='utf8')
     return dict(config['FORMATTING']), dict(config['ICONS']), dict(config['ALIASES']), dict(config['SUFFIXES'])
 
 
 ANSI, ICONS, ALIAS, SUFFIX = get_config()
```

### Comparing `argsreq-1.5/setup.py` & `argsreq-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5'
+VERSION = '1.6'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="argsreq",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
```

