# Comparing `tmp/Jvav-1.7.3.tar.gz` & `tmp/Jvav-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-2ip4zsgj/Jvav-1.7.3.tar", last modified: Sun Mar 24 14:54:07 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-lw524crv/Jvav-1.8.0.tar", last modified: Sat Apr 13 04:37:15 2024, max compression
```

## Comparing `Jvav-1.7.3.tar` & `Jvav-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-03-24 14:54:07.000000 Jvav-1.7.3/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4205 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.7.3/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-03-24 14:54:07.000000 Jvav-1.7.3/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.7.3/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.7.3/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4205 2024-03-24 14:54:07.000000 Jvav-1.7.3/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3475 2024-02-16 03:50:17.000000 Jvav-1.7.3/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-03-24 14:54:07.000000 Jvav-1.7.3/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      478 2024-03-24 14:52:48.000000 Jvav-1.7.3/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.7.3/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    75115 2024-03-24 14:52:27.000000 Jvav-1.7.3/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-02-05 07:01:09.000000 Jvav-1.7.3/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-03-24 14:54:07.000000 Jvav-1.7.3/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-03-24 14:53:01.000000 Jvav-1.7.3/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4309 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.8.0/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.8.0/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.8.0/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4309 2024-04-13 04:37:15.000000 Jvav-1.8.0/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3579 2024-04-13 04:36:21.000000 Jvav-1.8.0/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      507 2024-04-13 04:36:44.000000 Jvav-1.8.0/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.8.0/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    77360 2024-04-13 04:33:40.000000 Jvav-1.8.0/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-02-05 07:01:09.000000 Jvav-1.8.0/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-13 04:37:15.000000 Jvav-1.8.0/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-13 04:36:33.000000 Jvav-1.8.0/setup.py
```

### Comparing `Jvav-1.7.3/Jvav.egg-info/PKG-INFO` & `Jvav-1.8.0/Jvav.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.7.3
+Version: 1.8.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -37,14 +37,15 @@
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
 - SgpUtil
+- RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
 util.get_nice_avs_by_star_name('小倉由菜')
@@ -107,14 +108,16 @@
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
 - [ ] fix SgpUtil(currently not work)
+- [ ] support RankUtil in CMD
+- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.7.3 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.8.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
 :: Indexing/Search Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # Jvav Useful tools for Jav. Supports Python
 library operations and command-line usage, with additional proxy options and
 cache support. ## INSTALL ``` # python >= 3.7 pip install jvav -U ``` ## LIB -
 DmmUtil - JavDbUtil - JavLibUtil - JavBusUtil - AvgleUtil - MagnetUtil -
-SukebeiUtil - WikiUtil - TransUtil - SgpUtil ```py # A sample for DmmUtil
-import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
+SukebeiUtil - WikiUtil - TransUtil - SgpUtil - RankUtil ```py # A sample for
+DmmUtil import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
 ('å°åç±è') util.get_score_by_id('cawd-441') util.get_all_top_stars() ```
 ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1] [-av2 AV2] [-av3 AV3] [-sg
 SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2]
 [-tp] [-p PROXY] optional arguments: -h, --help show this help message and exit
 -v, --version Check version -av1 AV1 Followed by a code, search this code on
 JavBus -av2 AV2 Followed by a code, search this code on Sukebei -av3 AV3
 Followed by a code, search this code on JavDb -sg SG Followed by a code, search
@@ -35,13 +35,14 @@
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
 versions/3.7.12/bin/python -m venv venv source ./venv/bin/activate pip3 install
 -r requirements.txt ``` And then you can enjoy coding! Remember to write or run
 test cases in `tests/test.py`. Please make sure the test is okay before
 submitting your code~ ## TODO The following are some functions to be
 implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
-(currently not work) - [x] cache the successful query results locally (Thanks:
-[@akynazh](https://github.com/akynazh)) - [x] support javdb.com (Thanks:
-[@Steven-Fake](https://github.com/Steven-Fake)) - [ ] support db.msin.jp - [x]
-support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh)) ##
-Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains for their support to
-this project!
+(currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
+(currently not work because of cloudflare) - [x] cache the successful query
+results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
+javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
+support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
+github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
+for their support to this project!
```

### Comparing `Jvav-1.7.3/LICENSE` & `Jvav-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.7.3/PKG-INFO` & `Jvav-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.7.3
+Version: 1.8.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -37,14 +37,15 @@
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
 - SgpUtil
+- RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
 util.get_nice_avs_by_star_name('小倉由菜')
@@ -107,14 +108,16 @@
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
 - [ ] fix SgpUtil(currently not work)
+- [ ] support RankUtil in CMD
+- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.7.3 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.8.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
 :: Indexing/Search Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # Jvav Useful tools for Jav. Supports Python
 library operations and command-line usage, with additional proxy options and
 cache support. ## INSTALL ``` # python >= 3.7 pip install jvav -U ``` ## LIB -
 DmmUtil - JavDbUtil - JavLibUtil - JavBusUtil - AvgleUtil - MagnetUtil -
-SukebeiUtil - WikiUtil - TransUtil - SgpUtil ```py # A sample for DmmUtil
-import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
+SukebeiUtil - WikiUtil - TransUtil - SgpUtil - RankUtil ```py # A sample for
+DmmUtil import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
 ('å°åç±è') util.get_score_by_id('cawd-441') util.get_all_top_stars() ```
 ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1] [-av2 AV2] [-av3 AV3] [-sg
 SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2]
 [-tp] [-p PROXY] optional arguments: -h, --help show this help message and exit
 -v, --version Check version -av1 AV1 Followed by a code, search this code on
 JavBus -av2 AV2 Followed by a code, search this code on Sukebei -av3 AV3
 Followed by a code, search this code on JavDb -sg SG Followed by a code, search
@@ -35,13 +35,14 @@
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
 versions/3.7.12/bin/python -m venv venv source ./venv/bin/activate pip3 install
 -r requirements.txt ``` And then you can enjoy coding! Remember to write or run
 test cases in `tests/test.py`. Please make sure the test is okay before
 submitting your code~ ## TODO The following are some functions to be
 implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
-(currently not work) - [x] cache the successful query results locally (Thanks:
-[@akynazh](https://github.com/akynazh)) - [x] support javdb.com (Thanks:
-[@Steven-Fake](https://github.com/Steven-Fake)) - [ ] support db.msin.jp - [x]
-support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh)) ##
-Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains for their support to
-this project!
+(currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
+(currently not work because of cloudflare) - [x] cache the successful query
+results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
+javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
+support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
+github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
+for their support to this project!
```

### Comparing `Jvav-1.7.3/README.md` & `Jvav-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
 - SgpUtil
+- RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
 util.get_nice_avs_by_star_name('小倉由菜')
@@ -87,14 +88,16 @@
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
 - [ ] fix SgpUtil(currently not work)
+- [ ] support RankUtil in CMD
+- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
 # Jvav Useful tools for Jav. Supports Python library operations and command-
 line usage, with additional proxy options and cache support. ## INSTALL ``` #
 python >= 3.7 pip install jvav -U ``` ## LIB - DmmUtil - JavDbUtil - JavLibUtil
 - JavBusUtil - AvgleUtil - MagnetUtil - SukebeiUtil - WikiUtil - TransUtil -
-SgpUtil ```py # A sample for DmmUtil import jvav util = jvav.DmmUtil()
-util.get_nice_avs_by_star_name('å°åç±è') util.get_score_by_id('cawd-441')
-util.get_all_top_stars() ``` ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1]
-[-av2 AV2] [-av3 AV3] [-sg SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-
-tg TG] [-pv1 PV1] [-pv2 PV2] [-tp] [-p PROXY] optional arguments: -h, --help
-show this help message and exit -v, --version Check version -av1 AV1 Followed
-by a code, search this code on JavBus -av2 AV2 Followed by a code, search this
-code on Sukebei -av3 AV3 Followed by a code, search this code on JavDb -sg SG
-Followed by a code, search the explainer video of this code -auth AUTH Followed
-by a authentication code for JavBus, get it from cookie key: bus_auth -nc
-Filter out high-definition subtitles magnet links -uc Filter out uncoded magnet
-links -sr SR Followed by an actress name, get a list of high-rated codes based
-on the actress name -srn SRN Followed by an actress name, get a list of the
-most recent codes based on the actress name -tg TG Followed by a keyword,
-search for codes based on the keyword -pv1 PV1 Followed by a code, get the
-corresponding preview video of the code on DMM -pv2 PV2 Follow a code, get the
-corresponding preview video of the code on Avgle -tp Get the top 25 ranking of
-DMM actresses -p PROXY, --proxy PROXY Followed by a proxy server address (by
+SgpUtil - RankUtil ```py # A sample for DmmUtil import jvav util = jvav.DmmUtil
+() util.get_nice_avs_by_star_name('å°åç±è') util.get_score_by_id('cawd-
+441') util.get_all_top_stars() ``` ## CMD ```shell usage: cmd.py [-h] [-v] [-
+av1 AV1] [-av2 AV2] [-av3 AV3] [-sg SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn
+SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2] [-tp] [-p PROXY] optional arguments: -h, --
+help show this help message and exit -v, --version Check version -av1 AV1
+Followed by a code, search this code on JavBus -av2 AV2 Followed by a code,
+search this code on Sukebei -av3 AV3 Followed by a code, search this code on
+JavDb -sg SG Followed by a code, search the explainer video of this code -auth
+AUTH Followed by a authentication code for JavBus, get it from cookie key:
+bus_auth -nc Filter out high-definition subtitles magnet links -uc Filter out
+uncoded magnet links -sr SR Followed by an actress name, get a list of high-
+rated codes based on the actress name -srn SRN Followed by an actress name, get
+a list of the most recent codes based on the actress name -tg TG Followed by a
+keyword, search for codes based on the keyword -pv1 PV1 Followed by a code, get
+the corresponding preview video of the code on DMM -pv2 PV2 Follow a code, get
+the corresponding preview video of the code on Avgle -tp Get the top 25 ranking
+of DMM actresses -p PROXY, --proxy PROXY Followed by a proxy server address (by
 default reads the value of the environment variable http_proxy) ``` ## DEV I
 use python-3.7.12 for development, please use python <= 3.7. And it is
 recommended to use python virtual environment to avoid some unnecessary
 problems. Here is my developing steps: ```shell git clone https://github.com/
 akynazh/jvav.git cd jvav ~/.pyenv/versions/3.7.12/bin/python -m venv venv
 source ./venv/bin/activate pip3 install -r requirements.txt ``` And then you
 can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~ ## TODO The
 following are some functions to be implemented, and I look forward to your
-contribution~ - [ ] fix SgpUtil(currently not work) - [x] cache the successful
-query results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x]
-support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) -
-[ ] support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh]
-(https://github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to
-JetBrains for their support to this project!
+contribution~ - [ ] fix SgpUtil(currently not work) - [ ] support RankUtil in
+CMD - [ ] fix JavLibUtil(currently not work because of cloudflare) - [x] cache
+the successful query results locally (Thanks: [@akynazh](https://github.com/
+akynazh)) - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/
+Steven-Fake)) - [ ] support db.msin.jp - [x] support JavDbUtil in cmd (Thanks:
+[@akynazh](https://github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)
+_l_o_g_o_._]Thanks to JetBrains for their support to this project!
```

### Comparing `Jvav-1.7.3/jvav/cmd.py` & `Jvav-1.8.0/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.7.3/jvav/utils.py` & `Jvav-1.8.0/jvav/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 import unicodedata
 import wikipediaapi
 from anti_useragent import UserAgent
 from bs4 import BeautifulSoup
 from deep_translator import GoogleTranslator
 
 
-# requests_cache.install_cache('jvav_cache')
-
 class BaseUtil:
-    def __init__(self, proxy_addr=""):
+    def __init__(self, proxy_addr="", use_cache=True):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
         """
 
         self.log = logging.getLogger(__name__)
         self.proxy_addr = ""
+        self.use_cache = use_cache
         if proxy_addr != "":
             self.proxy_addr = proxy_addr
         if self.proxy_addr != "":
             self.proxy_json = {"http": proxy_addr, "https": proxy_addr}
         else:
             self.proxy_json = {"http": "", "https": ""}
 
@@ -52,70 +51,59 @@
     def ua() -> str:
         """随机返回 UserAgent
 
         :return str: UserAgent
         """
         return UserAgent().random
 
+    def _inner_send_req(
+        self, url: str, session, headers={}, proxies={}, m=0, **args
+    ) -> typing.Tuple[int, requests.Response]:
+        if headers == {}:
+            headers = {"user-agent": self.ua()}
+        if proxies == {}:
+            proxies = self.proxy_json
+        try:
+            if m == 0:
+                resp = session.get(url, proxies=proxies, headers=headers, **args)
+            elif m == 1:
+                resp = session.post(url, proxies=proxies, headers=headers, **args)
+            elif m == 2:
+                resp = session.delete(url, proxies=proxies, headers=headers, **args)
+            elif m == 3:
+                resp = session.put(url, proxies=proxies, headers=headers, **args)
+            if resp.status_code != 200:
+                return 404, None
+            return 200, resp
+        except Exception as e:
+            self.log.error(f"BaseUtil: 访问 {url}: {e}")
+            return 502, None
+
     def send_req(
-            self, url: str, headers={}, proxies={}, m=0, **args
+        self, url: str, headers={}, proxies={}, m=0, **args
     ) -> typing.Tuple[int, requests.Response]:
         """发送请求
 
         :param str url: 地址
         :param dict headers: 请求头, 默认使用随机请求头
         :param dict proxies: 代理字典, 默认使用类初始化时指定的代理进行配置
         :param int m: 请求方法, 默认为 get(0), 其他为 post(1), delete(2), put(3)
         :param dict args: 其他 requests 参数
         :return tuple[int, requests.Response] 状态码和请求返回值
         关于状态码:
         200: 成功
         404: 未找到
         502: 网络问题
         """
-        if headers == {}:
-            headers = {"user-agent": self.ua()}
-        if proxies == {}:
-            proxies = self.proxy_json
-        with requests_cache.CachedSession(cache_name="jvav_cache") as session:
-            try:
-                if m == 0:
-                    resp = session.get(
-                        url,
-                        proxies=proxies,
-                        headers=headers,
-                        **args
-                    )
-                elif m == 1:
-                    resp = session.post(
-                        url,
-                        proxies=proxies,
-                        headers=headers,
-                        **args
-                    )
-                elif m == 2:
-                    resp = session.delete(
-                        url,
-                        proxies=proxies,
-                        headers=headers,
-                        **args
-                    )
-                elif m == 3:
-                    resp = session.put(
-                        url,
-                        proxies=proxies,
-                        headers=headers,
-                        **args
-                    )
-                if resp.status_code != 200:
-                    return 404, None
-                return 200, resp
-            except Exception as e:
-                self.log.error(f"BaseUtil: 访问 {url}: {e}")
-                return 502, None
+        if self.use_cache:
+            with requests_cache.CachedSession(cache_name="jvav_cache") as session:
+                return self._inner_send_req(url, session, headers, proxies, m, **args)
+        else:
+            with requests.Session() as session:
+                return self._inner_send_req(url, session, headers, proxies, m, **args)
 
     @staticmethod
     def get_soup(resp: requests.Response) -> BeautifulSoup:
         """从请求结果得到 soup
 
         :param requests.Response resp: 请求结果
         :return BeautifulSoup
@@ -124,71 +112,113 @@
 
     @staticmethod
     def write_html(resp: requests.Response):
         with open(f"./tmp.html", "w") as f:
             f.write(resp.text)
 
 
+class RankUtil(BaseUtil):
+    BASE_URL_AV_RANK = "https://gist.githubusercontent.com/jinjier/7a405fad753f996d85ed43073e3bf009/raw/29bf7a4635c1283a1415aad9fb335f92ece2972b/250.csv"
+    BASE_URL_STAR_RANK = ""  # DmmUtil supports
+
+    def random_get_av_from_rank(self) -> typing.Tuple[int, str]:
+        """从排行榜随机获取一个番号
+
+        :return tuple[int, str]: 状态码和番号
+        """
+        code, resp = self.send_req(self.BASE_URL_AV_RANK)
+        if code != 200:
+            return code, None
+        lines = str(resp.text).splitlines()
+        id = lines[random.randint(0, len(lines) - 1)].split(",")[1]
+        return 200, id
+
+    def get_av_250_rank(self) -> typing.Tuple[int, list]:
+        """获取 av 排行榜
+
+        :return tuple[int, list]: 状态码和番号列表
+        """
+        code, resp = self.send_req(self.BASE_URL_AV_RANK)
+        if code != 200:
+            return code, None
+        lines = str(resp.text).splitlines()
+        return 200, [line.split(",")[1] for line in lines]
+
+
 class JavDbUtil(BaseUtil):
     BASE_URL = "https://javdb.com"
+    BASE_URL_NEW_AV = BASE_URL + "/?vft=1&vst=1"
     BASE_URL_SEARCH = BASE_URL + "/search?q="
     BASE_URL_VIDEO = BASE_URL + "/v/"
     BASE_URL_ACTOR = BASE_URL + "/actors/"
     BASE_URL_SEARCH_STAR = BASE_URL + "/search?f=actor&q="
     BASE_PARAM_NICE_AVS_OF_STAR = "?sort_type=1"
     PAT_SCORE = re.compile(r"(\d+\.?\d+)分")
 
     def __init__(
-            self,
-            proxy_addr="",
-            max_home_page_count=100,
-            max_new_avs_count=8,
+        self,
+        proxy_addr="",
+        use_cache=True,
+        max_home_page_count=100,
+        max_new_avs_count=8,
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存, 默认为 True
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
         """
-        super().__init__(proxy_addr)
+        super().__init__(proxy_addr, use_cache)
         self.max_home_page_count = max_home_page_count
         self.max_new_avs_count = max_new_avs_count
 
     def get_max_page(self, url: str) -> typing.Tuple[int, int]:
         """获取最大页数
 
         :param str url: 页面地址
         :return tuple[int, int]: 状态码和最大页数
         """
         code, resp = self.send_req(url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
-            last_page = int(soup.find(class_="pagination-list").find_all("li")[-1].a.text)
+            last_page = int(
+                soup.find(class_="pagination-list").find_all("li")[-1].a.text
+            )
             if not last_page:
                 return 404, None
             return 200, last_page
         except Exception as e:
             self.log.error(f"JavDbUtil: 从 {url} 获取最大页数: {e}")
             return 404, None
 
+    def get_new_ids(self) -> typing.Tuple[int, list]:
+        """获取最新的番号列表
+
+        :return typing.Tuple[int, list]: 状态码和番号列表
+        """
+        return self.get_ids_from_page(self.BASE_URL_NEW_AV)
+
     def get_ids_from_page(self, url: str) -> typing.Tuple[int, list]:
         """从页面 url 获取番号列表
 
         :param str url: 首页/搜索页
         :return typing.Tuple[int, list]: 状态码和番号列表
         """
         code, resp = self.send_req(url=url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
-            ids = [item.find(class_="video-title").strong.text.strip() for item in items]
+            ids = [
+                item.find(class_="video-title").strong.text.strip() for item in items
+            ]
             if not ids:
                 return 404, None
             return 200, ids
         except Exception as e:
             self.log.error(f"JavDbUtil: 从页面获取番号列表: {e}")
             return 404, None
 
@@ -253,20 +283,22 @@
         code, url = self.get_star_page_by_star_name(star_name)
         if code != 200:
             return code, None
         try:
             code, ids = self.get_ids_from_page(url)
             if code != 200:
                 return code, None
-            return 200, ids[:self.max_new_avs_count]
+            return 200, ids[: self.max_new_avs_count]
         except Exception as e:
             self.log.error(f"JavDbUtil: 根据演员名字获取最新番号列表: {e}")
             return 404, None
 
-    def get_nice_avs_by_star_name(self, star_name: str, cookie: str) -> typing.Tuple[int, list]:
+    def get_nice_avs_by_star_name(
+        self, star_name: str, cookie: str
+    ) -> typing.Tuple[int, list]:
         """根据演员名字获取高分番号列表(需要登录)
 
         :param str star_name: 演员名字
         :param str cookie: 该方法需要登录，cookie 中的 _jdb_session 为必须值
         :return typing.Tuple[int, list]: 状态码和番号列表
         番号列表单个对象结构:
         {
@@ -274,30 +306,33 @@
             'id': id # 番号
         }
         """
         code, base_page_url = self.get_star_page_by_star_name(star_name)
         if code != 200:
             return code, None
         url = f"{base_page_url}{self.BASE_PARAM_NICE_AVS_OF_STAR}"
-        code, resp = self.send_req(url=url, headers={
-            'cookie': cookie,
-            'user-agent': self.ua_desktop()
-        })
+        code, resp = self.send_req(
+            url=url, headers={"cookie": cookie, "user-agent": self.ua_desktop()}
+        )
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             items = soup.find_all(class_="item")
             res = []
             for item in items:
                 try:
-                    res.append({
-                        "rate": self.PAT_SCORE.findall(item.find(class_="score").text)[0],
-                        "id": item.find(class_="video-title").strong.text.strip()
-                    })
+                    res.append(
+                        {
+                            "rate": self.PAT_SCORE.findall(
+                                item.find(class_="score").text
+                            )[0],
+                            "id": item.find(class_="video-title").strong.text.strip(),
+                        }
+                    )
                 except Exception:
                     pass
             if not res:
                 return 404, None
             return 200, res
         except Exception as e:
             self.log.error(f"JavDbUtil: 从页面获取番号列表: {e}")
@@ -478,20 +513,21 @@
                 return 404, None
             return 200, [t.attrs["href"] for t in img_tags]
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览图片: {e}")
             return 404, None
 
     def get_av_by_javdb_id(
-            self,
-            javdb_id: str,
-            is_nice: bool,
-            is_uncensored: bool,
-            sex_limit: bool = False,
-            magnet_max_count=10, ) -> typing.Tuple[int, dict]:
+        self,
+        javdb_id: str,
+        is_nice: bool,
+        is_uncensored: bool,
+        sex_limit: bool = False,
+        magnet_max_count=10,
+    ) -> typing.Tuple[int, dict]:
         """通过 JavDB ID 获取 av
 
         :param javdb_id: JavDB 内部 ID
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param bool sex_limit: 是否只获取女优信息
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -543,27 +579,31 @@
                 "producer": "",
                 "publisher": "",
                 "series": "",
                 "score": "",
                 "tags": [],
                 "stars": [],
                 "magnets": [],
-                "url": JavDbUtil.BASE_URL_VIDEO + javdb_id
+                "url": JavDbUtil.BASE_URL_VIDEO + javdb_id,
             }
             soup = self.get_soup(resp)
             # 获取元信息
             title_cn = soup.find("strong", {"class": "current-title"})
             title = soup.find("span", {"class": "origin-title"})
             if not title:
                 title, title_cn = title_cn, ""
             av["title_cn"] = title_cn.text.strip() if title_cn else ""
             av["title"] = title.text.strip() if title else ""
-            av["img"] = soup.find("div", {"class": "column column-video-cover"}).find("img")["src"]
+            av["img"] = soup.find("div", {"class": "column column-video-cover"}).find(
+                "img"
+            )["src"]
             # 由于nav栏会因为实际信息不同而导致行数不同，所以只能用循环的方式检索信息
-            metainfos = soup.find("nav", {"class": "panel movie-panel-info"}).find_all("div", {"class": "panel-block"})
+            metainfos = soup.find("nav", {"class": "panel movie-panel-info"}).find_all(
+                "div", {"class": "panel-block"}
+            )
             for info in metainfos:  # 遍历nav栏所有信息
                 text = unicodedata.normalize("NFKD", re.sub("[\n ]", "", info.text))
                 if re.search("番號:.+", text):
                     av["id"] = re.search("(番號: )(.+)", text).group(2).strip()
                 elif re.search("日期:.+", text):
                     av["date"] = re.search("(日期: )(.+)", text).group(2).strip()
                 elif re.search("\d+(分鍾)", text):
@@ -573,50 +613,78 @@
                 elif re.search("發行:.+", text):
                     av["publisher"] = re.search("(發行: )(.+)", text).group(2).strip()
                 elif re.search("系列:.+", text):
                     av["series"] = re.search("(系列: )(.+)", text).group(2).strip()
                 elif re.search("類別:.+", text):
                     av["tags"] = re.search("(類別: )(.+)", text).group(2).split(", ")
                 elif re.search("評分:.+", text):
-                    av["score"] = re.search("(評分: +)(\d+\.*\d*)(分.+)", text).group(2).strip()
+                    av["score"] = (
+                        re.search("(評分: +)(\d+\.*\d*)(分.+)", text).group(2).strip()
+                    )
                 elif re.search("演員:.+", text):
                     actor_info = info.find_all(("a", "strong"))[1:]
                     for a in range(len(actor_info) // 2):
-                        actor = {"name": actor_info[a * 2].text.strip(),
-                                 "id": actor_info[a * 2]["href"].split("/")[-1],
-                                 "sex": "女" if actor_info[a * 2 + 1].text.endswith("♀") else "男"}
-                        if not (sex_limit and actor['sex'] == '男'):
+                        actor = {
+                            "name": actor_info[a * 2].text.strip(),
+                            "id": actor_info[a * 2]["href"].split("/")[-1],
+                            "sex": (
+                                "女"
+                                if actor_info[a * 2 + 1].text.endswith("♀")
+                                else "男"
+                            ),
+                        }
+                        if not (sex_limit and actor["sex"] == "男"):
                             av["stars"].append(actor)
             # 获取磁链
-            magnet_list = soup.find_all("div", {"class": "item columns is-desktop"}) + \
-                          soup.find_all("div", {"class": "item columns is-desktop odd"})
+            magnet_list = soup.find_all(
+                "div", {"class": "item columns is-desktop"}
+            ) + soup.find_all("div", {"class": "item columns is-desktop odd"})
             for link in magnet_list:
-                magnet = {"link": link.find("a")["href"], "hd": "0", "zm": "0", "uc": "0", "size": "0"}
+                magnet = {
+                    "link": link.find("a")["href"],
+                    "hd": "0",
+                    "zm": "0",
+                    "uc": "0",
+                    "size": "0",
+                }
                 # 获取大小
                 size = link.find("span", {"class": "meta"})
                 if size:
-                    magnet["size"] = size.text.strip().split(',')[0]
+                    magnet["size"] = size.text.strip().split(",")[0]
                 # 检查是否为uc
                 title = link.find("span", {"class": "name"}).text
-                if any(k in title for k in
-                       ['-U', '无码', '無碼', '无码流出', '無碼流出', '无码破解', '無碼破解', 'uncensored',
-                        'Uncensored']):
+                if any(
+                    k in title
+                    for k in [
+                        "-U",
+                        "无码",
+                        "無碼",
+                        "无码流出",
+                        "無碼流出",
+                        "无码破解",
+                        "無碼破解",
+                        "uncensored",
+                        "Uncensored",
+                    ]
+                ):
                     magnet["uc"] = "1"
                 # 检查tag
                 tags_elements = link.find("div", {"class": "tags"})
                 if tags_elements:
                     tags_contents = tags_elements.findAll("span")
                     for i in tags_contents:
                         if i.text.strip() == "高清":
                             magnet["hd"] = "1"
                         elif i.text.strip() == "字幕":
                             magnet["zm"] = "1"
                 av["magnets"].append(magnet)
             if is_uncensored:
-                av["magnets"] = MagnetUtil.get_nice_magnets(av["magnets"], "uc", expect_val="1")
+                av["magnets"] = MagnetUtil.get_nice_magnets(
+                    av["magnets"], "uc", expect_val="1"
+                )
             if is_nice:
                 magnets = av["magnets"]
                 magnets = MagnetUtil.get_nice_magnets(
                     magnets, "hd", expect_val="1"
                 )  # 过滤高清
                 magnets = MagnetUtil.get_nice_magnets(
                     magnets, "zm", expect_val="1"
@@ -626,20 +694,20 @@
                 av["magnets"] = magnets
             return 200, av
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取av信息: {e}")
             return 404, None
 
     def get_av_by_id(
-            self,
-            id: str,
-            is_nice: bool,
-            is_uncensored: bool,
-            sex_limit: bool = False,
-            magnet_max_count=10,
+        self,
+        id: str,
+        is_nice: bool,
+        is_uncensored: bool,
+        sex_limit: bool = False,
+        magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 javdb 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -674,29 +742,32 @@
         {
             'name': '', # 演员名称
             'id': ''    # 演员编号
             'sex': ''   # 演员性别
         }
         """
         code, j_id = self.get_javdb_id_by_id(id)
-        return self.get_av_by_javdb_id(j_id, is_nice, is_uncensored, sex_limit,
-                                       magnet_max_count) if code == 200 else (code, None)
+        return (
+            self.get_av_by_javdb_id(
+                j_id, is_nice, is_uncensored, sex_limit, magnet_max_count
+            )
+            if code == 200
+            else (code, None)
+        )
 
 
 class JavLibUtil(BaseUtil):
     BASE_URL = "https://www.javlibrary.com"
     # nice
     BASE_URL_BEST_RATED_LAST_MONTH = BASE_URL + "/cn/vl_bestrated.php?mode=1&page="
     BASE_URL_BEST_RATED_ALL = BASE_URL + "/cn/vl_bestrated.php?mode=2&page="
-    BASE_URL_MOST_WANTED_LAST_MONTH = BASE_URL + \
-                                      "/cn/vl_mostwanted.php?&mode=1&page="
+    BASE_URL_MOST_WANTED_LAST_MONTH = BASE_URL + "/cn/vl_mostwanted.php?&mode=1&page="
     BASE_URL_MOST_WANTED_ALL = BASE_URL + "/cn/vl_mostwanted.php?&mode=2&page="
     # new
-    BASE_URL_NEW_RELEASE_HAVE_COMMENT = BASE_URL + \
-                                        "/cn/vl_newrelease.php?&mode=1&page="
+    BASE_URL_NEW_RELEASE_HAVE_COMMENT = BASE_URL + "/cn/vl_newrelease.php?&mode=1&page="
     BASE_URL_NEW_RELEASE_ALL = BASE_URL + "/cn/vl_newrelease.php?&mode=2&page="
     BASE_URL_NEW_ENTRIES = BASE_URL + "/cn/vl_newentries.php?page="
     URLS_NICE = [
         BASE_URL_BEST_RATED_LAST_MONTH,
         BASE_URL_BEST_RATED_ALL,
         BASE_URL_MOST_WANTED_LAST_MONTH,
         BASE_URL_MOST_WANTED_ALL,
@@ -712,27 +783,31 @@
     BASE_URL_COMMENT = BASE_URL + "/cn/videocomments.php?v="
     # review 最佳评论
     BASE_URL_REVIEW = BASE_URL + "/cn/videoreviews.php?v="
     # 排行榜最大页数
     MAX_RANK_PAGE = 25
 
     def get_random_ids_from_rank_by_page(
-            self, page: int, list_type: int
+        self, page: int, list_type: int
     ) -> typing.Tuple[int, str]:
         """从排行榜某页中获取该页番号列表
 
         :param int page: 第几页
         :param int list_type: 排行榜类型 0 nice | 1 new
         :return typing.Tuple[int, list]: 状态码和番号列表
         """
         if list_type == 0:
             url = random.choice(JavLibUtil.URLS_NICE)
         elif list_type == 1:
             url = random.choice(JavLibUtil.URLS_NEW)
-        code, resp = self.send_req(url=url + str(page))
+        headers = {
+            "cookie": "over18=18;",
+            "user-agent": self.ua_desktop(),
+        }
+        code, resp = self.send_req(url=url + str(page), headers=headers)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             tag_ids = soup.find_all(class_="id")
             ids = [tag.text for tag in tag_ids]
             if len(ids) > 0:
@@ -770,21 +845,21 @@
             return code, None
         javlib_av_id = ""
         if resp.url == url:
             try:
                 soup = self.get_soup(resp)
                 videos = soup.find_all(class_="video")
                 video_href = videos[0].a["href"]
-                javlib_av_id = video_href[video_href.find("v=") + 2:]
+                javlib_av_id = video_href[video_href.find("v=") + 2 :]
             except Exception as e:
                 self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
                 return 404, None
         else:
             r_url = resp.url
-            javlib_av_id = r_url[r_url.find("v=") + 2:]
+            javlib_av_id = r_url[r_url.find("v=") + 2 :]
         comment_url = JavLibUtil.BASE_URL_REVIEW + javlib_av_id
         code, resp = self.send_req(url=comment_url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             comment_tags = soup.find_all(class_="t")
@@ -798,17 +873,19 @@
             self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
             return 404, None
 
 
 class DmmUtil(BaseUtil):
     BASE_URL = "https://www.dmm.co.jp"
     BASE_URL_SEARCH_AV = BASE_URL + "/digital/-/list/search/=/sort=ranking/?searchstr="
-    BASE_URL_SEARCH_AV_MONTHLY = BASE_URL + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
+    BASE_URL_SEARCH_AV_MONTHLY = (
+        BASE_URL + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
+    )
     BASE_URL_SEARCH_STAR = (
-            BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
+        BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
     )
     BASE_URL_TOP_STARS = BASE_URL + "/digital/videoa/-/ranking/=/type=actress"
     PAT_CID = re.compile(r"/cid=.+/")
     PAT_CID_REAL = re.compile(r"[A-Za-z]+0+[0-9]+")
     PAT_AV = re.compile(r"[a-z]+\d+")
 
     def get_pv_by_id(self, id: str) -> typing.Tuple[int, str]:
@@ -853,15 +930,15 @@
             return code, None
         try:
             soup = self.get_soup(resp)
             tmb_tags = soup.find_all(class_="tmb")
             cids = []
             for tmb in tmb_tags:
                 try:
-                    lk = tmb.a['href']
+                    lk = tmb.a["href"]
                     cid = self.get_cid_from_link(lk)
                     if cid:
                         cids.append(cid)
                 except Exception:
                     pass
             return 200, cids
         except Exception as e:
@@ -878,15 +955,15 @@
             return code, None
         try:
             soup = self.get_soup(resp)
             li_tags = soup.find(id="list").find_all("li")
             cids = []
             for li in li_tags:
                 try:
-                    lk = li.div.a['href']
+                    lk = li.div.a["href"]
                     cid = self.get_cid_from_link(lk)
                     if cid:
                         cids.append(cid)
                 except Exception:
                     pass
             return 200, cids
         except Exception as e:
@@ -1039,59 +1116,62 @@
     BASE_URL_SEARCH_BY_STAR_ID = f"{BASE_URL}/star"
     BASE_URL_SEARCH_STAR = f"{BASE_URL}/searchstar"
     BASE_URL_MAGNET = f"{BASE_URL}/ajax/uncledatoolsbyajax.php?lang=zh"
     BASE_URL_GENRE = f"{BASE_URL}/genre"
 
     def get_headers(self):
         return {
-            'authority': 'www.javbus.com',
-            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
-            'accept-language': 'zh-CN,zh;q=0.9,en;q=0.8,en-US;q=0.7,fr-FR;q=0.6,fr;q=0.5',
-            'cookie': f'bus_auth={self.bus_auth};',
-            'dnt': '1',
-            'sec-ch-ua-platform': '"Windows"',
-            'user-agent': self.ua_desktop()
+            "authority": "www.javbus.com",
+            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-US;q=0.7,fr-FR;q=0.6,fr;q=0.5",
+            "cookie": f"bus_auth={self.bus_auth};",
+            "dnt": "1",
+            "sec-ch-ua-platform": '"Windows"',
+            "user-agent": self.ua_desktop(),
         }
 
     def __init__(
-            self,
-            bus_auth: str,
-            proxy_addr="",
-            max_home_page_count=100,
-            max_new_avs_count=8,
+        self,
+        bus_auth: str,
+        proxy_addr="",
+        use_cache=True,
+        max_home_page_count=100,
+        max_new_avs_count=8,
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
+        :param bool use_cache: 是否使用缓存
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
         :param str bus_auth: cookie 需要用到的值
         """
-        super().__init__(proxy_addr)
+        super().__init__(proxy_addr, use_cache)
         self.max_home_page_count = max_home_page_count
         self.max_new_avs_count = max_new_avs_count
         self.bus_auth = bus_auth
 
     def get_all_genres(self) -> typing.Tuple[int, list]:
         """获取所有类别
 
         :return typing.Tuple[int, list]: 状态码和类别列表
         """
-        code, resp = self.send_req(url=JavBusUtil.BASE_URL_GENRE, headers=self.get_headers())
+        code, resp = self.send_req(
+            url=JavBusUtil.BASE_URL_GENRE, headers=self.get_headers()
+        )
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             boxes = soup.find_all(class_="row genre-box")
             genres = []
             for box in boxes:
                 tags = box.find_all("a")
                 for tag in tags:
-                    genres.append(
-                        {tag.text: tag["href"][tag["href"].rfind("/") + 1:]})
+                    genres.append({tag.text: tag["href"][tag["href"].rfind("/") + 1 :]})
             if genres == []:
                 return 404, None
             return 200, genres
         except Exception as e:
             self.log.error(f"JavBusUtil: 获取所有标签失败: {e}")
             return 404, None
 
@@ -1155,22 +1235,23 @@
             return code, None
         try:
             ids = []
             soup = self.get_soup(resp)
             tags = soup.find_all(class_="movie-box")
             for tag in tags:
                 id_link = tag["href"]
-                id = id_link[id_link.rfind("/") + 1:]
+                id = id_link[id_link.rfind("/") + 1 :]
                 ids.append(id)
             if ids == []:
                 return 404, None
             return 200, ids
         except Exception as e:
             self.log.error(
-                f"JavBusUtil: 从 av 列表页面 {base_page_url} 获取该页面全部番号: {e}")
+                f"JavBusUtil: 从 av 列表页面 {base_page_url} 获取该页面全部番号: {e}"
+            )
             return 404, None
 
     def get_id_from_page(self, base_page_url: str, page=-1) -> typing.Tuple[int, str]:
         """从 av 列表页面获取一个番号
 
         :param str base_page: 基础页地址, 也是第一页地址
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
@@ -1208,16 +1289,18 @@
     def get_ids_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, list]:
         """根据演员名称获取一批番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, list]: 状态码和番号
         """
-        return self.get_ids_from_page(base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_NAME}/{star_name}",
-                                      page=page)
+        return self.get_ids_from_page(
+            base_page_url=f"{JavBusUtil.BASE_URL_SEARCH_BY_STAR_NAME}/{star_name}",
+            page=page,
+        )
 
     def get_new_ids_by_star_name(self, star_name: str) -> typing.Tuple[int, list]:
         """根据演员名字获取最新番号列表
 
         :param str star_name: 演员名称
         :return typing.Tuple[int, list]: 状态码和番号列表
         """
@@ -1288,34 +1371,37 @@
         dict 格式:
         {
             "star_id": star_id,
             "star_name": star_name
         }
         """
         code, resp = self.send_req(
-            url=f"{JavBusUtil.BASE_URL_SEARCH_STAR}/{star_name}", headers=self.get_headers())
+            url=f"{JavBusUtil.BASE_URL_SEARCH_STAR}/{star_name}",
+            headers=self.get_headers(),
+        )
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             star = soup.find(class_="avatar-box text-center")
             star_id = star["href"].split("star/")[1]
             res_star_name = star.find("img")["title"]
             return 200, {"star_id": star_id, "star_name": res_star_name}
         except Exception as e:
             self.log.error(
-                f"JavBusUtil: 根据演员名称 {star_name} 确认该演员在 javbus 是否存在: {e}")
+                f"JavBusUtil: 根据演员名称 {star_name} 确认该演员在 javbus 是否存在: {e}"
+            )
             return 404, None
 
     def get_av_by_id(
-            self,
-            id: str,
-            is_nice: bool,
-            is_uncensored: bool,
-            magnet_max_count=10,
+        self,
+        id: str,
+        is_nice: bool,
+        is_uncensored: bool,
+        magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 javbus 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -1384,15 +1470,15 @@
                 elif p.text.find("發行日期:") != -1:
                     av["date"] = "".join(
                         p.text.replace("發行日期:", "").replace('"', "").split()
                     )
                 # 获取标签
                 elif p.text.find("類別:") != -1:
                     tags = paras[i + 1].find_all("a")
-                    av["tags"] = [''.join(tag.text.split()) for tag in tags]
+                    av["tags"] = ["".join(tag.text.split()) for tag in tags]
                 # 获取演员
                 elif i == len(paras) - 1:
                     tags = p.find_all("a")
                     for tag in tags:
                         star = {"name": "", "id": ""}
                         star["name"] = "".join(tag.text.split())
                         star["id"] = tag["href"].split("star/")[1]
@@ -1433,18 +1519,18 @@
                 magnet = {"link": "", "hd": "0", "zm": "0", "uc": "0"}
                 tds = tr.find_all("td")
                 for i, td in enumerate(tds):
                     if i == 0:
                         magnet["link"] = td.a["href"]
                         magnet_title = td.a.text.strip().lower()
                         if (
-                                "uncensor" in magnet_title
-                                or "無修正" in magnet_title
-                                or "无修正" in magnet_title
-                                or "无码" in magnet_title
+                            "uncensor" in magnet_title
+                            or "無修正" in magnet_title
+                            or "无修正" in magnet_title
+                            or "无码" in magnet_title
                         ):
                             magnet["uc"] = "1"
                         links = td.find_all("a")
                         for link in links:
                             text = link.text.strip()
                             if text == "高清":
                                 magnet["hd"] = "1"
@@ -1565,38 +1651,36 @@
 
         :param list magnets: 磁链列表
         :return list: 排列好的磁链列表
         """
         # 统一单位为 MB
         for magnet in magnets:
             magnet["size_no_unit"] = -1
-            size = magnet["size"].lower().replace(
-                "gib", "gb").replace("mib", "mb")
+            size = magnet["size"].lower().replace("gib", "gb").replace("mib", "mb")
             gb_idx = size.find("gb")
             mb_idx = size.find("mb")
             if gb_idx != -1:  # 单位为 GB
                 magnet["size_no_unit"] = float(size[:gb_idx]) * 1024
             elif mb_idx != -1:  # 单位为 MB
                 magnet["size_no_unit"] = float(size[:mb_idx])
         # magnets = list(filter(lambda m: m["size_no_unit"] != -1, magnets))
         # 根据 size_no_unit 大小排序
-        magnets = sorted(
-            magnets, key=lambda m: m["size_no_unit"], reverse=True)
+        magnets = sorted(magnets, key=lambda m: m["size_no_unit"], reverse=True)
         return magnets
 
 
 class SukebeiUtil(BaseUtil):
     BASE_URL = "https://sukebei.nyaa.si"
 
     def get_av_by_id(
-            self,
-            id: str,
-            is_nice: bool,
-            is_uncensored: bool,
-            magnet_max_count=10,
+        self,
+        id: str,
+        is_nice: bool,
+        is_uncensored: bool,
+        magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 sukebei 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -1659,18 +1743,18 @@
                     "zm": "0",  # 是否有字幕 0 否 | 1 是
                     "uc": "0",  # 是否未经审查 0 否 | 1 是
                 }
                 for j, td in enumerate(tds):
                     if j == 1:  # 获取标题
                         title = td.a.text
                         if (
-                                "uncensor" in title
-                                or "無修正" in title
-                                or "无修正" in title
-                                or "无码" in title
+                            "uncensor" in title
+                            or "無修正" in title
+                            or "无修正" in title
+                            or "无码" in title
                         ):
                             magnet["uc"] = "1"
                         if i == 0:
                             av["title"] = title
                     if j == 2:  # 获取磁链
                         magnet["link"] = td.find_all("a")[-1]["href"]
                     if j == 3:  # 获取大小
@@ -1778,16 +1862,15 @@
         {
             'title': '', # 标题
             'url': '', # 地址
             'lang': '' # 语言码
         }
         """
         try:
-            wiki = wikipediaapi.Wikipedia(
-                language=from_lang, proxies=self.proxy_json)
+            wiki = wikipediaapi.Wikipedia(language=from_lang, proxies=self.proxy_json)
             page = wiki.page(title=topic)
             # links = page.links
             # for k in links.keys():
             #     if links[k].title.find(topic) != -1:
             #         print(links[k].fullurl)
             if page.text:
                 langlinks = page.langlinks
@@ -1835,19 +1918,17 @@
         dd_list = nex.find_all("dd")
         rank_list = []
         for dd in dd_list:
             try:
                 img = dd.find("img")["src"]
                 url = dd.find("h5").a["href"]
                 title = dd.find("h5").a.text
-                rank_list.append({
-                    "img": img,
-                    "url": f"{SjsUtil.BASE_URL}/{url}",
-                    "title": title
-                })
+                rank_list.append(
+                    {"img": img, "url": f"{SjsUtil.BASE_URL}/{url}", "title": title}
+                )
             except Exception:
                 pass
         return rank_list
 
     def get_rank_by_nex_for_cosimg(self, nex) -> list:
         """根据标签元素 nex 获取司机社排行榜 (cosimg)
 
@@ -1856,19 +1937,17 @@
         dd_list = nex.find_all("dd")
         rank_list = []
         for dd in dd_list:
             try:
                 img = dd.find("img")["src"]
                 url = dd.find("a")["href"]
                 title = dd.find("h5").text
-                rank_list.append({
-                    "img": img,
-                    "url": f"{SjsUtil.BASE_URL}/{url}",
-                    "title": title
-                })
+                rank_list.append(
+                    {"img": img, "url": f"{SjsUtil.BASE_URL}/{url}", "title": title}
+                )
             except Exception:
                 pass
         return rank_list
 
     def get_rank(self, rank_type=1) -> typing.Tuple[int, list]:
         """获取司机社排行榜
 
@@ -1919,45 +1998,55 @@
 class SgpUtil(BaseUtil):
     BASE_URL = "http://www.fpie2.com"
     BASE_URL_SEARCH = "https://api.cbbee0.com/v1_2/articleSearch"
     BASE_URL_DETAIL = f"{BASE_URL}/play-details/1/"
 
     def get_video_by_av_id(self, av_id: str) -> typing.Tuple[int, str]:
         headers = {
-            'authority': 'api.cbbee0.com',
-            'accept': 'application/json, text/plain, */*',
-            'accept-language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6,zh-TW;q=0.5',
-            'content-type': 'application/json;charset=UTF-8',
-            'origin': SgpUtil.BASE_URL,
-            'referer': SgpUtil.BASE_URL + '/',
-            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Microsoft Edge";v="114"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"macOS"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'cross-site',
-            'user-agent': self.ua(),
+            "authority": "api.cbbee0.com",
+            "accept": "application/json, text/plain, */*",
+            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6,zh-TW;q=0.5",
+            "content-type": "application/json;charset=UTF-8",
+            "origin": SgpUtil.BASE_URL,
+            "referer": SgpUtil.BASE_URL + "/",
+            "sec-ch-ua": '"Not.A/Brand";v="8", "Chromium";v="114", "Microsoft Edge";v="114"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"macOS"',
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "cross-site",
+            "user-agent": self.ua(),
         }
-        data = '{"conditions": "' + av_id + '", "field": 0, "target": 1, "sort": 1, "userToken": "", "hm": "008-api", "device_id": ""}'
+        data = (
+            '{"conditions": "'
+            + av_id
+            + '", "field": 0, "target": 1, "sort": 1, "userToken": "", "hm": "008-api", "device_id": ""}'
+        )
 
-        code, resp = self.send_req(url=SgpUtil.BASE_URL_SEARCH, headers=headers, m=1, data=data)
+        code, resp = self.send_req(
+            url=SgpUtil.BASE_URL_SEARCH, headers=headers, m=1, data=data
+        )
         if code != 200:
             return code, None
         res = resp.json()
-        code, resp = self.send_req(url=SgpUtil.BASE_URL_DETAIL, headers=headers, json={
-            "encrypt_key": res["encrypt_key"],
-            "encrypt_data": res["encrypt_data"]
-        })
+        code, resp = self.send_req(
+            url=SgpUtil.BASE_URL_DETAIL,
+            headers=headers,
+            json={
+                "encrypt_key": res["encrypt_key"],
+                "encrypt_data": res["encrypt_data"],
+            },
+        )
         if code != 200:
             return code, None
         soup = self.get_soup(resp)
         try:
             suffix = soup.find("iframe")["src"]
-            video_addr = f'{SgpUtil.BASE_URL}{suffix}'
-            video_content = soup.find('div', {'class': 'content'})
+            video_addr = f"{SgpUtil.BASE_URL}{suffix}"
+            video_content = soup.find("div", {"class": "content"})
             res = f"""解说视频地址: {video_addr}
             
             解说内容:
             
             {video_content}
             
             解说视频地址: {video_addr}"""
```

### Comparing `Jvav-1.7.3/setup.py` & `Jvav-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.7.3",
+    version="1.8.0",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

