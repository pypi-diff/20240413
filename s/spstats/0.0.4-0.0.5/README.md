# Comparing `tmp/spstats-0.0.4-py3-none-any.whl.zip` & `tmp/spstats-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3336 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3986 b- defN 24-Apr-13 14:05 myfunc/function.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 14:05 spstats-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-13 14:05 spstats-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 14:05 spstats-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 14:05 spstats-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 14:05 spstats-0.0.4.dist-info/RECORD
-6 files, 5874 bytes uncompressed, 2504 bytes compressed:  57.4%
+Zip file size: 3354 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4034 b- defN 24-Apr-13 14:20 myfunc/function.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 14:24 spstats-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      278 b- defN 24-Apr-13 14:24 spstats-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 14:24 spstats-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-13 14:24 spstats-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      459 b- defN 24-Apr-13 14:24 spstats-0.0.5.dist-info/RECORD
+6 files, 5936 bytes uncompressed, 2522 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myfunc/function.py
 Comment: 
 
-Filename: spstats-0.0.4.dist-info/LICENSE
+Filename: spstats-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: spstats-0.0.4.dist-info/METADATA
+Filename: spstats-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: spstats-0.0.4.dist-info/WHEEL
+Filename: spstats-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: spstats-0.0.4.dist-info/top_level.txt
+Filename: spstats-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: spstats-0.0.4.dist-info/RECORD
+Filename: spstats-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myfunc/function.py

```diff
@@ -35,48 +35,48 @@
     """데이터의 왜도를 계산합니다."""
     return skew(data)
 
 def kurtosis(data):
     """데이터의 첨도를 계산합니다."""
     return kurtosis(data)
     
-def hist(data, xlabel, ylabel, title):
+def hist(data, xlabel="", ylabel="", title=""):
     """
     NumPy 배열 또는 Pandas Series의 히스토그램을 플로팅합니다.
     데이터의 길이를 기반으로 bin의 수를 결정합니다.
     """
     plt.hist(data, bins=int(1 + np.log2(len(data))))
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     plt.show()
 
-def pie(data, labels, title):
+def pie(data, labels, title=""):
     """파이 차트를 생성합니다."""
     plt.pie(data, labels=labels, autopct='%1.1f%%')
     plt.title(title)
     plt.show()
 
-def line_plot(x, y, xlabel, ylabel, title):
+def line_plot(x, y, xlabel="", ylabel="", title=""):
     """두 데이터 집합의 선 그래프를 생성합니다."""
     plt.plot(x, y)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     plt.show()
 
-def scatter_plot(x, y, xlabel, ylabel, title):
+def scatter_plot(x, y, xlabel="", ylabel="", title=""):
     """두 데이터 집합의 산점도를 생성합니다."""
     plt.scatter(x, y)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     plt.show()
 
-def bar(categories, values, xlabel, ylabel, title):
+def bar(categories, values, xlabel="", ylabel="", title=""):
     """막대 그래프를 생성합니다."""
     plt.bar(categories, values)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     plt.show()
     
@@ -91,15 +91,15 @@
     """두 데이터 집합 사이의 피어슨 상관 계수를 계산합니다."""
     return np.corrcoef(data1, data2)[0, 1]
 
 def standardize(data):
     """데이터 집합의 값을 표준화합니다."""
     return (data - np.mean(data)) / np.std(data)
 
-def box_plot(data, xlabel, ylabel, title):
+def box_plot(data, xlabel="", ylabel="", title=""):
     """데이터 집합의 상자 그림을 생성합니다."""
     plt.boxplot(data)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     plt.show()
```

## Comparing `spstats-0.0.4.dist-info/LICENSE` & `spstats-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

