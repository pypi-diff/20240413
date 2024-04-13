# Comparing `tmp/chuangliang-0.0.8.tar.gz` & `tmp/chuangliang-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chuangliang-0.0.8.tar", last modified: Fri Nov  3 04:14:06 2023, max compression
+gzip compressed data, was "chuangliang-0.0.9.tar", last modified: Tue Apr  9 07:49:28 2024, max compression
```

## Comparing `chuangliang-0.0.8.tar` & `chuangliang-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-11-03 04:14:06.696695 chuangliang-0.0.8/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-10-21 06:40:13.000000 chuangliang-0.0.8/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)      750 2023-11-03 04:14:06.696538 chuangliang-0.0.8/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      347 2023-10-21 06:40:13.000000 chuangliang-0.0.8/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-11-03 04:14:06.694025 chuangliang-0.0.8/chuangliang/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      228 2023-10-21 06:40:13.000000 chuangliang-0.0.8/chuangliang/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    17329 2023-11-03 04:13:34.000000 chuangliang-0.0.8/chuangliang/crawler.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      183 2023-10-21 06:40:13.000000 chuangliang-0.0.8/chuangliang/open_api.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-11-03 04:14:06.696298 chuangliang-0.0.8/chuangliang.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      750 2023-11-03 04:14:06.000000 chuangliang-0.0.8/chuangliang.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      271 2023-11-03 04:14:06.000000 chuangliang-0.0.8/chuangliang.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-11-03 04:14:06.000000 chuangliang-0.0.8/chuangliang.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2023-11-03 04:14:06.000000 chuangliang-0.0.8/chuangliang.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2023-11-03 04:14:06.000000 chuangliang-0.0.8/chuangliang.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-11-03 04:14:06.696799 chuangliang-0.0.8/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-11-03 04:13:34.000000 chuangliang-0.0.8/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-09 07:49:28.700591 chuangliang-0.0.9/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-10-21 06:40:13.000000 chuangliang-0.0.9/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      750 2024-04-09 07:49:28.700485 chuangliang-0.0.9/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      347 2023-10-21 06:40:13.000000 chuangliang-0.0.9/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-09 07:49:28.699789 chuangliang-0.0.9/chuangliang/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      228 2023-10-21 06:40:13.000000 chuangliang-0.0.9/chuangliang/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    17217 2024-04-09 07:48:55.000000 chuangliang-0.0.9/chuangliang/crawler.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      183 2023-10-21 06:40:13.000000 chuangliang-0.0.9/chuangliang/open_api.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-09 07:49:28.700329 chuangliang-0.0.9/chuangliang.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      750 2024-04-09 07:49:28.000000 chuangliang-0.0.9/chuangliang.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      271 2024-04-09 07:49:28.000000 chuangliang-0.0.9/chuangliang.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-09 07:49:28.000000 chuangliang-0.0.9/chuangliang.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-09 07:49:28.000000 chuangliang-0.0.9/chuangliang.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2024-04-09 07:49:28.000000 chuangliang-0.0.9/chuangliang.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-09 07:49:28.700631 chuangliang-0.0.9/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2024-04-09 07:48:55.000000 chuangliang-0.0.9/setup.py
```

### Comparing `chuangliang-0.0.8/LICENSE` & `chuangliang-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chuangliang-0.0.8/PKG-INFO` & `chuangliang-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chuangliang
-Version: 0.0.8
+Version: 0.0.9
 Summary: 创量广告平台SDK
 Home-page: https://gitee.com/ZeroSeeker/chuangliang
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chuangliang-0.0.8/chuangliang/crawler.py` & `chuangliang-0.0.9/chuangliang/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+from lazysdk import lazyrequests
 from lazysdk import lazytime
 from lazysdk import lazymd5
 from urllib import parse
 import requests
 import showlog
 import copy
 import json
@@ -80,21 +81,20 @@
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0",
     }
     data = {
         'email': email,
         'password': lazymd5.md5_str(password),
         'product_version': product_version
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
         headers=headers
     )
-    return response
 
 
 def login(
         email: str,
         password: str
 ):
     """
@@ -119,19 +119,20 @@
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0",
     }
     data = {
         'email': email,
         'password': lazymd5.md5_str(password)
     }
-    response = requests.request(
+    response = lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
-        headers=headers
+        headers=headers,
+        return_json=False
     )
     response_json = response.json()
     if response_json['code'] == 0:
         cookie_dict = requests.utils.dict_from_cookiejar(response.cookies)
         cookie_str = ''
         for cookie_key, cookie_value in cookie_dict.items():
             cookie_str += f'{cookie_key}={cookie_value}; '
@@ -178,21 +179,20 @@
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0",
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='GET',
         url=url,
         params=params,
         headers=headers
     )
-    return response.json()
 
 
 def get_material_report_sum(
         cookie: str,
         start_date: str = None,
         end_date: str = None,
         make_user_list: list = None,
@@ -274,21 +274,20 @@
         "Origin": "https://cl.mobgi.com",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0",
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
         headers=headers
     )
-    return response.json()
 
 
 def get_sub_user_list(
         cookie: str,
         page: int = 1,
         page_size: int = 10,
         keyword: str = None,
@@ -338,21 +337,20 @@
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0"
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='GET',
         url=url,
         params=params,
         headers=headers
     )
-    return response.json()
 
 
 def get_material_manage_list(
         cookie: str,
         page: int = 1,
         page_size: int = 20,
         keyword: str = "",
@@ -415,21 +413,20 @@
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0"
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
         headers=headers
     )
-    return response.json()
 
 
 def material_edit(
         cookie: str,
         material_id: int,
         material_name: str
 ):
@@ -460,21 +457,20 @@
         "Pragma": "no-cache",
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/118.0",
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
         headers=headers
     )
-    return response.json()
 
 
 def material_detail(
         cookie: str,
         material_id: int
 ):
     """
@@ -500,21 +496,20 @@
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "TE": "trailers",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:105.0) Gecko/20100101 Firefox/105.0"
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='GET',
         url=url,
         params=data,
         headers=headers
     )
-    return response.json()
 
 
 def material_group_child_list(
         cookie: str,
         special_id: int = 0,
         group_id: int = None
 ):
@@ -545,21 +540,20 @@
         "Pragma": "no-cache",
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/119.0"
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='GET',
         url=url,
         params=data,
         headers=headers
     )
-    return response.json()
 
 
 def material_move(
         cookie: str,
         material_ids: list,
         special_id: int = 0,
         group_id: int = None
@@ -592,14 +586,13 @@
         "Pragma": "no-cache",
         "Referer": "https://cl.mobgi.com/",
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-site",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/119.0"
     }
-    response = requests.request(
+    return lazyrequests.lazy_requests(
         method='POST',
         url=url,
         json=data,
         headers=headers
     )
-    return response.json()
```

### Comparing `chuangliang-0.0.8/chuangliang.egg-info/PKG-INFO` & `chuangliang-0.0.9/chuangliang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chuangliang
-Version: 0.0.8
+Version: 0.0.9
 Summary: 创量广告平台SDK
 Home-page: https://gitee.com/ZeroSeeker/chuangliang
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chuangliang-0.0.8/setup.py` & `chuangliang-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chuangliang",
-    version="0.0.8",
+    version="0.0.9",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="创量广告平台SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/chuangliang",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'lazysdk>=0.1.64'
+        'lazysdk>=0.1.89'
     ]
 )
```

