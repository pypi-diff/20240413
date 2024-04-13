# Comparing `tmp/stelladb-0.2.8.tar.gz` & `tmp/stelladb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stelladb-0.2.8.tar", last modified: Fri Apr  5 02:05:57 2024, max compression
+gzip compressed data, was "stelladb-0.2.9.tar", last modified: Mon Apr  8 22:03:13 2024, max compression
```

## Comparing `stelladb-0.2.8.tar` & `stelladb-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:57.232554 stelladb-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-05 02:05:04.000000 stelladb-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 02:05:57.232554 stelladb-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-05 02:05:04.000000 stelladb-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 02:05:57.236554 stelladb-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 02:05:04.000000 stelladb-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:57.236554 stelladb-0.2.8/stelladb/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 02:05:04.000000 stelladb-0.2.8/stelladb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 02:05:57.236554 stelladb-0.2.8/stelladb/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-05 02:05:04.000000 stelladb-0.2.8/stelladb/db_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-05 02:05:04.000000 stelladb-0.2.8/stelladb/db_vmec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-05 02:05:04.000000 stelladb-0.2.8/stelladb/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-05 02:05:04.000000 stelladb-0.2.8/stelladb/getters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:57.232554 stelladb-0.2.8/stelladb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 02:05:57.000000 stelladb-0.2.8/stelladb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-05 02:05:57.000000 stelladb-0.2.8/stelladb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:05:57.000000 stelladb-0.2.8/stelladb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 02:05:57.000000 stelladb-0.2.8/stelladb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:05:57.000000 stelladb-0.2.8/stelladb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:03:13.923205 stelladb-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 22:02:17.000000 stelladb-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 22:03:13.923205 stelladb-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-08 22:02:17.000000 stelladb-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 22:03:13.923205 stelladb-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 22:02:17.000000 stelladb-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:03:13.923205 stelladb-0.2.9/stelladb/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 22:02:17.000000 stelladb-0.2.9/stelladb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 22:03:13.923205 stelladb-0.2.9/stelladb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-04-08 22:02:17.000000 stelladb-0.2.9/stelladb/db_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-08 22:02:17.000000 stelladb-0.2.9/stelladb/db_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-08 22:02:17.000000 stelladb-0.2.9/stelladb/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-08 22:02:17.000000 stelladb-0.2.9/stelladb/getters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:03:13.923205 stelladb-0.2.9/stelladb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 22:03:13.000000 stelladb-0.2.9/stelladb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-08 22:03:13.000000 stelladb-0.2.9/stelladb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:03:13.000000 stelladb-0.2.9/stelladb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 22:03:13.000000 stelladb-0.2.9/stelladb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 22:03:13.000000 stelladb-0.2.9/stelladb.egg-info/top_level.txt
```

### Comparing `stelladb-0.2.8/LICENSE` & `stelladb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.8/PKG-INFO` & `stelladb-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.8
+Version: 0.2.9
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
@@ -16,17 +16,19 @@
 
 # Stellarator-Database
 Includes the functions required to upload DESC or VMEC results to the stellarator database. You can access the database [here](https://ye2698.mycpanel.princeton.edu/).
 
 This is still a work in progress.
 
 ## Install using pip
+If you are on Linux, WSL or MacOS, you should be able to install `stelladb` directly from PyPi.
 ```bash
 pip install stelladb
 ```
+You may have difficulty installing on Windows due to `simsopt` dependency. More detailed instructions will come for that. For now, you can use the repo on Windows with slight difference on building the environment.
 
 ## Install using GIT
 
 ### Clone GIT repo
 ```bash
 git clone https://github.com/PlasmaControl/Stellarator-Database.git
 ```
@@ -38,14 +40,22 @@
 ### Building conda environment
 ```bash
 conda create --name db 'python>=3.9, <=3.12'
 conda activate db
 pip install -r requirements.txt
 ```
 
+If you are on Windows, `simsopt` might need additional instructions. If you just want to upload DESC results, follow these steps for creating conda environment,
+```bash
+conda create --name db 'python>=3.9, <=3.12'
+conda activate db
+pip install desc-opt selenium
+```
+Then, you can upload to database inside the repo, or anywhere where you can access the module `stelladb`.
+
 ## Sample usage
 
 For more detailed explanation, refer to the `tutorial.ipynb` notebook in the [repo](https://github.com/PlasmaControl/Stellarator-Database.git).
 
 ```python
 from desc.examples import get
 from stelladb import save_to_db_desc
```

### Comparing `stelladb-0.2.8/README.md` & `stelladb-0.2.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Stellarator-Database
 Includes the functions required to upload DESC or VMEC results to the stellarator database. You can access the database [here](https://ye2698.mycpanel.princeton.edu/).
 
 This is still a work in progress.
 
 ## Install using pip
+If you are on Linux, WSL or MacOS, you should be able to install `stelladb` directly from PyPi.
 ```bash
 pip install stelladb
 ```
+You may have difficulty installing on Windows due to `simsopt` dependency. More detailed instructions will come for that. For now, you can use the repo on Windows with slight difference on building the environment.
 
 ## Install using GIT
 
 ### Clone GIT repo
 ```bash
 git clone https://github.com/PlasmaControl/Stellarator-Database.git
 ```
@@ -22,14 +24,22 @@
 ### Building conda environment
 ```bash
 conda create --name db 'python>=3.9, <=3.12'
 conda activate db
 pip install -r requirements.txt
 ```
 
+If you are on Windows, `simsopt` might need additional instructions. If you just want to upload DESC results, follow these steps for creating conda environment,
+```bash
+conda create --name db 'python>=3.9, <=3.12'
+conda activate db
+pip install desc-opt selenium
+```
+Then, you can upload to database inside the repo, or anywhere where you can access the module `stelladb`.
+
 ## Sample usage
 
 For more detailed explanation, refer to the `tutorial.ipynb` notebook in the [repo](https://github.com/PlasmaControl/Stellarator-Database.git).
 
 ```python
 from desc.examples import get
 from stelladb import save_to_db_desc
```

### Comparing `stelladb-0.2.8/setup.py` & `stelladb-0.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     url="https://github.com/PlasmaControl/Stellarator-Database/",
     author="Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen",
     author_email="PlasmaControl@princeton.edu",
     license="MIT",
     keywords="stellarator tokamak equilibrium perturbation mhd "
     + "magnetohydrodynamics stability confinement plasma physics "
     + "optimization design fusion data database",
-    packages=find_packages(),
+    packages=find_packages(exclude=["tutorials"]),
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.9",
 )
```

### Comparing `stelladb-0.2.8/stelladb/db_desc.py` & `stelladb-0.2.9/stelladb/db_desc.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from desc.equilibrium import Equilibrium, EquilibriaFamily
 from desc.grid import LinearGrid
 from desc.vmec_utils import ptolemy_identity_rev, zernike_to_fourier
 from desc.io.hdf5_io import hdf5Reader
 from desc.io.equilibrium_io import load
 
-from .getters import get_hash_config, get_driver, get_hash_desc
+from .getters import get_driver
 from .device import device_or_concept_to_csv
 
 
-def save_to_db_desc(  # pragma: no cover
+def save_to_db_desc(
     eq,
     config_name,
     user,
     description=None,
     provenance=None,
     deviceid=None,
     isDeviceNew=False,
@@ -277,15 +277,15 @@
             os.remove(config_csv_filename)
             if isDeviceNew:
                 os.remove(device_csv_filename)
             if auto_input:
                 os.remove(inputfilename)
 
 
-def desc_to_csv(  # noqa
+def desc_to_csv(
     eq,
     name=None,
     provenance=None,
     description=None,
     inputfilename=None,
     initialization_method="surface",
     user_created=None,
@@ -425,15 +425,18 @@
             eq.compute("iota", grid=rho_grid_dense)["iota"]
         )
         data_desc_runs["iota_min"] = np.min(
             eq.compute("iota", grid=rho_grid_dense)["iota"]
         )
         data_configurations["current_specification"] = "net enclosed current"
         data_desc_runs["current_specification"] = "net enclosed current"
-    Dmerc = eq.compute("D_Mercier", grid=rho_grid)["D_Mercier"]
+
+    rho_mercier = np.linspace(0.1, 1.0, 11, endpoint=True)
+    rho_grid_mercier = LinearGrid(rho=rho_mercier, M=2 * eq.M, N=0, NFP=eq.NFP)
+    Dmerc = eq.compute("D_Mercier", grid=rho_grid_mercier)["D_Mercier"]
     data_desc_runs["D_Mercier_max"] = np.max(Dmerc)
     data_desc_runs["D_Mercier_min"] = np.min(Dmerc)
     data_desc_runs["D_Mercier"] = Dmerc
 
     data_desc_runs["iota_min"] = np.min(eq.compute("iota", grid=rho_grid_dense)["iota"])
     data_desc_runs["pressure_profile"] = eq.pressure(rho)
     data_desc_runs["pressure_max"] = np.max(eq.pressure(rho_dense))
@@ -550,19 +553,14 @@
     data_configurations["date_created"] = kwargs.get("date_created", today)
     data_configurations["date_updated"] = kwargs.get("date_updated", today)
     if user_created is not None:
         data_configurations["user_created"] = user_created
     if user_updated is not None:
         data_configurations["user_updated"] = user_updated
 
-    data_configurations["configid"] = get_hash_config(data_configurations)
-    data_desc_runs["hashkey"] = get_hash_desc(
-        eq, data_desc_runs, data_configurations["configid"]
-    )
-
     csv_columns_desc_runs = list(data_desc_runs.keys())
     csv_columns_desc_runs.sort()
     desc_runs_csv_exists = os.path.isfile(desc_runs_csv_name)
 
     try:
         with open(desc_runs_csv_name, "a+") as csvfile:
             writer = csv.DictWriter(csvfile, fieldnames=csv_columns_desc_runs)
```

### Comparing `stelladb-0.2.8/stelladb/db_vmec.py` & `stelladb-0.2.9/stelladb/db_vmec.py`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.8/stelladb/device.py` & `stelladb-0.2.9/stelladb/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import csv
 import os
 from datetime import date
-from .getters import get_hash_device
 
 
-def device_or_concept_to_csv(  # noqa
+def device_or_concept_to_csv(
     deviceid,
     name=None,
     device_class=None,
     NFP=None,
     description=None,
     stell_sym=False,
     user_created=None,
@@ -56,16 +55,14 @@
     if user_updated is not None:
         devices_and_concepts["user_updated"] = user_updated
 
     today = date.today()
     devices_and_concepts["date_created"] = today
     devices_and_concepts["date_updated"] = today
 
-    devices_and_concepts["hashkey"] = get_hash_device(devices_and_concepts)
-
     csv_columns_desc_runs = list(devices_and_concepts.keys())
     csv_columns_desc_runs.sort()
     desc_runs_csv_exists = os.path.isfile(devices_csv_name)
 
     try:
         with open(devices_csv_name, "a+") as csvfile:
             writer = csv.DictWriter(csvfile, fieldnames=csv_columns_desc_runs)
```

### Comparing `stelladb-0.2.8/stelladb/getters.py` & `stelladb-0.2.9/stelladb/getters.py`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.8/stelladb.egg-info/PKG-INFO` & `stelladb-0.2.9/stelladb.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.8
+Version: 0.2.9
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
@@ -16,17 +16,19 @@
 
 # Stellarator-Database
 Includes the functions required to upload DESC or VMEC results to the stellarator database. You can access the database [here](https://ye2698.mycpanel.princeton.edu/).
 
 This is still a work in progress.
 
 ## Install using pip
+If you are on Linux, WSL or MacOS, you should be able to install `stelladb` directly from PyPi.
 ```bash
 pip install stelladb
 ```
+You may have difficulty installing on Windows due to `simsopt` dependency. More detailed instructions will come for that. For now, you can use the repo on Windows with slight difference on building the environment.
 
 ## Install using GIT
 
 ### Clone GIT repo
 ```bash
 git clone https://github.com/PlasmaControl/Stellarator-Database.git
 ```
@@ -38,14 +40,22 @@
 ### Building conda environment
 ```bash
 conda create --name db 'python>=3.9, <=3.12'
 conda activate db
 pip install -r requirements.txt
 ```
 
+If you are on Windows, `simsopt` might need additional instructions. If you just want to upload DESC results, follow these steps for creating conda environment,
+```bash
+conda create --name db 'python>=3.9, <=3.12'
+conda activate db
+pip install desc-opt selenium
+```
+Then, you can upload to database inside the repo, or anywhere where you can access the module `stelladb`.
+
 ## Sample usage
 
 For more detailed explanation, refer to the `tutorial.ipynb` notebook in the [repo](https://github.com/PlasmaControl/Stellarator-Database.git).
 
 ```python
 from desc.examples import get
 from stelladb import save_to_db_desc
```

