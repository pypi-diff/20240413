# Comparing `tmp/the_real_genotools-1.2.1.tar.gz` & `tmp/the_real_genotools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_real_genotools-1.2.1.tar", last modified: Tue Feb 27 17:00:35 2024, max compression
+gzip compressed data, was "the_real_genotools-1.2.2.tar", last modified: Fri Apr 12 23:10:48 2024, max compression
```

## Comparing `the_real_genotools-1.2.1.tar` & `the_real_genotools-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vitaled2 (524967535) 1360859114        0 2024-02-27 17:00:35.511451 the_real_genotools-1.2.1/
--rw-r--r--   0 vitaled2 (524967535) 1360859114    11357 2023-12-11 21:57:13.000000 the_real_genotools-1.2.1/LICENSE
--rw-r--r--   0 vitaled2 (524967535) 1360859114     4305 2024-02-27 17:00:35.511308 the_real_genotools-1.2.1/PKG-INFO
--rwxr-xr-x   0 vitaled2 (524967535) 1360859114     3835 2024-01-05 20:44:01.000000 the_real_genotools-1.2.1/README.md
-drwxr-xr-x   0 vitaled2 (524967535) 1360859114        0 2024-02-27 17:00:35.505358 the_real_genotools-1.2.1/genotools/
--rwxr-xr-x   0 vitaled2 (524967535) 1360859114      688 2023-12-11 20:48:31.000000 the_real_genotools-1.2.1/genotools/__init__.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    10948 2024-02-26 23:28:32.000000 the_real_genotools-1.2.1/genotools/__main__.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    48333 2024-01-10 23:20:07.000000 the_real_genotools-1.2.1/genotools/ancestry.py
-drwxr-xr-x   0 vitaled2 (524967535) 1360859114        0 2024-02-27 17:00:35.510187 the_real_genotools-1.2.1/genotools/container/
--rw-r--r--   0 vitaled2 (524967535) 1360859114      266 2023-12-26 14:04:51.000000 the_real_genotools-1.2.1/genotools/container/Dockerfile
--rw-r--r--   0 vitaled2 (524967535) 1360859114  1169711 2023-09-29 14:53:34.000000 the_real_genotools-1.2.1/genotools/container/GP2_merge_APRIL_2023_ready_genotools_callrate_sex_ancestry_umap_linearsvc_ancestry_model.pkl
--rwxr-xr-x   0 vitaled2 (524967535) 1360859114        0 2023-11-08 23:51:50.000000 the_real_genotools-1.2.1/genotools/container/__init__.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114      141 2023-09-29 14:53:34.000000 the_real_genotools-1.2.1/genotools/container/requirements.txt
--rw-r--r--   0 vitaled2 (524967535) 1360859114     1600 2023-09-29 14:53:34.000000 the_real_genotools-1.2.1/genotools/container/run.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114     5917 2024-02-27 01:25:49.000000 the_real_genotools-1.2.1/genotools/dependencies.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114     5275 2023-12-13 19:52:07.000000 the_real_genotools-1.2.1/genotools/download_refs.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    13158 2024-02-26 23:28:32.000000 the_real_genotools-1.2.1/genotools/gwas.py
--rwxr-xr-x   0 vitaled2 (524967535) 1360859114     6909 2023-12-11 20:48:31.000000 the_real_genotools-1.2.1/genotools/imputation.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    14278 2024-02-26 23:28:32.000000 the_real_genotools-1.2.1/genotools/pipeline.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    39640 2024-02-26 23:28:32.000000 the_real_genotools-1.2.1/genotools/qc.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114    22877 2023-12-20 22:27:06.000000 the_real_genotools-1.2.1/genotools/utils.py
--rw-r--r--   0 vitaled2 (524967535) 1360859114       38 2024-02-27 17:00:35.511507 the_real_genotools-1.2.1/setup.cfg
--rwxr-xr-x   0 vitaled2 (524967535) 1360859114     2276 2024-02-27 16:56:36.000000 the_real_genotools-1.2.1/setup.py
-drwxr-xr-x   0 vitaled2 (524967535) 1360859114        0 2024-02-27 17:00:35.511053 the_real_genotools-1.2.1/the_real_genotools.egg-info/
--rw-r--r--   0 vitaled2 (524967535) 1360859114     4305 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/PKG-INFO
--rw-r--r--   0 vitaled2 (524967535) 1360859114      738 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/SOURCES.txt
--rw-r--r--   0 vitaled2 (524967535) 1360859114        1 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/dependency_links.txt
--rw-r--r--   0 vitaled2 (524967535) 1360859114      122 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/entry_points.txt
--rw-r--r--   0 vitaled2 (524967535) 1360859114      353 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/requires.txt
--rw-r--r--   0 vitaled2 (524967535) 1360859114       10 2024-02-27 17:00:35.000000 the_real_genotools-1.2.1/the_real_genotools.egg-info/top_level.txt
+drwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        0 2024-04-12 23:10:48.664892 the_real_genotools-1.2.2/
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    11357 2023-12-11 21:57:13.000000 the_real_genotools-1.2.2/LICENSE
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     4646 2024-04-12 23:10:48.664729 the_real_genotools-1.2.2/PKG-INFO
+-rwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     4176 2024-03-28 01:05:52.000000 the_real_genotools-1.2.2/README.md
+drwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        0 2024-04-12 23:10:48.659533 the_real_genotools-1.2.2/genotools/
+-rwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      688 2023-12-11 20:48:31.000000 the_real_genotools-1.2.2/genotools/__init__.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    10963 2024-03-28 01:05:52.000000 the_real_genotools-1.2.2/genotools/__main__.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    48333 2024-01-10 23:20:07.000000 the_real_genotools-1.2.2/genotools/ancestry.py
+drwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        0 2024-04-12 23:10:48.663387 the_real_genotools-1.2.2/genotools/container/
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      266 2023-12-26 14:04:51.000000 the_real_genotools-1.2.2/genotools/container/Dockerfile
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)  1169711 2023-09-29 14:53:34.000000 the_real_genotools-1.2.2/genotools/container/GP2_merge_APRIL_2023_ready_genotools_callrate_sex_ancestry_umap_linearsvc_ancestry_model.pkl
+-rwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        0 2023-11-08 23:51:50.000000 the_real_genotools-1.2.2/genotools/container/__init__.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      141 2023-09-29 14:53:34.000000 the_real_genotools-1.2.2/genotools/container/requirements.txt
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     1600 2023-09-29 14:53:34.000000 the_real_genotools-1.2.2/genotools/container/run.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     6729 2024-03-28 01:05:52.000000 the_real_genotools-1.2.2/genotools/dependencies.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     5275 2023-12-13 19:52:07.000000 the_real_genotools-1.2.2/genotools/download_refs.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    13077 2024-04-12 14:37:36.000000 the_real_genotools-1.2.2/genotools/gwas.py
+-rwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     6909 2023-12-11 20:48:31.000000 the_real_genotools-1.2.2/genotools/imputation.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    14765 2024-03-28 01:05:52.000000 the_real_genotools-1.2.2/genotools/pipeline.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    45404 2024-04-12 14:37:36.000000 the_real_genotools-1.2.2/genotools/qc.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)    22822 2024-04-12 14:37:36.000000 the_real_genotools-1.2.2/genotools/utils.py
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)       38 2024-04-12 23:10:48.664942 the_real_genotools-1.2.2/setup.cfg
+-rwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     2276 2024-04-12 23:08:47.000000 the_real_genotools-1.2.2/setup.py
+drwxr-xr-x   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        0 2024-04-12 23:10:48.664480 the_real_genotools-1.2.2/the_real_genotools.egg-info/
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)     4646 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/PKG-INFO
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      738 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)        1 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      122 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/entry_points.txt
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)      353 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/requires.txt
+-rw-r--r--   0 vitaled2 (524967535) NIH\Domain Users (1360859114)       10 2024-04-12 23:10:48.000000 the_real_genotools-1.2.2/the_real_genotools.egg-info/top_level.txt
```

### Comparing `the_real_genotools-1.2.1/LICENSE` & `the_real_genotools-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/PKG-INFO` & `the_real_genotools-1.2.2/the_real_genotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: the_real_genotools
-Version: 1.2.1
+Name: the-real-genotools
+Version: 1.2.2
 Summary: A collection of tools for genotype quality control and analysis
 Home-page: https://github.com/dvitale199/GenoTools
 Author: Dan Vitale
 Author-email: d.vitale199@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # GenoTools
 [![DOI](https://zenodo.org/badge/337965715.svg)](https://zenodo.org/doi/10.5281/zenodo.10443257)
 
+## Documentation
+You can find the full documentation with the following links:
+- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
+- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
+- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+- [JSON output guide](https://github.com/dvitale199/GenoTools/blob/main/docs/json_output_overview.md)
+
 ## Getting Started
 
 GenoTools is a suite of automated genotype data processing steps written in Python. The core pipeline was built for Quality Control and Ancestry estimation of data in the Global Parkinson's Genetics Program (GP2)
 
 To download the most current version from pip:
 ```
 pip install the_real_genotools
@@ -82,18 +89,15 @@
 ```
 Note: add the ```--singularity``` flag to run containerized ancestry predictions on HPC
 
 This will find common snps between your genotype data and the reference panel, run PCA, UMAP-transform PCs, and train a new XGBoost classifier specific to your data/ref panel.
 
 genotools accept `--pfile`, `--bfile`, or `--vcf`. Any bfile or vcf will be converted to a pfile before running any steps. 
 
-## Documentation
-- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
-- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
-- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+Please consult the docs links listed at the top of the README for the full argument guide, function guide, Default pipeline overview, and guide for navigating the output JSON.
 
 ## Acknowledgements
 GenoTools was developed as the core genotype and wgs processing pipeline for the Global Parkinson's Genetics Program (GP2) at the Center for Alzheimer's and Related Dementias (CARD) at the National Institutes of Health.
 
 This tool relies on PLINK, a whole genome association analysis toolset, for various genetic data processing functionalities. We gratefully acknowledge the developers of PLINK for their foundational contributions to the field of genetics. More about PLINK can be found at [their website](https://www.cog-genomics.org/plink/2.0/).
```

### Comparing `the_real_genotools-1.2.1/README.md` & `the_real_genotools-1.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # GenoTools
 [![DOI](https://zenodo.org/badge/337965715.svg)](https://zenodo.org/doi/10.5281/zenodo.10443257)
 
+## Documentation
+You can find the full documentation with the following links:
+- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
+- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
+- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+- [JSON output guide](https://github.com/dvitale199/GenoTools/blob/main/docs/json_output_overview.md)
+
 ## Getting Started
 
 GenoTools is a suite of automated genotype data processing steps written in Python. The core pipeline was built for Quality Control and Ancestry estimation of data in the Global Parkinson's Genetics Program (GP2)
 
 To download the most current version from pip:
 ```
 pip install the_real_genotools
@@ -67,18 +74,15 @@
 ```
 Note: add the ```--singularity``` flag to run containerized ancestry predictions on HPC
 
 This will find common snps between your genotype data and the reference panel, run PCA, UMAP-transform PCs, and train a new XGBoost classifier specific to your data/ref panel.
 
 genotools accept `--pfile`, `--bfile`, or `--vcf`. Any bfile or vcf will be converted to a pfile before running any steps. 
 
-## Documentation
-- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
-- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
-- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+Please consult the docs links listed at the top of the README for the full argument guide, function guide, Default pipeline overview, and guide for navigating the output JSON.
 
 ## Acknowledgements
 GenoTools was developed as the core genotype and wgs processing pipeline for the Global Parkinson's Genetics Program (GP2) at the Center for Alzheimer's and Related Dementias (CARD) at the National Institutes of Health.
 
 This tool relies on PLINK, a whole genome association analysis toolset, for various genetic data processing functionalities. We gratefully acknowledge the developers of PLINK for their foundational contributions to the field of genetics. More about PLINK can be found at [their website](https://www.cog-genomics.org/plink/2.0/).
```

### Comparing `the_real_genotools-1.2.1/genotools/__init__.py` & `the_real_genotools-1.2.2/genotools/__init__.py`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/__main__.py` & `the_real_genotools-1.2.2/genotools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import tempfile
 import pandas as pd
 import json
 from genotools.pipeline import gt_argparse
 
 
 def handle_main():
-    
+
     args = gt_argparse()
 
     args_dict = vars(args)
-    
+
     from numba.core.errors import NumbaDeprecationWarning
     import warnings
     warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
 
     from umap import UMAP
     from genotools.utils import upfront_check, bfiles_to_pfiles, vcf_to_pfiles, gt_header
     from genotools.qc import SampleQC, VariantQC
@@ -41,16 +41,17 @@
     samp_qc = SampleQC()
     var_qc = VariantQC()
     ancestry = Ancestry()
     assoc = Assoc()
 
     # ordered steps with their methods to be called
     ordered_steps =  {'ancestry':ancestry.run_ancestry,'callrate':samp_qc.run_callrate_prune,'sex':samp_qc.run_sex_prune,
-                    'related':samp_qc.run_related_prune,'het':samp_qc.run_het_prune,'case_control':var_qc.run_case_control_prune,
-                    'haplotype':var_qc.run_haplotype_prune,'hwe':var_qc.run_hwe_prune,'geno':var_qc.run_geno_prune,
+                    'related':samp_qc.run_related_prune,'het':samp_qc.run_het_prune,'kinship_check':samp_qc.run_confirming_kinship,
+                    'case_control':var_qc.run_case_control_prune, 'haplotype':var_qc.run_haplotype_prune,
+                    'hwe':var_qc.run_hwe_prune,'geno':var_qc.run_geno_prune,
                     'ld':var_qc.run_ld_prune,'assoc':assoc.run_association}
 
     # some up-front editing of pipeline arguments (booleans and lists)
     for step in args_dict:
         if (args_dict[step] == 'True') or (args_dict[step] == 'False'):
             args_dict[step] = bool(args_dict[step] == 'True')
 
@@ -63,52 +64,52 @@
 
     if args_dict['het'] is not None:
         if len(args_dict['het']) == 0:
             args_dict['het'] = [-0.25, 0.25]
 
         else:
             args_dict['het'] = [float(i) for i in args_dict['sex']]
-        
+
     if args_dict['ld'] is not None:
         if len(args_dict['ld']) == 0:
             args_dict['ld'] = [50, 5, 0.5]
 
         else:
             args_dict['ld'] = [int(args_dict['ld'][0]), int(args_dict['ld'][1]), float(args_dict['ld'][2])]
 
     # if all sample or all variant called, replace necessary items with defaults
     if args_dict['all_sample']:
         args_dict['callrate'] = 0.05
         args_dict['sex'] = [0.25, 0.75]
         args_dict['related'] = True
         args_dict['het'] = [-0.25, 0.25]
-    
+
     if args_dict['all_variant']:
         args_dict['geno'] = 0.05
         args_dict['case_control'] = 1e-4
         args_dict['haplotype'] = 1e-4
         args_dict['hwe'] = 1e-4
         args_dict['filter_controls'] = True
         args_dict['ld'] = None
-    
+
     # run data breakdows
     if (args_dict['bfile'] is None) and (args_dict['pfile'] is None) and (args_dict['vcf'] is None):
         raise KeyError('No bfiles, pfiles, or vcf genotypes were provided!')
-    
+
     elif args_dict['bfile'] and (args_dict['pfile'] is None):
         bfiles_to_pfiles(bfile_path=args_dict['bfile'])
         args_dict['geno_path'] = args_dict['bfile']
-    
+
     elif args_dict['vcf'] and (args_dict['pfile'] is None):
         vcf_to_pfiles(vcf_path=args_dict['vcf'])
         args_dict['geno_path'] = args_dict['vcf'].split('.vcf')[0]
-    
+
     else:
         args_dict['geno_path'] = args_dict['pfile']
-    
+
     # run model-side error catching
     if args_dict['model'] and args_dict['container']:
         raise KeyError('Cannot pass a pre-trained model and run predictions using the NeuroBooster array model in a container! Please choose one of the two.')
     elif args_dict['model'] and args_dict['cloud']:
         raise KeyError('Cannot pass a pre-trained model and run predictions in the cloud! Please choose one of the two.')
     elif args_dict['container'] and args_dict['cloud']:
         raise KeyError('Cannot run predictions using the NeuroBooster array model in a container and run predictions in the cloud! Please choose one of the two.')
@@ -119,42 +120,42 @@
     if os.path.exists(f"{args_dict['out']}_all_logs.log"):
         os.remove(f"{args_dict['out']}_all_logs.log")
     if os.path.exists(f"{args_dict['out']}_cleaned_logs.log"):
         os.remove(f"{args_dict['out']}_cleaned_logs.log")
 
     # create empty log files in output directory
     header = gt_header()
-    with open(f"{args_dict['out']}_all_logs.log", "w") as fp: 
+    with open(f"{args_dict['out']}_all_logs.log", "w") as fp:
         fp.write(header)
         fp.write("\n")
-    with open(f"{args_dict['out']}_cleaned_logs.log", "w") as fp: 
+    with open(f"{args_dict['out']}_cleaned_logs.log", "w") as fp:
         pass
 
     # get correct order of steps to run
     run_steps_list = []
     for key in args_dict:
         if (args_dict[key] != None) and args_dict[key]:
             if key in ordered_steps.keys():
                 run_steps_list.append(key)
             if ((key == 'pca') or (key == 'gwas')) and ('assoc' not in run_steps_list):
                 run_steps_list.append('assoc')
-    
+
     # check run steps and output step
     if len(run_steps_list) == 0:
         raise KeyError('No main Ancestry, QC, or GWAS flags were used.')
     else:
         print(f'Output steps: {run_steps_list[-1]}')
 
     # create tmp dir
     out_dir = os.path.dirname(args_dict['out'])
     tmp_dir = tempfile.TemporaryDirectory(suffix='_tmp', prefix='.', dir=out_dir)
 
     # run pipeline
     out_dict = execute_pipeline(run_steps_list, ordered_steps, args_dict['geno_path'], args_dict['out'], samp_qc=samp_qc, var_qc=var_qc, ancestry=ancestry, assoc=assoc, args=args_dict, tmp_dir=tmp_dir)
-    
+
     # build output
     clean_out_dict = dict()
     metrics_df = pd.DataFrame()
     pruned_df = pd.DataFrame()
     gwas_df = pd.DataFrame()
     related_df = pd.DataFrame()
 
@@ -181,15 +182,15 @@
         clean_out_dict['test_accuracy'] = out_dict['ancestry']['metrics']['test_accuracy']
 
         clean_out_dict['ref_pcs'] = out_dict['ancestry']['data']['ref_pcs'].to_dict()
         clean_out_dict['projected_pcs'] = out_dict['ancestry']['data']['projected_pcs'].to_dict()
         clean_out_dict['total_umap'] = out_dict['ancestry']['data']['total_umap'].to_dict()
         clean_out_dict['ref_umap'] = out_dict['ancestry']['data']['ref_umap'].to_dict()
         clean_out_dict['new_samples_umap'] = out_dict['ancestry']['data']['new_samples_umap'].to_dict()
-    
+
         for ancestry in ['AFR', 'SAS', 'EAS', 'EUR', 'AMR', 'AJ', 'CAS', 'MDE', 'FIN', 'AAC', 'CAH']:
             if ancestry in out_dict.keys():
                 metrics_df, pruned_df, gwas_df, related_df = build_metrics_pruned_df(metrics_df=metrics_df, pruned_df=pruned_df, gwas_df=gwas_df, related_df=related_df, dictionary=out_dict[ancestry], out=args_dict['out'], ancestry=ancestry)
 
     else:
         metrics_df, pruned_df, gwas_df, related_df = build_metrics_pruned_df(metrics_df=metrics_df, pruned_df=pruned_df, gwas_df=gwas_df, related_df=related_df, dictionary=out_dict, out=args_dict['out'])
```

### Comparing `the_real_genotools-1.2.1/genotools/ancestry.py` & `the_real_genotools-1.2.2/genotools/ancestry.py`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/container/GP2_merge_APRIL_2023_ready_genotools_callrate_sex_ancestry_umap_linearsvc_ancestry_model.pkl` & `the_real_genotools-1.2.2/genotools/container/GP2_merge_APRIL_2023_ready_genotools_callrate_sex_ancestry_umap_linearsvc_ancestry_model.pkl`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/container/run.py` & `the_real_genotools-1.2.2/genotools/container/run.py`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/dependencies.py` & `the_real_genotools-1.2.2/genotools/dependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,21 +76,21 @@
             zip_file = url.split('/')[-1]
             zip_file_path = os.path.join(__executable_folder, zip_file)
 
             r = requests.get(url)
             r.raise_for_status()
             with open(zip_file_path, 'wb') as fp:
                 fp.write(r.content)
-            
+
             with zipfile.ZipFile(zip_file_path, 'r') as fp:
                 fp.extractall(__executable_folder)
 
             permissions = 0o100
             os.chmod(os.path.join(__executable_folder, 'plink2'), permissions)
-        
+
     elif '.tar.gz' in url:
         file = tarfile.open(fileobj=r.raw, mode="r|gz")
         file.extractall(__executable_folder)
 
     binary_path = os.path.join(__executable_folder, exec_path)
 
     os.chmod(binary_path, stat.S_IEXEC)
@@ -100,16 +100,20 @@
     platform_system = platform.system()
     platform_processor = platform.processor()
 
     if name not in __DEPENDENCIES:
         raise EnvironmentError("Unknown package: {}".format(name))
 
     if platform_system not in __DEPENDENCIES[name]:
-        raise EnvironmentError(
-            "Unknown supported OK: {}".format(platform_system))
+        if name == 'KING':
+            logging.warning("Can not install {} on non-Linux OS".format(name))
+            return
+        else:
+            raise EnvironmentError(
+                "Unknown supported OK: {}".format(platform_system))
 
     if (platform_system == "Darwin") and (platform_processor == "arm") and (name == "Plink2"):
         platform_system = "Darwin_arm64"
 
     entry = __DEPENDENCIES[name][platform_system]
 
     binary_name = entry["binary"]
@@ -142,14 +146,17 @@
 
 def check_plink():
     return __check_package('Plink')
 
 def check_plink2():
     return __check_package('Plink2')
 
+def check_king():
+    return __check_package('KING')
+
 __DEPENDENCIES = {
     'Plink': {
         'checker': check_plink,
         'Darwin': {
             'binary': 'plink',
             'version_args': ['--version'],
             'url': 'https://s3.amazonaws.com/plink1-assets/dev/plink_mac.zip'
@@ -179,9 +186,28 @@
             'url': 'https://s3.amazonaws.com/plink2-assets/alpha5/plink2_mac_avx2_20240105.zip'
         },
         'Linux': {
             'binary': 'plink2',
             'version_args': ['--version'],
             'url': 'https://s3.amazonaws.com/plink2-assets/alpha5/plink2_linux_x86_64_20240105.zip'
         },
+    },
+
+    'KING': {
+        'checker': check_king,
+        # 'Darwin': {
+        #     'binary': 'king',
+        #     'version_args': ['--version'],
+        #     'url': 'https://www.kingrelatedness.com/executables/Linux-king232.tar.gz'
+        # },
+        'Linux': {
+            'binary': 'king',
+            'version_args': ['--version'],
+            'url': 'https://www.kingrelatedness.com/executables/Linux-king232.tar.gz'
+        },
+        'Windows': {
+            'binary': 'king',
+            'version_args': ['--version'],
+            'url': 'https://www.kingrelatedness.com/executables/Windows-king232.zip'
+        }
     }
 }
```

### Comparing `the_real_genotools-1.2.1/genotools/download_refs.py` & `the_real_genotools-1.2.2/genotools/download_refs.py`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/gwas.py` & `the_real_genotools-1.2.2/genotools/gwas.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.out_path = out_path
         self.pca = pca
         self.build = build
         self.gwas = gwas
         self.pheno_name = pheno_name
         self.covar_path = covar_path
         self.covar_names = covar_names
-    
+
 
     def write_exclusion_file(self):
         if self.build == 'hg19':
             exclusion_regions = """
         5 44000000 51500000 r1
         6 25000000 33500000 r2
         8 8000000 12000000 r3
@@ -62,32 +62,32 @@
         8   110987771   113987771   r12
         11  87789108    90766832    r13
         12  109062195   111562196   r14
         20  33412194    35912078    r15
         """
         else:
             raise ValueError("Invalid build specified.")
-        
+
         exclusion_file = f'{self.out_path}_{self.build}.exclusion'
         with open(exclusion_file, 'w') as f:
             f.write(exclusion_regions)
-        
+
         return exclusion_file
-    
-    
+
+
     def run_pca_pruning(self, maf=0.01, geno=0.01, hwe=5e-6, indep_pairwise=[1000, 10, 0.02]):
-        
+
         step = 'plink_pruning'
 
         exclusion_file = self.write_exclusion_file()
 
         # Filter data
         filter_cmd = f"{plink2_exec} --pfile {self.geno_path} --maf {maf} --geno {geno} --hwe {hwe} --autosome --exclude {exclusion_file} --make-pgen psam-cols=fid,parents,sex,pheno1,phenos --out {self.out_path}_tmp"
         shell_do(filter_cmd)
-        
+
         # Prune SNPs
         prune_cmd = f"{plink2_exec} --pfile {self.out_path}_tmp --indep-pairwise {indep_pairwise[0]} {indep_pairwise[1]} {indep_pairwise[2]} --autosome --out {self.out_path}_pruned"
         shell_do(prune_cmd)
 
         # Check if prune.in file exists
         if os.path.isfile(f'{self.out_path}_pruned.prune.in'):
             # Extract pruned SNPs
@@ -125,15 +125,15 @@
 
         return out_dict
 
 
     def run_plink_pca(self):
 
         step = 'plink_pca'
- 
+
         # Calculate/generate PCs
         pca_pruned = self.run_pca_pruning()
         pca_cmd = f"{plink2_exec} --pfile {pca_pruned['output']} --pca {self.pca} --out {self.out_path}"
         shell_do(pca_cmd)
 
         listOfFiles = [f'{self.out_path}.log']
         concat_logs(step, self.out_path, listOfFiles)
@@ -224,79 +224,79 @@
             '+a1freqcc,'
             '+a1count,'
             '+totallele,'
             '+a1countcc,'
             '+totallelecc,'
             '+err'
             )
-        
+
         if covars:
             # covar names are column names of covariate file minus #FID and IID unless specified
             if self.covar_path and not self.covar_names:
                 covar_cols = pd.read_csv(f'{self.covar_path}', sep='\s+', header=0, nrows=0).columns.tolist()
                 if '#FID' in covar_cols:
                     # account for 1st two cols being #FID and IID
                     covar_names = ','.join(covar_cols[2:])
                 else:
                     covar_names = ','.join(covar_cols[1:])
             else:
                 # if no covar path then default is PCA
                 covar_names = self.covar_names
-            
+
             gwas_cmd = (
                 f"{plink2_exec} --pfile {self.geno_path} "
                 f"--glm {glm_options} "
                 f"--pheno-name {self.pheno_name} "
                 f"--pheno {self.geno_path}.pheno "
                 f"--covar {self.covar_path} "
                 f"--covar-variance-standardize "
                 f"--covar-name {covar_names} "
                 f"--out {self.out_path}"
                 )
-        
+
         else:
             gwas_cmd = (
                 f"{plink2_exec} --pfile {self.geno_path} "
                 f"--glm {glm_options} allow-no-covars "
                 f"--pheno-name {self.pheno_name} "
                 f"--pheno {self.geno_path}.pheno "
                 f"--out {self.out_path}"
                 )
-            
+
         shell_do(gwas_cmd)
 
         if os.path.isfile(f'{self.out_path}.PHENO1.glm.logistic.hybrid'):
             print('logistic')
 
             # calculate inflation
             gwas_df = pd.read_csv(f'{self.out_path}.PHENO1.glm.logistic.hybrid', sep='\s+', dtype={'#CHROM': str})
             psam = pd.read_csv(f'{self.geno_path}.psam', sep='\s+', dtype={'PHENO1':str})
-            ncontrols = psam.PHENO1.value_counts()[0]
-            ncases = psam.PHENO1.value_counts()[1]
+            ncontrols = psam.PHENO1.value_counts()['1']
+            ncases = psam.PHENO1.value_counts()['2']
 
             # add pruning step here (pre lambdas)
             gwas_df_add = gwas_df.loc[gwas_df.TEST=='ADD']
 
             # calculate inflation
             lambda_dict = Assoc.calculate_inflation(gwas_df_add.P, normalize=False)
             lambda1000_dict = Assoc.calculate_inflation(gwas_df_add.P, normalize=True, ncases=ncases, ncontrols=ncontrols)
 
             metrics_dict = {
                 'lambda': lambda_dict['metrics']['inflation'],
                 'lambda1000': lambda1000_dict['metrics']['inflation'],
                 'cases': ncases,
                 'controls': ncontrols
                 }
-            
+
             process_complete = True
 
             outfiles_dict = {
                 'gwas_output': f'{self.out_path}.PHENO1.glm.logistic.hybrid'
             }
-        
+
         elif os.path.isfile(f'{self.out_path}.PHENO1.glm.linear'):
             print('linear')
 
             # calculate inflation
             gwas_df = pd.read_csv(f'{self.out_path}.PHENO1.glm.linear', sep='\s+', dtype={'#CHROM': str})
 
             # add pruning step here (pre lambdas)
@@ -325,28 +325,28 @@
 
             metrics_dict = {
                 'lambda': None,
                 'lambda1000': None,
                 'cases': None,
                 'controls': None
                 }
-            
+
             outfiles_dict = {
                 'gwas_output': None
             }
 
         out_dict = {
             'pass': process_complete,
             'step': step,
             'metrics': metrics_dict,
             'output': outfiles_dict
         }
 
         return out_dict
-    
+
 
     def run_prs(self):
         print('COMING SOON')
 
 
     def run_association(self):
         # Check that paths are set
@@ -363,20 +363,20 @@
         if self.pca:
             assoc['pca'] = self.run_plink_pca()
 
         # run gwas
         if self.gwas:
             # if pca called and covars passed, warn and default to passed covars
             if os.path.isfile(f'{self.out_path}.eigenvec') and (self.covar_path is not None):
-                warnings.warn('PCA ran and Covar passed! Defaulting to passed covars!')
+                warnings.warn('PCA ran and Covars passed! Defaulting to passed covars! Recommend merging the PCAs with the inputted Covars and rerunning.')
                 assoc['gwas'] = self.run_gwas(covars=True)
-            
+
             # if pca called and no covars pass, defult to pca
             elif os.path.isfile(f'{self.out_path}.eigenvec') and (self.covar_path is None):
                 self.covar_path = f'{self.out_path}.eigenvec'
                 assoc['gwas'] = self.run_gwas(covars=True)
-            
+
             # otherwise run GWAS with no covars
             else:
                 assoc['gwas'] = self.run_gwas(covars=False)
-        
+
         return assoc
```

### Comparing `the_real_genotools-1.2.1/genotools/imputation.py` & `the_real_genotools-1.2.2/genotools/imputation.py`

 * *Files identical despite different names*

### Comparing `the_real_genotools-1.2.1/genotools/pipeline.py` & `the_real_genotools-1.2.2/genotools/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 import os
 import shutil
 import argparse
 import warnings
 import pathlib
+import platform
 import pandas as pd
 
 
 def gt_argparse():
     # definte arg parse
     parser = argparse.ArgumentParser(description='Arguments for Genotyping QC (data in Plink .bim/.bam/.fam format)')
 
@@ -52,14 +53,15 @@
     parser.add_argument('--sex', nargs='*', help='Sex prune with cutoffs')
     parser.add_argument('--related', type=str, nargs='?', default='False', const='True', help='Relatedness prune')
     parser.add_argument('--related_cutoff', type=float, nargs='?', default=0.0884, const=0.0884, help='Relatedness cutoff')
     parser.add_argument('--duplicated_cutoff', type=float, nargs='?', default=0.354, const=0.354, help='Relatedness cutoff')
     parser.add_argument('--prune_related', type=str, nargs='?', default='False', const='True', help='Relatedness prune')
     parser.add_argument('--prune_duplicated', type=str, nargs='?', default='True', const='True', help='Relatedness prune')
     parser.add_argument('--het', nargs='*', help='Het prune with cutoffs')
+    parser.add_argument('--kinship_check', type=str, nargs='?', default='False', const='True', help='Confirming familial labels')
     parser.add_argument('--all_sample', type=str, nargs='?', default='False', const='True', help='Run all sample-level QC')
 
     # variant-level qc arguments
     parser.add_argument('--geno', type=float, nargs='?', default=None, const=0.05, help='Minimum Missingness threshold for QC')
     parser.add_argument('--case_control', type=float, nargs='?', default=None, const=1e-4, help='Case control prune')
     parser.add_argument('--haplotype', type=float, nargs='?', default=None, const=1e-4, help='Haplotype prune')
     parser.add_argument('--hwe', type=float, nargs='?', default=None, const=1e-4, help='HWE pruning')
@@ -73,21 +75,21 @@
     parser.add_argument('--gwas', type=str, nargs='?', default='False', const='True', help='Run GWAS')
     parser.add_argument('--covars', type=str, nargs='?', default=None, const=None, help='Path to external covars')
     parser.add_argument('--covar_names', type=str, nargs='?', default=None, const=None, help='Covar names to use from external file')
 
 
     # parse args and turn into dict
     args = parser.parse_args()
-    
+
     return args
 
 
 def execute_pipeline(steps, steps_dict, geno_path, out_path, samp_qc, var_qc, ancestry, assoc, args, tmp_dir):
     # to know which class to call
-    samp_steps = ['callrate','sex','related','het']
+    samp_steps = ['callrate','sex','related','het','kinship_check']
     var_steps = ['case_control','haplotype','hwe','geno','ld']
 
     # if full output requested, go to out path
     if args['full_output']:
         step_paths = [out_path]
 
     # otherwise tmpdir
@@ -135,67 +137,75 @@
                     out_dict[label] = execute_pipeline(steps_ancestry, steps_dict, geno, f'{out_path}_{label}', samp_qc, var_qc, ancestry, assoc, args, tmp_dir)
 
         else:
             # if warn is True and step input doesn't exist print error and reset step input
             if args['warn'] and (not os.path.isfile(f'{step_input}.pgen')) and (len(step_paths) > 1):
                 warnings.warn(f'{step_input}.pgen was not created. Continuing to next step...', stacklevel=2)
                 step_input = f'{step_paths[-2]}' if step != steps[1] else geno_path
-                
+
                 # very rare edge case when multiple steps fail
                 if not os.path.isfile(f'{step_input}.pgen'):
                     step_input = f'{step_paths[-3]}'
 
                 step_output = f'{step_paths[-2]}_{step}' if step != steps[-1] else out_path
                 step_paths.append(step_output)
-            
+
             # otherwise keep track of paths
             else:
                 step_paths.append(step_output)
 
         # samp qc setup and call
         if step in samp_steps:
             samp_qc.geno_path = step_input
             samp_qc.out_path = step_output
 
             # related has more than one parameter
             if step == 'related':
                 out_dict[step] = steps_dict[step](related_cutoff=args['related_cutoff'], duplicated_cutoff=args['duplicated_cutoff'],
                                  prune_related=args['prune_related'], prune_duplicated=args['prune_duplicated'])
-            
+
+            elif step == 'kinship_check':
+                # check that OS is not macOS
+                if platform.system() != 'Linux':
+                    print('Relatedness Assessment can only run on a linux or windows OS!')
+                    out_dict.pop(step, None)
+                elif platform.system() == 'Linux':
+                    out_dict[step] = steps_dict[step]()
+
             else:
                 out_dict[step] = steps_dict[step](args[step])
-        
+
         # var qc setup and call
         if step in var_steps:
             var_qc.geno_path = step_input
             var_qc.out_path = step_output
 
             # hwe and ld have extra parameters
             if step == 'hwe':
                 out_dict[step] = steps_dict[step](hwe_threshold=args['hwe'], filter_controls=args['filter_controls'])
 
             elif step == 'ld':
                 out_dict[step] = steps_dict[step](window_size=args['ld'][0], step_size=args['ld'][1], r2_threshold=args['ld'][2])
-            
+
             else:
                 out_dict[step] = steps_dict[step](args[step])
-            
+
         # assoc setup and call
         if step == 'assoc':
             assoc.geno_path = step_input
             assoc.out_path = step_output
             assoc.pca = args['pca']
             assoc.build = args['build']
             assoc.gwas = args['gwas']
             assoc.covar_path = args['covars']
             assoc.covar_names = args['covar_names']
             out_dict[step] = steps_dict[step]()
-        
-        # remove old files when appropriate 
-        if (not args['full_output']) and (step != 'assoc') and (step != 'ancestry'):
+
+        # remove old files when appropriate
+        if (not args['full_output']) and (step != 'assoc') and (step != 'ancestry') and (step != 'kinship_check'):
             # when warn is True and step fails, don't remove old file
             if args['warn'] and ('pass' in out_dict[step].keys()) and (not out_dict[step]['pass']):
                 remove = False
             else:
                 remove = True
                 remove_step_index = step_paths.index(step_output) - 1
```

### Comparing `the_real_genotools-1.2.1/genotools/qc.py` & `the_real_genotools-1.2.2/genotools/qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # ==============================================================================
 
 
 import pandas as pd
 import numpy as np
 import os
 import shutil
+import platform
 from genotools.utils import shell_do, count_file_lines, concat_logs, bfiles_to_pfiles
-from genotools.dependencies import check_plink, check_plink2
+from genotools.dependencies import check_plink, check_plink2, check_king
 
 plink_exec = check_plink()
 plink2_exec = check_plink2()
-
+king_exec = check_king()
 
 class SampleQC:
 
     def __init__(self, geno_path=None, out_path=None):
         self.geno_path = geno_path
         self.out_path = out_path
 
@@ -558,14 +559,170 @@
             'metrics': metrics_dict,
             'output': outfiles_dict
         }
 
         return out_dict
 
 
+    def run_confirming_kinship(self):
+
+        """
+        Find samples with discordant FIDs using PLINK and KING.
+
+        Parameters:
+        - None
+
+        Returns:
+        - dict: A structured dictionary containing:
+            * 'pass': Boolean indicating the successful completion of the process.
+            * 'step': The label for this procedure ('confirming_kinship').
+            * 'metrics': Metrics associated with the counts.
+            * 'output': Dictionary containing paths to the generated output files.
+        """
+        geno_path = self.geno_path
+        out_path = self.out_path
+
+        step = 'confirming_kinship'
+
+        duplicated_cutoff = 0.354 # or greater
+        first_deg_cutoff = 0.177 # to 0.354
+        second_deg_cutoff = 0.0884 # to 0.177
+        third_deg_cutoff = 0.0442 # to 0.0884
+
+        # create output files
+        temp = f'{out_path}_temp'
+        same_fid_unrelated = f'{out_path}_same_fid.unrelated'
+        diff_fid_related = f'{out_path}_diff_fid.related'
+        num_same_fid_unrelated = 0
+        num_diff_fid_related = 0
+
+        # check OS is NOT macOS
+        # Will only run this method if os is linux or windows
+        if platform.system() != 'Linux':
+        # if (platform.system() != 'Linux') or (platform.system() != 'Windows'):
+            print('Relatedness Assessment can only run on a linux OS!')
+            process_complete = False
+
+            outfiles_dict = {
+                'same_fid_unrelated': None,
+                'diff_fid_related': None
+            }
+
+            metrics_dict = {
+                'same_fid_unrelated_count': 0,
+                'diff_fid_related_count': 0
+            }
+
+            out_dict = {
+            'pass': process_complete,
+            'step': step,
+            'metrics': metrics_dict,
+            'output': outfiles_dict
+            }
+
+            return out_dict
+
+
+        # if data is bfiles, proceed
+        if not os.path.isfile(f'{geno_path}.bed'):
+            # # if data is vcf, convert to pfiles
+            # if os.path.isfile(f'{geno_path}.vcf'):
+            #     vfiles_to_pfiles(vcf_path=geno_path)
+            # if data is in pfiles, convert to bfiles for KING
+            if os.path.isfile(f'{geno_path}.pgen'):
+                bfiles_to_pfiles(pfile_path=geno_path)
+
+        print('If data does NOT contain pedigree (PAT/MAT) info, the Error column will be 1.0 for any found relationships')
+
+        # run KING
+        king_cmd = f'{king_exec} -b {geno_path}.bed --related --build --degree 3 --prefix {temp}'
+        shell_do(king_cmd)
+
+        if (os.path.isfile(f'{temp}.kin0')) or (os.path.isfile(f'{temp}.kin')):
+            # pairs with different FID but found to be related
+            if os.path.isfile(f'{temp}.kin0'):
+                os.rename(f'{temp}.kin0', diff_fid_related)
+                num_diff_fid_related = sum(1 for _ in open(diff_fid_related)) - 1
+
+            # pairs with same FID but found to be unrelated
+            if os.path.isfile(f'{temp}.kin'):
+                kin = pd.read_csv(f'{temp}.kin', sep='\s+')
+                unrelated = kin[kin['Kinship']<=third_deg_cutoff]
+                unrelated.to_csv(same_fid_unrelated, sep='\t', header=True, index=False)
+                num_same_fid_unrelated = sum(1 for _ in open(same_fid_unrelated)) - 1
+
+            # create log file
+            with open(f'{out_path}.log', 'w') as log:
+                log.write('KING relatedness options in effect:\n')
+                log.write('  --related\n')
+                log.write('  --build\n')
+                log.write('  --degree 3\n')
+                log.write(f'  --prefix {temp}\n')
+                log.write(f'  -b {geno_path}.bed\n')
+                log.write('Note: if no pedigree info given, Error column will be 1.0 for any found relationship\n')
+                log.write(f'{num_same_fid_unrelated + num_diff_fid_related} total noncongruent relationships found\n')
+                # log.write('Potential pedigree is as follows:\n')
+                # with open(f'{temp}build.log', 'r') as build:
+                #     for line in build:
+                #         if line != '\n':
+                #         log.write(line)
+
+            shutil.copyfile(f'{out_path}.log', f'{out_path}_test.log')
+
+            if os.path.isfile(f'{out_path}.log'):
+                listOfFiles = [f'{out_path}.log']
+                concat_logs(step, out_path, listOfFiles)
+
+            # remove intermediate files
+            os.remove(f'{temp}.kin')
+            os.remove(f'{temp}.seg')
+            os.remove(f'{temp}X.kin')
+            os.remove(f'{temp}X.kin0')
+            os.remove(f'{temp}.segments.gz')
+            os.remove(f'{temp}allsegs.txt')
+            os.remove(f'{temp}build.log')
+            os.remove(f'{temp}updateids.txt')
+            os.remove(f'{temp}updateparents.txt')
+
+            process_complete = True
+
+            outfiles_dict = {
+                'same_fid_unrelated': same_fid_unrelated,
+                'diff_fid_related': diff_fid_related
+            }
+
+            metrics_dict = {
+                'same_fid_unrelated_count': num_same_fid_unrelated,
+                'diff_fid_related_count': num_diff_fid_related
+            }
+
+        else:
+            print('Relatedness Assessment has failed!')
+            process_complete = False
+
+            outfiles_dict = {
+                'same_fid_unrelated': None,
+                'diff_fid_related': None
+            }
+
+            metrics_dict = {
+                'same_fid_unrelated_count': 0,
+                'diff_fid_related_count': 0
+            }
+
+        out_dict = {
+            'pass': process_complete,
+            'step': step,
+            'metrics': metrics_dict,
+            'output': outfiles_dict
+        }
+
+        return out_dict
+
+
 class VariantQC:
 
     def __init__(self, geno_path=None, out_path=None):
         self.geno_path = geno_path
         self.out_path = out_path
 
     def run_geno_prune(self, geno_threshold=0.05):
@@ -796,23 +953,23 @@
 
         # convert to bfiles
         bfiles_to_pfiles(pfile_path=geno_path)
 
         # get initial snp count
         initial_snp_count = count_file_lines(f'{geno_path}.bim')
 
-        
+
         # if sample size is over 10k, correct and make P more stringent
         sample_size = count_file_lines(f'{geno_path}.fam')
         if sample_size > 10000:
             p_threshold = 0.05/sample_size
 
 
         # missingness by haplotype (--test-mishap), using P > 1E-4
-        plink_cmd1 = f"{plink_exec} --bfile {geno_path} --test-mishap --out {hap_tmp}"
+        plink_cmd1 = f"{plink_exec} --bfile {geno_path} --maf 0.05 --test-mishap --out {hap_tmp}"
         shell_do(plink_cmd1)
 
         listOfFiles = [f'{hap_tmp}.log']
         concat_logs(step, out_path, listOfFiles)
 
         if os.path.isfile(f'{hap_tmp}.missing.hap'):
 
@@ -827,15 +984,15 @@
 
             listOfFiles = [f'{out_path}.log']
             concat_logs(step, out_path, listOfFiles)
 
             # hap pruned count
             hap_snp_count = count_file_lines(f'{out_path}.pvar') - 1
             hap_rm_count = initial_snp_count - hap_snp_count
-        
+
         else:
             print(f'Haplotype pruning failed!')
             print(f'Check {hap_tmp}.log for more information')
             process_complete = False
             hap_snp_count = count_file_lines(f'{geno_path}.bim')
             hap_rm_count = 0
 
@@ -845,15 +1002,15 @@
 
         metrics_dict = {
             'haplotype_removed_count': hap_rm_count
         }
 
         process_complete = True
 
-        for file in [f'{hap_tmp}.exclude',f'{hap_tmp}.hh',f'{hap_tmp}.missing.hap']:
+        for file in [f'{hap_tmp}.hh']:
             if os.path.isfile(file):
                 os.remove(file)
 
         os.remove(f'{geno_path}.bed')
         os.remove(f'{geno_path}.bim')
         os.remove(f'{geno_path}.fam')
```

### Comparing `the_real_genotools-1.2.1/genotools/utils.py` & `the_real_genotools-1.2.2/genotools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 
 
 import subprocess
 import sys
 import os
 import shutil
 import pandas as pd
-import warnings 
+import warnings
 import numpy as np
 from scipy.stats import norm
 from genotools.dependencies import check_plink, check_plink2
 
 plink_exec = check_plink()
 plink2_exec = check_plink2()
 
 def gt_header():
-    
+
     header = """
      ██████╗ ███████╗███╗  ██╗ █████╗ ████████╗ █████╗  █████╗ ██╗      ██████╗
     ██╔════╝ ██╔════╝████╗ ██║██╔══██╗╚══██╔══╝██╔══██╗██╔══██╗██║     ██╔════╝
-    ██║  ██╗ █████╗  ██╔██╗██║██║  ██║   ██║   ██║  ██║██║  ██║██║     ╚█████╗ 
+    ██║  ██╗ █████╗  ██╔██╗██║██║  ██║   ██║   ██║  ██║██║  ██║██║     ╚█████╗
     ██║  ╚██╗██╔══╝  ██║╚████║██║  ██║   ██║   ██║  ██║██║  ██║██║      ╚═══██╗
     ╚██████╔╝███████╗██║ ╚███║╚█████╔╝   ██║   ╚█████╔╝╚█████╔╝███████╗██████╔╝
-    ╚═════╝ ╚══════╝╚═╝  ╚══╝ ╚════╝    ╚═╝    ╚════╝  ╚════╝ ╚══════╝╚═════╝ 
+    ╚═════╝ ╚══════╝╚═╝  ╚══╝ ╚════╝    ╚═╝    ╚════╝  ╚════╝ ╚══════╝╚═════╝
     """
     return header
-    
+
 
 def shell_do(command, print_cmd=False, log=False, return_log=False, err=False):
     if print_cmd:
         print(f'Executing: {(" ").join(command.split())}', file=sys.stderr)
 
     res=subprocess.run(command.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
@@ -50,55 +50,55 @@
 
     if log:
         print(output)
     if return_log:
         return output
     if err:
         return res.stderr.decode('utf-8')
-    
+
 
 def bfiles_to_pfiles(bfile_path=None, pfile_path=None):
     # check if both are none
     if not (bfile_path or pfile_path):
         print()
         print('ERROR: Need either PLINK1.9 or PLINK2 binaries!')
         print()
-    
+
     elif bfile_path and pfile_path:
         print()
         print('ERROR: Cannot accept both PLINK1.9 and PLINK2 binaries simulaneously!')
         print()
-    
+
     elif bfile_path and (not pfile_path):
         if not os.path.isfile(f'{bfile_path}.bed'):
             raise FileNotFoundError(f'{bfile_path} does not exist.')
 
         convert_cmd = f'{plink2_exec} --bfile {bfile_path} --make-pgen psam-cols=fid,parents,sex,pheno1,phenos --out {bfile_path}'
         shell_do(convert_cmd)
-    
+
     else:
         if not os.path.isfile(f'{pfile_path}.pgen'):
             raise FileNotFoundError(f'{pfile_path} does not exist.')
-        
+
         convert_cmd = f'{plink2_exec} --pfile {pfile_path} --make-bed --out {pfile_path}'
         shell_do(convert_cmd)
 
 
 def vcf_to_pfiles(vcf_path):
     if not os.path.isfile(vcf_path):
         raise FileNotFoundError(f'{vcf_path} does not exist.')
-    
+
     prefix = vcf_path.split('.vcf')[0]
 
     convert_cmd1 = f'{plink2_exec} --vcf {vcf_path} --make-bed --out {prefix}'
     shell_do(convert_cmd1)
 
     if not os.path.isfile(f'{prefix}.bed'):
         raise FileNotFoundError(f'{prefix} bed/bim/fam files do not exist. Conversion from VCF failed')
-    
+
     bfiles_to_pfiles(bfile_path=prefix)
 
     if os.path.isfile(f'{prefix}.pgen'):
         os.remove(f'{prefix}.bed')
         os.remove(f'{prefix}.bim')
         os.remove(f'{prefix}.fam')
     else:
@@ -112,27 +112,27 @@
 
     # if no pgen present, but bed is present, and skip fails is True, convert to pgen
     if not os.path.isfile(f'{geno_path}.pgen') and os.path.isfile(f'{geno_path}.bed') and (not args['skip_fails']):
         warnings.warn(f'{geno_path} exists but it is in PLINK1.9 binary format. Converting to PLINK2 binaries...', stacklevel=2)
         bfiles_to_pfiles(bfile_path=geno_path)
 
     sam = pd.read_csv(f'{geno_path}.psam', sep = '\s+')
-    var = pd.read_csv(f'{geno_path}.pvar', sep = '\s+', low_memory = False)
+    var = pd.read_csv(f'{geno_path}.pvar', delimiter='\t', comment='#', header=None, names=['#CHROM', 'POS', 'ID', 'REF', 'ALT', 'FILTER', 'INFO'], low_memory=False)
 
-    if 'SEX' not in sam.columns: 
+    if 'SEX' not in sam.columns:
         raise KeyError(f'{geno_path}.psam is missing SEX column. Even if no SEX information is present, GenoTools requires a SEX column.')
-    
+
     if 'PHENO1' not in sam.columns:
         raise KeyError(f'{geno_path}.psam is missing PHENO1 column. Even if no PHENO1 information is present, GenoTools requires a PHENO1 column.')
 
     sex_counts = sam['SEX'].value_counts().to_dict()
     pheno_counts = sam['PHENO1'].value_counts().to_dict()
     chr_counts = var['#CHROM'].value_counts().to_dict()
 
-    # print breakdown of data 
+    # print breakdown of data
     print("Your data has the following breakdown:")
     print("- Genetic Sex:")
     for sex in sex_counts.keys():
         if sex == 1:
             print(f'{sex_counts[sex]} Males \n')
         if sex == 2:
             print(f'{sex_counts[sex]} Females \n')
@@ -161,20 +161,20 @@
                 warnings.warn('You tried calling sex prune but no X chromosome data is available. Skipping...', stacklevel=2)
                 args['sex'] = None
 
         # change hwe prune to be run without controls filtered when no controls present
         if (args['hwe'] is not None) and (args['filter_controls'] == True) and (1 not in pheno_counts.keys()):
             warnings.warn('You tried calling hwe prune with controls filtered but no controls are available. Skipping...', stacklevel=2)
             args['filter_controls'] = False
-        
+
         # skip case control when called without cases or controls present
         if (args['case_control'] is not None) and ((1 not in pheno_counts.keys()) or (2 not in pheno_counts.keys())):
             warnings.warn('You tried calling case-control prune but only cases or controls are available, not both. Skipping...', stacklevel=2)
             args['case_control'] = None
-        
+
         # skip het prune if less than 50 samples are present
         if (args['het'] is not None) and (var.shape[0] < 50):
             warnings.warn('You tried calling het prune with less than 50 samples. Skipping...', stacklevel=2)
             args['het'] = None
 
         return args
 
@@ -189,28 +189,28 @@
 def process_log(out_path, concat_log):
     out_dir = os.path.dirname(os.path.abspath(out_path))
 
     # ancestry labels
     ancestries = ['AFR', 'SAS', 'EAS', 'EUR', 'AMR', 'AJ', 'CAS', 'MDE', 'FIN', 'AAC']
 
     # exclude lines containing this information from log file
-    exclude = ['Hostname', 'Working directory', 'Intel', 'Start time', 'Random number seed', 'RAM detected', 'threads', 'thread', 
+    exclude = ['Hostname', 'Working directory', 'Intel', 'Start time', 'Random number seed', 'RAM detected', 'threads', 'thread',
     'written to', 'done.', 'End time:', 'Writing', '.bed', '.bim', '.fam', '.id', '.hh', '.sexcheck', '.psam', '-bit', 'from',
     '.pvar', '.pgen', '.in', '.out', '.het', '.missing', '.snplist', '.kin0', '.eigenvec', '.eigenval', '(--maf/', '--make-bed to','+']
 
     # save all indices in log file where these instances occur
     step_indices = [i for i, s in enumerate(concat_log) if 'Log:' in s]
-    out_indices = [i for i, s in enumerate(concat_log) if '--out' in s]
+    out_indices = [i for i, s in enumerate(concat_log) if any(x in s for x in ('--prefix', '--out'))]
     ancestry_ran = [True if 'split_cohort_ancestry' in line else False for line in concat_log]
 
     # add final index of log to traverse entire log
     step_indices.append(len(concat_log))
     start = 0
     stop = 1
-    
+
     # exclude/replace from text
     fillers = ['and', '.']
     replace = {'loaded from': 'loaded', '(see': '', ');': ';'}
 
     # write final processed log
     with open(f"{out_path}_cleaned_logs.log", "w") as f:
         header = gt_header()
@@ -224,15 +224,15 @@
 
             # write final labels for concise step name & ancestry of focus
             if any(ancestry_ran):
                 # find ancestry acronym in output line
                 ancestry_tokens = [s for s in out_name.split("_") if s in ancestries]
                 if len(ancestry_tokens) >= 1:
                     f.write(f'Ancestry: {ancestry_tokens[-1]}\n')
-            
+
             # rewrite concatenated log section by section with exclusion criteria
             for i in range(step_indices[start], step_indices[stop]):
                 if "error" in concat_log[i].strip('\n'):
                     f.write(concat_log[i])
                 elif concat_log[i].strip('\n') in fillers:
                     pass
                 elif len(concat_log[i]) == 1:
@@ -261,15 +261,15 @@
         if file.endswith("_all_logs.log"):
             # log_exists = True
             log_paths.append(file)
 
     # if no genotools logs exist, create one
     if len(log_paths) == 0:
         log_path = os.path.join(out_dir, os.path.split(out_path)[1])
-    
+
     # if one genotools log exists, point to it
     if len(log_paths) == 1:
         log_path = os.path.join(out_dir, log_paths[0])
 
     # if more than one genotools log exists, point to the one modified most recently
     if len(log_paths) > 1:
         mtimes = {}
@@ -284,15 +284,15 @@
             with open(name) as file:
                 new_file.write(f'Log: {name}\n')
                 new_file.write(f'Process: {step}\n')
                 for line in file:
                     new_file.write(line)
                 new_file.write("\n")
 
-    # remove intermediate log files 
+    # remove intermediate log files
     for files in listOfFiles:
         os.remove(files)
 
     # calls for processing
     with open(log_path, 'r') as file:
         out_path = log_path.replace('_all_logs.log', '')
         process_log(out_path, file.readlines())
@@ -311,31 +311,31 @@
     if not os.path.exists(gene_reference):
         raise FileNotFoundError(f"{gene_reference} not found")
 
     # Load SNP data from bim file
     snps = pd.read_table(bim_file, sep='\s+', header=None, names=['chr', 'snp_id', 'cm_pos', 'pos', 'a1', 'a2'], dtype={'chr': str})
     # Load gene information
     glist = pd.read_table(gene_reference, sep='\s+', header=None, names=['chr', 'start', 'end', 'name'], dtype={'chr': str})
-    
+
     # convert glist chr X to 23, Y to 24, XY to 25
     glist.loc[glist.chr=='X', 'chr'] = '23'
     glist.loc[glist.chr=='Y', 'chr'] = '24'
     glist.loc[glist.chr=='XY', 'chr'] = '25'
 
     # Add a new column to hold the gene labels
     snps['gene'] = 'NA'
 
     # Loop through each row in the gene list
     for _, row in glist.iterrows():
 
         start = row['start'] - locus_size
         stop = row['end'] + locus_size
         # Find the positions that fall within the current start and stop values
-        include_snps = snps.loc[(snps['chr'] == row['chr']) & 
-                                (snps['pos'] >= start) & 
+        include_snps = snps.loc[(snps['chr'] == row['chr']) &
+                                (snps['pos'] >= start) &
                                 (snps['pos'] <= stop)].copy()
 
         # Assign gene name to included SNPs
         include_snps.loc[:, 'gene'] = row['name']
 
         # Update the label for the included SNPs
         snps.update(include_snps)
@@ -364,84 +364,84 @@
             bash5 = f"{plink_exec} --bfile {geno_path1}_flip_pruned --allow-no-sex --bmerge {geno_path2} --out  {out_name} --make-bed"
 
             cmds2 = [bash4, bash5]
 
             for cmd in cmds2:
                 shell_do(cmd)
 
-        # if second attempt at merge is successful, there are no triallelic snps and we can go ahead and move the _flip files to our _merged_ref_panel filenames 
+        # if second attempt at merge is successful, there are no triallelic snps and we can go ahead and move the _flip files to our _merged_ref_panel filenames
         # for further processing
         else:
             suffix_list = ['bed','bim','fam']
             for suffix in suffix_list:
                 shutil.copy(f'{out_name}_flip.{suffix}',f'{out_name}.{suffix}')
 
     # if first merge works, there are no alleles in need of flipping and no triallelic positions and we can proceed!
     else:
         pass
 
-        
+
 def ld_prune(geno_path, out_name, window_size=1000, step_size=50, rsq_thresh=0.05):
     # now prune for LD
     ld_prune1 = f'{plink_exec} --bfile {geno_path} --allow-no-sex --indep-pairwise {window_size} {step_size} {rsq_thresh} --autosome --out {geno_path}_pruned_data'
     ld_prune2 = f'{plink_exec} --bfile {geno_path} --allow-no-sex --extract {geno_path}_pruned_data.prune.in --make-bed --out {out_name}'
 
     ld_prune_cmds = [ld_prune1, ld_prune2]
 
     for cmd in ld_prune_cmds:
         shell_do(cmd)
-    
 
-def get_common_snps(geno_path1, geno_path2, out_name):  
-    
+
+def get_common_snps(geno_path1, geno_path2, out_name):
+
     """
-    Gets common snps between 2 genotype files and extracts from geno_path1. outputs plink bed/bim/fam file 
+    Gets common snps between 2 genotype files and extracts from geno_path1. outputs plink bed/bim/fam file
     for geno_path1 with only matching snps from geno_path2
     """
-   
-    print('Getting Common SNPs')	
-    
+
+    print('Getting Common SNPs')
+
     # read both bim files
     bim1 = pd.read_csv(f'{geno_path1}.bim', sep='\t', header=None)
     bim1.columns = ['chr', 'rsid', 'kb', 'pos', 'a1', 'a2']
     bim2 = pd.read_csv(f'{geno_path2}.bim', sep='\t', header=None)
     bim2.columns = ['chr', 'rsid', 'kb', 'pos', 'a1', 'a2']
-    
+
     # write bim 1 ids to snplist
     bim1['rsid'].to_csv(f'{geno_path1}.snplist', sep='\t', header=None, index=None)
 
     # creating merge ids
     bim1['merge_id'] = bim1['chr'].astype(str) + ':' + bim1['pos'].astype(str) + ':' + bim1['a2'] + ':' + bim1['a1']
     bim2['merge_id1'] = bim2['chr'].astype(str) + ':' + bim2['pos'].astype(str) + ':' + bim2['a2'] + ':' + bim2['a1']
     bim2['merge_id2'] = bim2['chr'].astype(str) + ':' + bim2['pos'].astype(str) + ':' + bim2['a1'] + ':' + bim2['a2']
 
     # two merges and concatenation
     common_snps1 = bim2[['rsid','merge_id1','a1','a2']].merge(bim1, how='inner', left_on=['merge_id1'], right_on=['merge_id'])
-    common_snps2 = bim2[['rsid','merge_id2','a1','a2']].merge(bim1, how='inner', left_on=['merge_id2'], right_on=['merge_id'])	
+    common_snps2 = bim2[['rsid','merge_id2','a1','a2']].merge(bim1, how='inner', left_on=['merge_id2'], right_on=['merge_id'])
     common_snps = pd.concat([common_snps1, common_snps2], axis=0)
-    
+
     # flip and merge again
     flip_cmd = f'{plink_exec} --bfile {geno_path1} --flip {geno_path1}.snplist --make-bed --out {geno_path1}_flip'
     shell_do(flip_cmd)
 
     bim1_flip = pd.read_csv(f'{geno_path1}_flip.bim', sep='\t', header=None)
     bim1_flip.columns = ['chr', 'rsid', 'kb', 'pos', 'a1', 'a2']
 
     bim1_flip['merge_id'] = bim1_flip['chr'].astype(str) + ':' + bim1_flip['pos'].astype(str) + ':' + bim1_flip['a2'] + ':' + bim1_flip['a1']
     common_snps1 = bim2[['rsid','merge_id1','a1','a2']].merge(bim1_flip, how='inner', left_on=['merge_id1'], right_on=['merge_id'])
-    common_snps2 = bim2[['rsid','merge_id2','a1','a2']].merge(bim1_flip, how='inner', left_on=['merge_id2'], right_on=['merge_id'])	
+    common_snps2 = bim2[['rsid','merge_id2','a1','a2']].merge(bim1_flip, how='inner', left_on=['merge_id2'], right_on=['merge_id'])
 
     # concat merges and drop duplicates
     common_snps = pd.concat([common_snps, common_snps1, common_snps2], axis=0)
     common_snps = common_snps.drop_duplicates(subset=['chr','pos'], ignore_index=True)
 
     # write snps to txt and extract
     common_snps_file = f'{out_name}.common_snps'
     common_snps['rsid_y'].to_csv(f'{common_snps_file}', sep='\t', header=False, index=False)
-    
+
     ext_snps_cmd = f'{plink2_exec} --bfile {geno_path1} --extract {common_snps_file} --make-bed --out {out_name}'
     shell_do(ext_snps_cmd)
 
     # return outfiles
     outfiles = {
         'common_snps': common_snps_file,
         'bed': out_name
@@ -498,34 +498,34 @@
     avg_vmiss = vmiss.F_MISS.mean()
     avg_smiss = smiss.F_MISS.mean()
     # print(f'Average Missing Call Rate (lmiss): {avg_lmiss}')
     # print(f'Average Missing Genotyping Rate (imiss): {avg_imiss}')
 
     s_total = smiss.shape[0]
     thresh_list = np.arange(0.0, max_threshold+0.01, 0.01)
-    
+
     # suggest most-stringent threshold which retains >= 90% of samples
     accept_list = []
-    
+
     for thresh in thresh_list:
-        
+
         s_pass = smiss.loc[smiss.F_MISS<=thresh]
         pass_prop = s_pass.shape[0]/s_total
 
         if pass_prop < 0.9:
             pass
         else:
             accept_list.append(thresh)
-    
+
     if len(accept_list) > 0:
         suggested_threshold = min(accept_list)
     else:
         print('No acceptable threshold found! Try a less-stringent max_threshold')
         suggested_threshold = None
-        
+
     metrics = {
         'avg_lmiss': avg_vmiss,
         'avg_imiss': avg_smiss,
         'suggested_threshold': suggested_threshold
     }
 
     return metrics
@@ -533,25 +533,25 @@
 
 def zscore_pval_conversion(zscores=None, pvals=None, stats=None):
 
     # neither zscore or pvals provided provided
     if zscores is None and pvals is None:
         print('Conversion Failed!')
         print('Either p-values or z-scores must be provided')
-    
+
     # both zscores and pvals provided
     elif zscores is not None and pvals is not None:
         print('Conversion Failed!')
         print('Provide only p-values or z-scores, not both')
-    
+
     # pvals provided but stats not provided to determine sign of zscore
     elif pvals is not None and stats is None:
         print('Conversion Failed!')
         print('Stats must be provided when going from p-values to z-scores')
-    
+
     else:
         # convert pvals to zscores using stats to get proper sign
         if zscores is None:
             z = np.where(stats > 0, norm.isf(pvals/2), -norm.isf(pvals/2))
             return z
         # convert zscores to pvals
         if pvals is None:
```

### Comparing `the_real_genotools-1.2.1/setup.py` & `the_real_genotools-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='the_real_genotools', 
-    version='1.2.1', 
+    version='1.2.2', 
     packages=find_packages(),
     author='Dan Vitale',
     author_email='d.vitale199@gmail.com',
     description='A collection of tools for genotype quality control and analysis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dvitale199/GenoTools',
```

### Comparing `the_real_genotools-1.2.1/the_real_genotools.egg-info/PKG-INFO` & `the_real_genotools-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: the-real-genotools
-Version: 1.2.1
+Name: the_real_genotools
+Version: 1.2.2
 Summary: A collection of tools for genotype quality control and analysis
 Home-page: https://github.com/dvitale199/GenoTools
 Author: Dan Vitale
 Author-email: d.vitale199@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # GenoTools
 [![DOI](https://zenodo.org/badge/337965715.svg)](https://zenodo.org/doi/10.5281/zenodo.10443257)
 
+## Documentation
+You can find the full documentation with the following links:
+- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
+- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
+- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+- [JSON output guide](https://github.com/dvitale199/GenoTools/blob/main/docs/json_output_overview.md)
+
 ## Getting Started
 
 GenoTools is a suite of automated genotype data processing steps written in Python. The core pipeline was built for Quality Control and Ancestry estimation of data in the Global Parkinson's Genetics Program (GP2)
 
 To download the most current version from pip:
 ```
 pip install the_real_genotools
@@ -82,18 +89,15 @@
 ```
 Note: add the ```--singularity``` flag to run containerized ancestry predictions on HPC
 
 This will find common snps between your genotype data and the reference panel, run PCA, UMAP-transform PCs, and train a new XGBoost classifier specific to your data/ref panel.
 
 genotools accept `--pfile`, `--bfile`, or `--vcf`. Any bfile or vcf will be converted to a pfile before running any steps. 
 
-## Documentation
-- [GenoTools Command Line Arguments](https://github.com/dvitale199/GenoTools/blob/main/docs/cli_args.md)
-- [Default Pipeline Overview](https://github.com/dvitale199/GenoTools/blob/main/docs/default_pipeline_overview.md)
-- [Package Function Guide (for developers)](https://github.com/dvitale199/GenoTools/blob/main/docs/genotools_function_guide.md)
+Please consult the docs links listed at the top of the README for the full argument guide, function guide, Default pipeline overview, and guide for navigating the output JSON.
 
 ## Acknowledgements
 GenoTools was developed as the core genotype and wgs processing pipeline for the Global Parkinson's Genetics Program (GP2) at the Center for Alzheimer's and Related Dementias (CARD) at the National Institutes of Health.
 
 This tool relies on PLINK, a whole genome association analysis toolset, for various genetic data processing functionalities. We gratefully acknowledge the developers of PLINK for their foundational contributions to the field of genetics. More about PLINK can be found at [their website](https://www.cog-genomics.org/plink/2.0/).
```

### Comparing `the_real_genotools-1.2.1/the_real_genotools.egg-info/SOURCES.txt` & `the_real_genotools-1.2.2/the_real_genotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

