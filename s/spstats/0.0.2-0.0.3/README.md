# Comparing `tmp/spstats-0.0.2-py3-none-any.whl.zip` & `tmp/spstats-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2905 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2776 b- defN 24-Apr-13 12:25 myfunc/function.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 12:31 spstats-0.0.2.dist-info/RECORD
-6 files, 4664 bytes uncompressed, 2073 bytes compressed:  55.6%
+Zip file size: 3251 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3658 b- defN 24-Apr-13 13:48 myfunc/function.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 13:48 spstats-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-13 13:48 spstats-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 13:48 spstats-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 13:48 spstats-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 13:48 spstats-0.0.3.dist-info/RECORD
+6 files, 5546 bytes uncompressed, 2419 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myfunc/function.py
 Comment: 
 
-Filename: spstats-0.0.2.dist-info/LICENSE
+Filename: spstats-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: spstats-0.0.2.dist-info/METADATA
+Filename: spstats-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: spstats-0.0.2.dist-info/WHEEL
+Filename: spstats-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: spstats-0.0.2.dist-info/top_level.txt
+Filename: spstats-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: spstats-0.0.2.dist-info/RECORD
+Filename: spstats-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myfunc/function.py

```diff
@@ -1,99 +1,112 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy import stats
 
-def random_array(size):
-    """Generate a random NumPy array of given size."""
+def randomarr(size):
+    """지정된 크기의 랜덤한 NumPy 배열을 생성합니다."""
     return np.random.rand(size)
 
 def mean(data):
-    """Calculate the mean of a NumPy array or Pandas Series."""
+    """NumPy 배열 또는 Pandas Series의 평균을 계산합니다."""
     return np.mean(data)
 
 def mode(data):
-    """Calculate the mode of a NumPy array or Pandas Series."""
+    """NumPy 배열 또는 Pandas Series의 최빈값을 계산합니다."""
     return stats.mode(data)[0][0]
 
-def median(data):
-    """Calculate the median of a NumPy array or Pandas Series."""
+def med(data):
+    """NumPy 배열 또는 Pandas Series의 중앙값을 계산합니다."""
     return np.median(data)
 
-def std_deviation(data):
-    """Calculate the standard deviation of a NumPy array or Pandas Series."""
+def std(data):
+    """NumPy 배열 또는 Pandas Series의 표준편차를 계산합니다."""
     return np.std(data)
 
-def variance(data):
-    """Calculate the variance of a NumPy array or Pandas Series."""
+def var(data):
+    """NumPy 배열 또는 Pandas Series의 분산을 계산합니다."""
     return np.var(data)
 
-def histogram(data):
+def hist(data, xlabel, ylabel, title):
     """
-    Plot a histogram of a NumPy array or Pandas Series.
-    Determine the bins based on the length of the data.
+    NumPy 배열 또는 Pandas Series의 히스토그램을 플로팅합니다.
+    데이터의 길이를 기반으로 bin의 수를 결정합니다.
     """
     plt.hist(data, bins=int(1 + np.log2(len(data))))
-    plt.xlabel('Value')
-    plt.ylabel('Frequency')
-    plt.title('Histogram')
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title(title)
     plt.show()
 
-def pie(data, labels):
-    """Create a pie chart."""
+def pie(data, labels, title):
+    """파이 차트를 생성합니다."""
     plt.pie(data, labels=labels, autopct='%1.1f%%')
-    plt.title('Pie Chart')
+    plt.title(title)
     plt.show()
 
-def line_plot(x, y):
-    """Create a line plot of two sets of data."""
+def line_plot(x, y, xlabel, ylabel, title):
+    """두 데이터 집합의 선 그래프를 생성합니다."""
     plt.plot(x, y)
-    plt.xlabel('X')
-    plt.ylabel('Y')
-    plt.title('Line Plot')
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title(title)
     plt.show()
 
-def scatter_plot(x, y):
-    """Create a scatter plot of two sets of data."""
+def scatter_plot(x, y, xlabel, ylabel, title):
+    """두 데이터 집합의 산점도를 생성합니다."""
     plt.scatter(x, y)
-    plt.xlabel('X')
-    plt.ylabel('Y')
-    plt.title('Scatter Plot')
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title(title)
     plt.show()
 
-def bar(categories, values):
-    """Create a bar chart."""
+def bar(categories, values, xlabel, ylabel, title):
+    """막대 그래프를 생성합니다."""
     plt.bar(categories, values)
-    plt.xlabel('Categories')
-    plt.ylabel('Values')
-    plt.title('Bar Chart')
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title(title)
     plt.show()
 
 def t_test(data1, data2):
-    """Perform a t-test for two samples using scipy.stats."""
+    """scipy.stats를 사용하여 두 샘플에 대한 t-test을 수행합니다."""
     return stats.ttest_ind(data1, data2)
 
 def correlation(data1, data2):
-    """Calculate the Pearson correlation coefficient between two datasets."""
+    """두 데이터 집합 사이의 피어슨 상관 계수를 계산합니다."""
     return np.corrcoef(data1, data2)[0, 1]
 
 def standardize(data):
-    """Standardize the values of a dataset."""
+    """데이터 집합의 값을 표준화합니다."""
     return (data - np.mean(data)) / np.std(data)
 
-def boxplot(data):
-    """Create a box plot of a dataset."""
+def box_plot(data, xlabel, ylabel, title):
+    """데이터 집합의 상자 그림을 생성합니다."""
     plt.boxplot(data)
-    plt.xlabel('Data')
-    plt.ylabel('Value')
-    plt.title('Box Plot')
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.title(title)
     plt.show()
 
 def linear_regression(x, y):
-    """Perform linear regression on two sets of data."""
+    """두 데이터 집합에 대한 선형 회귀를 수행합니다."""
     slope, intercept, r_value, p_value, std_err = stats.linregress(x, y)
     return slope, intercept, r_value, p_value, std_err
 
-def resample_bootstrap(data, n_samples):
-    """Perform bootstrap resampling on a dataset."""
+def bootstrap_resample(data, n_samples):
+    """데이터 집합에 대한 부트스트랩 재표본을 생성합니다."""
     boot_samples = [np.random.choice(data, len(data), replace=True) for _ in range(n_samples)]
     return boot_samples
+
+def probability_distribution(rv, size=1000):
+    """주어진 무작위 변수를 기반으로 확률분포표를 작성합니다."""
+    samples = rv.rvs(size=size)
+    df = pd.DataFrame(samples, columns=['Value'])
+    value_counts = df['Value'].value_counts(normalize=True).reset_index()
+    value_counts.columns = ['Value', 'Probability']
+    value_counts = value_counts.sort_values(by='Value').reset_index(drop=True)
+    return value_counts
+
+def describe(data):
+    """NumPy 배열 또는 Pandas의 describe"""
+    return pd.DataFrame(data).describe()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `spstats-0.0.2.dist-info/LICENSE` & `spstats-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

