# Comparing `tmp/tred-0.1.2.tar.gz` & `tmp/tred-0.1.3.tar.gz`

## Comparing `tred-0.1.2.tar` & `tred-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.2/requirements.txt
--rw-r--r--   0        0        0    18447 2020-02-02 00:00:00.000000 tred-0.1.2/examples/basic.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_m_transforms.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_tensor_ops.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_tensor_pca.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tred-0.1.2/tred/__init__.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_m_transforms.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_tensor_ops.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_tensor_pca.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_utils.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.2/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.2/LICENSE
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.2/README.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.3/README.txt
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.3/requirements.txt
+-rw-r--r--   0        0        0    18850 2020-02-02 00:00:00.000000 tred-0.1.3/examples/basic.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.3/tests/test_m_transforms.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.3/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0     6510 2020-02-02 00:00:00.000000 tred-0.1.3/tests/test_tensor_pca.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tred-0.1.3/tred/__init__.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tred-0.1.3/tred/_m_transforms.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 tred-0.1.3/tred/_tensor_ops.py
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 tred-0.1.3/tred/_tensor_pca.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 tred-0.1.3/tred/_utils.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.3/LICENSE
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tred-0.1.3/pypi.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tred-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tred-0.1.3/PKG-INFO
```

### Comparing `tred-0.1.2/examples/basic.ipynb` & `tred-0.1.3/examples/basic.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896335891812865%*

 * *Differences: {"'cells'": "{18: {'execution_count': 12, 'outputs': {0: {'execution_count': 12}}}, 20: "*

 * *            "{'execution_count': 13}, 22: {'execution_count': 14}, 25: {'execution_count': 15, "*

 * *            "'outputs': {0: {'traceback': {insert: [(2, 'Cell \\x1b[1;32mIn[15], line "*

 * *            '2\\x1b[0m\\n\\x1b[0;32m      1\\x1b[0m \\x1b[38;5;66;03m# '*

 * *            'ERROR\\x1b[39;00m\\n\\x1b[1;32m----> 2\\x1b[0m X_transformed_1 '*

 * *            '\\x1b[38;5;241m=\\x1b[39m '*

 * *            "\\x1b[43mtpca\\x1b[49m\\x1b[38;5 […]*

```diff
@@ -240,31 +240,48 @@
                 "assert_allclose(X_reconstructed, X)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "__UPDATE__!: If you have ```tred.__version__ >= \"0.1.3\"```, you can do the following..."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "X_reconstructed2 = tred.m_product(U, S, Vt)\n",
+                "assert_allclose(X_reconstructed2, X)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Notice how the last column of `S` is all zeroes. This means that some of the\n",
                 "`V` tensor is redundant. We can pass in `full_frontal_slices=False` to only\n",
                 "return us the necessary elements in the tensor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "((3, 3, 2), (3, 3, 2), (4, 3, 2))"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "U2, S2, V2 = tred.tsvdm(X, full_frontal_slices=False)\n",
                 "\n",
@@ -277,15 +294,15 @@
             "source": [
                 "Sense check that we have not 'loss' any information, and we can still \n",
                 "fully reconstruct our original tensor"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "V2t = V2.transpose(1, 0, 2)\n",
                 "X_reconstructed2 = reduce(m_product_wrapper, (U2, S2, V2t))\n",
                 "assert_allclose(X_reconstructed2, X)"
             ]
@@ -296,15 +313,15 @@
             "source": [
                 "## TPCA unsupervised tensor dimensionality reduction algorithm\n",
                 "Now, let's use the tensor decomposition using the `tpca` object. Revise some basics of object oriented programming and scikit-learn's interface if you are coming from R."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# first, create a transformer object\n",
                 "tpca = tred.TPCA()"
             ]
         },
@@ -322,40 +339,41 @@
                 "1. You explicitly fit your tpca object _first_, and then transform your data.\n",
                 "\n",
                 "Let's see what happens if you call `transform` _before_ `fit`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "NotFittedError",
                     "evalue": "This TPCA instance is not fitted yet. Call 'fit' with appropriate arguments before using this estimator.",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[1;31mNotFittedError\u001b[0m                            Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[14], line 2\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[38;5;66;03m# ERROR\u001b[39;00m\n\u001b[1;32m----> 2\u001b[0m X_transformed_1 \u001b[38;5;241m=\u001b[39m \u001b[43mtpca\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mtransform\u001b[49m\u001b[43m(\u001b[49m\u001b[43mX\u001b[49m\u001b[43m)\u001b[49m\n",
+                        "Cell \u001b[1;32mIn[15], line 2\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[38;5;66;03m# ERROR\u001b[39;00m\n\u001b[1;32m----> 2\u001b[0m X_transformed_1 \u001b[38;5;241m=\u001b[39m \u001b[43mtpca\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mtransform\u001b[49m\u001b[43m(\u001b[49m\u001b[43mX\u001b[49m\u001b[43m)\u001b[49m\n",
                         "File \u001b[1;32mc:\\Users\\brend\\OneDrive\\Documents\\GITHUB STUFF\\tred\\.venv\\lib\\site-packages\\sklearn\\utils\\_set_output.py:157\u001b[0m, in \u001b[0;36m_wrap_method_output.<locals>.wrapped\u001b[1;34m(self, X, *args, **kwargs)\u001b[0m\n\u001b[0;32m    155\u001b[0m \u001b[38;5;129m@wraps\u001b[39m(f)\n\u001b[0;32m    156\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mwrapped\u001b[39m(\u001b[38;5;28mself\u001b[39m, X, \u001b[38;5;241m*\u001b[39margs, \u001b[38;5;241m*\u001b[39m\u001b[38;5;241m*\u001b[39mkwargs):\n\u001b[1;32m--> 157\u001b[0m     data_to_wrap \u001b[38;5;241m=\u001b[39m f(\u001b[38;5;28mself\u001b[39m, X, \u001b[38;5;241m*\u001b[39margs, \u001b[38;5;241m*\u001b[39m\u001b[38;5;241m*\u001b[39mkwargs)\n\u001b[0;32m    158\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(data_to_wrap, \u001b[38;5;28mtuple\u001b[39m):\n\u001b[0;32m    159\u001b[0m         \u001b[38;5;66;03m# only wrap the first output for cross decomposition\u001b[39;00m\n\u001b[0;32m    160\u001b[0m         return_tuple \u001b[38;5;241m=\u001b[39m (\n\u001b[0;32m    161\u001b[0m             _wrap_data_with_container(method, data_to_wrap[\u001b[38;5;241m0\u001b[39m], X, \u001b[38;5;28mself\u001b[39m),\n\u001b[0;32m    162\u001b[0m             \u001b[38;5;241m*\u001b[39mdata_to_wrap[\u001b[38;5;241m1\u001b[39m:],\n\u001b[0;32m    163\u001b[0m         )\n",
-                        "File \u001b[1;32m~\\OneDrive\\Documents\\GITHUB STUFF\\tred\\tred\\_tensor_pca.py:318\u001b[0m, in \u001b[0;36mTPCA.transform\u001b[1;34m(self, X)\u001b[0m\n\u001b[0;32m    298\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mtransform\u001b[39m(\u001b[38;5;28mself\u001b[39m, X):\n\u001b[0;32m    299\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Apply dimensionality reduction to X.\u001b[39;00m\n\u001b[0;32m    300\u001b[0m \n\u001b[0;32m    301\u001b[0m \u001b[38;5;124;03m    See the TCAM algorithm from Mor et al. (2022)\u001b[39;00m\n\u001b[1;32m   (...)\u001b[0m\n\u001b[0;32m    315\u001b[0m \u001b[38;5;124;03m        TCAM projections in 2D transformed space.\u001b[39;00m\n\u001b[0;32m    316\u001b[0m \u001b[38;5;124;03m    \"\"\"\u001b[39;00m\n\u001b[1;32m--> 318\u001b[0m     \u001b[43mcheck_is_fitted\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[43m)\u001b[49m\n\u001b[0;32m    319\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28mlen\u001b[39m(X\u001b[38;5;241m.\u001b[39mshape) \u001b[38;5;241m==\u001b[39m \u001b[38;5;241m3\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure order-3 tensor input\u001b[39m\u001b[38;5;124m\"\u001b[39m\n\u001b[0;32m    320\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m (\n\u001b[0;32m    321\u001b[0m         X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m1\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mp_ \u001b[38;5;129;01mand\u001b[39;00m X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m2\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mt_\n\u001b[0;32m    322\u001b[0m     ), \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure the number of features, and time points, matches the model fit data\u001b[39m\u001b[38;5;124m\"\u001b[39m\n",
+                        "File \u001b[1;32m~\\OneDrive\\Documents\\GITHUB STUFF\\tred\\tred\\_tensor_pca.py:284\u001b[0m, in \u001b[0;36mTPCA.transform\u001b[1;34m(self, X)\u001b[0m\n\u001b[0;32m    264\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mtransform\u001b[39m(\u001b[38;5;28mself\u001b[39m, X):\n\u001b[0;32m    265\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Apply dimensionality reduction to X.\u001b[39;00m\n\u001b[0;32m    266\u001b[0m \n\u001b[0;32m    267\u001b[0m \u001b[38;5;124;03m    See the TCAM algorithm from Mor et al. (2022)\u001b[39;00m\n\u001b[1;32m   (...)\u001b[0m\n\u001b[0;32m    281\u001b[0m \u001b[38;5;124;03m        TCAM projections in 2D transformed space.\u001b[39;00m\n\u001b[0;32m    282\u001b[0m \u001b[38;5;124;03m    \"\"\"\u001b[39;00m\n\u001b[1;32m--> 284\u001b[0m     \u001b[43mcheck_is_fitted\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[43m)\u001b[49m\n\u001b[0;32m    285\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28mlen\u001b[39m(X\u001b[38;5;241m.\u001b[39mshape) \u001b[38;5;241m==\u001b[39m \u001b[38;5;241m3\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure order-3 tensor input\u001b[39m\u001b[38;5;124m\"\u001b[39m\n\u001b[0;32m    286\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m (\n\u001b[0;32m    287\u001b[0m         X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m1\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mp_ \u001b[38;5;129;01mand\u001b[39;00m X\u001b[38;5;241m.\u001b[39mshape[\u001b[38;5;241m2\u001b[39m] \u001b[38;5;241m==\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mt_\n\u001b[0;32m    288\u001b[0m     ), \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mEnsure the number of features, and time points, matches the model fit data\u001b[39m\u001b[38;5;124m\"\u001b[39m\n",
                         "File \u001b[1;32mc:\\Users\\brend\\OneDrive\\Documents\\GITHUB STUFF\\tred\\.venv\\lib\\site-packages\\sklearn\\utils\\validation.py:1461\u001b[0m, in \u001b[0;36mcheck_is_fitted\u001b[1;34m(estimator, attributes, msg, all_or_any)\u001b[0m\n\u001b[0;32m   1458\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m \u001b[38;5;167;01mTypeError\u001b[39;00m(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;132;01m%s\u001b[39;00m\u001b[38;5;124m is not an estimator instance.\u001b[39m\u001b[38;5;124m\"\u001b[39m \u001b[38;5;241m%\u001b[39m (estimator))\n\u001b[0;32m   1460\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;129;01mnot\u001b[39;00m _is_fitted(estimator, attributes, all_or_any):\n\u001b[1;32m-> 1461\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m NotFittedError(msg \u001b[38;5;241m%\u001b[39m {\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mname\u001b[39m\u001b[38;5;124m\"\u001b[39m: \u001b[38;5;28mtype\u001b[39m(estimator)\u001b[38;5;241m.\u001b[39m\u001b[38;5;18m__name__\u001b[39m})\n",
                         "\u001b[1;31mNotFittedError\u001b[0m: This TPCA instance is not fitted yet. Call 'fit' with appropriate arguments before using this estimator."
                     ]
                 }
             ],
             "source": [
+                "%%capture\n",
                 "# ERROR\n",
                 "X_transformed_1 = tpca.transform(X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# so, we need to fit the tpca object first - then call transform!\n",
                 "tpca.fit(X)\n",
                 "X_transformed_1 = tpca.transform(X)"
             ]
@@ -368,15 +386,15 @@
                 "works for matrix and vector inputs too. It just does a bit of rounding and \n",
                 "prints the size of the input. We have left the unfortunate original name as is, \n",
                 "to avoid breaking existing workflows. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix with shape (3, 6)\n",
@@ -401,24 +419,24 @@
                 "use a slightly more efficient computation to obtain the transformed data. \n",
                 "\n",
                 "See the `tred` library implementation for more details"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_transformed_2 = tpca.fit_transform(X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Matrix with shape (3, 6)\n",
@@ -433,15 +451,15 @@
                 "# some numbers might LOOK different, but you'll see that they are tiny and\n",
                 "# are effectively the same\n",
                 "disp(X_transformed_2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# the tensor operations produce some floating point errors\n",
                 "# below are the tolerances we use in tred's testing module, which show that the two\n",
                 "# transformations of X are indeed the same\n",
                 "RTOL = 1e-7\n",
@@ -454,25 +472,25 @@
             "metadata": {},
             "source": [
                 "We can use the fitted objects to transform out of bag data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# imagine one new observation, with p features, across t time points\n",
                 "new_obs = RNG.random(size=(1, p, t))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Tensor with shape (1, 4, 2)\n",
```

### Comparing `tred-0.1.2/tests/test_m_transforms.py` & `tred-0.1.3/tests/test_m_transforms.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/tests/test_tensor_ops.py` & `tred-0.1.3/tests/test_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/tests/test_tensor_pca.py` & `tred-0.1.3/tests/test_tensor_pca.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,23 +109,15 @@
         - include_negatives * 0.5 * element_scale
     )
 
     M, Minv = transform_generator(t)
     U, S, V = tsvdm(X, M=M, Minv=Minv, full_frontal_slices=return_full_frontal_slices)
     Vt = V.transpose(1, 0, 2)
 
-    # make sure that the m-product below has a 'non-None' set of inputs for M and Minv
-    if M is None:
-        M, Minv = generate_default_m_transform_pair(t)
-
-    def m_product_wrapper(A, B):
-        """m-product with fixed M and Minv to use for functools reduce"""
-        return m_product(A, B, M=M, Minv=Minv)
-
-    X_reconstruct = reduce(m_product_wrapper, (U, S, Vt))
+    X_reconstruct = m_product(U, S, Vt, M=M, Minv=Minv)
     assert_allclose(X, X_reconstruct)
 
 
 @pytest.mark.parametrize("tensor_shape", TENSOR_SHAPES)
 @pytest.mark.parametrize("element_scale", ELEMENT_SCALES)
 @pytest.mark.parametrize("include_negatives", [0, 1])
 @pytest.mark.parametrize("n_components", [None, 1, 6, 0.8])
```

### Comparing `tred-0.1.2/tests/test_utils.py` & `tred-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/tred/__init__.py` & `tred-0.1.3/tred/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 The `tred` module implements tensor decomposition methods such as tensor PCA and tensor 
 SVD. Most of the functionality in this module can be regarded as dimensionality reduction 
 strategies for order-3 datasets of size n, p, t, where p >> n > t. 
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 from ._m_transforms import (
+    generate_default_m_transform_pair,
     generate_transform_pair_from_matrix,
     generate_dstii_m_transform_pair,
     generate_dctii_m_transform_pair,
 )
 from ._tensor_ops import facewise_product, m_product
-from ._tensor_pca import generate_default_m_transform_pair, tsvdm, TPCA
+from ._tensor_pca import tsvdm, TPCA
 from ._utils import display_tensor_facewise
 
 # private - for testing
 ##########################################################################################
 from ._tensor_ops import _mode_1_unfold, _mode_2_unfold, _mode_3_unfold
 from ._utils import _singular_vals_tensor_to_mat, _singular_vals_mat_to_tensor
 
 __all__ = [
+    "generate_default_m_transform_pair",
     "generate_transform_pair_from_matrix",
     "generate_dctii_m_transform_pair",
     "generate_dstii_m_transform_pair",
     "facewise_product",
     "m_product",
-    "generate_default_m_transform_pair",
     "tsvdm",
     "TPCA",
     "display_tensor_facewise",
 ]
```

### Comparing `tred-0.1.2/tred/_m_transforms.py` & `tred-0.1.3/tred/_m_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,41 +24,77 @@
         len(X_input.shape) in SUPPORTED_TRANSFORM_DIMENSIONS
     ), "Expecting 1D (vector), 2D (matrix) or 3D (tensor) input"
     assert (
         X_input.shape[-1] == t_expected
     ), f"Expecting last input dimension to be {t_expected}"
 
 
+def generate_default_m_transform_pair(t):
+    """Wrapper for a function that generates functions M and Minv given the length of
+    a tubal fibre. Allows tred user to retrive the tubal transform functions for direct
+    computations using the tensor-tensor m-product.
+
+    The algorithms in the tred library do not require the user to explicitly specify a
+    tensor m-transform. In those cases, they revert to the default specified in this
+    function here.
+
+    We may choose to choose a different default family of mappings later.
+
+    Parameters
+    ----------
+        t : int
+            The length of the transform (length of the tubal fibers)
+
+    Returns
+    -------
+        M : Callable[[ndarray], ndarray]
+            A function which expects an order-3 tensor as input, and applies a tensor
+            transform to each of the tubal fibres. This preserves the dimensions of
+            the tensor.
+
+        Minv : Callable[[ndarray], ndarray]
+            A tensor transform (the inverse of `fun_m`)
+
+    References
+    ----------
+    The use of this transform with the m-product was introduced in:
+    `Mor, U., Cohen, Y., Valdés-Mas, R., Kviatcovsky, D., Elinav, E. and Avron,
+    H., 2022. Dimensionality reduction of longitudinal’omics data using modern
+    tensor factorizations. PLoS Computational Biology, 18(7), p.e1010212.`
+    """
+    return generate_dctii_m_transform_pair(t)
+
+
 def generate_transform_pair_from_matrix(M_mat, Minv_mat=None, *, inplace=False):
     """Generate a pair of functions to apply a matrix, and its inverse, to the tubal
     fibres of an order-3 tensor. See Kilmer et al. (20211).
 
     Parameters
     ----------
-        M_mat : ArrayLike
+        M_mat : ndarray
             Square matrix
 
-        Minv_mat : ArrayLike or None, default=None
+        Minv_mat : ndarray or None, default=None
             Square matrix, the inverse of M_mat. If not specified, this function will
             numerically evaluate the inverse of `M_mat`
 
         inplace : bool, default=False
             Control whether or not the generated functions modify the input tensor
             in-place, or return a copy with the m-transform applied
 
             THIS ARGUMENT DOES NOT CURRENTLY ALTER ANY BEHAVIOUR FOR THIS FUNCTION, BUT
             IS A PLACEHOLDER FOR FUTURE DEVELOPMENT.
 
     Returns
     -------
-        M : Callable[[ArrayLike], ndarray]
+        M : Callable[[ndarray], ndarray]
             A function which expects an order-3 tensor as input, and applies `M_mat`
             to each of the tubal fibres. This preserves the dimensions of the tensor.
 
-        Minv : Callable[[ArrayLike], ndarray]
+        Minv : Callable[[ndarray], ndarray]
             A tensor transform (the inverse of `M`)
 
     References
     ----------
     `Kilmer, M.E., Horesh, L., Avron, H. and Newman, E., 2021. Tensor-tensor
     algebra for optimal representation and compression of multiway data. Proceedings
     of the National Academy of Sciences, 118(28), p.e2015851118.`
@@ -124,19 +160,19 @@
             in-place, or return a copy with the m-transform applied
 
         norm : {“backward”, “ortho”, “forward”}, default="ortho"
             See https://docs.scipy.org/doc/scipy/reference/generated/scipy.fft.dct.html#scipy.fft.dct
 
     Returns
     -------
-        M : Callable[[ArrayLike], ndarray]
+        M : Callable[[ndarray], ndarray]
             A function which expects an order-3 tensor as input, and applies DCT-II to
             each of the tubal fibres. This preserves the dimensions of the tensor.
 
-        Minv : Callable[[ArrayLike], ndarray]
+        Minv : Callable[[ndarray], ndarray]
             A tensor transform (the inverse of `M`)
 
     References
     ----------
     The use of this transform with the m-product was introduced in:
     `Mor, U., Cohen, Y., Valdés-Mas, R., Kviatcovsky, D., Elinav, E. and Avron,
     H., 2022. Dimensionality reduction of longitudinal’omics data using modern
@@ -184,20 +220,20 @@
             in-place, or return a copy with the m-transform applied
 
         norm : {“backward”, “ortho”, “forward”}, default="ortho"
             See https://docs.scipy.org/doc/scipy/reference/generated/scipy.fft.dst.html#scipy.fft.dst
 
     Returns
     -------
-        M : Callable[[ArrayLike], ndarray]
+        M : Callable[[ndarray], ndarray]
             A function which expects an order-3 tensor as input, and applies DFT via a FFT
             algorithm to each of the tubal fibres. This preserves the dimensions of the
             tensor.
 
-        Minv : Callable[[ArrayLike], ndarray]
+        Minv : Callable[[ndarray], ndarray]
             A tensor transform (the inverse of `M`)
     """
 
     def M(X):
         _assert_t_and_order(X, t)
         return dst(
             X,
```

### Comparing `tred-0.1.2/tred/_tensor_pca.py` & `tred-0.1.3/tred/_tensor_pca.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,49 +14,15 @@
     ClassNamePrefixFeaturesOutMixin,
     TransformerMixin,
 )
 from sklearn.utils.validation import check_is_fitted
 
 from ._tensor_ops import facewise_product, _rank_q_truncation_zero_out
 from ._utils import RealNotInt, _singular_vals_mat_to_tensor
-from ._m_transforms import generate_dctii_m_transform_pair
-
-
-def generate_default_m_transform_pair(t):
-    """Wrapper for a function that generates functions M and Minv given the length of
-    a tubal fibre.
-
-    Both the tsvdm and TPCA do not require the user to explicitly specify a tensor
-    m-transform. In those cases, they rely on this function here.
-
-    We may choose to choose a different default family of mappings later.
-
-    Parameters
-    ----------
-        t : int
-            The length of the transform (length of the tubal fibers)
-
-    Returns
-    -------
-        M : Callable[[ArrayLike], ndarray]
-            A function which expects an order-3 tensor as input, and applies a tensor
-            transform to each of the tubal fibres. This preserves the dimensions of
-            the tensor.
-
-        Minv : Callable[[ArrayLike], ndarray]
-            A tensor transform (the inverse of `fun_m`)
-
-    References
-    ----------
-    The use of this transform with the m-product was introduced in:
-    `Mor, U., Cohen, Y., Valdés-Mas, R., Kviatcovsky, D., Elinav, E. and Avron,
-    H., 2022. Dimensionality reduction of longitudinal’omics data using modern
-    tensor factorizations. PLoS Computational Biology, 18(7), p.e1010212.`
-    """
-    return generate_dctii_m_transform_pair(t)
+from ._m_transforms import generate_default_m_transform_pair
 
 
 def tsvdm(
     A,
     M=None,
     Minv=None,
     *,
@@ -70,22 +36,22 @@
     or adopt other matrix svd implementations.
 
     NOTE: For now, unlike some other implementations (Numpy, Scipy), we will return the
     tensor $V$ NOT $V^T$.
 
     Parameters
     ----------
-        A : ArrayLike, shape: (n, p, t)
+        A : ndarray, shape: (n, p, t)
             $n \times p \times t$ data tensor
 
-        M : Callable[[ArrayLike], ndarray] or None, default=None
+        M : Callable[[ndarray], ndarray] or None, default=None
             A function which, given some order-3 tensor, returns it under some $\times_3$
             invertible transformation.
 
-        MInv : Callable[[ArrayLike], ndarray] or None, default=None
+        MInv : Callable[[ndarray], ndarray] or None, default=None
             The inverse transformation of M
 
         keep_hats : bool, default=False
             Setting to `True` will return the tSVDM factors in the tensor domain transform
             space, under the specified $M$
 
         full_frontal_slices : bool, default=True
@@ -116,15 +82,15 @@
     """
 
     assert len(A.shape) == 3, "Ensure order-3 tensor input"
     assert not (
         callable(M) ^ callable(Minv)
     ), "If explicitly defined, both M and its inverse must be defined"
 
-    if M is None:  # and Minv is None - guaranteed by assertion
+    if not callable(M):  # and Minv is not defined - guaranteed by assertion
         M, Minv = generate_default_m_transform_pair(A.shape[-1])
 
     # transform the tensor to new space via the mode-3 product
     hatA = M(A)
 
     # an appropriate transposition allows Numpys array broadcasting to do facewise svd's
     # S_mat contains the singular values per matrix in the input stack of matrices
@@ -195,33 +161,33 @@
         the amount of variance that needs to be explained is greater than the percentage
         specified.
 
     copy : bool, default=True
         If False, data passed to fit are overwritten and running fit(X).transform(X) will
         not yield the expected results. Use fit_transform(X) instead.
 
-    M : Callable[[ArrayLike], ndarray] or None, default=None
+    M : Callable[[ndarray], ndarray] or None, default=None
         A function which, given some order-3 tensor, returns it under some $\times_3$
         invertible transformation. If unspecified TPCA will use the Discrete Consine
         Transform (ii) from scipy fft.
 
-    MInv : Callable[[ArrayLike], ndarray] or None, default=None
+    MInv : Callable[[ndarray], ndarray] or None, default=None
         The inverse transformation of M.
 
     centre : bool, default=True
         If False, the data tensor will not be centralized into Mean Deviation Form.
         By default, the mean horizontal slice of the tensor is subtracted, so that all of
         the horizontal slices sum to 0, analagous to centering the data in PCA.
 
     Attributes
     ----------
     n_, p_, t_, k_ : int
         The dimensions of the training data. ``k_ == min(n_, p_)``
 
-    M_, MInv_ : Callable[[ArrayLike], ndarray]
+    M_, MInv_ : Callable[[ndarray], ndarray]
         The m-transform pair (forward and inverse) used for the underlying tensor-tensor
         m-product.
 
     n_components_ : int
         The estimated number of components. If ``n_components`` was explicitly set by an
         integer value, this will be the same as that. If `n_components` was a number
         between 0 and 1, this number is estimated from input data. Otherwise, if not set
@@ -276,15 +242,15 @@
         self.centre = centre
 
     def fit(self, X, y=None):
         """Fit the model with X.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n, p, t)
+        X : ndarray of shape (n, p, t)
             Training data, where `n` is the number of samples, `p` is the number of
             features, as `t` is the number of time points.
 
         y : Ignored
             Ignored.
 
         Returns
@@ -298,15 +264,15 @@
     def transform(self, X):
         """Apply dimensionality reduction to X.
 
         See the TCAM algorithm from Mor et al. (2022)
 
         Parameters
         ----------
-        X : ArrayLike of shape (n, p, t)
+        X : ndarray of shape (n, p, t)
             Training data, where `n` is the number of samples, `p` is the number of
             features, as `t` is the number of time points.
 
         y : Ignored
             Ignored.
 
         Returns
@@ -336,15 +302,15 @@
 
         The output here will not be identical to calling fix(X).transform(X). But, the
         two give the same results up to machine precision. We provide a brief discussion
         of this below.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n, p, t)
+        X : ndarray of shape (n, p, t)
             Training data, where `n` is the number of samples, `p` is the number of
             features, as `t` is the number of time points.
 
         y : Ignored
             Ignored.
 
         Returns
@@ -397,15 +363,15 @@
         if self.copy:
             X = X.copy()
         if self.centre:
             X -= self.mean_
 
         # if there is no explicitly defined transform in __init__, assign functions to
         # perform a default transformation
-        if self.M is None:  # and Minv is None - guaranteed by assertion
+        if not callable(self.M):  # and Minv is not defined - guaranteed by assertion
             self.M_, self.Minv_ = generate_default_m_transform_pair(X.shape[2])
         else:
             self.M_, self.Minv_ = self.M, self.Minv
 
         # perform tensor decomposition via Kilmer's tSVDM
         hatU, hatS_mat, hatV = tsvdm(
             X,
```

### Comparing `tred-0.1.2/tred/_utils.py` & `tred-0.1.3/tred/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     print output is a more intuitive sequence of frontal slices. We often use this in
     notebooks. It also prints the rounded values.
 
     UPDATE: Also works for matrices and vectors now.
 
     Parameters
     ----------
-        tens : ArrayLike of shape (n, p, t)
+        tens : ndarray of shape (n, p, t)
             Order-3 tensor representation
 
     Examples
     --------
     >>> import numpy as np
     >>> from tdim import display_tensor_facewise as disp
     >>> test = np.eye(3)[:, :, None] # a 3x3x1 tensor
@@ -75,15 +75,15 @@
     """Decompress $k \times t$ matrix of singular values into $\hat{S}$ from literature.
 
     NOTE: There's probably a cool numpy way to do this without the for loop...but for now
     it works fine as $t$ is usually modest for the data we work with
 
     Parameters
     ----------
-        mat : ArrayLike of shape (k, t_)
+        mat : ndarray of shape (k, t_)
             $k \times t_$ matrix representation, the function checks if `t_ == t`
 
         n : int
             first dimension of output tensor
 
         p : int
             second dimension of output tensor
@@ -111,15 +111,15 @@
     into a $k \times t$ matrix. Each row contains the $k$ singular values from that
     longitudinal slice.
 
     Reverses _singular_vals_mat_to_tensor
 
     Parameters
     ----------
-        tensor : ArrayLike of shape: (n, p, t)
+        tensor : ndarray of shape: (n, p, t)
             $n \times p \times t$ tensor representation
 
     Returns
     -------
         mat : ndarray of shape: (min(n, p), t)
             $k \times t$ matrix representation of singular values, where
             $k = \min{(n,p)}$
```

### Comparing `tred-0.1.2/.gitignore` & `tred-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/LICENSE` & `tred-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/README.txt` & `tred-0.1.3/README.txt`

 * *Files identical despite different names*

### Comparing `tred-0.1.2/pyproject.toml` & `tred-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "tred"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Brendan Lu", email="brendannlu5@gmail.com" },
 ]
 description = "Dimensionality reduction techniques for order-3 tensors"
-readme = "README.txt"
+readme = "pypi.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
```

