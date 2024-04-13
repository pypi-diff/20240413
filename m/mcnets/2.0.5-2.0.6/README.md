# Comparing `tmp/mcnets-2.0.5.tar.gz` & `tmp/mcnets-2.0.6.tar.gz`

## Comparing `mcnets-2.0.5.tar` & `mcnets-2.0.6.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0   129295 2020-02-02 00:00:00.000000 mcnets-2.0.5/src/mcnets/__deprecated.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-2.0.5/src/mcnets/__init__.py
--rw-r--r--   0        0        0    31992 2020-02-02 00:00:00.000000 mcnets-2.0.5/src/mcnets/_experimental.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 mcnets-2.0.5/src/mcnets/activations.py
--rw-r--r--   0        0        0    42967 2020-02-02 00:00:00.000000 mcnets-2.0.5/src/mcnets/main.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mcnets-2.0.5/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-2.0.5/LICENSE
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mcnets-2.0.5/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 mcnets-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0   129361 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/__deprecated.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/__init__.py
+-rw-r--r--   0        0        0    38662 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/_experimental.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/_nlp_tools.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/activations.py
+-rw-r--r--   0        0        0    37101 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/main.py
+-rw-r--r--   0        0        0    14837 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/tools.py
+-rw-r--r--   0        0        0   792684 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/spy
+-rw-r--r--   0        0        0    68789 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/stocks.xlsx
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/top500tickers_list
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mcnets-2.0.6/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-2.0.6/LICENSE
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mcnets-2.0.6/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 mcnets-2.0.6/PKG-INFO
```

### Comparing `mcnets-2.0.5/src/mcnets/__deprecated.py` & `mcnets-2.0.6/src/mcnets/__deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 plt = None
 
 import numpy as np
 import textwrap as txt
 import os
 from multiprocessing import Pool
 from time import perf_counter as pc
+from warnings import warn
 
 # Warn on loading all this
-print("MCNets: *WARNING* Deprecated tools and models have been loaded. None of these are guranteed to be in working order and may mess up other working tools.")
+warn("MCNets: *WARNING* Deprecated tools and models have been loaded. None of these are guranteed to be in working order and may mess up other working tools.",
+     category=DeprecationWarning)
 
 
 # ==================== Models ==================== #
 
 # Original Neural Network Model
 class MCNeuralNetwork:
     ## Default Functions ## 
@@ -1607,15 +1609,15 @@
                                 input_activation=af_start[0], output_activation=af_start[-1])
 
         # ## TEMP/TEST ##
         model.use_biases = _use_biases
         model.setup_model(X, Y)
         
         # Test initial model
-        xt, xv, yt, yv = TTSplit(X, Y, percentTrain=train_split_percent)
+        xt, xv, yt, yv = TTSplit(X, Y, percent_train=train_split_percent)
         model.fit(xt, yt, Ieta=Ieta, Beta=Beta, Gamma=Gamma, verbose=False)
         best_score = model.score(xv, yv)
         best_model = model.CopyNet()
 
         # Do round-robin improvments
         num_test_models = iterations*num_layers*len(test_activations)
         i = 0
@@ -1638,15 +1640,15 @@
                     model.activationFunction[li] = AF.upper()
 
                     # Skip test AF if its the current one
                     if skip_current and initial_af.upper() == AF.upper():
                         continue
 
                     # Test model score
-                    xt, xv, yt, yv = TTSplit(X, Y, percentTrain=train_split_percent)
+                    xt, xv, yt, yv = TTSplit(X, Y, percent_train=train_split_percent)
                     model.fit(xt, yt, Ieta=Ieta, Beta=Beta, Gamma=Gamma, verbose=False)
                     test_score = model.score(xv, yv)
 
                     if test_score > best_score:
                         # Keep model as best
                         best_score = test_score
                         best_model = model.CopyNet()
@@ -1780,15 +1782,15 @@
         errors += 1
 
     if y_diff/y_copy.size >= 1e-12:
         print("Y Denormalization error is large!")
         errors += 1
     
     # Test test/train split
-    xt, xv, yt, yv = TTSplit(X, Y, percentTrain=75)
+    xt, xv, yt, yv = TTSplit(X, Y, percent_train=75)
 
     print("Step 1 Done - TTSplit(), normalize() and denormalize() verified\n")
 
     # Step 2 (MCNeuralNetwork)
     model = MCNeuralNetwork([10, 10], activations=['relu', 'silu'])
     if print_sub_steps:
         print("Step 2 Part 1/4 Done (make MCNeuralNetwork)")
@@ -2024,15 +2026,15 @@
     input_activation = 'lin'
     output_activation = 'lin'
 
     I = round(10 * training_depth)
     B = round(10 * training_depth)
     G = round(1.5 * training_depth)
 
-    x_train, x_val, y_train, y_val = TTSplit(X, Y, percentTrain=100*(1 - validation_size))
+    x_train, x_val, y_train, y_val = TTSplit(X, Y, percent_train=100*(1 - validation_size))
 
 
     ## Main loop (For First Layer Activation) ##
     if test_ends:
         initial_scores = []
         for i, l1 in enumerate(activation_tests):
             # Make test model
@@ -2377,15 +2379,15 @@
               to assist in error checking            
         """
         
         # Get initial score
         bestAverageScore = netMetrics(self, XData, YData, useFast=useFast)
 
         # Make train/test split
-        xTrain, yTrain, xTest, yTest = TTSplit(XData, YData, percentTrain=70)
+        xTrain, yTrain, xTest, yTest = TTSplit(XData, YData, percent_train=70)
         bestNet = self
         for Itr in range(Ieta):
             # Get current tweak amplitude
             Tau = 2 ** (-Itr / Gamma)
 
             # Make test batch
             testNets = []
```

### Comparing `mcnets-2.0.5/src/mcnets/_experimental.py` & `mcnets-2.0.6/src/mcnets/_experimental.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,181 @@
 import mcnets.main as mc
-from __deprecated import MCNeuralNetwork
+# from __deprecated import MCNeuralNetwork
 import numpy as np
+from warnings import warn
 
 # SOUP requirements
-from main import copy, r2d2, sig
-
+from main import copy, r2d2, sig, test_activations, NeuralNetwork, score_model
 
+warn("MCNet Experimental features loaded; Note that these are not guranteed to be in working order",
+     category=ImportWarning)
 
 # ==================== Models ==================== #
+# Neural Ensemble #
+class NeuralEnsemble():
+    def __init__(self, main_model, num_nns:int=3, nn_size:int=5, normalize_nns:bool=False, 
+                 nn_early_stopping:bool=False, verbose:bool=False) -> None:
+        """
+        EXPERIMENTAL
+
+        This currently tends to lead to lots of overfitting, and preforms quite poorly
+        in cross-validations
+
+        Constructs some neural networks with activations
+        that are best suited for the given training data.
+        Calling .predict for this ensemble combines the
+        given X with the hidden layer features from these
+        neural networks and is then passed to the final
+        model to create an output.
+
+        - `main_model`
+            - The final model that uses the given X data and neural network hidden layer features
+            to generate the final output
+
+        - `num_nns`
+            - Number of top neural networks to use for generating features; each has a unique activation
+            - NOTE: Each network adds nn_size # of features! Having too
+            many models will greatly slow down the main_model's training
+            and this model overall
+        
+        - `nn_size`
+            - The size of the 1 hidden layer generated in the neural networks
+
+        - 'normalize_nns`
+            - Decides if the neural networks used for generating features should normalize
+            their inputs
+
+        - `nn_early_stopping`
+            - Decides if the NNs used for making features shoul use early stopping when being fit
+        """
+
+        # Neural network things
+        self._num_nns = num_nns
+        self._nn_size = nn_size
+        self._normalize = normalize_nns
+        self._early_stop = nn_early_stopping
+        self._networks = []
+
+        # Fitting
+        self._is_fitted = False
+
+        # Other main attributes
+        self.model = main_model
+        self.verbose = verbose
+
+    def get_neural_features(self, X:np.ndarray):
+        # Gather all the neural features
+        xbig = X.copy()
+        for mi in self._networks:
+            xbig = np.hstack([xbig, mi.predict_layer(X, 1)])
+        return xbig
+    
+    def predict(self, X:np.ndarray):
+        # Use base model predictions to get actual predictions from dictator
+        X_nn = self.get_neural_features(X)
+        return self.model.predict(X_nn)
+
+    def compile_nns(self, X:np.ndarray, Y:np.ndarray):
+        if self.verbose:
+            print("Generating NeuralEnsemble NNs ...", end='\r')
+
+        # Get top activations for dataset
+        results = test_activations(X, Y, cv=3, verbose=False, 
+                                    nn_kwargs={'hidden_counts': self._nn_size, 
+                                                'early_stopping': self._early_stop, 
+                                                'normalize_input': self._normalize,
+                                                'max_iter': 750},
+                                    custom_activations=['lin', 'relu', 'sig', 'silu', 'dsilu', 'rnd', 'lrelu', 'tanh'],
+                                    only_custom=True)
+        
+        if self.verbose:
+            print("Generating NeuralEnsemble NNs ... Done       ", end='\r')
+
+        # Get top activations 
+        top_afs = results[:self._num_nns]
+        top_afs = [scr_af[1] for scr_af in top_afs] # Get only functions, not scores
+
+        # Make models and add to model storage
+        for AF in top_afs:
+            self._networks.append(NeuralNetwork(hidden_counts=(self._nn_size), activations=AF, 
+                                                normalize_input=self._normalize, early_stopping=self._early_stop))
+            
+        # Fit the neural networks
+        if self.verbose:
+            print("Initalizing NeuralEnsemble NNs ...              ", end='\r')
+        
+        for mi in self._networks:
+            # mi._initialize_model(input_size=X.shape[1], output_size=1 if Y.ndim == 1 else Y.shape[1])
+            mi.fit(X, Y)
+
+        if self.verbose:
+            print("Initalizing NeuralEnsemble NNs ... Done          ", end='\r')
+
+        # Finish
+        self._is_fitted = True
+
+    def fit(self, X:np.ndarray, Y:np.ndarray, score_type='r2'):
+        # Generate neural networks to use
+        if not self._is_fitted:
+            self.compile_nns(X, Y)
+
+        # Add on NN features to X
+        X = self.get_neural_features(X)
+
+        # Fit main model to all data above (try passing through score_type)
+        try:
+            self.model.fit(X, Y, score_type=score_type)
+        except TypeError as e:
+            if 'got an unexpected keyword argument' in str(e):
+                self.model.fit(X, Y)
+            else:
+                raise ValueError(e)
+
+    def score(self, X:np.ndarray, Y:np.ndarray, score_type='r2'):
+        return score_model(self, X, Y, method=score_type)
+
+# Psuedo RNN
+class EasyRNN:
+    def __init__(self, layers=(10), afs=('relu'), inaf='lin', outaf='lin', max_iter=250, lookback=3, verbose=True) -> None:
+        self.nn = mc.NeuralNetwork(hidden_counts=layers,
+                                   activations=afs,
+                                   input_acti=inaf,
+                                   output_acti=outaf,
+                                   max_iter=max_iter,
+                                   early_stopping=False,
+                                   verbose=verbose)
+        self.lookback = lookback
+
+    def predict(self, X):
+        return self.nn.predict(self.make_rnn_data(X))
+    
+    def make_rnn_data(self, X, Y=None):
+        # Reshape X; get correct Y data
+        for i in range(self.lookback, X.shape[0]):
+            if i == self.lookback:
+                Xrnn = X[i-self.lookback:i+1].flatten().copy()
+                Xrnn = Xrnn.reshape((1, len(Xrnn)))
+            else:
+                Xrnn = np.vstack([Xrnn, X[i-self.lookback:i+1].flatten().copy().reshape((1, Xrnn.shape[1]))])
+        
+        if not Y is None:
+            Yrnn = Y[self.lookback:].copy()
+            return Xrnn, Yrnn
+        else:
+            return Xrnn
+    
+    def fit(self, X, Y, score_type='r2'):
+        self.nn._initialize_model(
+            input_size=X.shape[1]*(self.lookback+1),
+            output_size=X.shape[1]
+        )
+
+        Xrnn, Yrnn = self.make_rnn_data(X, Y)
+
+        self.nn.fit(Xrnn, Yrnn, score_type=score_type)
 
 # SOUP Regressor (Sub-Ordinary Universal Polynomial)
 ## The SOUP models are good, but the np.clip should really
 ## be replaced with L2 and L1 penalties instead
 class MCSoupRegressor:
     def __init__(self, coef_bounds = (-1, 1), use_tan=False, round_threshold=1e-5):
         # Desc
```

### Comparing `mcnets-2.0.5/src/mcnets/activations.py` & `mcnets-2.0.6/src/mcnets/activations.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,23 @@
 def silu(calcVec):
     """SiLU / Swish activation function
     
     Alternative to the ReLU function"""
     return calcVec / (1 + np.exp(-np.clip(calcVec, -7e2, None)))
 
 # SIG-Like
-e = 2.7182818284590452353602874713527
-def sig(cv):
-    """Sigmoid activation function"""
-    cv = np.maximum(cv, -7e2)
-    # cv[cv <= -7e2] = 7e2
-    return 1 / (1 + e**(-cv))
+def sig(x):
+    return (np.tanh(x/2)/2+0.5)
+
+# e = 2.7182818284590452353602874713527
+# def sig(cv):
+#     # """Sigmoid activation function"""
+#     cv = np.maximum(cv, -7e2)
+#     cv[cv <= -7e2] = 7e2
+#     return 1 / (1 + e**(-cv))
 
 def dsilu(calcVec):
     """dSiLU / dSwish activation function
     
     Alternative to the sig function"""
     return sig(calcVec) * (1 + calcVec * (1 - sig(calcVec)))
```

### Comparing `mcnets-2.0.5/src/mcnets/main.py` & `mcnets-2.0.6/src/mcnets/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# Python Dependancies
-from random import sample
-import copy
-
-# External Dependancies
-import numpy as np
-from joblib import load, dump
-
 # MCNet Dependancies
 from mcnets.activations import *
+from tools import *
+
+# Early Fitting - Ignore polynomial rank warnings
+import warnings
+warnings.simplefilter('ignore', np.RankWarning)
+
 
-## Models ##
+## =================== Models ==================== ##
 # Primary Monte-Carlo Neural Network Model
 class NeuralNetwork:
     def __init__(self, hidden_counts:'tuple[int]'=(100), activations:'tuple[str, function]'=('relu'), input_acti='identity', 
                  output_acti='identity', max_iter=1000, learning_rate_init=1, learning_rate_mode=('adaptive', 'dynamic', 'constant'), 
-                 gamma=0.0025, n_iter_no_change=100, l2_reg=0, l1_reg=0, dropout=0.0, validation_fraction:float=0, early_stopping=True, 
-                 quad_tol:float=-0.01, tri_tol:float=-0.01, verbose=False):
+                 gamma=0.0025, n_iter_no_change=25, l2_reg=0, l1_reg=0, dropout=0.0, validation_fraction:float=0, early_stopping=True, 
+                 quad_tol:float=-0.01, tri_tol:float=-0.01, normalize_input=False, verbose=False):
         """
         Neural Network that uses Monte-Carlo training. Can be either a regressor or classifier depending on the
         output_activation used (i.e. use sigmoid/sig for a classifier).
 
         - `hidden_counts`
             - List of count of units to have per hidden layer
             - Length of this list == number of hidden layers
@@ -85,31 +83,38 @@
         - `tri_tol`
             - Early stopping method
             - Fits a polynomial (degree 3) to the current training scores during fitting
             - If the polynomial has a tangent/slope value less than this tolerance, training stops
             - If None:
                 - Doesn't consider this for early stopping, even if early_stopping is True
                 - Helpful for only considering one of the tols (quad or tri)
+
+        - `normalize_input`
+            - Automatically normalize input data
         """
 
         # Assemble hidden counts to a list
         if isinstance(hidden_counts, list):
             self.hidden_counts = hidden_counts
         elif isinstance(hidden_counts, tuple):
             self.hidden_counts = list(hidden_counts)
-        elif isinstance(hidden_counts, (str, int)):
+        elif isinstance(hidden_counts, (int)):
             self.hidden_counts = [hidden_counts]
+        else:
+            raise ValueError("Unknown type given for hidden_counts")
 
         # Assemble activations to a list
         if isinstance(activations, list):
             self.activations = activations
         elif isinstance(activations, tuple):
             self.activations = list(activations)
-        elif isinstance(activations, str):
-            self.activations = [activations]
+        elif isinstance(activations, str) or callable(activations):
+            self.activations = [activations]*len(self.hidden_counts)
+        else:
+            raise ValueError("Unknown type given for activations")
 
         # Main params
         self.input_acti = input_acti
         self.output_acti = output_acti
         self.max_iter = max_iter
         self.learning_rate_init = learning_rate_init
         self.learning_rate_mode = 'adaptive' if isinstance(learning_rate_mode, tuple) else learning_rate_mode
@@ -118,18 +123,22 @@
         self.l2_reg = l2_reg
         self.l1_reg = l1_reg
         self.dropout = dropout
         self.val_frac = validation_fraction
         self.stop_early = early_stopping
         self.quad_tol = quad_tol
         self.tri_tol = tri_tol
+        self.normalize_input = normalize_input
         self.verbose = verbose
 
         # Fit-generated params
         self._use_score_history = 'train' if self.val_frac <= 0 else 'val'
+        self._has_normalized_info = False
+        self._normalized_mean = None
+        self._normalized_stdev = None
         self._is_fitted = False
         self.input_size = None
         self.output_size = None
         self.weights = []
         self.biases = []
 
         # Initial checks
@@ -171,26 +180,62 @@
     def get_weights(self):
         return [wi.copy() for wi in self.weights]
     
     def get_biases(self):
         return [bi.copy() for bi in self.biases]
 
     def predict(self, X:np.ndarray):
+        # Normalize input if wequested
+        if self.normalize_input and self._has_normalized_info:
+            X = (X - self._normalized_mean) / self._normalized_stdev
+        elif self.normalize_input and not self._has_normalized_info:
+            raise ValueError("Model should have Mean and StDev info for input data normalization but it doesnt!")
+
         # Apply initial activation
         X = self.input_acti(X)
 
         # Hidden Layers yipeeeeeeeeeee
         for afunc, W, B in zip(self.activations+[self.output_acti], self.weights, self.biases):
             X = afunc(np.dot(X, W) + B)
 
         # Shape accordingly
         if self.output_size == 1:
             X = X.flatten()
         return X
     
+    def predict_layer(self, X:np.ndarray, from_h_layer:int):
+        """Specialized predict function to allow for getting model features from
+        any of the hidden layers (specified from `layer`)
+        
+        - `from_h_layer`:
+            - Integer deciding which hidden layer to snatch features from
+            - Should be a value in the domain [1, (# of hidden layers)]
+        """
+        # Prevent fetching outputs of layers that dont exist =)
+        if from_h_layer > len(self.hidden_counts):
+            raise ValueError(f"Features from hidden layer #{from_h_layer} requested but the model only has {len(self.hidden_counts)} hidden layers!")
+        from_h_layer = np.clip(from_h_layer, 1, len(self.hidden_counts))
+        
+        ## Modified prediction algorithm ##
+        # Normalize input if wequested
+        if self.normalize_input and self._has_normalized_info:
+            X = (X - self._normalized_mean) / self._normalized_stdev
+        elif self.normalize_input and not self._has_normalized_info:
+            raise ValueError("Model should have Mean and StDev info for input data normalization but it doesnt!")
+
+        # Apply initial activation
+        X = self.input_acti(X)
+
+        # Hidden Layers yipeeeeeeeeeee
+        for afunc, W, B in zip(list(self.activations+[self.output_acti])[:from_h_layer], self.weights[:from_h_layer], self.biases[:from_h_layer]):
+            X = afunc(np.dot(X, W) + B)
+
+        # Shape accordingly
+        return X.flatten() if self.output_acti == 1 else X
+        
     def _current_l2_penalty(self):
         return self.l2_reg*np.sum([np.sum(wi**2) for wi in self.get_weights()])
     
     def _current_l1_penalty(self):
         return self.l1_reg*np.sum([np.sum(np.abs(wi)) for wi in self.get_weights()])
     
     def score(self, X, Y, score_type='r2'):
@@ -218,24 +263,33 @@
         """
 
         # History dict
         history = {'train': [], 'val': []}
 
         # Train/Validation split
         if self.val_frac > 0:
-            xt, xv, yt, yv = TTSplit(X, Y, percentTrain=(1-self.val_frac))
+            xt, xv, yt, yv = TTSplit(X, Y, percent_train=(1-self.val_frac))
         else:
             xv = None; yv = None
+            xt = X.copy()
+            yt = Y.copy()
 
         # Make val score function for easy handling of both cases (val_frac == 0 and val_frac > 0)
         def val_score(self:NeuralNetwork, xv, yv, score_type=score_type):
             if self.val_frac <= 0:
                 return 0
             else:
                 return self.score(xv, yv, score_type=score_type)
+            
+        # Get normalization info if applicable
+        if not self._is_fitted and self.normalize_input:
+            msinfo = normalize(X)[1]
+            self._normalized_mean = msinfo[0]
+            self._normalized_stdev = msinfo[1]
+            self._has_normalized_info = True
 
         # Generate model
         self._initialize_model(input_size=1 if len(X.shape)==1 else X.shape[1],
                                output_size=1 if len(Y.shape)==1 else Y.shape[1],
                                force_generate=False)
 
         # Single Column inputs - check for correct size (len(X), 1)
@@ -298,15 +352,16 @@
 
                         ## Quad Tol check #
                         if self.quad_tol != None:
                             # Coefficients
                             p2_coefs = np.polyfit(poly_x, history[self._use_score_history], deg=2)
 
                             # Y (score) predictions
-                            p2_y = [sum([ci*x**(2-i) for i, ci in enumerate(p2_coefs)]) for x in poly_x]
+                            p2_y = np.polyval(p2_coefs, poly_x)
+                            # p2_y = [sum([ci*x**(2-i) for i, ci in enumerate(p2_coefs)]) for x in poly_x]
 
                             # Numerical tangents
                             dp2_y = [y1-y2 for y1, y2 in zip(p2_y[1:], p2_y[:-1])]
 
                             # Check min quad tangent slope
                             if min(dp2_y) < self.quad_tol:
                                 if self.verbose:
@@ -316,15 +371,16 @@
                             
                         ## Tri Tol check #
                         if self.tri_tol != None:
                             # Coefficients
                             p3_coefs = np.polyfit(poly_x, history[self._use_score_history], deg=3)
 
                             # Y (score) predictions
-                            p3_y = [sum([ci*x**(3-i) for i, ci in enumerate(p3_coefs)]) for x in poly_x]
+                            p3_y = np.polyval(p3_coefs, poly_x)
+                            # p3_y = [sum([ci*x**(3-i) for i, ci in enumerate(p3_coefs)]) for x in poly_x]
 
                             # Numerical tangents
                             dp3_y = [y1-y2 for y1, y2 in zip(p3_y[1:], p3_y[:-1])]
 
                             # Check min quad tangent slope
                             if min(dp3_y) < self.tri_tol:
                                 if self.verbose:
@@ -370,14 +426,15 @@
             'l2_reg': (1e-10, 1),
             'l1_reg': (1e-10, 1),
             'dropout': (0, 0.9), 
             'validation_fraction': (0.1, 0.75),
             'early_stopping': [True, False],
             'quad_tol': (-1, 1),
             'tri_tol': (-1, 1),
+            'normalize_input': [True, False],
         }
 
     def copy(self):
         """Returns a deep copy of the model"""
         return copy.deepcopy(self)
     
     def make_mutation(self, learning_rate=1):
@@ -590,532 +647,177 @@
         return score_model(self, X, Y, method=method) - self._current_l2_penalty() - self._current_l1_penalty()
     
     def copy(self):
         """Returns a copy of the model"""
         return copy.deepcopy(self)
 
 
-## External Functions ##
-def save_model(model, name:str):
-    """
-    Load the model object saved under the given name
-    """
-    dump(model, filename=name)
-
-def load_model(name:str):
-    """
-    Uses joblib function 'load' to recall a model object previous saved
-    """
-    try:
-        return load(name)
-    except:
-        raise ValueError("Could not find a model with the given name")
-
-def TTSplit(Xdata, Ydata, percentTrain:float = 70):
-    """
-    Universal Train-Test data split via random selection.
+## ================== Ensembles ================== ##
+# Standard Ensemble #
+class StandardEnsemble():
+    def __init__(self, models:list) -> None:
+        """
+        A wrapper for combining multiple models into one. By default, uses weights
+        equal weights for each individual model given unless `optimize_model_weights`
+        is called.
 
-    Returns in the order xTrain, xTest, yTrain, yTest
-    
-    - percentTrain
-        - sets the amount of data given back for training data, 
-          while the rest is sent into the testing data set
-        - Values less than 1 are interpreted as decimal percent
-    """
+        - `models`
+            - The list of models to make an ensemble out of
+        """
+        self.models = models
+        self.model_weights = [1/len(self.models) for _ in range(len(self.models))]
 
-    # Scale percent
-    if percentTrain < 1:
-        percentTrain *= 100
-
-    # Defaults
-    sortSets = True # No need to make other method rn, sorting isn't that slow
-    xTest = []
-    yTest = []
-    xTrain = []
-    yTrain = []
-
-    # Generate the indicies used for collecting train data
-    dataLen = len(Xdata)
-    numTrainSamples = round(dataLen * percentTrain/100)
-    numTestSamples = dataLen - numTrainSamples
-    trainIndicies = sample(range(dataLen), numTrainSamples)
-    if sortSets:
-        trainIndicies.sort()
-
-    # All-in-one train/test collector (sorted method)
-    if sortSets:
-        crntIndex = 0
-        while crntIndex < dataLen:
-            # Check if its a training index
-            if len(trainIndicies) >= 1:
-                if crntIndex == trainIndicies[0]:
-                    xTrain.append(Xdata[crntIndex])
-                    yTrain.append(Ydata[crntIndex])
-                    
-                    trainIndicies.pop(0)
-                    crntIndex += 1
-                # Else add to test data
+    def fit(self, X, Y, score_type='r2'):
+        """Fit all of the individual models in the ensemble"""
+        # Fit all the models
+        for mi in self.models:
+            try:
+                mi.fit(X, Y, score_type=score_type)
+            except TypeError as e:
+                if 'unexpected keyword argument' in str(e):
+                    mi.fit(X, Y)
                 else:
-                    xTest.append(Xdata[crntIndex])
-                    yTest.append(Ydata[crntIndex])
+                    raise ValueError(e)
 
-                    crntIndex += 1
+    def predict(self, X):
+        # Combine all model outputs
+        output = 0
+        for mi, wi in zip(self.models, self.model_weights):
+            output += wi*mi.predict(X)
+        return output
+
+    def optimize_model_weights(self, X, Y, verbose=False):
+        """Tests each individual model by scoring them via a 5-fold cross validation
+        to the given data. All of these scores are normalized, and then used as the
+        individual models' effective weight in the ensemble."""
+        scores = [cross_val(mi, X, Y, score_type='r2', verbose=verbose).mean() for mi in self.models]
+        scores = [s/sum(scores) for s in scores]
+        self.model_weights = scores
 
-            # Else add to test data
-            else:
-                xTest.append(Xdata[crntIndex])
-                yTest.append(Ydata[crntIndex])
-
-                crntIndex += 1
-
-    # Shape data lists (accoutning for 1D lists)
-    try:
-        xTrain = np.array(xTrain).reshape(numTrainSamples, np.size(Xdata, 1))
-        xTest = np.array(xTest).reshape(numTestSamples, np.size(Xdata, 1))
-    except:
-        xTrain = np.array(xTrain).reshape(numTrainSamples)
-        xTest = np.array(xTest).reshape(numTestSamples)
-    try:
-        yTrain = np.array(yTrain).reshape(numTrainSamples, np.size(Ydata, 1))
-        yTest = np.array(yTest).reshape(numTestSamples, np.size(Ydata, 1))
-    except:
-        yTrain = np.array(yTrain).reshape(numTrainSamples)
-        yTest = np.array(yTest).reshape(numTestSamples)
-
-    return xTrain, xTest, yTrain, yTest
-
-def cross_val(model, X, Y, cv=5, score_type='r2', return_models=False, verbose=0, **kwargs) -> np.ndarray:
-    """
-    Cross validation of model using X and Y with N number of splits
-
-    ## Params
-
-    - `cv`
-        - Number of train/validation split tests to complete
-
-    - `scoreType`
-        - One of the score/error functions avalible in score()
-        - ['r2', 'sse', 'mae', 'mse', 'rae', 'acc']
-        - If a function is given, should be the form:
-            - scorer_func(predictor, X, Y)
-
-    - `return_models`
-        - If True, returns (models, weights) from the models tested and their
-          weights derived from their relative overall score to the others.
-
-    - `verbose`
-        - 0 = No output printing
-        - 1 = Outputs current step/progress
-    """
-
-    # Old 'N' kwarg for cv
-    if 'N' in kwargs.keys():
-        cv = kwargs['N'] 
-
-    # Old for previous gen MCNN
-    if 'train_depth' in kwargs.keys():
-        train_depth = kwargs['train_depth']
-    else:
-        train_depth = 2
-
-    if 'scoreType' in kwargs.keys():
-        score_type = kwargs['scoreType']
-
-    # Check for enough data 
-    if len(X) < cv:
-        raise ValueError(f"Not enough data for {cv} cycles")
-
-    # Verbose settings
-    fit_verbose = False     # Old for previous gen MCNN
-    step_verbose = False    # Verbosity for each CV step
-    if verbose == 1:
-        fit_verbose = False
-        step_verbose = True
-    elif verbose == 2:
-        fit_verbose = True
-        step_verbose = True
-
-    # Main loop
-    if return_models:
-        models = []
-
-    base_model = copy.deepcopy(model)
+    def score(self, X, Y, score_type='r2'):
+        return score_model(self, X, Y, method=score_type)
 
-    scores = []
-    step = round(len(X) / cv)
-    for n in range(cv):
-        # Data Split
-        start = n*step
-        if n == cv-1:
-            stop = len(X)
-        else:
-            stop  = (n+1)*step
 
-        X_val = X[start:stop+1]
-        Y_val = Y[start:stop+1]
+# Dictator Ensemble #
+class DictatorEnsemble():
+    def __init__(self, base_models:list, dictator_model) -> None:
+        """
+        Adds a main (dictator) model to a standard ensemble made
+        from the base models. The main model gets the X and outputs
+        from the base models as an input to create the final output.
+        """
+        self.ensemble = StandardEnsemble(models=base_models)
+        self.dictator = dictator_model
 
-        if len(X.shape) > 1:
-            X_train = np.row_stack([X[:start], X[stop+1:]])
-        else:
-            X_train = np.array(X[:start].tolist() + X[stop+1:].tolist())
+    def _base_predict(self, X):
+        # Gather all the normies outputs for the dictator to use
+        for i, mi in enumerate(self.ensemble.models):
+            if i == 0:
+                # Get first prediction; set to column type for stacking purposes
+                # (This will be the dictator's 'X')
+                output = mi.predict(X)
+                if output.ndim == 1:
+                    output = output.reshape((output.size, 1))
+            else:
+                # Get othe predictions, set to column type
+                new_out = mi.predict(X)
+                if new_out.ndim == 1:
+                    new_out = new_out.reshape((new_out.size, 1))
+                output = np.hstack([output, new_out])
+        return output
+    
+    def predict(self, X):
+        # Use base model predictions to get actual predictions from dictator
+        options = self._base_predict(X)
+        return self.dictator.predict(options)
 
-        if len(Y.shape) > 1:
-            Y_train = np.row_stack([Y[:start], Y[stop+1:]])
-        else:
-            Y_train = np.array(Y[:start].tolist() + Y[stop+1:].tolist())
+    def fit(self, X, Y, score_type='r2'):
+        # Standard fitting
+        self.ensemble.fit(X, Y, score_type=score_type)
 
-        # Train model
-        model = copy.deepcopy(base_model)
+        # Fit dictator
+        options = self._base_predict(X) 
         try:
-            # Old for previous generation MCNN
-            model.fit(X_train, Y_train, Ieta=round(5*train_depth), verbose=fit_verbose)
-        except:
-            model.fit(X_train, Y_train)
-
-        if return_models:
-            models.append(model)
-
-        # Record model score
-        scores.append(score_model(model, X_val, Y_val, method=score_type))
-
-        # Print step results
-        if step_verbose:
-            print(f"Cross-Validation: Step {n+1}/{cv} Complete     ", end='\r')
-
-    # Generate model weights if needed
-    if return_models:
-        weights = [m.score(X, Y) for m in models]
-        weights = np.array(weights)
-        weights /= np.sum(weights)
-        weights = weights.tolist()
-
-    # Finish
-    if step_verbose:
-        # print(f"Cross-Validation: All Steps Completed")
-        print(f"Mean Model {score_type} Validation Score/Error = {np.mean(scores):.4e} +- {np.std(scores):.4e}")
-
-    if return_models:
-        return models, weights
-    else:
-        return np.array(scores)
-
-def score(ytrue, ypred, method='r2') -> float:
-    """
-    Main scorer function given a model's output and true values.
-
-    - `method`
-        - 'r2': R^2 Score
-        - 'sse': -Sum Squared Error
-        - 'mre': -Root Mean Squared Error
-        - 'mae': -Mean Absolute Error
-        - 'rae': Custom R^2-like Score
-        - 'acc'/'accuracy': Accuracy Score
-        - Function: form of `scorer(ytrue, ypred)`
-    """
-
-    # Force correct case
-    method = method.lower()
-
-    ## R^2 Method ##
-    if method == 'r2':
-        return r2d2(ypred, ytrue)
-
-    ## Sum Squared Error ##
-    elif method == 'sse':
-        return -np.sum((ypred - ytrue)**2)
-    
-    ## Mean Root Error ##
-    elif method == 'mre':
-        return -(np.sum((ypred - ytrue)**2) / len(ypred))**0.5
-
-    ## Mean Absolute Error ##
-    elif method == 'mae':
-        return -(1/len(ypred)) * np.sum(np.abs(np.array(ypred) - ytrue))
-
-    ## RAE Score ##
-    elif method == 'rae':
-        return raeScore(ytrue, ypred)
-    
-    ## Accuracy Score ##
-    elif method in ['acc', 'accuracy']:
-        return np.sum(ypred == ytrue) / ypred.size
-    
-    ## Custom Function ##
-    elif isinstance(method, callable):
-        return method(ytrue, ypred)
-
-    # Raise error if one of the possible methods was not given
-    else:
-        raise ValueError(f"Given score type '{method.upper()}' is not one of the avalible types.")
-
-def score_model(model, X:np.ndarray, ytrue:np.ndarray, method='r2') -> float:
-    """
-    Main scorer function given a model, input data, and true values.
-
-    - `method`
-        - 'r2': R^2 Score
-        - 'sse': -Sum Squared Error
-        - 'mre': -Root Mean Squared Error
-        - 'mae': -Mean Absolute Error
-        - 'rae': Custom R^2-like Score
-        - 'acc'/'accuracy': Accuracy Score
-        - Function: form of `scorer(model, X, ytrue)`
-    """
-
-    # Force lowercase
-    if not callable(method):
-        method = method.lower()
-    
-    # Get model output
-    ypred = model.predict(X)
-
-    # For callable scorers given
-    if callable(method):
-        return method(model, X, ytrue)
-    
-    # Otherwise use main score function
-    else:
-        return score(ytrue, ypred, method=method)
-
-
-## Helper/Smol Functions ##
-def r2d2(yModel:np.ndarray, yTrue:np.ndarray):
-    """
-    Returns the R^2 value of the model values (yModel) against the true
-    y data (yTrue).
-    """
-
-    # List checking for idoits like me
-    if type(yModel) == list:
-        yModel = np.array(yModel)
-    if type(yTrue) == list:
-        yTrue = np.array(yTrue)
-
-    # Check if needs to be flattened
-    # if len(yTrue.shape) == 1 and len(yModel.shape) > 1:
-    #     yModel = yModel.flatten()
-    
-    # if len(yTrue.shape) > 1:
-    #     if yTrue.shape[1] == 1:
-    #         yTrue = yTrue.flatten()
-    #         yModel = yModel.flatten()
-    
-    yTrue = yTrue.reshape(yModel.shape)
-
-    # R2 Calc
-    yMean = np.mean(yTrue)
-    RES = np.sum(np.clip(yTrue - yModel, -1e154, 1e154) ** 2)
-    TOT = np.sum((yTrue - yMean) ** 2)
-    if TOT == 0:
-        TOT = np.inf
+            self.dictator.fit(options, Y, score_type=score_type)
+        except TypeError as e:
+            if 'got an unexpected keyword argument' in str(e):
+                self.dictator.fit(options, Y)
+            else:
+                raise ValueError(e)
+        
 
-    return 1 - (RES / TOT)
+    def score(self, X, Y, score_type='r2'):
+        return score_model(self, X, Y, method=score_type)
     
-def raeScore(yTrue:np.ndarray, yPred:np.ndarray):
-    """
-    ## Relative Average Error Score
-
-    ### Preforms the following calculation sequence:
-
-    #### 1 Element-wise Absolute Relative Error (ARE)
-
-        - score_ij = |yTrue_ij - yPred_ij| / |yTrue_ij| -> [0, inf]
-
-    or
-
-        - score_ij = |yPred_ij| -> [0, inf] if yTrue_ij == 0
-
-    #### 2 Get Average ARE
-
-        - <score> = MEAN(score_array)
-
-    #### 3 Convert to return in range [0, 1]
-
-        - RAE = e^(-<score>)
-    """
-
-    # Get locations of zeros and all else
-    zeroLocs = np.where(yTrue == 0)
-    nonZeroLocs = np.where(yTrue != 0)
-
-    # Get scores form zero locations and non-zero locations
-    if len(zeroLocs[0]) > 0:
-        score_zeros = np.mean(np.abs(yPred[zeroLocs]))
-    else:
-        score_zeros = 0
-
-    if len(nonZeroLocs[0]) > 0:
-        score_nonzeros = np.mean(np.abs(yTrue[nonZeroLocs] - yPred[nonZeroLocs]) / np.abs(yTrue[nonZeroLocs]))
-    else:
-        score_nonzeros = 0
 
-    # Get score average
-    avgScore = (score_zeros + score_nonzeros) / 2
-
-    # Get/return RAE
-    return np.e ** (-avgScore)
-
-def normalize(array:np.ndarray):
-    """
-    ## Function
-
-    Normalizes a given array (per col.) such that each point is the z-score for the given 
-    columns mean and standard deviation. The returned array is a copy.
-
-    Columns with only two unique values are automatically converted to be just 0's and 1's
-
-    ## Returns
-
-    normalized_array, mean_std_data
-
-    ## Usage
-
-    The following should generate a normalized array where each column of the array has a
-    mean of (essentially*) 0, and a standard deviation of (essentially*) 1.
-
-    *Due to floating point errors, the values might be off by a very minimal amount
-
-    ```
-    import numpy as np
-    import mcnets as mc
-
-    # Column index to look at
-    col_index = 2
-
-    # Generate an array with 5 columns and 100 samples
-    array = np.random.rand(100, 5)
-    mean = np.mean(array[:, col_index])
-    std  = np.std(array[:, col_index])
-    print("Original array:")
-    print(f"{mean = }")
-    print(f"{std = }")
-
-    # Normalize the array on a per-column basis
-    norm_array, MS_data = mc.normalize(array)
-
-    # Use a columns to prove it is normalized (mean of 0, std of 1)
-    mean = np.mean(norm_array[:, col_index])
-    std  = np.std(norm_array[:, col_index])
-    print()
-    print("Normalized array:")
-    print(f"{mean = }")
-    print(f"{std = }")
-    ```
-    """
-
-    # dtype Check
-    array = array.astype(np.float64).copy()
-
-    # Normalize depending on if many cols or one
-    ms_data = []
-    if len(array.shape) > 1:
-        # Normalize col-by-col
-        for ci in range(array.shape[1]):
-            # Check if is a bool col
-            if len(set(array[:, ci])) == 2:
-                vals = set(array[:, ci])
-                for i, val in enumerate(vals):
-                    array[array == val] = i
-
-                # Dont make M/S adjustments
-                ms_data.append((0, 1))
-                continue
-
-            # Get Mean and STD
-            M = np.mean(array[:, ci])
-            S = np.std(array[:, ci])
-            ms_data.append((M, S))
-
-            # Adjust col in array
-            array[:, ci] -= M
-            array[:, ci] /= S if S != 0 else 1
-            
-    else:
-        # Normalize single-col array
-        M = np.mean(array)
-        S = np.std(array)
-        ms_data.append((M, S))
-
-        array -= M
-        array /= S
-
-    return array, ms_data
-
-def denormalize(normalized_array:np.ndarray, mean_std_data):
-    """
-    ## Function
-
-    Denormalizes an array that has been normalized by the normalize() function, and
-    given the mean_std_data from the array's normalization process. The returned array
-    is a copy.
-
-    ## Returns
-
-    denormalized_array
-
-    ## Usage
-
-    The following should generate a normalized array where each column of the array has a
-    mean of (essentially*) 0, and a standard deviation of (essentially*) 1. After this, it 
-    will denormalize it using this function and bring the array back to its original mean/std.
-
-    *Due to floating point errors, the values might be off by a very minimal amount
-
-    ```
-    import numpy as np
-    import mcnets as mc
-
-    # Column index to look at
-    col_index = 2
-
-    # Generate an array with 5 columns and 100 samples
-    array = np.random.rand(100, 5)
-    mean = np.mean(array[:, col_index])
-    std  = np.std(array[:, col_index])
-    print("Original array:")
-    print(f"{mean = }")
-    print(f"{std = }")
-
-    # Normalize the array on a per-column basis
-    norm_array, MS_data = mc.normalize(array)
-
-    # Use a columns to prove it is normalized (mean of 0, std of 1)
-    mean = np.mean(norm_array[:, col_index])
-    std  = np.std(norm_array[:, col_index])
-    print()
-    print("Normalized array:")
-    print(f"{mean = }")
-    print(f"{std = }")
-
-    # Denormalize the array, per-column
-    denorm_array = mc.denormalize(norm_array, MS_data)
-
-    # Use a columns to prove it is no longer normalized
-    mean = np.mean(denorm_array[:, col_index])
-    std  = np.std(denorm_array[:, col_index])
-    print()
-    print("Denormalized array (Should be same as original):")
-    print(f"{mean = }")
-    print(f"{std = }")
-    ```
+## ================== High-Level Tools ================== ##
+def test_activations(X:np.ndarray, Y:np.ndarray, custom_activations=(), only_custom=False,
+                     cv=5, cv_score_type='r2', nn_kwargs:dict={}, verbose=True):
+    """Builds and test 1-hidden layer Neural Networks each with
+    a different activation to test how well they fit to the given data.
+
+    Returns a sorted (greatest to least) list of (scores, function)
+
+    - `custom_activations`
+        - List of other (external) activation functions to test to the data
+    - `only_custom`
+        - Decides if only the custom activations are tested (as to not waste
+        time testing the normal ones).
+    - `cv`
+        - Number of folds to use for the cross validation test, per activation
+    - `nn_args`
+        - Arguments to pass to the `NeuralNetwork` test models made
+    - `verbose`
+        - Report which CV is currently being done & display score results at end
     """
+    # Setup base arguments in args (if not already sepcified)
+    if "activations" in nn_kwargs.keys():
+        nn_kwargs.pop("activations")
+    if "hidden_counts" not in nn_kwargs.keys():
+        nn_kwargs["hidden_counts"] = (25)
+
+    # Get activations to test
+    af_test_funcs = list(custom_activations)
+    af_test_names = [f.__name__ if callable(f) else f for f in af_test_funcs]
+
+    if not only_custom:
+        af_test_funcs += list(AFDict.values())[2:-3]  # ignore extra lin/linear & experimental last 3
+        af_test_names += list(AFDict.keys())[2:-3]    # ignore extra lin/linear & experimental last 3
 
-    # Make array copy
-    denorm_arr = normalized_array.copy()
-
-    # Get number of columns
-    if len(denorm_arr.shape) > 1:
-        # Do denormalization
-        for col in range(denorm_arr.shape[1]):
-            denorm_arr[:, col] = (denorm_arr[:, col] * mean_std_data[col][1]) + mean_std_data[col][0]
-    else:
-        # Do denormalization (single col)
-        denorm_arr[:] = (denorm_arr[:] * mean_std_data[0][1]) + mean_std_data[0][0]
-
-    return denorm_arr
+    # Test all activations
+    scores = []
+    for i, af in enumerate(af_test_funcs):
+        # Make test model
+        mod = NeuralNetwork(activations=(af), **nn_kwargs)
+        
+        # Test it and record average score
+        scores.append(cross_val(mod, X, Y, score_type=cv_score_type, cv=cv, verbose=False).mean())
+        if verbose:
+            print(f'Finished CV #{i+1}/{len(af_test_funcs)}', end='\r')
+
+    # Report best activations and their names
+    if verbose:
+        # Sort results (Greatest to Smallest)
+        scores_names = list(zip(scores, af_test_names))
+        scores_names.sort(reverse=True)
+
+        # Report scores and such and yeah
+        s1 = 'Activation Tested'
+        s2 = 'Avg. Cross Val Score'
+        print('|', s1, '|', s2, '|')
+        print('='*(len(s1+s2) + 7))
+        for s, afi in scores_names:
+            s1 = f'{afi}'.center(len(s1))
+            s2 = f'{s:.6f}'.center(len(s2))
+            print('|', s1, '|', s2, '|')
+
+    # Return a sorted zip of (scores, functions)
+    scores_funcs = list(zip(scores, af_test_funcs))
+    scores_funcs.sort(reverse=True)
+    return scores_funcs
 
 
 ## Libraries ##
 AFDict = {
         "LIN": lin,
         "LINEAR": lin,
         "IDENTITY": lin,
@@ -1132,21 +834,19 @@
         "RESU": resu,
         "RESU2": resu2,
         "EXP": exp
     }
 
 
 ## Neat Paper/Other References ##
-notes = """
-
+"""
 1. SILU and dSILU activation functions
 Stefan Elfwing, Eiji Uchibe, Kenji Doya,
 Sigmoid-weighted linear units for neural network function approximation in reinforcement learning,
 Neural Networks,
 Volume 107,
 2018,
 Pages 3-11,
 ISSN 0893-6080,
 https://doi.org/10.1016/j.neunet.2017.12.012.
 (https://www.sciencedirect.com/science/article/pii/S0893608017302976)
-
 """
```

### Comparing `mcnets-2.0.5/LICENSE` & `mcnets-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.5/README.md` & `mcnets-2.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 ## Overview
 A very lightweight machine learning package.
 
 Has models that use a unique and simple Monte Carlo approach to training. This method used is
 very generalizable and can therefore be extended to a variety of models both known and new. 
 
-The primary model, the 'NeuralNetwork' class, is on par with other similar models such as the 
-MLPRegressor/MLPClassifier featured in SciKit-Learn, but has more customizability.
+The primary model, the `NeuralNetwork` class, is on par with other similar models such as the 
+`MLPRegressor`/`MLPClassifier` featured in SciKit-Learn, but has more customizability.
 
-In V2.0.5 the list of models avaliable and some of their features includes:
-- NeuralNetwork
+The current list of models avaliable and some of their features includes:
+- `NeuralNetwork`
     - Complete hidden layer size and activations customization
     - Supports externally defined activation functions
     - Allows customizing the input and output activations
     - Easy-access hyperparam ranges for Optuna (via .get_param_ranges_for_optuna)
-- SoupRegressor
+- `SoupRegressor`
     - A unique combination of many various functions with trainable coefficients
     - Typically on-par with the NeuralNetwork; slightly more interpretable
     - Many hyperparams to adjust, with more to come
 
 Some QoL functions and features included are:
-- TTSplit: Included train-test splitter
-- cross_val: Simple cross validation system
+- `TTSplit`: Included train-test splitter
+- `cross_val`: Simple cross validation system
 - Built-in scorer functions with support for external functions
 - Ability to save and load models at any point (.save & load_model)
 - Ability to copy a model via .copy
 
 ## GitHub and QuickStart
 More explanations, examples, and technicals can be found on the GitHub page:
 https://github.com/SciCapt/Monte-Carlo-Neural-Nets
```

### Comparing `mcnets-2.0.5/pyproject.toml` & `mcnets-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "numpy", "joblib"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mcnets"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
   { name="Sean", email="svs.2k15@gmail.com" },
 ]
 description = "Lightweight Machine Learning package with models that train using simple Monte Carlo-like methods."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mcnets-2.0.5/PKG-INFO` & `mcnets-2.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mcnets
-Version: 2.0.5
+Version: 2.0.6
 Summary: Lightweight Machine Learning package with models that train using simple Monte Carlo-like methods.
 Project-URL: Homepage, https://github.com/SciCapt/Monte-Carlo-Neural-Nets
 Project-URL: Bug Tracker, https://github.com/SciCapt/Monte-Carlo-Neural-Nets/issues
 Author-email: Sean <svs.2k15@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,31 +16,31 @@
 
 ## Overview
 A very lightweight machine learning package.
 
 Has models that use a unique and simple Monte Carlo approach to training. This method used is
 very generalizable and can therefore be extended to a variety of models both known and new. 
 
-The primary model, the 'NeuralNetwork' class, is on par with other similar models such as the 
-MLPRegressor/MLPClassifier featured in SciKit-Learn, but has more customizability.
+The primary model, the `NeuralNetwork` class, is on par with other similar models such as the 
+`MLPRegressor`/`MLPClassifier` featured in SciKit-Learn, but has more customizability.
 
-In V2.0.5 the list of models avaliable and some of their features includes:
-- NeuralNetwork
+The current list of models avaliable and some of their features includes:
+- `NeuralNetwork`
     - Complete hidden layer size and activations customization
     - Supports externally defined activation functions
     - Allows customizing the input and output activations
     - Easy-access hyperparam ranges for Optuna (via .get_param_ranges_for_optuna)
-- SoupRegressor
+- `SoupRegressor`
     - A unique combination of many various functions with trainable coefficients
     - Typically on-par with the NeuralNetwork; slightly more interpretable
     - Many hyperparams to adjust, with more to come
 
 Some QoL functions and features included are:
-- TTSplit: Included train-test splitter
-- cross_val: Simple cross validation system
+- `TTSplit`: Included train-test splitter
+- `cross_val`: Simple cross validation system
 - Built-in scorer functions with support for external functions
 - Ability to save and load models at any point (.save & load_model)
 - Ability to copy a model via .copy
 
 ## GitHub and QuickStart
 More explanations, examples, and technicals can be found on the GitHub page:
 https://github.com/SciCapt/Monte-Carlo-Neural-Nets
```

