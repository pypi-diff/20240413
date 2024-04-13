# Comparing `tmp/VASP2KP-1.0.2.tar.gz` & `tmp/VASP2KP-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VASP2KP-1.0.2.tar", last modified: Tue Dec 12 08:53:31 2023, max compression
+gzip compressed data, was "VASP2KP-1.1.1.tar", last modified: Sat Apr 13 14:57:39 2024, max compression
```

## Comparing `VASP2KP-1.0.2.tar` & `VASP2KP-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2023-12-12 08:53:31.440622 VASP2KP-1.0.2/
--rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.0.2/LICENSE.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2023-12-12 08:53:31.440364 VASP2KP-1.0.2/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.0.2/README.md
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2023-12-12 08:53:31.439047 VASP2KP-1.0.2/VASP2KP/
--rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.0.2/VASP2KP/__init__.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    30147 2023-12-06 06:46:18.000000 VASP2KP-1.0.2/VASP2KP/_get_kp_Zeeman.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    61690 2023-12-06 06:46:36.000000 VASP2KP-1.0.2/VASP2KP/_numeric_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    19910 2023-12-06 06:46:47.000000 VASP2KP-1.0.2/VASP2KP/_read_data.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    90097 2023-12-10 16:48:18.000000 VASP2KP-1.0.2/VASP2KP/_standard_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2023-12-06 06:46:42.000000 VASP2KP-1.0.2/VASP2KP/_transform_matrix.py
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2023-12-12 08:53:31.440082 VASP2KP-1.0.2/VASP2KP.egg-info/
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2023-12-12 08:53:31.000000 VASP2KP-1.0.2/VASP2KP.egg-info/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)      421 2023-12-12 08:53:31.000000 VASP2KP-1.0.2/VASP2KP.egg-info/SOURCES.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2023-12-12 08:53:31.000000 VASP2KP-1.0.2/VASP2KP.egg-info/dependency_links.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2023-12-06 08:19:29.000000 VASP2KP-1.0.2/VASP2KP.egg-info/not-zip-safe
--rw-r--r--   0 shengzhang   (501) staff       (20)       34 2023-12-12 08:53:31.000000 VASP2KP-1.0.2/VASP2KP.egg-info/requires.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        8 2023-12-12 08:53:31.000000 VASP2KP-1.0.2/VASP2KP.egg-info/top_level.txt
--rwxrwxrwx   0 shengzhang   (501) staff       (20)     7909 2023-12-06 06:48:38.000000 VASP2KP-1.0.2/mat2kp
--rw-r--r--   0 shengzhang   (501) staff       (20)       38 2023-12-12 08:53:31.440673 VASP2KP-1.0.2/setup.cfg
--rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2023-12-12 08:52:56.000000 VASP2KP-1.0.2/setup.py
--rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.0.2/vasp2mat.5.3-patch-1.0.1.sh
--rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.0.2/vasp2mat.6.4-patch-1.0.1.sh
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.310530 VASP2KP-1.1.1/
+-rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.1/LICENSE.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-13 14:57:39.310247 VASP2KP-1.1.1/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.1/README.md
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.308596 VASP2KP-1.1.1/VASP2KP/
+-rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.1/VASP2KP/__init__.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    31348 2024-04-13 14:51:46.000000 VASP2KP-1.1.1/VASP2KP/_get_kp_Zeeman.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.1/VASP2KP/_numeric_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    51333 2024-04-13 14:47:52.000000 VASP2KP-1.1.1/VASP2KP/_read_data.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.1/VASP2KP/_standard_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.1/VASP2KP/_transform_matrix.py
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.309955 VASP2KP-1.1.1/VASP2KP.egg-info/
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/SOURCES.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/dependency_links.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/not-zip-safe
+-rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/requires.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/top_level.txt
+-rwxrwxrwx   0 shengzhang   (501) staff       (20)     8618 2024-04-13 13:03:07.000000 VASP2KP-1.1.1/mat2kp
+-rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-13 14:57:39.310595 VASP2KP-1.1.1/setup.cfg
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-13 14:57:31.000000 VASP2KP-1.1.1/setup.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.1/vasp2mat.5.3-patch-1.0.1.sh
+-rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.1/vasp2mat.6.4-patch-1.0.1.sh
```

### Comparing `VASP2KP-1.0.2/LICENSE.txt` & `VASP2KP-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.0.2/PKG-INFO` & `VASP2KP-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.0.2
+Version: 1.1.1
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.0.2/README.md` & `VASP2KP-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.0.2/VASP2KP/__init__.py` & `VASP2KP-1.1.1/VASP2KP/__init__.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.0.2/VASP2KP/_get_kp_Zeeman.py` & `VASP2KP-1.1.1/VASP2KP/_get_kp_Zeeman.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,80 +5,80 @@
 
 @author: Sheng Zhang, Institute of Physics, Chinese Academy of Sciences
 
 Main function of VASP2KP
 """
 
 
-from ._numeric_kp import get_numeric_kp,get_U_pi_sigma,SymmetryError,Symmetry_conjugate_flag
+from ._numeric_kp import get_numeric_kp,get_U_pi_sigma,SymmetryERROR,Symmetry_conjugate_flag
 from ._standard_kp import get_std_kp,get_Zeeman
 from ._read_data import load_data
 
 
 import sys
 import os
 import subprocess
 import kdotp_generator as kp
 import sympy as sp
 from sympy.core.numbers import I
 import numpy as np
 import warnings
 
 ###############################################################################
-# define Error class(type)
-class ModelTooHighOrderError(Exception):
+# define ERROR class(type)
+class ModelTooHighOrderERROR(Exception):
     '''
-    If order >=4: raise this Error
+    If order >=4: raise this ERROR
     '''
     pass
 
-class PrintFlagError(Exception):
+class PrintFlagERROR(Exception):
     '''
-    If print_flag not in [0,1,2]: raise this Error
+    If print_flag not in [0,1,2]: raise this ERROR
     '''
     pass
 
-class GFactorError(Exception):
+class GFactorERROR(Exception):
     '''
-    If gfactor not in [0,1]: raise this Error
+    If gfactor not in [0,1]: raise this ERROR
     '''
     pass
 
-class BandChooseError(Exception):
+class BandChooseERROR(Exception):
     pass
 
-class OrderChooseError(Exception):
+class OrderChooseERROR(Exception):
     '''
-    If order not in [1,2,3]: raise this Error
+    If order not in [1,2,3]: raise this ERROR
     '''
     pass
 
-class LogChooseError(Exception):
+class LogChooseERROR(Exception):
     '''
-    If log not in [0,1]: raise this Error
+    If log not in [0,1]: raise this ERROR
     '''
     pass
 
-class AccSetError(Exception):
+class AccSetERROR(Exception):
     '''
-    If acc not in [0,1]: raise this Error
+    If acc not in [0,1]: raise this ERROR
     '''
     pass
 
-class numbaNotInstallError(Exception):
+class numbaNotInstallERROR(Exception):
     '''
-    If 'import numba' fails: raise this Error
+    If 'import numba' fails: raise this ERROR
     '''
     pass
 ###############################################################################
 
 
 
 ###############################################################################
-def get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,order = 2,gfactor = 1,print_flag = 2,log = 0, acc = 0, msg_num = None,kvec = None):
+def get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,repr_split = True,dim_list=[],order = 2,gfactor = 1,print_flag = 2,log = 0, acc = 0, msg_num = None,kvec = None):
     '''
     After reading the VASP calculation data, get the kp Hamiltonian matrix as well as the Zeeman's coupling as well as the numerical parameters
 
     Parameters
     ----------
     data : dictionary
         the input DFT data, generalized momentum matrices as well as spin matrices
@@ -123,42 +123,48 @@
     Zeeman_coe : dictionary
         the keys are coefficients' names, the values are lists
                     the zeroth element of each list is the value of the coefficient
                     the first element of each list is a matrix of each independent Zeeman's coupling
                     result_Zeeman_array is the sum of the zeroth element* the first element of each list
         
     '''
+    
+    if dim_list == []:
+        dim_list = list(operator.values())[0].shape[0]
 
     # get the list of pi (3 components), the list of sigma (3 components), similarity transformation matrix between two corepresentation
-    pi_list,sigma_list,U,Symmetry = get_U_pi_sigma(data,operator,Symmetry,gfactor,log)
+    pi_list,sigma_list,U,Symmetry = get_U_pi_sigma(data,operator,Symmetry,repr_split ,dim_list,gfactor,log)
+    print("Find the unitary transformation U successfully (U^-1 D^num U= D^std) !")
     
     # calculate the numerical kp hamiltonian and Zeeman's coupling
     numeric_kp = get_numeric_kp(pi_list,sigma_list,U,eigen_energy,band_interest_set,order,gfactor,acc)
+    print("Finish downfolding processes!")
     
     # calculate the standard kp Hamiltonian
     if order>=1:
         result_kp_array,kpmodel_coe = get_std_kp(Symmetry,order,gfactor,msg_num,kvec,numeric_kp,print_flag,log)
+        print('''Finish constructing kp invariant Hamiltonian in "kp-parameters.out"!''')
     else:
         result_kp_array = 0
         kpmodel_coe={}
     
     if gfactor == 1: # calculate the Zeeman's coupling
     
         G_4c4 = numeric_kp["B"]
         result_Zeeman_array,Zeeman_coe = get_Zeeman(Symmetry,msg_num,kvec,G_4c4,order,print_flag,log)
-        
+        print('''Finish constructing Zeeman's coupling in "g-factors.out"!''')
         return result_kp_array,kpmodel_coe,result_Zeeman_array,Zeeman_coe
     
     return result_kp_array,kpmodel_coe
 ###############################################################################
 
 
 
 ###############################################################################
-def get_std_kp_Zeeman(Symmetry,vaspMAT='mat',kpmodel = 1, order = 2,gfactor = 1,print_flag = 2,log = 0,acc = 0,msg_num = None,kvec = None):
+def get_std_kp_Zeeman(Symmetry,vaspMAT='mat',vmat_k = 1,kpmodel = 1, repr_split = True,order = 2,gfactor = 1,print_flag = 2,log = 0,acc = 0,msg_num = None,kvec = None):
     '''
     The main function 
     Obtain the kp Hamiltonian matrix as well as the Zeeman's coupling as well as the numerical parameters
     
     Notice: you can treat the parameters msg_num and kvec as not existing
     
     Parameters
@@ -202,28 +208,28 @@
     msg_num : decimal or integer, optional
         user's input, magnetic space group number. The default is None. 
     kvec : list, optional
         user's input, the high symmetry point coordinate. The default is None.
 
     Raises
     ------
-    ModelTooHighOrderError
-        if order>4, raise this error: the package can just deal with at most third-order Hamiltonians.
-    OrderChooseError
-        if order<0 or order is not a integer, raise this error.
-    PrintFlagError
-        if print_flag not in [0,1,2], raise this error: the wrong parameter print_flag.
-    GFactorError
-        if gfactor not in [0,1], raise this error: the wrong parameter gfactor.
-    LogChooseError
-        if log not in [0,1], raise this error: the wrong parameter log
-    AccSetError
-        if acc not in [0,1], raise this error: the wrong parameter acc
-    numbaNotInstallError
-        if acc==1 and numba has not been installed, raise this error
+    ModelTooHighOrderERROR
+        if order>4, raise this ERROR: the package can just deal with at most third-order Hamiltonians.
+    OrderChooseERROR
+        if order<0 or order is not a integer, raise this ERROR.
+    PrintFlagERROR
+        if print_flag not in [0,1,2], raise this ERROR: the wrong parameter print_flag.
+    GFactorERROR
+        if gfactor not in [0,1], raise this ERROR: the wrong parameter gfactor.
+    LogChooseERROR
+        if log not in [0,1], raise this ERROR: the wrong parameter log
+    AccSetERROR
+        if acc not in [0,1], raise this ERROR: the wrong parameter acc
+    numbaNotInstallERROR
+        if acc==1 and numba has not been installed, raise this ERROR
 
     Returns
     -------
     result_kp_array : sympy.matrices.dense.MutableDenseMatrix
         the effective kp model(the sum of the effective kp models of each order as well as their parameters)
     result_kpmodel_g : sympy.matrices.dense.MutableDenseMatrix
         the effective Zeeman's coupling(the parameters have been found and substituted in.)
@@ -239,69 +245,79 @@
     Zeeman_coe : a dictionary
         keys: coefficient name, TYPE: sympy.core.symbol.Symbol
         values: a list,
             The zeroth element is the value of the parameter.
             The first element is the matrix of the independent Zeeman coupling. 
             
     '''
-    
-    # simple input error detection
+
+    # simple input ERROR detection
     if order>=4:
-        raise ModelTooHighOrderError("The order of the kp model is too high"+"("+str(order)+")"+", please adjust the parameter order to <=3!")
+        #raise ModelTooHighOrderERROR("The order of the kp model is too high"+"("+str(order)+")"+", please adjust the parameter order to <=3!")
+        print("ERROR: The order of the kp model is too high"+"("+str(order)+")"+", please adjust the parameter order to <=3!")
         sys.exit()
-        
-    if order not in [2,3]:
-        raise OrderChooseError("The parameter order cannot be negative or decimal!")
+
+    if order not in [1,2,3]:
+        #raise OrderChooseERROR("The parameter order cannot be negative or decimal!")
+        print("ERROR: The parameter order cannot be negative or decimal!")
         sys.exit()
         
     if print_flag not in [0,1,2]:
-        raise PrintFlagError("The parameter print_flag should be 0,1 or 2!")
+        #raise PrintFlagERROR("The parameter print_flag should be 0,1 or 2!")
+        print("TERROR: The parameter print_flag should be 0,1 or 2!")
         sys.exit()
     
     if gfactor not in [0,1]:
-        raise GFactorError()("The parameter gfactor should be 0,1!")
+        #raise GFactorERROR("The parameter gfactor should be 0,1!")
+        print("ERROR: The parameter gfactor should be 0,1!")
         sys.exit()
     
     if log not in [0,1]:
-        raise LogChooseError("The parameter log should be 0,1!")
+        #raise LogChooseERROR("The parameter log should be 0,1!")
+        print("ERROR: The parameter log should be 0,1!")
         sys.exit()
         
     if acc not in [0,1]:
-        raise AccSetError("The parameter acc should be 0,1!")
+        #raise AccSetERROR("The parameter acc should be 0,1!")
+        print("ERROR: The parameter acc should be 0,1!")
         sys.exit()
         
     if acc == 1:
         
         # test
         try:
             import numba
             
         except:
-            raise numbaNotInstallError("The package numba is not installed! If you do not want to accelerate the code, set parameter acc to 0.")
+            #raise numbaNotInstallERROR("The package numba is not installed! If you do not want to accelerate the code, set parameter acc to 0.")
+            print("ERROR: The package numba is not installed! If you do not want to accelerate the code, set parameter acc to 0.")
             sys.exit()
-            
+    
     for i in Symmetry.keys():
         i_val = Symmetry[i]
         
         if 'rotation_matrix' not in i_val.keys():
             wrong_str = "The key 'rotation_matrix' of '"+i+"' not exist!"
             
-            raise SymmetryError(wrong_str)
+            #raise SymmetryERROR(wrong_str)
+            print("ERROR: "+wrong_str)
+            sys.exit()
             
         if 'repr_has_cc' not in i_val.keys():
             wrong_str = "The key 'repr_has_cc' of '"+i+"' not exist!"
             
-            raise SymmetryError(wrong_str)
+            #raise SymmetryERROR(wrong_str)
+            print('ERROR: '+wrong_str)
+            sys.exit()
     
     if kpmodel == 0:
         order = 0        
     
     # load data from .m file
-    operator,data,eigen_energy,band_interest_set = load_data(Symmetry,vaspMAT,gfactor)
-        
+    operator,data,eigen_energy,band_interest_set,dim_list = load_data(Symmetry,vaspMAT,gfactor,vmat_k,repr_split)
     # unified dimensions
     size = 0
     
     for i in data.keys():
         size = max(size,data[i].shape[0])
         
     eigen_energy = eigen_energy[:size]
@@ -324,21 +340,21 @@
         Symmetry = Symmetry_copy
         
     #print(Symmetry_conjugate_flag)
     
     #print(Symmetry)
     
     if gfactor == 1: # calculate the Zeeman coupling
-        result_kp_array,kpmodel_coe,result_kpmodel_g,Zeeman_coe=get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,order,gfactor,print_flag,log,acc,msg_num,kvec)
+        result_kp_array,kpmodel_coe,result_kpmodel_g,Zeeman_coe=get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,repr_split ,dim_list,order,gfactor,print_flag,log,acc,msg_num,kvec)
         #return result_kp_array,kpmodel_coe,result_kpmodel_g,Zeeman_coe
         warnings.filterwarnings("ignore")
         return result_kp_array,result_kpmodel_g
     
     else:
-        result_kp_array,kpmodel_coe = get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,order,gfactor,print_flag,log,acc,msg_num,kvec)
+        result_kp_array,kpmodel_coe = get_std_kp_Zeeman_given_data(data,operator,eigen_energy,Symmetry,band_interest_set,repr_split ,dim_list,order,gfactor,print_flag,log,acc,msg_num,kvec)
         #return result_kp_array,kpmodel_coe,None,None
         warnings.filterwarnings("ignore")
         return result_kp_array,None
 ###############################################################################
 
 
 
@@ -379,46 +395,46 @@
     msg_num : decimal or integer, optional
         user's input, magnetic space group number. The default is None. 
     kvec : list, optional
         user's input, the high symmetry point coordinate. The default is None.
 
     Raises
     ------
-    OrderChooseError
-        if order<0 or order is not a integer, raise this error.
-    PrintFlagError
-        if print_flag not in [0,1,2], raise this error: the wrong parameter print_flag.
-    GchooseError
-        if gfactor not in [0,1], raise this error: the wrong parameter gchoose.
-    LogChooseError
-        if log not in [0,1], raise this error: the wrong parameter log
+    OrderChooseERROR
+        if order<0 or order is not a integer, raise this ERROR.
+    PrintFlagERROR
+        if print_flag not in [0,1,2], raise this ERROR: the wrong parameter print_flag.
+    GchooseERROR
+        if gfactor not in [0,1], raise this ERROR: the wrong parameter gchoose.
+    LogChooseERROR
+        if log not in [0,1], raise this ERROR: the wrong parameter log
 
     Returns
     -------
     sum_kp : sympy.matrices.dense.MutableDenseMatrix
         the effective kp model(without getting the values of the parameters.)
     sum_Zeeman : sympy.matrices.dense.MutableDenseMatrix
         the effective Zeeman coupling(without getting the values of the parameters.)
 
     '''
     
     if int(order) != order and order > 0:
-        raise OrderChooseError("The parameter order cannot be negative or decimal!")
+        raise OrderChooseERROR("The parameter order cannot be negative or decimal!")
         sys.exit()
         
     if print_flag not in [0,1,2]:
-        raise PrintFlagError("The parameter print_flag should be 0,1 or 2!")
+        raise PrintFlagERROR("The parameter print_flag should be 0,1 or 2!")
         sys.exit()
     
     if gfactor not in [0,1]:
-        raise GFactorError("The parameter gchoose should be 0,1!")
+        raise GFactorERROR("The parameter gchoose should be 0,1!")
         sys.exit()
     
     if log not in [0,1]:
-        raise LogChooseError("The parameter log should be 0,1!")
+        raise LogChooseERROR("The parameter log should be 0,1!")
         sys.exit()
     
     if log != 0:
         logging = open("independent_kp_models(without numerical parameters).log","w")
         logging.write('\nPrint kp results:\n')
         
     else:
```

### Comparing `VASP2KP-1.0.2/VASP2KP/_numeric_kp.py` & `VASP2KP-1.1.1/VASP2KP/_numeric_kp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 """
 
 import numpy as np
 import sympy as sp
 import sys
 
 from ._transform_matrix import get_transform_matrix
-from ._transform_matrix import CoRepresentationInequivalenceError
+from ._transform_matrix import CoRepresentationInequivalenceERROR
 
 ###############################################################################
 # whether to reduce 'repr_matrix' to 'band_rep_matrix_list' then calculation
-flag_reduce_Symmetry = False
+flag_reduce_Symmetry = True
 
 # whether take the conjugate
 Symmetry_conjugate_flag = False
 ###############################################################################
 
 ###############################################################################
-# define Error class(type)
-class SymmetryError(Exception):
+# define ERROR class(type)
+class SymmetryERROR(Exception):
     '''
-    if the keys of the parameter Symmetry are not correct, raise this error
+    if the keys of the parameter Symmetry are not correct, raise this ERROR
     '''
     pass
 
-class VASPMomentumMatrixError(Exception):
+class VASPMomentumMatrixERROR(Exception):
     '''
-    if the generalized momentum matrices' names got by vasp2mat are not 'Pix', 'Piy' and 'Piz', raise this error.
+    if the generalized momentum matrices' names got by vasp2mat are not 'Pix', 'Piy' and 'Piz', raise this ERROR.
     '''
     pass
 
-class VASPSpinMatrixError(Exception):
+class VASPSpinMatrixERROR(Exception):
     '''
-    if the spin matrices's names are not 'Pix', 'Piy' and 'Piz', raise this error.
+    if the spin matrices's names are not 'Pix', 'Piy' and 'Piz', raise this ERROR.
     '''
     pass
 ###############################################################################
 
 
 
 ###############################################################################
@@ -192,24 +192,24 @@
 
     Returns
     -------
     diagonal_block_dimensions : list
         The list comprised of each dimension.
 
     '''
+
     rows, cols = A.shape
     
     diagonal_block_dimensions = []
     
     j=0
     j0 = 0
     dim = 0
     
     while True:
-        
         if A[j:,j:].is_zero_matrix:
             
             for l in range(rows-j):
                 diagonal_block_dimensions.append(1)
                 
             break
         
@@ -251,15 +251,15 @@
             dim = max(i,k)+1
         
             if dim>=rows:
                 break
             
             tmp_flag = 0
             
-            for l in range(j,dim):
+            for l in range(dim):
                 
                 if not A[l,dim:].is_zero_matrix:
                     tmp_flag = 1
                     
                     break
                 
                 if not A[dim:,l].is_zero_matrix:
@@ -270,21 +270,21 @@
             if tmp_flag == 0:
                 diagonal_block_dimensions.append(dim-j0)
                 j0 = dim
                 
             j=dim
             
             
-    
     diagonal_block_dimensions.append(rows-sum(diagonal_block_dimensions))
     
     # remove redundant elements
     if diagonal_block_dimensions[-1] == 0:
         del diagonal_block_dimensions[-1]
     
+    #sys.exit()
     return diagonal_block_dimensions
 ###############################################################################
 
 
 
 ###############################################################################
 def get_max_dim(dim_list):
@@ -464,15 +464,15 @@
         
     return new_Symmetry, max_dim_list
 ###############################################################################
 
 
 
 ###############################################################################
-def get_corep_dim_reduce(Symmetry):
+def get_corep_dim_reduce(Symmetry,other_dim_list=[]):
     '''
     reduce 'repr_matrix' to 'band_rep_matrix_list'
 
     Parameters
     ----------
     Symmetry : dictionary
         user's input. O(3) matrices, corepresentation matrices and whether complex conjugate contains
@@ -485,23 +485,32 @@
     max_dim_list : list
         the list of the shared dimensions of each blocks
 
     '''
     #deep copy
     new_Symmetry = Symmetry.copy()
     
+
     # reduce the calculation time
     sum_rep = sp.zeros(*(list(new_Symmetry.values())[0]['repr_matrix'].shape))
     
     for i in new_Symmetry.keys():
         new_Symmetry[i] = Symmetry[i].copy()
         sum_rep += abs(new_Symmetry[i]['repr_matrix'])
 
         
-    max_dim_list = get_block_dim(sum_rep)
+    dim_list = get_block_dim(sum_rep)
+    
+    if len(other_dim_list) != 0:
+        max_dim_list_input = other_dim_list.copy()
+        max_dim_list_input.append(dim_list)
+
+        max_dim_list = get_max_dim(max_dim_list_input)
+    else:
+        max_dim_list = dim_list
     
     for i in new_Symmetry.keys():
         new_Symmetry[i]['band_repr_matrix_list'] = get_matrix_per_block(new_Symmetry[i]['repr_matrix'], max_dim_list)
         
         del new_Symmetry[i]['repr_matrix']
         
     return new_Symmetry, max_dim_list
@@ -928,15 +937,15 @@
         else:
             return {"1":eigen_trans,"k":linear_V2,"k^2":quadratic_V2_symm,"k^3":cubic_V2_symm,"B":G_4c4}
 ###############################################################################        
         
         
 
 ###############################################################################        
-def get_U_pi_sigma(data,operator,Symmetry,gfactor=1,log=0):
+def get_U_pi_sigma(data,operator,Symmetry,repr_split=True,dim_list = [],gfactor=1,log=0):
     '''
     find the similarity transformation matrix between VASP corep and standard corep, and transform the data to the list
 
     Parameters
     ----------
     data : dictionary
         the momentum matrices and the spin matrices under the VASP basis.
@@ -960,19 +969,22 @@
 
     '''
     
     flag = True #if the information of unitaryizing process will be printed to console when log = 0
     
     band_num = list(operator.values())[0].shape[0]
     
+    if dim_list == []:
+        dim_list = list(operator.values())[0].shape[0]
+        
     save_stdout = sys.stdout
     
     if log != 0:
         logging = open("find_similarity_transformation_matrix.log","w")
-        #logging.write('Errors in the optimization process (unitaryizing the similarity transformation matrix)\n')
+        #logging.write('ERRORs in the optimization process (unitaryizing the similarity transformation matrix)\n')
         
     else:
         if flag:
             # set the output stream to empty
             
             # judge what the system is
             import platform
@@ -1003,34 +1015,35 @@
     
     if flag_reduce_Symmetry:
         
         if 'repr_matrix' not in Symmetry[list(Symmetry.keys())[0]].keys():
             flag_reduce_Symmetry = False
             
         else:
-            Symmetry, dim_list = get_corep_dim_reduce(Symmetry)
+            
+            Symmetry, dim_list = get_corep_dim_reduce(Symmetry,[dim_list])
             operator = get_corep_VASP_reduce(operator,dim_list)
         
             print("Dimension composition:",dim_list)
-        
+
     if 'repr_matrix' in Symmetry[list(Symmetry.keys())[0]].keys():
         # try to find the similarity transformation matrix between VASP corep and standard corep
-        trace_error = False
+        trace_ERROR = False
         try:
             
             # reduce the tolerence gradually
             try:
                 U = get_transform_matrix(operator,Symmetry,band_num,tol = 1e-4)
                 
-            except (CoRepresentationInequivalenceError):
+            except (CoRepresentationInequivalenceERROR):
                 # trace not equal
-                raise CoRepresentationInequivalenceError("The standard corepresentation is not equivalent to VASP corepresentation!(traces error)")
+                raise CoRepresentationInequivalenceERROR("The standard corepresentation is not equivalent to VASP corepresentation!(traces ERROR)")
                 
-                if not trace_error:
-                    trace_error = True
+                if not trace_ERROR:
+                    trace_ERROR = True
                     
             except:
                 
                 try:
                     U = get_transform_matrix(operator,Symmetry,band_num,tol = 5e-4)
                 
                 except:
@@ -1061,18 +1074,18 @@
             for i in Symmetry.keys():
                 Symmetry[i]['repr_matrix']=sp.conjugate(Symmetry[i]['repr_matrix'])
             
             # reduce the tolerence gradually
             try:
                 U = get_transform_matrix(operator,Symmetry,band_num,tol = 1e-4)
                 
-            except (CoRepresentationInequivalenceError):
+            except (CoRepresentationInequivalenceERROR):
                 # trace not equal
-                if trace_error:
-                    raise CoRepresentationInequivalenceError("The standard corepresentation is not equivalent to VASP corepresentation!(traces error)")
+                if trace_ERROR:
+                    raise CoRepresentationInequivalenceERROR("The standard corepresentation is not equivalent to VASP corepresentation!(traces ERROR)")
                     sys.exit()
                     
                 else:
                     raise ValueError('Fail to find unitary U!')
                 
             except:
                 
@@ -1086,15 +1099,26 @@
                     
                     except:
                         
                         try:
                             U = get_transform_matrix(operator,Symmetry,band_num,tol = 5e-3)
                             
                         except:
-                            U = get_transform_matrix(operator,Symmetry,band_num,tol = 1e-2)
+                            try:
+                                U = get_transform_matrix(operator,Symmetry,band_num,tol = 1e-2)
+                            except:
+                                print("ERROR: Fail to find unitary U!")
+                                sys.stdout = save_stdout
+                                print("ERROR: Fail to find the unitary transformation U!")
+                                print('''Please check: 1. Whether the standard representation matrices in "mat2kp.in" are correct.''')
+                                print('''              2. Whether WAVECAR is not empty and LWAVE=.TRUE. is set in INCAR when running vasp2mat.''')
+                                print('''              3. Whether rot_n and rot_tau in "INCAR.mat" in INCAR.mat are correct when running vasp2mat.''')
+                                if repr_split:
+                                    print('''              4. If the above points are all checked but mat2kp still fails, or you do not use representation matrices from BCS Server, you can set "repr_split = False" in "mat2kp.in" and run mat2kp again.''')
+                                sys.exit()
                     
                     
     elif 'band_repr_matrix_list' in Symmetry[list(Symmetry.keys())[0]].keys():
         
         corepr_num = len(Symmetry[list(Symmetry.keys())[0]]['band_repr_matrix_list'])
         key_list = list(Symmetry.keys())
         dimension_tot = 0
@@ -1153,17 +1177,17 @@
                 
                 # reduce the tolerence gradually
                 try:
                     #print('flag1')
                     U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 1e-4)
                     #print('flag2')
                     
-                except (CoRepresentationInequivalenceError):
+                except (CoRepresentationInequivalenceERROR):
                     # trace not equal
-                    raise CoRepresentationInequivalenceError("The standard corepresentation is not equivalent to VASP corepresentation!(traces error)")
+                    raise CoRepresentationInequivalenceERROR("The standard corepresentation is not equivalent to VASP corepresentation!(traces ERROR)")
                 
                 except:
                     
                     try:
                         U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 5e-4)
                     
                     except:
@@ -1190,17 +1214,17 @@
                     Symmetry[k]['repr_matrix']=sp.conjugate(Symmetry[k]['repr_matrix'])
                     Symmetry[k]['band_repr_matrix_list'][i]=sp.conjugate(Symmetry[k]['band_repr_matrix_list'][i])
                 
                 # reduce the tolerence gradually
                 try:
                     U_ = get_transform_matrix(operator_,Symmetry,band_num,tol = 1e-4)
                     
-                except (CoRepresentationInequivalenceError):
+                except (CoRepresentationInequivalenceERROR):
                     # trace not equal
-                    raise CoRepresentationInequivalenceError("The standard corepresentation is not equivalent to VASP corepresentation!(traces error)")
+                    raise CoRepresentationInequivalenceERROR("The standard corepresentation is not equivalent to VASP corepresentation!(traces ERROR)")
                 
                 except:
                     
                     try:
                         U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 5e-4)
                     
                     except:
@@ -1210,68 +1234,77 @@
                         
                         except:
                             
                             try:
                                 U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 5e-3)
                                 
                             except:
-                                U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 1e-2)
+                                try:
+                                    U_ = get_transform_matrix(operator_,Symmetry,dimension,tol = 1e-2)
+                                except:
+                                    print("ERROR: Fail to find unitary U!")
+                                    sys.stdout = save_stdout
+                                    print("ERROR: Fail to find the unitary transformation U!")
+                                    print('''Please check: 1. Whether the standard representation matrices in "mat2kp.in" are correct.''')
+                                    print('''              2. Whether WAVECAR is not empty and LWAVE=.TRUE. is set in INCAR when running vasp2mat.''')
+                                    print('''              3. Whether rot_n and rot_tau in "INCAR.mat" in INCAR.mat are correct when running vasp2mat.''')
+                                    sys.exit()
                                     
             print("End finding the similarity transformation matrix of the part "+str(i+1))
             print("------------------------------------------------")
             print('\n-----------  Result of Unitary similarity transformation matrix  ----------')
             print("Unitary similarity transformation matrix for part "+str(i+1)+":")
             
             print(sp.Matrix(U_))
             
             print("\n")
-            print("Error:")
-            print("error for unitaryizing:", end=' ')
+            print("ERROR:")
+            print("ERROR for unitaryizing:", end=' ')
             #print(abs(U.conj().T@U-np.eye(band_num)).max())
             U__ = np.array(U_,dtype = np.complex128)
             
-            error = sum(abs(U__.conj().T@U__-np.eye(dimension))).sum()
-            print(error)
+            ERROR = sum(abs(U__.conj().T@U__-np.eye(dimension))).sum()
+            print(ERROR)
             
             #print(operator_.keys())
             for j in Symmetry.keys():
                 
-                print("error for "+j+":", end=' ')
+                print("ERROR for "+j+":", end=' ')
                 
                 if Symmetry[j]['repr_has_cc']:    
                     #print(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix'].evalf())).max())
                     try:
-                        error = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i].evalf()))).sum()
+                        ERROR = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i].evalf()))).sum()
                         
                     except:
                         
                         try:
-                            error = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).sum()
+                            ERROR = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).sum()
                         
                         except:
-                            error = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).evalf()
-                            error = abs(error)
+                            ERROR = sum(abs(U__.conj().T@operator_[j]@U__.conj()-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).evalf()
+                            ERROR = abs(ERROR)
                             
-                    print(error)
+                    print(ERROR)
                     
                 else:
                     #print(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix'].evalf())).max())
                     try:
-                        error = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i].evalf()))).sum()
+                        ERROR = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i].evalf()))).sum()
                         
                     except:
                         
                         try:
-                            error = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).sum()
+                            ERROR = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).sum()
                         
                         except:
-                            error = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).evalf()
-                            error = abs(error)
+                            ERROR = sum(abs(U__.conj().T@operator_[j]@U__-np.array(Symmetry[j]['band_repr_matrix_list'][i]))).evalf()
+                            ERROR = abs(ERROR)
                             
-                    print(error)
+                    print(ERROR)
                 
                 
                 
             if i==0: 
                 U = U_
                 
             else:
@@ -1279,73 +1312,74 @@
                 
             dimension_tot = dimension_tot_
             
         Symmetry = get_std_Symmetry(Symmetry)
         
     
     else:
-        
-        raise SymmetryError("There must be 'band_repr_matrix_list' or 'repr_matrix' keys!")
+        sys.stdout = save_stdout
+        print("ERROR: There must be 'band_repr_matrix_list' or 'repr_matrix' keys!")
+        #raise SymmetryERROR("There must be 'band_repr_matrix_list' or 'repr_matrix' keys!")
         sys.exit()
         
         
                 
     print("End finding similarity transformation")
     print("==================================================")
     
-    # calculate the error
+    # calculate the ERROR
     print('\n\n\n')
     print("==================================================")
     print('\n==========  Result of Unitary similarity transformation matrix  ==========')
     print("Unitary similarity transformation matrix:")
     print(sp.Matrix(U))
     print("\n")
-    print("Error:")
-    print("error for unitaryizing:", end=' ')
+    print("ERROR:")
+    print("ERROR for unitaryizing:", end=' ')
     #print(abs(U.conj().T@U-np.eye(band_num)).max())
     U = np.array(U,dtype = np.complex128)
     
-    error = sum(abs(U.conj().T@U-np.eye(band_num))).sum()
-    print(error)
+    ERROR = sum(abs(U.conj().T@U-np.eye(band_num))).sum()
+    print(ERROR)
     
     for i in Symmetry.keys():
         
-        print("error for "+i+":", end=' ')
+        print("ERROR for "+i+":", end=' ')
         
         if Symmetry[i]['repr_has_cc']:    
             #print(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix'].evalf())).max())
             try:
-                error = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix'].evalf()))).sum()
+                ERROR = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix'].evalf()))).sum()
                 
             except:
                 
                 try:
-                    error = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix']))).sum()
+                    ERROR = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix']))).sum()
                 
                 except:
-                    error = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix']))).evalf()
-                    error = abs(error)
+                    ERROR = sum(abs(U.conj().T@operator[i]@U.conj()-np.array(Symmetry[i]['repr_matrix']))).evalf()
+                    ERROR = abs(ERROR)
                     
-            print(error)
+            print(ERROR)
             
         else:
             #print(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix'].evalf())).max())
             try:
-                error = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix'].evalf()))).sum()
+                ERROR = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix'].evalf()))).sum()
                 
             except:
                 
                 try:
-                    error = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix']))).sum()
+                    ERROR = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix']))).sum()
                 
                 except:
-                    error = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix']))).evalf()
-                    error = abs(error)
+                    ERROR = sum(abs(U.conj().T@operator[i]@U-np.array(Symmetry[i]['repr_matrix']))).evalf()
+                    ERROR = abs(ERROR)
                     
-            print(error)
+            print(ERROR)
     
     print('\n\n\n')
     
     
     if log != 0:
         
         if flag:
@@ -1364,43 +1398,47 @@
         
     else:
         
         try: 
             pi_list=[data['pix'],data['piy'],data['piz']]
             
         except:
-            raise VASPMomentumMatrixError("The generalized momentum matrices' names got by vasp2mat should be 'Pix', 'Piy', 'Piz'! The vat_name in the input file INCAR.mat of vasp2mat should be 'Pi'!")
-            
+            #raise VASPMomentumMatrixERROR("The generalized momentum matrices' names got by vasp2mat should be 'Pix', 'Piy', 'Piz'! The vat_name in the input file INCAR.mat of vasp2mat should be 'Pi'!")
+            print("ERROR: The generalized momentum matrices' names got by vasp2mat should be 'Pix', 'Piy', 'Piz'! The vat_name in the input file INCAR.mat of vasp2mat should be 'Pi'!")
             sys.exit()
 
     if gfactor == 1:
         # put the input spin matrices into a list
         if 'sigz' in data.keys():
             sigma_list=[data['sigx'],data['sigy'],data['sigz']]
             
         else:
             
             try:
                 sigma_list=[data['Sigx'],data['Sigy'],data['Sigz']]
                 
             except:
-                raise VASPSpinMatrixError("The spin matrices' names got by vasp2mat should be 'sigx', 'sigy', 'sigz'! The 'vat_name' in the input file INCAR.mat of vasp2mat should be 'sig'!")
+                print("ERROR: The spin matrices' names got by vasp2mat should be 'sigx', 'sigy', 'sigz'! The 'vat_name' in the input file INCAR.mat of vasp2mat should be 'sig'!")
+                #raise VASPSpinMatrixERROR("The spin matrices' names got by vasp2mat should be 'sigx', 'sigy', 'sigz'! The 'vat_name' in the input file INCAR.mat of vasp2mat should be 'sig'!")
                 
                 sys.exit()
         
     else:    
         sigma_list=[]
     
     return pi_list,sigma_list,U,Symmetry
 ###############################################################################
 
 
 
 ###############################################################################
 if __name__ == "__main__":
+    A = sp.Matrix([[2, 0, 0, 0, 2, 0, 0, 0], [0, 2, 0, 0, 0, 2, 0, 0], [0, 0, 2, 0, 0, 0, 2, 0], [0, 0, 0, 2, 0, 0, 0, 2], [2, 0, 0, 0, 2, 0, 0, 0], [0, 2, 0, 0, 0, 2, 0, 0], [0, 0, 2, 0, 0, 0, 2, 0], [0, 0, 0, 2, 0, 0, 0, 2]])
+    get_block_dim(A)
+if False:
     from sympy import I
     Symmetry = {
 
     'C3z' : {
         'rotation_matrix': sp.Matrix([[-sp.Rational(1,2),-sp.sqrt(3)/2,0],
                                       [sp.sqrt(3)/2, -sp.Rational(1,2), 0],
                                       [0, 0, 1]]),
```

### Comparing `VASP2KP-1.0.2/VASP2KP/_standard_kp.py` & `VASP2KP-1.1.1/VASP2KP/_standard_kp.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 import subprocess
 import warnings
 
 #warnings.filterwarnings("ignore", category=sp.SymPyDeprecationWarning)
 
 ###############################################################################
 # Hidden parameter region
-error_flag = 0 # 0,1 or 2
+ERROR_flag = 0 # 0,1 or 2
 
 tol = {0:1e-4,  1:1e-3,  2:1e-2,  3:1e-1,  "Zeeman":1e-3}
 #tol = {0:0,  1:0,  2:0,  3:0,  "Zeeman":0}
 
 print_each_order_flag = False
 
 ###############################################################################
 
 
 
 ###############################################################################
-# define Error class(type)
-class NumericalStandardKpMatrixError(Exception):
+# define ERROR class(type)
+class NumericalStandardKpMatrixERROR(Exception):
     '''
     if the absolute value of the element of the numerical standard Hamiltonian whose value should be zero is larger than tol, 
-        raise this error
+        raise this ERROR
     '''
     pass
 
-class Error_FlagChooseError(Exception):
+class ERROR_FlagChooseERROR(Exception):
     '''
-    if the parameter error_flag is not in [0,1,2]: raise this error
+    if the parameter ERROR_flag is not in [0,1,2]: raise this ERROR
     '''
     pass
 
 
 class suppress_stdout_stderr(object):
     '''A context manager for doing a "deep suppression" of stdout and stderr in Python, i.e. will suppress all print, even if the print originates in acompiled C/Fortran sub-function.This will not suppress raised exceptions, since exceptions are printedto stderr just before a script exits, and after the context manager hasexited (at least, I think that is why it lets exceptions through).'''
     def __init__(self):
@@ -85,15 +85,15 @@
         the tuple of the object.
 
     Returns
     -------
     coe : list
         the value of the undetermined parameters.
     residuals : float
-        the error of the linear least squard method.
+        the ERROR of the linear least squard method.
 
     '''
     
     # transform the equation set to the matrix
     A, B = sp.linear_eq_to_matrix(eql, coe_sym)
     #coe, residuals, rank, singular_values = np.linalg.lstsq(np.array(A,dtype=complex), np.array(B,dtype=complex), rcond=None)
     
@@ -111,15 +111,15 @@
     
     # construct the new parameters matrix and value vector
     A_matrix=np.vstack([A_r,A_i])
     B_matrix=np.vstack([B_r,B_i])
     #print(A_matrix)
     #print(B_matrix)
     
-    # linear least squares method to get the parameters as well as error
+    # linear least squares method to get the parameters as well as ERROR
     coe, residuals, rank, singular_values = np.linalg.lstsq(A_matrix, B_matrix, rcond=None)
     
     return coe, residuals
 ###############################################################################
 
 
 
@@ -143,27 +143,27 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     coe_0, list
         the list of the values of the undetermined parameters.
     coe_0_sym, tuple
         the tuple of all the symbol variables of the undetermined parameters. The type of the element is 'sympy.core.symbol.Symbol'.
     sum_result_kpmodel_0, sympy.matrices.dense.MutableDenseMatrix
         the part of the analytical standard kp hamiltonian: terms without any the wave vector k.
-    error, float
-        the error of the linear least squares method.
+    ERROR, float
+        the ERROR of the linear least squares method.
     all_dif, float
         the sum of the absolute values of the numerical zero matrix elements.
 
     '''
     
     
     # define symbol variables of the undetermined paramters
@@ -191,53 +191,53 @@
     for i in range(dimension):
         
         for j in range(dimension):
             
             ele=sp.Eq(sum_kpmodel_0[i,j]-zeros_k[i,j],0)
             
             ###############################################################
-            # calculate the errors of the matrix elements whose theoretical value is zero
+            # calculate the ERRORs of the matrix elements whose theoretical value is zero
             if (ele is sp.false) or (ele is sp.true):
                 
-                # calculate error
+                # calculate ERROR
                 dif = abs(zeros_k[i,j])
                 all_dif += dif
                 
                 if dif > tol[0]:
                     
-                    if error_flag == 0:
+                    if ERROR_flag == 0:
                         pass
                     
-                    elif error_flag == 1:
-                        # raise an error
-                        raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                    elif ERROR_flag == 1:
+                        # raise an ERROR
+                        raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                         
                         return 
                     
-                    elif error_flag == 2:
+                    elif ERROR_flag == 2:
                         
                         if log == 1:
                             
                             if wrong_flag == 0:
-                                error_file = open("Matrix_error.log","a")
-                                error_file.write('\n\n==========  Error of 0-order kp model  ==========\n')
-                                error_file.write("VASP_element \t\t Difference\n")
-                                error_file.write(str(zeros_k[i,j])+'\t'+str(dif)+'\n')
+                                ERROR_file = open("Matrix_ERROR.log","a")
+                                ERROR_file.write('\n\n==========  ERROR of 0-order kp model  ==========\n')
+                                ERROR_file.write("VASP_element \t\t Difference\n")
+                                ERROR_file.write(str(zeros_k[i,j])+'\t'+str(dif)+'\n')
                                 wrong_flag = 1
                                 
                             else:
-                                error_file.write(str(zeros_k[i,j])+'\t'+str(dif)+'\n')
+                                ERROR_file.write(str(zeros_k[i,j])+'\t'+str(dif)+'\n')
                                 
                         else:
                             sys.stdout.flush()
                             tmp_stdout = sys.stdout
                             sys.stdout = sys.__stdout__
                             
                             if wrong_flag == 0:
-                                print('\n\n==========  Error of 0-order kp model  ==========')
+                                print('\n\n==========  ERROR of 0-order kp model  ==========')
                                 print("VASP_element \t\t Difference")
                                 print(str(zeros_k[i,j])+'\t'+str(dif))
                                 wrong_flag = 1
                             
                             else:
                                 print(str(zeros_k[i,j])+'\t'+str(dif))
                             
@@ -247,18 +247,18 @@
             
             eql.append(ele)
             
     if wrong_flag == 1:
         
         if log == 1:
             
-            error_file.write('---------- VASP matrix ----------\n')
-            error_file.write(str(sp.Matrix(zeros_k))+'\n')
-            error_file.write('---------- kp matrix ----------\n')
-            error_file.write(str(sum_kpmodel_0)+'\n')
+            ERROR_file.write('---------- VASP matrix ----------\n')
+            ERROR_file.write(str(sp.Matrix(zeros_k))+'\n')
+            ERROR_file.write('---------- kp matrix ----------\n')
+            ERROR_file.write(str(sum_kpmodel_0)+'\n')
         
         else:
             sys.stdout.flush()
             tmp_stdout = sys.stdout
             sys.stdout = sys.__stdout__
             
             print('---------- VASP matrix ----------')
@@ -266,46 +266,46 @@
             print('---------- kp matrix ----------')
             print(sum_kpmodel_0)
             
             sys.stdout.flush()
             sys.stdout = tmp_stdout
     
     if log == 1 and wrong_flag == 1:
-        error_file.close()
+        ERROR_file.close()
         
     if len(eql) == 0:
         return [],[],0,0,all_dif
     
     coe_0, residuals=get_coeff(eql,coe_0_sym)
-    error = residuals[0]
+    ERROR = residuals[0]
     
     ###########################################################################
     # output the result
     if print_each_order_flag and print_flag != 0:
         print("0-order kp Hamiltonian:")
         print(sum_kpmodel_0)
         print("Parameters:")
         
         for i in range(coe_0_num):
             coe_0[i][0] = round(coe_0[i][0].real,4)
             print(coe_0_sym[i],"=",coe_0[i][0].real,";")
             
-        error_print = "{:.2e}".format(error)
+        ERROR_print = "{:.2e}".format(ERROR)
         all_dif_print = "{:.2e}".format(all_dif)
         
-        print("Error of the linear least square method:",error_print)
+        print("Error of the linear least square method:",ERROR_print)
         print("Sum of absolute values of numerical zero elements:",all_dif_print)
         
     sum_result_kpmodel_0=sp.zeros(dimension)
     
     for i in range(len(kpmodel)):
         sum_result_kpmodel_0 = sum_result_kpmodel_0 + coe_0[i,0]*kpmodel[i]
 
     
-    return coe_0,coe_0_sym,sum_result_kpmodel_0,error,all_dif
+    return coe_0,coe_0_sym,sum_result_kpmodel_0,ERROR,all_dif
 ###############################################################################
 
 
 
 ###############################################################################
 def get_std_kp_1_order(kpmodel,linear_V2,print_flag=2,log=0):
     '''
@@ -326,27 +326,27 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     coe_1, list
         the list of the values of the undetermined parameters.
     coe_1_sym, tuple
         the tuple of all the symbol variables of the undetermined parameters. The type of the element is 'sympy.core.symbol.Symbol'.
     sum_result_kpmodel_1, sympy.matrices.dense.MutableDenseMatrix
         the part of the analytical standard kp hamiltonian: terms whose vector k are of 1 order.
-    error, float
-        the error of the linear least squares method.
+    ERROR, float
+        the ERROR of the linear least squares method.
     all_dif, float
         the sum of the absolute values of the numerical zero matrix elements.
 
     '''
     
     # define the symbol variables(constant)
     kx,ky,kz = sp.symbols("kx ky kz")
@@ -386,59 +386,59 @@
         for i in range(dimension):
             
             for j in range(dimension):
                 
                 ele=sp.Eq(tmp_sum_kpmodel_1[i,j]-linear_V2_part[i,j],0)
                 
                 ###############################################################
-                # calculate the errors of the matrix elements whose theoretical value is zero
+                # calculate the ERRORs of the matrix elements whose theoretical value is zero
                 if (ele is sp.false) or (ele is sp.true):
                     
                     dif = abs(linear_V2_part[i,j])
                     all_dif += dif
                     
                     if dif > tol[1]:
                         
-                        if error_flag == 0:
+                        if ERROR_flag == 0:
                             pass
                         
-                        elif error_flag == 1:
-                            raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                        elif ERROR_flag == 1:
+                            raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                             
                             return 
                         
-                        elif error_flag == 2:
+                        elif ERROR_flag == 2:
                             
                             if log == 1:
                                 
                                 if wrong_flag == 0:
-                                    error_file = open("Matrix_error.log","a")
-                                    error_file.write('\n\n==========  Error of 1-order kp model  ==========\n')
-                                    error_file.write('========== {} ==========\n'.format(char_k[ii]))
-                                    error_file.write("VASP_element \t\t Difference\n")
-                                    error_file.write(str(linear_V2_part)+'\t'+str(dif)+'\n')
+                                    ERROR_file = open("Matrix_ERROR.log","a")
+                                    ERROR_file.write('\n\n==========  ERROR of 1-order kp model  ==========\n')
+                                    ERROR_file.write('========== {} ==========\n'.format(char_k[ii]))
+                                    ERROR_file.write("VASP_element \t\t Difference\n")
+                                    ERROR_file.write(str(linear_V2_part)+'\t'+str(dif)+'\n')
                                     wrong_flag = 1
                                     wrong_flag_per = 1
                                     
                                 elif wrong_flag_per == 0:
-                                    error_file.write('\n========== {} ==========\n'.format(char_k[ii]))
-                                    error_file.write("VASP_element \t\t Difference\n")
-                                    error_file.write(str(linear_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                    ERROR_file.write('\n========== {} ==========\n'.format(char_k[ii]))
+                                    ERROR_file.write("VASP_element \t\t Difference\n")
+                                    ERROR_file.write(str(linear_V2_part[i,j])+'\t'+str(dif)+'\n')
                                     wrong_flag_per = 1
                                     
                                 else:
-                                    error_file.write(str(linear_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                    ERROR_file.write(str(linear_V2_part[i,j])+'\t'+str(dif)+'\n')
                                     
                             else:
                                 sys.stdout.flush()
                                 tmp_stdout = sys.stdout
                                 sys.stdout = sys.__stdout__
                                 
                                 if wrong_flag == 0:
-                                    print('\n\n==========  Error of 1-order kp model  ==========')
+                                    print('\n\n==========  ERROR of 1-order kp model  ==========')
                                     print('========== {} =========='.format(char_k[ii]))
                                     print("VASP_element \t\t Difference")
                                     print(str(linear_V2_part[i,j])+'\t'+str(dif))
                                     wrong_flag = 1
                                     wrong_flag_per = 1
                                 
                                 elif wrong_flag_per == 0:
@@ -456,18 +456,18 @@
                     continue
                 
                 eql.append(ele)
                 
         if wrong_flag_per == 1:
             
             if log == 1:
-                error_file.write('---------- VASP matrix for {} ----------\n'.format(char_k[ii]))
-                error_file.write(str(sp.Matrix(linear_V2_part))+'\n')
-                error_file.write('---------- kp matrix for {} ----------\n'.format(char_k[ii]))
-                error_file.write(str(tmp_sum_kpmodel_1))
+                ERROR_file.write('---------- VASP matrix for {} ----------\n'.format(char_k[ii]))
+                ERROR_file.write(str(sp.Matrix(linear_V2_part))+'\n')
+                ERROR_file.write('---------- kp matrix for {} ----------\n'.format(char_k[ii]))
+                ERROR_file.write(str(tmp_sum_kpmodel_1))
                 
             else:
                 sys.stdout.flush()
                 tmp_stdout = sys.stdout
                 sys.stdout = sys.__stdout__
                 
                 print('---------- VASP matrix for {} ----------'.format(char_k[ii]))
@@ -475,46 +475,46 @@
                 print('---------- kp matrix for {} ----------'.format(char_k[ii]))
                 print(tmp_sum_kpmodel_1)
                 
                 sys.stdout.flush()
                 sys.stdout = tmp_stdout
     
     if log == 1 and wrong_flag == 1:
-        error_file.close()
+        ERROR_file.close()
         
     if len(eql) == 0:
         return [],[],0,0,all_dif
     
     coe_1, residuals=get_coeff(eql,coe_1_sym)
-    error = residuals[0]
+    ERROR = residuals[0]
     
     ###########################################################################
     # output the result
     if print_each_order_flag and print_flag != 0:
         print("1-order kp Hamiltonian:")
         print(sum_kpmodel_1)
         print("Parameters:")
         
         for i in range(coe_1_num):
             coe_1[i][0] = round(coe_1[i][0].real,4)
             print(coe_1_sym[i],"=",coe_1[i][0].real,";")
             
-        error_print = "{:.2e}".format(error)
+        ERROR_print = "{:.2e}".format(ERROR)
         all_dif_print = "{:.2e}".format(all_dif)
             
-        print("Error of the linear least square method:",error_print)
+        print("Error of the linear least square method:",ERROR_print)
         print("Sum of absolute values of numerical zero elements:",all_dif_print)
         
     sum_result_kpmodel_1=sp.zeros(dimension)
     
     for i in range(len(kpmodel)):
         sum_result_kpmodel_1 = sum_result_kpmodel_1 + coe_1[i,0]*kpmodel[i]
         
         
-    return coe_1,coe_1_sym,sum_result_kpmodel_1,error,all_dif
+    return coe_1,coe_1_sym,sum_result_kpmodel_1,ERROR,all_dif
 ###############################################################################
 
 
 
 ###############################################################################
 def get_std_kp_2_order(kpmodel,quadratic_V2_symm,print_flag=2,log=0):
     '''
@@ -535,27 +535,27 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     coe_2, list
         the list of the values of the undetermined parameters.
     coe_2_sym, tuple
         the tuple of all the symbol variables of the undetermined parameters. The type of the element is 'sympy.core.symbol.Symbol'.
     sum_result_kpmodel_2, sympy.matrices.dense.MutableDenseMatrix
         the part of the analytical standard kp hamiltonian: terms whose vector k are of 2 order.
-    error, float
-        the error of the linear least squares method.
+    ERROR, float
+        the ERROR of the linear least squares method.
     all_dif, float
         the sum of the absolute values of the numerical zero matrix elements.
 
     '''
     
     
     # define the symbol variables(constant)
@@ -602,60 +602,60 @@
             for i in range(dimension):
                 
                 for j in range(dimension):
                     
                     ele=sp.Eq(tmp_sum_kpmodel_2[i,j]-quadratic_V2_part[i,j],0)
                     
                     ###############################################################
-                    # calculate the errors of the matrix elements whose theoretical value is zero
+                    # calculate the ERRORs of the matrix elements whose theoretical value is zero
                     if (ele is sp.false) or (ele is sp.true):
                         #print(abs(tmp_sum_kpmodel_2[i,j]-quadratic_V2_part[i,j]).evalf())
                         
                         dif = abs(quadratic_V2_part[i,j])
                         all_dif += dif
                         
                         if dif > tol[2]:
                             
-                            if error_flag == 0:
+                            if ERROR_flag == 0:
                                 pass
                             
-                            elif error_flag == 1:
-                                raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                            elif ERROR_flag == 1:
+                                raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                                 
                                 return 
                             
-                            elif error_flag == 2:
+                            elif ERROR_flag == 2:
                                 
                                 if log == 1:
                                     
                                     if wrong_flag == 0:
-                                        error_file = open("Matrix_error.log","a")
-                                        error_file.write('\n\n==========  Error of 2-order kp model  ==========\n')
-                                        error_file.write('========== {}{} ==========\n'.format(char_k[ii],char_k[jj]))
-                                        error_file.write("VASP_element \t\t Difference\n")
-                                        error_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                        ERROR_file = open("Matrix_ERROR.log","a")
+                                        ERROR_file.write('\n\n==========  ERROR of 2-order kp model  ==========\n')
+                                        ERROR_file.write('========== {}{} ==========\n'.format(char_k[ii],char_k[jj]))
+                                        ERROR_file.write("VASP_element \t\t Difference\n")
+                                        ERROR_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                         wrong_flag = 1
                                         wrong_flag_per = 1
                                         
                                     elif wrong_flag_per == 0:
-                                        error_file.write('\n========== {}{} ==========\n'.format(char_k[ii],char_k[jj]))
-                                        error_file.write("VASP_element \t\t Difference\n")
-                                        error_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                        ERROR_file.write('\n========== {}{} ==========\n'.format(char_k[ii],char_k[jj]))
+                                        ERROR_file.write("VASP_element \t\t Difference\n")
+                                        ERROR_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                         wrong_flag_per = 1
                                         
                                     else:
-                                        error_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                        ERROR_file.write(str(quadratic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                         
                                 else:
                                     tmp_stdout = sys.stdout
                                     sys.stdout.flush()
                                     sys.stdout = sys.__stdout__
                                     
                                     if wrong_flag == 0:
-                                        print('\n\n==========  Error of 2-order kp model  ==========')
+                                        print('\n\n==========  ERROR of 2-order kp model  ==========')
                                         print('========== {}{} =========='.format(char_k[ii],char_k[jj]))
                                         print("VASP_element \t\t Difference")
                                         print(str(quadratic_V2_part[i,j])+'\t'+str(dif))
                                         wrong_flag = 1
                                         wrong_flag_per = 1
                                     
                                     elif wrong_flag_per == 0:
@@ -672,18 +672,18 @@
                         continue
                     
                     eql.append(ele)
                     
             if wrong_flag_per == 1:
                 
                 if log == 1:
-                    error_file.write('---------- VASP matrix for {}{} ----------\n'.format(char_k[ii],char_k[jj]))
-                    error_file.write(str(sp.Matrix(quadratic_V2_part))+'\n')
-                    error_file.write('---------- kp matrix for {}{} ----------\n'.format(char_k[ii],char_k[jj]))
-                    error_file.write(str(tmp_sum_kpmodel_2)+'\n')
+                    ERROR_file.write('---------- VASP matrix for {}{} ----------\n'.format(char_k[ii],char_k[jj]))
+                    ERROR_file.write(str(sp.Matrix(quadratic_V2_part))+'\n')
+                    ERROR_file.write('---------- kp matrix for {}{} ----------\n'.format(char_k[ii],char_k[jj]))
+                    ERROR_file.write(str(tmp_sum_kpmodel_2)+'\n')
                 
                 else:
                     sys.stdout.flush()
                     tmp_stdout = sys.stdout
                     sys.stdout = sys.__stdout__
                     
                     print('---------- VASP matrix for {}{} ----------'.format(char_k[ii],char_k[jj]))
@@ -691,47 +691,47 @@
                     print('---------- kp matrix for {}{} ----------'.format(char_k[ii],char_k[jj]))
                     print(tmp_sum_kpmodel_2)
                     
                     sys.stdout.flush()
                     sys.stdout = tmp_stdout
                     
     if log == 1 and wrong_flag == 1:
-        error_file.close()
+        ERROR_file.close()
         
     if len(eql) == 0:
         return [],[],0,0,all_dif
     
     coe_2, residuals=get_coeff(eql,coe_2_sym)
     #print(coe_2)
     #print(residuals)
-    error = residuals[0]
+    ERROR = residuals[0]
     
     ###########################################################################
     # output the result
     if print_each_order_flag and print_flag != 0:
         print("2-order kp Hamiltonian:")
         print(sum_kpmodel_2)
         print("Parameters:")
         
         for i in range(coe_2_num):
             coe_2[i][0] = round(coe_2[i][0].real,4)
             print(coe_2_sym[i],"=",coe_2[i][0].real,";")
             
-        error_print = "{:.2e}".format(error)
+        ERROR_print = "{:.2e}".format(ERROR)
         all_dif_print = "{:.2e}".format(all_dif)
         
-        print("Error of the linear least square method:",error_print)
+        print("Error of the linear least square method:",ERROR_print)
         print("Sum of absolute values of numerical zero elements:",all_dif_print)
     
     sum_result_kpmodel_2=sp.zeros(dimension)
     
     for i in range(len(kpmodel)):
         sum_result_kpmodel_2 = sum_result_kpmodel_2 + coe_2[i,0]*kpmodel[i]
     
-    return coe_2,coe_2_sym,sum_result_kpmodel_2,error,all_dif
+    return coe_2,coe_2_sym,sum_result_kpmodel_2,ERROR,all_dif
 ###############################################################################
 
 
 
 ###############################################################################
 def get_std_kp_3_order(kpmodel,cubic_V2_symm,print_flag=2,log=0):
     '''
@@ -752,27 +752,27 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     coe_2, list
         the list of the values of the undetermined parameters.
     coe_2_sym, tuple
         the tuple of all the symbol variables of the undetermined parameters. The type of the element is 'sympy.core.symbol.Symbol'.
     sum_result_kpmodel_2, sympy.matrices.dense.MutableDenseMatrix
         the part of the analytical standard kp hamiltonian: terms whose vector k are of 2 order.
-    error, float
-        the error of the linear least squares method.
+    ERROR, float
+        the ERROR of the linear least squares method.
     all_dif, float
         the sum of the absolute values of the numerical zero matrix elements.
 
     '''
 
     
     # define the symbol variables(constant)
@@ -835,59 +835,59 @@
                 for i in range(dimension):
                     
                     for j in range(dimension):
                         
                         ele=sp.Eq(tmp_sum_kpmodel_3[i,j]-cubic_V2_part[i,j],0)
                         
                         ###############################################################
-                        # calculate the errors of the matrix elements whose theoretical value is zero
+                        # calculate the ERRORs of the matrix elements whose theoretical value is zero
                         if (ele is sp.false) or (ele is sp.true):
                             #print(abs(tmp_sum_kpmodel_3[i,j]-cubic_V2_part[i,j]).evalf())
                             dif = abs(cubic_V2_part[i,j])
                             all_dif += dif
                             
                             if dif > tol[3]:
                                 
-                                if error_flag == 0:
+                                if ERROR_flag == 0:
                                     pass
                                 
-                                elif error_flag == 1:
-                                    raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                                elif ERROR_flag == 1:
+                                    raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                                     
                                     return 
                                 
-                                elif error_flag == 2:
+                                elif ERROR_flag == 2:
                                     
                                     if log == 1:
                                         
                                         if wrong_flag == 0:
-                                            error_file = open("Matrix_error.log","a")
-                                            error_file.write('\n\n==========  Error of 3-order kp model  ==========\n')
-                                            error_file.write('========== {}{}{} ==========\n'.format(char_k[ii],char_k[jj],char_k[kk]))
-                                            error_file.write("VASP_element \t\t Difference\n")
-                                            error_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                            ERROR_file = open("Matrix_ERROR.log","a")
+                                            ERROR_file.write('\n\n==========  ERROR of 3-order kp model  ==========\n')
+                                            ERROR_file.write('========== {}{}{} ==========\n'.format(char_k[ii],char_k[jj],char_k[kk]))
+                                            ERROR_file.write("VASP_element \t\t Difference\n")
+                                            ERROR_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                             wrong_flag = 1
                                             wrong_flag_per = 1
                                             
                                         elif wrong_flag_per == 0:
-                                            error_file.write('\n========== {}{}{} ==========\n'.format(char_k[ii],char_k[jj],char_k[kk]))
-                                            error_file.write("VASP_element \t\t Difference\n")
-                                            error_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                            ERROR_file.write('\n========== {}{}{} ==========\n'.format(char_k[ii],char_k[jj],char_k[kk]))
+                                            ERROR_file.write("VASP_element \t\t Difference\n")
+                                            ERROR_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                             wrong_flag_per = 1
                                             
                                         else:
-                                            error_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
+                                            ERROR_file.write(str(cubic_V2_part[i,j])+'\t'+str(dif)+'\n')
                                             
                                     else:
                                         tmp_stdout = sys.stdout
                                         sys.stdout.flush()
                                         sys.stdout = sys.__stdout__
                                         
                                         if wrong_flag == 0:
-                                            print('\n\n==========  Error of 3-order kp model  ==========')
+                                            print('\n\n==========  ERROR of 3-order kp model  ==========')
                                             print('========== {}{}{} =========='.format(char_k[ii],char_k[jj],char_k[kk]))
                                             print("VASP_element \t\t Difference")
                                             print(str(cubic_V2_part[i,j])+'\t'+str(dif))
                                             wrong_flag = 1
                                             wrong_flag_per = 1
                                         
                                         elif wrong_flag_per == 0:
@@ -905,18 +905,18 @@
                             continue
                         
                         eql.append(ele)
                         
                 if wrong_flag_per == 1:
                     
                     if log == 1:
-                        error_file.write('---------- VASP matrix for {}{}{} ----------\n'.format(char_k[ii],char_k[jj],char_k[kk]))
-                        error_file.write(str(sp.Matrix(cubic_V2_part))+'\n')
-                        error_file.write('---------- kp matrix for {}{}{} ----------\n'.format(char_k[ii],char_k[jj],char_k[kk]))
-                        error_file.write(str(tmp_sum_kpmodel_3)+'\n')
+                        ERROR_file.write('---------- VASP matrix for {}{}{} ----------\n'.format(char_k[ii],char_k[jj],char_k[kk]))
+                        ERROR_file.write(str(sp.Matrix(cubic_V2_part))+'\n')
+                        ERROR_file.write('---------- kp matrix for {}{}{} ----------\n'.format(char_k[ii],char_k[jj],char_k[kk]))
+                        ERROR_file.write(str(tmp_sum_kpmodel_3)+'\n')
                     
                     else:
                         sys.stdout.flush()
                         tmp_stdout = sys.stdout
                         sys.stdout = sys.__stdout__
                         
                         print('---------- VASP matrix for {}{}{} ----------'.format(char_k[ii],char_k[jj],char_k[kk]))
@@ -924,45 +924,45 @@
                         print('---------- kp matrix for {}{}{} ----------'.format(char_k[ii],char_k[jj],char_k[kk]))
                         print(tmp_sum_kpmodel_3)
                         
                         sys.stdout.flush()
                         sys.stdout = tmp_stdout
     
     if log == 1 and wrong_flag == 1:
-        error_file.close()
+        ERROR_file.close()
         
     if len(eql) == 0:
         return [],[],0,0,all_dif
     
     coe_3, residuals=get_coeff(eql,coe_3_sym)
-    error = residuals[0]
+    ERROR = residuals[0]
     
     ###########################################################################
     # output the result
     if print_each_order_flag and print_flag != 0:
         print("3-order kp Hamiltonian:")
         print(sum_kpmodel_3)
         print("Parameters:")
         
         for i in range(coe_3_num):
             coe_3[i][0] = round(coe_3[i][0].real,4)
             print(coe_3_sym[i],"=",coe_3[i][0].real,";")
             
-        error_print = "{:.2e}".format(error)
+        ERROR_print = "{:.2e}".format(ERROR)
         all_dif_print = "{:.2e}".format(all_dif)
             
-        print("Error of the linear least square method:",error_print)
+        print("Error of the linear least square method:",ERROR_print)
         print("Sum of absolute values of numerical zero elements:",all_dif_print)
     
     sum_result_kpmodel_3 = sp.zeros(dimension)
     
     for i in range(len(kpmodel)):
         sum_result_kpmodel_3 = sum_result_kpmodel_3 + coe_3[i,0]*kpmodel[i]
     
-    return coe_3,coe_3_sym,sum_result_kpmodel_3,error,all_dif
+    return coe_3,coe_3_sym,sum_result_kpmodel_3,ERROR,all_dif
 ###############################################################################
 
 
 
 ###############################################################################        
 def get_Zeeman(Symmetry,msg_num,kvec,G_4c4,order = 0,print_flag = 2,log = 0):
     '''
@@ -987,34 +987,34 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    Error_FlagChooseError
-        If error_flag is not in [0,1,2]: raise this error.
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    ERROR_FlagChooseERROR
+        If ERROR_flag is not in [0,1,2]: raise this ERROR.
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     sum_result_kpmodel_g : sympy.matrices.dense.MutableDenseMatrix
         the effective Zeeman's coupling.
     Zeeman_coe : a dictionary
         keys: parameters' name, TYPE: sympy.core.symbol.Symbol
             You can use list(Zeeman_coe.keys()) to get the list of keys and then get the variable name.
         values: a list, 
             The zeroth element is the value of the parameters.
             The first element is the matrix of the independent Zeeman's coupling. 
 
     '''
     
-    if error_flag not in [0,1,2]:
-        raise Error_FlagChooseError("The parameter error_flag in _standard_kp must be in [0,1,2]!")
+    if ERROR_flag not in [0,1,2]:
+        raise ERROR_FlagChooseERROR("The parameter ERROR_flag in _standard_kp must be in [0,1,2]!")
         
         sys.exit(0)
     
     # define the symbol variables(constant)
     Bx,By,Bz = sp.symbols("Bx By Bz")
     variable_list = sp.symbols("Bx By Bz")
     Bx_,By_,Bz_= sp.symbols("B_x B_y B_z",commutative = False)
@@ -1222,67 +1222,67 @@
         for i in range(dimension):
             
             for j in range(dimension):
                 
                 ele = sp.Eq(tmp_sum_kpmodel_g[i,j]-G_4c4_part[i,j],0)
                 
                 ###############################################################
-                # calculate the errors of the matrix elements whose theoretical value is zero
+                # calculate the ERRORs of the matrix elements whose theoretical value is zero
                 if (ele is sp.false) or (ele is sp.true):
-                    # calculate the error
+                    # calculate the ERROR
                     dif = abs(G_4c4_part[i,j])
                     all_dif += dif
                     
                     if dif > tol["Zeeman"]:
                         
-                        if error_flag == 0:
+                        if ERROR_flag == 0:
                             pass
                         
-                        elif error_flag == 1:
+                        elif ERROR_flag == 1:
                             sys.stdout = save_stdout
                             
                             if log == 1:
                                 logging.close()
                             
                             if print_flag == 2:
                                 outfile.close()
                             
-                            raise NumericalStandardKpMatrixError("The numerical Zeeman's coupling and the analytical Zeeman's coupling do not match!")
+                            raise NumericalStandardKpMatrixERROR("The numerical Zeeman's coupling and the analytical Zeeman's coupling do not match!")
                             
                             sys.exit()
                             
-                        elif error_flag == 2:
+                        elif ERROR_flag == 2:
                             
                             if log == 1:
                                 
                                 if wrong_flag == 0:
-                                    error_file = open("Matrix_error.log","a")
-                                    error_file.write('\n\n==========  Error of Zeeman\'s coupling matrix  ==========\n')
-                                    error_file.write('========== {} ==========\n'.format(char_B[ii]))
-                                    error_file.write("VASP_element \t\t Difference\n")
-                                    error_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
+                                    ERROR_file = open("Matrix_ERROR.log","a")
+                                    ERROR_file.write('\n\n==========  ERROR of Zeeman\'s coupling matrix  ==========\n')
+                                    ERROR_file.write('========== {} ==========\n'.format(char_B[ii]))
+                                    ERROR_file.write("VASP_element \t\t Difference\n")
+                                    ERROR_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
                                     wrong_flag = 1
                                     wrong_flag_per = 1
                                     
                                 elif wrong_flag_per == 0:
-                                    error_file.write('\n========== {} ==========\n'.format(char_B[ii]))
-                                    error_file.write("VASP_element \t\t Difference\n")
-                                    error_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
+                                    ERROR_file.write('\n========== {} ==========\n'.format(char_B[ii]))
+                                    ERROR_file.write("VASP_element \t\t Difference\n")
+                                    ERROR_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
                                     wrong_flag_per = 1
                                     
                                 else:
-                                    error_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
+                                    ERROR_file.write(str(G_4c4_part[i,j])+'\t'+str(dif)+'\n')
                                     
                             else:
                                 tmp_stdout = sys.stdout
                                 sys.stdout.flush()
                                 sys.stdout = save_stdout
                                 
                                 if wrong_flag == 0:
-                                    print('\n\n==========  Error of Zeeman\'s coupling matrix  ==========')
+                                    print('\n\n==========  ERROR of Zeeman\'s coupling matrix  ==========')
                                     print('========== {} =========='.format(char_B[ii]))
                                     print("VASP_element \t\t Difference")
                                     print(str(G_4c4_part[i,j])+'\t'+str(dif))
                                     wrong_flag = 1
                                     wrong_flag_per = 1
                                 
                                 elif wrong_flag_per == 0:
@@ -1301,18 +1301,18 @@
                     continue
                 
                 eql.append(ele)
                 
         if wrong_flag_per == 1:
             
             if log == 1:
-                error_file.write('---------- VASP matrix for {} ----------\n'.format(char_B[ii]))
-                error_file.write(str(sp.Matrix(G_4c4_part))+'\n')
-                error_file.write('---------- Zeeman\'s coupling matrix for {} ----------\n'.format(char_B[ii]))
-                error_file.write(str(tmp_sum_kpmodel_g)+'\n')
+                ERROR_file.write('---------- VASP matrix for {} ----------\n'.format(char_B[ii]))
+                ERROR_file.write(str(sp.Matrix(G_4c4_part))+'\n')
+                ERROR_file.write('---------- Zeeman\'s coupling matrix for {} ----------\n'.format(char_B[ii]))
+                ERROR_file.write(str(tmp_sum_kpmodel_g)+'\n')
                 
             else:
                 sys.stdout.flush()
                 tmp_stdout = sys.stdout
                 sys.stdout = sys.__stdout__
                 
                 print('---------- VASP matrix for {}----------'.format(char_B[ii]))
@@ -1358,24 +1358,24 @@
             try:
                 import platform
                 
                 system = platform.system()
                 
                 if system == 'Windows':
                     if order !=0:
-                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian-Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian-Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                         
                     else:
-                        pdf_flag = subprocess.run(r"pdflatex Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                         
                 else:
                     if order !=0:
-                        pdf_flag = subprocess.run("pdflatex kp_Hamiltonian-Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run("pdflatex kp_Hamiltonian-Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     else:
-                        pdf_flag = subprocess.run("pdflatex Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run("pdflatex Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                         
                 if pdf_flag.returncode == 0:
                     
                     try:
                         os.remove(texfile_name+".log")
                         os.remove(texfile_name+".aux")
                         os.remove(texfile_name+".out")
@@ -1397,25 +1397,25 @@
         if log == 0:
             logging.close()
         
         if log == 1:
             logging.close()
             
             if wrong_flag == 1:
-                error_file.close()
+                ERROR_file.close()
         
         sys.stdout = save_stdout
         
         return 0,dict()
     
     
     
     # calculate equations by the linear least squares method
     coe_g, residuals=get_coeff(eql,coe_g_sym)
-    error = residuals[0]
+    ERROR = residuals[0]
     
     ###########################################################################
     # output the result
      
         
     if print_flag != 0:
         print("Zeeman\'s coupling")
@@ -1425,18 +1425,18 @@
         print("Parameters:")
         
         # write to a .out file or print to screen
         for i in range(coe_g_num):
             coe_g[i][0]=round(coe_g[i][0].real,4)*2
             print(coe_g_sym[i],"=",coe_g[i][0].real,";")
             
-        error_print = "{:.2e}".format(error)
+        ERROR_print = "{:.2e}".format(ERROR)
         all_dif_print = "{:.2e}".format(all_dif)
         
-        print("Error of the linear least square method:",error_print)
+        print("Error of the linear least square method:",ERROR_print)
         print("Sum of absolute values of numerical zero elements:",all_dif_print)
         
         if print_flag == 2:
             
             # write to a .tex source file
             if order == 0:
                 texfile_name = "Zeeman's_coupling"
@@ -1500,24 +1500,24 @@
                 
                 import platform
                 
                 system = platform.system()
                 
                 if system == 'Windows':
                     if order !=0:
-                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian-Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian-Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     else:
-                        pdf_flag = subprocess.run(r"pdflatex Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex Zeeman's_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                         
                 else:
                     if order!=0:
-                        pdf_flag = subprocess.run("pdflatex kp_Hamiltonian-Zeeman\\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run("pdflatex kp_Hamiltonian-Zeeman\\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     
                     else:
-                        pdf_flag = subprocess.run(r"pdflatex Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex Zeeman\'s_coupling.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     
                 #delete the compile log
                 if pdf_flag.returncode == 0:
                     
                     try:
                         os.remove(texfile_name+".log")
                         os.remove(texfile_name+".aux")
@@ -1543,15 +1543,15 @@
     if log == 0:
         logging.close()
     
     if log == 1:
         logging.close()
         
         if wrong_flag == 1:
-            error_file.close()
+            ERROR_file.close()
         
     if print_flag == 2:
         outfile.close()
         
     sys.stdout = save_stdout
     
     return sum_result_kpmodel_g,Zeeman_coe
@@ -1587,18 +1587,18 @@
         If log == 0, there will be no .log file.
         If log == 1, there will be log files containing the result of finding the similarity transformation matrices,
                                                         the independent of each order as well as some warnings.
         The default is 0.
 
     Raises
     ------
-    Error_FlagChooseError
-        If error_flag is not in [0,1,2]: raise this error.
-    NumericalStandardKpMatrixError
-        If the error is larger than tol and error_flag is set to be 1, raise this error(error too large)
+    ERROR_FlagChooseERROR
+        If ERROR_flag is not in [0,1,2]: raise this ERROR.
+    NumericalStandardKpMatrixERROR
+        If the ERROR is larger than tol and ERROR_flag is set to be 1, raise this ERROR(ERROR too large)
 
     Returns
     -------
     result_kp_array : sympy.matrices.dense.MutableDenseMatrix
         the effective kp model(the sum of the effective kp models of each order as well as their parameters).
     kpmodel_coe : a dictionary
         keys: parameters' name, TYPE: sympy.core.symbol.Symbol
@@ -1606,25 +1606,26 @@
         values: a list, 
             The zeroth element is the value of the parameters.
             The first element is the matrix of the independent kp hamiltonian. 
 
     '''
     
     # simple judgement
-    if error_flag not in [0,1,2]:
-        raise Error_FlagChooseError("The parameter error_flag in _standard_kp must be in [0,1,2]!")
+    if ERROR_flag not in [0,1,2]:
+        print("The parameter ERROR_flag in _standard_kp must be in [0,1,2]!")
+        #raise ERROR_FlagChooseERROR("The parameter ERROR_flag in _standard_kp must be in [0,1,2]!")
         
         sys.exit(0)
     
     # update log file
-    if error_flag == 2:
+    if ERROR_flag == 2:
         file_list = os.listdir()
         
-        if "Matrix_error.log" in file_list:
-            os.remove("Matrix_error.log")
+        if "Matrix_ERROR.log" in file_list:
+            os.remove("Matrix_ERROR.log")
     
     save_stdout = sys.stdout
     
     order_list = [ [i] for i in range(order+1) ]
     sym_ops = list(Symmetry.values()) # kdotp-generator input parameter
     dimension=sym_ops[0]['repr_matrix'].shape[0]
     result_kp_array = sp.zeros(dimension)
@@ -1775,31 +1776,32 @@
                 coe_0,coe_0_sym,sum_result_kpmodel_0,res0,all_dif0 = get_std_kp_0_order(kpmodel,eigen_trans,print_flag,log)
                 all_dif += all_dif0
                 sys.stdout.flush()
                 
                 # cannot find any analytical kp
                 if len(coe_0) == 0:
                     
+                    print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     if print_each_order_flag:
                         
                         all_dif0_print = "{:.2e}".format(all_dif0)
                         print("No symmetry-allowed kp models.")
                         print("Sum of absolute values of numerical zero elements:",all_dif0_print)
-                    
+                        #print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     continue
                 
             except:
                 sys.stdout = save_stdout
                 
                 if print_flag == 2:
                     outfile.close()
                     
                 logging.close()
                 
-                raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                 sys.exit()
                 
             #result_kp.append(sum_result_kpmodel_0)
             result_kp_array = result_kp_array + sum_result_kpmodel_0
             result_res += res0
             all_dif += all_dif0
             
@@ -1830,31 +1832,31 @@
                 sys.stdout.flush()
                 coe_1,coe_1_sym,sum_result_kpmodel_1,res1,all_dif1 = get_std_kp_1_order(kpmodel,linear_V2,print_flag,log)
                 all_dif += all_dif1
                 sys.stdout.flush()
                 
                 # cannot find any analytical kp
                 if len(coe_1) == 0:
-                    
+                    print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     if print_each_order_flag:
                         print("No symmetry-allowed kp models.")
                         all_dif1_print = "{:.2e}".format(all_dif1)
                         print("Sum of absolute values of numerical zero elements:",all_dif1_print)
-                    
+                        
                     continue
                 
             except:
                 sys.stdout = save_stdout
                 
                 if print_flag == 2:
                     outfile.close()
                     
                 logging.close()
                 
-                raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                 sys.exit()
                 
             #result_kp.append(sum_result_kpmodel_1)
             result_kp_array = result_kp_array + sum_result_kpmodel_1
             result_res += res1
             
             variable_basis = []
@@ -1923,31 +1925,32 @@
                 sys.stdout.flush()
                 coe_2,coe_2_sym,sum_result_kpmodel_2,res2,all_dif2 = get_std_kp_2_order(kpmodel,quadratic_V2_symm,print_flag,log)
                 all_dif += all_dif2
                 sys.stdout.flush()
                 
                 # cannot find any analytical kp
                 if len(coe_2) == 0:
-                    
-                    all_dif2_print = "{:.2e}".format(all_dif2)
-                    print("No symmetry-allowed kp models.")
-                    print("Sum of absolute values of numerical zero elements:",all_dif2_print)
-                    
+                    print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
+                    if print_each_order_flag:
+                        all_dif2_print = "{:.2e}".format(all_dif2)
+                        print("No symmetry-allowed kp models.")
+                        print("Sum of absolute values of numerical zero elements:",all_dif2_print)
+                        print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     continue
                 
             except:
                 
                 sys.stdout = save_stdout
                 
                 if print_flag == 2:
                     outfile.close()
                     
                 logging.close()
                 
-                raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                 sys.exit()
                 
             #result_kp.append(sum_result_kpmodel_2)
             result_kp_array = result_kp_array + sum_result_kpmodel_2
             result_res += res2
             
             variable_basis = []
@@ -2019,33 +2022,33 @@
                 sys.stdout.flush()
                 coe_3,coe_3_sym,sum_result_kpmodel_3,res3,all_dif3 = get_std_kp_3_order(kpmodel,cubic_V2_symm,print_flag,log)
                 all_dif += all_dif3
                 sys.stdout.flush()
                 
                 # cannot find any analytical kp
                 if len(coe_3) == 0:
-                    
+                    print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     if print_each_order_flag:
                         
                         all_dif3_print = "{:.2e}".format(all_dif3)
                         print("No symmetry-allowed kp models.")
                         print("Sum of absolute values of numerical zero elements:",all_dif3_print)
-                    
+                        print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
                     continue
             
             except:
                 sys.stdout = save_stdout
                 
                 if print_flag == 2:
                     outfile.close()
                     
                 if log != 0:
                     logging.close()
                     
-                raise NumericalStandardKpMatrixError("The numerical kp model and the analytical kp model do not match!")
+                raise NumericalStandardKpMatrixERROR("The numerical kp model and the analytical kp model do not match!")
                 
                 sys.exit()
                 
             #result_kp.append(sum_result_kpmodel_3)
             result_kp_array = result_kp_array + sum_result_kpmodel_3
             result_res += res3
             
@@ -2105,14 +2108,17 @@
             
             for i in range(len(coe_3)):
                 kpmodel_coe[coe_3_sym[i]]=[coe_3[i,0],kpmodel[i],irrep_expr_basis[i],irrep_repr_basis[i]]
                 
                 if print_flag != 0:
                     result_kp_no_coe += coe_3_sym[i]*kpmodel[i]
                     result_kp_no_coe_tex += coe_3_sym[i]*kpmodel_tex[i]
+        
+        #sys.stdout = save_stdout
+        print("Finish constructing kp invariant Hamiltonian of order "+str(order[0])+"!",file = save_stdout)
          
     ###########################################################################
     # output the result
     
     #print(sp.simplify(result_kp_no_coe_tex.subs(kx_,kx).subs(ky_,ky).subs(kz_,kz)-result_kp_no_coe))
     if print_each_order_flag:
         print("\n\n\nkp Hamiltonian")
@@ -2218,18 +2224,18 @@
                 # if the system has the command 'pdflatex': compile the .tex
                 try:
                     import platform
                 
                     system = platform.system()
                     
                     if system == 'Windows':
-                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run(r"pdflatex kp_Hamiltonian.tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     
                     else:
-                        pdf_flag = subprocess.run("pdflatex "+texfile_name+".tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                        pdf_flag = subprocess.run("pdflatex "+texfile_name+".tex", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True,timeout=10)
                     #print(pdf_flag)
                     
                     #delete the compile log
                     if pdf_flag.returncode == 0:
                         
                         try:
                             os.remove(texfile_name+".log")
```

### Comparing `VASP2KP-1.0.2/VASP2KP/_transform_matrix.py` & `VASP2KP-1.1.1/VASP2KP/_transform_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 import sympy as sp
 #import random
 #import numba
 
 
 
 ###############################################################################
-class CoRepresentationInequivalenceError(Exception):
+class CoRepresentationInequivalenceERROR(Exception):
     '''
     the VASP corepresentation are not equivalent to the standard corepresentation
-    if traces of the corepresentation are not equal: raise this error
+    if traces of the corepresentation are not equal: raise this ERROR
     '''
     pass
 ###############################################################################
 
 
 
 ###############################################################################
@@ -73,15 +73,15 @@
     is_TRS : bool, optional
         if there is an antiunitary element. The default is False.
     Tmat : np.array((2,d,d)), optional
         Anti-unitary element. The default is None.
         Tmat[0,:,:]: A^{(i)}
         Tmat[1,:,:]: D^{(i)}
     tol : float, optional
-        Tolerance error. The default is 1e-9.
+        Tolerance ERROR. The default is 1e-9.
 
     Returns
     -------
     ns_mat, np.array
         similarity transformation matrix
     cn, integer
         the number of columns
@@ -99,15 +99,15 @@
     if trace_judge:
         
         for i in range(unitary_len):
             trace_dif = abs(np.trace(matrix_in1[i,:])-np.trace(matrix_in2[i,:]))
             # if the trace are not equal, the corepresentations are not equivelent
             if trace_dif > max(tol,5e-3):
                 
-                raise CoRepresentationInequivalenceError("The standard representation is not equivalent to VASP representation!(traces error)")
+                raise CoRepresentationInequivalenceERROR("The standard representation is not equivalent to VASP representation!(traces ERROR)")
                 sys.exit()
     
     if dim == 1:
         
         if is_TRS:
             m1 = Tmat[0,0,0]
             m2 = Tmat[1,0,0]
@@ -330,15 +330,15 @@
         #coe = sp.symbols('b0:{}'.format(num))
         #total_mat = 0
         
         
         import random
         print("Start unitaryzing procedure")
         print("==================================================")
-        print("Errors in the optimization process (unitaryizing the similarity transformation matrix)")
+        print("ERRORs in the optimization process (unitaryizing the similarity transformation matrix)")
         
         basis = []
         
         for i in range(num):
             basis.append(colC[:,i].reshape((dim,dim)))
         
         for tmp in range(30):
@@ -376,35 +376,35 @@
             
             
             
             opt_num = 1 # Number of optimization steps, nonlocal
             
             #@numba.njit
             def loss(coe_num):
-                # define the loss function (error)
+                # define the loss function (ERROR)
                 tmp_matrix = 0
                 
                 for i in range(len(coe_num)):
                     tmp_matrix += coe_num[i]*basis[i]
                     
                 #print(abs((tmp_matrix.H@tmp_matrix-sp.eye(tmp_matrix.shape[0]).evalf())))
                 min_mat = tmp_matrix.T.conj()@tmp_matrix
                 min_val = sum(abs((min_mat-np.eye(tmp_matrix.shape[0]))))
                 #min_val = sum(abs((min_mat-np.eye(tmp_matrix.shape[0])))**2)
                 
                 nonlocal opt_num
                 
-                print("steps_num:",opt_num,';',"error:",sum(min_val))
+                print("steps_num:",opt_num,';',"ERROR:",sum(min_val))
                 
                 opt_num += 1
                 
                 return sum(min_val)
             
             
-            #error = []
+            #ERROR = []
             #tol = 1e-5
             #construct the tolerence limit
             constraints=({'type':'ineq','fun':lambda x:tol - loss(x)})
             
             #find the unitary
             result = minimize(loss, coe_num, method='SLSQP',constraints=constraints)
             #result = minimize(loss, coe_num, method='TNC',constraints=constraints)
@@ -426,15 +426,15 @@
                 print("End")
                 print("==================================================")
                 
                 return U
             
         else:
             #print(result.x)
-            raise ValueError('Fail to find unitary U!')
+            raise ValueERROR('Fail to find unitary U!')
         
 
     
     #print(ns.shape)
     _,cn = ns.shape
     
     ### vec in ns: {real,imag} ,dim = 2*row
@@ -463,15 +463,15 @@
     operator : dictionary
         VASP corepresentation
     Symmetry : dictionary
         Users' input. The standard corepresentation and rotation matrix.
     band_num : integer
         The total number of the bands which we are interested in.
     tol : float, optional
-        Tolerance error. The default is 1e-9.
+        Tolerance ERROR. The default is 1e-9.
 
     Returns
     -------
     U : np.matrix
         the similarity transformation matrix between DFT representation and the standard representation
 
     """
```

### Comparing `VASP2KP-1.0.2/VASP2KP.egg-info/PKG-INFO` & `VASP2KP-1.1.1/VASP2KP.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.0.2
+Version: 1.1.1
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.0.2/mat2kp` & `VASP2KP-1.1.1/mat2kp`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!python
+#!/Users/shengzhang/anaconda3/bin/python
 # -*- coding: utf-8 -*-
 """
 Created on Sun Aug 20 19:30:07 2023
 Last modified on Wedn Dec 6 14:45:00 2023
 
 @author: Sheng Zhang, Institute of Physics, Chinese Academy of Sciences
 
@@ -174,17 +174,36 @@
     
     if 'kpmodel' in locals_key_low:
         kpmodel_id = locals_key_low.index('kpmodel')
         kpmodel = eval(locals_key[kpmodel_id])
         
     else:
         kpmodel = 1
+     
+if 'vmat_k' not in locals_key:
+    
+    if 'vmat_k' in locals_key_low:
+        vmat_k_id = locals_key_low.index('vmat_k')
+        vmat_k = eval(locals_key[vmat_k_id])
         
-        
+    else:
+        vmat_k = 1
     
+if 'repr_split' not in locals_key:
+    if 'repr_split' in locals_key_low:
+        repr_split_id = locals_key_low.index('repr_split')
+        repr_split = eval(locals_key[repr_split_id])
+        
+    else:
+        repr_split = True
+        
+        
+        
+        
+        
 '''    
 if 'folder_path' not in locals_key:
     
     if 'folder_path' in locals_key_low:
         folder_path_id = locals_key_low.index('folder_path')
         folder_path = eval(locals_key[folder_path_id])
         
@@ -209,22 +228,28 @@
 
 
 elif print_flag == 1:
     print(r"Warning!!! Parameter 'print_flag' is set to 1, all the result will be output on console, not into files!")
     
     
 # calculate the result
-if no_vasp_kp:
-    result_kp, result_Zeeman = \
-    get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log)
+try:
+    if no_vasp_kp:
+        result_kp, result_Zeeman = \
+        get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, vmat_k = vmat_k,repr_split = repr_split)
+    
+    else:
+        result_kp, result_Zeeman = \
+        get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, vmat_k = vmat_k,repr_split = repr_split)
+
+except:
+    pass
 
 else:
-    result_kp, result_Zeeman = \
-    get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc)
-    
+    print("Congratulations! The computation of VASP2KP has finished!!!")
 
 
 if gfactor == 1 and (not no_vasp_kp) and mathematica_flag:
     mathematica_file = open("kp-Zeeman.nb",'w')
     mathematica_file.write(r'Clear["Global`*"];')
     mathematica_file.write('\n')
     kp_string = str(sp.simplify(result_kp.evalf()))
```

### Comparing `VASP2KP-1.0.2/setup.py` & `VASP2KP-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Aug 21 15:54:57 2023
-Last modified on Wedn Dec 6 14:45:00 2023
+Last modified on Fri Apr 12 14:45:00 2024
 
 @author: Sheng Zhang, Institute of Physics, Chinese Academy of Sciences
 
 Set up VASP2KP
 """
 
 
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 README = """A tool for computing k.p effective Hamiltonians and Zeeman's coupling under given symmetry constraints from VASP calculations."""
 
 
 setup(name='VASP2KP',
       python_requires=">=3.6",
-      version = "1.0.2",
+      version = "1.1.1",
       long_description=README,
       install_requires=[
         'sympy', 'numpy', 'scipy', 'kdotp_generator'
         ],
       packages=['VASP2KP'],
       author = 'Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang',
       author_email='zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn',
```

### Comparing `VASP2KP-1.0.2/vasp2mat.5.3-patch-1.0.1.sh` & `VASP2KP-1.1.1/vasp2mat.5.3-patch-1.0.1.sh`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.0.2/vasp2mat.6.4-patch-1.0.1.sh` & `VASP2KP-1.1.1/vasp2mat.6.4-patch-1.0.1.sh`

 * *Files identical despite different names*

