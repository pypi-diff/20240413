# Comparing `tmp/epidemik-0.0.19.tar.gz` & `tmp/epidemik-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.19.tar", last modified: Fri Apr 12 20:36:32 2024, max compression
+gzip compressed data, was "epidemik-0.0.20.tar", last modified: Sat Apr 13 16:10:52 2024, max compression
```

## Comparing `epidemik-0.0.19.tar` & `epidemik-0.0.20.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837699 epidemik-0.0.19/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.19/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     6348 2024-04-12 20:36:32.837494 epidemik-0.0.19/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     5647 2024-04-12 20:16:57.000000 epidemik-0.0.19/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      852 2024-04-12 20:34:33.000000 epidemik-0.0.19/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-12 20:36:32.837739 epidemik-0.0.19/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.834674 epidemik-0.0.19/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.836303 epidemik-0.0.19/src/epidemik/
--rw-r--r--   0 bgoncalves   (501) staff       (20)    18449 2024-04-12 20:04:35.000000 epidemik-0.0.19/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)    11348 2024-04-11 17:58:26.000000 epidemik-0.0.19/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.19/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      329 2024-04-12 20:36:11.000000 epidemik-0.0.19/src/epidemik/__init__.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      264 2024-04-12 20:04:35.000000 epidemik-0.0.19/src/epidemik/utils.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837263 epidemik-0.0.19/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     6348 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)       72 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837077 epidemik-0.0.19/tests/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.19/tests/tests_EpiModel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 16:10:43.000000 epidemik-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-13 16:10:52.133417 epidemik-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-13 16:10:43.000000 epidemik-0.0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-13 16:10:43.000000 epidemik-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:10:52.133417 epidemik-0.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.129418 epidemik-0.0.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.129418 epidemik-0.0.20/src/epidemik/
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/src/epidemik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-13 16:10:43.000000 epidemik-0.0.20/tests/tests_EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 16:10:43.000000 epidemik-0.0.20/tests/tests_MetaEpiModel.py
```

### Comparing `epidemik-0.0.19/LICENSE` & `epidemik-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.19/PKG-INFO` & `epidemik-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.19
+Version: 0.0.20
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.19 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.20 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-
```

### Comparing `epidemik-0.0.19/README.md` & `epidemik-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.19/pyproject.toml` & `epidemik-0.0.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.19/src/epidemik/EpiModel.py` & `epidemik-0.0.20/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.19/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.20/src/epidemik/MetaEpiModel.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 tqdm.pandas()
 
 class MetaEpiModel:
     """Simple Epidemic Model Implementation
     
         Provides a way to implement and numerically integrate 
     """
-    def __init__(self, travel_graph, populations):
+    def __init__(self, travel_graph, populations, population='Population'):
         """
         Initialize the EpiModel object
         
         Parameters:
         - compartments_: list of strings, optional
             List of compartment names
         
         Returns:
         None
         """
         self.travel_graph = travel_graph
         self.populations = populations
+        self.population = population
 
         models = {}
 
         self.transitions = None
         self.prototype = None
         self.seasonality = None
 
@@ -118,33 +119,39 @@
         
         Returns:
         None
         """
         for state in self.models:  
             self.models[state].add_vaccination(source, target, rate, start)
     
+    def R0(self):
+        key = list(self.models.keys())[0]
+        return self.models[key].R0()
+
     def get_state(self, state):
         """
         Return a reference to a state EpiModel object
 
         Parameters:
         - state: string
             Name of the state to return
         """
 
         return self.models[state]
 
-    def _initialize_populations(self, susceptible):
+    def _initialize_populations(self, susceptible, population=None):
         columns = list(self.transitions.nodes())
         self.compartments_ = pd.DataFrame(np.zeros((self.travel_graph.shape[0], len(columns)), dtype='int'), columns=columns)
         self.compartments_.index = self.populations.index
 
-        susceptible = list(self.prototype._get_susceptible())[0]
+        if population is None:
+            population = self.population
 
-        self.compartments_.loc[:, susceptible] = self.populations['Population']
+        for state in self.compartments_.index:
+            self.compartments_.loc[state, susceptible]  = self.populations.loc[state, population]
 
     def _run_travel(self, compartments_, travel):
         def travel_step(x, populations):
             n = populations.loc[x.name]
             p = travel.loc[x.name].values.tolist()
             output = np.random.multinomial(n, p)
 
@@ -156,17 +163,17 @@
         # Travel occurs independently for each compartment
         # since we don't allow in-flight transitions
         for comp in compartments_.columns:
             new_compartments[comp] = travel.apply(travel_step, populations=compartments_[comp]).sum(axis=1)
             
         return new_compartments
     
-    def _run_spread(self, models, compartments_, seasonality):
+    def _run_spread(self):
         for state in self.compartments_.index:
-            pop = dict(self.compartments_.loc[state].to_dict())
+            pop = self.compartments_.loc[state].to_dict()
             self.models[state].single_step(**pop)
             self.compartments_.loc[state] = self.models[state].values_.iloc[[-1]].values[0]
 
     def simulate(self, timestamp, t_min=1, seasonality=None, seed_state=None, susceptible='S', **kwargs):
         if seed_state is None:
             raise NotInitialized("You have to specify the seed_state")
 
@@ -176,17 +183,23 @@
 
         for comp in kwargs:
             if comp != susceptible and comp in pos:
                 self.compartments_.loc[seed_state, comp] += kwargs[comp]
                 self.compartments_.loc[seed_state, susceptible] -= kwargs[comp]
 
         for t in tqdm(range(t_min, timestamp+1), total=timestamp):
-            self._run_spread(self.models, self.compartments_, self.seasonality)
+            self._run_spread()
             self.compartments_ = self._run_travel(self.compartments_, self.travel_graph)
     
+    def integrate(self, **kwargs):
+        raise NotImplementedError("MetaEpiModel doesn't support direct integration of the ODE")
+
+    def draw_model(self):
+        return self.models.iloc[0].draw_model()
+
     def plot(self, title=None, normed=True, layout=None, **kwargs):
         if layout is None:
             n_pop = self.travel_graph.shape[0]
             N = int(np.round(np.sqrt(n_pop), 0)+1)
 
             coords = [[i%N, i//N] for i in range(n_pop)]
             coords = pd.DataFrame(coords, columns=['x', 'y'])
@@ -284,52 +297,8 @@
 
         ax.imshow(peaks.loc[self.travel_graph.index].fillna(0).values, cmap=plt.cm.rainbow)
         ax.set_yticks(np.arange(0, len(self.travel_graph.index)))
         ax.set_yticklabels(self.travel_graph.index, fontsize=10)
         ax.set_xticks(np.arange(0, peaks.shape[1], 3))
         ax.set_xticklabels(np.arange(0, peaks.shape[1], 3), fontsize=10)
         # ax.set_aspect(1)
-        fig.patch.set_facecolor('#FFFFFF')
-    
-if __name__ == '__main__':
-
-    Nk_uk = pd.read_csv("data/United Kingdom-2020.csv", index_col=0)
-    Nk_ke = pd.read_csv("data/Kenya-2020.csv", index_col=0)
-
-    contacts_uk = pd.read_excel("data/MUestimates_all_locations_2.xlsx", sheet_name="United Kingdom of Great Britain", header=None)
-    contacts_ke = pd.read_excel("data/MUestimates_all_locations_1.xlsx", sheet_name="Kenya")
-
-    beta = 0.05
-    mu = 0.1
-
-    SIR_uk = EpiModel()
-    SIR_uk.add_interaction('S', 'I', 'I', beta)
-    SIR_uk.add_spontaneous('I', 'R', mu)
-
-
-    SIR_ke = EpiModel()
-    SIR_ke.add_interaction('S', 'I', 'I', beta)
-    SIR_ke.add_spontaneous('I', 'R', mu)
-
-    N_uk = int(Nk_uk.sum())
-    N_ke = int(Nk_ke.sum())
-
-
-    SIR_uk.add_age_structure(contacts_uk, Nk_uk)
-    SIR_ke.add_age_structure(contacts_ke, Nk_ke)
-
-    SIR_uk.integrate(100, S=N_uk*.99, I=N_uk*.01, R=0)
-    SIR_ke.integrate(100, S=N_ke*.99, I=N_ke*.01, R=0)
-
-    fig, ax = plt.subplots(1)
-    SIR_uk.draw_model(ax)
-    fig.savefig('SIR_model.png', dpi=300, facecolor='white')
-
-    fig, ax = plt.subplots(1)
-
-    (SIR_uk['I']*100/N_uk).plot(ax=ax)
-    (SIR_ke['I']*100/N_ke).plot(ax=ax)
-    ax.legend(['UK', 'Kenya'])
-    ax.set_xlabel('Time')
-    ax.set_ylabel('Population (%)')
-
-    fig.savefig('SIR_age.png', dpi=300, facecolor='white')
+        fig.patch.set_facecolor('#FFFFFF')
```

### Comparing `epidemik-0.0.19/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.20/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.19/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.20/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.19
+Version: 0.0.20
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.19 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.20 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-
```

### Comparing `epidemik-0.0.19/tests/tests_EpiModel.py` & `epidemik-0.0.20/tests/tests_EpiModel.py`

 * *Files identical despite different names*

