# Comparing `tmp/schubmult-1.3.2.tar.gz` & `tmp/schubmult-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.2.tar", last modified: Wed Apr  3 21:06:44 2024, max compression
+gzip compressed data, was "schubmult-1.3.3.tar", last modified: Sat Apr 13 16:40:11 2024, max compression
```

## Comparing `schubmult-1.3.2.tar` & `schubmult-1.3.3.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.764000 schubmult-1.3.2/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 21:06:44.722000 schubmult-1.3.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3745 2024-04-03 18:41:26.000000 schubmult-1.3.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.020000 schubmult-1.3.2/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.2/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15361 2024-04-03 21:04:46.000000 schubmult-1.3.2/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.729000 schubmult-1.3.2/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.2/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.2/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4586 2023-12-24 14:56:44.000000 schubmult-1.3.2/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.030000 schubmult-1.3.2/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.2/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.2/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4248 2023-12-24 14:56:50.000000 schubmult-1.3.2/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.326000 schubmult-1.3.2/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.2/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.2/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     2817 2024-04-03 21:05:09.000000 schubmult-1.3.2/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:44.649000 schubmult-1.3.2/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.2/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.2/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42129 2024-03-18 16:03:30.000000 schubmult-1.3.2/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:06:43.447000 schubmult-1.3.2/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4127 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-03 21:06:42.000000 schubmult-1.3.2/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-03 21:06:41.000000 schubmult-1.3.2/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-03 21:06:44.758000 schubmult-1.3.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1117 2024-04-03 21:06:00.000000 schubmult-1.3.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.919000 schubmult-1.3.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5231 2024-04-13 16:40:11.868000 schubmult-1.3.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4849 2024-04-13 16:38:44.000000 schubmult-1.3.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:09.299000 schubmult-1.3.3/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.3/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.3/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.072000 schubmult-1.3.3/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.3/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.3/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.3/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.412000 schubmult-1.3.3/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.3/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.3/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.3/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.759000 schubmult-1.3.3/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.3/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.3/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9008 2024-04-08 20:08:59.000000 schubmult-1.3.3/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.082000 schubmult-1.3.3/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.3/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.3/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3042 2024-04-12 20:25:54.000000 schubmult-1.3.3/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.421000 schubmult-1.3.3/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5865 2024-04-12 18:47:48.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.802000 schubmult-1.3.3/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.3/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.3/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.3/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:09.745000 schubmult-1.3.3/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5231 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-13 16:40:08.000000 schubmult-1.3.3/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-13 16:40:11.904000 schubmult-1.3.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-12 18:51:29.000000 schubmult-1.3.3/setup.py
```

### Comparing `schubmult-1.3.2/LICENSE` & `schubmult-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.2/README.md` & `schubmult-1.3.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.0, it also handles quantum Schubert polynomials. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.3, it also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
-schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6
-schubmult_q 5 1 4 3 2 - 2 1 3 5 4
+schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6 --display-positive
+schubmult_q 5 1 4 3 2 - 5 1 3 4 2
+schubmult_q_double 5 1 4 3 2 - 5 1 3 4 2
+schubmult_q_yz 5 1 4 3 2 - 2 5 1 3 4 --display-positive
 ```
 
 The same execution with the Lehmer code:
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
-schubmult_yz -code 0 1 1 2 - 1 0 2 3
-schubmult_q -code 4 0 2 1 - 1 0 0 1
+schubmult_yz -code 0 1 1 2 - 1 0 2 3 --display-positive
+schubmult_q -code 4 0 2 1 - 4 0 1 1
+schubmult_q_double -code 4 0 2 1 - 4 0 1 1
+schubmult_q_yz 5 4 0 2 1 - 1 3 --display-positive
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
-schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4
+schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4 --display-positive
 ```
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
-schubmult_yz -code -coprod 0 1 2 3 - 2 4
+schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
 
 
-Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative and the problem is in GapP, it is not known to be in #P at this time.
+Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
-schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Both have the same command line syntax as schubmult. schubmult_double displays the result with nonnegative coefficients in terms of the negative simple roots. Both are of course slower than schubmult_py, and expressing the result positively for schubmult_double slows it down even more.
+schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
 New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
@@ -52,14 +56,12 @@
 
 ```
 from schubmult.schubmult_py import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6))
 ```
 
-Note versions 1.0.15 and prior had a bug that failed to upgrade the executable. The coefficients it computed were correct, but it was not using the updated version.
-
-Version 1.0.18 adds the command line argument --display-positive to schubmult_yz, which displays the result positively (if possible, this is still only always possible conjecturally). This is highly processor intensive.
+Version 1.0.18 adds the command line argument --display-positive to schubmult_yz (and version 1.3.3 adds --display-positive to schubmult_q_yz), which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
 
 ![](https://raw.githubusercontent.com/matthematics/schubmult/main/positive_image.png)
 
 [Homepage of schubmult](http://schubmult.org/)
```

### Comparing `schubmult-1.3.2/schubmult/perm_lib.py` & `schubmult-1.3.3/schubmult/perm_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -309,14 +309,36 @@
 		if u2[j]==j+1:
 			yvars += [varl1[u2[j]]]
 	for j in range(len(u2),k):
 		yvars += [varl1[j+1]]
 	zvars = [varl2[i] for i in call_zvars(v1,v2,k,i)]
 	return elem_sym_poly(newk-vdiff,newk,yvars,zvars)
 
+def elem_sym_func_q(k,i,u1,u2,v1,v2,udiff,vdiff,varl1,varl2):
+	global zero, one
+	newk = k - udiff
+	if newk < vdiff:
+		return zero
+	if newk == vdiff:
+		return one
+	yvars = []
+	mlen = max(len(u1),len(u2))
+	u1 = [*u1] + [a+1 for a in range(len(u1),mlen)]
+	u2 = [*u2] + [a+1 for a in range(len(u2),mlen)]
+	for j in range(min(len(u1),k)):
+		if u1[j]==u2[j]:
+			yvars += [varl1[u2[j]]]
+	for j in range(len(u1),min(k,len(u2))):
+		if u2[j]==j+1:
+			yvars += [varl1[u2[j]]]
+	for j in range(len(u2),k):
+		yvars += [varl1[j+1]]
+	zvars = [varl2[a] for a in call_zvars(v1,v2,k,i)]
+	return elem_sym_poly(newk-vdiff,newk,yvars,zvars)
+
 def trimcode(perm):
 	cd = code(perm)
 	while len(cd)>0 and cd[-1] == 0:
 		cd.pop()
 	return cd
 
 def p_trans(part):
```

### Comparing `schubmult-1.3.2/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.3/schubmult/schubmult_double/schubmult_double.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 n = 100
 
 var = symarray('x', n)
 var2 = symarray('y',n)
 var3 = var2
 var_r = symarray('r',n)
 
+var_q = Symbol("q")
+
 subs_dict = {}
 
 for i in range(1,n):
 	sm = var_r[0]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 
+
+
 def main():
 	try:			
 		perms=[]
 		curperm = []
 		
 		pr = True
 		ascode = False
@@ -41,20 +45,23 @@
 					continue
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
+			print("**** schubmult_double ****")
+			print("Purpose: Compute products (and coproducts) of double Schubert polynomials in the same set of variables")
 			print("Usage: schubmult_double <-np|--no-print> <-code> perm1 - perm2 < - perm 3 ... >")
 			print("Alternative usage: schubmult_double <-code> -coprod perm - indexlist")
 			exit(1)
 		
 		perms += [curperm]
 		
+		
 		if coprod:
 			subs_dict_coprod = {}
 			if ascode:
 				mperm = tuple(permtrim(uncode(perms[0])))
 			else:
 				mperm = tuple(permtrim(perms[0]))
```

### Comparing `schubmult-1.3.2/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.3/schubmult/schubmult_py/schubmult_py.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,16 @@
 					continue
 				if s == "-":
 					perms += [tuple(curperm)]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
+			print("**** schubmult_py ****")
+			print("Purpose: Compute products (and coproducts) of ordinary Schubert polynomials")
 			print("Usage: schubmult_py <-np|--no-print> <-code> perm1 - perm2 <- perm3...>")
 			print("Alternative usage: schubmult_py -coprod <-np> <perm> - <index list>")
 			exit(1)
 		
 		perms += [tuple(curperm)]
 		
 		if coprod:
```

### Comparing `schubmult-1.3.2/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.3/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1323,14 +1323,16 @@
 					exit(0)
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
+			print("**** schubmult_yz ****")
+			print("Purpose: Compute products (and coproducts) of double Schubert polynomials in different sets of variables")
 			print("Usage: schubmult_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
 			print("Alternative usage: schubmult_yz <-code> <--display-positive> <--optimizer-message> -coprod perm - indexlist")
 			exit(1)
 				
 		perms += [curperm]
 		posified = False
 		if coprod:
@@ -1506,18 +1508,22 @@
 						notint = False
 						try:
 							int(val)
 						except Exception:
 							notint = True
 						if notint and display_positive:
 							valu = val
-							if len(perms) == 2 and not posified:
-								val = posify(val,perms[0],perms[1],perm,var2,var3,msg)							
-							elif not posified:								
-								val = compute_positive_rep(val,var2,var3,msg)								
+							try:
+								if len(perms) == 2 and not posified:
+									val = posify(val,perms[0],perms[1],perm,var2,var3,msg)							
+								elif not posified:								
+									val = compute_positive_rep(val,var2,var3,msg)
+							except TypeError:
+								print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
+								exit(1)
 							if check and expand(val - check_coeff_dict.get(perm,0))!=0:
 								print(f"error; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {check_coeff_dict.get(perm,0)=}")
 								exit(1)
 						if val!=0:
 							if ascode:
 								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ')}")	
 							else:
```

### Comparing `schubmult-1.3.2/setup.py` & `schubmult-1.3.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.2",
+    version="1.3.3",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
@@ -27,10 +27,12 @@
 		"psutil",
 		"cachetools",
 		"sortedcontainers"
     ],
     entry_points={"console_scripts": ["schubmult_py=schubmult.schubmult_py.__main__:main",
 	"schubmult_double=schubmult.schubmult_double.__main__:main",
 	"schubmult_yz=schubmult.schubmult_yz.__main__:main",
-	"schubmult_q=schubmult.schubmult_q.__main__:main"
+	"schubmult_q=schubmult.schubmult_q.__main__:main",
+	"schubmult_q_double=schubmult.schubmult_q_double.__main__:main",
+	"schubmult_q_yz=schubmult.schubmult_q_yz.__main__:main"
 	]},
 )
```

