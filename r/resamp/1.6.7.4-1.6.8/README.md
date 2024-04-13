# Comparing `tmp/resamp-1.6.7.4.tar.gz` & `tmp/resamp-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.7.4.tar", last modified: Wed Apr 10 06:55:39 2024, max compression
+gzip compressed data, was "resamp-1.6.8.tar", last modified: Sat Apr 13 21:26:53 2024, max compression
```

## Comparing `resamp-1.6.7.4.tar` & `resamp-1.6.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:55:39.685889 resamp-1.6.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 06:55:33.000000 resamp-1.6.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:55:39.685889 resamp-1.6.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-10 06:55:33.000000 resamp-1.6.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:55:39.685889 resamp-1.6.7.4/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-10 06:55:33.000000 resamp-1.6.7.4/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-04-10 06:55:33.000000 resamp-1.6.7.4/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:55:39.685889 resamp-1.6.7.4/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-10 06:55:39.000000 resamp-1.6.7.4/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 06:55:39.000000 resamp-1.6.7.4/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:55:39.000000 resamp-1.6.7.4/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 06:55:39.000000 resamp-1.6.7.4/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 06:55:39.000000 resamp-1.6.7.4/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:55:39.685889 resamp-1.6.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-10 06:55:33.000000 resamp-1.6.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 21:26:43.000000 resamp-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-13 21:26:53.852687 resamp-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-13 21:26:43.000000 resamp-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-13 21:26:43.000000 resamp-1.6.8/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34332 2024-04-13 21:26:43.000000 resamp-1.6.8/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:26:53.852687 resamp-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-13 21:26:43.000000 resamp-1.6.8/setup.py
```

### Comparing `resamp-1.6.7.4/LICENSE` & `resamp-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.7.4/PKG-INFO` & `resamp-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.7.4
-Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
+Version: 1.6.8
+Summary: A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,15 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.6.4 Documentation
+`resamp.py` Version 1.6.8 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
```

### Comparing `resamp-1.6.7.4/README.md` & `resamp-1.6.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.6.4 Documentation
+`resamp.py` Version 1.6.8 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
```

### Comparing `resamp-1.6.7.4/resamp/__init__.py` & `resamp-1.6.8/resamp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     calculate_probabilities_for_each_treatment,
     plot_relative_risk_distribution,
     calculate_p_value,
     plot_null_distribution,
     permute_correlation,
     compute_correlation_ci,
     resample_one_group_count,
+    confidence_interval_count,
+    CI_percentile_to_pivotal,
     cal_ci_one_sample,
     bootstrap_confidence_interval,
     plot_bootstrap_lines,
     calculate_statistic,
     power_analysis,
 )
 
@@ -56,13 +58,15 @@
     "calculate_probabilities_for_each_treatment",
     "plot_relative_risk_distribution",
     "calculate_p_value",
     "plot_null_distribution",
     "permute_correlation",
     "compute_correlation_ci",
     "resample_one_group_count",
+    "confidence_interval_count",
+    "CI_percentile_to_pivotal",
     "cal_ci_one_sample",
     "bootstrap_confidence_interval",
     "plot_bootstrap_lines",
     "calculate_statistic",
     "power_analysis",
 ]
```

### Comparing `resamp-1.6.7.4/resamp/resamp.py` & `resamp-1.6.8/resamp/resamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # LS 40 resampling library to complement/combine with Hypothesize
 
 ### ACTIVE FINAL SCRIPT
 
-## VERSION - 1.6.4
-## STATUS: ALL MODIFICATION ACTIVE AND LIVE IN PYPI (PIP INSTALL STATISTICS_LIBRARY)
-## DATE: 9 APRIL 2024 
+## VERSION - 1.6.8
+## DATE: 10 APRIL 2024 
 ## AUTHOR: VISHANTH HARI RAJ
 ## SUPERVISOR: JANE SHEVTSOV
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import chi2
@@ -75,15 +74,15 @@
     if observed.shape != expected.shape:
         raise ValueError("Dimensions of observed and expected data do not match")
 
 def calculate_chi_squared(observed, expected):
     chi_squared = ((observed - expected) ** 2 / expected).sum().sum()
     return chi_squared
 
-# #Calculating the expected Value 
+#Calculating the expected Value 
 def calculate_expected(observed):
     row_sums = observed.sum(axis=1)
     col_sums = observed.sum(axis=0)
     total = observed.sum().sum()
     expected = np.outer(row_sums, col_sums) / total
     return expected
 
@@ -450,14 +449,15 @@
         if two_tailed:
             p_value = (np.sum(sims <= corr_obs) + np.sum(sims >= -corr_obs)) / len(sims)
         else:
             # For one-tailed, we assume a negative relationship.
             p_value = np.sum(sims <= corr_obs) / len(sims)
     return p_value
 
+
 def plot_null_distribution(sims, corr_obs, two_tailed=False):
     """
     Plot the null distribution of simulated correlation coefficients and the observed correlation.
     
     Parameters:
     - sims (np.array): Simulated correlation coefficients.
     - corr_obs (float): Observed correlation coefficient.
@@ -470,14 +470,15 @@
         if two_tailed:
             plt.axvline(-corr_obs, color='red', label=f'Negative Observed Correlation: {-corr_obs:.3f}')
         plt.legend(loc='upper right')
         plt.show()
     except Exception as e:
         print(f"Error plotting null distribution: {e}")
 
+
 def permute_correlation(x, y, num_simulations=10000):
     """
     Generate simulated correlation coefficients by permuting one variable and calculating Pearson's correlation.
     
     Parameters:
     - x (np.array): Values of variable 1.
     - y (np.array): Values of variable 2.
@@ -494,14 +495,15 @@
             permuted_x = np.random.permutation(x)
             simulated_correlations[i] = pearsonr(permuted_x, y)[0]
         return simulated_correlations
     except Exception as e:
         print(f"Error generating simulated correlations: {e}")
         return np.array([])  # Return an empty array in case of error
 
+
 def compute_correlation_ci(x, y, num_simulations=10000, confidence_interval=0.95):
     """
     Compute the confidence interval around the observed correlation by resampling the dataset
     and plotting the distribution of correlation coefficients from the resampled datasets with error handling.
     
     Parameters:
     - x (np.array): Values of variable 1.
@@ -565,15 +567,15 @@
     """
 
     dataArr = np.array(box)  #Converts box model to NumPy array
 
     #Resampling loop
     resampleArr = np.zeros(sims)  #Preallocates array to store resampling results
     for i in range(sims):
-        p_sample = np.random.choice(box, sample_size, replace=True)  #Samples from the box model (with replacement)
+        p_sample = np.random.choice(dataArr, sample_size, replace=True)  #Samples from the box model (with replacement)
         p_count = np.sum(p_sample == count_what)
         resampleArr[i] = p_count
     
     #Compute p-value
     if proportion == False:
         observed = np.sum(dataArr == count_what)
     else:
@@ -583,14 +585,69 @@
     #Return results
     if return_resamples:
         return p, resampleArr
     else:
         return p
 
 
+def confidence_interval_count(box, sample_size, confidence_level=99, count_what="A", sims=10000, pivotal=True, proportion=False, return_resamples=False):
+    """
+    Calculate percentile confidence interval for a count or proportion.
+    
+    Parameters:
+        box (np array or list): Box model representing population
+        sample_size (int): Number of individuals (or sites, etc.) in sample
+        confidence_level (float): The level of confidence interval you want (95%, 99%, etc.) This needs to be a number between 0 and 100.
+        count_what (char): What character in the box model should be counted. Default "A".
+        sims (int): How many simulations to run. Default 10,000
+        pivotal (bool): Whether to compute a pivotal confidence interval (default True). If False, percentile will be used.
+        proportion (bool): Calculate count or proportion (default count)
+        return_resamples (bool): Whether to return resampling results used to generate p-value. Primarily for pedagogical purposes.
+    
+    Returns:
+        confidence interval (as numpy array)
+        resampling data (if desired)
+    """
+    
+    dataArr = np.array(box)  #Converts box model to NumPy array
+    
+    if pivotal==True and proportion==False:  #Percentile CIs don't use Mobs
+        Mobs = np.sum(dataArr==count_what)
+    elif pivotal==True and proportion==True:
+        Mobs = np.mean(dataArr==count_what)
+
+    #Resampling loop
+    resampleArr = np.zeros(sims)
+    for i in range(sims):
+        p_sample = np.random.choice(dataArr, sample_size, replace=True)  #Samples from the box model (with replacement)
+        p_count = np.sum(p_sample == count_what)
+        resampleArr[i] = p_count
+   
+    #Convert to proportions if desired
+    if proportion:
+        resampleArr = resampleArr/sample_size
+    
+    #Compute confidence interval
+    CIpercentile = np.percentile(resampleArr, sorted([(100-confidence_level)/2, 100-(100-confidence_level)/2]))
+    if pivotal:
+        CIpivotal = np.array([2*Mobs-CIpercentile[1], 2*Mobs-CIpercentile[0]])
+        CI = CIpivotal
+    else:
+        CI = CIpercentile
+      
+    #Return results
+    if return_resamples:
+        return CI, resampleArr
+    else:
+        return CI
+
+
+def CI_percentile_to_pivotal(Mobs, CIpercentile):
+    return np.array([2*Mobs-CIpercentile[1], 2*Mobs-CIpercentile[0]])
+
 
 # Additional this function also do the same job : def calculate_confidence_interval(simulated_rr, percentile=95):
 def cal_ci_one_sample(data, confidence_level=99):
     """
     Calculate a custom confidence interval for a 1-D array based on the specified confidence level.
     
     Parameters:
```

### Comparing `resamp-1.6.7.4/resamp.egg-info/PKG-INFO` & `resamp-1.6.8/resamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.7.4
-Summary: A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.
+Version: 1.6.8
+Summary: A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,15 @@
 
 RESAMP Library Documentation
 
 - Author: Vishanth Hari Raj
 - GitHub Repository: https://github.com/vishanth10/resamp
 
 
-`resamp.py` Version 1.6.4 Documentation
+`resamp.py` Version 1.6.8 Documentation
 Overview
 `resamp.py` is a comprehensive Python library designed for statistical analysis and resampling techniques. This document serves as a guide for utilizing the library's functions, including statistical tests, data analysis, and visualization tools.
 Installation
 To install `resamp.py`, run the following command in your terminal:
 ```bash
 pip install statistics_library
 ```
```

### Comparing `resamp-1.6.7.4/setup.py` & `resamp-1.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.7.4',
+    version='1.6.8',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
-    description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
+    description='A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
     install_requires=[
         'numpy>=1.18.5',
         'pandas>=1.0.5',
```

