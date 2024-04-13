# Comparing `tmp/mngs-1.3.0.tar.gz` & `tmp/mngs-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-1.3.0.tar", last modified: Fri Apr 12 16:59:36 2024, max compression
+gzip compressed data, was "mngs-1.3.1.tar", last modified: Sat Apr 13 08:10:30 2024, max compression
```

## Comparing `mngs-1.3.0.tar` & `mngs-1.3.1.tar`

### file list

```diff
@@ -1,234 +1,257 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:30:42.000000 mngs-1.3.0/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.3.0/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      914 2024-04-12 16:59:36.899178 mngs-1.3.0/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      289 2024-04-12 16:59:09.000000 mngs-1.3.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-12 16:59:36.903178 mngs-1.3.0/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.887178 mngs-1.3.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.888178 mngs-1.3.0/src/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      541 2024-04-12 16:56:31.000000 mngs-1.3.0/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.889178 mngs-1.3.0/src/mngs/dsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.3.0/src/mngs/dsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      476 2024-04-12 06:37:09.000000 mngs-1.3.0/src/mngs/dsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8264 2024-04-12 15:58:47.000000 mngs-1.3.0/src/mngs/dsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-04-12 16:24:37.000000 mngs-1.3.0/src/mngs/dsp/_hilbert.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2298 2024-04-12 06:33:44.000000 mngs-1.3.0/src/mngs/dsp/_listen.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.3.0/src/mngs/dsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.3.0/src/mngs/dsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1847 2024-04-12 16:39:54.000000 mngs-1.3.0/src/mngs/dsp/_modulation_index.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4134 2024-04-12 16:40:18.000000 mngs-1.3.0/src/mngs/dsp/_pac.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2315 2024-04-12 15:32:38.000000 mngs-1.3.0/src/mngs/dsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1653 2024-04-12 16:35:11.000000 mngs-1.3.0/src/mngs/dsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1663 2024-04-08 02:41:59.000000 mngs-1.3.0/src/mngs/dsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2549 2024-04-12 14:51:36.000000 mngs-1.3.0/src/mngs/dsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2875 2024-04-12 15:18:24.000000 mngs-1.3.0/src/mngs/dsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6150 2024-04-05 14:36:19.000000 mngs-1.3.0/src/mngs/dsp/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3701 2024-04-12 16:49:23.000000 mngs-1.3.0/src/mngs/dsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.891178 mngs-1.3.0/src/mngs/dsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.0/src/mngs/dsp/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.0/src/mngs/dsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.0/src/mngs/dsp/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.0/src/mngs/dsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.0/src/mngs/dsp/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.0/src/mngs/dsp/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.0/src/mngs/dsp/nn/_PAC_working.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.0/src/mngs/dsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.0/src/mngs/dsp/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/dsp/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.0/src/mngs/dsp/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.0/src/mngs/dsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.0/src/mngs/dsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.3.0/src/mngs/dsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.3.0/src/mngs/dsp/reference.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      438 2024-04-10 05:57:54.000000 mngs-1.3.0/src/mngs/dsp/template.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.891178 mngs-1.3.0/src/mngs/dsp/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      349 2024-04-12 09:54:43.000000 mngs-1.3.0/src/mngs/dsp/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3338 2024-04-12 10:11:47.000000 mngs-1.3.0/src/mngs/dsp/utils/_differential_bandpass_filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      201 2024-04-10 01:59:50.000000 mngs-1.3.0/src/mngs/dsp/utils/_ensure_even_len.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      548 2024-04-10 22:26:21.000000 mngs-1.3.0/src/mngs/dsp/utils/_zero_pad.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13225 2024-04-12 16:04:54.000000 mngs-1.3.0/src/mngs/dsp/utils/filter.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3212 2024-04-11 11:36:33.000000 mngs-1.3.0/src/mngs/dsp/utils/pac.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.892178 mngs-1.3.0/src/mngs/general/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.3.0/src/mngs/general/_TimeStamper.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-04-12 00:56:17.000000 mngs-1.3.0/src/mngs/general/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2255 2024-04-10 09:53:27.000000 mngs-1.3.0/src/mngs/general/_close.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-10 22:17:57.000000 mngs-1.3.0/src/mngs/general/_converters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_cuda_collect_env.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1947 2024-04-12 00:46:27.000000 mngs-1.3.0/src/mngs/general/_embed.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.3.0/src/mngs/general/_norm.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      695 2024-04-12 01:01:58.000000 mngs-1.3.0/src/mngs/general/_paste.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4315 2024-04-10 07:23:22.000000 mngs-1.3.0/src/mngs/general/_reload.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4094 2024-04-10 09:44:58.000000 mngs-1.3.0/src/mngs/general/_reproduce.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_shell.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4525 2024-04-12 13:27:12.000000 mngs-1.3.0/src/mngs/general/_start.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/_xml2dict.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/email.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/latex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.0/src/mngs/general/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/mat2py.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22771 2024-04-10 07:34:26.000000 mngs-1.3.0/src/mngs/general/misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/general/pandas.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.0/src/mngs/general/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.0/src/mngs/general/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.892178 mngs-1.3.0/src/mngs/gists/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/_SigMacro_processFigure_S.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/_SigMacro_toBlue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/gists/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/io/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      485 2024-04-10 07:36:15.000000 mngs-1.3.0/src/mngs/io/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.0/src/mngs/io/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.0/src/mngs/io/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.0/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/linalg/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/linalg/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/linalg/_misc.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/ClassificationReporter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/ClassifierServer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.3.0/src/mngs/ml/EarlyStopping.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/LearningCurveLogger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/__Classifiers.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.3.0/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/act/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/act/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/clustering/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.3.0/src/mngs/ml/clustering/_UMAP.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.3.0/src/mngs/ml/clustering/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.3.0/src/mngs/ml/clustering/_umap.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.893178 mngs-1.3.0/src/mngs/ml/layer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/_Pass.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/loss/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/MultiTaskLoss.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/_L1L2Losses.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/metrics/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.3.0/src/mngs/ml/metrics/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.3.0/src/mngs/ml/metrics/_bACC.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.894178 mngs-1.3.0/src/mngs/ml/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.3.0/src/mngs/ml/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.3.0/src/mngs/ml/plt/_conf_mat.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.3.0/src/mngs/ml/plt/_learning_curve.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.3.0/src/mngs/ml/plt/_optuna_study.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/plt/aucs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/plt/aucs/roc_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/sk/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.3.0/src/mngs/ml/sk/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.3.0/src/mngs/ml/sk/_clf.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.3.0/src/mngs/ml/sk/_to_sktime.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/ml/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_DefaultDataset.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.3.0/src/mngs/ml/utils/_LabelEncoder.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.3.0/src/mngs/ml/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.3.0/src/mngs/ml/utils/_check_params.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.3.0/src/mngs/ml/utils/_merge_labels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_sliding_window_data_augmentation.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_under_sample.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.895178 mngs-1.3.0/src/mngs/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/mngs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/mngs/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.0/src/mngs/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.0/src/mngs/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.0/src/mngs/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.0/src/mngs/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.0/src/mngs/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.0/src/mngs/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.0/src/mngs/nn/_PAC_working.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.0/src/mngs/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.0/src/mngs/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.0/src/mngs/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.0/src/mngs/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.0/src/mngs/nn/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/os/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.3.0/src/mngs/os/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1379 2024-04-05 22:00:45.000000 mngs-1.3.0/src/mngs/os/_mv.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.897178 mngs-1.3.0/src/mngs/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.3.0/src/mngs/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_add_hue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_annotated_heatmap.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5826 2024-04-10 01:00:32.000000 mngs-1.3.0/src/mngs/plt/_configure_mpl.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_draw_a_cube.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_get_RGBA_from_colormap.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_mk_colorbar.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/_mk_patches.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    11703 2024-04-12 14:36:46.000000 mngs-1.3.0/src/mngs/plt/_subplots.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.3.0/src/mngs/plt/_tpl.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.898178 mngs-1.3.0/src/mngs/plt/ax/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:34:39.000000 mngs-1.3.0/src/mngs/plt/ax/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_circular_hist.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_extend.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_fill_between.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.3.0/src/mngs/plt/ax/_hide_spines.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_map_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_panel.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_sci_note.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:15:04.000000 mngs-1.3.0/src/mngs/plt/ax/_set_n_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.3.0/src/mngs/plt/ax/_set_pos.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/ax/_set_size.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      401 2024-04-07 04:39:32.000000 mngs-1.3.0/src/mngs/plt/ax/_set_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/colors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.898178 mngs-1.3.0/src/mngs/resource/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/get.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/src/mngs/stats/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.3.0/src/mngs/stats/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_bonferroni_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_brunner_munzel_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_calc_partial_corr.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_corr_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_fdr_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.3.0/src/mngs/stats/_general.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_multicompair.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_smirnov_grubbs.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.3.0/src/mngs/stats/_to_asterisks.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.899178 mngs-1.3.0/src/mngs/torch/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.3.0/src/mngs/torch/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.3.0/src/mngs/torch/_apply_to.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-12 16:59:36.888178 mngs-1.3.0/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      914 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6094 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      433 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-12 16:59:36.000000 mngs-1.3.0/src/mngs.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.481493 mngs-1.3.1/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:30:42.000000 mngs-1.3.1/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.3.1/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1344 2024-04-13 08:10:30.481493 mngs-1.3.1/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-04-13 08:01:23.000000 mngs-1.3.1/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-13 08:10:30.481493 mngs-1.3.1/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.1/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.468493 mngs-1.3.1/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.469493 mngs-1.3.1/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      463 2024-04-13 08:10:09.000000 mngs-1.3.1/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.470493 mngs-1.3.1/src/mngs/dsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.3.1/src/mngs/dsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      476 2024-04-12 06:37:09.000000 mngs-1.3.1/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8264 2024-04-12 15:58:47.000000 mngs-1.3.1/src/mngs/dsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-04-12 16:24:37.000000 mngs-1.3.1/src/mngs/dsp/_hilbert.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2298 2024-04-12 06:33:44.000000 mngs-1.3.1/src/mngs/dsp/_listen.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.3.1/src/mngs/dsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.3.1/src/mngs/dsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1847 2024-04-12 16:39:54.000000 mngs-1.3.1/src/mngs/dsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4134 2024-04-12 16:40:18.000000 mngs-1.3.1/src/mngs/dsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2315 2024-04-12 15:32:38.000000 mngs-1.3.1/src/mngs/dsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1653 2024-04-12 16:35:11.000000 mngs-1.3.1/src/mngs/dsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1663 2024-04-08 02:41:59.000000 mngs-1.3.1/src/mngs/dsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2549 2024-04-12 14:51:36.000000 mngs-1.3.1/src/mngs/dsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2875 2024-04-13 02:10:11.000000 mngs-1.3.1/src/mngs/dsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6150 2024-04-05 14:36:19.000000 mngs-1.3.1/src/mngs/dsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3746 2024-04-12 17:46:41.000000 mngs-1.3.1/src/mngs/dsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.472493 mngs-1.3.1/src/mngs/dsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.1/src/mngs/dsp/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.1/src/mngs/dsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.1/src/mngs/dsp/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.1/src/mngs/dsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.1/src/mngs/dsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.1/src/mngs/dsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.1/src/mngs/dsp/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.1/src/mngs/dsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.1/src/mngs/dsp/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/dsp/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.1/src/mngs/dsp/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.1/src/mngs/dsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.1/src/mngs/dsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.3.1/src/mngs/dsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.3.1/src/mngs/dsp/reference.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      438 2024-04-10 05:57:54.000000 mngs-1.3.1/src/mngs/dsp/template.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.472493 mngs-1.3.1/src/mngs/dsp/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      349 2024-04-12 09:54:43.000000 mngs-1.3.1/src/mngs/dsp/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3338 2024-04-12 10:11:47.000000 mngs-1.3.1/src/mngs/dsp/utils/_differential_bandpass_filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      201 2024-04-10 01:59:50.000000 mngs-1.3.1/src/mngs/dsp/utils/_ensure_even_len.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      548 2024-04-10 22:26:21.000000 mngs-1.3.1/src/mngs/dsp/utils/_zero_pad.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13225 2024-04-12 16:04:54.000000 mngs-1.3.1/src/mngs/dsp/utils/filter.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3212 2024-04-11 11:36:33.000000 mngs-1.3.1/src/mngs/dsp/utils/pac.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.473493 mngs-1.3.1/src/mngs/gen/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.3.1/src/mngs/gen/_TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1363 2024-04-13 04:23:18.000000 mngs-1.3.1/src/mngs/gen/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2255 2024-04-10 09:53:27.000000 mngs-1.3.1/src/mngs/gen/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-10 22:17:57.000000 mngs-1.3.1/src/mngs/gen/_converters.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1947 2024-04-12 00:46:27.000000 mngs-1.3.1/src/mngs/gen/_embed.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.3.1/src/mngs/gen/_norm.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      695 2024-04-12 01:01:58.000000 mngs-1.3.1/src/mngs/gen/_paste.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4315 2024-04-10 07:23:22.000000 mngs-1.3.1/src/mngs/gen/_reload.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4094 2024-04-10 09:44:58.000000 mngs-1.3.1/src/mngs/gen/_reproduce.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4525 2024-04-12 13:27:12.000000 mngs-1.3.1/src/mngs/gen/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.1/src/mngs/gen/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22777 2024-04-13 03:13:13.000000 mngs-1.3.1/src/mngs/gen/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gen/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.1/src/mngs/gen/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.1/src/mngs/gen/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.474493 mngs-1.3.1/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.3.1/src/mngs/general/_TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1363 2024-04-13 04:23:18.000000 mngs-1.3.1/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2255 2024-04-10 09:53:27.000000 mngs-1.3.1/src/mngs/general/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-10 22:17:57.000000 mngs-1.3.1/src/mngs/general/_converters.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1947 2024-04-12 00:46:27.000000 mngs-1.3.1/src/mngs/general/_embed.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.3.1/src/mngs/general/_norm.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      695 2024-04-12 01:01:58.000000 mngs-1.3.1/src/mngs/general/_paste.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4315 2024-04-10 07:23:22.000000 mngs-1.3.1/src/mngs/general/_reload.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4094 2024-04-10 09:44:58.000000 mngs-1.3.1/src/mngs/general/_reproduce.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4525 2024-04-12 13:27:12.000000 mngs-1.3.1/src/mngs/general/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.1/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22777 2024-04-13 03:13:13.000000 mngs-1.3.1/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.1/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.1/src/mngs/general/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.474493 mngs-1.3.1/src/mngs/gists/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gists/_SigMacro_processFigure_S.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gists/_SigMacro_toBlue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/gists/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.474493 mngs-1.3.1/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      485 2024-04-10 07:36:15.000000 mngs-1.3.1/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9708 2024-04-10 08:40:45.000000 mngs-1.3.1/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5350 2024-04-10 08:22:30.000000 mngs-1.3.1/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8977 2024-04-10 07:35:39.000000 mngs-1.3.1/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.475493 mngs-1.3.1/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.475493 mngs-1.3.1/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.3.1/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/__Classifiers.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.3.1/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.475493 mngs-1.3.1/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.475493 mngs-1.3.1/src/mngs/ml/clustering/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.3.1/src/mngs/ml/clustering/_UMAP.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.3.1/src/mngs/ml/clustering/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.3.1/src/mngs/ml/clustering/_umap.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.475493 mngs-1.3.1/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/metrics/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.3.1/src/mngs/ml/metrics/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.3.1/src/mngs/ml/metrics/_bACC.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.476493 mngs-1.3.1/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.3.1/src/mngs/ml/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.3.1/src/mngs/ml/plt/_conf_mat.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.3.1/src/mngs/ml/plt/_learning_curve.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.3.1/src/mngs/ml/plt/_optuna_study.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.477493 mngs-1.3.1/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.477493 mngs-1.3.1/src/mngs/ml/sk/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.3.1/src/mngs/ml/sk/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.3.1/src/mngs/ml/sk/_clf.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.3.1/src/mngs/ml/sk/_to_sktime.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.477493 mngs-1.3.1/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/utils/_DefaultDataset.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.3.1/src/mngs/ml/utils/_LabelEncoder.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.3.1/src/mngs/ml/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.3.1/src/mngs/ml/utils/_check_params.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.3.1/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/utils/_sliding_window_data_augmentation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.477493 mngs-1.3.1/src/mngs/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/mngs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/mngs/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.478493 mngs-1.3.1/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.3.1/src/mngs/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    12234 2024-04-12 13:29:54.000000 mngs-1.3.1/src/mngs/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.3.1/src/mngs/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1291 2024-04-11 00:17:15.000000 mngs-1.3.1/src/mngs/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4867 2024-04-12 13:51:57.000000 mngs-1.3.1/src/mngs/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8752 2024-04-12 13:29:16.000000 mngs-1.3.1/src/mngs/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.3.1/src/mngs/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-11 11:50:09.000000 mngs-1.3.1/src/mngs/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.3.1/src/mngs/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.3.1/src/mngs/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5702 2024-04-11 12:28:40.000000 mngs-1.3.1/src/mngs/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      902 2024-04-12 09:55:23.000000 mngs-1.3.1/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.478493 mngs-1.3.1/src/mngs/os/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.3.1/src/mngs/os/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1379 2024-04-05 22:00:45.000000 mngs-1.3.1/src/mngs/os/_mv.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.479493 mngs-1.3.1/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.3.1/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5826 2024-04-10 01:00:32.000000 mngs-1.3.1/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    11703 2024-04-12 14:36:46.000000 mngs-1.3.1/src/mngs/plt/_subplots.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.3.1/src/mngs/plt/_tpl.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.480493 mngs-1.3.1/src/mngs/plt/ax/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:34:39.000000 mngs-1.3.1/src/mngs/plt/ax/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.3.1/src/mngs/plt/ax/_hide_spines.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_map_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_panel.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_sci_note.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:15:04.000000 mngs-1.3.1/src/mngs/plt/ax/_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.3.1/src/mngs/plt/ax/_set_pos.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/ax/_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      401 2024-04-07 04:39:32.000000 mngs-1.3.1/src/mngs/plt/ax/_set_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.480493 mngs-1.3.1/src/mngs/res/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      193 2024-04-13 07:55:03.000000 mngs-1.3.1/src/mngs/res/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6683 2024-04-13 08:05:09.000000 mngs-1.3.1/src/mngs/res/_info.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.480493 mngs-1.3.1/src/mngs/res/_utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      174 2024-04-13 07:56:05.000000 mngs-1.3.1/src/mngs/res/_utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15837 2024-04-13 07:48:42.000000 mngs-1.3.1/src/mngs/res/_utils/_cuda_collect_env.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/res/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.481493 mngs-1.3.1/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.3.1/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.3.1/src/mngs/stats/_general.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.3.1/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.481493 mngs-1.3.1/src/mngs/torch/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.3.1/src/mngs/torch/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.3.1/src/mngs/torch/_apply_to.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-13 08:10:30.469493 mngs-1.3.1/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1344 2024-04-13 08:10:30.000000 mngs-1.3.1/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6586 2024-04-13 08:10:30.000000 mngs-1.3.1/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-13 08:10:30.000000 mngs-1.3.1/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      433 2024-04-13 08:10:30.000000 mngs-1.3.1/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-13 08:10:30.000000 mngs-1.3.1/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-1.3.0/LICENSE` & `mngs-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/PKG-INFO` & `mngs-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.3.0
+Version: 1.3.1
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
-Description: ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
+Description: # monogusa (= lazy in Japanese)
+        mngs is Python utilities for ML and DSP projects
+        
+        ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
+        
+        ![Hard Working Sloth](./docs/hard_working_sloth.jpg)
         
         ## Installation
         ``` bash
         $ pip install mngs
         ```
         
         ## Galleries
-        [`mngs.dsp`](https://github.com/ywatanabe1989/mngs/tree/develop/src/mngs/dsp#readme)
+        - [`mngs.dsp`](https://github.com/ywatanabe1989/mngs/tree/main/src/mngs/dsp#readme)
+          Digital Signal Processing
+        - [`mngs.res`](https://github.com/ywatanabe1989/mngs/tree/main/src/mngs/res#readme)
+          Resource
+        
+        - mngs.general
+        - mngs.io
+        - mngs.plt
+        - mngs.ml
+        - mngs.stats
         
         ## Contact
         Yusuke Watanabe (ywata1989@gmail.com).
         
         
 Keywords: utils,utilities,python,machine learning
 Platform: UNKNOWN
```

### Comparing `mngs-1.3.0/setup.py` & `mngs-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/PARAMS.py` & `mngs-1.3.1/src/mngs/dsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_demo_sig.py` & `mngs-1.3.1/src/mngs/dsp/_demo_sig.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_hilbert.py` & `mngs-1.3.1/src/mngs/dsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_listen.py` & `mngs-1.3.1/src/mngs/dsp/_listen.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_misc.py` & `mngs-1.3.1/src/mngs/dsp/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_mne.py` & `mngs-1.3.1/src/mngs/dsp/_mne.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_modulation_index.py` & `mngs-1.3.1/src/mngs/dsp/_modulation_index.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_pac.py` & `mngs-1.3.1/src/mngs/dsp/_pac.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_psd.py` & `mngs-1.3.1/src/mngs/dsp/_psd.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_resample.py` & `mngs-1.3.1/src/mngs/dsp/_resample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_transform.py` & `mngs-1.3.1/src/mngs/dsp/_transform.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/_wavelet.py` & `mngs-1.3.1/src/mngs/dsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/add_noise.py` & `mngs-1.3.1/src/mngs/dsp/add_noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!./env/bin/python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-13 01:18:23 (ywatanabe)"
+# Time-stamp: "2024-04-13 12:10:10 (ywatanabe)"
 
 """
 Functions to add noise to signals.
 """
 
 # Imports
 import sys
```

### Comparing `mngs-1.3.0/src/mngs/dsp/example.py` & `mngs-1.3.1/src/mngs/dsp/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/filt.py` & `mngs-1.3.1/src/mngs/dsp/filt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!./env/bin/python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-13 02:49:22 (ywatanabe)"
+# Time-stamp: "2024-04-13 03:46:40 (ywatanabe)"
 
 
 import mngs
 import numpy as np
 from mngs.general import torch_fn
 from mngs.nn import (
     BandPassFilter,
@@ -48,22 +48,22 @@
     import sys
 
     import matplotlib.pyplot as plt
     import mngs
     import torch
 
     # Start
-    CONFIG, sys.stdout, sys.stderr, plt, cc = mngs.gen.start(sys, plt)
+    CONFIG, sys.stdout, sys.stderr, plt, CC = mngs.gen.start(sys, plt)
 
     # Parametes
     T_SEC = 1
     SRC_FS = 1024
-    FREQS_HZ = list(np.linspace(0, 500, 10, endpoint=False))
+    FREQS_HZ = list(np.linspace(0, 500, 10, endpoint=False).astype(int))
     SIG_TYPE = "periodic"
-    BANDS = np.vstack([[80, 300]])
+    BANDS = np.vstack([[80, 310]])
     SIGMA = 3
 
     # Demo Signal
     xx, tt, fs = mngs.dsp.demo_sig(
         t_sec=T_SEC,
         fs=SRC_FS,
         freqs_hz=FREQS_HZ,
@@ -131,22 +131,22 @@
         elif _psd.ndim == 4:
             _psd = _psd[i_batch, i_ch, i_filt]
 
         ax.plot(ff, _psd, label=k)
         ax.legend(loc="upper left")
 
         for bb in np.hstack(BANDS):
-            ax.axvlines(x=bb, color="gray", line_style="--")
+            ax.axvline(x=bb, color=CC["grey"], linestyle="--")
 
-    fig.suptitle("Filtered")
+    fig.suptitle("PSD (power spectrum density) of filtered signals")
     fig.supxlabel("Frequency [Hz]")
-    fig.supylabel("Power Spectral Density")
+    fig.supylabel("log(Power [uV^2 / Hz]) [a.u.]")
     mngs.io.save(fig, "psd.png")
 
     # Close
     mngs.gen.close(CONFIG)
 
-    """
-    /home/ywatanabe/proj/mngs/src/mngs/dsp/filt.py
-    """
+# EOF
 
-    # EOF
+"""
+/home/ywatanabe/proj/mngs/src/mngs/dsp/filt.py
+"""
```

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_AxiswiseDropout.py` & `mngs-1.3.1/src/mngs/dsp/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_BNet.py` & `mngs-1.3.1/src/mngs/dsp/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_BNet_Res.py` & `mngs-1.3.1/src/mngs/dsp/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_ChannelGainChanger.py` & `mngs-1.3.1/src/mngs/dsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_DropoutChannels.py` & `mngs-1.3.1/src/mngs/dsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_Filters.py` & `mngs-1.3.1/src/mngs/dsp/nn/_Filters.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_FreqGainChanger.py` & `mngs-1.3.1/src/mngs/dsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_GaussianFilter.py` & `mngs-1.3.1/src/mngs/dsp/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_Hilbert.py` & `mngs-1.3.1/src/mngs/dsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_MNet_1000.py` & `mngs-1.3.1/src/mngs/dsp/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_ModulationIndex.py` & `mngs-1.3.1/src/mngs/dsp/nn/_ModulationIndex.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_PAC.py` & `mngs-1.3.1/src/mngs/dsp/nn/_PAC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_PAC_working.py` & `mngs-1.3.1/src/mngs/dsp/nn/_PAC_working.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_PSD.py` & `mngs-1.3.1/src/mngs/dsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_ResNet1D.py` & `mngs-1.3.1/src/mngs/dsp/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_SpatialAttention.py` & `mngs-1.3.1/src/mngs/dsp/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_Spectrogram.py` & `mngs-1.3.1/src/mngs/dsp/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_SwapChannels.py` & `mngs-1.3.1/src/mngs/dsp/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/_Wavelet.py` & `mngs-1.3.1/src/mngs/dsp/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/nn/__init__.py` & `mngs-1.3.1/src/mngs/dsp/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/reference.py` & `mngs-1.3.1/src/mngs/dsp/reference.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/utils/_differential_bandpass_filters.py` & `mngs-1.3.1/src/mngs/dsp/utils/_differential_bandpass_filters.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/utils/_zero_pad.py` & `mngs-1.3.1/src/mngs/dsp/utils/_zero_pad.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/utils/filter.py` & `mngs-1.3.1/src/mngs/dsp/utils/filter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/dsp/utils/pac.py` & `mngs-1.3.1/src/mngs/dsp/utils/pac.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_TimeStamper.py` & `mngs-1.3.1/src/mngs/gen/_TimeStamper.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/__init__.py` & `mngs-1.3.1/src/mngs/gen/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,48 +14,47 @@
 
 # Confirmed
 from ._paste import paste
 from ._reload import reload
 
 _ = None
 from ..io.__init__ import *
-from ._cuda_collect_env import main as cuda_collect_env
 from ._norm import to_z
 from ._reproduce import fix_seeds, gen_ID, gen_timestamp, tee
 from ._shell import run_shellcommand, run_shellscript
 from ._start import start
 from ._TimeStamper import TimeStamper
 from .email import notify, send_gmail
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
 
 # from .mat2py import *
+from .misc import color_text  # fmt_size,
 from .misc import (
     _return_counting_process,
-    color_text,
     connect_nums,
     connect_strs,
     copy_files,
     copy_the_file,
     ct,
     decapitalize,
     describe,
-    fmt_size,
     grep,
     is_defined_global,
     is_defined_local,
     is_later_or_equal,
     is_listed_X,
     is_nan,
     isclose,
     listed_dict,
     merge_dicts_wo_overlaps,
     mv_col,
     partial_at,
     pop_keys,
     print_block,
+    readable_bytes,
     search,
     squeeze_spaces,
     suppress_output,
     symlink,
     take_the_closest,
     to_even,
     to_odd,
```

### Comparing `mngs-1.3.0/src/mngs/general/_close.py` & `mngs-1.3.1/src/mngs/gen/_close.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_converters.py` & `mngs-1.3.1/src/mngs/gen/_converters.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_cuda_collect_env.py` & `mngs-1.3.1/src/mngs/res/_utils/_cuda_collect_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 #!/usr/bin/env python3
 
 # This script outputs relevant system environment info
 # Run it with `python collect_env.py`.
 import locale
+import os
 import re
 import subprocess
 import sys
-import os
 from collections import namedtuple
 
 try:
     import torch
+
     TORCH_AVAILABLE = True
 except (ImportError, NameError, AttributeError, OSError):
     TORCH_AVAILABLE = False
 
 # System Environment Information
-SystemEnv = namedtuple('SystemEnv', [
-    'torch_version',
-    'is_debug_build',
-    'cuda_compiled_version',
-    'gcc_version',
-    'clang_version',
-    'cmake_version',
-    'os',
-    'python_version',
-    'is_cuda_available',
-    'cuda_runtime_version',
-    'nvidia_driver_version',
-    'nvidia_gpu_models',
-    'cudnn_version',
-    'pip_version',  # 'pip' or 'pip3'
-    'pip_packages',
-    'conda_packages',
-    'hip_compiled_version',
-    'hip_runtime_version',
-    'miopen_runtime_version',
-])
+SystemEnv = namedtuple(
+    "SystemEnv",
+    [
+        "torch_version",
+        "is_debug_build",
+        "cuda_compiled_version",
+        "gcc_version",
+        "clang_version",
+        "cmake_version",
+        "os",
+        "python_version",
+        "is_cuda_available",
+        "cuda_runtime_version",
+        "nvidia_driver_version",
+        "nvidia_gpu_models",
+        "cudnn_version",
+        "pip_version",  # 'pip' or 'pip3'
+        "pip_packages",
+        "conda_packages",
+        "hip_compiled_version",
+        "hip_runtime_version",
+        "miopen_runtime_version",
+    ],
+)
 
 
 def run(command):
     """Returns (return-code, stdout, stderr)"""
-    p = subprocess.Popen(command, stdout=subprocess.PIPE,
-                         stderr=subprocess.PIPE, shell=True)
+    p = subprocess.Popen(
+        command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+    )
     raw_output, raw_err = p.communicate()
     rc = p.returncode
-    if get_platform() == 'win32':
-        enc = 'oem'
+    if get_platform() == "win32":
+        enc = "oem"
     else:
         enc = locale.getpreferredencoding()
     output = raw_output.decode(enc)
     err = raw_err.decode(enc)
     return rc, output.strip(), err.strip()
 
 
@@ -70,239 +75,286 @@
     match = re.search(regex, out)
     if match is None:
         return None
     return match.group(1)
 
 
 def get_conda_packages(run_lambda):
-    if get_platform() == 'win32':
-        system_root = os.environ.get('SYSTEMROOT', 'C:\\Windows')
-        findstr_cmd = os.path.join(system_root, 'System32', 'findstr')
-        grep_cmd = r'{} /R "torch numpy cudatoolkit soumith mkl magma"'.format(findstr_cmd)
+    if get_platform() == "win32":
+        system_root = os.environ.get("SYSTEMROOT", "C:\\Windows")
+        findstr_cmd = os.path.join(system_root, "System32", "findstr")
+        grep_cmd = r'{} /R "torch numpy cudatoolkit soumith mkl magma"'.format(
+            findstr_cmd
+        )
     else:
         grep_cmd = r'grep "torch\|numpy\|cudatoolkit\|soumith\|mkl\|magma"'
-    conda = os.environ.get('CONDA_EXE', 'conda')
-    out = run_and_read_all(run_lambda, conda + ' list | ' + grep_cmd)
+    conda = os.environ.get("CONDA_EXE", "conda")
+    out = run_and_read_all(run_lambda, conda + " list | " + grep_cmd)
     if out is None:
         return out
     # Comment starting at beginning of line
-    comment_regex = re.compile(r'^#.*\n')
-    return re.sub(comment_regex, '', out)
+    comment_regex = re.compile(r"^#.*\n")
+    return re.sub(comment_regex, "", out)
 
 
 def get_gcc_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'gcc --version', r'gcc (.*)')
+    return run_and_parse_first_match(run_lambda, "gcc --version", r"gcc (.*)")
+
 
 def get_clang_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'clang --version', r'clang version (.*)')
+    return run_and_parse_first_match(
+        run_lambda, "clang --version", r"clang version (.*)"
+    )
 
 
 def get_cmake_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'cmake --version', r'cmake (.*)')
+    return run_and_parse_first_match(
+        run_lambda, "cmake --version", r"cmake (.*)"
+    )
 
 
 def get_nvidia_driver_version(run_lambda):
-    if get_platform() == 'darwin':
-        cmd = 'kextstat | grep -i cuda'
-        return run_and_parse_first_match(run_lambda, cmd,
-                                         r'com[.]nvidia[.]CUDA [(](.*?)[)]')
+    if get_platform() == "darwin":
+        cmd = "kextstat | grep -i cuda"
+        return run_and_parse_first_match(
+            run_lambda, cmd, r"com[.]nvidia[.]CUDA [(](.*?)[)]"
+        )
     smi = get_nvidia_smi()
-    return run_and_parse_first_match(run_lambda, smi, r'Driver Version: (.*?) ')
+    return run_and_parse_first_match(
+        run_lambda, smi, r"Driver Version: (.*?) "
+    )
 
 
 def get_gpu_info(run_lambda):
-    if get_platform() == 'darwin' or (TORCH_AVAILABLE and hasattr(torch.version, 'hip') and torch.version.hip is not None):
+    if get_platform() == "darwin" or (
+        TORCH_AVAILABLE
+        and hasattr(torch.version, "hip")
+        and torch.version.hip is not None
+    ):
         if TORCH_AVAILABLE and torch.cuda.is_available():
             return torch.cuda.get_device_name(None)
         return None
     smi = get_nvidia_smi()
-    uuid_regex = re.compile(r' \(UUID: .+?\)')
-    rc, out, _ = run_lambda(smi + ' -L')
+    uuid_regex = re.compile(r" \(UUID: .+?\)")
+    rc, out, _ = run_lambda(smi + " -L")
     if rc != 0:
         return None
     # Anonymize GPUs by removing their UUID
-    return re.sub(uuid_regex, '', out)
+    return re.sub(uuid_regex, "", out)
 
 
 def get_running_cuda_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'nvcc --version', r'release .+ V(.*)')
+    return run_and_parse_first_match(
+        run_lambda, "nvcc --version", r"release .+ V(.*)"
+    )
 
 
 def get_cudnn_version(run_lambda):
     """This will return a list of libcudnn.so; it's hard to tell which one is being used"""
-    if get_platform() == 'win32':
-        system_root = os.environ.get('SYSTEMROOT', 'C:\\Windows')
-        cuda_path = os.environ.get('CUDA_PATH', "%CUDA_PATH%")
-        where_cmd = os.path.join(system_root, 'System32', 'where')
+    if get_platform() == "win32":
+        system_root = os.environ.get("SYSTEMROOT", "C:\\Windows")
+        cuda_path = os.environ.get("CUDA_PATH", "%CUDA_PATH%")
+        where_cmd = os.path.join(system_root, "System32", "where")
         cudnn_cmd = '{} /R "{}\\bin" cudnn*.dll'.format(where_cmd, cuda_path)
-    elif get_platform() == 'darwin':
+    elif get_platform() == "darwin":
         # CUDA libraries and drivers can be found in /usr/local/cuda/. See
         # https://docs.nvidia.com/cuda/cuda-installation-guide-mac-os-x/index.html#install
         # https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#installmac
         # Use CUDNN_LIBRARY when cudnn library is installed elsewhere.
-        cudnn_cmd = 'ls /usr/local/cuda/lib/libcudnn*'
+        cudnn_cmd = "ls /usr/local/cuda/lib/libcudnn*"
     else:
         cudnn_cmd = 'ldconfig -p | grep libcudnn | rev | cut -d" " -f1 | rev'
     rc, out, _ = run_lambda(cudnn_cmd)
     # find will return 1 if there are permission errors or if not found
     if len(out) == 0 or (rc != 1 and rc != 0):
-        l = os.environ.get('CUDNN_LIBRARY')
+        l = os.environ.get("CUDNN_LIBRARY")
         if l is not None and os.path.isfile(l):
             return os.path.realpath(l)
         return None
     files_set = set()
-    for fn in out.split('\n'):
+    for fn in out.split("\n"):
         fn = os.path.realpath(fn)  # eliminate symbolic links
         if os.path.isfile(fn):
             files_set.add(fn)
     if not files_set:
         return None
     # Alphabetize the result because the order is non-deterministic otherwise
     files = list(sorted(files_set))
     if len(files) == 1:
         return files[0]
-    result = '\n'.join(files)
-    return 'Probably one of the following:\n{}'.format(result)
+    result = "\n".join(files)
+    return "Probably one of the following:\n{}".format(result)
 
 
 def get_nvidia_smi():
     # Note: nvidia-smi is currently available only on Windows and Linux
-    smi = 'nvidia-smi'
-    if get_platform() == 'win32':
-        system_root = os.environ.get('SYSTEMROOT', 'C:\\Windows')
-        program_files_root = os.environ.get('PROGRAMFILES', 'C:\\Program Files')
-        legacy_path = os.path.join(program_files_root, 'NVIDIA Corporation', 'NVSMI', smi)
-        new_path = os.path.join(system_root, 'System32', smi)
+    smi = "nvidia-smi"
+    if get_platform() == "win32":
+        system_root = os.environ.get("SYSTEMROOT", "C:\\Windows")
+        program_files_root = os.environ.get(
+            "PROGRAMFILES", "C:\\Program Files"
+        )
+        legacy_path = os.path.join(
+            program_files_root, "NVIDIA Corporation", "NVSMI", smi
+        )
+        new_path = os.path.join(system_root, "System32", smi)
         smis = [new_path, legacy_path]
         for candidate_smi in smis:
             if os.path.exists(candidate_smi):
                 smi = f'"{candidate_smi}"'
                 break
     return smi
 
 
 def get_platform():
-    if sys.platform.startswith('linux'):
-        return 'linux'
-    elif sys.platform.startswith('win32'):
-        return 'win32'
-    elif sys.platform.startswith('cygwin'):
-        return 'cygwin'
-    elif sys.platform.startswith('darwin'):
-        return 'darwin'
+    if sys.platform.startswith("linux"):
+        return "linux"
+    elif sys.platform.startswith("win32"):
+        return "win32"
+    elif sys.platform.startswith("cygwin"):
+        return "cygwin"
+    elif sys.platform.startswith("darwin"):
+        return "darwin"
     else:
         return sys.platform
 
 
 def get_mac_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'sw_vers -productVersion', r'(.*)')
+    return run_and_parse_first_match(
+        run_lambda, "sw_vers -productVersion", r"(.*)"
+    )
 
 
 def get_windows_version(run_lambda):
-    system_root = os.environ.get('SYSTEMROOT', 'C:\\Windows')
-    wmic_cmd = os.path.join(system_root, 'System32', 'Wbem', 'wmic')
-    findstr_cmd = os.path.join(system_root, 'System32', 'findstr')
-    return run_and_read_all(run_lambda, '{} os get Caption | {} /v Caption'.format(wmic_cmd, findstr_cmd))
+    system_root = os.environ.get("SYSTEMROOT", "C:\\Windows")
+    wmic_cmd = os.path.join(system_root, "System32", "Wbem", "wmic")
+    findstr_cmd = os.path.join(system_root, "System32", "findstr")
+    return run_and_read_all(
+        run_lambda,
+        "{} os get Caption | {} /v Caption".format(wmic_cmd, findstr_cmd),
+    )
 
 
 def get_lsb_version(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'lsb_release -a', r'Description:\t(.*)')
+    return run_and_parse_first_match(
+        run_lambda, "lsb_release -a", r"Description:\t(.*)"
+    )
 
 
 def check_release_file(run_lambda):
-    return run_and_parse_first_match(run_lambda, 'cat /etc/*-release',
-                                     r'PRETTY_NAME="(.*)"')
+    return run_and_parse_first_match(
+        run_lambda, "cat /etc/*-release", r'PRETTY_NAME="(.*)"'
+    )
 
 
 def get_os(run_lambda):
     from platform import machine
+
     platform = get_platform()
 
-    if platform == 'win32' or platform == 'cygwin':
+    if platform == "win32" or platform == "cygwin":
         return get_windows_version(run_lambda)
 
-    if platform == 'darwin':
+    if platform == "darwin":
         version = get_mac_version(run_lambda)
         if version is None:
             return None
-        return 'macOS {} ({})'.format(version, machine())
+        return "macOS {} ({})".format(version, machine())
 
-    if platform == 'linux':
+    if platform == "linux":
         # Ubuntu/Debian based
         desc = get_lsb_version(run_lambda)
         if desc is not None:
-            return '{} ({})'.format(desc, machine())
+            return "{} ({})".format(desc, machine())
 
         # Try reading /etc/*-release
         desc = check_release_file(run_lambda)
         if desc is not None:
-            return '{} ({})'.format(desc, machine())
+            return "{} ({})".format(desc, machine())
 
-        return '{} ({})'.format(platform, machine())
+        return "{} ({})".format(platform, machine())
 
     # Unknown platform
     return platform
 
 
 def get_pip_packages(run_lambda):
     """Returns `pip list` output. Note: will also find conda-installed pytorch
     and numpy packages."""
     # People generally have `pip` as `pip` or `pip3`
     def run_with_pip(pip):
-        if get_platform() == 'win32':
-            system_root = os.environ.get('SYSTEMROOT', 'C:\\Windows')
-            findstr_cmd = os.path.join(system_root, 'System32', 'findstr')
+        if get_platform() == "win32":
+            system_root = os.environ.get("SYSTEMROOT", "C:\\Windows")
+            findstr_cmd = os.path.join(system_root, "System32", "findstr")
             grep_cmd = r'{} /R "numpy torch"'.format(findstr_cmd)
         else:
             grep_cmd = r'grep "torch\|numpy"'
-        return run_and_read_all(run_lambda, pip + ' list --format=freeze | ' + grep_cmd)
+        return run_and_read_all(
+            run_lambda, pip + " list --format=freeze | " + grep_cmd
+        )
 
     # Try to figure out if the user is running pip or pip3.
-    out2 = run_with_pip('pip')
-    out3 = run_with_pip('pip3')
+    out2 = run_with_pip("pip")
+    out3 = run_with_pip("pip3")
 
     num_pips = len([x for x in [out2, out3] if x is not None])
     if num_pips == 0:
-        return 'pip', out2
+        return "pip", out2
 
     if num_pips == 1:
         if out2 is not None:
-            return 'pip', out2
-        return 'pip3', out3
+            return "pip", out2
+        return "pip3", out3
 
     # num_pips is 2. Return pip3 by default b/c that most likely
     # is the one associated with Python 3
-    return 'pip3', out3
+    return "pip3", out3
 
 
 def get_env_info():
     run_lambda = run
     pip_version, pip_list_output = get_pip_packages(run_lambda)
 
     if TORCH_AVAILABLE:
         version_str = torch.__version__
         debug_mode_str = str(torch.version.debug)
         cuda_available_str = str(torch.cuda.is_available())
         cuda_version_str = torch.version.cuda
-        if not hasattr(torch.version, 'hip') or torch.version.hip is None:  # cuda version
-            hip_compiled_version = hip_runtime_version = miopen_runtime_version = 'N/A'
+        if (
+            not hasattr(torch.version, "hip") or torch.version.hip is None
+        ):  # cuda version
+            hip_compiled_version = (
+                hip_runtime_version
+            ) = miopen_runtime_version = "N/A"
         else:  # HIP version
-            cfg = torch._C._show_config().split('\n')
-            hip_runtime_version = [s.rsplit(None, 1)[-1] for s in cfg if 'HIP Runtime' in s][0]
-            miopen_runtime_version = [s.rsplit(None, 1)[-1] for s in cfg if 'MIOpen' in s][0]
-            cuda_version_str = 'N/A'
+            cfg = torch._C._show_config().split("\n")
+            hip_runtime_version = [
+                s.rsplit(None, 1)[-1] for s in cfg if "HIP Runtime" in s
+            ][0]
+            miopen_runtime_version = [
+                s.rsplit(None, 1)[-1] for s in cfg if "MIOpen" in s
+            ][0]
+            cuda_version_str = "N/A"
             hip_compiled_version = torch.version.hip
     else:
-        version_str = debug_mode_str = cuda_available_str = cuda_version_str = 'N/A'
-        hip_compiled_version = hip_runtime_version = miopen_runtime_version = 'N/A'
+        version_str = (
+            debug_mode_str
+        ) = cuda_available_str = cuda_version_str = "N/A"
+        hip_compiled_version = (
+            hip_runtime_version
+        ) = miopen_runtime_version = "N/A"
 
     return SystemEnv(
         torch_version=version_str,
         is_debug_build=debug_mode_str,
-        python_version='{}.{} ({}-bit runtime)'.format(sys.version_info[0], sys.version_info[1], sys.maxsize.bit_length() + 1),
+        python_version="{}.{} ({}-bit runtime)".format(
+            sys.version_info[0],
+            sys.version_info[1],
+            sys.maxsize.bit_length() + 1,
+        ),
         is_cuda_available=cuda_available_str,
         cuda_compiled_version=cuda_version_str,
         cuda_runtime_version=get_running_cuda_version(run_lambda),
         nvidia_gpu_models=get_gpu_info(run_lambda),
         nvidia_driver_version=get_nvidia_driver_version(run_lambda),
         cudnn_version=get_cudnn_version(run_lambda),
         hip_compiled_version=hip_compiled_version,
@@ -313,14 +365,15 @@
         conda_packages=get_conda_packages(run_lambda),
         os=get_os(run_lambda),
         gcc_version=get_gcc_version(run_lambda),
         clang_version=get_clang_version(run_lambda),
         cmake_version=get_cmake_version(run_lambda),
     )
 
+
 env_info_fmt = """
 PyTorch version: {torch_version}
 Is debug build: {is_debug_build}
 CUDA used to build PyTorch: {cuda_compiled_version}
 ROCM used to build PyTorch: {hip_compiled_version}
 
 OS: {os}
@@ -340,92 +393,110 @@
 Versions of relevant libraries:
 {pip_packages}
 {conda_packages}
 """.strip()
 
 
 def pretty_str(envinfo):
-    def replace_nones(dct, replacement='Could not collect'):
+    def replace_nones(dct, replacement="Could not collect"):
         for key in dct.keys():
             if dct[key] is not None:
                 continue
             dct[key] = replacement
         return dct
 
-    def replace_bools(dct, true='Yes', false='No'):
+    def replace_bools(dct, true="Yes", false="No"):
         for key in dct.keys():
             if dct[key] is True:
                 dct[key] = true
             elif dct[key] is False:
                 dct[key] = false
         return dct
 
-    def prepend(text, tag='[prepend]'):
-        lines = text.split('\n')
+    def prepend(text, tag="[prepend]"):
+        lines = text.split("\n")
         updated_lines = [tag + line for line in lines]
-        return '\n'.join(updated_lines)
+        return "\n".join(updated_lines)
 
-    def replace_if_empty(text, replacement='No relevant packages'):
+    def replace_if_empty(text, replacement="No relevant packages"):
         if text is not None and len(text) == 0:
             return replacement
         return text
 
     def maybe_start_on_next_line(string):
         # If `string` is multiline, prepend a \n to it.
-        if string is not None and len(string.split('\n')) > 1:
-            return '\n{}\n'.format(string)
+        if string is not None and len(string.split("\n")) > 1:
+            return "\n{}\n".format(string)
         return string
 
     mutable_dict = envinfo._asdict()
 
     # If nvidia_gpu_models is multiline, start on the next line
-    mutable_dict['nvidia_gpu_models'] = \
-        maybe_start_on_next_line(envinfo.nvidia_gpu_models)
+    mutable_dict["nvidia_gpu_models"] = maybe_start_on_next_line(
+        envinfo.nvidia_gpu_models
+    )
 
     # If the machine doesn't have CUDA, report some fields as 'No CUDA'
     dynamic_cuda_fields = [
-        'cuda_runtime_version',
-        'nvidia_gpu_models',
-        'nvidia_driver_version',
+        "cuda_runtime_version",
+        "nvidia_gpu_models",
+        "nvidia_driver_version",
     ]
-    all_cuda_fields = dynamic_cuda_fields + ['cudnn_version']
+    all_cuda_fields = dynamic_cuda_fields + ["cudnn_version"]
     all_dynamic_cuda_fields_missing = all(
-        mutable_dict[field] is None for field in dynamic_cuda_fields)
-    if TORCH_AVAILABLE and not torch.cuda.is_available() and all_dynamic_cuda_fields_missing:
+        mutable_dict[field] is None for field in dynamic_cuda_fields
+    )
+    if (
+        TORCH_AVAILABLE
+        and not torch.cuda.is_available()
+        and all_dynamic_cuda_fields_missing
+    ):
         for field in all_cuda_fields:
-            mutable_dict[field] = 'No CUDA'
+            mutable_dict[field] = "No CUDA"
         if envinfo.cuda_compiled_version is None:
-            mutable_dict['cuda_compiled_version'] = 'None'
+            mutable_dict["cuda_compiled_version"] = "None"
 
     # Replace True with Yes, False with No
     mutable_dict = replace_bools(mutable_dict)
 
     # Replace all None objects with 'Could not collect'
     mutable_dict = replace_nones(mutable_dict)
 
     # If either of these are '', replace with 'No relevant packages'
-    mutable_dict['pip_packages'] = replace_if_empty(mutable_dict['pip_packages'])
-    mutable_dict['conda_packages'] = replace_if_empty(mutable_dict['conda_packages'])
+    mutable_dict["pip_packages"] = replace_if_empty(
+        mutable_dict["pip_packages"]
+    )
+    mutable_dict["conda_packages"] = replace_if_empty(
+        mutable_dict["conda_packages"]
+    )
 
     # Tag conda and pip packages with a prefix
     # If they were previously None, they'll show up as ie '[conda] Could not collect'
-    if mutable_dict['pip_packages']:
-        mutable_dict['pip_packages'] = prepend(mutable_dict['pip_packages'],
-                                               '[{}] '.format(envinfo.pip_version))
-    if mutable_dict['conda_packages']:
-        mutable_dict['conda_packages'] = prepend(mutable_dict['conda_packages'],
-                                                 '[conda] ')
+    if mutable_dict["pip_packages"]:
+        mutable_dict["pip_packages"] = prepend(
+            mutable_dict["pip_packages"], "[{}] ".format(envinfo.pip_version)
+        )
+    if mutable_dict["conda_packages"]:
+        mutable_dict["conda_packages"] = prepend(
+            mutable_dict["conda_packages"], "[conda] "
+        )
     return env_info_fmt.format(**mutable_dict)
 
 
 def get_pretty_env_info():
     return pretty_str(get_env_info())
 
 
 def main():
     print("Collecting environment information...")
     output = get_pretty_env_info()
     print(output)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
+
+
+def main():
+    print("Collecting environment information...")
+    env_info = get_env_info()
+    print(env_info)
```

### Comparing `mngs-1.3.0/src/mngs/general/_embed.py` & `mngs-1.3.1/src/mngs/gen/_embed.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_norm.py` & `mngs-1.3.1/src/mngs/gen/_norm.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_paste.py` & `mngs-1.3.1/src/mngs/gen/_paste.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_reload.py` & `mngs-1.3.1/src/mngs/gen/_reload.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_reproduce.py` & `mngs-1.3.1/src/mngs/gen/_reproduce.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_shell.py` & `mngs-1.3.1/src/mngs/gen/_shell.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_start.py` & `mngs-1.3.1/src/mngs/gen/_start.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/_xml2dict.py` & `mngs-1.3.1/src/mngs/gen/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/email.py` & `mngs-1.3.1/src/mngs/gen/email.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/load.py` & `mngs-1.3.1/src/mngs/gen/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/mat2py.py` & `mngs-1.3.1/src/mngs/gen/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/misc.py` & `mngs-1.3.1/src/mngs/gen/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     pop_keys(keys_list, keys_to_pop)
     """
     indi_to_remain = [k not in keys_to_pop for k in keys_list]
     keys_remainded_list = list(np.array(keys_list)[list(indi_to_remain)])
     return keys_remainded_list
 
 
-def fmt_size(num, suffix="B"):
+def readable_bytes(num, suffix="B"):
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, "Yi", suffix)
```

### Comparing `mngs-1.3.0/src/mngs/general/pandas.py` & `mngs-1.3.1/src/mngs/gen/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/path.py` & `mngs-1.3.1/src/mngs/gen/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/general/save.py` & `mngs-1.3.1/src/mngs/gen/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/gists/_SigMacro_processFigure_S.py` & `mngs-1.3.1/src/mngs/gists/_SigMacro_processFigure_S.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/gists/_SigMacro_toBlue.py` & `mngs-1.3.1/src/mngs/gists/_SigMacro_toBlue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/io/load.py` & `mngs-1.3.1/src/mngs/general/load.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/io/path.py` & `mngs-1.3.1/src/mngs/general/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/io/save.py` & `mngs-1.3.1/src/mngs/general/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/linalg/_misc.py` & `mngs-1.3.1/src/mngs/linalg/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/ClassificationReporter.py` & `mngs-1.3.1/src/mngs/ml/ClassificationReporter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/ClassifierServer.py` & `mngs-1.3.1/src/mngs/ml/ClassifierServer.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/EarlyStopping.py` & `mngs-1.3.1/src/mngs/ml/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/LearningCurveLogger.py` & `mngs-1.3.1/src/mngs/ml/LearningCurveLogger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/__Classifiers.py` & `mngs-1.3.1/src/mngs/ml/__Classifiers.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/clustering/_UMAP.py` & `mngs-1.3.1/src/mngs/ml/clustering/_UMAP.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/clustering/_umap.py` & `mngs-1.3.1/src/mngs/ml/clustering/_umap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-1.3.1/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-1.3.1/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/metrics/_bACC.py` & `mngs-1.3.1/src/mngs/ml/metrics/_bACC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-1.3.1/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/optim/_get_set.py` & `mngs-1.3.1/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/_conf_mat.py` & `mngs-1.3.1/src/mngs/ml/plt/_conf_mat.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/_learning_curve.py` & `mngs-1.3.1/src/mngs/ml/plt/_learning_curve.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/_optuna_study.py` & `mngs-1.3.1/src/mngs/ml/plt/_optuna_study.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/aucs/example.py` & `mngs-1.3.1/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-1.3.1/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/plt/aucs/roc_auc.py` & `mngs-1.3.1/src/mngs/ml/plt/aucs/roc_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/silhoute_score_block.py` & `mngs-1.3.1/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/sk/_clf.py` & `mngs-1.3.1/src/mngs/ml/sk/_clf.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/sk/_to_sktime.py` & `mngs-1.3.1/src/mngs/ml/sk/_to_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-1.3.1/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_LabelEncoder.py` & `mngs-1.3.1/src/mngs/ml/utils/_LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_check_params.py` & `mngs-1.3.1/src/mngs/ml/utils/_check_params.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-1.3.1/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_merge_labels.py` & `mngs-1.3.1/src/mngs/ml/utils/_merge_labels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/ml/utils/_under_sample.py` & `mngs-1.3.1/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/mngs/setup.py` & `mngs-1.3.1/src/mngs/mngs/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_AxiswiseDropout.py` & `mngs-1.3.1/src/mngs/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_BNet.py` & `mngs-1.3.1/src/mngs/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_BNet_Res.py` & `mngs-1.3.1/src/mngs/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_ChannelGainChanger.py` & `mngs-1.3.1/src/mngs/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_DropoutChannels.py` & `mngs-1.3.1/src/mngs/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_Filters.py` & `mngs-1.3.1/src/mngs/nn/_Filters.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_FreqGainChanger.py` & `mngs-1.3.1/src/mngs/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_GaussianFilter.py` & `mngs-1.3.1/src/mngs/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_Hilbert.py` & `mngs-1.3.1/src/mngs/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_MNet_1000.py` & `mngs-1.3.1/src/mngs/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_ModulationIndex.py` & `mngs-1.3.1/src/mngs/nn/_ModulationIndex.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_PAC.py` & `mngs-1.3.1/src/mngs/nn/_PAC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_PAC_working.py` & `mngs-1.3.1/src/mngs/nn/_PAC_working.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_PSD.py` & `mngs-1.3.1/src/mngs/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_ResNet1D.py` & `mngs-1.3.1/src/mngs/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_SpatialAttention.py` & `mngs-1.3.1/src/mngs/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_Spectrogram.py` & `mngs-1.3.1/src/mngs/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_SwapChannels.py` & `mngs-1.3.1/src/mngs/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/_Wavelet.py` & `mngs-1.3.1/src/mngs/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/nn/__init__.py` & `mngs-1.3.1/src/mngs/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/os/_mv.py` & `mngs-1.3.1/src/mngs/os/_mv.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_add_hue.py` & `mngs-1.3.1/src/mngs/plt/_add_hue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_annotated_heatmap.py` & `mngs-1.3.1/src/mngs/plt/_annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_configure_mpl.py` & `mngs-1.3.1/src/mngs/plt/_configure_mpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_draw_a_cube.py` & `mngs-1.3.1/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-1.3.1/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_mk_colorbar.py` & `mngs-1.3.1/src/mngs/plt/_mk_colorbar.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_subplots.py` & `mngs-1.3.1/src/mngs/plt/_subplots.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/_tpl.py` & `mngs-1.3.1/src/mngs/plt/_tpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_circular_hist.py` & `mngs-1.3.1/src/mngs/plt/ax/_circular_hist.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_extend.py` & `mngs-1.3.1/src/mngs/plt/ax/_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_hide_spines.py` & `mngs-1.3.1/src/mngs/plt/ax/_hide_spines.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_map_ticks.py` & `mngs-1.3.1/src/mngs/plt/ax/_map_ticks.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_panel.py` & `mngs-1.3.1/src/mngs/plt/ax/_panel.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_sci_note.py` & `mngs-1.3.1/src/mngs/plt/ax/_sci_note.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/ax/_set_pos.py` & `mngs-1.3.1/src/mngs/plt/ax/_set_pos.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/colors.py` & `mngs-1.3.1/src/mngs/plt/colors.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/plt/get_mpl_color.py` & `mngs-1.3.1/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/resource/limit_RAM.py` & `mngs-1.3.1/src/mngs/res/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/__init__.py` & `mngs-1.3.1/src/mngs/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_bonferroni_correction.py` & `mngs-1.3.1/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_brunner_munzel_test.py` & `mngs-1.3.1/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_corr_test.py` & `mngs-1.3.1/src/mngs/stats/_corr_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_fdr_correction.py` & `mngs-1.3.1/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_general.py` & `mngs-1.3.1/src/mngs/stats/_general.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_multicompair.py` & `mngs-1.3.1/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_nocorrelation_test.py` & `mngs-1.3.1/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/stats/_smirnov_grubbs.py` & `mngs-1.3.1/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs/torch/_apply_to.py` & `mngs-1.3.1/src/mngs/torch/_apply_to.py`

 * *Files identical despite different names*

### Comparing `mngs-1.3.0/src/mngs.egg-info/PKG-INFO` & `mngs-1.3.1/src/mngs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.3.0
+Version: 1.3.1
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
-Description: ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
+Description: # monogusa (= lazy in Japanese)
+        mngs is Python utilities for ML and DSP projects
+        
+        ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
+        
+        ![Hard Working Sloth](./docs/hard_working_sloth.jpg)
         
         ## Installation
         ``` bash
         $ pip install mngs
         ```
         
         ## Galleries
-        [`mngs.dsp`](https://github.com/ywatanabe1989/mngs/tree/develop/src/mngs/dsp#readme)
+        - [`mngs.dsp`](https://github.com/ywatanabe1989/mngs/tree/main/src/mngs/dsp#readme)
+          Digital Signal Processing
+        - [`mngs.res`](https://github.com/ywatanabe1989/mngs/tree/main/src/mngs/res#readme)
+          Resource
+        
+        - mngs.general
+        - mngs.io
+        - mngs.plt
+        - mngs.ml
+        - mngs.stats
         
         ## Contact
         Yusuke Watanabe (ywata1989@gmail.com).
         
         
 Keywords: utils,utilities,python,machine learning
 Platform: UNKNOWN
```

### Comparing `mngs-1.3.0/src/mngs.egg-info/SOURCES.txt` & `mngs-1.3.1/src/mngs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -51,19 +51,38 @@
 src/mngs/dsp/nn/__init__.py
 src/mngs/dsp/utils/__init__.py
 src/mngs/dsp/utils/_differential_bandpass_filters.py
 src/mngs/dsp/utils/_ensure_even_len.py
 src/mngs/dsp/utils/_zero_pad.py
 src/mngs/dsp/utils/filter.py
 src/mngs/dsp/utils/pac.py
+src/mngs/gen/_TimeStamper.py
+src/mngs/gen/__init__.py
+src/mngs/gen/_close.py
+src/mngs/gen/_converters.py
+src/mngs/gen/_embed.py
+src/mngs/gen/_norm.py
+src/mngs/gen/_paste.py
+src/mngs/gen/_reload.py
+src/mngs/gen/_reproduce.py
+src/mngs/gen/_shell.py
+src/mngs/gen/_start.py
+src/mngs/gen/_xml2dict.py
+src/mngs/gen/email.py
+src/mngs/gen/latex.py
+src/mngs/gen/load.py
+src/mngs/gen/mat2py.py
+src/mngs/gen/misc.py
+src/mngs/gen/pandas.py
+src/mngs/gen/path.py
+src/mngs/gen/save.py
 src/mngs/general/_TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_close.py
 src/mngs/general/_converters.py
-src/mngs/general/_cuda_collect_env.py
 src/mngs/general/_embed.py
 src/mngs/general/_norm.py
 src/mngs/general/_paste.py
 src/mngs/general/_reload.py
 src/mngs/general/_reproduce.py
 src/mngs/general/_shell.py
 src/mngs/general/_start.py
@@ -179,17 +198,19 @@
 src/mngs/plt/ax/_map_ticks.py
 src/mngs/plt/ax/_panel.py
 src/mngs/plt/ax/_sci_note.py
 src/mngs/plt/ax/_set_n_ticks.py
 src/mngs/plt/ax/_set_pos.py
 src/mngs/plt/ax/_set_size.py
 src/mngs/plt/ax/_set_ticks.py
-src/mngs/resource/__init__.py
-src/mngs/resource/get.py
-src/mngs/resource/limit_RAM.py
+src/mngs/res/__init__.py
+src/mngs/res/_info.py
+src/mngs/res/limit_RAM.py
+src/mngs/res/_utils/__init__.py
+src/mngs/res/_utils/_cuda_collect_env.py
 src/mngs/stats/__init__.py
 src/mngs/stats/_bonferroni_correction.py
 src/mngs/stats/_brunner_munzel_test.py
 src/mngs/stats/_calc_partial_corr.py
 src/mngs/stats/_corr_test.py
 src/mngs/stats/_fdr_correction.py
 src/mngs/stats/_general.py
```

