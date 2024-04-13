# Comparing `tmp/mngs-1.2.3.tar.gz` & `tmp/mngs-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-1.2.3.tar", last modified: Mon Apr  8 15:28:46 2024, max compression
+gzip compressed data, was "mngs-1.3.0.tar", last modified: Fri Apr 12 16:59:36 2024, max compression
```

## Comparing `mngs-1.2.3.tar` & `mngs-1.3.0.tar`

### file list

```diff
@@ -1,226 +1,234 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:30:42.000000 mngs-1.2.3/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.3/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1887 2024-04-08 15:28:46.887353 mngs-1.2.3/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.3/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-08 15:28:46.887353 mngs-1.2.3/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.3/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.859353 mngs-1.2.3/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.860353 mngs-1.2.3/src/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      586 2024-04-08 02:29:53.000000 mngs-1.2.3/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.862353 mngs-1.2.3/src/mngs/dsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.3/src/mngs/dsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      435 2024-04-08 01:51:33.000000 mngs-1.2.3/src/mngs/dsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6008 2024-04-08 00:35:43.000000 mngs-1.2.3/src/mngs/dsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.3/src/mngs/dsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.2.3/src/mngs/dsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.3/src/mngs/dsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3483 2024-04-07 23:40:24.000000 mngs-1.2.3/src/mngs/dsp/_modulation_index.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5874 2024-04-08 02:24:40.000000 mngs-1.2.3/src/mngs/dsp/_pac.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.3/src/mngs/dsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1672 2024-04-04 21:38:57.000000 mngs-1.2.3/src/mngs/dsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1663 2024-04-08 02:41:59.000000 mngs-1.2.3/src/mngs/dsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.3/src/mngs/dsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2755 2024-04-05 03:19:19.000000 mngs-1.2.3/src/mngs/dsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6150 2024-04-05 14:36:19.000000 mngs-1.2.3/src/mngs/dsp/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1909 2024-04-04 10:07:16.000000 mngs-1.2.3/src/mngs/dsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.862353 mngs-1.2.3/src/mngs/dsp/fx/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       95 2024-04-05 06:28:18.000000 mngs-1.2.3/src/mngs/dsp/fx/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.863353 mngs-1.2.3/src/mngs/dsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.3/src/mngs/dsp/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7199 2024-04-07 17:06:51.000000 mngs-1.2.3/src/mngs/dsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.3/src/mngs/dsp/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 mngs-1.2.3/src/mngs/dsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-08 00:30:03.000000 mngs-1.2.3/src/mngs/dsp/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9591 2024-04-08 02:28:29.000000 mngs-1.2.3/src/mngs/dsp/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.2.3/src/mngs/dsp/nn/_PAC_working.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.3/src/mngs/dsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.3/src/mngs/dsp/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.3/src/mngs/dsp/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.3/src/mngs/dsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      962 2024-04-08 01:51:20.000000 mngs-1.2.3/src/mngs/dsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.2.3/src/mngs/dsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.3/src/mngs/dsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.867353 mngs-1.2.3/src/mngs/general/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.2.3/src/mngs/general/_TimeStamper.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1520 2024-04-07 09:17:14.000000 mngs-1.2.3/src/mngs/general/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.3/src/mngs/general/_close.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-07 10:54:07.000000 mngs-1.2.3/src/mngs/general/_converters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_cuda_collect_env.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.3/src/mngs/general/_norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2061 2024-04-07 09:16:08.000000 mngs-1.2.3/src/mngs/general/_reload.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_shell.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.3/src/mngs/general/_start.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_xml2dict.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/email.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/latex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9812 2024-04-05 21:59:08.000000 mngs-1.2.3/src/mngs/general/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/mat2py.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.3/src/mngs/general/misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/pandas.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.3/src/mngs/general/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.3/src/mngs/general/repro.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.3/src/mngs/general/save.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/torch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.867353 mngs-1.2.3/src/mngs/gists/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/_SigMacro_processFigure_S.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/_SigMacro_toBlue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.868353 mngs-1.2.3/src/mngs/io/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-05 14:24:05.000000 mngs-1.2.3/src/mngs/io/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9812 2024-04-05 21:59:08.000000 mngs-1.2.3/src/mngs/io/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.3/src/mngs/io/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.3/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.868353 mngs-1.2.3/src/mngs/linalg/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/linalg/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/linalg/_misc.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.869353 mngs-1.2.3/src/mngs/ml/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/ClassificationReporter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/ClassifierServer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.3/src/mngs/ml/EarlyStopping.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/LearningCurveLogger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/__Classifiers.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.3/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.870353 mngs-1.2.3/src/mngs/ml/act/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/act/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.870353 mngs-1.2.3/src/mngs/ml/clustering/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.3/src/mngs/ml/clustering/_UMAP.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.3/src/mngs/ml/clustering/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.3/src/mngs/ml/clustering/_umap.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.871353 mngs-1.2.3/src/mngs/ml/layer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/_Pass.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/loss/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/MultiTaskLoss.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/_L1L2Losses.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/metrics/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.3/src/mngs/ml/metrics/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.3/src/mngs/ml/metrics/_bACC.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.874353 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.874353 mngs-1.2.3/src/mngs/ml/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.3/src/mngs/ml/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.3/src/mngs/ml/plt/_conf_mat.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.3/src/mngs/ml/plt/_learning_curve.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.3/src/mngs/ml/plt/_optuna_study.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.875353 mngs-1.2.3/src/mngs/ml/plt/aucs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/roc_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.876353 mngs-1.2.3/src/mngs/ml/sk/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.3/src/mngs/ml/sk/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.3/src/mngs/ml/sk/_clf.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.3/src/mngs/ml/sk/_to_sktime.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.877353 mngs-1.2.3/src/mngs/ml/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_DefaultDataset.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.3/src/mngs/ml/utils/_LabelEncoder.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.3/src/mngs/ml/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.3/src/mngs/ml/utils/_check_params.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.3/src/mngs/ml/utils/_merge_labels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_sliding_window_data_augmentation.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_under_sample.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.878352 mngs-1.2.3/src/mngs/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/mngs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/mngs/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.879353 mngs-1.2.3/src/mngs/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.3/src/mngs/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7199 2024-04-07 17:06:51.000000 mngs-1.2.3/src/mngs/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.3/src/mngs/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 mngs-1.2.3/src/mngs/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-08 00:30:03.000000 mngs-1.2.3/src/mngs/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9591 2024-04-08 02:28:29.000000 mngs-1.2.3/src/mngs/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.2.3/src/mngs/nn/_PAC_working.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.3/src/mngs/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.3/src/mngs/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.3/src/mngs/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.3/src/mngs/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      962 2024-04-08 01:51:20.000000 mngs-1.2.3/src/mngs/nn/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.879353 mngs-1.2.3/src/mngs/os/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.3/src/mngs/os/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1379 2024-04-05 22:00:45.000000 mngs-1.2.3/src/mngs/os/_mv.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.881353 mngs-1.2.3/src/mngs/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.3/src/mngs/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_add_hue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_annotated_heatmap.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-05 06:07:27.000000 mngs-1.2.3/src/mngs/plt/_configure_mpl.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_draw_a_cube.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_get_RGBA_from_colormap.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_mk_colorbar.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_mk_patches.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    14273 2024-04-08 14:14:38.000000 mngs-1.2.3/src/mngs/plt/_subplots.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.3/src/mngs/plt/_tpl.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.883353 mngs-1.2.3/src/mngs/plt/ax/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:34:39.000000 mngs-1.2.3/src/mngs/plt/ax/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_circular_hist.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_extend.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_fill_between.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.3/src/mngs/plt/ax/_hide_spines.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_map_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_panel.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_sci_note.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:15:04.000000 mngs-1.2.3/src/mngs/plt/ax/_set_n_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.3/src/mngs/plt/ax/_set_pos.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_set_size.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      401 2024-04-07 04:39:32.000000 mngs-1.2.3/src/mngs/plt/ax/_set_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/colors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.884353 mngs-1.2.3/src/mngs/resource/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/get.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.886352 mngs-1.2.3/src/mngs/stats/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.3/src/mngs/stats/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_bonferroni_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_brunner_munzel_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_calc_partial_corr.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_corr_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_fdr_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.3/src/mngs/stats/_general.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_multicompair.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_smirnov_grubbs.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_to_asterisks.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/src/mngs/torch/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.3/src/mngs/torch/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.3/src/mngs/torch/_apply_to.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1887 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5824 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:30:42.000000 mngs-1.3.0/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.3.0/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      914 2024-04-12 16:59:36.899178 mngs-1.3.0/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      289 2024-04-12 16:59:09.000000 mngs-1.3.0/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-12 16:59:36.903178 mngs-1.3.0/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.0/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.887178 mngs-1.3.0/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.888178 mngs-1.3.0/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      541 2024-04-12 16:56:31.000000 mngs-1.3.0/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.889178 mngs-1.3.0/src/mngs/dsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.3.0/src/mngs/dsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      476 2024-04-12 06:37:09.000000 mngs-1.3.0/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8264 2024-04-12 15:58:47.000000 mngs-1.3.0/src/mngs/dsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-04-12 16:24:37.000000 mngs-1.3.0/src/mngs/dsp/_hilbert.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2298 2024-04-12 06:33:44.000000 mngs-1.3.0/src/mngs/dsp/_listen.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.3.0/src/mngs/dsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.3.0/src/mngs/dsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1847 2024-04-12 16:39:54.000000 mngs-1.3.0/src/mngs/dsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4134 2024-04-12 16:40:18.000000 mngs-1.3.0/src/mngs/dsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2315 2024-04-12 15:32:38.000000 mngs-1.3.0/src/mngs/dsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1653 2024-04-12 16:35:11.000000 mngs-1.3.0/src/mngs/dsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1663 2024-04-08 02:41:59.000000 mngs-1.3.0/src/mngs/dsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2549 2024-04-12 14:51:36.000000 mngs-1.3.0/src/mngs/dsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2875 2024-04-12 15:18:24.000000 mngs-1.3.0/src/mngs/dsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6150 2024-04-05 14:36:19.000000 mngs-1.3.0/src/mngs/dsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3701 2024-04-12 16:49:23.000000 mngs-1.3.0/src/mngs/dsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.891178 mngs-1.3.0/src/mngs/dsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.0/src/mngs/dsp/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.0/src/mngs/dsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.0/src/mngs/dsp/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.0/src/mngs/dsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.0/src/mngs/dsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.0/src/mngs/dsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.0/src/mngs/dsp/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.0/src/mngs/dsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.0/src/mngs/dsp/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.0/src/mngs/dsp/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.0/src/mngs/dsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.0/src/mngs/dsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.3.0/src/mngs/dsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.3.0/src/mngs/dsp/reference.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      438 2024-04-10 05:57:54.000000 mngs-1.3.0/src/mngs/dsp/template.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.891178 mngs-1.3.0/src/mngs/dsp/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      349 2024-04-12 09:54:43.000000 mngs-1.3.0/src/mngs/dsp/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3338 2024-04-12 10:11:47.000000 mngs-1.3.0/src/mngs/dsp/utils/_differential_bandpass_filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      201 2024-04-10 01:59:50.000000 mngs-1.3.0/src/mngs/dsp/utils/_ensure_even_len.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      548 2024-04-10 22:26:21.000000 mngs-1.3.0/src/mngs/dsp/utils/_zero_pad.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13225 2024-04-12 16:04:54.000000 mngs-1.3.0/src/mngs/dsp/utils/filter.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3212 2024-04-11 11:36:33.000000 mngs-1.3.0/src/mngs/dsp/utils/pac.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.892178 mngs-1.3.0/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.3.0/src/mngs/general/_TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-04-12 00:56:17.000000 mngs-1.3.0/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2255 2024-04-10 09:53:27.000000 mngs-1.3.0/src/mngs/general/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-10 22:17:57.000000 mngs-1.3.0/src/mngs/general/_converters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_cuda_collect_env.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1947 2024-04-12 00:46:27.000000 mngs-1.3.0/src/mngs/general/_embed.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.3.0/src/mngs/general/_norm.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      695 2024-04-12 01:01:58.000000 mngs-1.3.0/src/mngs/general/_paste.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4315 2024-04-10 07:23:22.000000 mngs-1.3.0/src/mngs/general/_reload.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4094 2024-04-10 09:44:58.000000 mngs-1.3.0/src/mngs/general/_reproduce.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4525 2024-04-12 13:27:12.000000 mngs-1.3.0/src/mngs/general/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.0/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22771 2024-04-10 07:34:26.000000 mngs-1.3.0/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.0/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.0/src/mngs/general/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.892178 mngs-1.3.0/src/mngs/gists/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/_SigMacro_processFigure_S.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/_SigMacro_toBlue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      485 2024-04-10 07:36:15.000000 mngs-1.3.0/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.0/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.0/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.0/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.3.0/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/__Classifiers.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.3.0/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/clustering/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.3.0/src/mngs/ml/clustering/_UMAP.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.3.0/src/mngs/ml/clustering/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.3.0/src/mngs/ml/clustering/_umap.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/metrics/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.3.0/src/mngs/ml/metrics/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.3.0/src/mngs/ml/metrics/_bACC.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.3.0/src/mngs/ml/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.3.0/src/mngs/ml/plt/_conf_mat.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.3.0/src/mngs/ml/plt/_learning_curve.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.3.0/src/mngs/ml/plt/_optuna_study.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/sk/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.3.0/src/mngs/ml/sk/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.3.0/src/mngs/ml/sk/_clf.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.3.0/src/mngs/ml/sk/_to_sktime.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_DefaultDataset.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.3.0/src/mngs/ml/utils/_LabelEncoder.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.3.0/src/mngs/ml/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.3.0/src/mngs/ml/utils/_check_params.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.3.0/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_sliding_window_data_augmentation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/mngs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/mngs/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.0/src/mngs/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.0/src/mngs/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.0/src/mngs/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.0/src/mngs/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.0/src/mngs/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.0/src/mngs/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.0/src/mngs/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.0/src/mngs/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.0/src/mngs/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.0/src/mngs/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.0/src/mngs/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.0/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/os/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.3.0/src/mngs/os/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1379 2024-04-05 22:00:45.000000 mngs-1.3.0/src/mngs/os/_mv.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.3.0/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5826 2024-04-10 01:00:32.000000 mngs-1.3.0/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    11703 2024-04-12 14:36:46.000000 mngs-1.3.0/src/mngs/plt/_subplots.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.3.0/src/mngs/plt/_tpl.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.898178 mngs-1.3.0/src/mngs/plt/ax/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:34:39.000000 mngs-1.3.0/src/mngs/plt/ax/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.3.0/src/mngs/plt/ax/_hide_spines.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_map_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_panel.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_sci_note.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:15:04.000000 mngs-1.3.0/src/mngs/plt/ax/_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.3.0/src/mngs/plt/ax/_set_pos.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      401 2024-04-07 04:39:32.000000 mngs-1.3.0/src/mngs/plt/ax/_set_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.898178 mngs-1.3.0/src/mngs/resource/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/get.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.3.0/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.3.0/src/mngs/stats/_general.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/src/mngs/torch/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.3.0/src/mngs/torch/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.3.0/src/mngs/torch/_apply_to.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.888178 mngs-1.3.0/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      914 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6094 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      433 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-1.2.3/LICENSE` & `mngs-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/setup.py` & `mngs-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/PARAMS.py` & `mngs-1.3.0/src/mngs/dsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/_demo_sig.py` & `mngs-1.3.0/src/mngs/dsp/_demo_sig.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,61 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 11:35:43 (ywatanabe)"
+# Time-stamp: "2024-04-13 01:58:46 (ywatanabe)"
 
+
+"""
+This script does XYZ.
+"""
+
+# Imports
 import random
+import sys
 import warnings
 
+import matplotlib.pyplot as plt
 import mne
 import mngs
 import numpy as np
-from mne import Epochs, compute_covariance, find_events, make_ad_hoc_cov
 from mne.datasets import sample
 from mne.simulation import (
     add_ecg,
     add_eog,
     add_noise,
     simulate_raw,
     simulate_sparse_stc,
 )
 from ripple_detection.simulate import simulate_LFP, simulate_time
 from scipy.signal import chirp
 from tensorpac.signals import pac_signals_wavelet
 
+# Config
+CONFIG = mngs.gen.load_configs(verbose=False)
 
-def _demo_sig_tensorpac(
-    batch_size=8,
-    n_chs=19,
-    t_sec=4,
-    fs=512,
-    f_pha=10,
-    f_amp=100,
-    noise=0.8,
-    n_segments=20,
-    verbose=False,
-):
-    n_times = int(t_sec * fs)
-    x_2d, tt = pac_signals_wavelet(
-        sf=fs,
-        f_pha=f_pha,
-        f_amp=f_amp,
-        noise=noise,
-        n_epochs=n_segments,
-        n_times=n_times,
-    )
-    x_3d = np.stack([x_2d for _ in range(batch_size)], axis=0)
-    x_4d = np.stack([x_3d for _ in range(n_chs)], axis=1)
-    return x_4d, tt
-
-
+# Functions
 def demo_sig(
+    sig_type="periodic",
     batch_size=8,
     n_chs=19,
+    n_segments=20,
     t_sec=4,
     fs=512,
     freqs_hz=None,
-    sig_type="periodic",
     verbose=False,
 ):
 
     assert sig_type in [
         "uniform",
         "gauss",
         "periodic",
         "chirp",
         "ripple",
         "meg",
         "tensorpac",
+        "pac",
     ]
     tt = np.linspace(0, t_sec, int(t_sec * fs), endpoint=False)
 
     if sig_type == "uniform":
         return (
             np.random.uniform(
                 low=-0.5, high=0.5, size=(batch_size, n_chs, len(tt))
@@ -93,14 +80,25 @@
             fs,
         )
 
     elif sig_type == "tensorpac":
         xx, tt = _demo_sig_tensorpac(
             batch_size=batch_size,
             n_chs=n_chs,
+            n_segments=n_segments,
+            t_sec=t_sec,
+            fs=fs,
+        )
+        return xx.astype(np.float32)[..., : len(tt)], tt, fs
+
+    elif sig_type == "pac":
+        xx = _demo_sig_pac(
+            batch_size=batch_size,
+            n_chs=n_chs,
+            n_segments=n_segments,
             t_sec=t_sec,
             fs=fs,
         )
         return xx.astype(np.float32)[..., : len(tt)], tt, fs
 
     else:
         fn_1d = {
@@ -126,14 +124,91 @@
                 .astype(np.float32)[..., : len(tt)]
             ),
             tt,
             fs,
         )
 
 
+def _demo_sig_pac(
+    batch_size=8,
+    n_chs=19,
+    t_sec=4,
+    fs=512,
+    f_pha=10,
+    f_amp=100,
+    noise=0.8,
+    n_segments=20,
+    verbose=False,
+):
+    """
+    Generate a demo signal with phase-amplitude coupling.
+
+    Parameters:
+        batch_size (int): Number of batches.
+        n_chs (int): Number of channels.
+        t_sec (int): Duration of the signal in seconds.
+        fs (int): Sampling frequency.
+        f_pha (float): Frequency of the phase-modulating signal.
+        f_amp (float): Frequency of the amplitude-modulated signal.
+        noise (float): Noise level added to the signal.
+        n_segments (int): Number of segments.
+        verbose (bool): If True, print additional information.
+
+    Returns:
+        np.array: Generated signals with shape (batch_size, n_chs, n_segments, seq_len).
+    """
+    seq_len = t_sec * fs
+    t = np.arange(seq_len) / fs
+    if verbose:
+        print(f"Generating signal with length: {seq_len}")
+
+    # Create empty array to store the signals
+    signals = np.zeros((batch_size, n_chs, n_segments, seq_len))
+
+    for b in range(batch_size):
+        for ch in range(n_chs):
+            for seg in range(n_segments):
+                # Phase signal
+                theta = np.sin(2 * np.pi * f_pha * t)
+                # Amplitude envelope
+                amplitude_env = 1 + np.sin(2 * np.pi * f_amp * t)
+                # Combine phase and amplitude modulation
+                signal = theta * amplitude_env
+                # Add Gaussian noise
+                signal += noise * np.random.randn(seq_len)
+                signals[b, ch, seg, :] = signal
+
+    return signals
+
+
+def _demo_sig_tensorpac(
+    batch_size=8,
+    n_chs=19,
+    t_sec=4,
+    fs=512,
+    f_pha=10,
+    f_amp=100,
+    noise=0.8,
+    n_segments=20,
+    verbose=False,
+):
+    n_times = int(t_sec * fs)
+    x_2d, tt = pac_signals_wavelet(
+        sf=fs,
+        f_pha=f_pha,
+        f_amp=f_amp,
+        noise=noise,
+        n_epochs=n_segments,
+        n_times=n_times,
+    )
+    x_3d = np.stack([x_2d for _ in range(batch_size)], axis=0)
+    x_4d = np.stack([x_3d for _ in range(n_chs)], axis=1)
+    return x_4d, tt
+
+
 def _demo_sig_meg(
     batch_size=8, n_chs=19, t_sec=10, fs=512, verbose=False, **kwargs
 ):
     data_path = sample.data_path()
     meg_path = data_path / "MEG" / "sample"
     raw_fname = meg_path / "sample_audvis_raw.fif"
     fwd_fname = meg_path / "sample_audvis-meg-eeg-oct-6-fwd.fif"
@@ -198,27 +273,43 @@
     t = simulate_time(n_samples, fs)
     n_ripples = random.randint(1, 5)
     mid_time = np.random.permutation(t)[:n_ripples]
     return simulate_LFP(t, mid_time, noise_amplitude=1.2, ripple_amplitude=5)
 
 
 if __name__ == "__main__":
-    uu, tt, fs = demo_sig(sig_type="uniform")
-    gg, tt, fs = demo_sig(sig_type="gauss")
-    mm, tt, fs = demo_sig(sig_type="meg")
-    pp, tt, fs = demo_sig(sig_type="periodic")
-    cc, tt, fs = demo_sig(sig_type="chirp")
-    rr, tt, fs = demo_sig(sig_type="ripple")
-    tp, tt, fs = demo_sig(sig_type="tensorpac")
-
-    fig, axes = mngs.plt.subplots(nrows=7)
-    axes[0].plot(uu[0, 0], label="uniform")
-    axes[1].plot(gg[0, 0], label="gauss")
-    axes[2].plot(mm[0, 0], label="meg")
-    axes[3].plot(pp[0, 0], label="periodic")
-    axes[4].plot(cc[0, 0], label="chirp")
-    axes[5].plot(rr[0, 0], label="ripple")
-    axes[6].plot(tp[0, 0, 0], label="tensorpac")
-    for ax in axes:
-        ax.legend(loc="upper right")
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
+
+    SIG_TYPES = [
+        "uniform",
+        "gauss",
+        "periodic",
+        "chirp",
+        "meg",
+        "ripple",
+        "tensorpac",
+        "pac",
+    ]
 
-    plt.show()
+    i_batch, i_ch, i_segment = 0, 0, 0
+    fig, axes = mngs.plt.subplots(nrows=len(SIG_TYPES))
+    for ax, (i_sig_type, sig_type) in zip(axes, enumerate(SIG_TYPES)):
+        xx, tt, fs = demo_sig(sig_type=sig_type)
+        if sig_type not in ["tensorpac", "pac"]:
+            ax.plot(tt, xx[i_batch, i_ch], label=sig_type)
+        else:
+            ax.plot(tt, xx[i_batch, i_ch, i_segment], label=sig_type)
+        ax.legend(loc="upper left")
+    fig.suptitle("Demo signals")
+    fig.supxlabel("Time [s]")
+    fig.supylabel("Amplitude [?V]")
+    mngs.io.save(fig, "traces.png")
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
+
+"""
+/home/ywatanabe/proj/entrance/mngs/dsp/_demo_sig.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/dsp/_misc.py` & `mngs-1.3.0/src/mngs/dsp/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/_mne.py` & `mngs-1.3.0/src/mngs/dsp/_mne.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/_modulation_index.py` & `mngs-1.3.0/src/mngs/dsp/utils/pac.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,135 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 10:40:23 (ywatanabe)"
-
-import torch
-from mngs.general import torch_fn
-from mngs.nn import ModulationIndex
-
-
-@torch_fn
-def modulation_index(pha, amp, n_bins=18):
-    """
-    pha: (batch_size, n_chs, n_freqs_pha, n_segments, seq_len)
-    amp: (batch_size, n_chs, n_freqs_amp, n_segments, seq_len)
-    """
-    return ModulationIndex(n_bins=n_bins)(pha, amp)
-
-
-def plot_comodulogram_tensorpac(xx, fs, t_sec, ts=None):
-    import tensorpac
-    from tensorpac import Pac
+"""
+This script does XYZ.
+"""
 
+# Imports
+import sys
+
+import matplotlib.pyplot as plt
+import mngs
+import numpy as np
+import tensorpac
+
+
+# Functions
+def calc_pac_with_tensorpac(xx, fs, t_sec, i_batch=0, i_ch=0):
     # Morlet's Wavelet Transfrmation
-    p = tensorpac.Pac(f_pha="hres", f_amp="hres", dcomplex="wavelet")
+    p = tensorpac.Pac(f_pha="hres", f_amp="mres", dcomplex="wavelet")
 
     # Bandpass Filtering and Hilbert Transformation
-    i_batch, i_ch = 0, 0
-    ts("Bandpassfiltering and Hilbert Transformation with Tensorpac starts.")
     phases = p.filter(
         fs, xx[i_batch, i_ch], ftype="phase", n_jobs=1
     )  # (50, 20, 2048)
     amplitudes = p.filter(
         fs, xx[i_batch, i_ch], ftype="amplitude", n_jobs=1
     )  # (50, 20, 2048)
-    ts("Bandpassfiltering and Hilbert Transformation with Tensorpac ends.")
 
     # Calculates xpac
     k = 2
     p.idpac = (k, 0, 0)
-    ts("PAC Calculation with Tensorpac starts.")
-
     xpac = p.fit(phases, amplitudes)  # (50, 50, 20)
     pac = xpac.mean(axis=-1)  # (50, 50)
 
-    ts("PAC Calculation with Tensorpac ends.")
-
-    ## Plot
-    fig, ax = plt.subplots()
-    ax = p.comodulogram(
-        pac, title=p.method.replace(" (", f" ({k})\n("), cmap="viridis"
-    )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    import ipdb
-
-    ipdb.set_trace()
+    # ## Plot
+    # fig, ax = plt.subplots()
+    # ax = p.comodulogram(
+    #     pac, title=p.method.replace(" (", f" ({k})\n("), cmap="viridis"
+    # )
+    # ax = mngs.plt.ax.set_n_ticks(ax)
     freqs_amp = p.f_amp.mean(axis=-1)
     freqs_pha = p.f_pha.mean(axis=-1)
 
-    return phases, amplitudes, freqs_pha, freqs_amp
+    pac = pac.T  # (amp, pha) -> (pha, amp)
+
+    return phases, amplitudes, freqs_pha, freqs_amp, pac
     # return phases and amplitudes for future use in my implementation
     # as the aim of this code is to confirm the calculation of Modulation Index only
     # without considering bandpass filtering and hilbert transformation.
 
 
-@torch_fn
-def reshape_pha_amp(pha, amp, batch_size=2, n_chs=4):
-    pha = torch.tensor(pha).half()
-    amp = torch.tensor(amp).half()
-    pha = pha.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    amp = amp.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    return pha, amp
-
+def plot_PAC_mngs_vs_tensorpac(pac_mngs, pac_tp, freqs_pha, freqs_amp):
+    assert pac_mngs.shape == pac_tp.shape
 
-if __name__ == "__main__":
-    import matplotlib.pyplot as plt
-    import mngs
+    # Plots
+    fig, axes = mngs.plt.subplots(ncols=3)
 
-    # Parameters
-    fs = 128
-    t_sec = 5
+    # To align scalebars
+    vmin = min(np.min(pac_mngs), np.min(pac_tp), np.min(pac_mngs - pac_tp))
+    vmax = max(np.max(pac_mngs), np.max(pac_tp), np.max(pac_mngs - pac_tp))
 
-    # Timestamper
-    ts = mngs.gen.TimeStamper()
-
-    # Demo signal
-    xx, tt, fs = mngs.dsp.demo_sig(fs=fs, t_sec=t_sec, sig_type="tensorpac")
-    # xx.shape: (8, 19, 20, 512)
+    # mngs version
+    ax = axes[0]
+    ax.imshow2d(
+        pac_mngs,
+        cbar=False,
+        vmin=vmin,
+        vmax=vmax,
+    )
+    ax.set_title("mngs")
 
     # Tensorpac
-    pha, amp, freqs_pha, freqs_amp = plot_comodulogram_tensorpac(
-        xx,
-        fs,
-        t_sec=t_sec,
-        ts=ts,
+    ax = axes[1]
+    ax.imshow2d(
+        pac_tp,
+        cbar=False,
+        vmin=vmin,
+        vmax=vmax,
     )
-    # mngs.io.save((pha, amp, freqs_pha, freqs_amp), "/tmp/out.pkl")
-    # pha, amp, freqs_pha, freqs_amp = mngs.io.load("/tmp/out.pkl")
+    ax.set_title("Tensorpac")
 
-    # GPU calculation
-    pha, amp = reshape_pha_amp(pha, amp)
+    # Diff.
+    ax = axes[2]
+    ax.imshow2d(
+        pac_mngs - pac_tp,
+        cbar_label="PAC values",
+        cbar_shrink=0.5,
+        vmin=vmin,
+        vmax=vmax,
+    )
+    ax.set_title(f"Difference\n(mngs - Tensorpac)")
 
-    ts("PAC Calculation with mngs.dsp starts.")
+    for ax in axes:
+        ax = mngs.plt.ax.set_ticks(
+            ax, xticks=freqs_pha.astype(int), yticks=freqs_amp.astype(int)
+        )
+        ax = mngs.plt.ax.set_n_ticks(ax)
+
+    fig.suptitle("PAC (MI) values")
+    fig.supxlabel("Frequency for phase [Hz]")
+    fig.supylabel("Frequency for amplitude [Hz]")
 
-    pac = mngs.dsp.modulation_index(pha, amp)
+    return fig
 
-    ts("PAC Calculation with mngs.dsp ends.")
 
-    ## Convert y-axis
-    i_batch, i_ch = 0, 0
+if __name__ == "__main__":
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
 
-    fig, ax = mngs.plt.subplots()
-    ax.imshow2d(
-        pac[i_batch, i_ch],
-        cbar_label="PAC values",
+    # Parameters
+    FS = 512
+    T_SEC = 8
+
+    xx, tt, fs = mngs.dsp.demo_sig(
+        batch_size=4,
+        n_chs=19,
+        n_segments=2,
+        fs=FS,
+        t_sec=T_SEC,
+        sig_type="tensorpac",
     )
-    ax = mngs.plt.ax.set_ticks(
-        ax, xticks=freqs_pha.astype(int), yticks=freqs_amp.astype(int)
+    xx = torch.tensor(xx)
+
+    phases, amplitudes, freqs_pha, freqs_amp, pac = calc_pac_with_tensorpac(
+        xx, fs, T_SEC, i_batch=0, i_ch=0
     )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    ax.set_xlabel("Frequency for phase [Hz]")
-    ax.set_ylabel("Frequency for amplitude [Hz]")
-    ax.set_title("GPU calculation")
 
-    plt.show()
+    phases.shape
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
+
+"""
+/ssh:ywatanabe@444:/home/ywatanabe/proj/entrance/mngs/dsp/utils/_calc_pac_with_tensorpac.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/dsp/_psd.py` & `mngs-1.3.0/src/mngs/dsp/_psd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 19:07:30 (ywatanabe)"
+# Time-stamp: "2024-04-13 01:32:37 (ywatanabe)"
+
+"""
+This script does XYZ.
+"""
 
 import torch
 import torch.nn as nn
 from mngs.general import torch_fn
 from mngs.nn import PSD
 
 
@@ -54,19 +58,47 @@
 
     # Average Power in Each Frequency Band
     avg_band_powers = self.calc_band_avg_power(psd, freqs)
     return (avg_band_powers,)
 
 
 if __name__ == "__main__":
+    import sys
+
     import matplotlib.pyplot as plt
     import mngs
 
-    x, t, f = mngs.dsp.demo_sig()  # (8, 19, 384)
-    BANDS = mngs.dsp.PARAMS.BANDS
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
 
-    pp, ff = psd(x, f, prob=True)
+    # Parameters
+    SIG_TYPE = "chirp"
 
-    plt, CC = mngs.plt.configure_mpl(plt)
-    fig, ax = mngs.plt.subplots()
-    ax.plot(ff, pp[0, 0])
-    plt.show()
+    # Demo signal
+    xx, tt, fs = mngs.dsp.demo_sig(SIG_TYPE)  # (8, 19, 384)
+
+    # PSD calculation
+    pp, ff = psd(xx, fs, prob=True)
+
+    # Plots
+    fig, axes = mngs.plt.subplots(nrows=2)
+
+    axes[0].plot(tt, xx[0, 0], label=SIG_TYPE)
+    axes[1].set_title("Signal")
+    axes[0].set_xlabel("Time [s]")
+    axes[0].set_ylabel("Amplitude [?V]")
+
+    axes[1].plot(ff, pp[0, 0])
+    axes[1].set_title("PSD (power spectrum density)")
+    axes[1].set_xlabel("Frequency [Hz]")
+    axes[1].set_ylabel("Log(Power [?V^2 / Hz]) [a.u.]")
+
+    mngs.io.save(fig, "psd.png")
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
+
+"""
+/home/ywatanabe/proj/entrance/mngs/dsp/_psd.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/dsp/_transform.py` & `mngs-1.3.0/src/mngs/dsp/_transform.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/add_noise.py` & `mngs-1.3.0/src/mngs/dsp/add_noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-#!/usr/bin/env python3
+#!./env/bin/python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 14:19:18 (ywatanabe)"
+# Time-stamp: "2024-04-13 01:18:23 (ywatanabe)"
 
-import mngs
+"""
+Functions to add noise to signals.
+"""
+
+# Imports
+import sys
 
-# import numpy as np
+import matplotlib.pyplot as plt
+import mngs
+import numpy as np
+import pandas as pd
 import torch
 from mngs.general import torch_fn
 
 
+# Functions
 def _uniform(shape, amp=1.0):
     a, b = -amp, amp
     return -amp + (2 * amp) * torch.rand(shape)
 
 
 @torch_fn
 def gauss(x, amp=1.0):
@@ -55,45 +64,56 @@
     noise = _uniform(x.shape, amp=amp)
     noise = torch.cumsum(noise, dim=dim)
     noise = mngs.dsp.norm.minmax(noise, amp=amp, dim=dim)
     return x + noise.to(x.device)
 
 
 if __name__ == "__main__":
-    import matplotlib.pyplot as plt
+    import mngs
 
-    plt, CC = mngs.plt.configure_mpl(plt)
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
 
-    t_sec = 1
-    fs = 128
-    xx, tt, fs = mngs.dsp.demo_sig(t_sec=t_sec, fs=fs)
+    # Parameters
+    T_SEC = 1
+    FS = 128
 
-    # t = np.linspace(0, t_sec, x.shape[-1])
+    # Demo signal
+    xx, tt, fs = mngs.dsp.demo_sig(t_sec=T_SEC, fs=FS)
 
     funcs = {
         "orig": lambda x: x,
         "gauss": gauss,
         "white": white,
         "pink": pink,
         "brown": brown,
     }
 
-    fig, axes = plt.subplots(
+    # Plots
+    fig, axes = mngs.plt.subplots(
         nrows=len(funcs), ncols=2, sharex=True, sharey=True
     )
     count = 0
     for (k, fn), axes_row in zip(funcs.items(), axes):
         for ax in axes_row:
             if count % 2 == 0:
                 ax.plot(tt, fn(xx)[0, 0], label=k, c="blue")
             else:
                 ax.plot(tt, (fn(xx) - xx)[0, 0], label=f"{k} - orig", c="red")
             count += 1
             ax.legend(loc="upper right")
-    plt.show()
 
-    # fig, axes = plt.subplots(nrows=len(funcs), sharex=True, sharey=True)
-    # for (k, fn), ax in zip(funcs.items(), axes):
-    #     ax.plot(t, fn(x)[0, 0], label=k, c="blue")
-    #     ax.plot(t, (fn(x) - x)[0, 0], label=f"{k} - orig", c="red")
-    #     ax.legend(loc="upper right")
-    # plt.show()
+    fig.supxlabel("Time [s]")
+    fig.supylabel("Amplitude [?V]")
+    axes[0, 0].set_title("Signal + Noise")
+    axes[0, 1].set_title("Noise")
+
+    mngs.io.save(fig, "traces.png")
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
+
+"""
+/home/ywatanabe/proj/entrance/mngs/dsp/add_noise.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/dsp/example.py` & `mngs-1.3.0/src/mngs/dsp/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_AxiswiseDropout.py` & `mngs-1.3.0/src/mngs/dsp/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_BNet.py` & `mngs-1.3.0/src/mngs/dsp/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_BNet_Res.py` & `mngs-1.3.0/src/mngs/dsp/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_ChannelGainChanger.py` & `mngs-1.3.0/src/mngs/dsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_DropoutChannels.py` & `mngs-1.3.0/src/mngs/dsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_Filters.py` & `mngs-1.3.0/src/mngs/dsp/nn/_Wavelet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,230 +1,171 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 04:06:50 (ywatanabe)"
+# Time-stamp: "2024-04-11 22:28:40 (ywatanabe)"
 
-import math
-import warnings
 
 import mngs
 import numpy as np
-import seaborn as sns
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mngs.general import torch_fn
 
 
-class BaseFilter1D(nn.Module):
+class Wavelet(nn.Module):
     def __init__(
-        self,
+        self, samp_rate, kernel_size=None, freq_scale="linear", out_scale="log"
     ):
         super().__init__()
+        self.register_buffer("dummy", torch.tensor(0))
         self.kernel = None
+        self.init_kernel(
+            samp_rate, kernel_size=kernel_size, freq_scale=freq_scale
+        )
+        self.out_scale = out_scale
 
-    @property
-    def kernel_size(
-        self,
-    ):
-        return mngs.gen.to_even(self.kernel.shape[-1])
-
-    @property
-    def radius(
-        self,
-    ):
-        return self.kernel_size // 2
-
-    def forward(self, x, t=None):
-        """Apply the filter to input signal x with shape: (batch_size, n_chs, seq_len)"""
-
-        x = mngs.dsp.ensure_3d(x)
+    def forward(self, x):
+        """Apply the 2D filter (n_filts, kernel_size) to input signal x with shape: (batch_size, n_chs, seq_len)"""
+        x = mngs.dsp.ensure_3d(x).to(self.dummy.device)
         seq_len = x.shape[-1]
 
         # Ensure the kernel is initialized
         if self.kernel is None:
             self.init_kernel()
             if self.kernel is None:
                 raise ValueError("Filter kernel has not been initialized.")
+        assert self.kernel.ndim == 2
+        self.kernel = self.kernel.to(x.device)  # cuda, torch.complex128
 
         # Edge handling and convolution
         extension_length = self.radius
         first_segment = x[:, :, :extension_length].flip(dims=[-1])
         last_segment = x[:, :, -extension_length:].flip(dims=[-1])
         extended_x = torch.cat([first_segment, x, last_segment], dim=-1)
 
-        channels = extended_x.size(1)
+        # working??
+        kernel_batched = self.kernel.unsqueeze(1)
+        extended_x_reshaped = extended_x.view(-1, 1, extended_x.shape[-1])
 
-        kernel = (
-            self.kernel.expand(channels, 1, -1)
-            .to(extended_x.device)
-            .to(extended_x.dtype)
+        filtered_x_real = F.conv1d(
+            extended_x_reshaped, kernel_batched.real.float(), groups=1
+        )
+        filtered_x_imag = F.conv1d(
+            extended_x_reshaped, kernel_batched.imag.float(), groups=1
         )
 
-        x_filted_extended = F.conv1d(
-            extended_x, kernel, padding=0, groups=channels
-        )[..., :seq_len]
-
-        assert x.shape == x_filted_extended.shape
-
-        # # Remove edges
-        # x_filted_extended[..., : self.radius] *= 0
-        # x_filted_extended[..., -self.radius :] *= 0
-
-        nn_remove = x_filted_extended.shape[-1] // 4
-        x_filted_extended = x_filted_extended[..., nn_remove:-nn_remove]
-        return x_filted_extended
-
-
-class GaussianFilter(BaseFilter1D):
-    def __init__(self, sigma):
-        super().__init__()
-        self.sigma = mngs.gen.to_even(sigma)
-        self.init_kernel()
-
-    def init_kernel(self):
-        # Create a Gaussian kernel
-        kernel_size = self.sigma * 6  # +/- 3SD
-        kernel_range = torch.arange(kernel_size) - kernel_size // 2
-        kernel = torch.exp(-0.5 * (kernel_range / self.sigma) ** 2)
-        kernel /= kernel.sum()  # Normalize the kernel
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
-
+        filtered_x = torch.view_as_complex(
+            torch.stack([filtered_x_real, filtered_x_imag], dim=-1)
+        )
 
-class LowPassFilter(BaseFilter1D):
-    def __init__(self, cutoff_hz, fs, kernel_size=None):
-        super().__init__()
-        self.cutoff_hz = cutoff_hz
-        self.fs = fs
+        filtered_x = filtered_x.view(
+            x.shape[0], x.shape[1], kernel_batched.shape[0], -1
+        )
+        filtered_x = filtered_x.view(
+            x.shape[0], x.shape[1], kernel_batched.shape[0], -1
+        )
+        filtered_x = filtered_x[..., :seq_len]
+        assert filtered_x.shape[-1] == seq_len
 
-        kernel_size = (
-            mngs.gen.to_even(int(1 / cutoff_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[
-            freqs <= self.cutoff_hz
-        ] = 1  # Allow frequencies below the cutoff
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.abs().sum()  # Normalize the kernel by its absolute sum
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+        pha = filtered_x.angle()
+        amp = filtered_x.abs()
 
+        if self.out_scale == "log":
+            return torch.log(pha + 1e-5), torch.log(amp + 1e-5), self.freqs
+        else:
+            return pha, amp, self.freqs
 
-class HighPassFilter(BaseFilter1D):
-    def __init__(self, cutoff_hz, fs, kernel_size=None):
-        super().__init__()
-        self.cutoff_hz = cutoff_hz
-        self.fs = fs
-        kernel_size = (
-            mngs.gen.to_even(int(1 / cutoff_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[
-            freqs >= self.cutoff_hz
-        ] = 1  # Allow frequencies above the cutoff
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.abs().sum()  # Normalize the kernel by its absolute sum
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+    def init_kernel(self, samp_rate, kernel_size=None, freq_scale="log"):
+        device = self.dummy.device
+        morlets, freqs = self.gen_morlet_to_nyquist(
+            samp_rate, kernel_size=kernel_size, freq_scale=freq_scale
+        )
+        self.kernel = torch.tensor(morlets).to(device)
+        self.freqs = torch.tensor(freqs).float().to(device)
 
+    @staticmethod
+    def gen_morlet_to_nyquist(
+        samp_rate, kernel_size=None, freq_scale="linear"
+    ):
+        """
+        Generates Morlet wavelets for exponentially increasing frequency bands up to the Nyquist frequency.
 
-class BandPassFilter(BaseFilter1D):
-    def __init__(self, low_hz, high_hz, fs, kernel_size=None):
-        super().__init__()
+        Parameters:
+        - samp_rate (int): The sampling rate of the signal, in Hertz.
+        - kernel_size (int): The size of the kernel, in number of samples.
+
+        Returns:
+        - np.ndarray: A 2D array of complex values representing the Morlet wavelets for each frequency band.
+        """
+        if kernel_size is None:
+            kernel_size = int(samp_rate)  # * 2.5)
+
+        nyquist_freq = samp_rate / 2
+
+        # Log freq_scale
+        def calc_freq_boundaries_log(nyquist_freq):
+            n_kernels = int(np.floor(np.log2(nyquist_freq)))
+            mid_hz = np.array([2 ** (n + 1) for n in range(n_kernels)])
+            width_hz = np.hstack([np.array([1]), np.diff(mid_hz) / 2]) + 1
+            low_hz = mid_hz - width_hz
+            high_hz = mid_hz + width_hz
+            low_hz[0] = 0.1
+            return low_hz, high_hz
+
+        def calc_freq_boundaries_linear(nyquist_freq):
+            n_kernels = int(nyquist_freq)
+            high_hz = np.linspace(1, nyquist_freq, n_kernels)
+            low_hz = high_hz - np.hstack([np.array(1), np.diff(high_hz)])
+            low_hz[0] = 0.1
+            return low_hz, high_hz
+
+        if freq_scale == "linear":
+            fn = calc_freq_boundaries_linear
+        if freq_scale == "log":
+            fn = calc_freq_boundaries_log
+        low_hz, high_hz = fn(nyquist_freq)
+
+        morlets = []
+        freqs = []
+
+        for _, (ll, hh) in enumerate(zip(low_hz, high_hz)):
+            if ll > nyquist_freq:
+                break
+
+            center_frequency = (ll + hh) / 2
+
+            t = np.arange(-kernel_size // 2, kernel_size // 2) / samp_rate
+            # Calculate standard deviation of the gaussian window for a given center frequency
+            sigma = 7 / (2 * np.pi * center_frequency)
+            sine_wave = np.exp(2j * np.pi * center_frequency * t)
+            gaussian_window = np.exp(-(t**2) / (2 * sigma**2))
+            morlet_wavelet = sine_wave * gaussian_window
 
-        assert 0 < low_hz
-        assert low_hz < high_hz
-        assert high_hz <= fs / 2
-
-        kernel_size = (
-            mngs.gen.to_even(int(1 / low_hz * fs * 3))
-            # mngs.gen.to_even(int(low_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-
-        self.low_hz = low_hz
-        self.high_hz = high_hz
-        self.fs = fs
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[(self.low_hz <= freqs) & (freqs <= self.high_hz)] = 1
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.sum()
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+            freqs.append(center_frequency)
+            morlets.append(morlet_wavelet)
 
+        return np.array(morlets), np.array(freqs)
 
-class BandStopFilter(BaseFilter1D):
-    def __init__(self, low_hz, high_hz, fs, kernel_size=None):
-        super().__init__()
-        kernel_size = (
-            mngs.gen.to_even(int(1 / low_hz * fs * 3))
-            # mngs.gen.to_even(int(low_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-        self.low_hz = low_hz
-        self.high_hz = high_hz
-        self.fs = fs
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.ones(kernel_size)
-        kernel[(freqs >= self.low_hz) & (freqs <= self.high_hz)] = 0
-        kernel = torch.fft.ifft(
-            kernel
-        ).real  # Inverse FFT to get the time-domain kernel
-        # kernel /= kernel.sum()  # Normalize the kernel
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+    @property
+    def kernel_size(
+        self,
+    ):
+        return mngs.gen.to_even(self.kernel.shape[-1])
 
+    @property
+    def radius(
+        self,
+    ):
+        return mngs.gen.to_even(self.kernel_size // 2)
 
-class HanningFilter(BaseFilter1D):
-    def __init__(self, window_size):
-        super().__init__()
-        self.window_size = mngs.gen.to_even(int(window_size))
-        self.init_kernel()
 
-    def init_kernel(self):
-        # Create a Hanning window
-        self.kernel = (
-            torch.hann_window(self.window_size).unsqueeze(0).unsqueeze(0)
-        )
+if __name__ == "__main__":
+    import mngs
 
-    def forward(self, x):
-        """Apply the Hanning window to input signal x with shape: (batch_size, n_chs, seq_len)"""
+    xx, tt, fs = mngs.dsp.demo_sig(sig_type="chirp")
 
-        x = mngs.dsp.ensure_3d(x)
-        seq_len = x.shape[-1]
+    ww, ff = mngs.dsp.wavelet(xx, fs)
 
-        # Check if the input signal is longer than the window size
-        if seq_len < self.window_size:
-            raise ValueError(
-                "Input signal length must be greater than the window size."
-            )
-
-        # Apply the window to the signal
-        # Assuming that we want to apply the window to the central part of the signal
-        start = (seq_len - self.window_size) // 2
-        end = start + self.window_size
-        windowed_x = x.clone()  # Create a copy of x to apply window
-        windowed_x[:, :, start:end] *= self.kernel.to(x.device).to(x.dtype)
-
-        return windowed_x
-
-
-# @torch_fn
-# def hanning(x, window_size):
-#     return HanningFilter(window_size)(x)
+    fig, ax = mngs.plt.subplots()
+    ax.imshow2d(ww[0, 0].T)
+    ax = mngs.plt.ax.set_ticks(ax, xticks=tt, yticks=ff)
+    ax = mngs.plt.ax.set_n_ticks(ax)
+    plt.show()
```

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_FreqGainChanger.py` & `mngs-1.3.0/src/mngs/dsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_GaussianFilter.py` & `mngs-1.3.0/src/mngs/dsp/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_MNet_1000.py` & `mngs-1.3.0/src/mngs/dsp/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_ModulationIndex.py` & `mngs-1.3.0/src/mngs/dsp/nn/_ModulationIndex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 11:30:02 (ywatanabe)"
+# Time-stamp: "2024-04-12 23:51:57 (ywatanabe)"
 
+"""
+This script does XYZ.
+"""
 
+# Imports
 import math
+import sys
 import time
 
+import mngs
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mngs.general import torch_fn
 
+# Config
+CONFIG = mngs.gen.load_configs()
 
+# Functions
 class ModulationIndex(nn.Module):
-    def __init__(self, n_bins=18):
+    def __init__(self, n_bins=18, fp16=False):
         super(ModulationIndex, self).__init__()
         self.n_bins = n_bins
+        self.fp16 = fp16
         self.register_buffer(
             "pha_bin_cutoffs", torch.linspace(-np.pi, np.pi, n_bins + 1)
         )
 
     def forward(self, pha, amp, epsilon=1e-9):
         """
         Compute the Modulation Index based on phase (pha) and amplitude (amp) tensors.
@@ -32,15 +42,19 @@
                               (batch_size, n_channels, n_freqs_amp, n_segments, sequence_length).
 
         Returns:
         - MI (torch.Tensor): The Modulation Index for each batch and channel.
         """
         assert pha.ndim == amp.ndim == 5
 
-        pha, amp = pha.float().contiguous(), amp.float().contiguous()
+        if self.fp16:
+            pha, amp = pha.half().contiguous(), amp.half().contiguous()
+        else:
+            pha, amp = pha.float().contiguous(), amp.float().contiguous()
+
         device = pha.device
 
         pha_masks = self._phase_to_masks(pha, self.pha_bin_cutoffs.to(device))
         # (batch_size, n_channels, n_freqs_pha, n_segments, sequence_length, n_bins)
 
         # Expands amp and masks to utilize broadcasting
         i_batch = 0
@@ -64,20 +78,21 @@
         amp_probs = amp_means / (
             amp_means.sum(dim=-1, keepdims=True) + epsilon
         )
 
         MI = (
             torch.log(torch.tensor(self.n_bins, device=device) + epsilon)
             + (amp_probs * (amp_probs + epsilon).log()).sum(dim=-1)
-        ) / (
-            torch.log(torch.tensor(self.n_bins, device=device) + epsilon)
-            + epsilon
-        )
+        ) / torch.log(torch.tensor(self.n_bins, device=device))
+
+        # Squeeze the n_bin dimension
+        MI = MI.squeeze(-1)
 
-        MI = MI.squeeze(-1).mean(axis=-1)
+        # Takes mean along the n_segments dimension
+        MI = MI.mean(axis=-1)
 
         if MI.isnan().any():
             raise ValueError(
                 "NaN values detected in Modulation Index calculation."
             )
 
         return MI
@@ -97,98 +112,68 @@
         one_hot_masks = F.one_hot(
             bin_indices,
             num_classes=n_bins,
         )
         return one_hot_masks
 
 
-def plot_comodulogram_tensorpac(xx, fs, t_sec):
-    # Morlet's Wavelet Transfrmation
-    p = tensorpac.Pac(f_pha="hres", f_amp="hres", dcomplex="wavelet")
-
-    # Bandpass Filtering and Hilbert Transformation
-    i_batch, i_ch = 0, 0
-    phases = p.filter(
-        fs, xx[i_batch, i_ch], ftype="phase", n_jobs=1
-    )  # (50, 20, 2048)
-    amplitudes = p.filter(
-        fs, xx[i_batch, i_ch], ftype="amplitude", n_jobs=1
-    )  # (50, 20, 2048)
-
-    # Calculates xpac
-    k = 2
-    p.idpac = (k, 0, 0)
-    xpac = p.fit(phases, amplitudes)  # (50, 50, 20)
-    pac = xpac.mean(axis=-1)  # (50, 50)
-
-    ## Plot
-    fig, ax = plt.subplots()
-    ax = p.comodulogram(
-        pac, title=p.method.replace(" (", f" ({k})\n("), cmap="viridis"
+def _reshape(x, batch_size=2, n_chs=4):
+    return (
+        torch.tensor(x)
+        .float()
+        .unsqueeze(0)
+        .unsqueeze(0)
+        .repeat(batch_size, n_chs, 1, 1, 1)
     )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    freqs_amp = p.f_amp.mean(axis=-1)
-    freqs_pha = p.f_pha.mean(axis=-1)
-
-    return phases, amplitudes, freqs_pha, freqs_amp
-    # return phases and amplitudes for future use in my implementation
-    # as the aim of this code is to confirm the calculation of Modulation Index only
-    # without considering bandpass filtering and hilbert transformation.
-
-
-def reshape_pha_amp(pha, amp, batch_size=2, n_chs=4):
-    pha = torch.tensor(pha).half()
-    amp = torch.tensor(amp).half()
-    pha = pha.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    amp = amp.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    return pha, amp
-
-
-@torch_fn
-def modulation_index(pha, amp, n_bins=18):
-    return ModulationIndex(n_bins=18)(pha, amp)
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
     import mngs
     import seaborn as sns
     import tensorpac
     from tensorpac import Pac
     from tqdm import tqdm
 
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(
+        sys, plt, fig_scale=3
+    )
+
     # Parameters
-    fs = 128
-    t_sec = 5
+    FS = 512
+    T_SEC = 5
 
     # Demo signal
-    xx, tt, fs = mngs.dsp.demo_sig(fs=fs, t_sec=t_sec, sig_type="tensorpac")
+    xx, tt, fs = mngs.dsp.demo_sig(fs=FS, t_sec=T_SEC, sig_type="tensorpac")
     # xx.shape: (8, 19, 20, 512)
 
     # Tensorpac
-    pha, amp, freqs_pha, freqs_amp = plot_comodulogram_tensorpac(
-        xx, fs, t_sec=t_sec
-    )
-    # mngs.io.save((pha, amp, freqs_pha, freqs_amp), "/tmp/out.pkl")
-    # pha, amp, freqs_pha, freqs_amp = mngs.io.load("/tmp/out.pkl")
-
-    # GPU calculation
-    pha, amp = reshape_pha_amp(pha, amp)
-    pac = mngs.dsp.modulation_index(pha, amp)
-
-    ## Convert y-axis
+    (
+        pha,
+        amp,
+        freqs_pha,
+        freqs_amp,
+        pac_tp,
+    ) = mngs.dsp.utils.pac.calc_pac_with_tensorpac(xx, fs, t_sec=T_SEC)
+
+    # GPU calculation with mngs.dsp.nn.ModulationIndex
+    pha, amp = _reshape(pha), _reshape(amp)
+    pac_mngs = mngs.dsp.modulation_index(pha, amp).cpu().numpy()
     i_batch, i_ch = 0, 0
+    pac_mngs = pac_mngs[i_batch, i_ch]
 
-    fig, ax = mngs.plt.subplots()
-    ax.imshow2d(
-        pac[i_batch, i_ch].cpu().numpy(),
-        cbar_label="PAC values",
+    # Plots
+    fig = mngs.dsp.utils.pac.plot_PAC_mngs_vs_tensorpac(
+        pac_mngs, pac_tp, freqs_pha, freqs_amp
     )
-    ax = mngs.plt.ax.set_ticks(
-        ax, xticks=freqs_pha.astype(int), yticks=freqs_amp.astype(int)
-    )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    ax.set_xlabel("Frequency for phase [Hz]")
-    ax.set_ylabel("Frequency for amplitude [Hz]")
-    ax.set_title("GPU calculation")
+    # fig = plot_PAC_mngs_vs_tensorpac(pac_mngs, pac_tp, freqs_pha, freqs_amp)
+    mngs.io.save(fig, CONFIG["SDIR"] + "modulation_index.png")  # plt.show()
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
 
-    plt.show()
+"""
+/home/ywatanabe/proj/entrance/mngs/nn/_ModulationIndex.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_PAC_working.py` & `mngs-1.3.0/src/mngs/dsp/nn/_PAC_working.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_PSD.py` & `mngs-1.3.0/src/mngs/dsp/nn/_PSD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 19:03:07 (ywatanabe)"
+# Time-stamp: "2024-04-11 21:50:09 (ywatanabe)"
 
 import torch
 import torch.nn as nn
 
 
 class PSD(nn.Module):
     def __init__(self, sample_rate, prob=False, dim=-1):
```

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_ResNet1D.py` & `mngs-1.3.0/src/mngs/dsp/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_SpatialAttention.py` & `mngs-1.3.0/src/mngs/dsp/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_Spectrogram.py` & `mngs-1.3.0/src/mngs/dsp/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/_SwapChannels.py` & `mngs-1.3.0/src/mngs/dsp/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/dsp/nn/__init__.py` & `mngs-1.3.0/src/mngs/dsp/nn/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 12:51:19 (ywatanabe)"
+# Time-stamp: "2024-04-12 19:55:23 (ywatanabe)"
 
 from ._AxiswiseDropout import AxiswiseDropout
-
-# from ._BandPassFilter import BandPassFilter
 from ._BNet import BNet, BNet_config
 from ._ChannelGainChanger import ChannelGainChanger
 from ._DropoutChannels import DropoutChannels
-
-# from ._GaussianFilter import GaussianFilter
 from ._Filters import (
     BandPassFilter,
     BandStopFilter,
+    DifferentiableBandPassFilter,
     GaussianFilter,
     HighPassFilter,
     LowPassFilter,
 )
 from ._FreqGainChanger import FreqGainChanger
 from ._Hilbert import Hilbert
```

### Comparing `mngs-1.2.3/src/mngs/dsp/ref.py` & `mngs-1.3.0/src/mngs/dsp/reference.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/_TimeStamper.py` & `mngs-1.3.0/src/mngs/general/_TimeStamper.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/__init__.py` & `mngs-1.3.0/src/mngs/general/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 #!/usr/bin/env python3
 
-# from .path import find_the_git_root_dir, get_this_fpath, mk_spath, split_fpath
-# from .load import get_data_path_from_a_package, load
-# from .save import is_listed_X, save, save_listed_dfs_as_csv, save_listed_scalars_as_csv
-# from .debug import *
-from ..io.__init__ import *
+
 from ._close import close
 from ._converters import (
     numpy_fn,
     squeeze_if,
     to_numpy,
     to_torch,
     torch_fn,
     unsqueeze_if,
 )
+from ._embed import embed
+
+# Confirmed
+from ._paste import paste
+from ._reload import reload
+
+_ = None
+from ..io.__init__ import *
 from ._cuda_collect_env import main as cuda_collect_env
 from ._norm import to_z
-from ._reload import reload
+from ._reproduce import fix_seeds, gen_ID, gen_timestamp, tee
 from ._shell import run_shellcommand, run_shellscript
 from ._start import start
 from ._TimeStamper import TimeStamper
 from .email import notify, send_gmail
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
-from .mat2py import *
+
+# from .mat2py import *
 from .misc import (
     _return_counting_process,
     color_text,
     connect_nums,
     connect_strs,
     copy_files,
     copy_the_file,
@@ -34,14 +39,15 @@
     decapitalize,
     describe,
     fmt_size,
     grep,
     is_defined_global,
     is_defined_local,
     is_later_or_equal,
+    is_listed_X,
     is_nan,
     isclose,
     listed_dict,
     merge_dicts_wo_overlaps,
     mv_col,
     partial_at,
     pop_keys,
@@ -60,9 +66,7 @@
 from .pandas import (
     col_to_last,
     col_to_top,
     force_dataframe,
     ignore_SettingWithCopyWarning,
     merge_columns,
 )
-from .repro import *
-from .torch import *
```

### Comparing `mngs-1.2.3/src/mngs/general/_close.py` & `mngs-1.3.0/src/mngs/general/_close.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-11 14:28:22 (ywatanabe)"
+# Time-stamp: "2024-04-10 19:53:26 (ywatanabe)"
 
 import os
 import shutil
 from datetime import datetime, timedelta
 from glob import glob
 from time import sleep
 
@@ -60,18 +60,20 @@
 
 
 def finish(src_dir):
     dest_dir = src_dir.replace("RUNNING", "FINISHED")
     os.makedirs(dest_dir, exist_ok=True)
     try:
         os.rename(src_dir, dest_dir)
-        print(f"\nRenamed from: {src_dir} to {dest_dir}")
+        mngs.gen.print_block(
+            f"Congratulations! Results have been moved from RUNNING to FINISHED.\n\n{src_dir}\n\nv\nv\n\n{dest_dir}",
+            c="yellow",
+        )
     except Exception as e:
-        pass
-        # print(e)
+        print(e)
 
 
 if __name__ == "__main__":
     import sys
 
     import matplotlib.pyplot as plt
     import mngs
```

### Comparing `mngs-1.2.3/src/mngs/general/_converters.py` & `mngs-1.3.0/src/mngs/general/_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-07 21:54:06 (ywatanabe)"#!/usr/bin/env python3
+# Time-stamp: "2024-04-11 08:17:56 (ywatanabe)"#!/usr/bin/env python3
 
 import warnings
 from functools import wraps
 
 import numpy as np
 import pandas as pd
 import torch
```

### Comparing `mngs-1.2.3/src/mngs/general/_cuda_collect_env.py` & `mngs-1.3.0/src/mngs/general/_cuda_collect_env.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/_norm.py` & `mngs-1.3.0/src/mngs/general/_norm.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/_shell.py` & `mngs-1.3.0/src/mngs/general/_shell.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/_start.py` & `mngs-1.3.0/src/mngs/general/_start.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,100 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-25 12:12:15 (ywatanabe)"
+# Time-stamp: "2024-04-12 23:27:11 (ywatanabe)"
 
 import inspect
 import os as _os
 from datetime import datetime
 from glob import glob
 from pprint import pprint
 from time import sleep
 
+import matplotlib
 import mngs
 
 
 def start(
     sys=None,
     plt=None,
     sdir=None,
-    show=True,
+    verbose=True,
     # Random seeds
     os=None,
     random=None,
     np=None,
     torch=None,
     tf=None,
     seed=42,
     # matplotlib
+    agg=False,
     fig_size_mm=(160, 100),
     fig_scale=1.0,
     dpi_display=100,
     dpi_save=300,
     font_size_base=8,
     font_size_title=8,
     font_size_axis_label=8,
     font_size_tick_label=7,
     font_size_legend=6,
     hide_top_right_spines=True,
-    alpha=0.75,
+    alpha=0.9,
+    line_width=0.5,
 ):
     """
-    import sys
-    import matplotlib.pyplot as plt
+    Example:
+
+    \"""
+    This script does XYZ.
+    \"""
+
+    # Imports
     import mngs
+    import matplotlib.pyplot as plt
+    import numpy as np
+    import pandas as pd
+    import torch
+    import torch.nn as nn
+    import torch.nn.functional as F
+
+    # Config
+    CONFIG = mngs.gen.load_configs()
+
+    # Functions
+    # (Your awesome code here)
+
+    if __name__ == '__main__':
+        # Start
+        CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
 
-    CONFIG, sys.stdout, sys.stderr, plt, cc = mngs.gen.start(sys, plt)
+        # (Your awesome code here)
 
-    # YOUR CODE HERE
+        # Close
+        mngs.gen.close(CONFIG)
 
-    mngs.gen.close(CONFIG)
+    # EOF
+
+    \"""
+    /home/ywatanabe/template.py
+    \"""
     """
+
     # Timer
     start_time = datetime.now()
 
     # Debug mode check
     try:
-        IS_DEBUG = mngs.io.load("./config/IS_DEBUG.yaml").get(
-            "IS_DEBUG", False
-        )
+        IS_DEBUG_PATH = "./config/IS_DEBUG.yaml"
+        if _os.path.exists(IS_DEBUG_PATH):
+            IS_DEBUG = mngs.io.load(IS_DEBUG_PATH).get("IS_DEBUG", False)
+        else:
+            IS_DEBUG = False
+
     except Exception as e:
+        print(e)
         IS_DEBUG = False
 
     # ID
     ID = mngs.gen.gen_ID(N=4)
     ID = ID if not IS_DEBUG else "DEBUG_" + ID
     print(f"\n{'#'*40}\n## {ID}\n{'#'*40}\n")
     sleep(1)
@@ -68,35 +102,34 @@
     # Defines SDIR
     if sdir is None:
         __file__ = inspect.stack()[1].filename
         if "ipython" in __file__:
             __file__ = "/tmp/fake.py"
         spath = __file__
         _sdir, sfname, _ = mngs.general.split_fpath(spath)
-        sdir = (
-            _sdir + sfname + "/" + "RUNNING" + "/" + ID + "/"
-        )  # " # + "/log/"
+        sdir = _sdir + sfname + "/" + "RUNNING" + "/" + ID + "/"
     _os.makedirs(sdir, exist_ok=True)
 
     # CONFIGs
     CONFIGS = mngs.io.load_configs(IS_DEBUG)
     CONFIGS["ID"] = ID
     CONFIGS["START_TIME"] = start_time
     CONFIGS["SDIR"] = sdir.replace("/./", "/")
-    if show:
+    if verbose:
         print(f"\n{'-'*40}\n")
         print(f"CONFIG:")
         for k, v in CONFIGS.items():
             print(f"\n{k}:\n{v}\n")
-            # sleep(0.1)
         print(f"\n{'-'*40}\n")
 
     # Logging (tee)
     if sys is not None:
-        sys.stdout, sys.stderr = mngs.general.tee(sys, sdir=sdir, show=show)
+        sys.stdout, sys.stderr = mngs.general.tee(
+            sys, sdir=sdir, verbose=verbose
+        )
 
     # Random seeds
     if (
         (os is not None)
         or (random is not None)
         or (np is not None)
         or (torch is not None)
@@ -110,46 +143,67 @@
             tf=tf,
             seed=seed,
             show=show,
         )
 
     # Matplotlib configuration
     if plt is not None:
-        plt, cc = mngs.plt.configure_mpl(
+        plt, CC = mngs.plt.configure_mpl(
             plt,
             fig_size_mm=(160, 100),
             fig_scale=fig_scale,
             dpi_display=dpi_display,
             dpi_save=dpi_save,
             font_size_base=font_size_base,
             font_size_title=font_size_title,
             font_size_axis_label=font_size_axis_label,
             font_size_tick_label=font_size_tick_label,
             font_size_legend=font_size_legend,
             hide_top_right_spines=hide_top_right_spines,
             alpha=alpha,
-            show=show,
+            line_width=line_width,
+            verbose=verbose,
         )
 
-    return CONFIGS, sys.stdout, sys.stderr, plt, cc
+    if agg:
+        matplotlib.use("Agg")
+
+    return CONFIGS, sys.stdout, sys.stderr, plt, CC
 
 
 if __name__ == "__main__":
+    """
+    This script does XYZ.
+    """
+
+    # Imports
+    import os
     import sys
 
     import matplotlib.pyplot as plt
     import mngs
+    import numpy as np
+    import pandas as pd
+    import torch
+    import torch.nn as nn
+    import torch.nn.functional as F
 
-    # --------------------------------------------------------------------------- #
-    CONFIG, sys.stdout, sys.stderr, plt, cc = mngs.gen.start(
-        sys, plt, sdir=None
-    )
-    # --------------------------------------------------------------------------- #
-
-    # YOUR CODE HERE
-    print("Hello world from mngs.")
-
-    # --------------------------------------------------------------------------- #
-    mngs.gen.close(CONFIG)
-    # --------------------------------------------------------------------------- #
+    # Config
+    CONFIG = mngs.gen.load_configs()
 
-    # EOF
+    # Functions
+    # Your awesome code here :)
+
+    if __name__ == "__main__":
+        # Start
+        CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
+
+        # Your awesome code here :)
+
+        # Close
+        mngs.gen.close(CONFIG)
+
+# EOF
+
+"""
+/home/ywatanabe/proj/entrance/mngs/general/_start.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/general/_xml2dict.py` & `mngs-1.3.0/src/mngs/general/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/email.py` & `mngs-1.3.0/src/mngs/general/email.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/load.py` & `mngs-1.3.0/src/mngs/general/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,16 @@
 import mne
 import mngs
 import numpy as np
 import pandas as pd
 import torch
 import yaml
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.load" will be removed. '
-            'Please use "mngs.io.load" instead.',
-            PendingDeprecationWarning,
-        )
-
 
-def load(lpath, show=False, **kwargs):
+def load(lpath, show=False, verbose=False, **kwargs):
     import logging
 
     try:
         extension = "." + lpath.split(".")[-1]  # [REVISED]
 
         # csv
         if extension == ".csv":
@@ -146,22 +137,25 @@
         ]:
             obj = load_eeg_data(lpath, **kwargs)
 
         else:
             print(f"\nNot loaded from: {lpath}\n")
             return None
 
-        if show:
+        if show or verbose:
             print(f"\nLoaded from: {lpath}\n")
 
         return obj
 
     except Exception as e:
-        logging.error(f"\n{lpath} was not loaded:\n{e}")
-        return None
+        if verbose:
+            print(f"\n{lpath} was not loaded:\n{e}")
+
+        # logging.error(f"\n{lpath} was not loaded:\n{e}")
+        # return None
 
 
 def load_eeg_data(filename, **kwargs):
     """
     Load EEG data based on file extension and associated files using MNE-Python.
 
     Parameters:
@@ -287,34 +281,35 @@
     # rdb_raw_bytes_url = "sqlite:////tmp/fake/ywatanabe/_MicroNN_WindowSize-1.0-sec_MaxEpochs_100_2021-1216-1844/optuna_study_test_file#0.db"
     storage = optuna.storages.RDBStorage(url=rdb_raw_bytes_url)
     study = optuna.load_study(study_name=study_name, storage=storage)
     print(f"\nLoaded: {rdb_raw_bytes_url}\n")
     return study
 
 
-def load_configs(IS_DEBUG=None, show=False):
+def load_configs(IS_DEBUG=None, show=False, verbose=False):
+
     if os.getenv("CI") == "true":
         IS_DEBUG = True
 
     def update_debug(config, IS_DEBUG):
         if IS_DEBUG:
             debug_keys = mngs.gen.search("^DEBUG_", list(config.keys()))[1]
             for dk in debug_keys:
                 dk_wo_debug_prefix = dk.split("DEBUG_")[1]
                 config[dk_wo_debug_prefix] = config[dk]
-                if show:
+                if show or verbose:
                     print(f"\n{dk} -> {dk_wo_debug_prefix}\n")
         return config
 
     # Check ./config/IS_DEBUG.yaml file if IS_DEBUG argument is not passed
     if IS_DEBUG is None:
-        try:
-            IS_DEBUG = mngs.io.load("./config/IS_DEBUG.yaml")["IS_DEBUG"]
-        except Exception as e:
-            print(e)
+        IS_DEBUG_PATH = "./config/IS_DEBUG.yaml"
+        if os.path.exists(IS_DEBUG_PATH):
+            IS_DEBUG = mngs.io.load("./config/IS_DEBUG.yaml").get("IS_DEBUG")
+        else:
             IS_DEBUG = False
 
     # Main
     CONFIGS = {}
     for lpath in glob("./config/*.yaml"):
         CONFIG = update_debug(mngs.io.load(lpath), IS_DEBUG)
         CONFIGS.update(CONFIG)
```

### Comparing `mngs-1.2.3/src/mngs/general/mat2py.py` & `mngs-1.3.0/src/mngs/general/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/misc.py` & `mngs-1.3.0/src/mngs/general/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,14 +178,44 @@
         num /= 1024.0
     return "%.1f%s%s" % (num, "Yi", suffix)
 
 
 ################################################################################
 ## list
 ################################################################################
+def is_listed_X(obj, types):
+    """
+    Example:
+        obj = [3, 2, 1, 5]
+        _is_listed_X(obj,
+    """
+    import numpy as np
+
+    try:
+        conditions = []
+        condition_list = isinstance(obj, list)
+
+        if not (isinstance(types, list) or isinstance(types, tuple)):
+            types = [types]
+
+        _conditions_susp = []
+        for typ in types:
+            _conditions_susp.append(
+                (np.array([isinstance(o, typ) for o in obj]) == True).all()
+            )
+
+        condition_susp = np.any(_conditions_susp)
+
+        _is_listed_X = np.all([condition_list, condition_susp])
+        return _is_listed_X
+
+    except:
+        return False
+
+
 def take_the_closest(list_obj, num_insert):
     """
     Assumes list_obj is sorted. Returns the closest value to num.
     If the same number is included in list_obj, the smaller number is returned.
 
     Example:
         list_obj = np.array([0, 1, 1, 2, 3, 3])
```

### Comparing `mngs-1.2.3/src/mngs/general/pandas.py` & `mngs-1.3.0/src/mngs/general/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/general/path.py` & `mngs-1.3.0/src/mngs/general/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,14 @@
 import re
 import subprocess
 import warnings
 from glob import glob
 
 import mngs
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.path" will be removed. '
-            'Please use "mngs.io.path" instead.',
-            PendingDeprecationWarning,
-        )
-
 
 ################################################################################
 ## PATH
 ################################################################################
 def get_this_fpath(when_ipython="/tmp/fake.py"):
     __file__ = inspect.stack()[1].filename
     if "ipython" in __file__:  # for ipython
@@ -33,16 +24,14 @@
 
 def mk_spath(sfname, makedirs=False):
 
     __file__ = inspect.stack()[1].filename
     if "ipython" in __file__:  # for ipython
         __file__ = f'/tmp/fake-{os.getenv("USER")}.py'
 
-    # __file__ = get_current_file_name()
-
     ## spath
     fpath = __file__
     fdir, fname, _ = split_fpath(fpath)
     sdir = fdir + fname + "/"
     spath = sdir + sfname
 
     if makedirs:
```

### Comparing `mngs-1.2.3/src/mngs/general/repro.py` & `mngs-1.3.0/src/mngs/general/_reproduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             for f in self._files:
                 res = getattr(f, attr, *args)(*a, **kw)
             return res
 
         return g
 
 
-def tee(sys, sdir=None, show=True):
+def tee(sys, sdir=None, verbose=True):
     """
     import sys
 
     sys.stdout, sys.stderr = tee(sys)
 
     print("abc")  # stdout
     print(1 / 0)  # stderr
@@ -136,14 +136,16 @@
 
     # os.makedirs("/tmp/mngs/", exist_ok=True)
     # spath_stdout_def = "/tmp/mngs/stdout.log"
     # spath_stderr_def = "/tmp/mngs/stderr.log"
     # sys_stdout = Tee(sys.stdout, spath_stdout_def)
     # sys_stderr = Tee(sys.stderr, spath_stderr_def)
 
-    if show:
-        print(f"\n{'-'*40}\n")
-        print(
-            f"\nStandard Output/Error are going to be logged in the followings: \n  - {spath_stdout}\n  - {spath_stderr}\n"
-        )
-        print(f"\n{'-'*40}\n")
+    if verbose:
+        message = f"Standard Output/Error is being logged at:\n- {spath_stdout}\n- {spath_stderr}"
+        mngs.gen.print_block(message)
+        # print(f"\n{'-'*40}\n")
+        # print(
+        #     f"\nStandard Output/Error are going to be logged in the followings: \n  - {spath_stdout}\n  - {spath_stderr}\n"
+        # )
+        # print(f"\n{'-'*40}\n")
     return sys_stdout, sys_stderr
```

### Comparing `mngs-1.2.3/src/mngs/general/save.py` & `mngs-1.3.0/src/mngs/general/save.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,14 @@
 import warnings
 
 import mngs
 import numpy as np
 import pandas as pd
 import scipy
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.save" will be removed. '
-            'Please use "mngs.io.save" instead.',
-            PendingDeprecationWarning,
-        )
-
 
 def save(obj, sfname_or_spath, makedirs=True, show=True, **kwargs):
     """
     Example
       save(arr, 'data.npy')
       save(df, 'df.csv')
       save(serializable, 'serializable.pkl')
@@ -62,32 +53,31 @@
         sdir = os.path.dirname(spath)
         os.makedirs(sdir, exist_ok=True)
 
     ## Saves
     try:
         ## copy files
         is_copying_files = (
-            isinstance(obj, str) or is_listed_X(obj, str)
-        ) and (isinstance(spath, str) or is_listed_X(spath, str))
+            isinstance(obj, str) or mngs.gen.is_listed_X(obj, str)
+        ) and (isinstance(spath, str) or mngs.gen.is_listed_X(spath, str))
         if is_copying_files:
             mngs.general.copy_files(obj, spath)
 
         # csv
         elif spath.endswith(".csv"):
             if isinstance(obj, pd.DataFrame):  # DataFrame
                 obj.to_csv(spath)
-            if is_listed_X(obj, [int, float]):  # listed scalars
-                save_listed_scalars_as_csv(
+            if mngs.gen.is_listed_X(obj, [int, float]):  # listed scalars
+                _save_listed_scalars_as_csv(
                     obj,
                     spath,
                     **kwargs,
                 )
-            if is_listed_X(obj, pd.DataFrame):  # listed DataFrame
-                # save_listed_dfs_as_csv(obj, spath, indi_suffix=None, overwrite=False)
-                save_listed_dfs_as_csv(obj, spath, **kwargs)
+            if mngs.gen.is_listed_X(obj, pd.DataFrame):  # listed DataFrame
+                _save_listed_dfs_as_csv(obj, spath, **kwargs)
         # numpy
         elif spath.endswith(".npy"):
             np.save(spath, obj)
         # pkl
         elif spath.endswith(".pkl"):
             with open(spath, "wb") as s:  # 'w'
                 pickle.dump(obj, s)
@@ -119,15 +109,15 @@
         elif spath.endswith(".tiff") or spath.endswith(".tif"):
             obj.savefig(
                 spath, dpi=300, format="tiff"
             )  # obj is matplotlib.pyplot object
             del obj
         # mp4
         elif spath.endswith(".mp4"):
-            mk_mp4(obj, spath)  # obj is matplotlib.pyplot.figure object
+            _mk_mp4(obj, spath)  # obj is matplotlib.pyplot.figure object
             del obj
 
         # yaml
         elif spath.endswith(".yaml"):
             from ruamel.yaml import YAML
 
             yaml = YAML()
@@ -189,70 +179,40 @@
             if detector.done:
                 break
     detector.close()
     enc = detector.result["encoding"]
     return enc
 
 
-def is_listed_X(obj, types):
-    """
-    Example:
-        obj = [3, 2, 1, 5]
-        is_listed_X(obj,
-    """
-    import numpy as np
-
-    try:
-        conditions = []
-        condition_list = isinstance(obj, list)
-
-        if not (isinstance(types, list) or isinstance(types, tuple)):
-            types = [types]
-
-        _conditions_susp = []
-        for typ in types:
-            _conditions_susp.append(
-                (np.array([isinstance(o, typ) for o in obj]) == True).all()
-            )
-
-        condition_susp = np.any(_conditions_susp)
-
-        is_listed_X = np.all([condition_list, condition_susp])
-        return is_listed_X
-
-    except:
-        return False
-
-
-def save_listed_scalars_as_csv(
+def _save_listed_scalars_as_csv(
     listed_scalars,
     spath_csv,
     column_name="_",
     indi_suffix=None,
     round=3,
     overwrite=False,
     show=False,
 ):
     """Puts to df and save it as csv"""
     import numpy as np
 
     if overwrite == True:
-        mv_to_tmp(spath_csv, L=2)
+        _mv_to_tmp(spath_csv, L=2)
     indi_suffix = (
         np.arange(len(listed_scalars)) if indi_suffix is None else indi_suffix
     )
     df = pd.DataFrame(
         {"{}".format(column_name): listed_scalars}, index=indi_suffix
     ).round(round)
     df.to_csv(spath_csv)
     if show:
         print("\nSaved to: {}\n".format(spath_csv))
 
 
-def save_listed_dfs_as_csv(
+def _save_listed_dfs_as_csv(
     listed_dfs,
     spath_csv,
     indi_suffix=None,
     overwrite=False,
     show=False,
 ):
     """listed_dfs:
@@ -265,15 +225,15 @@
         At the left top cell on the output csv file, '{}'.format(indi_suffix[i])
         will be added, where i is the index of the df.On the other hand,
         when indi_suffix=None is passed, only '{}'.format(i) will be added.
     """
     import numpy as np
 
     if overwrite == True:
-        mv_to_tmp(spath_csv, L=2)
+        _mv_to_tmp(spath_csv, L=2)
 
     indi_suffix = (
         np.arange(len(listed_dfs)) if indi_suffix is None else indi_suffix
     )
     for i, df in enumerate(listed_dfs):
         with open(spath_csv, mode="a") as f:
             f_writer = csv.writer(f)
@@ -283,15 +243,28 @@
         with open(spath_csv, mode="a") as f:
             f_writer = csv.writer(f)
             f_writer.writerow([""])
     if show:
         print("Saved to: {}".format(spath_csv))
 
 
-def mk_mp4(fig, spath_mp4):
+def _mv_to_tmp(fpath, L=2):
+    import os
+    from shutil import move
+
+    try:
+        tgt_fname = connect_strs_with_hyphens(fpath.split("/")[-L:])
+        tgt_fpath = "/tmp/{}".format(tgt_fname)
+        move(fpath, tgt_fpath)
+        print("Moved to: {}".format(tgt_fpath))
+    except:
+        pass
+
+
+def _mk_mp4(fig, spath_mp4):
     from matplotlib import animation
 
     axes = fig.get_axes()
 
     def init():
         return (fig,)
 
@@ -307,27 +280,14 @@
     writermp4 = animation.FFMpegWriter(
         fps=60, extra_args=["-vcodec", "libx264"]
     )
     anim.save(spath_mp4, writer=writermp4)
     print("\nSaving to: {}\n".format(spath_mp4))
 
 
-def mv_to_tmp(fpath, L=2):
-    import os
-    from shutil import move
-
-    try:
-        tgt_fname = connect_strs_with_hyphens(fpath.split("/")[-L:])
-        tgt_fpath = "/tmp/{}".format(tgt_fname)
-        move(fpath, tgt_fpath)
-        print("Moved to: {}".format(tgt_fpath))
-    except:
-        pass
-
-
 def save_optuna_study_as_csv_and_pngs(study, sdir):
     import optuna
 
     ## Trials DataFrame
     trials_df = study.trials_dataframe()
 
     ## Figures
```

### Comparing `mngs-1.2.3/src/mngs/gists/_SigMacro_processFigure_S.py` & `mngs-1.3.0/src/mngs/gists/_SigMacro_processFigure_S.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/gists/_SigMacro_toBlue.py` & `mngs-1.3.0/src/mngs/gists/_SigMacro_toBlue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/io/load.py` & `mngs-1.3.0/src/mngs/io/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,16 @@
 import mne
 import mngs
 import numpy as np
 import pandas as pd
 import torch
 import yaml
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.load" will be removed. '
-            'Please use "mngs.io.load" instead.',
-            PendingDeprecationWarning,
-        )
-
 
-def load(lpath, show=False, **kwargs):
+def load(lpath, show=False, verbose=False, **kwargs):
     import logging
 
     try:
         extension = "." + lpath.split(".")[-1]  # [REVISED]
 
         # csv
         if extension == ".csv":
@@ -146,22 +137,25 @@
         ]:
             obj = load_eeg_data(lpath, **kwargs)
 
         else:
             print(f"\nNot loaded from: {lpath}\n")
             return None
 
-        if show:
+        if show or verbose:
             print(f"\nLoaded from: {lpath}\n")
 
         return obj
 
     except Exception as e:
-        logging.error(f"\n{lpath} was not loaded:\n{e}")
-        return None
+        if verbose:
+            print(f"\n{lpath} was not loaded:\n{e}")
+
+        # logging.error(f"\n{lpath} was not loaded:\n{e}")
+        # return None
 
 
 def load_eeg_data(filename, **kwargs):
     """
     Load EEG data based on file extension and associated files using MNE-Python.
 
     Parameters:
@@ -287,34 +281,35 @@
     # rdb_raw_bytes_url = "sqlite:////tmp/fake/ywatanabe/_MicroNN_WindowSize-1.0-sec_MaxEpochs_100_2021-1216-1844/optuna_study_test_file#0.db"
     storage = optuna.storages.RDBStorage(url=rdb_raw_bytes_url)
     study = optuna.load_study(study_name=study_name, storage=storage)
     print(f"\nLoaded: {rdb_raw_bytes_url}\n")
     return study
 
 
-def load_configs(IS_DEBUG=None, show=False):
+def load_configs(IS_DEBUG=None, show=False, verbose=False):
+
     if os.getenv("CI") == "true":
         IS_DEBUG = True
 
     def update_debug(config, IS_DEBUG):
         if IS_DEBUG:
             debug_keys = mngs.gen.search("^DEBUG_", list(config.keys()))[1]
             for dk in debug_keys:
                 dk_wo_debug_prefix = dk.split("DEBUG_")[1]
                 config[dk_wo_debug_prefix] = config[dk]
-                if show:
+                if show or verbose:
                     print(f"\n{dk} -> {dk_wo_debug_prefix}\n")
         return config
 
     # Check ./config/IS_DEBUG.yaml file if IS_DEBUG argument is not passed
     if IS_DEBUG is None:
-        try:
-            IS_DEBUG = mngs.io.load("./config/IS_DEBUG.yaml")["IS_DEBUG"]
-        except Exception as e:
-            print(e)
+        IS_DEBUG_PATH = "./config/IS_DEBUG.yaml"
+        if os.path.exists(IS_DEBUG_PATH):
+            IS_DEBUG = mngs.io.load("./config/IS_DEBUG.yaml").get("IS_DEBUG")
+        else:
             IS_DEBUG = False
 
     # Main
     CONFIGS = {}
     for lpath in glob("./config/*.yaml"):
         CONFIG = update_debug(mngs.io.load(lpath), IS_DEBUG)
         CONFIGS.update(CONFIG)
```

### Comparing `mngs-1.2.3/src/mngs/io/path.py` & `mngs-1.3.0/src/mngs/io/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,14 @@
 import re
 import subprocess
 import warnings
 from glob import glob
 
 import mngs
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.path" will be removed. '
-            'Please use "mngs.io.path" instead.',
-            PendingDeprecationWarning,
-        )
-
 
 ################################################################################
 ## PATH
 ################################################################################
 def get_this_fpath(when_ipython="/tmp/fake.py"):
     __file__ = inspect.stack()[1].filename
     if "ipython" in __file__:  # for ipython
@@ -33,16 +24,14 @@
 
 def mk_spath(sfname, makedirs=False):
 
     __file__ = inspect.stack()[1].filename
     if "ipython" in __file__:  # for ipython
         __file__ = f'/tmp/fake-{os.getenv("USER")}.py'
 
-    # __file__ = get_current_file_name()
-
     ## spath
     fpath = __file__
     fdir, fname, _ = split_fpath(fpath)
     sdir = fdir + fname + "/"
     spath = sdir + sfname
 
     if makedirs:
```

### Comparing `mngs-1.2.3/src/mngs/io/save.py` & `mngs-1.3.0/src/mngs/io/save.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,14 @@
 import warnings
 
 import mngs
 import numpy as np
 import pandas as pd
 import scipy
 
-if "general" in __file__:
-    with warnings.catch_warnings():
-        warnings.simplefilter("always")
-        warnings.warn(
-            '\n"mngs.general.save" will be removed. '
-            'Please use "mngs.io.save" instead.',
-            PendingDeprecationWarning,
-        )
-
 
 def save(obj, sfname_or_spath, makedirs=True, show=True, **kwargs):
     """
     Example
       save(arr, 'data.npy')
       save(df, 'df.csv')
       save(serializable, 'serializable.pkl')
@@ -62,32 +53,31 @@
         sdir = os.path.dirname(spath)
         os.makedirs(sdir, exist_ok=True)
 
     ## Saves
     try:
         ## copy files
         is_copying_files = (
-            isinstance(obj, str) or is_listed_X(obj, str)
-        ) and (isinstance(spath, str) or is_listed_X(spath, str))
+            isinstance(obj, str) or mngs.gen.is_listed_X(obj, str)
+        ) and (isinstance(spath, str) or mngs.gen.is_listed_X(spath, str))
         if is_copying_files:
             mngs.general.copy_files(obj, spath)
 
         # csv
         elif spath.endswith(".csv"):
             if isinstance(obj, pd.DataFrame):  # DataFrame
                 obj.to_csv(spath)
-            if is_listed_X(obj, [int, float]):  # listed scalars
-                save_listed_scalars_as_csv(
+            if mngs.gen.is_listed_X(obj, [int, float]):  # listed scalars
+                _save_listed_scalars_as_csv(
                     obj,
                     spath,
                     **kwargs,
                 )
-            if is_listed_X(obj, pd.DataFrame):  # listed DataFrame
-                # save_listed_dfs_as_csv(obj, spath, indi_suffix=None, overwrite=False)
-                save_listed_dfs_as_csv(obj, spath, **kwargs)
+            if mngs.gen.is_listed_X(obj, pd.DataFrame):  # listed DataFrame
+                _save_listed_dfs_as_csv(obj, spath, **kwargs)
         # numpy
         elif spath.endswith(".npy"):
             np.save(spath, obj)
         # pkl
         elif spath.endswith(".pkl"):
             with open(spath, "wb") as s:  # 'w'
                 pickle.dump(obj, s)
@@ -119,15 +109,15 @@
         elif spath.endswith(".tiff") or spath.endswith(".tif"):
             obj.savefig(
                 spath, dpi=300, format="tiff"
             )  # obj is matplotlib.pyplot object
             del obj
         # mp4
         elif spath.endswith(".mp4"):
-            mk_mp4(obj, spath)  # obj is matplotlib.pyplot.figure object
+            _mk_mp4(obj, spath)  # obj is matplotlib.pyplot.figure object
             del obj
 
         # yaml
         elif spath.endswith(".yaml"):
             from ruamel.yaml import YAML
 
             yaml = YAML()
@@ -189,70 +179,40 @@
             if detector.done:
                 break
     detector.close()
     enc = detector.result["encoding"]
     return enc
 
 
-def is_listed_X(obj, types):
-    """
-    Example:
-        obj = [3, 2, 1, 5]
-        is_listed_X(obj,
-    """
-    import numpy as np
-
-    try:
-        conditions = []
-        condition_list = isinstance(obj, list)
-
-        if not (isinstance(types, list) or isinstance(types, tuple)):
-            types = [types]
-
-        _conditions_susp = []
-        for typ in types:
-            _conditions_susp.append(
-                (np.array([isinstance(o, typ) for o in obj]) == True).all()
-            )
-
-        condition_susp = np.any(_conditions_susp)
-
-        is_listed_X = np.all([condition_list, condition_susp])
-        return is_listed_X
-
-    except:
-        return False
-
-
-def save_listed_scalars_as_csv(
+def _save_listed_scalars_as_csv(
     listed_scalars,
     spath_csv,
     column_name="_",
     indi_suffix=None,
     round=3,
     overwrite=False,
     show=False,
 ):
     """Puts to df and save it as csv"""
     import numpy as np
 
     if overwrite == True:
-        mv_to_tmp(spath_csv, L=2)
+        _mv_to_tmp(spath_csv, L=2)
     indi_suffix = (
         np.arange(len(listed_scalars)) if indi_suffix is None else indi_suffix
     )
     df = pd.DataFrame(
         {"{}".format(column_name): listed_scalars}, index=indi_suffix
     ).round(round)
     df.to_csv(spath_csv)
     if show:
         print("\nSaved to: {}\n".format(spath_csv))
 
 
-def save_listed_dfs_as_csv(
+def _save_listed_dfs_as_csv(
     listed_dfs,
     spath_csv,
     indi_suffix=None,
     overwrite=False,
     show=False,
 ):
     """listed_dfs:
@@ -265,15 +225,15 @@
         At the left top cell on the output csv file, '{}'.format(indi_suffix[i])
         will be added, where i is the index of the df.On the other hand,
         when indi_suffix=None is passed, only '{}'.format(i) will be added.
     """
     import numpy as np
 
     if overwrite == True:
-        mv_to_tmp(spath_csv, L=2)
+        _mv_to_tmp(spath_csv, L=2)
 
     indi_suffix = (
         np.arange(len(listed_dfs)) if indi_suffix is None else indi_suffix
     )
     for i, df in enumerate(listed_dfs):
         with open(spath_csv, mode="a") as f:
             f_writer = csv.writer(f)
@@ -283,15 +243,28 @@
         with open(spath_csv, mode="a") as f:
             f_writer = csv.writer(f)
             f_writer.writerow([""])
     if show:
         print("Saved to: {}".format(spath_csv))
 
 
-def mk_mp4(fig, spath_mp4):
+def _mv_to_tmp(fpath, L=2):
+    import os
+    from shutil import move
+
+    try:
+        tgt_fname = connect_strs_with_hyphens(fpath.split("/")[-L:])
+        tgt_fpath = "/tmp/{}".format(tgt_fname)
+        move(fpath, tgt_fpath)
+        print("Moved to: {}".format(tgt_fpath))
+    except:
+        pass
+
+
+def _mk_mp4(fig, spath_mp4):
     from matplotlib import animation
 
     axes = fig.get_axes()
 
     def init():
         return (fig,)
 
@@ -307,27 +280,14 @@
     writermp4 = animation.FFMpegWriter(
         fps=60, extra_args=["-vcodec", "libx264"]
     )
     anim.save(spath_mp4, writer=writermp4)
     print("\nSaving to: {}\n".format(spath_mp4))
 
 
-def mv_to_tmp(fpath, L=2):
-    import os
-    from shutil import move
-
-    try:
-        tgt_fname = connect_strs_with_hyphens(fpath.split("/")[-L:])
-        tgt_fpath = "/tmp/{}".format(tgt_fname)
-        move(fpath, tgt_fpath)
-        print("Moved to: {}".format(tgt_fpath))
-    except:
-        pass
-
-
 def save_optuna_study_as_csv_and_pngs(study, sdir):
     import optuna
 
     ## Trials DataFrame
     trials_df = study.trials_dataframe()
 
     ## Figures
```

### Comparing `mngs-1.2.3/src/mngs/linalg/_misc.py` & `mngs-1.3.0/src/mngs/linalg/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/ClassificationReporter.py` & `mngs-1.3.0/src/mngs/ml/ClassificationReporter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/ClassifierServer.py` & `mngs-1.3.0/src/mngs/ml/ClassifierServer.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/EarlyStopping.py` & `mngs-1.3.0/src/mngs/ml/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/LearningCurveLogger.py` & `mngs-1.3.0/src/mngs/ml/LearningCurveLogger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/__Classifiers.py` & `mngs-1.3.0/src/mngs/ml/__Classifiers.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/clustering/_UMAP.py` & `mngs-1.3.0/src/mngs/ml/clustering/_UMAP.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/clustering/_umap.py` & `mngs-1.3.0/src/mngs/ml/clustering/_umap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-1.3.0/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-1.3.0/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/metrics/_bACC.py` & `mngs-1.3.0/src/mngs/ml/metrics/_bACC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/optim/_get_set.py` & `mngs-1.3.0/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/_conf_mat.py` & `mngs-1.3.0/src/mngs/ml/plt/_conf_mat.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/_learning_curve.py` & `mngs-1.3.0/src/mngs/ml/plt/_learning_curve.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/_optuna_study.py` & `mngs-1.3.0/src/mngs/ml/plt/_optuna_study.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/aucs/example.py` & `mngs-1.3.0/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-1.3.0/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/plt/aucs/roc_auc.py` & `mngs-1.3.0/src/mngs/ml/plt/aucs/roc_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/silhoute_score_block.py` & `mngs-1.3.0/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/sk/_clf.py` & `mngs-1.3.0/src/mngs/ml/sk/_clf.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/sk/_to_sktime.py` & `mngs-1.3.0/src/mngs/ml/sk/_to_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-1.3.0/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_LabelEncoder.py` & `mngs-1.3.0/src/mngs/ml/utils/_LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_check_params.py` & `mngs-1.3.0/src/mngs/ml/utils/_check_params.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-1.3.0/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_merge_labels.py` & `mngs-1.3.0/src/mngs/ml/utils/_merge_labels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/ml/utils/_under_sample.py` & `mngs-1.3.0/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/mngs/setup.py` & `mngs-1.3.0/src/mngs/mngs/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_AxiswiseDropout.py` & `mngs-1.3.0/src/mngs/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_BNet.py` & `mngs-1.3.0/src/mngs/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_BNet_Res.py` & `mngs-1.3.0/src/mngs/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_ChannelGainChanger.py` & `mngs-1.3.0/src/mngs/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_DropoutChannels.py` & `mngs-1.3.0/src/mngs/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_Filters.py` & `mngs-1.3.0/src/mngs/nn/_Wavelet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,230 +1,171 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 04:06:50 (ywatanabe)"
+# Time-stamp: "2024-04-11 22:28:40 (ywatanabe)"
 
-import math
-import warnings
 
 import mngs
 import numpy as np
-import seaborn as sns
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mngs.general import torch_fn
 
 
-class BaseFilter1D(nn.Module):
+class Wavelet(nn.Module):
     def __init__(
-        self,
+        self, samp_rate, kernel_size=None, freq_scale="linear", out_scale="log"
     ):
         super().__init__()
+        self.register_buffer("dummy", torch.tensor(0))
         self.kernel = None
+        self.init_kernel(
+            samp_rate, kernel_size=kernel_size, freq_scale=freq_scale
+        )
+        self.out_scale = out_scale
 
-    @property
-    def kernel_size(
-        self,
-    ):
-        return mngs.gen.to_even(self.kernel.shape[-1])
-
-    @property
-    def radius(
-        self,
-    ):
-        return self.kernel_size // 2
-
-    def forward(self, x, t=None):
-        """Apply the filter to input signal x with shape: (batch_size, n_chs, seq_len)"""
-
-        x = mngs.dsp.ensure_3d(x)
+    def forward(self, x):
+        """Apply the 2D filter (n_filts, kernel_size) to input signal x with shape: (batch_size, n_chs, seq_len)"""
+        x = mngs.dsp.ensure_3d(x).to(self.dummy.device)
         seq_len = x.shape[-1]
 
         # Ensure the kernel is initialized
         if self.kernel is None:
             self.init_kernel()
             if self.kernel is None:
                 raise ValueError("Filter kernel has not been initialized.")
+        assert self.kernel.ndim == 2
+        self.kernel = self.kernel.to(x.device)  # cuda, torch.complex128
 
         # Edge handling and convolution
         extension_length = self.radius
         first_segment = x[:, :, :extension_length].flip(dims=[-1])
         last_segment = x[:, :, -extension_length:].flip(dims=[-1])
         extended_x = torch.cat([first_segment, x, last_segment], dim=-1)
 
-        channels = extended_x.size(1)
+        # working??
+        kernel_batched = self.kernel.unsqueeze(1)
+        extended_x_reshaped = extended_x.view(-1, 1, extended_x.shape[-1])
 
-        kernel = (
-            self.kernel.expand(channels, 1, -1)
-            .to(extended_x.device)
-            .to(extended_x.dtype)
+        filtered_x_real = F.conv1d(
+            extended_x_reshaped, kernel_batched.real.float(), groups=1
+        )
+        filtered_x_imag = F.conv1d(
+            extended_x_reshaped, kernel_batched.imag.float(), groups=1
         )
 
-        x_filted_extended = F.conv1d(
-            extended_x, kernel, padding=0, groups=channels
-        )[..., :seq_len]
-
-        assert x.shape == x_filted_extended.shape
-
-        # # Remove edges
-        # x_filted_extended[..., : self.radius] *= 0
-        # x_filted_extended[..., -self.radius :] *= 0
-
-        nn_remove = x_filted_extended.shape[-1] // 4
-        x_filted_extended = x_filted_extended[..., nn_remove:-nn_remove]
-        return x_filted_extended
-
-
-class GaussianFilter(BaseFilter1D):
-    def __init__(self, sigma):
-        super().__init__()
-        self.sigma = mngs.gen.to_even(sigma)
-        self.init_kernel()
-
-    def init_kernel(self):
-        # Create a Gaussian kernel
-        kernel_size = self.sigma * 6  # +/- 3SD
-        kernel_range = torch.arange(kernel_size) - kernel_size // 2
-        kernel = torch.exp(-0.5 * (kernel_range / self.sigma) ** 2)
-        kernel /= kernel.sum()  # Normalize the kernel
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
-
+        filtered_x = torch.view_as_complex(
+            torch.stack([filtered_x_real, filtered_x_imag], dim=-1)
+        )
 
-class LowPassFilter(BaseFilter1D):
-    def __init__(self, cutoff_hz, fs, kernel_size=None):
-        super().__init__()
-        self.cutoff_hz = cutoff_hz
-        self.fs = fs
+        filtered_x = filtered_x.view(
+            x.shape[0], x.shape[1], kernel_batched.shape[0], -1
+        )
+        filtered_x = filtered_x.view(
+            x.shape[0], x.shape[1], kernel_batched.shape[0], -1
+        )
+        filtered_x = filtered_x[..., :seq_len]
+        assert filtered_x.shape[-1] == seq_len
 
-        kernel_size = (
-            mngs.gen.to_even(int(1 / cutoff_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[
-            freqs <= self.cutoff_hz
-        ] = 1  # Allow frequencies below the cutoff
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.abs().sum()  # Normalize the kernel by its absolute sum
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+        pha = filtered_x.angle()
+        amp = filtered_x.abs()
 
+        if self.out_scale == "log":
+            return torch.log(pha + 1e-5), torch.log(amp + 1e-5), self.freqs
+        else:
+            return pha, amp, self.freqs
 
-class HighPassFilter(BaseFilter1D):
-    def __init__(self, cutoff_hz, fs, kernel_size=None):
-        super().__init__()
-        self.cutoff_hz = cutoff_hz
-        self.fs = fs
-        kernel_size = (
-            mngs.gen.to_even(int(1 / cutoff_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[
-            freqs >= self.cutoff_hz
-        ] = 1  # Allow frequencies above the cutoff
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.abs().sum()  # Normalize the kernel by its absolute sum
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+    def init_kernel(self, samp_rate, kernel_size=None, freq_scale="log"):
+        device = self.dummy.device
+        morlets, freqs = self.gen_morlet_to_nyquist(
+            samp_rate, kernel_size=kernel_size, freq_scale=freq_scale
+        )
+        self.kernel = torch.tensor(morlets).to(device)
+        self.freqs = torch.tensor(freqs).float().to(device)
 
+    @staticmethod
+    def gen_morlet_to_nyquist(
+        samp_rate, kernel_size=None, freq_scale="linear"
+    ):
+        """
+        Generates Morlet wavelets for exponentially increasing frequency bands up to the Nyquist frequency.
 
-class BandPassFilter(BaseFilter1D):
-    def __init__(self, low_hz, high_hz, fs, kernel_size=None):
-        super().__init__()
+        Parameters:
+        - samp_rate (int): The sampling rate of the signal, in Hertz.
+        - kernel_size (int): The size of the kernel, in number of samples.
+
+        Returns:
+        - np.ndarray: A 2D array of complex values representing the Morlet wavelets for each frequency band.
+        """
+        if kernel_size is None:
+            kernel_size = int(samp_rate)  # * 2.5)
+
+        nyquist_freq = samp_rate / 2
+
+        # Log freq_scale
+        def calc_freq_boundaries_log(nyquist_freq):
+            n_kernels = int(np.floor(np.log2(nyquist_freq)))
+            mid_hz = np.array([2 ** (n + 1) for n in range(n_kernels)])
+            width_hz = np.hstack([np.array([1]), np.diff(mid_hz) / 2]) + 1
+            low_hz = mid_hz - width_hz
+            high_hz = mid_hz + width_hz
+            low_hz[0] = 0.1
+            return low_hz, high_hz
+
+        def calc_freq_boundaries_linear(nyquist_freq):
+            n_kernels = int(nyquist_freq)
+            high_hz = np.linspace(1, nyquist_freq, n_kernels)
+            low_hz = high_hz - np.hstack([np.array(1), np.diff(high_hz)])
+            low_hz[0] = 0.1
+            return low_hz, high_hz
+
+        if freq_scale == "linear":
+            fn = calc_freq_boundaries_linear
+        if freq_scale == "log":
+            fn = calc_freq_boundaries_log
+        low_hz, high_hz = fn(nyquist_freq)
+
+        morlets = []
+        freqs = []
+
+        for _, (ll, hh) in enumerate(zip(low_hz, high_hz)):
+            if ll > nyquist_freq:
+                break
+
+            center_frequency = (ll + hh) / 2
+
+            t = np.arange(-kernel_size // 2, kernel_size // 2) / samp_rate
+            # Calculate standard deviation of the gaussian window for a given center frequency
+            sigma = 7 / (2 * np.pi * center_frequency)
+            sine_wave = np.exp(2j * np.pi * center_frequency * t)
+            gaussian_window = np.exp(-(t**2) / (2 * sigma**2))
+            morlet_wavelet = sine_wave * gaussian_window
 
-        assert 0 < low_hz
-        assert low_hz < high_hz
-        assert high_hz <= fs / 2
-
-        kernel_size = (
-            mngs.gen.to_even(int(1 / low_hz * fs * 3))
-            # mngs.gen.to_even(int(low_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-
-        self.low_hz = low_hz
-        self.high_hz = high_hz
-        self.fs = fs
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.zeros(kernel_size)
-        kernel[(self.low_hz <= freqs) & (freqs <= self.high_hz)] = 1
-        kernel = torch.fft.ifft(kernel).real
-        # kernel /= kernel.sum()
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+            freqs.append(center_frequency)
+            morlets.append(morlet_wavelet)
 
+        return np.array(morlets), np.array(freqs)
 
-class BandStopFilter(BaseFilter1D):
-    def __init__(self, low_hz, high_hz, fs, kernel_size=None):
-        super().__init__()
-        kernel_size = (
-            mngs.gen.to_even(int(1 / low_hz * fs * 3))
-            # mngs.gen.to_even(int(low_hz * fs * 3))
-            if kernel_size is None
-            else mngs.gen.to_even(kernel_size)
-        )
-        self.low_hz = low_hz
-        self.high_hz = high_hz
-        self.fs = fs
-        self.init_kernel(kernel_size)
-
-    def init_kernel(self, kernel_size):
-        freqs = torch.fft.fftfreq(kernel_size, d=1 / self.fs)
-        kernel = torch.ones(kernel_size)
-        kernel[(freqs >= self.low_hz) & (freqs <= self.high_hz)] = 0
-        kernel = torch.fft.ifft(
-            kernel
-        ).real  # Inverse FFT to get the time-domain kernel
-        # kernel /= kernel.sum()  # Normalize the kernel
-        self.kernel = kernel.unsqueeze(0).unsqueeze(0)
+    @property
+    def kernel_size(
+        self,
+    ):
+        return mngs.gen.to_even(self.kernel.shape[-1])
 
+    @property
+    def radius(
+        self,
+    ):
+        return mngs.gen.to_even(self.kernel_size // 2)
 
-class HanningFilter(BaseFilter1D):
-    def __init__(self, window_size):
-        super().__init__()
-        self.window_size = mngs.gen.to_even(int(window_size))
-        self.init_kernel()
 
-    def init_kernel(self):
-        # Create a Hanning window
-        self.kernel = (
-            torch.hann_window(self.window_size).unsqueeze(0).unsqueeze(0)
-        )
+if __name__ == "__main__":
+    import mngs
 
-    def forward(self, x):
-        """Apply the Hanning window to input signal x with shape: (batch_size, n_chs, seq_len)"""
+    xx, tt, fs = mngs.dsp.demo_sig(sig_type="chirp")
 
-        x = mngs.dsp.ensure_3d(x)
-        seq_len = x.shape[-1]
+    ww, ff = mngs.dsp.wavelet(xx, fs)
 
-        # Check if the input signal is longer than the window size
-        if seq_len < self.window_size:
-            raise ValueError(
-                "Input signal length must be greater than the window size."
-            )
-
-        # Apply the window to the signal
-        # Assuming that we want to apply the window to the central part of the signal
-        start = (seq_len - self.window_size) // 2
-        end = start + self.window_size
-        windowed_x = x.clone()  # Create a copy of x to apply window
-        windowed_x[:, :, start:end] *= self.kernel.to(x.device).to(x.dtype)
-
-        return windowed_x
-
-
-# @torch_fn
-# def hanning(x, window_size):
-#     return HanningFilter(window_size)(x)
+    fig, ax = mngs.plt.subplots()
+    ax.imshow2d(ww[0, 0].T)
+    ax = mngs.plt.ax.set_ticks(ax, xticks=tt, yticks=ff)
+    ax = mngs.plt.ax.set_n_ticks(ax)
+    plt.show()
```

### Comparing `mngs-1.2.3/src/mngs/nn/_FreqGainChanger.py` & `mngs-1.3.0/src/mngs/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_GaussianFilter.py` & `mngs-1.3.0/src/mngs/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_MNet_1000.py` & `mngs-1.3.0/src/mngs/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_ModulationIndex.py` & `mngs-1.3.0/src/mngs/nn/_ModulationIndex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 11:30:02 (ywatanabe)"
+# Time-stamp: "2024-04-12 23:51:57 (ywatanabe)"
 
+"""
+This script does XYZ.
+"""
 
+# Imports
 import math
+import sys
 import time
 
+import mngs
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mngs.general import torch_fn
 
+# Config
+CONFIG = mngs.gen.load_configs()
 
+# Functions
 class ModulationIndex(nn.Module):
-    def __init__(self, n_bins=18):
+    def __init__(self, n_bins=18, fp16=False):
         super(ModulationIndex, self).__init__()
         self.n_bins = n_bins
+        self.fp16 = fp16
         self.register_buffer(
             "pha_bin_cutoffs", torch.linspace(-np.pi, np.pi, n_bins + 1)
         )
 
     def forward(self, pha, amp, epsilon=1e-9):
         """
         Compute the Modulation Index based on phase (pha) and amplitude (amp) tensors.
@@ -32,15 +42,19 @@
                               (batch_size, n_channels, n_freqs_amp, n_segments, sequence_length).
 
         Returns:
         - MI (torch.Tensor): The Modulation Index for each batch and channel.
         """
         assert pha.ndim == amp.ndim == 5
 
-        pha, amp = pha.float().contiguous(), amp.float().contiguous()
+        if self.fp16:
+            pha, amp = pha.half().contiguous(), amp.half().contiguous()
+        else:
+            pha, amp = pha.float().contiguous(), amp.float().contiguous()
+
         device = pha.device
 
         pha_masks = self._phase_to_masks(pha, self.pha_bin_cutoffs.to(device))
         # (batch_size, n_channels, n_freqs_pha, n_segments, sequence_length, n_bins)
 
         # Expands amp and masks to utilize broadcasting
         i_batch = 0
@@ -64,20 +78,21 @@
         amp_probs = amp_means / (
             amp_means.sum(dim=-1, keepdims=True) + epsilon
         )
 
         MI = (
             torch.log(torch.tensor(self.n_bins, device=device) + epsilon)
             + (amp_probs * (amp_probs + epsilon).log()).sum(dim=-1)
-        ) / (
-            torch.log(torch.tensor(self.n_bins, device=device) + epsilon)
-            + epsilon
-        )
+        ) / torch.log(torch.tensor(self.n_bins, device=device))
+
+        # Squeeze the n_bin dimension
+        MI = MI.squeeze(-1)
 
-        MI = MI.squeeze(-1).mean(axis=-1)
+        # Takes mean along the n_segments dimension
+        MI = MI.mean(axis=-1)
 
         if MI.isnan().any():
             raise ValueError(
                 "NaN values detected in Modulation Index calculation."
             )
 
         return MI
@@ -97,98 +112,68 @@
         one_hot_masks = F.one_hot(
             bin_indices,
             num_classes=n_bins,
         )
         return one_hot_masks
 
 
-def plot_comodulogram_tensorpac(xx, fs, t_sec):
-    # Morlet's Wavelet Transfrmation
-    p = tensorpac.Pac(f_pha="hres", f_amp="hres", dcomplex="wavelet")
-
-    # Bandpass Filtering and Hilbert Transformation
-    i_batch, i_ch = 0, 0
-    phases = p.filter(
-        fs, xx[i_batch, i_ch], ftype="phase", n_jobs=1
-    )  # (50, 20, 2048)
-    amplitudes = p.filter(
-        fs, xx[i_batch, i_ch], ftype="amplitude", n_jobs=1
-    )  # (50, 20, 2048)
-
-    # Calculates xpac
-    k = 2
-    p.idpac = (k, 0, 0)
-    xpac = p.fit(phases, amplitudes)  # (50, 50, 20)
-    pac = xpac.mean(axis=-1)  # (50, 50)
-
-    ## Plot
-    fig, ax = plt.subplots()
-    ax = p.comodulogram(
-        pac, title=p.method.replace(" (", f" ({k})\n("), cmap="viridis"
+def _reshape(x, batch_size=2, n_chs=4):
+    return (
+        torch.tensor(x)
+        .float()
+        .unsqueeze(0)
+        .unsqueeze(0)
+        .repeat(batch_size, n_chs, 1, 1, 1)
     )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    freqs_amp = p.f_amp.mean(axis=-1)
-    freqs_pha = p.f_pha.mean(axis=-1)
-
-    return phases, amplitudes, freqs_pha, freqs_amp
-    # return phases and amplitudes for future use in my implementation
-    # as the aim of this code is to confirm the calculation of Modulation Index only
-    # without considering bandpass filtering and hilbert transformation.
-
-
-def reshape_pha_amp(pha, amp, batch_size=2, n_chs=4):
-    pha = torch.tensor(pha).half()
-    amp = torch.tensor(amp).half()
-    pha = pha.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    amp = amp.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    return pha, amp
-
-
-@torch_fn
-def modulation_index(pha, amp, n_bins=18):
-    return ModulationIndex(n_bins=18)(pha, amp)
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
     import mngs
     import seaborn as sns
     import tensorpac
     from tensorpac import Pac
     from tqdm import tqdm
 
+    # Start
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(
+        sys, plt, fig_scale=3
+    )
+
     # Parameters
-    fs = 128
-    t_sec = 5
+    FS = 512
+    T_SEC = 5
 
     # Demo signal
-    xx, tt, fs = mngs.dsp.demo_sig(fs=fs, t_sec=t_sec, sig_type="tensorpac")
+    xx, tt, fs = mngs.dsp.demo_sig(fs=FS, t_sec=T_SEC, sig_type="tensorpac")
     # xx.shape: (8, 19, 20, 512)
 
     # Tensorpac
-    pha, amp, freqs_pha, freqs_amp = plot_comodulogram_tensorpac(
-        xx, fs, t_sec=t_sec
-    )
-    # mngs.io.save((pha, amp, freqs_pha, freqs_amp), "/tmp/out.pkl")
-    # pha, amp, freqs_pha, freqs_amp = mngs.io.load("/tmp/out.pkl")
-
-    # GPU calculation
-    pha, amp = reshape_pha_amp(pha, amp)
-    pac = mngs.dsp.modulation_index(pha, amp)
-
-    ## Convert y-axis
+    (
+        pha,
+        amp,
+        freqs_pha,
+        freqs_amp,
+        pac_tp,
+    ) = mngs.dsp.utils.pac.calc_pac_with_tensorpac(xx, fs, t_sec=T_SEC)
+
+    # GPU calculation with mngs.dsp.nn.ModulationIndex
+    pha, amp = _reshape(pha), _reshape(amp)
+    pac_mngs = mngs.dsp.modulation_index(pha, amp).cpu().numpy()
     i_batch, i_ch = 0, 0
+    pac_mngs = pac_mngs[i_batch, i_ch]
 
-    fig, ax = mngs.plt.subplots()
-    ax.imshow2d(
-        pac[i_batch, i_ch].cpu().numpy(),
-        cbar_label="PAC values",
+    # Plots
+    fig = mngs.dsp.utils.pac.plot_PAC_mngs_vs_tensorpac(
+        pac_mngs, pac_tp, freqs_pha, freqs_amp
     )
-    ax = mngs.plt.ax.set_ticks(
-        ax, xticks=freqs_pha.astype(int), yticks=freqs_amp.astype(int)
-    )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    ax.set_xlabel("Frequency for phase [Hz]")
-    ax.set_ylabel("Frequency for amplitude [Hz]")
-    ax.set_title("GPU calculation")
+    # fig = plot_PAC_mngs_vs_tensorpac(pac_mngs, pac_tp, freqs_pha, freqs_amp)
+    mngs.io.save(fig, CONFIG["SDIR"] + "modulation_index.png")  # plt.show()
+
+    # Close
+    mngs.gen.close(CONFIG)
+
+# EOF
 
-    plt.show()
+"""
+/home/ywatanabe/proj/entrance/mngs/nn/_ModulationIndex.py
+"""
```

### Comparing `mngs-1.2.3/src/mngs/nn/_PAC_working.py` & `mngs-1.3.0/src/mngs/nn/_PAC_working.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_PSD.py` & `mngs-1.3.0/src/mngs/nn/_PSD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 19:03:07 (ywatanabe)"
+# Time-stamp: "2024-04-11 21:50:09 (ywatanabe)"
 
 import torch
 import torch.nn as nn
 
 
 class PSD(nn.Module):
     def __init__(self, sample_rate, prob=False, dim=-1):
```

### Comparing `mngs-1.2.3/src/mngs/nn/_ResNet1D.py` & `mngs-1.3.0/src/mngs/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_SpatialAttention.py` & `mngs-1.3.0/src/mngs/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_Spectrogram.py` & `mngs-1.3.0/src/mngs/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/_SwapChannels.py` & `mngs-1.3.0/src/mngs/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/nn/__init__.py` & `mngs-1.3.0/src/mngs/nn/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 12:51:19 (ywatanabe)"
+# Time-stamp: "2024-04-12 19:55:23 (ywatanabe)"
 
 from ._AxiswiseDropout import AxiswiseDropout
-
-# from ._BandPassFilter import BandPassFilter
 from ._BNet import BNet, BNet_config
 from ._ChannelGainChanger import ChannelGainChanger
 from ._DropoutChannels import DropoutChannels
-
-# from ._GaussianFilter import GaussianFilter
 from ._Filters import (
     BandPassFilter,
     BandStopFilter,
+    DifferentiableBandPassFilter,
     GaussianFilter,
     HighPassFilter,
     LowPassFilter,
 )
 from ._FreqGainChanger import FreqGainChanger
 from ._Hilbert import Hilbert
```

### Comparing `mngs-1.2.3/src/mngs/os/_mv.py` & `mngs-1.3.0/src/mngs/os/_mv.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_add_hue.py` & `mngs-1.3.0/src/mngs/plt/_add_hue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_annotated_heatmap.py` & `mngs-1.3.0/src/mngs/plt/_annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_configure_mpl.py` & `mngs-1.3.0/src/mngs/plt/_configure_mpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 17:07:26 (ywatanabe)"
+# Time-stamp: "2024-04-10 11:00:31 (ywatanabe)"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 
 def rgba_to_hex(rgba):
@@ -35,17 +35,17 @@
     font_size_title=8,
     font_size_axis_label=8,
     font_size_tick_label=7,
     font_size_legend=6,
     # Hide spines
     hide_top_right_spines=True,
     # line
-    line_width=0.1,
+    line_width=0.5,
     # Color transparency
-    alpha=0.75,
+    alpha=0.9,
     # Whether to print configurations or not
     verbose=False,
     **kwargs,
 ):
     """
     Configures Matplotlib and Seaborn settings for publication-quality plots.
     For axis control, refer to the mngs.plt.ax module.
```

### Comparing `mngs-1.2.3/src/mngs/plt/_draw_a_cube.py` & `mngs-1.3.0/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-1.3.0/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_mk_colorbar.py` & `mngs-1.3.0/src/mngs/plt/_mk_colorbar.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/_tpl.py` & `mngs-1.3.0/src/mngs/plt/_tpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_circular_hist.py` & `mngs-1.3.0/src/mngs/plt/ax/_circular_hist.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_extend.py` & `mngs-1.3.0/src/mngs/plt/ax/_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_hide_spines.py` & `mngs-1.3.0/src/mngs/plt/ax/_hide_spines.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_map_ticks.py` & `mngs-1.3.0/src/mngs/plt/ax/_map_ticks.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_panel.py` & `mngs-1.3.0/src/mngs/plt/ax/_panel.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_sci_note.py` & `mngs-1.3.0/src/mngs/plt/ax/_sci_note.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/ax/_set_pos.py` & `mngs-1.3.0/src/mngs/plt/ax/_set_pos.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/colors.py` & `mngs-1.3.0/src/mngs/plt/colors.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/plt/get_mpl_color.py` & `mngs-1.3.0/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/resource/get.py` & `mngs-1.3.0/src/mngs/resource/get.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/resource/limit_RAM.py` & `mngs-1.3.0/src/mngs/resource/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/__init__.py` & `mngs-1.3.0/src/mngs/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_bonferroni_correction.py` & `mngs-1.3.0/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_brunner_munzel_test.py` & `mngs-1.3.0/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_corr_test.py` & `mngs-1.3.0/src/mngs/stats/_corr_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_fdr_correction.py` & `mngs-1.3.0/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_general.py` & `mngs-1.3.0/src/mngs/stats/_general.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_multicompair.py` & `mngs-1.3.0/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_nocorrelation_test.py` & `mngs-1.3.0/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/stats/_smirnov_grubbs.py` & `mngs-1.3.0/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs/torch/_apply_to.py` & `mngs-1.3.0/src/mngs/torch/_apply_to.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.3/src/mngs.egg-info/SOURCES.txt` & `mngs-1.3.0/src/mngs.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 src/mngs.egg-info/dependency_links.txt
 src/mngs.egg-info/requires.txt
 src/mngs.egg-info/top_level.txt
 src/mngs/dsp/PARAMS.py
 src/mngs/dsp/__init__.py
 src/mngs/dsp/_demo_sig.py
 src/mngs/dsp/_hilbert.py
+src/mngs/dsp/_listen.py
 src/mngs/dsp/_misc.py
 src/mngs/dsp/_mne.py
 src/mngs/dsp/_modulation_index.py
 src/mngs/dsp/_pac.py
 src/mngs/dsp/_psd.py
 src/mngs/dsp/_resample.py
 src/mngs/dsp/_transform.py
 src/mngs/dsp/_wavelet.py
 src/mngs/dsp/add_noise.py
 src/mngs/dsp/example.py
 src/mngs/dsp/filt.py
 src/mngs/dsp/norm.py
-src/mngs/dsp/ref.py
-src/mngs/dsp/fx/__init__.py
+src/mngs/dsp/reference.py
+src/mngs/dsp/template.py
 src/mngs/dsp/nn/_AxiswiseDropout.py
 src/mngs/dsp/nn/_BNet.py
 src/mngs/dsp/nn/_BNet_Res.py
 src/mngs/dsp/nn/_ChannelGainChanger.py
 src/mngs/dsp/nn/_DropoutChannels.py
 src/mngs/dsp/nn/_Filters.py
 src/mngs/dsp/nn/_FreqGainChanger.py
@@ -44,34 +45,41 @@
 src/mngs/dsp/nn/_ResNet1D.py
 src/mngs/dsp/nn/_SpatialAttention.py
 src/mngs/dsp/nn/_Spectrogram.py
 src/mngs/dsp/nn/_SwapChannels.py
 src/mngs/dsp/nn/_TransposeLayer.py
 src/mngs/dsp/nn/_Wavelet.py
 src/mngs/dsp/nn/__init__.py
+src/mngs/dsp/utils/__init__.py
+src/mngs/dsp/utils/_differential_bandpass_filters.py
+src/mngs/dsp/utils/_ensure_even_len.py
+src/mngs/dsp/utils/_zero_pad.py
+src/mngs/dsp/utils/filter.py
+src/mngs/dsp/utils/pac.py
 src/mngs/general/_TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_close.py
 src/mngs/general/_converters.py
 src/mngs/general/_cuda_collect_env.py
+src/mngs/general/_embed.py
 src/mngs/general/_norm.py
+src/mngs/general/_paste.py
 src/mngs/general/_reload.py
+src/mngs/general/_reproduce.py
 src/mngs/general/_shell.py
 src/mngs/general/_start.py
 src/mngs/general/_xml2dict.py
 src/mngs/general/email.py
 src/mngs/general/latex.py
 src/mngs/general/load.py
 src/mngs/general/mat2py.py
 src/mngs/general/misc.py
 src/mngs/general/pandas.py
 src/mngs/general/path.py
-src/mngs/general/repro.py
 src/mngs/general/save.py
-src/mngs/general/torch.py
 src/mngs/gists/_SigMacro_processFigure_S.py
 src/mngs/gists/_SigMacro_toBlue.py
 src/mngs/gists/__init__.py
 src/mngs/io/__init__.py
 src/mngs/io/load.py
 src/mngs/io/path.py
 src/mngs/io/save.py
```

