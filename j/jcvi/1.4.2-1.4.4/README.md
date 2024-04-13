# Comparing `tmp/jcvi-1.4.2.tar.gz` & `tmp/jcvi-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.4.2.tar", last modified: Fri Mar  1 06:50:26 2024, max compression
+gzip compressed data, was "jcvi-1.4.4.tar", last modified: Sat Apr 13 02:04:57 2024, max compression
```

## Comparing `jcvi-1.4.2.tar` & `jcvi-1.4.4.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.997631 jcvi-1.4.2/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.2/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.2/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     9485 2024-03-01 06:50:26.997455 jcvi-1.4.2/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8250 2023-07-25 21:30:23.000000 jcvi-1.4.2/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.962449 jcvi-1.4.2/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.4.2/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.965337 jcvi-1.4.2/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/algorithms/maxsum.py
--rw-r--r--   0 bao        (501) staff       (20)     1203 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/algorithms/ml.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.2/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.967825 jcvi-1.4.2/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.972388 jcvi-1.4.2/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.4.2/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    68211 2024-03-01 06:44:50.000000 jcvi-1.4.2/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.4.2/jcvi/apps/grid.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/ks.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/apps/script.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.975956 jcvi-1.4.2/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.2/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.4.2/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.4.2/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.977736 jcvi-1.4.2/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.2/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    28049 2023-09-27 02:58:13.000000 jcvi-1.4.2/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.983225 jcvi-1.4.2/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63559 2023-12-20 05:50:50.000000 jcvi-1.4.2/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33830 2023-09-28 09:59:53.000000 jcvi-1.4.2/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    75058 2023-11-24 03:51:46.000000 jcvi-1.4.2/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.2/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.2/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   120171 2023-11-24 03:51:46.000000 jcvi-1.4.2/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.2/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.2/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.987777 jcvi-1.4.2/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    21857 2023-11-24 05:06:52.000000 jcvi-1.4.2/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22275 2023-11-24 05:06:52.000000 jcvi-1.4.2/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.2/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/grabseeds.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/graph.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.2/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.4.2/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/logo.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22507 2024-02-08 05:51:57.000000 jcvi-1.4.2/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.2/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/wheel.py
--rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.4.2/jcvi/graphics/whisker.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.990978 jcvi-1.4.2/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/alfalfa.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/heterosis.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.2/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/pistachio.py
--rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.4.2/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.993042 jcvi-1.4.2/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.2/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.995455 jcvi-1.4.2/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.2/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.2/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.2/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.997122 jcvi-1.4.2/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/tassel.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.963389 jcvi-1.4.2/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     9485 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4727 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.2/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      215 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.2/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1235 2024-03-01 06:50:26.998004 jcvi-1.4.2/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.2/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.191548 jcvi-1.4.4/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.4/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.4/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-13 02:04:57.191640 jcvi-1.4.4/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8250 2023-07-25 21:30:23.000000 jcvi-1.4.4/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.148704 jcvi-1.4.4/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.4.4/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.151765 jcvi-1.4.4/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.4/jcvi/algorithms/maxsum.py
+-rw-r--r--   0 bao        (501) staff       (20)     1203 2023-11-24 05:16:26.000000 jcvi-1.4.4/jcvi/algorithms/ml.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.4/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.154067 jcvi-1.4.4/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/annotation/train.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.159649 jcvi-1.4.4/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    20587 2024-04-12 01:41:38.000000 jcvi-1.4.4/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    68211 2024-03-01 06:44:50.000000 jcvi-1.4.4/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.4/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.4.4/jcvi/apps/grid.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/ks.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)     7525 2024-04-13 02:00:43.000000 jcvi-1.4.4/jcvi/apps/pedigree.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/apps/script.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.165105 jcvi-1.4.4/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    34986 2023-11-24 05:16:26.000000 jcvi-1.4.4/jcvi/assembly/ca.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.4/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.4.4/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.4.4/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/assembly/syntenypath.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/assembly/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.167783 jcvi-1.4.4/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.4/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    28757 2024-04-12 01:41:38.000000 jcvi-1.4.4/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.175243 jcvi-1.4.4/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63559 2023-12-20 05:50:50.000000 jcvi-1.4.4/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33830 2023-09-28 09:59:53.000000 jcvi-1.4.4/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    75058 2023-11-24 03:51:46.000000 jcvi-1.4.4/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.4/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.4/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   120223 2024-04-05 14:11:25.000000 jcvi-1.4.4/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.4/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.4/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.4/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.180705 jcvi-1.4.4/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    21857 2023-11-24 05:06:52.000000 jcvi-1.4.4/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22275 2023-11-24 05:06:52.000000 jcvi-1.4.4/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.4/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/grabseeds.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/graphics/graph.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.4/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.4.4/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/graphics/logo.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22507 2024-02-08 05:51:57.000000 jcvi-1.4.4/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.4/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.4/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/graphics/wheel.py
+-rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.4.4/jcvi/graphics/whisker.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.184523 jcvi-1.4.4/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/alfalfa.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/heterosis.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.4/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/pistachio.py
+-rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.4.4/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.4.4/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.187531 jcvi-1.4.4/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.4/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.189837 jcvi-1.4.4/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.4/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.4/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.4/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.191407 jcvi-1.4.4/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.4/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.4/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.4.4/jcvi/variation/tassel.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-13 02:04:57.149549 jcvi-1.4.4/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4749 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.4/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      215 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2024-04-13 02:04:57.000000 jcvi-1.4.4/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.4/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1235 2024-04-13 02:04:57.191999 jcvi-1.4.4/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.4/setup.py
```

### Comparing `jcvi-1.4.2/LICENSE` & `jcvi-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/PKG-INFO` & `jcvi-1.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,24 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.2
+Version: 1.4.4
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: CrossMap
-Requires-Dist: PyPDF2
-Requires-Dist: biopython
-Requires-Dist: boto3
-Requires-Dist: brewer2mpl
-Requires-Dist: deap
-Requires-Dist: ete3
-Requires-Dist: ftpretty
-Requires-Dist: gffutils
-Requires-Dist: goatools
-Requires-Dist: genomepy
-Requires-Dist: graphviz
-Requires-Dist: jinja2
-Requires-Dist: matplotlib
-Requires-Dist: more-itertools
-Requires-Dist: natsort
-Requires-Dist: networkx
-Requires-Dist: numpy
-Requires-Dist: ortools
-Requires-Dist: pybedtools
-Requires-Dist: rich
-Requires-Dist: scikit-image
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: webcolors
 
 # JCVI utility libraries
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.31631.svg)](https://doi.org/10.5281/zenodo.594205)
 [![Latest PyPI version](https://img.shields.io/pypi/v/jcvi.svg)](https://pypi.python.org/pypi/jcvi)
 [![bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/jcvi/README.html?highlight=jcvi)
 [![Github Actions](https://github.com/tanghaibao/jcvi/workflows/build/badge.svg)](https://github.com/tanghaibao/jcvi/actions)
@@ -246,7 +222,9 @@
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
 
 ## Star History
 
 [![Star History
 Chart](https://api.star-history.com/svg?repos=tanghaibao/jcvi&type=Date)](https://star-history.com/#tanghaibao/jcvi&Date)
+
+
```

### Comparing `jcvi-1.4.2/README.md` & `jcvi-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/__init__.py` & `jcvi-1.4.4/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/ec.py` & `jcvi-1.4.4/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/formula.py` & `jcvi-1.4.4/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/graph.py` & `jcvi-1.4.4/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/lis.py` & `jcvi-1.4.4/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/lpsolve.py` & `jcvi-1.4.4/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/matrix.py` & `jcvi-1.4.4/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/maxsum.py` & `jcvi-1.4.4/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/ml.py` & `jcvi-1.4.4/jcvi/algorithms/ml.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/supermap.py` & `jcvi-1.4.4/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/tsp.py` & `jcvi-1.4.4/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/ahrd.py` & `jcvi-1.4.4/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/automaton.py` & `jcvi-1.4.4/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/depth.py` & `jcvi-1.4.4/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/evm.py` & `jcvi-1.4.4/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/maker.py` & `jcvi-1.4.4/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/pasa.py` & `jcvi-1.4.4/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/qc.py` & `jcvi-1.4.4/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/reformat.py` & `jcvi-1.4.4/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/stats.py` & `jcvi-1.4.4/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/train.py` & `jcvi-1.4.4/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/align.py` & `jcvi-1.4.4/jcvi/apps/align.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 def run_formatdb(infile=None, outfile=None, dbtype="nucl"):
     cmd = "makeblastdb"
     cmd += " -dbtype {0} -in {1}".format(dbtype, infile)
     sh(cmd)
 
 
 @depends
+def run_diamond_makedb(infile=None, outfile=None):
+    cmd = "diamond makedb"
+    cmd += " --in {0} --db {1} -p 5".format(infile, infile)
+    sh(cmd)
+
+
+@depends
 def run_blat(
     infile=None,
     outfile=None,
     db="UniVec_Core",
     pctid=95,
     hitlen=50,
     cpus=16,
@@ -582,9 +589,130 @@
             logging.error(message)
             logging.fatal("Failed to run `lastal`. Aborted.")
             cleanup(lastfile)
             sys.exit(1)
     return lastfile
 
 
+def blast_main(args, dbtype=None):
+    """
+    %prog database.fasta query.fasta
+
+    Run blastp/blastn by calling BLAST+ blastp/blastn depends on dbtype.
+    """
+    p = OptionParser(blast_main.__doc__)
+    p.add_option(
+        "--dbtype",
+        default="nucl",
+        choices=("nucl", "prot"),
+        help="Molecule type of subject database",
+    )
+    p.add_option("--path", help="Specify BLAST path for blastn or blastp")
+
+    p.set_cpus()
+    p.set_outdir()
+    p.set_params()
+
+    opts, args = p.parse_args(args)
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    subject, query = args
+    path = opts.path
+    cpus = opts.cpus
+    if not dbtype:
+        dbtype = opts.dbtype
+
+    getpath = lambda x: op.join(path, x) if path else x
+    cmd = "blastn" if dbtype == "nucl" else "blastp"
+    lastdb_bin = getpath("makeblastdb")
+    lastal_bin = getpath(cmd)
+    for bin in (lastdb_bin, lastal_bin):
+        if not which(bin):
+            logging.fatal("`%s` not found on PATH. Have you installed BLAST?", bin)
+            sys.exit(1)
+
+    db_suffix = '.nin' if dbtype == "nucl" else ".pin"
+
+    run_formatdb(
+        infile=subject,
+        outfile=subject + db_suffix,
+        dbtype=dbtype)
+
+    blastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
+    # Make several attempts to run LASTAL
+    try:
+        sh(
+            cmd + f" -num_threads {cpus} -query {query} -db {subject} -out {blastfile}" +
+            " -outfmt 6 -max_target_seqs 1000 -evalue 1e-5",
+            check=False,
+            redirect_error=STDOUT,
+        )
+    except CalledProcessError as e:  # multi-threading disabled
+        message = f"{cmd} failed with message:"
+        message += "\n{0}".format(e.output.decode())
+        logging.error(message)
+        logging.fatal("Failed to run `blast`. Aborted.")
+        cleanup(blastfile)
+        sys.exit(1)
+    return blastfile
+
+
+def diamond_blastp_main(args, dbtype="prot"):
+    """
+    %prog database.fasta query.fasta
+
+    Run diamond blastp for protein alignment.
+    """
+    p = OptionParser(diamond_blastp_main.__doc__)
+
+    p.add_option("--path", help="Specify diamond path for diamond blastp")
+
+    p.set_cpus()
+    p.set_outdir()
+    p.set_params()
+
+    opts, args = p.parse_args(args)
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    subject, query = args
+    path = opts.path
+    cpus = opts.cpus
+    if not dbtype:
+        dbtype = opts.dbtype
+
+    getpath = lambda x: op.join(path, x) if path else x
+    cmd = "diamond blastp"
+    diamond_bin = getpath("diamond")
+    for bin in (diamond_bin,):
+        if not which(bin):
+            logging.fatal("`%s` not found on PATH. Have you installed Diamond?", bin)
+            sys.exit(1)
+
+    run_diamond_makedb(
+        infile=subject,
+        outfile=subject + '.dmnd',)
+
+    blastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
+    # Make several attempts to run LASTAL
+    try:
+        sh(
+            cmd + f" --threads {cpus} --query {query} --db {subject} --out {blastfile}" +
+            " --ultra-sensitive --max-target-seqs 1000 --evalue 1e-5 --outfmt 6",
+            check=False,
+            redirect_error=STDOUT,
+        )
+    except CalledProcessError as e:  # multi-threading disabled
+        message = f"{cmd} failed with message:"
+        message += "\n{0}".format(e.output.decode())
+        logging.error(message)
+        logging.fatal("Failed to run `diamond blastp`. Aborted.")
+        cleanup(blastfile)
+        sys.exit(1)
+    return blastfile
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.2/jcvi/apps/base.py` & `jcvi-1.4.4/jcvi/apps/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/biomart.py` & `jcvi-1.4.4/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/blastplus.py` & `jcvi-1.4.4/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/bowtie.py` & `jcvi-1.4.4/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/bwa.py` & `jcvi-1.4.4/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/cdhit.py` & `jcvi-1.4.4/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/emboss.py` & `jcvi-1.4.4/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/fetch.py` & `jcvi-1.4.4/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/gbsubmit.py` & `jcvi-1.4.4/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/gmap.py` & `jcvi-1.4.4/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/grid.py` & `jcvi-1.4.4/jcvi/apps/grid.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/ks.py` & `jcvi-1.4.4/jcvi/apps/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/lastz.py` & `jcvi-1.4.4/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/mask.py` & `jcvi-1.4.4/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/phylo.py` & `jcvi-1.4.4/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/r.py` & `jcvi-1.4.4/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/restriction.py` & `jcvi-1.4.4/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/script.py` & `jcvi-1.4.4/jcvi/apps/script.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/softlink.py` & `jcvi-1.4.4/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/uclust.py` & `jcvi-1.4.4/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/uniprot.py` & `jcvi-1.4.4/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/vecscreen.py` & `jcvi-1.4.4/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/allmaps.py` & `jcvi-1.4.4/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/allpaths.py` & `jcvi-1.4.4/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/automaton.py` & `jcvi-1.4.4/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/base.py` & `jcvi-1.4.4/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/ca.py` & `jcvi-1.4.4/jcvi/assembly/ca.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/chic.pyx` & `jcvi-1.4.4/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/coverage.py` & `jcvi-1.4.4/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/gaps.py` & `jcvi-1.4.4/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/geneticmap.py` & `jcvi-1.4.4/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/goldenpath.py` & `jcvi-1.4.4/jcvi/assembly/goldenpath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/hic.py` & `jcvi-1.4.4/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/kmer.py` & `jcvi-1.4.4/jcvi/assembly/kmer.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/opticalmap.py` & `jcvi-1.4.4/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/patch.py` & `jcvi-1.4.4/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/postprocess.py` & `jcvi-1.4.4/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/preprocess.py` & `jcvi-1.4.4/jcvi/assembly/preprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/sim.py` & `jcvi-1.4.4/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/soap.py` & `jcvi-1.4.4/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/syntenypath.py` & `jcvi-1.4.4/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/trinity.py` & `jcvi-1.4.4/jcvi/assembly/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/base.py` & `jcvi-1.4.4/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/blastfilter.py` & `jcvi-1.4.4/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/catalog.py` & `jcvi-1.4.4/jcvi/compara/catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -605,26 +605,28 @@
     The pipeline runs LAST and generate .lifted.anchors.
 
     `--full` mode would assume 1-to-1 quota synteny blocks as the backbone of
     such predictions. Extra orthologs will be recruited from reciprocal best
     match (RBH).
     """
     from jcvi.apps.align import last as last_main
+    from jcvi.apps.align import diamond_blastp_main, blast_main
     from jcvi.compara.blastfilter import main as blastfilter_main
     from jcvi.compara.quota import main as quota_main
     from jcvi.compara.synteny import scan, mcscan, liftover
     from jcvi.formats.blast import cscore, filter, filtered_blastfile_name
 
     p = OptionParser(ortholog.__doc__)
     p.add_option(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
+
     p.add_option(
         "--full",
         default=False,
         action="store_true",
         help="Run in full 1x1 mode, including blocks and RBH",
     )
     p.add_option("--cscore", default=0.7, type="float", help="C-score cutoff")
@@ -669,14 +671,21 @@
     p.add_option(
         "--ignore_zero_anchor",
         default=False,
         action="store_true",
         help="Ignore this pair of ortholog identification instead of throwing an error when performing many pairs of cataloging."
     )
 
+    p.add_option(
+        "--align_soft",
+        default="last",
+        choices=("last", "blast", "diamond_blastp"),
+        help="Sequence alignment software. Default <last> for both <nucl> and <prot>. Users could also use <blast> for both <nucl> and <prot>, or <diamond_blastp> for <prot>.",
+    )
+
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     a, b = args
     dbtype = opts.dbtype
@@ -686,22 +695,32 @@
     bbed, bfasta = b + ".bed", b + suffix
     ccscore = opts.cscore
     quota = opts.quota
     exclude = opts.exclude
     dist = "--dist={0}".format(opts.dist)
     minsize_flag = "--min_size={}".format(opts.n)
     cpus_flag = "--cpus={}".format(opts.cpus)
+    align_soft = opts.align_soft
 
     aprefix = op.basename(a)
     bprefix = op.basename(b)
     pprefix = ".".join((aprefix, bprefix))
     qprefix = ".".join((bprefix, aprefix))
     last = pprefix + ".last"
     if need_update((afasta, bfasta), last, warn=True):
-        last_main([bfasta, afasta, cpus_flag], dbtype)
+        if align_soft == "blast":
+            blast_main(
+                [bfasta, afasta, cpus_flag], dbtype
+            )
+        elif dbtype == "prot" and align_soft == "diamond_blastp":
+            diamond_blastp_main(
+                [bfasta, afasta, cpus_flag], dbtype
+            )
+        else:
+            last_main([bfasta, afasta, cpus_flag], dbtype)
 
     self_remove = opts.self_remove
     if a == b:
         lastself = filtered_blastfile_name(last, self_remove, 0, inverse=True)
         if need_update(last, lastself, warn=True):
             filter(
                 [last, "--hitlen=0", f"--pctid={self_remove}", "--inverse", "--noself"]
```

### Comparing `jcvi-1.4.2/jcvi/compara/fractionation.py` & `jcvi-1.4.4/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/pad.py` & `jcvi-1.4.4/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/phylogeny.py` & `jcvi-1.4.4/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/quota.py` & `jcvi-1.4.4/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/reconstruct.py` & `jcvi-1.4.4/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/synfind.py` & `jcvi-1.4.4/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/synteny.py` & `jcvi-1.4.4/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/agp.py` & `jcvi-1.4.4/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/base.py` & `jcvi-1.4.4/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/bed.py` & `jcvi-1.4.4/jcvi/formats/bed.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/blast.py` & `jcvi-1.4.4/jcvi/formats/blast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/cblast.pyx` & `jcvi-1.4.4/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/cdt.py` & `jcvi-1.4.4/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/chain.py` & `jcvi-1.4.4/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/contig.py` & `jcvi-1.4.4/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/coords.py` & `jcvi-1.4.4/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/excel.py` & `jcvi-1.4.4/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/fasta.py` & `jcvi-1.4.4/jcvi/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/fastq.py` & `jcvi-1.4.4/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/genbank.py` & `jcvi-1.4.4/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/gff.py` & `jcvi-1.4.4/jcvi/formats/gff.py`

 * *Files 0% similar despite different names*

```diff
@@ -3052,15 +3052,14 @@
     ensembl_cds = opts.ensembl_cds
     if opts.type:
         type = set(x.strip() for x in opts.type.split(","))
     if opts.source:
         source = set(x.strip() for x in opts.source.split(","))
     if ensembl_cds:
         type = {"CDS"}
-        source = {"protein_coding"}
 
     gff = Gff(
         gffile,
         key=key,
         parent_key=parent_key,
         append_source=opts.append_source,
         append_ftype=opts.append_ftype,
@@ -3091,14 +3090,16 @@
         if span:
             bl.score = bl.span
         if human_chr:
             if bl.seqid not in VALID_HUMAN_CHROMOSMES:
                 continue
             bl.seqid = "chr" + bl.seqid
         if ensembl_cds:
+            if g.get_attr("gene_biotype") != "protein_coding":
+                continue
             bl.accn = "{0}.{1}".format(
                 g.get_attr("transcript_name"), g.get_attr("exon_number")
             )
             position = (bl.seqid, bl.start, bl.end)
             if position in seen:
                 skipped_identical_range += 1
                 continue
```

### Comparing `jcvi-1.4.2/jcvi/formats/html.py` & `jcvi-1.4.4/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/maf.py` & `jcvi-1.4.4/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/obo.py` & `jcvi-1.4.4/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/paf.py` & `jcvi-1.4.4/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/pdf.py` & `jcvi-1.4.4/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/psl.py` & `jcvi-1.4.4/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/pyblast.py` & `jcvi-1.4.4/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/sam.py` & `jcvi-1.4.4/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/sizes.py` & `jcvi-1.4.4/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/vcf.py` & `jcvi-1.4.4/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/align.py` & `jcvi-1.4.4/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/assembly.py` & `jcvi-1.4.4/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/base.py` & `jcvi-1.4.4/jcvi/graphics/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/blastplot.py` & `jcvi-1.4.4/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/chromosome.py` & `jcvi-1.4.4/jcvi/graphics/chromosome.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/coverage.py` & `jcvi-1.4.4/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/dotplot.py` & `jcvi-1.4.4/jcvi/graphics/dotplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/glyph.py` & `jcvi-1.4.4/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/grabseeds.py` & `jcvi-1.4.4/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/graph.py` & `jcvi-1.4.4/jcvi/graphics/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/heatmap.py` & `jcvi-1.4.4/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/histogram.py` & `jcvi-1.4.4/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/karyotype.py` & `jcvi-1.4.4/jcvi/graphics/karyotype.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/landscape.py` & `jcvi-1.4.4/jcvi/graphics/landscape.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/logo.py` & `jcvi-1.4.4/jcvi/graphics/logo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/mummerplot.py` & `jcvi-1.4.4/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/synteny.py` & `jcvi-1.4.4/jcvi/graphics/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/table.py` & `jcvi-1.4.4/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/tree.py` & `jcvi-1.4.4/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/wheel.py` & `jcvi-1.4.4/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/whisker.py` & `jcvi-1.4.4/jcvi/graphics/whisker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/age.py` & `jcvi-1.4.4/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/alfalfa.py` & `jcvi-1.4.4/jcvi/projects/alfalfa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/allmaps.py` & `jcvi-1.4.4/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/bites.py` & `jcvi-1.4.4/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/heterosis.py` & `jcvi-1.4.4/jcvi/projects/heterosis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/ies.py` & `jcvi-1.4.4/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/misc.py` & `jcvi-1.4.4/jcvi/projects/misc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/napus.py` & `jcvi-1.4.4/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/pineapple.py` & `jcvi-1.4.4/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/pistachio.py` & `jcvi-1.4.4/jcvi/projects/pistachio.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/str.py` & `jcvi-1.4.4/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/sugarcane.py` & `jcvi-1.4.4/jcvi/projects/sugarcane.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/synfind.py` & `jcvi-1.4.4/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/tgbs.py` & `jcvi-1.4.4/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/vanilla.py` & `jcvi-1.4.4/jcvi/projects/vanilla.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/aws.py` & `jcvi-1.4.4/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/cbook.py` & `jcvi-1.4.4/jcvi/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/Airswing.ttf` & `jcvi-1.4.4/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/Collegia.ttf` & `jcvi-1.4.4/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.4.4/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.4.4/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.4.4/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/adapters.fasta` & `jcvi-1.4.4/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/blosum80.mat` & `jcvi-1.4.4/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.4.4/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/hg38.band.txt` & `jcvi-1.4.4/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.4.4/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/instance.json` & `jcvi-1.4.4/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/db.py` & `jcvi-1.4.4/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/ez_setup.py` & `jcvi-1.4.4/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/grouper.py` & `jcvi-1.4.4/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/orderedcollections.py` & `jcvi-1.4.4/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/range.py` & `jcvi-1.4.4/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/table.py` & `jcvi-1.4.4/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/taxonomy.py` & `jcvi-1.4.4/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/validator.py` & `jcvi-1.4.4/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/webcolors.py` & `jcvi-1.4.4/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/cnv.py` & `jcvi-1.4.4/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/deconvolute.py` & `jcvi-1.4.4/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/delly.py` & `jcvi-1.4.4/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/impute.py` & `jcvi-1.4.4/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/phase.py` & `jcvi-1.4.4/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/snp.py` & `jcvi-1.4.4/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/str.py` & `jcvi-1.4.4/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/tassel.py` & `jcvi-1.4.4/jcvi/variation/tassel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi.egg-info/PKG-INFO` & `jcvi-1.4.4/jcvi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,24 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.2
+Version: 1.4.4
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: CrossMap
-Requires-Dist: PyPDF2
-Requires-Dist: biopython
-Requires-Dist: boto3
-Requires-Dist: brewer2mpl
-Requires-Dist: deap
-Requires-Dist: ete3
-Requires-Dist: ftpretty
-Requires-Dist: gffutils
-Requires-Dist: goatools
-Requires-Dist: genomepy
-Requires-Dist: graphviz
-Requires-Dist: jinja2
-Requires-Dist: matplotlib
-Requires-Dist: more-itertools
-Requires-Dist: natsort
-Requires-Dist: networkx
-Requires-Dist: numpy
-Requires-Dist: ortools
-Requires-Dist: pybedtools
-Requires-Dist: rich
-Requires-Dist: scikit-image
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: webcolors
 
 # JCVI utility libraries
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.31631.svg)](https://doi.org/10.5281/zenodo.594205)
 [![Latest PyPI version](https://img.shields.io/pypi/v/jcvi.svg)](https://pypi.python.org/pypi/jcvi)
 [![bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/jcvi/README.html?highlight=jcvi)
 [![Github Actions](https://github.com/tanghaibao/jcvi/workflows/build/badge.svg)](https://github.com/tanghaibao/jcvi/actions)
@@ -246,7 +222,9 @@
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
 
 ## Star History
 
 [![Star History
 Chart](https://api.star-history.com/svg?repos=tanghaibao/jcvi&type=Date)](https://star-history.com/#tanghaibao/jcvi&Date)
+
+
```

### Comparing `jcvi-1.4.2/jcvi.egg-info/SOURCES.txt` & `jcvi-1.4.4/jcvi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 jcvi/apps/fetch.py
 jcvi/apps/gbsubmit.py
 jcvi/apps/gmap.py
 jcvi/apps/grid.py
 jcvi/apps/ks.py
 jcvi/apps/lastz.py
 jcvi/apps/mask.py
+jcvi/apps/pedigree.py
 jcvi/apps/phylo.py
 jcvi/apps/r.py
 jcvi/apps/restriction.py
 jcvi/apps/script.py
 jcvi/apps/softlink.py
 jcvi/apps/uclust.py
 jcvi/apps/uniprot.py
```

### Comparing `jcvi-1.4.2/setup.cfg` & `jcvi-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/setup.py` & `jcvi-1.4.4/setup.py`

 * *Files identical despite different names*

