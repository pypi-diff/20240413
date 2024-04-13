# Comparing `tmp/PyPyNum-1.7.0.tar.gz` & `tmp/PyPyNum-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPyNum-1.7.0.tar", last modified: Tue Mar 19 12:55:50 2024, max compression
+gzip compressed data, was "PyPyNum-1.8.0.tar", last modified: Fri Apr 12 14:50:36 2024, max compression
```

## Comparing `PyPyNum-1.7.0.tar` & `PyPyNum-1.8.0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:55:50.468750 PyPyNum-1.7.0/
--rw-rw-rw-   0        0        0    84411 2024-03-19 12:55:50.468750 PyPyNum-1.7.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 12:55:49.899750 PyPyNum-1.7.0/PyPyNum.egg-info/
--rw-rw-rw-   0        0        0    84411 2024-03-19 12:55:49.000000 PyPyNum-1.7.0/PyPyNum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-03-19 12:55:49.000000 PyPyNum-1.7.0/PyPyNum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:55:49.000000 PyPyNum-1.7.0/PyPyNum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-19 12:55:49.000000 PyPyNum-1.7.0/PyPyNum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 12:55:50.458750 PyPyNum-1.7.0/pypynum/
--rw-rw-rw-   0        0        0     6632 2024-03-15 05:10:12.000000 PyPyNum-1.7.0/pypynum/Array.py
--rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.7.0/pypynum/FourierT.py
--rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.7.0/pypynum/Geometry.py
--rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.7.0/pypynum/Group.py
--rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.7.0/pypynum/Logic.py
--rw-rw-rw-   0        0        0    11024 2024-03-15 05:10:12.000000 PyPyNum-1.7.0/pypynum/Matrix.py
--rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.7.0/pypynum/NeuralN.py
--rw-rw-rw-   0        0        0     8007 2024-01-25 08:45:23.000000 PyPyNum-1.7.0/pypynum/Quaternion.py
--rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.7.0/pypynum/Symbolics.py
--rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.7.0/pypynum/Tensor.py
--rw-rw-rw-   0        0        0     2816 2024-03-06 10:08:03.000000 PyPyNum-1.7.0/pypynum/Tree.py
--rw-rw-rw-   0        0        0     3552 2024-03-15 05:10:12.000000 PyPyNum-1.7.0/pypynum/Vector.py
--rw-rw-rw-   0        0        0     1782 2024-03-13 11:36:14.000000 PyPyNum-1.7.0/pypynum/__init__.py
--rw-rw-rw-   0        0        0     5860 2024-01-22 12:57:34.000000 PyPyNum-1.7.0/pypynum/__temporary.py
--rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.7.0/pypynum/chars.py
--rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.7.0/pypynum/cipher.py
--rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.7.0/pypynum/constants.py
--rw-rw-rw-   0        0        0      744 2024-01-22 13:17:32.000000 PyPyNum-1.7.0/pypynum/equations.py
--rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.7.0/pypynum/errors.py
--rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.7.0/pypynum/file.py
--rw-rw-rw-   0        0        0    24753 2024-03-18 05:35:43.000000 PyPyNum-1.7.0/pypynum/maths.py
--rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.7.0/pypynum/numbers.py
--rw-rw-rw-   0        0        0     8326 2024-02-01 12:22:16.000000 PyPyNum-1.7.0/pypynum/plotting.py
--rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.7.0/pypynum/probability.py
--rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.7.0/pypynum/random.py
--rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.7.0/pypynum/regression.py
--rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.7.0/pypynum/sequence.py
--rw-rw-rw-   0        0        0     8428 2024-01-24 05:43:19.000000 PyPyNum-1.7.0/pypynum/test.py
--rw-rw-rw-   0        0        0     2129 2024-02-27 12:58:01.000000 PyPyNum-1.7.0/pypynum/this.py
--rw-rw-rw-   0        0        0     9823 2024-03-19 11:31:45.000000 PyPyNum-1.7.0/pypynum/tools.py
--rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.7.0/pypynum/types.py
--rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.7.0/pypynum/utils.py
--rw-rw-rw-   0        0        0       42 2024-03-19 12:55:50.468750 PyPyNum-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0    35853 2024-03-19 12:54:41.000000 PyPyNum-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:50:36.375800 PyPyNum-1.8.0/
+-rw-rw-rw-   0        0        0    85418 2024-04-12 14:50:36.374800 PyPyNum-1.8.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 14:50:35.904800 PyPyNum-1.8.0/PyPyNum.egg-info/
+-rw-rw-rw-   0        0        0    85418 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 14:50:35.000000 PyPyNum-1.8.0/PyPyNum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 14:50:36.355800 PyPyNum-1.8.0/pypynum/
+-rw-rw-rw-   0        0        0     6632 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Array.py
+-rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.0/pypynum/FourierT.py
+-rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.0/pypynum/Geometry.py
+-rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.0/pypynum/Graph.py
+-rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.0/pypynum/Group.py
+-rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.0/pypynum/Logic.py
+-rw-rw-rw-   0        0        0    11024 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Matrix.py
+-rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.0/pypynum/NeuralN.py
+-rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.0/pypynum/PyPyNum.png
+-rw-rw-rw-   0        0        0     8007 2024-01-25 08:45:23.000000 PyPyNum-1.8.0/pypynum/Quaternion.py
+-rw-rw-rw-   0        0        0    43971 2024-04-12 12:58:03.000000 PyPyNum-1.8.0/pypynum/README.md
+-rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.0/pypynum/Symbolics.py
+-rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Tensor.py
+-rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.0/pypynum/Tree.py
+-rw-rw-rw-   0        0        0     3552 2024-03-15 05:10:12.000000 PyPyNum-1.8.0/pypynum/Vector.py
+-rw-rw-rw-   0        0        0     1831 2024-04-12 12:05:55.000000 PyPyNum-1.8.0/pypynum/__init__.py
+-rw-rw-rw-   0        0        0     5860 2024-01-22 12:57:34.000000 PyPyNum-1.8.0/pypynum/__temporary.py
+-rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.0/pypynum/chars.py
+-rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.0/pypynum/cipher.py
+-rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.0/pypynum/constants.py
+-rw-rw-rw-   0        0        0      744 2024-01-22 13:17:32.000000 PyPyNum-1.8.0/pypynum/equations.py
+-rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.0/pypynum/errors.py
+-rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.0/pypynum/file.py
+-rw-rw-rw-   0        0        0    26518 2024-03-28 08:22:55.000000 PyPyNum-1.8.0/pypynum/maths.py
+-rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.0/pypynum/numbers.py
+-rw-rw-rw-   0        0        0     8326 2024-02-01 12:22:16.000000 PyPyNum-1.8.0/pypynum/plotting.py
+-rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.0/pypynum/polynomial.py
+-rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.0/pypynum/probability.py
+-rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.0/pypynum/random.py
+-rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.0/pypynum/regression.py
+-rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.0/pypynum/sequence.py
+-rw-rw-rw-   0        0        0     8428 2024-01-24 05:43:19.000000 PyPyNum-1.8.0/pypynum/test.py
+-rw-rw-rw-   0        0        0     2129 2024-02-27 12:58:01.000000 PyPyNum-1.8.0/pypynum/this.py
+-rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.0/pypynum/tools.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.0/pypynum/types.py
+-rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.0/pypynum/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:50:36.377800 PyPyNum-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0    36764 2024-04-12 14:50:12.000000 PyPyNum-1.8.0/setup.py
```

### Comparing `PyPyNum-1.7.0/PKG-INFO` & `PyPyNum-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.7.0
+Version: 1.8.0
 Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
 Home-page: https://www.gitee.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -664,14 +664,15 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <http://www.gnu.org/licenses/>.
         
+Keywords: math,数学,mathematics,数学计算,numerical,数值,computation,计算,scientific,科学,algebra,代数,calculus,微积分,statistics,统计,linear-algebra,线性代数,optimization,优化,numerical-analysis,数值分析,matrix,矩阵,vector,向量,tensor,张量,numerics,数值计算,library,库,tools,工具,utils,实用程序,algorithms,算法,software,软件,package,包,methods,方法,data-science,数据科学,machine-learning,机器学习,computational,计算的,operations,操作,functions,函数,processing,处理,programming,编程,simulation,仿真,visualization,可视化,physics,物理
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 ﻿# <font color = blue>PyPyNum</font>
 
 <font color = gree>A multifunctional mathematical calculation package written in pure Python programming language
 </font><font color = red>[Python>=3.5]</font>
@@ -687,15 +688,15 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.7.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
@@ -736,98 +737,98 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增代码行数：
-约八百行
+新增代码行数为603行
 
-New code lines:
-approximately 800 lines
+Add 603 new lines of code
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-部分函数再次优化，性能提高一倍。
+新增函数“magic_square”的功能简介：可
+以生成任意大于等于三的整数阶幻方。
 
-Partial functions were optimized
-again, resulting in a doubling
-of performance.
+Introduction to the newly added
+function "magic square": It can
+generate any integer order magic
+square greater than or equal to
+three.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增的好玩功能举例。
+新增模块“Graph”的功能简介：具有有向图
+、无向图、带权有向图、带权无向图这四个对
+象，支持添加或删除顶点和边，以及深度优先
+搜索与广度优先搜索这两种图的遍历方式，还
+有计算最短路径等功能。
+
+Introduction to the functions of
+the newly added module "Graph":
+it has four objects: directed
+graph, undirected graph,
+weighted directed graph, and
+weighted undirected graph. It
+supports adding or removing
+vertices and edges, as well as
+depth first search and breadth
+first search for graph
+traversal. It also has functions
+such as calculating the shortest
+path.
 
-Examples of newly added fun
-features.
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增的有序集合包含绝大多数内置集合的运算
-，并且另有几个新函数。请注意它不是从内置
-集合继承的。
-
-The newly added ordered set
-contains the majority of
-built-in set operations, and
-there are also several new
-functions. Please note that it
-does not inherit from the
-built-in set.
-
-新增的无穷迭代器支持迭代多种数列，默认的
-空字符串即为自增数列。目前支持的数列有等
-差数列、等比数列、斐波那契数列与卡特兰数
-列。
-
-The newly added infinite
-iterator supports iterating
-multiple sequences, and the
-default empty string is the self
-increasing sequence. The
-currently supported sequences
-include arithmetic sequences,
-proportional sequences,
-Fibonacci sequences, and Catalan
-sequences.
+新增模块“polynomial”的功能简介：有一
+个多项式对象，可以通过传入包含“(次数,
+系数)”的二元组组成的序列创建多项式对象
+，可以随时设置某一项的数值，并且支持多
+项式形式的四则运算，还有取商式、取余式
+、求幂、求模幂的功能。
+
+Introduction to the newly added
+module "polynomial": There is a
+polynomial object that can be
+created by passing in a sequence
+of binary tuples containing
+"degree, coefficient". The value
+of a certain term can be set at
+any time, and it supports
+polynomial form arithmetic
+operations. It also has
+functions such as quotient,
+remainder, exponentiation, and
+modular exponentiation.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
 <<<以下结构中的省略号表示原有的部分>>>
 
 <<<The ellipsis in the following structure represents the original part>>>
 
 PyPyNum
-    ★ Tree [Various trees]
+    ★ Graph [Graph theory]
         CLASSES
-            MultiTree
-            MultiTreeNode
-    ★ maths [Mathematical functions]
-        FUNCTIONS
-            ...
-            totient(n: int) -> int
-            mod_order(a: int, n: int, b: int) -> int
-            primitive_root(a: int, single: bool = False) -> Union[int, list]
-            normalize(data: arr, target: num = 1) -> arr
-            average(data, weights, expected=False)
-            exgcd(a: int, b: int) -> tuple
-            crt(n: arr, a: arr) -> int
-    ★ sequence [Various sequences]
+            BaseGraph
+                BaseWeGraph
+                    WeDiGraph
+                    WeUnGraph
+                DiGraph
+                UnGraph
+    ★ polynomial [Polynomial object]
+        CLASSES
+            Polynomial
         FUNCTIONS
-            farey(n: int) -> list
-            ...
+            poly(terms=None)
     ★ tools [Other useful tools]
         FUNCTIONS
             ...
-            primality(n: int, iter_num: int = 10) -> bool
-            generate_primes(limit: int) -> list
-            prime_factors(integer: int, dictionary: bool = False, pollard_rho: bool = True) -> Union[list, dict]
-    ★ utils [Other useful tools]
-        CLASSES
-            InfIterator
-            OrderedSet
+            magic_square(n)
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -889,14 +890,22 @@
             Line
             Point
             Polygon
             Quadrilateral
             Triangle
         FUNCTIONS
             distance(g1, g2, error: int | float = 0) -> float
+    ★ Graph [Graph theory]
+        CLASSES
+            BaseGraph
+                BaseWeGraph
+                    WeDiGraph
+                    WeUnGraph
+                DiGraph
+                UnGraph
     ★ Group [Group theory]
         CLASSES
             Group
         FUNCTIONS
             add(x, y)
             divide(x, y)
             group(data)
@@ -1134,14 +1143,19 @@
         FUNCTIONS
             color(text: str, rgb: arr) -> str
             change(data: thing) -> thing
             background(right: real = 5, left: real = -5, top: real = 5, bottom: real = -5...
             unary(function, right: real = 5, left: real = -5, top: real = 5, bottom: real = -5, complexity: real = 5...
             binary(function, right: real = 5, left: real = -5, top: real = 5, bottom: real = -5, complexity: real = 5...
             c_unary(function, start: real, end: real, interval: real = 5, projection: str = "ri", right: real = 5...
+    ★ polynomial [Polynomial object]
+        CLASSES
+            Polynomial
+        FUNCTIONS
+            poly(terms=None)
     ★ probability [Probability function]
         FUNCTIONS
             binomial(sample_size: int, successes: int, success_probability: Union[int, float]) -> float
             hypergeometric(total_items: int, success_items: int, sample_size: int, successes_in_sample: int) -> float
     ★ random [Generate random numbers or random arrays]
         FUNCTIONS
             choice(seq: Union[list, tuple, str], shape: Union[list, tuple] = None)
@@ -1172,14 +1186,15 @@
             deduplicate(iterable: ite) -> ite
             classify(array: arr) -> dict
             split(iterable: ite, key: arr, retain: bool = False) -> list
             interpolation(data: arr, length: int) -> list
             primality(n: int, iter_num: int = 10) -> bool
             generate_primes(limit: int) -> list
             prime_factors(integer: int, dictionary: bool = False, pollard_rho: bool = True) -> Union[list, dict]
+            magic_square(n)
     ★ utils [Other useful tools]
         CLASSES
             InfIterator
             OrderedSet
 ```
 
 ### 代码测试
```

### Comparing `PyPyNum-1.7.0/PyPyNum.egg-info/PKG-INFO` & `PyPyNum-1.8.0/PyPyNum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.7.0
+Version: 1.8.0
 Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
 Home-page: https://www.gitee.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -664,14 +664,15 @@
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <http://www.gnu.org/licenses/>.
         
+Keywords: math,数学,mathematics,数学计算,numerical,数值,computation,计算,scientific,科学,algebra,代数,calculus,微积分,statistics,统计,linear-algebra,线性代数,optimization,优化,numerical-analysis,数值分析,matrix,矩阵,vector,向量,tensor,张量,numerics,数值计算,library,库,tools,工具,utils,实用程序,algorithms,算法,software,软件,package,包,methods,方法,data-science,数据科学,machine-learning,机器学习,computational,计算的,operations,操作,functions,函数,processing,处理,programming,编程,simulation,仿真,visualization,可视化,physics,物理
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 ﻿# <font color = blue>PyPyNum</font>
 
 <font color = gree>A multifunctional mathematical calculation package written in pure Python programming language
 </font><font color = red>[Python>=3.5]</font>
@@ -687,15 +688,15 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.7.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.0 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
@@ -736,98 +737,98 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增代码行数：
-约八百行
+新增代码行数为603行
 
-New code lines:
-approximately 800 lines
+Add 603 new lines of code
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-部分函数再次优化，性能提高一倍。
+新增函数“magic_square”的功能简介：可
+以生成任意大于等于三的整数阶幻方。
 
-Partial functions were optimized
-again, resulting in a doubling
-of performance.
+Introduction to the newly added
+function "magic square": It can
+generate any integer order magic
+square greater than or equal to
+three.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增的好玩功能举例。
+新增模块“Graph”的功能简介：具有有向图
+、无向图、带权有向图、带权无向图这四个对
+象，支持添加或删除顶点和边，以及深度优先
+搜索与广度优先搜索这两种图的遍历方式，还
+有计算最短路径等功能。
+
+Introduction to the functions of
+the newly added module "Graph":
+it has four objects: directed
+graph, undirected graph,
+weighted directed graph, and
+weighted undirected graph. It
+supports adding or removing
+vertices and edges, as well as
+depth first search and breadth
+first search for graph
+traversal. It also has functions
+such as calculating the shortest
+path.
 
-Examples of newly added fun
-features.
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-新增的有序集合包含绝大多数内置集合的运算
-，并且另有几个新函数。请注意它不是从内置
-集合继承的。
-
-The newly added ordered set
-contains the majority of
-built-in set operations, and
-there are also several new
-functions. Please note that it
-does not inherit from the
-built-in set.
-
-新增的无穷迭代器支持迭代多种数列，默认的
-空字符串即为自增数列。目前支持的数列有等
-差数列、等比数列、斐波那契数列与卡特兰数
-列。
-
-The newly added infinite
-iterator supports iterating
-multiple sequences, and the
-default empty string is the self
-increasing sequence. The
-currently supported sequences
-include arithmetic sequences,
-proportional sequences,
-Fibonacci sequences, and Catalan
-sequences.
+新增模块“polynomial”的功能简介：有一
+个多项式对象，可以通过传入包含“(次数,
+系数)”的二元组组成的序列创建多项式对象
+，可以随时设置某一项的数值，并且支持多
+项式形式的四则运算，还有取商式、取余式
+、求幂、求模幂的功能。
+
+Introduction to the newly added
+module "polynomial": There is a
+polynomial object that can be
+created by passing in a sequence
+of binary tuples containing
+"degree, coefficient". The value
+of a certain term can be set at
+any time, and it supports
+polynomial form arithmetic
+operations. It also has
+functions such as quotient,
+remainder, exponentiation, and
+modular exponentiation.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
 <<<以下结构中的省略号表示原有的部分>>>
 
 <<<The ellipsis in the following structure represents the original part>>>
 
 PyPyNum
-    ★ Tree [Various trees]
+    ★ Graph [Graph theory]
         CLASSES
-            MultiTree
-            MultiTreeNode
-    ★ maths [Mathematical functions]
-        FUNCTIONS
-            ...
-            totient(n: int) -> int
-            mod_order(a: int, n: int, b: int) -> int
-            primitive_root(a: int, single: bool = False) -> Union[int, list]
-            normalize(data: arr, target: num = 1) -> arr
-            average(data, weights, expected=False)
-            exgcd(a: int, b: int) -> tuple
-            crt(n: arr, a: arr) -> int
-    ★ sequence [Various sequences]
+            BaseGraph
+                BaseWeGraph
+                    WeDiGraph
+                    WeUnGraph
+                DiGraph
+                UnGraph
+    ★ polynomial [Polynomial object]
+        CLASSES
+            Polynomial
         FUNCTIONS
-            farey(n: int) -> list
-            ...
+            poly(terms=None)
     ★ tools [Other useful tools]
         FUNCTIONS
             ...
-            primality(n: int, iter_num: int = 10) -> bool
-            generate_primes(limit: int) -> list
-            prime_factors(integer: int, dictionary: bool = False, pollard_rho: bool = True) -> Union[list, dict]
-    ★ utils [Other useful tools]
-        CLASSES
-            InfIterator
-            OrderedSet
+            magic_square(n)
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -889,14 +890,22 @@
             Line
             Point
             Polygon
             Quadrilateral
             Triangle
         FUNCTIONS
             distance(g1, g2, error: int | float = 0) -> float
+    ★ Graph [Graph theory]
+        CLASSES
+            BaseGraph
+                BaseWeGraph
+                    WeDiGraph
+                    WeUnGraph
+                DiGraph
+                UnGraph
     ★ Group [Group theory]
         CLASSES
             Group
         FUNCTIONS
             add(x, y)
             divide(x, y)
             group(data)
@@ -1134,14 +1143,19 @@
         FUNCTIONS
             color(text: str, rgb: arr) -> str
             change(data: thing) -> thing
             background(right: real = 5, left: real = -5, top: real = 5, bottom: real = -5...
             unary(function, right: real = 5, left: real = -5, top: real = 5, bottom: real = -5, complexity: real = 5...
             binary(function, right: real = 5, left: real = -5, top: real = 5, bottom: real = -5, complexity: real = 5...
             c_unary(function, start: real, end: real, interval: real = 5, projection: str = "ri", right: real = 5...
+    ★ polynomial [Polynomial object]
+        CLASSES
+            Polynomial
+        FUNCTIONS
+            poly(terms=None)
     ★ probability [Probability function]
         FUNCTIONS
             binomial(sample_size: int, successes: int, success_probability: Union[int, float]) -> float
             hypergeometric(total_items: int, success_items: int, sample_size: int, successes_in_sample: int) -> float
     ★ random [Generate random numbers or random arrays]
         FUNCTIONS
             choice(seq: Union[list, tuple, str], shape: Union[list, tuple] = None)
@@ -1172,14 +1186,15 @@
             deduplicate(iterable: ite) -> ite
             classify(array: arr) -> dict
             split(iterable: ite, key: arr, retain: bool = False) -> list
             interpolation(data: arr, length: int) -> list
             primality(n: int, iter_num: int = 10) -> bool
             generate_primes(limit: int) -> list
             prime_factors(integer: int, dictionary: bool = False, pollard_rho: bool = True) -> Union[list, dict]
+            magic_square(n)
     ★ utils [Other useful tools]
         CLASSES
             InfIterator
             OrderedSet
 ```
 
 ### 代码测试
```

### Comparing `PyPyNum-1.7.0/PyPyNum.egg-info/SOURCES.txt` & `PyPyNum-1.8.0/PyPyNum.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 PyPyNum.egg-info/PKG-INFO
 PyPyNum.egg-info/SOURCES.txt
 PyPyNum.egg-info/dependency_links.txt
 PyPyNum.egg-info/top_level.txt
 pypynum/Array.py
 pypynum/FourierT.py
 pypynum/Geometry.py
+pypynum/Graph.py
 pypynum/Group.py
 pypynum/Logic.py
 pypynum/Matrix.py
 pypynum/NeuralN.py
+pypynum/PyPyNum.png
 pypynum/Quaternion.py
+pypynum/README.md
 pypynum/Symbolics.py
 pypynum/Tensor.py
 pypynum/Tree.py
 pypynum/Vector.py
 pypynum/__init__.py
 pypynum/__temporary.py
 pypynum/chars.py
@@ -22,14 +25,15 @@
 pypynum/constants.py
 pypynum/equations.py
 pypynum/errors.py
 pypynum/file.py
 pypynum/maths.py
 pypynum/numbers.py
 pypynum/plotting.py
+pypynum/polynomial.py
 pypynum/probability.py
 pypynum/random.py
 pypynum/regression.py
 pypynum/sequence.py
 pypynum/test.py
 pypynum/this.py
 pypynum/tools.py
```

### Comparing `PyPyNum-1.7.0/pypynum/Array.py` & `PyPyNum-1.8.0/pypynum/Array.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/FourierT.py` & `PyPyNum-1.8.0/pypynum/FourierT.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Geometry.py` & `PyPyNum-1.8.0/pypynum/Geometry.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Group.py` & `PyPyNum-1.8.0/pypynum/Group.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Logic.py` & `PyPyNum-1.8.0/pypynum/Logic.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Matrix.py` & `PyPyNum-1.8.0/pypynum/Matrix.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/NeuralN.py` & `PyPyNum-1.8.0/pypynum/NeuralN.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Quaternion.py` & `PyPyNum-1.8.0/pypynum/Quaternion.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Symbolics.py` & `PyPyNum-1.8.0/pypynum/Symbolics.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Tensor.py` & `PyPyNum-1.8.0/pypynum/Tensor.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/Tree.py` & `PyPyNum-1.8.0/pypynum/Tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,8 +83,8 @@
             return self.root.find_node(data)
         return None
 
     def traverse(self, traversal_type="preorder"):
         if self.root:
             self.root.traverse(traversal_type)
         else:
-            print("Tree is empty")
+            raise ValueError("Tree is empty")
```

### Comparing `PyPyNum-1.7.0/pypynum/Vector.py` & `PyPyNum-1.8.0/pypynum/Vector.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/__init__.py` & `PyPyNum-1.8.0/pypynum/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,33 @@
 from .cipher import *
 from . import constants
 from .equations import *
 from . import errors
 from .file import read, write
 from .FourierT import *
 from .Geometry import *
+from .Graph import *
 from .Group import group
 from .Logic import *
 from .maths import *
 from .Matrix import mat, identity, lu, qr, eig, svd
 from .NeuralN import *
 from .numbers import *
 from .plotting import unary, binary, c_unary, color
+from .polynomial import *
 from .probability import *
 from .Quaternion import quat, euler
 from .random import *
 from .regression import *
 from .sequence import *
 from .Symbolics import *
 from .Tensor import ten, tensorproduct
 from .tools import *
 from .Tree import *
 from . import types
 from .utils import OrderedSet, InfIterator
 from .Vector import vec
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 print("PyPyNum", "Version -> " + __version__, "PyPI -> https://pypi.org/project/PyPyNum/",
       "Gitee -> https://www.gitee.com/PythonSJL/PyPyNum", sep=" | ")
 del math, arr, ite, num, real, geom, ContentError, RandomError, LogicError, InputError, FullError, Union
```

### Comparing `PyPyNum-1.7.0/pypynum/__temporary.py` & `PyPyNum-1.8.0/pypynum/__temporary.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/chars.py` & `PyPyNum-1.8.0/pypynum/chars.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/cipher.py` & `PyPyNum-1.8.0/pypynum/cipher.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/constants.py` & `PyPyNum-1.8.0/pypynum/constants.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/equations.py` & `PyPyNum-1.8.0/pypynum/equations.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/file.py` & `PyPyNum-1.8.0/pypynum/file.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/maths.py` & `PyPyNum-1.8.0/pypynum/maths.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import math
 from .types import Union, arr, num, real
 
+__and = {0, 1, 4, 9, 16, 17, 25, 33, 36, 41, 49, 57, 64, 65, 68, 73, 81, 89, 97, 100, 105, 113,
+         121, 129, 132, 137, 144, 145, 153, 161, 164, 169, 177, 185, 193, 196, 201, 209, 217, 225, 228, 233, 241, 249}
+__max = 1 << 1023
+__mod = {0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 145, 160, 169,
+         180, 196, 225, 241, 244, 256, 265, 289, 304, 324, 340, 361, 369, 385, 400, 409,
+         436, 441, 481, 484, 496, 505, 529, 544, 576, 580, 585, 601, 625, 640, 649, 676}
+
 
 def root(x: num, y: num) -> num:
     """
     introduction
     ==========
     Root \n
     ʸ√x̄
@@ -1273,13 +1280,81 @@
             return 0
         else:
             inv = x % ni
         s += ai * inv * p
     return s % prod
 
 
+def isqrt(x: int) -> int:
+    """
+    introduction
+    ==========
+    Round after square root \n
+    [√x̄]
+
+    example
+    ==========
+    >>> isqrt(620448401733239439360000)
+    787685471322
+    >>>
+    :param x: integer
+    :return:
+    """
+    return iroot(x, 2)
+
+
+def is_possibly_square(n: int) -> bool:
+    """
+    introduction
+    ==========
+    Check if it is a possible square number
+
+    example
+    ==========
+    >>> is_possibly_square(123456 ** 789)
+    True
+    >>>
+    :param n: integer
+    :return:
+    """
+    if n < 0:
+        return False
+    if n % 720 not in __mod:
+        return False
+    if n & 0xFF not in __and:
+        return False
+    return True
+
+
+def is_square(n: int) -> bool:
+    """
+    introduction
+    ==========
+    Check if it is a square number
+
+    example
+    ==========
+    >>> is_square(123456 ** 789)
+    False
+    >>>
+    :param n: integer
+    :return:
+    """
+    if is_possibly_square(n):
+        if n <= __max:
+            sqrt = math.sqrt(n)
+            return int(sqrt) == sqrt
+        try:
+            from math import isqrt as f
+        except ImportError:
+            f = isqrt
+        sqrt = f(n)
+        return sqrt * sqrt == n
+    return False
+
+
 A = arrangement
 C = combination
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod(verbose=True)
```

### Comparing `PyPyNum-1.7.0/pypynum/numbers.py` & `PyPyNum-1.8.0/pypynum/numbers.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/plotting.py` & `PyPyNum-1.8.0/pypynum/plotting.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/probability.py` & `PyPyNum-1.8.0/pypynum/probability.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/random.py` & `PyPyNum-1.8.0/pypynum/random.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/regression.py` & `PyPyNum-1.8.0/pypynum/regression.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/sequence.py` & `PyPyNum-1.8.0/pypynum/sequence.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/test.py` & `PyPyNum-1.8.0/pypynum/test.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/this.py` & `PyPyNum-1.8.0/pypynum/this.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/pypynum/tools.py` & `PyPyNum-1.8.0/pypynum/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     return True
 
 
 def generate_primes(limit: int) -> list:
     """
     introduction
     ==========
-    Generate all prime numbers within specified limit values using linear screening method
+    Generate all prime numbers within the specified limit using linear filtering method
 
     example
     ==========
     >>> generate_primes(100)
     [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
     >>>
     :param limit: integer
@@ -272,14 +272,42 @@
             for i in range(s, limit + 1, p):
                 primes[i] = 0
         p += 1
         s = p * p
     return [x for x in primes if x != 0]
 
 
+def generate_semiprimes(limit: int) -> list:
+    """
+    introduction
+    ==========
+    Generate all semiprime numbers within the specified limit
+
+    example
+    ==========
+    >>> generate_semiprimes(64)
+    [4, 6, 9, 10, 14, 15, 21, 22, 25, 26, 33, 34, 35, 38, 39, 46, 49, 51, 55, 57, 58, 62]
+    >>>
+    :param limit: integer
+    :return:
+    """
+    primes = generate_primes(limit // 2)
+    length = len(primes)
+    semiprimes = []
+    for i in range(length):
+        first = primes[i]
+        maximum = limit // first
+        for j in range(i, length):
+            second = primes[j]
+            if second > maximum:
+                break
+            semiprimes.append(first * second)
+    return sorted(semiprimes)
+
+
 def prime_factors(integer: int, dictionary: bool = False, pollard_rho: bool = True) -> Union[list, dict]:
     """
     introduction
     ==========
     Using the Pollard Rho method to decompose prime factors of positive integers
 
     example
@@ -340,11 +368,79 @@
             return {number: output.count(number) for number in set(output)}
         else:
             return sorted(output)
     else:
         return []
 
 
+def magic_square(n):
+    """
+    introduction
+    ==========
+    Generate a magic square of a specified order
+
+    example
+    ==========
+    >>> magic_square(4)
+    [[16, 2, 3, 13], [5, 11, 10, 8], [9, 7, 6, 12], [4, 14, 15, 1]]
+    >>>
+    :param n: integer
+    :return:
+    """
+    if not isinstance(n, int) or n < 3:
+        raise ValueError("The order of the magic square must be an integer greater than or equal to three")
+    result = [[0] * n for _ in range(n)]
+
+    def odd():
+        i, j = 0, n // 2
+        for m in range(1, n * n + 1):
+            result[i][j] = m
+            new_i, new_j = (i - 1) % n, (j + 1) % n
+            if result[new_i][new_j] != 0:
+                new_i, new_j = (i + 1) % n, j
+            i, j = new_i, new_j
+
+    def single_even():
+        half = n // 2
+        left = magic_square(half)
+        x = n ** 2 // 4
+        k = (n - 2) // 4
+        for i in range(half):
+            for j in range(half):
+                result[i][j] = left[i][j]
+                result[i][j + half] = left[i][j] + 2 * x
+                result[i + half][j] = left[i][j] + 3 * x
+                result[i + half][j + half] = left[i][j] + x
+        for i in range(half):
+            for j in range(n):
+                if j > (half + k + 1):
+                    result[i][j], result[i + half][j] = result[i + half][j], result[i][j]
+                if j < k:
+                    result[i][j], result[i + half][j] = result[i + half][j], result[i][j]
+        result[k][0], result[k + half][0] = result[k + half][0], result[k][0]
+        result[k][k], result[k + half][k] = result[k + half][k], result[k][k]
+
+    def double_even():
+        c1 = 1
+        c2 = n * n
+        for i in range(n):
+            for j in range(n):
+                if i % 4 == j % 4 or (i + j) % 4 == 3:
+                    result[i][j] = c2
+                else:
+                    result[i][j] = c1
+                c2 -= 1
+                c1 += 1
+
+    if n & 1:
+        odd()
+    elif n & 3:
+        single_even()
+    else:
+        double_even()
+    return result
+
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod(verbose=True)
```

### Comparing `PyPyNum-1.7.0/pypynum/utils.py` & `PyPyNum-1.8.0/pypynum/utils.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.7.0/setup.py` & `PyPyNum-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 ﻿from setuptools import setup, find_packages
 
 with open("pypynum/README.md", "r", encoding="UTF-8") as r:
     md = r.read()
 
+keywords = [
+    "math", "数学", "mathematics", "数学计算",
+    "numerical", "数值", "computation", "计算",
+    "scientific", "科学", "algebra", "代数",
+    "calculus", "微积分", "statistics", "统计",
+    "linear-algebra", "线性代数", "optimization", "优化",
+    "numerical-analysis", "数值分析", "matrix", "矩阵",
+    "vector", "向量", "tensor", "张量",
+    "numerics", "数值计算", "library", "库",
+    "tools", "工具", "utils", "实用程序",
+    "algorithms", "算法", "software", "软件",
+    "package", "包", "methods", "方法",
+    "data-science", "数据科学", "machine-learning", "机器学习",
+    "computational", "计算的", "operations", "操作",
+    "functions", "函数", "processing", "处理",
+    "programming", "编程", "simulation", "仿真",
+    "visualization", "可视化", "physics", "物理"
+]
+
 LICENSE = """
                     GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
@@ -665,21 +684,22 @@
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <http://www.gnu.org/licenses/>.
 """
 
 setup(
     name="PyPyNum",
-    version="1.7.0",
-    packages=["pypynum"],
+    version="1.8.0",
+    packages=find_packages(),
     url="https://www.gitee.com/PythonSJL/PyPyNum",
     license=LICENSE,
     author="Shen Jiayi",
     author_email="2261748025@qq.com",
     description="""
     A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
     """,
     python_requires=">=3.5",
-    package_data={"pypynum": ["pypynum/*"]},
+    package_data={"pypynum": ["*"]},
     long_description=md,
-    long_description_content_type="text/markdown"
+    long_description_content_type="text/markdown",
+    keywords=keywords
 )
```

