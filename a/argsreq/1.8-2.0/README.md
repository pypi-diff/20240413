# Comparing `tmp/argsreq-1.8.tar.gz` & `tmp/argsreq-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsreq-1.8.tar", last modified: Sat Apr 13 13:35:58 2024, max compression
+gzip compressed data, was "argsreq-2.0.tar", last modified: Sat Apr 13 16:28:16 2024, max compression
```

## Comparing `argsreq-1.8.tar` & `argsreq-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.231321 argsreq-1.8/
--rw-rw-rw-   0        0        0      311 2024-04-13 13:35:58.230311 argsreq-1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.227340 argsreq-1.8/argsreq.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 13:35:58.000000 argsreq-1.8/argsreq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 13:35:58.229309 argsreq-1.8/reqargs/
--rw-rw-rw-   0        0        0    15014 2024-04-13 13:34:04.000000 argsreq-1.8/reqargs/__init__.py
--rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.8/reqargs/__main__.py
--rw-rw-rw-   0        0        0    14609 2024-04-13 13:34:11.000000 argsreq-1.8/reqargs/colorls.py
--rw-rw-rw-   0        0        0    15014 2024-04-13 13:34:16.000000 argsreq-1.8/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-13 13:35:58.231321 argsreq-1.8/setup.cfg
--rw-rw-rw-   0        0        0      641 2024-04-13 13:35:52.000000 argsreq-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 16:28:16.322468 argsreq-2.0/
+-rw-rw-rw-   0        0        0      311 2024-04-13 16:28:16.322468 argsreq-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 16:28:16.314336 argsreq-2.0/argsreq.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-13 16:28:16.000000 argsreq-2.0/argsreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-13 16:28:16.000000 argsreq-2.0/argsreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 16:28:16.000000 argsreq-2.0/argsreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 16:28:16.000000 argsreq-2.0/argsreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 16:28:16.320445 argsreq-2.0/reqargs/
+-rw-rw-rw-   0        0        0    14963 2024-04-13 16:25:07.000000 argsreq-2.0/reqargs/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-2.0/reqargs/__main__.py
+-rw-rw-rw-   0        0        0    14559 2024-04-13 16:27:27.000000 argsreq-2.0/reqargs/colorls.py
+-rw-rw-rw-   0        0        0    14963 2024-04-13 16:27:31.000000 argsreq-2.0/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 16:28:16.323450 argsreq-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      641 2024-04-13 16:28:08.000000 argsreq-2.0/setup.py
```

### Comparing `argsreq-1.8/reqargs/__init__.py` & `argsreq-2.0/reqargs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import requests
 import subprocess
 import os
 import tempfile
-import numpy as np
-import matplotlib.pyplot as plt
+
 #!/usr/bin/python3
 # -*- coding: utf-8 - *-
 
 # Copyright (c) 2020 Romeet Chhabra
 
 # Permission is hereby granted, free of charge, to any person obtatomlng a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `argsreq-1.8/reqargs/colorls.py` & `argsreq-2.0/reqargs/colorls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import requests
 import subprocess
 import os
 import tempfile
-import numpy as np
-import matplotlib.pyplot as plt
+
 #!/usr/bin/python3
 # -*- coding: utf-8 - *-
 
 # Copyright (c) 2020 Romeet Chhabra
 
 # Permission is hereby granted, free of charge, to any person obtatomlng a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `argsreq-1.8/reqargs/reqargs.py` & `argsreq-2.0/reqargs/reqargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import requests
 import subprocess
 import os
 import tempfile
-import numpy as np
-import matplotlib.pyplot as plt
+
 #!/usr/bin/python3
 # -*- coding: utf-8 - *-
 
 # Copyright (c) 2020 Romeet Chhabra
 
 # Permission is hereby granted, free of charge, to any person obtatomlng a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `argsreq-1.8/setup.py` & `argsreq-2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.8'
+VERSION = '2.0'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="argsreq",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
```

