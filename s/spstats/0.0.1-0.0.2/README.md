# Comparing `tmp/spstats-0.0.1-py3-none-any.whl.zip` & `tmp/spstats-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2941 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2843 b- defN 24-Apr-13 13:18 myfunc/function.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 13:21 spstats-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-13 13:21 spstats-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 13:21 spstats-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 13:21 spstats-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 13:21 spstats-0.0.1.dist-info/RECORD
-6 files, 4731 bytes uncompressed, 2109 bytes compressed:  55.4%
+Zip file size: 2905 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2776 b- defN 24-Apr-13 12:25 myfunc/function.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/RECORD
+6 files, 4664 bytes uncompressed, 2073 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myfunc/function.py
 Comment: 
 
-Filename: spstats-0.0.1.dist-info/LICENSE
+Filename: spstats-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: spstats-0.0.1.dist-info/METADATA
+Filename: spstats-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: spstats-0.0.1.dist-info/WHEEL
+Filename: spstats-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: spstats-0.0.1.dist-info/top_level.txt
+Filename: spstats-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spstats-0.0.1.dist-info/RECORD
+Filename: spstats-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myfunc/function.py

```diff
@@ -1,8 +1,7 @@
-from __future__ import barry_as_FLUFL
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy import stats
 
 def random_array(size):
     """Generate a random NumPy array of given size."""
@@ -94,10 +93,7 @@
     slope, intercept, r_value, p_value, std_err = stats.linregress(x, y)
     return slope, intercept, r_value, p_value, std_err
 
 def resample_bootstrap(data, n_samples):
     """Perform bootstrap resampling on a dataset."""
     boot_samples = [np.random.choice(data, len(data), replace=True) for _ in range(n_samples)]
     return boot_samples
-
-def add(a, b):
-  return a+b
```

## Comparing `spstats-0.0.1.dist-info/LICENSE` & `spstats-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

