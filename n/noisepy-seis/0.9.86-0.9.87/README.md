# Comparing `tmp/noisepy_seis-0.9.86.tar.gz` & `tmp/noisepy_seis-0.9.87.tar.gz`

## Comparing `noisepy_seis-0.9.86.tar` & `noisepy_seis-0.9.87.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/functions_2019/S0B_to_ASDF_2019.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/functions_2019/noise_module.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_plotting.py
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_utils.py
--rw-r--r--   0        0        0    50445 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/monitoring_utils.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/correlate.py
--rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/fdsn_download.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/main.py
--rw-r--r--   0        0        0    47935 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/stack.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/LICENSE
--rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/pyproject.toml
--rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/PKG-INFO
+-rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/functions_2019/S0B_to_ASDF_2019.py
+-rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/functions_2019/noise_module.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/imaging/dispersion_analysis.py
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/monitoring/attenuation_utils.py
+-rw-r--r--   0        0        0    50445 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/monitoring/monitoring_methods.py
+-rw-r--r--   0        0        0     8154 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/monitoring/monitoring_utils.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/monitoring/plotting_attenuation.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/correlate.py
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/fdsn_download.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0    48062 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/src/noisepy/seis/stack.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/LICENSE
+-rw-r--r--   0        0        0     8003 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/pyproject.toml
+-rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 noisepy_seis-0.9.87/PKG-INFO
```

### Comparing `noisepy_seis-0.9.86/src/noisepy/functions_2019/S0B_to_ASDF_2019.py` & `noisepy_seis-0.9.87/src/noisepy/functions_2019/S0B_to_ASDF_2019.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/functions_2019/noise_module.py` & `noisepy_seis-0.9.87/src/noisepy/functions_2019/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_plotting.py` & `noisepy_seis-0.9.87/src/noisepy/monitoring/plotting_attenuation.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_utils.py` & `noisepy_seis-0.9.87/src/noisepy/monitoring/attenuation_utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/monitoring/monitoring_utils.py` & `noisepy_seis-0.9.87/src/noisepy/monitoring/monitoring_methods.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.87/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/correlate.py` & `noisepy_seis-0.9.87/src/noisepy/seis/correlate.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/fdsn_download.py` & `noisepy_seis-0.9.87/src/noisepy/seis/fdsn_download.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/main.py` & `noisepy_seis-0.9.87/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.87/src/noisepy/seis/noise_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,21 +243,26 @@
     dataS:      2D matrix of the segmented data
     """
     # define return variables first
     source_params = []
     dataS_t = []
     dataS = []
 
-    # useful parameters for trace sliding
-    nseg = int(np.floor((fc_para.inc_hours / 24 * 86400 - fc_para.cc_len) / fc_para.step))
     sps = int(ch_data.sampling_rate)
     starttime = ch_data.start_timestamp
     # copy data into array
     data = ch_data.data
 
+    if fc_para.inc_hours == 0:
+        # specifically for DAS data, set the inc_hours to 0
+        nseg = 1
+    else:
+        # useful parameters for trace sliding
+        nseg = int(np.floor((fc_para.inc_hours / 24 * 86400 - fc_para.cc_len) / fc_para.step))
+
     # if the data is shorter than the tim chunck, return zero values
     if data.size < sps * fc_para.inc_hours * 3600:
         logger.warning(
             f"The data ({data.size}) is shorter than the time chunk ({sps*fc_para.inc_hours*3600})"
             ", returning zero values."
         )
         return source_params, dataS_t, dataS
```

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.87/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/stack.py` & `noisepy_seis-0.9.87/src/noisepy/seis/stack.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.87/src/noisepy/imaging/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/.gitignore` & `noisepy_seis-0.9.87/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/LICENSE` & `noisepy_seis-0.9.87/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.86/README.md` & `noisepy_seis-0.9.87/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,118 +1,105 @@
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
 
-Disclaimer: this code should not be used "as-is" and not run like a blackbox. The user is expected to change local paths and parameters. Submit an issue to github with information such as the scripts+error messages to debug.
-
-Detailed documentation can be found at https://noisepy.github.io/NoisePy/
-
 [![Documentation Status](https://github.com/noisepy/NoisePy/actions/workflows/notebooks.yml/badge.svg)](https://noisepy.github.io/NoisePy/)
 [![Build Status](https://github.com/noisepy/NoisePy/actions/workflows/test.yaml/badge.svg)](https://github.com/noisepy/NoisePy/actions/workflows/test.yaml)
 [![Codecov](https://codecov.io/gh/noisepy/NoisePy/branch/main/graph/badge.svg)](https://codecov.io/gh/noisepy/NoisePy)
 [![DOI](https://zenodo.org/badge/157871462.svg)](https://zenodo.org/badge/latestdoi/157871462)
 
 <img src="https://raw.githubusercontent.com/noisepy/NoisePy/main/docs_old/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
 NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to [contribute](CONTRIBUTING.md).
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
-### Note the order of the command lines below matters ###
+**Note the order of the command lines below matters**
 
-## With Conda and pip:
+## With Conda and pip
 ```bash
-conda create -n noisepy python=3.10 pip
+conda create -n noisepy -y python=3.10 pip
 conda activate noisepy
 pip install noisepy-seis
 ```
 
-## With Conda and pip and MPI support:
+## With Conda and pip and MPI support
 ```bash
-conda create -n noisepy python=3.10 pip
+conda create -n noisepy -y python=3.10 pip mpi4py
 conda activate noisepy
-conda install -c conda-forge openmpi
 pip install noisepy-seis[mpi]
 ```
 
-## With virtual environment:
+## With virtual environment
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis
 ```
-## With virtual environment and MPI support:
+
+## With virtual environment and MPI support
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis[mpi]
 ```
 
-
 # Functionality
 Here is a list of features of the package:
 * download continous noise data based:
    + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
    + on AWS S3 bucket calls, with a test on the SCEDC AWS Open Dataset.
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers scripts to precondition data sets before cross correlations. This involves working with gappy data from various formats (SAC/miniSEED) and storing it on local in ASDF.
-
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * **Applications module**:
    + *Ambient noise monitoring*: measure dv/v using a wide variety of techniques in time, fourier, and wavelet domain (Yuan et al., 2021)
    + *Surface wave dispersion*: construct dispersion images using conventional techniques.
 
-
-
 # Usage
 
 To run the code on a single core, open the terminal and activate the noisepy environment before run following commands. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster.
 
 ## Deploy using Docker
 We use I/O on disk, so users need root access to the file system. To install rootless docker, see instructions [here](https://docs.docker.com/engine/security/rootless/#install).
 ```bash
 docker pull  ghcr.io/noisepy/noisepy:latest
 docker run -v ~/tmp:/tmp ghcr.io/noisepy/noisepy:latest cross_correlate --path /tmp
 ```
 
 # Tutorials
-A short tutorial on how to use NoisePy-seis can be is available as a [web page](https://noisepy.github.io/NoisePy/noisepy_scedc_tutorial.html) or [Jupyter notebook](https://github.com/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb) and can be
+A short tutorial on how to use NoisePy can be is available as a [web page](https://noisepy.github.io/NoisePy/noisepy_scedc_tutorial.html) or [Jupyter notebook](https://github.com/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb) and can be
 [run directly in Colab](https://colab.research.google.com/github/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb).
 
-
-This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
+This tutorial presents one simple example of how NoisePy might work. We strongly encourage you to download the NoisePy package and play it on your own! If you have any comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
-Marine Denolle (mdenolle@uw.edu).
+Marine Denolle (mdenolle@uw.edu)
+Yiyu Ni (niyiyu@uw.edu)
 
 ## Taxonomy
 Taxonomy of the NoisePy variables.
 
 * ``station`` refers to the site that has the seismic instruments that records ground shaking.
-* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
+* ``channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
 * ``ista`` is the index name for looping over stations
-
 * ``cc_len`` correlation length, basic window length in seconds
 * ``step`` is the window that get skipped when sliding windows in seconds
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
-
 # Acknowledgements
-
-## Contributing
-
 Thanks to our contributors so far!
 
 [![Contributors](https://contrib.rocks/image?repo=noisepy/NoisePy)](https://github.com/noisepy/NoisePy/graphs/contributors)
 
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
@@ -123,9 +110,8 @@
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
 * (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
 
 * (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
-
 This research received software engineering support from the University of Washington’s Scientific Software Engineering Center ([SSEC](https://escience.washington.edu/software-engineering/ssec/)) supported by Schmidt Futures, as part of the Virtual Institute for Scientific Software (VISS). We would like to acknowledge [Carlos Garcia Jurado Suarez](https://github.com/carlosgjs) and [Nicholas Rich](https://github.com/nrich20) for their collaboration and contributions to the software.
```

### Comparing `noisepy_seis-0.9.86/pyproject.toml` & `noisepy_seis-0.9.87/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "s3fs==2023.4.0,<2024.0.0",
     "zarr==2.14.2",
     "aiobotocore==2.5.2", # "2.5.3 is broken"
     "pydantic==2.3.0",
     "PyYAML==6.0",
     "pydantic-yaml==1.0",
     "psutil>=5.9.5,<6.0.0",
-    "noisepy-seis-io>=0.1.13",
+    "noisepy-seis-io>=0.1.14",
     "scipy==1.12.0"
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/noisepy/NoisePy"
```

### Comparing `noisepy_seis-0.9.86/PKG-INFO` & `noisepy_seis-0.9.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noisepy-seis
-Version: 0.9.86
+Version: 0.9.87
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/noisepy/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <Chengxin.Jiang1@anu.edu.au>, Yiyu Ni <niyiyu@uw.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.9
 Requires-Dist: aiobotocore==2.5.2
 Requires-Dist: datetimerange<3.0.0,>=2.0.0
 Requires-Dist: diskcache<6.0.0,>=5.6.1
 Requires-Dist: fsspec<2024.0.0,>=2023.4.0
 Requires-Dist: h5py<4.0.0,>=3.8.0
-Requires-Dist: noisepy-seis-io>=0.1.13
+Requires-Dist: noisepy-seis-io>=0.1.14
 Requires-Dist: numba<1.0.0,>=0.57.0
 Requires-Dist: numpy<2.0.0,>=1.22.0
 Requires-Dist: pandas<2.0.0,>=1.5.3
 Requires-Dist: psutil<6.0.0,>=5.9.5
 Requires-Dist: pyasdf<1.0.0,>=0.7.5
 Requires-Dist: pycwt<1.0.0,>=0.3.0a22
 Requires-Dist: pydantic-yaml==1.0
@@ -63,122 +63,109 @@
 Provides-Extra: sql
 Requires-Dist: sqlite3-0611; extra == 'sql'
 Description-Content-Type: text/markdown
 
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
 
-Disclaimer: this code should not be used "as-is" and not run like a blackbox. The user is expected to change local paths and parameters. Submit an issue to github with information such as the scripts+error messages to debug.
-
-Detailed documentation can be found at https://noisepy.github.io/NoisePy/
-
 [![Documentation Status](https://github.com/noisepy/NoisePy/actions/workflows/notebooks.yml/badge.svg)](https://noisepy.github.io/NoisePy/)
 [![Build Status](https://github.com/noisepy/NoisePy/actions/workflows/test.yaml/badge.svg)](https://github.com/noisepy/NoisePy/actions/workflows/test.yaml)
 [![Codecov](https://codecov.io/gh/noisepy/NoisePy/branch/main/graph/badge.svg)](https://codecov.io/gh/noisepy/NoisePy)
 [![DOI](https://zenodo.org/badge/157871462.svg)](https://zenodo.org/badge/latestdoi/157871462)
 
 <img src="https://raw.githubusercontent.com/noisepy/NoisePy/main/docs_old/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
 NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to [contribute](CONTRIBUTING.md).
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
-### Note the order of the command lines below matters ###
+**Note the order of the command lines below matters**
 
-## With Conda and pip:
+## With Conda and pip
 ```bash
-conda create -n noisepy python=3.10 pip
+conda create -n noisepy -y python=3.10 pip
 conda activate noisepy
 pip install noisepy-seis
 ```
 
-## With Conda and pip and MPI support:
+## With Conda and pip and MPI support
 ```bash
-conda create -n noisepy python=3.10 pip
+conda create -n noisepy -y python=3.10 pip mpi4py
 conda activate noisepy
-conda install -c conda-forge openmpi
 pip install noisepy-seis[mpi]
 ```
 
-## With virtual environment:
+## With virtual environment
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis
 ```
-## With virtual environment and MPI support:
+
+## With virtual environment and MPI support
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis[mpi]
 ```
 
-
 # Functionality
 Here is a list of features of the package:
 * download continous noise data based:
    + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
    + on AWS S3 bucket calls, with a test on the SCEDC AWS Open Dataset.
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers scripts to precondition data sets before cross correlations. This involves working with gappy data from various formats (SAC/miniSEED) and storing it on local in ASDF.
-
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * **Applications module**:
    + *Ambient noise monitoring*: measure dv/v using a wide variety of techniques in time, fourier, and wavelet domain (Yuan et al., 2021)
    + *Surface wave dispersion*: construct dispersion images using conventional techniques.
 
-
-
 # Usage
 
 To run the code on a single core, open the terminal and activate the noisepy environment before run following commands. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster.
 
 ## Deploy using Docker
 We use I/O on disk, so users need root access to the file system. To install rootless docker, see instructions [here](https://docs.docker.com/engine/security/rootless/#install).
 ```bash
 docker pull  ghcr.io/noisepy/noisepy:latest
 docker run -v ~/tmp:/tmp ghcr.io/noisepy/noisepy:latest cross_correlate --path /tmp
 ```
 
 # Tutorials
-A short tutorial on how to use NoisePy-seis can be is available as a [web page](https://noisepy.github.io/NoisePy/noisepy_scedc_tutorial.html) or [Jupyter notebook](https://github.com/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb) and can be
+A short tutorial on how to use NoisePy can be is available as a [web page](https://noisepy.github.io/NoisePy/noisepy_scedc_tutorial.html) or [Jupyter notebook](https://github.com/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb) and can be
 [run directly in Colab](https://colab.research.google.com/github/noisepy/NoisePy/blob/main/tutorials/noisepy_scedc_tutorial.ipynb).
 
-
-This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
+This tutorial presents one simple example of how NoisePy might work. We strongly encourage you to download the NoisePy package and play it on your own! If you have any comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
-Marine Denolle (mdenolle@uw.edu).
+Marine Denolle (mdenolle@uw.edu)
+Yiyu Ni (niyiyu@uw.edu)
 
 ## Taxonomy
 Taxonomy of the NoisePy variables.
 
 * ``station`` refers to the site that has the seismic instruments that records ground shaking.
-* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
+* ``channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
 * ``ista`` is the index name for looping over stations
-
 * ``cc_len`` correlation length, basic window length in seconds
 * ``step`` is the window that get skipped when sliding windows in seconds
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
-
 # Acknowledgements
-
-## Contributing
-
 Thanks to our contributors so far!
 
 [![Contributors](https://contrib.rocks/image?repo=noisepy/NoisePy)](https://github.com/noisepy/NoisePy/graphs/contributors)
 
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
@@ -189,9 +176,8 @@
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
 * (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
 
 * (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
-
 This research received software engineering support from the University of Washington’s Scientific Software Engineering Center ([SSEC](https://escience.washington.edu/software-engineering/ssec/)) supported by Schmidt Futures, as part of the Virtual Institute for Scientific Software (VISS). We would like to acknowledge [Carlos Garcia Jurado Suarez](https://github.com/carlosgjs) and [Nicholas Rich](https://github.com/nrich20) for their collaboration and contributions to the software.
```

