# Comparing `tmp/ribotricer-1.3.3.tar.gz` & `tmp/ribotricer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ribotricer-1.3.3.tar", last modified: Thu Feb  9 19:38:51 2023, max compression
+gzip compressed data, was "ribotricer-1.4.0.tar", last modified: Sat Apr 13 19:28:29 2024, max compression
```

## Comparing `ribotricer-1.3.3.tar` & `ribotricer-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 saket      (501) staff       (20)        0 2023-02-09 19:38:51.437295 ribotricer-1.3.3/
--rw-r--r--   0 saket      (501) staff       (20)       68 2023-01-10 15:09:06.000000 ribotricer-1.3.3/AUTHORS
--rw-r--r--   0 saket      (501) staff       (20)     1633 2023-02-09 19:30:37.000000 ribotricer-1.3.3/HISTORY.md
--rw-r--r--   0 saket      (501) staff       (20)    35211 2023-01-10 15:09:06.000000 ribotricer-1.3.3/LICENSE
--rw-r--r--   0 saket      (501) staff       (20)      177 2023-01-10 15:09:06.000000 ribotricer-1.3.3/MANIFEST.in
--rw-r--r--   0 saket      (501) staff       (20)    11919 2023-02-09 19:38:51.437515 ribotricer-1.3.3/PKG-INFO
--rw-r--r--   0 saket      (501) staff       (20)    10895 2023-01-10 15:09:06.000000 ribotricer-1.3.3/README.md
--rw-r--r--   0 saket      (501) staff       (20)      154 2023-01-10 15:09:06.000000 ribotricer-1.3.3/requirements.txt
-drwxr-xr-x   0 saket      (501) staff       (20)        0 2023-02-09 19:38:51.434953 ribotricer-1.3.3/ribotricer/
--rw-r--r--   0 saket      (501) staff       (20)      112 2023-02-09 19:35:20.000000 ribotricer-1.3.3/ribotricer/__init__.py
--rw-r--r--   0 saket      (501) staff       (20)     5433 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/bam.py
--rw-r--r--   0 saket      (501) staff       (20)    15852 2023-02-09 17:41:09.000000 ribotricer-1.3.3/ribotricer/cli.py
--rw-r--r--   0 saket      (501) staff       (20)     3513 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/common.py
--rw-r--r--   0 saket      (501) staff       (20)     1222 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/const.py
--rw-r--r--   0 saket      (501) staff       (20)     8986 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/count_orfs.py
--rw-r--r--   0 saket      (501) staff       (20)    15936 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/detect_orfs.py
--rw-r--r--   0 saket      (501) staff       (20)     4337 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/fasta.py
--rw-r--r--   0 saket      (501) staff       (20)     4727 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/gtf.py
--rw-r--r--   0 saket      (501) staff       (20)     3912 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/infer_protocol.py
--rw-r--r--   0 saket      (501) staff       (20)     1323 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/interval.py
--rw-r--r--   0 saket      (501) staff       (20)     8849 2023-01-16 18:27:50.000000 ribotricer-1.3.3/ribotricer/learn_cutoff.py
--rw-r--r--   0 saket      (501) staff       (20)     9755 2023-01-11 16:56:00.000000 ribotricer-1.3.3/ribotricer/metagene.py
--rw-r--r--   0 saket      (501) staff       (20)     5700 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/orf.py
--rw-r--r--   0 saket      (501) staff       (20)     4280 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/orf_seq.py
--rw-r--r--   0 saket      (501) staff       (20)     4452 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/plotting.py
--rw-r--r--   0 saket      (501) staff       (20)    12128 2023-02-09 17:44:02.000000 ribotricer-1.3.3/ribotricer/prepare_orfs.py
--rw-r--r--   0 saket      (501) staff       (20)     3294 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/statistics.py
--rw-r--r--   0 saket      (501) staff       (20)    14483 2023-01-10 15:09:06.000000 ribotricer-1.3.3/ribotricer/utils.py
-drwxr-xr-x   0 saket      (501) staff       (20)        0 2023-02-09 19:38:51.437033 ribotricer-1.3.3/ribotricer.egg-info/
--rw-r--r--   0 saket      (501) staff       (20)    11919 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/PKG-INFO
--rw-r--r--   0 saket      (501) staff       (20)      728 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/SOURCES.txt
--rw-r--r--   0 saket      (501) staff       (20)        1 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/dependency_links.txt
--rw-r--r--   0 saket      (501) staff       (20)       50 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/entry_points.txt
--rw-r--r--   0 saket      (501) staff       (20)      154 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/requires.txt
--rw-r--r--   0 saket      (501) staff       (20)       11 2023-02-09 19:38:51.000000 ribotricer-1.3.3/ribotricer.egg-info/top_level.txt
--rw-r--r--   0 saket      (501) staff       (20)     3348 2023-01-10 15:09:06.000000 ribotricer-1.3.3/run_test.sh
--rw-r--r--   0 saket      (501) staff       (20)      712 2023-02-09 19:38:51.438245 ribotricer-1.3.3/setup.cfg
--rw-r--r--   0 saket      (501) staff       (20)     2049 2023-02-09 19:35:20.000000 ribotricer-1.3.3/setup.py
+drwxr-xr-x   0 saket      (501) staff       (20)        0 2024-04-13 19:28:29.254428 ribotricer-1.4.0/
+-rw-r--r--   0 saket      (501) staff       (20)       68 2024-04-13 16:51:19.000000 ribotricer-1.4.0/AUTHORS
+-rw-r--r--   0 saket      (501) staff       (20)     1822 2024-04-13 19:25:45.000000 ribotricer-1.4.0/HISTORY.md
+-rw-r--r--   0 saket      (501) staff       (20)    35211 2024-04-13 16:51:19.000000 ribotricer-1.4.0/LICENSE
+-rw-r--r--   0 saket      (501) staff       (20)      177 2024-04-13 16:51:19.000000 ribotricer-1.4.0/MANIFEST.in
+-rw-r--r--   0 saket      (501) staff       (20)    12240 2024-04-13 19:28:29.254344 ribotricer-1.4.0/PKG-INFO
+-rw-r--r--   0 saket      (501) staff       (20)    10760 2024-04-13 16:51:19.000000 ribotricer-1.4.0/README.md
+-rw-r--r--   0 saket      (501) staff       (20)      154 2024-04-13 16:51:19.000000 ribotricer-1.4.0/requirements.txt
+drwxr-xr-x   0 saket      (501) staff       (20)        0 2024-04-13 19:28:29.252734 ribotricer-1.4.0/ribotricer/
+-rw-r--r--   0 saket      (501) staff       (20)      112 2024-04-13 19:27:30.000000 ribotricer-1.4.0/ribotricer/__init__.py
+-rw-r--r--   0 saket      (501) staff       (20)     5433 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/bam.py
+-rw-r--r--   0 saket      (501) staff       (20)    16007 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/cli.py
+-rw-r--r--   0 saket      (501) staff       (20)     3582 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/common.py
+-rw-r--r--   0 saket      (501) staff       (20)     1307 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/const.py
+-rw-r--r--   0 saket      (501) staff       (20)     9455 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/count_orfs.py
+-rw-r--r--   0 saket      (501) staff       (20)    16416 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/detect_orfs.py
+-rw-r--r--   0 saket      (501) staff       (20)     4337 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/fasta.py
+-rw-r--r--   0 saket      (501) staff       (20)     4727 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/gtf.py
+-rw-r--r--   0 saket      (501) staff       (20)     3912 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/infer_protocol.py
+-rw-r--r--   0 saket      (501) staff       (20)     1323 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/interval.py
+-rw-r--r--   0 saket      (501) staff       (20)     8849 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/learn_cutoff.py
+-rw-r--r--   0 saket      (501) staff       (20)     9757 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/metagene.py
+-rw-r--r--   0 saket      (501) staff       (20)     5750 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/orf.py
+-rw-r--r--   0 saket      (501) staff       (20)     4269 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/orf_seq.py
+-rw-r--r--   0 saket      (501) staff       (20)     4546 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/plotting.py
+-rw-r--r--   0 saket      (501) staff       (20)    12127 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/prepare_orfs.py
+-rw-r--r--   0 saket      (501) staff       (20)     3294 2024-04-13 18:26:57.000000 ribotricer-1.4.0/ribotricer/statistics.py
+-rw-r--r--   0 saket      (501) staff       (20)    14482 2024-04-13 19:24:48.000000 ribotricer-1.4.0/ribotricer/utils.py
+drwxr-xr-x   0 saket      (501) staff       (20)        0 2024-04-13 19:28:29.254117 ribotricer-1.4.0/ribotricer.egg-info/
+-rw-r--r--   0 saket      (501) staff       (20)    12240 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/PKG-INFO
+-rw-r--r--   0 saket      (501) staff       (20)      728 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/SOURCES.txt
+-rw-r--r--   0 saket      (501) staff       (20)        1 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/dependency_links.txt
+-rw-r--r--   0 saket      (501) staff       (20)       50 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/entry_points.txt
+-rw-r--r--   0 saket      (501) staff       (20)      154 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/requires.txt
+-rw-r--r--   0 saket      (501) staff       (20)       11 2024-04-13 19:28:29.000000 ribotricer-1.4.0/ribotricer.egg-info/top_level.txt
+-rw-r--r--   0 saket      (501) staff       (20)     3348 2024-04-13 18:22:22.000000 ribotricer-1.4.0/run_test.sh
+-rw-r--r--   0 saket      (501) staff       (20)      712 2024-04-13 19:28:29.254769 ribotricer-1.4.0/setup.cfg
+-rw-r--r--   0 saket      (501) staff       (20)     2198 2024-04-13 19:27:30.000000 ribotricer-1.4.0/setup.py
```

### Comparing `ribotricer-1.3.3/HISTORY.md` & `ribotricer-1.4.0/HISTORY.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# V1.3.3 (2022-02-09)
+# v1.4.0 (2024-04-14)
+
+- Added `meta_min_reads` parameter to control minimum coverage for metagene plots ([#155](https://github.com/smithlabcode/ribotricer/pull/155))
+- Formatting changes
+
+# v1.3.3 (2022-02-09)
 
 - Print start codons when preparing orfs
 - Fix for custom start codons
 
 # v1.3.2 (2020-05-03)
 
 - Better support for extracting sequences from non-conventional GTFs
```

### Comparing `ribotricer-1.3.3/LICENSE` & `ribotricer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/PKG-INFO` & `ribotricer-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,11 @@
-Metadata-Version: 2.1
-Name: ribotricer
-Version: 1.3.3
-Summary: Python package to detect translating ORFs from Ribo-seq data
-Home-page: https://github.com/smithlabcode/ribotricer
-Author: Saket Choudhary, Wenzheng Li
-Author-email: saketkc@gmail.com
-Maintainer: Saket Choudhary
-Maintainer-email: saketkc@gmail.com
-License: GPLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 ![alt text](./ribotricer_logo.png)
 
 # ribotricer: Accurate detection of short and long active ORFs using Ribo-seq data
 
-[![Build Status](https://img.shields.io/travis/smithlabcode/ribotricer.svg?style=flat)](https://travis-ci.org/smithlabcode/ribotricer)
 [![install with pip](https://img.shields.io/pypi/v/ribotricer.svg?style=flat)](https://pypi.org/project/ribotricer/)
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/ribotricer/README.html)
 ![python versions](https://img.shields.io/pypi/pyversions/ribotricer)
 [![pypi downloads](https://img.shields.io/pypi/dm/ribotricer)](https://pypi.org/project/ribotricer/)
 [![Downloads](https://anaconda.org/bioconda/ribotricer/badges/downloads.svg)](https://anaconda.org/bioconda/ribotricer)
 [![license](https://img.shields.io/pypi/l/ribotricer)](LICENSE)
```

### Comparing `ribotricer-1.3.3/README.md` & `ribotricer-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,51 @@
+Metadata-Version: 2.1
+Name: ribotricer
+Version: 1.4.0
+Summary: Python package to detect translating ORFs from Ribo-seq data
+Home-page: https://github.com/smithlabcode/ribotricer
+Author: Saket Choudhary, Wenzheng Li
+Author-email: saketkc@gmail.com
+Maintainer: Saket Choudhary
+Maintainer-email: saketkc@gmail.com
+License: GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: click>=8.1.3
+Requires-Dist: click-help-colors>=0.9.1
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: numpy>=1.21.1
+Requires-Dist: pandas>=1.3
+Requires-Dist: pyfaidx>=0.7.1
+Requires-Dist: pysam>=0.19.1
+Requires-Dist: quicksect>=0.2.2
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: tqdm>=4.64.1
+
 ![alt text](./ribotricer_logo.png)
 
 # ribotricer: Accurate detection of short and long active ORFs using Ribo-seq data
 
-[![Build Status](https://img.shields.io/travis/smithlabcode/ribotricer.svg?style=flat)](https://travis-ci.org/smithlabcode/ribotricer)
 [![install with pip](https://img.shields.io/pypi/v/ribotricer.svg?style=flat)](https://pypi.org/project/ribotricer/)
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/ribotricer/README.html)
 ![python versions](https://img.shields.io/pypi/pyversions/ribotricer)
 [![pypi downloads](https://img.shields.io/pypi/dm/ribotricer)](https://pypi.org/project/ribotricer/)
 [![Downloads](https://anaconda.org/bioconda/ribotricer/badges/downloads.svg)](https://anaconda.org/bioconda/ribotricer)
 [![license](https://img.shields.io/pypi/l/ribotricer)](LICENSE)
```

### Comparing `ribotricer-1.3.3/ribotricer/bam.py` & `ribotricer-1.4.0/ribotricer/bam.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/cli.py` & `ribotricer-1.4.0/ribotricer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from . import __version__
 from .common import _clean_input
 from .const import CUTOFF
 from .const import MINIMUM_VALID_CODONS
 from .const import MINIMUM_VALID_CODONS_RATIO
 from .const import MINIMUM_READS_PER_CODON
 from .const import MINIMUM_DENSITY_OVER_ORF
+from .const import META_MIN_READS
 
 from .count_orfs import count_orfs
 from .count_orfs import count_orfs_codon
 from .detect_orfs import detect_orfs
 from .learn_cutoff import determine_cutoff_bam
 from .learn_cutoff import determine_cutoff_tsv
 
@@ -45,15 +46,15 @@
 )
 @click.version_option(version=__version__)
 def cli():
     """ribotricer: Tool for detecting translating ORF from Ribo-seq data"""
     pass
 
 
-###################### prepare-orfs function #########################################
+# prepare-orfs function #########################################
 @cli.command(
     "prepare-orfs",
     context_settings=CONTEXT_SETTINGS,
     help="Extract candidate ORFS based on GTF and FASTA files",
 )
 @click.option("--gtf", help="Path to GTF file", required=True)
 @click.option("--fasta", help="Path to FASTA file", required=True)
@@ -106,15 +107,15 @@
     if not all([len(x) == 3 and set(x) <= {"A", "C", "G", "T"} for x in stop_codons]):
         sys.exit("Error: invalid codon, only A, C, G, T allowed")
 
     print("Using start codons: {}".format(",".join(start_codons)))
     prepare_orfs(gtf, fasta, prefix, min_orf_length, start_codons, stop_codons, longest)
 
 
-###################### detect-orfs function #########################################
+# detect-orfs function #########################################
 @cli.command(
     "detect-orfs",
     context_settings=CONTEXT_SETTINGS,
     help="Detect translating ORFs from BAM file",
 )
 @click.option("--bam", help="Path to BAM file", required=True)
 @click.option(
@@ -193,48 +194,58 @@
     help="Minimum read density (total_reads/length) over an ORF total codons for determining active translation",
 )
 @click.option(
     "--report_all",
     help=("Whether output all ORFs including those " "non-translating ones"),
     is_flag=True,
 )
+@click.option(
+    "--meta-min-reads",
+    type=int,
+    default=META_MIN_READS,
+    show_default=True,
+    help="Minimum number of reads for a read length to be considered",
+)
 def detect_orfs_cmd(
     bam,
     ribotricer_index,
     prefix,
     stranded,
     read_lengths,
     psite_offsets,
     phase_score_cutoff,
     min_valid_codons,
     min_reads_per_codon,
     min_valid_codons_ratio,
     min_read_density,
     report_all,
+    meta_min_reads,
 ):
     if not os.path.isfile(bam):
         sys.exit("Error: BAM file not found")
 
     if not os.path.isfile(ribotricer_index):
         sys.exit("Error: ribotricer index file not found")
 
     if read_lengths is not None:
         try:
             read_lengths = [int(x.strip()) for x in read_lengths.strip().split(",")]
-        except:
+        except Exception:
             sys.exit("Error: cannot convert read_lengths into integers")
         if not all([x > 0 for x in read_lengths]):
             sys.exit("Error: read length must be positive")
 
     if read_lengths is None and psite_offsets is not None:
         sys.exit("Error: psite_offsets only allowed when read_lengths is provided")
     if read_lengths is not None and psite_offsets is not None:
         try:
-            psite_offsets = [int(x.strip()) for x in psite_offsets.strip().split(",")]
-        except:
+            psite_offsets = [
+                int(x.strip()) for x in psite_offsets.strip().split(",")
+            ]
+        except Exception:
             sys.exit("Error: cannot convert psite_offsets into integers")
         if len(read_lengths) != len(psite_offsets):
             sys.exit("Error: psite_offsets must match read_lengths")
         if not all(x >= 0 for x in psite_offsets):
             sys.exit("Error: P-site offset must be >= 0")
         if not all(x > y for (x, y) in zip(read_lengths, psite_offsets)):
             sys.exit("Error: P-site offset must be smaller than read length")
@@ -253,15 +264,15 @@
         min_reads_per_codon,
         min_valid_codons_ratio,
         min_read_density,
         report_all,
     )
 
 
-###################### count-orfs function #########################################
+# count-orfs function #########################################
 @cli.command(
     "count-orfs",
     context_settings=CONTEXT_SETTINGS,
     help="Count reads for detected ORFs at gene level",
 )
 @click.option(
     "--ribotricer_index",
@@ -295,15 +306,15 @@
         sys.exit("Error: detected orfs file not found")
 
     features = set(x.strip() for x in features.strip().split(","))
 
     count_orfs(ribotricer_index, detected_orfs, features, out, report_all)
 
 
-###################### count-orfs-codon function #########################################
+# count-orfs-codon function #########################################
 @cli.command(
     "count-orfs-codon",
     context_settings=CONTEXT_SETTINGS,
     help="Count reads for detected ORFs at codon level",
 )
 @click.option(
     "--ribotricer_index",
@@ -355,15 +366,15 @@
         features,
         ribotricer_index_fasta,
         prefix,
         report_all,
     )
 
 
-###################### orfs-seq function #########################################
+# orfs-seq function #########################################
 @cli.command(
     "orfs-seq",
     context_settings=CONTEXT_SETTINGS,
     help="Generate sequence for ORFs in ribotricer's index",
 )
 @click.option(
     "--ribotricer_index",
@@ -384,15 +395,15 @@
 
     if not os.path.isfile(fasta):
         sys.exit("Error: fasta file not found")
 
     orf_seq(ribotricer_index, fasta, saveto, protein)
 
 
-###################### learn-cutoff function #########################################
+# learn-cutoff function #########################################
 @cli.command(
     "learn-cutoff",
     context_settings=CONTEXT_SETTINGS,
     help="Learn phase score cutoff from BAM/TSV file",
 )
 @click.option("--ribo_bams", help="Path(s) to Ribo-seq BAM file separated by comma")
 @click.option("--rna_bams", help="Path(s) to RNA-seq BAM file separated by comma")
```

### Comparing `ribotricer-1.3.3/ribotricer/common.py` & `ribotricer-1.4.0/ribotricer/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         elif read.mapping_quality < 1:
             return False
         # NH tag not set so rely on flags
         elif read.flag in __SAM_NOT_UNIQ_FLAGS__:
             return False
         else:
             sys.stdout.write(
-                "WARNING: ribotricer was unable to detect any tags for determining multimapping status. All the reads will be treated as uniquely mapping\n"
+                "WARNING: ribotricer was unable to detect any tags for "
+                "determining multimapping status. All the reads will be "
+                "treated as uniquely mapping\n"
             )
 
 
 def merge_intervals(intervals):
     """
     Parameters
     ----------
@@ -72,15 +74,17 @@
     while i < len(intervals):
         to_merge = Interval(
             intervals[i].chrom,
             intervals[i].start,
             intervals[i].end,
             intervals[i].strand,
         )
-        while i + 1 < len(intervals) and intervals[i + 1].start <= to_merge.end:
+        while (
+            i + 1 < len(intervals) and intervals[i + 1].start <= to_merge.end
+        ):
             to_merge.end = max(to_merge.end, intervals[i + 1].end)
             i += 1
         merged_intervals.append(to_merge)
         i += 1
     return merged_intervals
 
 
@@ -120,10 +124,11 @@
               Nucleotide level counts
     Returns
     -------
     codon_coverage: list
                     Coverage collapsed to codon level
     """
     codon_coverage = [
-        sum(coverage[current : current + 3]) for current in range(0, len(coverage), 3)
+        sum(coverage[current: current + 3])
+        for current in range(0, len(coverage), 3)
     ]
     return codon_coverage
```

### Comparing `ribotricer-1.3.3/ribotricer/const.py` & `ribotricer-1.4.0/ribotricer/const.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,9 @@
 # default: 0 (decided by CUTOFF and MINIMUM_VALID_CODONS)
 MINIMUM_READS_PER_CODON = 0
 # fraction of codons with non zero reads
 MINIMUM_VALID_CODONS_RATIO = 0
 # Minimum read density over ORF
 # defined as the number of reads per unit length of the ORF
 MINIMUM_DENSITY_OVER_ORF = 0.0
+# Minimum number of reads for a read length to be considered
+META_MIN_READS = 100000
```

### Comparing `ribotricer-1.3.3/ribotricer/count_orfs.py` & `ribotricer-1.4.0/ribotricer/count_orfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from textwrap import wrap
 from .orf import ORF
 
 import numpy as np
 import pandas as pd
 
 
-def count_orfs(ribotricer_index, detected_orfs, features, outfile, report_all=False):
+def count_orfs(
+    ribotricer_index, detected_orfs, features, outfile, report_all=False
+):
     """
     Parameters
     ----------
     ribotricer_index: str
                       Path to the index file generated by ribotricer prepare_orfs
     detected_orfs: str
                    Path to the detected orfs file generated by ribotricer detect_orfs
@@ -53,15 +55,19 @@
             oid, otype, status = fields[:3]
             gene_id, gene_name, gene_type = fields[11:14]
             chrom, strand, start_codon, profile = fields[14:]
             if otype in features:
                 # do not output 'nontranslating' events unless report_all is set
                 if status != "nontranslating" or report_all:
                     intervals = orf_index[oid].intervals
-                    coor = [x for iv in intervals for x in range(iv.start, iv.end + 1)]
+                    coor = [
+                        x
+                        for iv in intervals
+                        for x in range(iv.start, iv.end + 1)
+                    ]
                     if strand == "-":
                         coor = coor[::-1]
                     profile_stripped = profile.strip()[1:-1].split(", ")
                     profile = list()
                     if profile_stripped[0]:
                         profile = list(map(int, profile_stripped))
                     for pos, cov in zip(coor, profile):
@@ -101,15 +107,17 @@
                             Path to fasta index generated using orf-seq
     prefix: str
            path to output file
     report_all: bool
                 if True, all coverages will be exported
     """
     orf_index = {}
-    fasta_df = pd.read_csv(ribotricer_index_fasta, sep="\t").set_index("ORF_ID")
+    fasta_df = pd.read_csv(ribotricer_index_fasta, sep="\t").set_index(
+        "ORF_ID"
+    )
     read_counts = defaultdict(dict)
     with open(ribotricer_index, "r") as fin:
         # Skip header
         fin.readline()
         for line in fin:
             orf = ORF.from_string(line)
             if orf.category in features:
@@ -122,17 +130,23 @@
             oid, otype, status = fields[:3]
             gene_id, gene_name, gene_type = fields[11:14]
             chrom, strand, start_codon, profile = fields[14:]
             if otype in features:
                 # do not output 'nontranslating' events unless report_all is set
                 if status != "nontranslating" or report_all:
                     intervals = orf_index[oid].intervals
-                    coor = [x for iv in intervals for x in range(iv.start, iv.end + 1)]
+                    coor = [
+                        x
+                        for iv in intervals
+                        for x in range(iv.start, iv.end + 1)
+                    ]
                     codon_coor = [
-                        x for iv in intervals for x in range(iv.start, iv.end + 1, 3)
+                        x
+                        for iv in intervals
+                        for x in range(iv.start, iv.end + 1, 3)
                     ]
                     if strand == "-":
                         coor = coor[::-1]
                     profile_stripped = profile.strip()[1:-1].split(", ")
                     profile = list()
                     if profile_stripped[0]:
                         profile = list(map(int, profile_stripped))
@@ -154,15 +168,25 @@
                     ):
                         if pos not in read_counts[gene_id, codon_seq]:
                             read_counts[gene_id, codon_seq][pos] = cov
 
     # Output count table
     with open("{}_genewise.tsv".format(prefix), "w") as fout:
         fout.write(
-            "gene_id\tcodon\tvalues\tmean_codon_coverage\tmedian_codon_coverage\tvar_codon_coverage\tcodon_occurences\ttotal_codon_coverage\n"
+            "\t".join(
+                "gene_id",
+                "codon",
+                "values",
+                "mean_codon_coverage",
+                "median_codon_coverage",
+                "var_codon_coverage",
+                "codon_occurences",
+                "total_codon_coverage",
+            )
+            + "\n"
         )
         for gene_id, codon_seq in sorted(read_counts):
             values = list(read_counts[gene_id, codon_seq].values())
             codon_occurences = len(values)
             total_codon_coverage = sum(values)
             mean_codon_coverage = np.mean(values)
             median_codon_coverage = np.median(values)
@@ -179,20 +203,24 @@
                     total_codon_coverage,
                 )
             )
     fout_df = pd.read_csv("{}_genewise.tsv".format(prefix), sep="\t")
     fout_df["per_codon_enrichment(total/n_occur)"] = (
         fout_df["total_codon_coverage"] / fout_df["codon_occurences"]
     )
-    fout_df["-log10_relative_enrichment(per_codon/total_gene_coverage)"] = -np.log10(
+    fout_df[
+        "-log10_relative_enrichment(per_codon/total_gene_coverage)"
+    ] = -np.log10(
         fout_df["per_codon_enrichment(total/n_occur)"]
         / fout_df.groupby("gene_id")["total_codon_coverage"].transform("sum")
     )
     # Overwrite
-    fout_df.to_csv("{}_genewise.tsv".format(prefix), sep="\t", index=False, header=True)
+    fout_df.to_csv(
+        "{}_genewise.tsv".format(prefix), sep="\t", index=False, header=True
+    )
     # Remove infs
     fout_df = fout_df.replace([np.inf, -np.inf], np.nan)
     fout_df = fout_df.dropna()
     fout_df["relative_enrichment"] = fout_df[
         "per_codon_enrichment(total/n_occur)"
     ] / fout_df.groupby("gene_id")["total_codon_coverage"].transform("sum")
```

### Comparing `ribotricer-1.3.3/ribotricer/detect_orfs.py` & `ribotricer-1.4.0/ribotricer/detect_orfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,18 @@
         for pos in range(interval.start, interval.end + 1):
             if orf.category == "annotated":
                 try:
                     coverage.append(alignments[strand][(chrom, pos)])
                 except KeyError:
                     coverage.append(0)
             else:
-                if strand in alignments and (chrom, pos) in alignments[strand]:
+                if (
+                    strand in alignments
+                    and (chrom, pos) in alignments[strand]
+                ):
                     coverage.append(alignments[strand][(chrom, pos)])
                 else:
                     coverage.append(0)
 
     for pos in range(last.end + 1, last.end + offset_3p + 1):
         if orf.category == "annotated":
             try:
@@ -262,15 +265,17 @@
                 n_codons = max(1, length // 3)
 
                 # codon level coverage
                 codon_coverage = np.array(collapse_coverage_to_codon(cov))
                 valid_codons_ratio = valid_codons / n_codons
                 # total reads in the ORF divided by the length
                 orf_density = np.sum(codon_coverage) / n_codons
-                codon_coverage_exceeds_min = codon_coverage >= min_reads_per_codon
+                codon_coverage_exceeds_min = (
+                    codon_coverage >= min_reads_per_codon
+                )
                 status = (
                     "translating"
                     if (
                         coh >= phase_score_cutoff
                         and valid_codons >= min_valid_codons
                         and np.all(codon_coverage_exceeds_min)
                         and valid_codons_ratio >= min_valid_codons_ratio
@@ -318,15 +323,17 @@
     for strand in merged_alignments:
         to_write = ""
         cur_chrom = ""
         for chrom, pos in sorted(merged_alignments[strand]):
             if chrom != cur_chrom:
                 cur_chrom = chrom
                 to_write += "variableStep chrom={}\n".format(chrom)
-            to_write += "{}\t{}\n".format(pos, merged_alignments[strand][(chrom, pos)])
+            to_write += "{}\t{}\n".format(
+                pos, merged_alignments[strand][(chrom, pos)]
+            )
         if strand == "+":
             fname = "{}_pos.wig".format(prefix)
         else:
             fname = "{}_neg.wig".format(prefix)
         with open(fname, "w") as output:
             output.write(to_write)
 
@@ -340,14 +347,15 @@
     psite_offsets,
     phase_score_cutoff,
     min_valid_codons,
     min_reads_per_codon,
     min_valid_codons_ratio,
     min_density_over_orf,
     report_all,
+    meta_min_reads=100000,
 ):
     """
     Parameters
     ----------
     bam: str
          Path to the bam file
     ribotricer_index: str
@@ -367,76 +375,94 @@
                    automatically aligned using cross-correlation
     phase_score_cutoff: float
                         Phase score cutoff value for tagging an ORF as translating o
                         or non-translating
     report_all: bool
                 Whether to output all ORFs' scores regardless of translation
                 status
+    meta_min_reads: int
+                    minimum number of reads for a read length to be considered. Passed to metagene_coverage().
     """
     now = datetime.datetime.now()
     print(now.strftime("%b %d %H:%M:%S ..... started ribotricer detect-orfs"))
 
     # parse the index file
     now = datetime.datetime.now()
-    print(now.strftime("%b %d %H:%M:%S ... started parsing ribotricer index file"))
+    print(
+        now.strftime(
+            "%b %d %H:%M:%S ... started parsing ribotricer index file"
+        )
+    )
     annotated, refseq = parse_ribotricer_index(ribotricer_index)
 
     # create directory
     mkdir_p(parent_dir(prefix))
 
     # infer experimental protocol if not provided
     if protocol is None:
         now = datetime.datetime.now()
         print(
             "{} ... {}".format(
-                now.strftime("%b %d %H:%M:%S"), "started inferring experimental design"
+                now.strftime("%b %d %H:%M:%S"),
+                "started inferring experimental design",
             )
         )
         protocol = infer_protocol(bam, refseq, prefix)
     del refseq
 
     # split bam file into strand and read length
     now = datetime.datetime.now()
     print(now.strftime("%b %d %H:%M:%S ... started reading bam file"))
-    alignments, read_length_counts = split_bam(bam, protocol, prefix, read_lengths)
+    alignments, read_length_counts = split_bam(
+        bam, protocol, prefix, read_lengths
+    )
 
     # plot read length distribution
     now = datetime.datetime.now()
     print(
         "{} ... {}".format(
-            now.strftime("%b %d %H:%M:%S"), "started plotting read length distribution"
+            now.strftime("%b %d %H:%M:%S"),
+            "started plotting read length distribution",
         )
     )
     plot_read_lengths(read_length_counts, prefix)
 
     # calculate metagene profiles
     now = datetime.datetime.now()
     print(
         "{} ... {}".format(
             now.strftime("%b %d %H:%M:%S"),
             "started calculating metagene profiles. This may take a long time...",
         )
     )
-    metagenes = metagene_coverage(annotated, alignments, read_length_counts, prefix)
+    metagenes = metagene_coverage(
+        annotated,
+        alignments,
+        read_length_counts,
+        prefix,
+        meta_min_reads=meta_min_reads,
+    )
 
     # plot metagene profiles
     now = datetime.datetime.now()
     print(
         "\n{} ... {}".format(
-            now.strftime("%b %d %H:%M:%S"), "started plotting metagene profiles"
+            now.strftime("%b %d %H:%M:%S"),
+            "started plotting metagene profiles",
         )
     )
     plot_metagene(metagenes, read_length_counts, prefix)
 
     # align metagenes if psite_offsets not provided
     if psite_offsets is None:
         now = datetime.datetime.now()
         print(
             "{} ... {}".format(
-                now.strftime("%b %d %H:%M:%S"), "started inferring P-site offsets"
+                now.strftime("%b %d %H:%M:%S"),
+                "started inferring P-site offsets",
             )
         )
         psite_offsets = align_metagenes(
             metagenes,
             read_length_counts,
             prefix,
             phase_score_cutoff,
```

### Comparing `ribotricer-1.3.3/ribotricer/fasta.py` & `ribotricer-1.4.0/ribotricer/fasta.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/gtf.py` & `ribotricer-1.4.0/ribotricer/gtf.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/infer_protocol.py` & `ribotricer-1.4.0/ribotricer/infer_protocol.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/interval.py` & `ribotricer-1.4.0/ribotricer/interval.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/learn_cutoff.py` & `ribotricer-1.4.0/ribotricer/learn_cutoff.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/metagene.py` & `ribotricer-1.4.0/ribotricer/metagene.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,14 @@
     reference = metagenes[base][0].values
     to_write = "relative lag to base: {}\n".format(base)
     for length, (meta, _, _, _, _, _) in list(metagenes.items()):
         cov = meta.values
         xcorr = np.correlate(reference, cov, "full")
         origin = len(xcorr) // 2
         bound = min(base, length)
-        xcorr = xcorr[origin - bound : origin + bound]
+        xcorr = xcorr[(origin - bound):(origin + bound)]
         lag = np.argmax(xcorr) - len(xcorr) // 2
         psite_offsets[length] = lag + TYPICAL_OFFSET
         to_write += "\tlag of {}: {}\n".format(length, lag)
     with open("{}_psite_offsets.txt".format(prefix), "w") as output:
         output.write(to_write)
     return psite_offsets
```

### Comparing `ribotricer-1.3.3/ribotricer/orf.py` & `ribotricer-1.4.0/ribotricer/orf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,16 @@
             sys.exit(
                 "{}\n{}".format(
                     "Error: unexpected number of columns found for index file",
                     "please run ribotricer prepare-orfs to regenerate",
                 )
             )
             return None
-        oid = fields[0]
+        # ADS: oid below is not used
+        oid = fields[0]  # noqa F841
         category = fields[1]
         tid = fields[2]
         ttype = fields[3]
         gid = fields[4]
         gname = fields[5]
         gtype = fields[6]
         chrom = fields[7]
```

### Comparing `ribotricer-1.3.3/ribotricer/orf_seq.py` & `ribotricer-1.4.0/ribotricer/orf_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         "TGT": "C",
         "TGA": "_",
         "TGG": "W",
     }
     protein = ""
     if len(seq) % 3 == 0:
         for i in range(0, len(seq), 3):
-            codon = seq[i : i + 3]
+            codon = seq[i: i + 3]
             if "N" in codon:
                 protein += "X"
             elif codon not in codon_table:
                 sys.stderr.write(
                     "Found unknown codon {}. Substituing with X..\n".format(codon)
                 )
             else:
@@ -138,14 +138,14 @@
 
             seq = ("").join(fasta.query(intervals))
             if strand == "-":
                 seq = fasta.reverse_complement(seq)
             if translate:
                 if len(seq) % 3 != 0:
                     sys.stderr.write(
-                        "WARNING: Sequence length with ORF ID '{}' is not a multiple of three. Output sequence might be truncated.\n".format(
-                            orf_id
-                        )
+                        "WARNING: Sequence length with ORF ID '{orf_id}' is not "
+                        "a multiple of three. Output sequence might be "
+                        "truncated.\n"
                     )
-                    seq = seq[0 : (len(seq) // 3) * 3]
+                    seq = seq[0: (len(seq) // 3) * 3]
                 seq = translate_nt_to_aa(seq)
             fh.write("{}\t{}\n".format(orf_id, seq))
```

### Comparing `ribotricer-1.3.3/ribotricer/plotting.py` & `ribotricer-1.4.0/ribotricer/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 import numpy as np
 import matplotlib
 matplotlib.use("Agg")
 
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_pdf import PdfPages
+# ADS: verify that matplotlib.use("Agg") must precede imports below
+import matplotlib.pyplot as plt  # noqa E402
+from matplotlib.backends.backend_pdf import PdfPages  # noqa E402
 
 matplotlib.rcParams["pdf.fonttype"] = 42
 matplotlib.rcParams["ps.fonttype"] = 42
 
 
 def plot_read_lengths(read_lengths, prefix):
     """
```

### Comparing `ribotricer-1.3.3/ribotricer/prepare_orfs.py` & `ribotricer-1.4.0/ribotricer/prepare_orfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                 for start in starts:
                     if idx - start >= min_orf_length:
                         ivs = transcript_to_genome_iv(
                             start, idx - 1, intervals, reverse
                         )
                         seq = merged_seq[start:idx]
                         leader = merged_seq[:start]
-                        trailer = merged_seq[idx + 3 :]
+                        trailer = merged_seq[idx + 3:]
                         if ivs:
                             orfs.append((ivs, seq, leader, trailer))
                     if longest:
                         break
                 starts = []
     return orfs
```

### Comparing `ribotricer-1.3.3/ribotricer/statistics.py` & `ribotricer-1.4.0/ribotricer/statistics.py`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/ribotricer/utils.py` & `ribotricer-1.4.0/ribotricer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     protein: str
              Translated sequence of amino acids
     """
 
     protein = ""
     if len(seq) % 3 == 0:
         for i in range(0, len(seq), 3):
-            codon = seq[i : i + 3]
+            codon = seq[i: i + 3]
             protein += CODON_TO_AA[codon]
     return protein
 
 
 def learn_ribotricer_cutoff(roc_input_file):
     """Learn ribotricer phase score cutoff
```

### Comparing `ribotricer-1.3.3/ribotricer.egg-info/PKG-INFO` & `ribotricer-1.4.0/ribotricer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ribotricer
-Version: 1.3.3
+Version: 1.4.0
 Summary: Python package to detect translating ORFs from Ribo-seq data
 Home-page: https://github.com/smithlabcode/ribotricer
 Author: Saket Choudhary, Wenzheng Li
 Author-email: saketkc@gmail.com
 Maintainer: Saket Choudhary
 Maintainer-email: saketkc@gmail.com
 License: GPLv3
@@ -14,26 +14,38 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: click>=8.1.3
+Requires-Dist: click-help-colors>=0.9.1
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: numpy>=1.21.1
+Requires-Dist: pandas>=1.3
+Requires-Dist: pyfaidx>=0.7.1
+Requires-Dist: pysam>=0.19.1
+Requires-Dist: quicksect>=0.2.2
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: tqdm>=4.64.1
 
 ![alt text](./ribotricer_logo.png)
 
 # ribotricer: Accurate detection of short and long active ORFs using Ribo-seq data
 
-[![Build Status](https://img.shields.io/travis/smithlabcode/ribotricer.svg?style=flat)](https://travis-ci.org/smithlabcode/ribotricer)
 [![install with pip](https://img.shields.io/pypi/v/ribotricer.svg?style=flat)](https://pypi.org/project/ribotricer/)
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/ribotricer/README.html)
 ![python versions](https://img.shields.io/pypi/pyversions/ribotricer)
 [![pypi downloads](https://img.shields.io/pypi/dm/ribotricer)](https://pypi.org/project/ribotricer/)
 [![Downloads](https://anaconda.org/bioconda/ribotricer/badges/downloads.svg)](https://anaconda.org/bioconda/ribotricer)
 [![license](https://img.shields.io/pypi/l/ribotricer)](LICENSE)
```

### Comparing `ribotricer-1.3.3/ribotricer.egg-info/SOURCES.txt` & `ribotricer-1.4.0/ribotricer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/run_test.sh` & `ribotricer-1.4.0/run_test.sh`

 * *Files identical despite different names*

### Comparing `ribotricer-1.3.3/setup.cfg` & `ribotricer-1.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.3
+current_version = 1.4.0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ribotricer-1.3.3/setup.py` & `ribotricer-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open("README.md") as readme_file:
     readme = readme_file.read()
 with open("requirements.txt") as req_file:
     requirements = req_file.read()
 
 setuptools.setup(
     name="ribotricer",
-    version="1.3.3",
+    version="1.4.0",
     author="Saket Choudhary, Wenzheng Li",
     author_email="saketkc@gmail.com",
     maintainer="Saket Choudhary",
     maintainer_email="saketkc@gmail.com",
     description="Python package to detect translating ORFs from Ribo-seq data",
     license="GPLv3",
     long_description=readme,
@@ -44,11 +44,14 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Utilities",
     ],
 )
```

