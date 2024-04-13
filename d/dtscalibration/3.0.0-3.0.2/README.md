# Comparing `tmp/dtscalibration-3.0.0.tar.gz` & `tmp/dtscalibration-3.0.2.tar.gz`

## Comparing `dtscalibration-3.0.0.tar` & `dtscalibration-3.0.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/.bumpversion.cfg
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/.readthedocs.yml
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/.zenodo.json
--rw-r--r--   0        0        0    12522 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/CITATION.cff
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/authors.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/changelog.rst
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/contributing.rst
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/index.rst
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/learn_by_examples.rst
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/readme.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/01Load_xml_measurement_files.ipynb
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/03Define_sections.ipynb
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/04Calculate_variance_Stokes.ipynb
--rw-r--r--   0        0        0    10323 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/07Calibrate_single_ended.ipynb
--rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/08Calibrate_double_ended.ipynb
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/09Import_timeseries.ipynb
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/10Align_double_ended_measurements.ipynb
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/13Fixed_parameter_calibration.ipynb
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/14Lossy_splices.ipynb
--rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/15Matching_sections.ipynb
--rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/16Averaging_temperatures.ipynb
--rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/A2Load_sensornet_files.ipynb
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/A3Load_ap_sensing_files.ipynb
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/notebooks/A4Load_sensortran_files.ipynb
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/docs/reference/index.rst
--rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/examples/Added uncertainty from fixing parameters.pdf
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/examples/README.md
--rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/examples/temperature_variance_from_stokes.pdf
--rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
--rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/__init__.py
--rw-r--r--   0        0        0    80227 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/calibrate_utils.py
--rw-r--r--   0        0        0   118572 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/dts_accessor.py
--rw-r--r--   0        0        0    45709 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/dts_accessor_utils.py
--rw-r--r--   0        0        0    23501 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/plot.py
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/variance_helpers.py
--rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/variance_stokes.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/calibration/section_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/__init__.py
--rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/apsensing.py
--rw-r--r--   0        0        0    17354 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/sensornet.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/sensortran.py
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/silixa.py
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/src/dtscalibration/io/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/test_averaging.py
--rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/test_datastore.py
--rw-r--r--   0        0        0    78659 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/test_dtscalibration.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/test_examples.py
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/test_variance_stokes.py
--rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
--rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
--rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/docs_notebooks/01Not_working.ipynb
--rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921112245510.xml
--rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921112746818.xml
--rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921113248085.xml
--rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014052498.xml
--rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014057119.xml
--rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014101652.xml
--rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014106243.xml
--rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014110917.xml
--rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014115480.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_ended2/info.txt
--rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
--rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
--rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
--rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
--rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
--rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
--rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
--rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
--rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
--rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
--rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
--rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
--rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
--rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
--rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
--rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
--rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
--rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
--rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
--rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
--rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
--rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
--rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
--rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
--rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
--rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
--rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
--rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
--rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
--rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
--rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
--rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
--rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
--rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
--rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
--rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
--rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
--rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
--rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
--rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
--rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
--rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
--rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
--rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
--rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
--rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
--rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132202074.xml
--rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132232903.xml
--rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132303723.xml
--rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/zipped data/double_ended.zip
--rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/zipped data/double_ended2.zip
--rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/zipped data/double_single_ended.zip
--rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/zipped data/silixa_v4.5.zip
--rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/tests/data/zipped data/single_ended.zip
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/.gitignore
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/AUTHORS.rst
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/LICENSE
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/README.rst
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 dtscalibration-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.zenodo.json
+-rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CITATION.cff
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/index.rst
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/learn_by_examples.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/readme.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/01Load_xml_measurement_files.ipynb
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/03Define_sections.ipynb
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/04Calculate_variance_Stokes.ipynb
+-rw-r--r--   0        0        0    10323 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/07Calibrate_single_ended.ipynb
+-rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/08Calibrate_double_ended.ipynb
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/09Import_timeseries.ipynb
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/10Align_double_ended_measurements.ipynb
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/11Merge_single_measurements_into_double.ipynb
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/13Fixed_parameter_calibration.ipynb
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/14Lossy_splices.ipynb
+-rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/15Matching_sections.ipynb
+-rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/16Averaging_temperatures.ipynb
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A2Load_sensornet_files.ipynb
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A3Load_ap_sensing_files.ipynb
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A4Load_sensortran_files.ipynb
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/reference/index.rst
+-rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/Added uncertainty from fixing parameters.pdf
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/README.md
+-rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/temperature_variance_from_stokes.pdf
+-rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
+-rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/__init__.py
+-rw-r--r--   0        0        0    80227 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/calibrate_utils.py
+-rw-r--r--   0        0        0   118552 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/dts_accessor.py
+-rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/dts_accessor_utils.py
+-rw-r--r--   0        0        0    23501 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/plot.py
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/variance_helpers.py
+-rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/variance_stokes.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/calibration/section_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/__init__.py
+-rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/apsensing.py
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/sensornet.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/sensortran.py
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/silixa.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_averaging.py
+-rw-r--r--   0        0        0    20532 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_datastore.py
+-rw-r--r--   0        0        0    78659 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_dtscalibration.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_examples.py
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_variance_stokes.py
+-rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
+-rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
+-rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/docs_notebooks/01Not_working.ipynb
+-rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112245510.xml
+-rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112746818.xml
+-rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921113248085.xml
+-rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014052498.xml
+-rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014057119.xml
+-rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014101652.xml
+-rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014106243.xml
+-rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014110917.xml
+-rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014115480.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/info.txt
+-rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
+-rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
+-rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
+-rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
+-rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
+-rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
+-rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
+-rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
+-rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
+-rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
+-rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
+-rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
+-rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
+-rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
+-rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
+-rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
+-rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
+-rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
+-rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
+-rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
+-rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
+-rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
+-rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
+-rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
+-rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
+-rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
+-rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
+-rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
+-rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
+-rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
+-rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
+-rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
+-rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
+-rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
+-rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
+-rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
+-rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
+-rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
+-rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
+-rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
+-rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
+-rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
+-rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
+-rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
+-rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
+-rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132202074.xml
+-rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132232903.xml
+-rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132303723.xml
+-rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_ended.zip
+-rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_ended2.zip
+-rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_single_ended.zip
+-rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/silixa_v4.5.zip
+-rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/single_ended.zip
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.gitignore
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/LICENSE
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/README.rst
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/PKG-INFO
```

### Comparing `dtscalibration-3.0.0/.zenodo.json` & `dtscalibration-3.0.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/CHANGELOG.rst` & `dtscalibration-3.0.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Changelog
 =========
 
+3.0.1 (2024-04-13)
+---
+
+Fixed
+
+* Oryx v4 double ended could have the backward measurements incorrectly cut off during loading.
+
 3.0.0 (2023-11-05)
 ---
 
 Added
 
 * Calibration functions are now accessed via the .dts accessor in favor of the DataStore class.
 * Improved the functionality of `merge_double_ended`, by adding a check that handles measurements missing in one channel while present in the other ([#171](https://github.com/dtscalibration/python-dts-calibration/pull/171))
```

### Comparing `dtscalibration-3.0.0/CITATION.cff` & `dtscalibration-3.0.2/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
   - calibration
   - Python
 cff-version: "1.0.3"
 doi: "10.5281/zenodo.1410097"
 license: "BSD-3-Clause"
 repository-code: "https://github.com/dtscalibration/python-dts-calibration"
 title: "Python distributed temperature sensing calibration"
-version: "v3.0.0"
+version: "v3.0.2"
 url: "https://python-dts-calibration.readthedocs.io"
```

### Comparing `dtscalibration-3.0.0/CONTRIBUTING.rst` & `dtscalibration-3.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/conf.py` & `dtscalibration-3.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 source_suffix = [".rst", ".md"]
 master_doc = "index"
 project = "dtscalibration"
 year = str(date.today().year)
 author = "Bas des Tombe and Bart Schilperoort"
 copyright = f"{year}, {author}"
-version = release = "3.0.0"
+version = release = "3.0.2"
 
 pygments_style = "trac"
 templates_path = [".", sphinx_autosummary_accessors.templates_path]
 extlinks = {
     "issue": (
         "https://github.com/dtscalibration/python-dts-calibration/issues" "/%s",
         "#",
```

### Comparing `dtscalibration-3.0.0/docs/learn_by_examples.rst` & `dtscalibration-3.0.2/docs/learn_by_examples.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/01Load_xml_measurement_files.ipynb` & `dtscalibration-3.0.2/docs/notebooks/01Load_xml_measurement_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/03Define_sections.ipynb` & `dtscalibration-3.0.2/docs/notebooks/03Define_sections.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/04Calculate_variance_Stokes.ipynb` & `dtscalibration-3.0.2/docs/notebooks/04Calculate_variance_Stokes.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/07Calibrate_single_ended.ipynb` & `dtscalibration-3.0.2/docs/notebooks/07Calibrate_single_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/08Calibrate_double_ended.ipynb` & `dtscalibration-3.0.2/docs/notebooks/08Calibrate_double_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/09Import_timeseries.ipynb` & `dtscalibration-3.0.2/docs/notebooks/09Import_timeseries.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/10Align_double_ended_measurements.ipynb` & `dtscalibration-3.0.2/docs/notebooks/10Align_double_ended_measurements.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb` & `dtscalibration-3.0.2/docs/notebooks/11Merge_single_measurements_into_double.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb` & `dtscalibration-3.0.2/docs/notebooks/12Datastore_from_numpy_arrays.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/13Fixed_parameter_calibration.ipynb` & `dtscalibration-3.0.2/docs/notebooks/13Fixed_parameter_calibration.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/14Lossy_splices.ipynb` & `dtscalibration-3.0.2/docs/notebooks/14Lossy_splices.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/15Matching_sections.ipynb` & `dtscalibration-3.0.2/docs/notebooks/15Matching_sections.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/16Averaging_temperatures.ipynb` & `dtscalibration-3.0.2/docs/notebooks/16Averaging_temperatures.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb` & `dtscalibration-3.0.2/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/A2Load_sensornet_files.ipynb` & `dtscalibration-3.0.2/docs/notebooks/A2Load_sensornet_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/A3Load_ap_sensing_files.ipynb` & `dtscalibration-3.0.2/docs/notebooks/A3Load_ap_sensing_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/notebooks/A4Load_sensortran_files.ipynb` & `dtscalibration-3.0.2/docs/notebooks/A4Load_sensortran_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/docs/reference/index.rst` & `dtscalibration-3.0.2/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/examples/Added uncertainty from fixing parameters.pdf` & `dtscalibration-3.0.2/examples/Added uncertainty from fixing parameters.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/examples/temperature_variance_from_stokes.pdf` & `dtscalibration-3.0.2/examples/temperature_variance_from_stokes.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf` & `dtscalibration-3.0.2/examples/conference presentations/EGU2019_poster_dtscalibration.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf` & `dtscalibration-3.0.2/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/__init__.py` & `dtscalibration-3.0.2/src/dtscalibration/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib.metadata
+import warnings
 
 from dtscalibration.dts_accessor import DtsAccessor  # noqa: F401
 from dtscalibration.dts_accessor_utils import get_netcdf_encoding
 from dtscalibration.dts_accessor_utils import merge_double_ended
 from dtscalibration.dts_accessor_utils import shift_double_ended
 from dtscalibration.dts_accessor_utils import suggest_cable_shift_double_ended
 from dtscalibration.io.apsensing import read_apsensing_files
@@ -19,7 +20,12 @@
     "read_sensortran_files",
     "read_silixa_files",
     "get_netcdf_encoding",
     "merge_double_ended",
     "shift_double_ended",
     "suggest_cable_shift_double_ended",
 ]
+
+warnings.filterwarnings(
+    "ignore",
+    message="Converting non-nanosecond precision timedelta values to nanosecond",
+)
```

### Comparing `dtscalibration-3.0.0/src/dtscalibration/calibrate_utils.py` & `dtscalibration-3.0.2/src/dtscalibration/calibrate_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/dts_accessor.py` & `dtscalibration-3.0.2/src/dtscalibration/dts_accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module provides an xarray accessor for DTS calibration."""
+"""The xarray accessor for DTS calibration."""
 
 import dask.array as da
 import numpy as np
 import scipy.stats as sst
 import xarray as xr
 import yaml
```

### Comparing `dtscalibration-3.0.0/src/dtscalibration/dts_accessor_utils.py` & `dtscalibration-3.0.2/src/dtscalibration/dts_accessor_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,25 +841,23 @@
         if direction == "fw" and direction_next == "bw":
             iuse_chfw.append(ind)
             iuse_chbw.append(ind_next)
 
         elif direction == "bw" and direction_next == "fw":
             pass
 
-        elif direction == "fw" and direction_next == "fw":
-            if verbose:
-                print(
-                    f"Missing backward measurement beween {ds_fw.time.values[ind]} and {ds_fw.time.values[ind_next]}"
-                )
+        elif direction == "fw" and direction_next == "fw" and verbose:
+            print(
+                f"Missing backward measurement beween {ds_fw.time.values[ind]} and {ds_fw.time.values[ind_next]}"
+            )
 
-        elif direction == "bw" and direction_next == "bw":
-            if verbose:
-                print(
-                    f"Missing forward measurement beween {ds_bw.time.values[ind]} and {ds_bw.time.values[ind_next]}"
-                )
+        elif direction == "bw" and direction_next == "bw" and verbose:
+            print(
+                f"Missing forward measurement beween {ds_bw.time.values[ind]} and {ds_bw.time.values[ind_next]}"
+            )
 
     # throw out is dt differs from its neighbors
     if verify_timedeltas:
         dt = (
             ds_bw.isel(time=iuse_chbw).time.values
             - ds_fw.isel(time=iuse_chfw).time.values
         ) / np.timedelta64(1, "s")
```

### Comparing `dtscalibration-3.0.0/src/dtscalibration/plot.py` & `dtscalibration-3.0.2/src/dtscalibration/plot.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/variance_helpers.py` & `dtscalibration-3.0.2/src/dtscalibration/variance_helpers.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/variance_stokes.py` & `dtscalibration-3.0.2/src/dtscalibration/variance_stokes.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/calibration/section_utils.py` & `dtscalibration-3.0.2/src/dtscalibration/calibration/section_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/io/apsensing.py` & `dtscalibration-3.0.2/src/dtscalibration/io/apsensing.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/io/sensornet.py` & `dtscalibration-3.0.2/src/dtscalibration/io/sensornet.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,21 @@
     valid = any([fnmatch.fnmatch(ddf_version, v_) for v_ in valid_versions])
 
     if valid and (
         fnmatch.fnmatch(ddf_version, "Halo DTS v1*")
         or fnmatch.fnmatch(ddf_version, "Sentinel DTS v5*")
     ):
         flip_reverse_measurements = True
+    elif fnmatch.fnmatch(ddf_version, "ORYX F/W v4*"):
+        flip_reverse_measurements = False
     else:
         flip_reverse_measurements = False
         warnings.warn(
-            f"Sensornet .dff version {ddf_version}"
-            " has not been tested.\nPlease open an issue on github"
+            f"\n    Sensornet .dff version {ddf_version}"
+            " has not been tested.\n    Please open an issue on github"
             " and provide an example file"
         )
 
     data_vars, coords, attrs = read_sensornet_files_routine_v3(
         filepathlist,
         timezone_netcdf=timezone_netcdf,
         timezone_input_files=timezone_input_files,
@@ -394,16 +396,22 @@
             fiber_bw_end_index = np.min(
                 [xraw.size, fiber_bw_1_index + (fiber_end_index - fiber_1_index)]
             )
             fiber_bw_start_index = np.max(
                 [0, fiber_bw_1_index - fiber_n_indices - fiber_n_indices_internal]
             )
 
-            REV_ST = REV_ST[fiber_bw_start_index:fiber_bw_end_index]
-            REV_AST = REV_AST[fiber_bw_start_index:fiber_bw_end_index]
+            if (fiber_end_index - fiber_start_index) == (
+                fiber_bw_end_index - fiber_bw_start_index
+            ):
+                REV_ST = REV_ST[fiber_bw_start_index:fiber_bw_end_index]
+                REV_AST = REV_AST[fiber_bw_start_index:fiber_bw_end_index]
+            else:
+                REV_ST = REV_ST[fiber_start_index:fiber_end_index]
+                REV_AST = REV_AST[fiber_start_index:fiber_end_index]
 
         else:
             # Use the fiber indices from the forward channel
             n_indices_internal_left = fiber_0_index - fiber_start_index
             n_indices_internal_right = np.max([0, fiber_end_index - fiber_1_index])
             n_indices_internal_shortest = np.min(
                 [n_indices_internal_left, n_indices_internal_right]
```

### Comparing `dtscalibration-3.0.0/src/dtscalibration/io/sensortran.py` & `dtscalibration-3.0.2/src/dtscalibration/io/sensortran.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/io/silixa.py` & `dtscalibration-3.0.2/src/dtscalibration/io/silixa.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/src/dtscalibration/io/utils.py` & `dtscalibration-3.0.2/src/dtscalibration/io/utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/test_averaging.py` & `dtscalibration-3.0.2/tests/test_averaging.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/test_datastore.py` & `dtscalibration-3.0.2/tests/test_datastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,23 +524,25 @@
 
 
 def test_resample_datastore():
     filepath = data_dir_single_ended
     ds = read_silixa_files(directory=filepath, timezone_netcdf="UTC", file_ext="*.xml")
     assert ds.time.size == 3
 
-    ds_resampled = Dataset(ds.resample(time="47S").mean())
+    ds_resampled = ds.resample(time="47s").mean()
 
     assert ds_resampled.time.size == 2
-    assert ds_resampled.st.dims == ("x", "time"), (
-        "The dimension have to "
-        "be manually transposed "
-        "after resampling. To "
-        "guarantee the order"
-    )
+
+    ## No control over dim order from resample with accessor
+    # assert ds_resampled.st.dims == ("x", "time"), (
+    #     "The dimension have to "
+    #     "be manually transposed "
+    #     "after resampling. To "
+    #     "guarantee the order"
+    # )
 
 
 def test_timeseries_keys():
     filepath = data_dir_single_ended
     ds = read_silixa_files(directory=filepath, timezone_netcdf="UTC", file_ext="*.xml")
 
     k = ds.dts.get_timeseries_keys()
```

### Comparing `dtscalibration-3.0.0/tests/test_dtscalibration.py` & `dtscalibration-3.0.2/tests/test_dtscalibration.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/test_examples.py` & `dtscalibration-3.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/test_variance_stokes.py` & `dtscalibration-3.0.2/tests/test_variance_stokes.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml` & `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml` & `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml` & `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/docs_notebooks/01Not_working.ipynb` & `dtscalibration-3.0.2/tests/data/docs_notebooks/01Not_working.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921112245510.xml` & `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112245510.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921112746818.xml` & `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112746818.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended/channel 1_20170921113248085.xml` & `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921113248085.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014052498.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014052498.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014057119.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014057119.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014101652.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014101652.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014106243.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014106243.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014110917.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014110917.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_ended2/channel 1_20180328014115480.xml` & `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014115480.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml` & `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv` & `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv` & `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv` & `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf` & `dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat` & `dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml` & `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml` & `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml` & `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml` & `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml` & `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml` & `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml` & `dtscalibration-3.0.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132202074.xml` & `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132202074.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132232903.xml` & `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132232903.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/single_ended/channel 2_20180504132303723.xml` & `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132303723.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/zipped data/double_ended.zip` & `dtscalibration-3.0.2/tests/data/zipped data/double_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/zipped data/double_ended2.zip` & `dtscalibration-3.0.2/tests/data/zipped data/double_ended2.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/zipped data/double_single_ended.zip` & `dtscalibration-3.0.2/tests/data/zipped data/double_single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/zipped data/silixa_v4.5.zip` & `dtscalibration-3.0.2/tests/data/zipped data/silixa_v4.5.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/tests/data/zipped data/single_ended.zip` & `dtscalibration-3.0.2/tests/data/zipped data/single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/.gitignore` & `dtscalibration-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/LICENSE` & `dtscalibration-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.0/README.rst` & `dtscalibration-3.0.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.2.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -67,22 +67,24 @@
 
 .. code-block:: zsh
 
     pip install https://github.com/dtscalibration/python-dts-calibration/zipball/main --upgrade
 
 Package features
 ================
+DTS measures temperature by calibrating backscatter measurements to sections with a known temperature. DTS devices provide a simple interface to perform a limited calibration. Re-calibrating your measurements with this Python package gives you better temperature estimates and additional options.
+
 * Advanced calibration routine
-   * Both single- and double-ended setups
-   * Confidence intervals of calibrated temperature
-   * Time integration of calibration parameters
+   * Supports `single <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_- and `double-ended <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_ setups
+   * Compute uncertainty of the calibrated temperature
+   * All measurements are used to estimate parameter values that are constant over time.
    * Weighted least-squares calibration
-   * `Fixing parameters to a previously determined value <..//main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
-   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_
-   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_
+   * `Fixing parameters to a previously determined value <../main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
+   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
+   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
 * Dynamic reference section definition
 * Tools for merging and aligning double-ended setups
 * Data formats of most manufacturers are supported
 
 Devices currently supported
 ===========================
 * Silixa Ltd.: **Ultima** & **XT-DTS** .xml files *(up to version 8.1)*
@@ -90,15 +92,15 @@
 * AP Sensing: **CP320** .xml files *(single ended only)*
 * SensorTran: **SensorTran 5100** .dat binary files *(single ended only)*
 
 Documentation
 =============
 
 * A full calibration procedure for single-ended setups is presented in notebook `07Calibrate_single_ended.ipynb <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_ and for double-ended setups in `08Calibrate_double_ended.ipynb <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_.
-* Documentation at https://python-dts-calibration.readthedocs.io/ .
+* Documentation at `readthedocs <https://python-dts-calibration.readthedocs.io/en/latest/>`_.
 * Example notebooks (`./docs/notebooks`) that work within the browser can be viewed `here <https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks>`_.
 
 How to cite
 ===========
 The following article explains and discusses the calibration procedure:
 
     des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235
@@ -106,10 +108,10 @@
 Cite the specific implementation / repository via Zenodo:
 
 1. Check the version of `dtscalibration` that is used in your Python console with:
 
     >>> # The following line introduces the .dts accessor for xarray datasets
     >>> import dtscalibration  # noqa: E401
     >>> dtscalibration.__version__
-    '3.0.0'
+    '3.0.1'
 2. Go to `Zenodo <https://zenodo.org/search?q=conceptrecid:%221410097%22&sort=-version&all_versions=True>`_ and follow the link to the version of interest.
 3. The citation is found on the bottom right of the page.
```

### Comparing `dtscalibration-3.0.0/pyproject.toml` & `dtscalibration-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 packages = ["src/dtscalibration"]
 
 [tool.hatch.publish.index]
 disable = true  # Requires confirmation when publishing to pypi.
 
 [project]
 name = "dtscalibration"
-version = "3.0.0"
+version = "3.0.2"
 description = "Load Distributed Temperature Sensing (DTS) files, calibrate the temperature and estimate its uncertainty."
 readme = "README.rst"
 license = "BSD-3-Clause"
 requires-python = ">=3.9, <3.12"
 authors = [
   {name = "Bas des Tombe, Bart Schilperoort"},
 ]
@@ -154,15 +154,15 @@
   # "PLR",  # Pylint refactor (e.g. too-many-arguments)
   "PLW",  # Pylint warning (useless-else-on-loop)
   # "I",  # isort
   "SIM",  # flake8-simplify
 
 ]
 extend-select = [
-  "D401",  # First line should be in imperative mood
+  #"D401",  # First line should be in imperative mood
   "D400",  # First line should end in a period.
   "D404",  # First word of the docstring should not be "This"
   "TID252",  # No relative imports (not pep8 compliant)
 ]
 ignore = [
   "PLR2004",  # magic value used in comparson
   "E501",  # Line too long (want to have fixed
```

### Comparing `dtscalibration-3.0.0/PKG-INFO` & `dtscalibration-3.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dtscalibration
-Version: 3.0.0
+Version: 3.0.2
 Summary: Load Distributed Temperature Sensing (DTS) files, calibrate the temperature and estimate its uncertainty.
 Author: Bas des Tombe, Bart Schilperoort
 Maintainer: Bas des Tombe, Bart Schilperoort
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: DTS,calibration,confidence intervals,distributed temperature sensing
@@ -93,15 +93,15 @@
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.2.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -135,22 +135,24 @@
 
 .. code-block:: zsh
 
     pip install https://github.com/dtscalibration/python-dts-calibration/zipball/main --upgrade
 
 Package features
 ================
+DTS measures temperature by calibrating backscatter measurements to sections with a known temperature. DTS devices provide a simple interface to perform a limited calibration. Re-calibrating your measurements with this Python package gives you better temperature estimates and additional options.
+
 * Advanced calibration routine
-   * Both single- and double-ended setups
-   * Confidence intervals of calibrated temperature
-   * Time integration of calibration parameters
+   * Supports `single <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_- and `double-ended <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_ setups
+   * Compute uncertainty of the calibrated temperature
+   * All measurements are used to estimate parameter values that are constant over time.
    * Weighted least-squares calibration
-   * `Fixing parameters to a previously determined value <..//main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
-   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_
-   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_
+   * `Fixing parameters to a previously determined value <../main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
+   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
+   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
 * Dynamic reference section definition
 * Tools for merging and aligning double-ended setups
 * Data formats of most manufacturers are supported
 
 Devices currently supported
 ===========================
 * Silixa Ltd.: **Ultima** & **XT-DTS** .xml files *(up to version 8.1)*
@@ -158,15 +160,15 @@
 * AP Sensing: **CP320** .xml files *(single ended only)*
 * SensorTran: **SensorTran 5100** .dat binary files *(single ended only)*
 
 Documentation
 =============
 
 * A full calibration procedure for single-ended setups is presented in notebook `07Calibrate_single_ended.ipynb <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_ and for double-ended setups in `08Calibrate_double_ended.ipynb <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_.
-* Documentation at https://python-dts-calibration.readthedocs.io/ .
+* Documentation at `readthedocs <https://python-dts-calibration.readthedocs.io/en/latest/>`_.
 * Example notebooks (`./docs/notebooks`) that work within the browser can be viewed `here <https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks>`_.
 
 How to cite
 ===========
 The following article explains and discusses the calibration procedure:
 
     des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235
@@ -174,10 +176,10 @@
 Cite the specific implementation / repository via Zenodo:
 
 1. Check the version of `dtscalibration` that is used in your Python console with:
 
     >>> # The following line introduces the .dts accessor for xarray datasets
     >>> import dtscalibration  # noqa: E401
     >>> dtscalibration.__version__
-    '3.0.0'
+    '3.0.1'
 2. Go to `Zenodo <https://zenodo.org/search?q=conceptrecid:%221410097%22&sort=-version&all_versions=True>`_ and follow the link to the version of interest.
 3. The citation is found on the bottom right of the page.
```

