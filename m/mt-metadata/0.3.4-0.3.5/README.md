# Comparing `tmp/mt_metadata-0.3.4.tar.gz` & `tmp/mt_metadata-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mt_metadata-0.3.4.tar", last modified: Wed Feb 28 00:11:36 2024, max compression
+gzip compressed data, was "mt_metadata-0.3.5.tar", last modified: Fri Apr 12 22:16:47 2024, max compression
```

## Comparing `mt_metadata-0.3.4.tar` & `mt_metadata-0.3.5.tar`

### file list

```diff
@@ -1,743 +1,743 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:36.390235 mt_metadata-0.3.4/
--rw-rw-rw-   0        0        0      706 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3684 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     4330 2023-11-15 19:37:13.000000 mt_metadata-0.3.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1080 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     1315 2023-10-18 17:07:51.000000 mt_metadata-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0    17146 2024-02-28 00:11:36.390235 mt_metadata-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    11942 2024-02-28 00:09:56.000000 mt_metadata-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.738591 mt_metadata-0.3.4/docs/
--rw-rw-rw-   0        0        0      625 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.397609 mt_metadata-0.3.4/docs/_build/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.397609 mt_metadata-0.3.4/docs/_build/doctrees/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.811317 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    32094 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_10_0.png
--rw-rw-rw-   0        0        0    23186 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_14_0.png
--rw-rw-rw-   0        0        0    19789 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_18_0.png
--rw-rw-rw-   0        0        0    25725 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_23_1.png
--rw-rw-rw-   0        0        0    57694 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_28_1.png
--rw-rw-rw-   0        0        0    10774 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_6_0.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.397609 mt_metadata-0.3.4/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.933048 mt_metadata-0.3.4/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   541810 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/_build/html/_images/example_mt_file_structure.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:26.021591 mt_metadata-0.3.4/docs/_build/html/_images/math/
--rw-rw-rw-   0        0        0      336 2023-09-28 23:30:27.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/000929b09e824936b9447ff8e01006701b495fba.png
--rw-rw-rw-   0        0        0      359 2023-09-28 23:30:21.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/23f55551d151d663ccc7820ad914a1823ca8ec0f.png
--rw-rw-rw-   0        0        0      135 2023-09-28 23:30:23.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/25f9afeac2f1f1f07e08db039b0d28955403ecc4.png
--rw-rw-rw-   0        0        0      293 2023-09-28 23:30:26.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/49562190f3c3e1653c3689177a1258bec888cecc.png
--rw-rw-rw-   0        0        0      203 2023-09-28 23:30:20.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/53bb25e8239563a86c5137ae758534125005551b.png
--rw-rw-rw-   0        0        0      340 2023-09-28 23:30:24.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/73aec0fabc50fc9e5d700e44fa7b0238032cedc9.png
--rw-rw-rw-   0        0        0      378 2023-09-28 23:30:22.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/c5a9382b989cdc1162ca003d6fe23230ff82fd5c.png
--rw-rw-rw-   0        0        0      298 2023-09-28 23:30:25.000000 mt_metadata-0.3.4/docs/_build/html/_images/math/e2533258291b316cd7c9150be2f6f692e5cafbdd.png
--rw-rw-rw-   0        0        0  1344293 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/_build/html/_images/reference_frame.png
--rw-rw-rw-   0        0        0    32094 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_10_0.png
--rw-rw-rw-   0        0        0    23186 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_14_0.png
--rw-rw-rw-   0        0        0    19789 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_18_0.png
--rw-rw-rw-   0        0        0    25725 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_23_1.png
--rw-rw-rw-   0        0        0    57694 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_28_1.png
--rw-rw-rw-   0        0        0    10774 2023-09-28 21:37:45.000000 mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_6_0.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:26.074040 mt_metadata-0.3.4/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-07-26 21:54:07.000000 mt_metadata-0.3.4/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mt_metadata-0.3.4/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/_build/html/_static/mt_metadata_logo.png
--rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mt_metadata-0.3.4/docs/_build/html/_static/plus.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:26.074040 mt_metadata-0.3.4/docs/_static/
--rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/_static/mt_metadata_logo.png
--rw-rw-rw-   0        0        0       29 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/authors.rst
--rw-rw-rw-   0        0        0     5566 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/contributing.rst
--rw-rw-rw-   0        0        0      716 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/conventions.rst
--rw-rw-rw-   0        0        0       29 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/history.rst
--rw-rw-rw-   0        0        0     2559 2023-09-29 16:49:35.000000 mt_metadata-0.3.4/docs/index.rst
--rw-rw-rw-   0        0        0     1755 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/make.bat
--rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/mt_metadata_logo.png
--rw-rw-rw-   0        0        0     1224 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:28.844020 mt_metadata-0.3.4/docs/source/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:28.859640 mt_metadata-0.3.4/docs/source/images/
--rw-rw-rw-   0        0        0   541810 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/images/example_mt_file_structure.png
--rw-rw-rw-   0        0        0  1344293 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/images/reference_frame.png
--rw-rw-rw-   0        0        0       77 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/modules.rst
--rw-rw-rw-   0        0        0      736 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.base.rst
--rw-rw-rw-   0        0        0      265 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.data.rst
--rw-rw-rw-   0        0        0      219 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.data.stationxml.rst
--rw-rw-rw-   0        0        0      348 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.rst
--rw-rw-rw-   0        0        0     3057 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.filters.rst
--rw-rw-rw-   0        0        0      258 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.filters.standards.rst
--rw-rw-rw-   0        0        0     5545 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.rst
--rw-rw-rw-   0        0        0      234 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.standards.rst
--rw-rw-rw-   0        0        0     2106 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.stationxml.rst
--rw-rw-rw-   0        0        0      499 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.tools.rst
--rw-rw-rw-   0        0        0     2101 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.edi.metadata.rst
--rw-rw-rw-   0        0        0      308 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.edi.metadata.standards.rst
--rw-rw-rw-   0        0        0      604 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.edi.rst
--rw-rw-rw-   0        0        0     8784 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.rst
--rw-rw-rw-   0        0        0      320 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.standards.rst
--rw-rw-rw-   0        0        0      644 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.emtfxml.rst
--rw-rw-rw-   0        0        0     1583 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.rst
--rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.standards.rst
--rw-rw-rw-   0        0        0      631 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.jfiles.rst
--rw-rw-rw-   0        0        0      761 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.rst
--rw-rw-rw-   0        0        0      701 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.rst
--rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.standards.rst
--rw-rw-rw-   0        0        0      625 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zfiles.rst
--rw-rw-rw-   0        0        0     3091 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.rst
--rw-rw-rw-   0        0        0      314 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.standards.rst
--rw-rw-rw-   0        0        0      624 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zonge.rst
--rw-rw-rw-   0        0        0      591 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.rst
--rw-rw-rw-   0        0        0     1343 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.tf.rst
--rw-rw-rw-   0        0        0      269 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.tf.standards.rst
--rw-rw-rw-   0        0        0     1117 2023-09-28 21:57:13.000000 mt_metadata-0.3.4/docs/source/mt_metadata.utils.rst
--rw-rw-rw-   0        0        0     6296 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/structure.rst
--rw-rw-rw-   0        0        0    75115 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_auxiliary.rst
--rw-rw-rw-   0        0        0     9860 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_battery.rst
--rw-rw-rw-   0        0        0    75111 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_channel.rst
--rw-rw-rw-   0        0        0    13746 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_citation.rst
--rw-rw-rw-   0        0        0     5928 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_comment.rst
--rw-rw-rw-   0        0        0     2046 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_copyright.rst
--rw-rw-rw-   0        0        0    47501 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_data_logger.rst
--rw-rw-rw-   0        0        0    15797 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_data_quality.rst
--rw-rw-rw-   0        0        0     7895 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_declination.rst
--rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_diagnostic.rst
--rw-rw-rw-   0        0        0    21536 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_data_section.rst
--rw-rw-rw-   0        0        0    17690 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_define_measurement.rst
--rw-rw-rw-   0        0        0    19563 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_e_measurement.rst
--rw-rw-rw-   0        0        0    15671 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_h_measurement.rst
--rw-rw-rw-   0        0        0    79587 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_header.rst
--rw-rw-rw-   0        0        0      307 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_index.rst
--rw-rw-rw-   0        0        0       77 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_edi_information.rst
--rw-rw-rw-   0        0        0   144298 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_electric.rst
--rw-rw-rw-   0        0        0    27399 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_electrode.rst
--rw-rw-rw-   0        0        0     3999 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_attachment.rst
--rw-rw-rw-   0        0        0     3973 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_channels.rst
--rw-rw-rw-   0        0        0    15713 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_citation.rst
--rw-rw-rw-   0        0        0     5928 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_comment.rst
--rw-rw-rw-   0        0        0    27446 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_copyright.rst
--rw-rw-rw-   0        0        0    11901 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_data_quality_notes.rst
--rw-rw-rw-   0        0        0     2044 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_data_quality_warnings.rst
--rw-rw-rw-   0        0        0    17676 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_data_type.rst
--rw-rw-rw-   0        0        0     2046 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_data_types.rst
--rw-rw-rw-   0        0        0     9846 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_dipole.rst
--rw-rw-rw-   0        0        0     9854 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_e_m_t_f.rst
--rw-rw-rw-   0        0        0    15663 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_electric.rst
--rw-rw-rw-   0        0        0     5946 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_electrode.rst
--rw-rw-rw-   0        0        0    11815 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_estimate.rst
--rw-rw-rw-   0        0        0     3991 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_external_url.rst
--rw-rw-rw-   0        0        0       75 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_field_notes.rst
--rw-rw-rw-   0        0        0     1100 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_index.rst
--rw-rw-rw-   0        0        0    11803 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_instrument.rst
--rw-rw-rw-   0        0        0    39355 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_location.rst
--rw-rw-rw-   0        0        0     9822 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_magnetic.rst
--rw-rw-rw-   0        0        0    11807 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_magnetometer.rst
--rw-rw-rw-   0        0        0     4025 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_orientation.rst
--rw-rw-rw-   0        0        0     3975 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_period_range.rst
--rw-rw-rw-   0        0        0     7877 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_person.rst
--rw-rw-rw-   0        0        0     2036 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_primary_data.rst
--rw-rw-rw-   0        0        0    93909 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_processing_info.rst
--rw-rw-rw-   0        0        0     5956 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_processing_software.rst
--rw-rw-rw-   0        0        0    19787 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_provenance.rst
--rw-rw-rw-   0        0        0    75668 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_remote_info.rst
--rw-rw-rw-   0        0        0     2024 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_remote_ref.rst
--rw-rw-rw-   0        0        0    27609 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_run.rst
--rw-rw-rw-   0        0        0    75231 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_site.rst
--rw-rw-rw-   0        0        0     4019 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_site_layout.rst
--rw-rw-rw-   0        0        0     5936 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_software.rst
--rw-rw-rw-   0        0        0     2066 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_statistical_estimates.rst
--rw-rw-rw-   0        0        0       87 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_emtfxml_transfer_function.rst
--rw-rw-rw-   0        0        0    11853 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_fdsn.rst
--rw-rw-rw-   0        0        0    23643 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/tf_filter.rst
--rw-rw-rw-   0        0        0    13782 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_filter_base.rst
--rw-rw-rw-   0        0        0     5938 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_filtered.rst
--rw-rw-rw-   0        0        0      715 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_index.rst
--rw-rw-rw-   0        0        0     9844 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_instrument.rst
--rw-rw-rw-   0        0        0     5936 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_jfile_birrp_angles.rst
--rw-rw-rw-   0        0        0     9846 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_jfile_birrp_block.rst
--rw-rw-rw-   0        0        0    43075 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_jfile_birrp_parameters.rst
--rw-rw-rw-   0        0        0    45218 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_jfile_header.rst
--rw-rw-rw-   0        0        0      265 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_jfile_index.rst
--rw-rw-rw-   0        0        0    39355 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_location.rst
--rw-rw-rw-   0        0        0    88902 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_magnetic.rst
--rw-rw-rw-   0        0        0     7951 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_orientation.rst
--rw-rw-rw-   0        0        0    11801 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_person.rst
--rw-rw-rw-   0        0        0    13838 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_band.rst
--rw-rw-rw-   0        0        0     3983 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_channel.rst
--rw-rw-rw-   0        0        0     9828 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_channel_nomenclature.rst
--rw-rw-rw-   0        0        0     7903 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_decimation.rst
--rw-rw-rw-   0        0        0    53500 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_decimation_level.rst
--rw-rw-rw-   0        0        0     4011 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_estimator.rst
--rw-rw-rw-   0        0        0      593 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_index.rst
--rw-rw-rw-   0        0        0    27803 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_processing.rst
--rw-rw-rw-   0        0        0     6014 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_regression.rst
--rw-rw-rw-   0        0        0     9884 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_run.rst
--rw-rw-rw-   0        0        0     7883 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_station.rst
--rw-rw-rw-   0        0        0     9888 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_stations.rst
--rw-rw-rw-   0        0        0     9876 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_aurora_window.rst
--rw-rw-rw-   0        0        0    11921 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_fcs_channel.rst
--rw-rw-rw-   0        0        0    37582 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_fcs_decimation.rst
--rw-rw-rw-   0        0        0    13850 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_fcs_f_c.rst
--rw-rw-rw-   0        0        0      265 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_processing_fcs_index.rst
--rw-rw-rw-   0        0        0    49368 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_provenance.rst
--rw-rw-rw-   0        0        0     5930 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_rating.rst
--rw-rw-rw-   0        0        0    83521 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_run.rst
--rw-rw-rw-   0        0        0     7901 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_software.rst
--rw-rw-rw-   0        0        0   203675 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_station.rst
--rw-rw-rw-   0        0        0    11867 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_statistical_estimate.rst
--rw-rw-rw-   0        0        0     4248 2023-09-28 22:04:55.000000 mt_metadata-0.3.4/docs/source/tf_structure.rst
--rw-rw-rw-   0        0        0    95093 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_survey.rst
--rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_time_period.rst
--rw-rw-rw-   0        0        0     9874 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_timing_system.rst
--rw-rw-rw-   0        0        0    53534 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_transfer_function.rst
--rw-rw-rw-   0        0        0     9836 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zmm_channel.rst
--rw-rw-rw-   0        0        0      180 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zmm_index.rst
--rw-rw-rw-   0        0        0     2026 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_auto.rst
--rw-rw-rw-   0        0        0    15697 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_c_h.rst
--rw-rw-rw-   0        0        0     2014 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_d_plus.rst
--rw-rw-rw-   0        0        0     7873 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_g_d_p.rst
--rw-rw-rw-   0        0        0     7875 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_g_p_s.rst
--rw-rw-rw-   0        0        0    92430 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_header.rst
--rw-rw-rw-   0        0        0      485 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_index.rst
--rw-rw-rw-   0        0        0     3961 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_job.rst
--rw-rw-rw-   0        0        0     3969 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_line.rst
--rw-rw-rw-   0        0        0     9922 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_m_t_edit.rst
--rw-rw-rw-   0        0        0     2024 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_m_t_f_t24.rst
--rw-rw-rw-   0        0        0     3989 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_phase_slope.rst
--rw-rw-rw-   0        0        0    19607 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_rx.rst
--rw-rw-rw-   0        0        0     2012 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_s_t_n.rst
--rw-rw-rw-   0        0        0     9838 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_survey.rst
--rw-rw-rw-   0        0        0     2010 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_tx.rst
--rw-rw-rw-   0        0        0     5908 2023-09-29 00:06:36.000000 mt_metadata-0.3.4/docs/source/tf_zonge_unit.rst
--rw-rw-rw-   0        0        0    75115 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_auxiliary.rst
--rw-rw-rw-   0        0        0     9860 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_battery.rst
--rw-rw-rw-   0        0        0    75111 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_channel.rst
--rw-rw-rw-   0        0        0    13746 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_citation.rst
--rw-rw-rw-   0        0        0     2046 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_copyright.rst
--rw-rw-rw-   0        0        0    47501 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_data_logger.rst
--rw-rw-rw-   0        0        0    15797 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_data_quality.rst
--rw-rw-rw-   0        0        0     7895 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_declination.rst
--rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_diagnostic.rst
--rw-rw-rw-   0        0        0   144298 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_electric.rst
--rw-rw-rw-   0        0        0    27399 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_electrode.rst
--rw-rw-rw-   0        0        0       75 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_experiment.rst
--rw-rw-rw-   0        0        0    11853 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_fdsn.rst
--rw-rw-rw-   0        0        0    13782 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_base.rst
--rw-rw-rw-   0        0        0     2086 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_channel_response_filter.rst
--rw-rw-rw-   0        0        0    13796 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_coefficient_filter.rst
--rw-rw-rw-   0        0        0    23653 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_f_i_r_filter.rst
--rw-rw-rw-   0        0        0    21674 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_frequency_response_table_filter.rst
--rw-rw-rw-   0        0        0      385 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_index.rst
--rw-rw-rw-   0        0        0    19679 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_pole_zero_filter.rst
--rw-rw-rw-   0        0        0    15745 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filter_time_delay_filter.rst
--rw-rw-rw-   0        0        0     5938 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_filtered.rst
--rw-rw-rw-   0        0        0    11819 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_funding_source.rst
--rw-rw-rw-   0        0        0    13784 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_geographic_location.rst
--rw-rw-rw-   0        0        0      708 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_index.rst
--rw-rw-rw-   0        0        0     9844 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_instrument.rst
--rw-rw-rw-   0        0        0    39355 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_location.rst
--rw-rw-rw-   0        0        0    88902 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_magnetic.rst
--rw-rw-rw-   0        0        0    16149 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/source/ts_metadata_guide.rst
--rw-rw-rw-   0        0        0     7951 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_orientation.rst
--rw-rw-rw-   0        0        0    11801 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_person.rst
--rw-rw-rw-   0        0        0    49368 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_provenance.rst
--rw-rw-rw-   0        0        0     5930 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_rating.rst
--rw-rw-rw-   0        0        0    83521 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_run.rst
--rw-rw-rw-   0        0        0     7901 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_software.rst
--rw-rw-rw-   0        0        0   150763 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_station.rst
--rw-rw-rw-   0        0        0    95093 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_survey.rst
--rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_time_period.rst
--rw-rw-rw-   0        0        0     9874 2023-09-29 00:06:35.000000 mt_metadata-0.3.4/docs/source/ts_timing_system.rst
--rw-rw-rw-   0        0        0     1965 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:28.890883 mt_metadata-0.3.4/mt_metadata/
--rw-rw-rw-   0        0        0     5588 2024-02-28 00:09:56.000000 mt_metadata-0.3.4/mt_metadata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:29.039399 mt_metadata-0.3.4/mt_metadata/base/
--rw-rw-rw-   0        0        0      184 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/base/__init__.py
--rw-rw-rw-   0        0        0    19721 2023-09-29 00:06:09.000000 mt_metadata-0.3.4/mt_metadata/base/helpers.py
--rw-rw-rw-   0        0        0    27012 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/base/metadata.py
--rw-rw-rw-   0        0        0    12842 2023-07-18 00:34:28.000000 mt_metadata-0.3.4/mt_metadata/base/schema.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:29.056356 mt_metadata-0.3.4/mt_metadata/data/
--rw-rw-rw-   0        0        0      217 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:29.128785 mt_metadata-0.3.4/mt_metadata/data/mt_xml/
--rw-rw-rw-   0        0        0       26 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/mt_xml/__init__.py
--rw-rw-rw-   0        0        0    57690 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/mt_xml/multi_run_experiment.xml
--rw-rw-rw-   0        0        0   236665 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/mt_xml/multi_run_experiment_02.xml
--rw-rw-rw-   0        0        0    86356 2023-07-18 00:25:45.000000 mt_metadata-0.3.4/mt_metadata/data/mt_xml/single_station_mt_experiment.xml
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:29.275897 mt_metadata-0.3.4/mt_metadata/data/stationxml/
--rw-rw-rw-   0        0        0      217 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/__init__.py
--rw-rw-rw-   0        0        0    12650 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/fdsn_no_mt_info.xml
--rw-rw-rw-   0        0        0    13230 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_electrode_example.xml
--rw-rw-rw-   0        0        0     9883 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_magnetometer_example.xml
--rw-rw-rw-   0        0        0   117239 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_single_station.xml
--rw-rw-rw-   0        0        0    76110 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/multiple_networks_example.xml
--rw-rw-rw-   0        0        0   105469 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/station_xml_with_fap_example.xml
--rw-rw-rw-   0        0        0   492319 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/stationxml/station_xml_with_fir_example.xml
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:29.761030 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/
--rw-rw-rw-   0        0        0   102844 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/NMX20.xml
--rw-rw-rw-   0        0        0    61145 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/PHXTest01.edi
--rw-rw-rw-   0        0        0       26 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/__init__.py
--rw-rw-rw-   0        0        0    31883 2023-09-27 22:58:29.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/example.xml
--rw-rw-rw-   0        0        0    32990 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/test.edi
--rw-rw-rw-   0        0        0    13326 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg.avg
--rw-rw-rw-   0        0        0    38811 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg_newer.avg
--rw-rw-rw-   0        0        0    39033 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg_tipper.avg
--rw-rw-rw-   0        0        0    46663 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_cgg.edi
--rw-rw-rw-   0        0        0    39022 2023-08-29 22:52:18.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_empower.edi
--rw-rw-rw-   0        0        0    34562 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_metronix.edi
--rw-rw-rw-   0        0        0    12987 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_no_error.edi
--rw-rw-rw-   0        0        0    61195 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_phoenix.edi
--rw-rw-rw-   0        0        0    31042 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_quantec.edi
--rw-rw-rw-   0        0        0     4895 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_rho_only.edi
--rw-rw-rw-   0        0        0    25251 2023-09-08 21:45:40.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_spectra_in.edi
--rw-rw-rw-   0        0        0    13446 2023-09-08 21:45:57.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_spectra_out.edi
--rw-rw-rw-   0        0        0    14251 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_jfile.j
--rw-rw-rw-   0        0        0    30095 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_poor_xml.xml
--rw-rw-rw-   0        0        0    92001 2023-06-09 21:33:27.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml.xml
--rw-rw-rw-   0        0        0    37102 2023-07-18 00:25:45.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_bad_comments.xml
--rw-rw-rw-   0        0        0    82850 2023-07-18 00:25:45.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_complete_remote_info.xml
--rw-rw-rw-   0        0        0    28104 2023-07-18 00:25:45.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_emtf_xml_iris.xml
--rw-rw-rw-   0        0        0    26903 2023-08-22 19:08:40.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_multiple_attachments.xml
--rw-rw-rw-   0        0        0    28593 2023-09-26 23:49:26.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_no_site_layout.xml
--rw-rw-rw-   0        0        0    96949 2023-07-18 00:25:45.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_with_derived_quantities.xml
--rw-rw-rw-   0        0        0    22671 2024-02-02 22:18:05.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_zmm.zmm
--rw-rw-rw-   0        0        0    16981 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_zss_tipper.zss
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:30.277871 mt_metadata-0.3.4/mt_metadata/timeseries/
--rw-rw-rw-   0        0        0     3339 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/__init__.py
--rw-rw-rw-   0        0        0      827 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/auxiliary.py
--rw-rw-rw-   0        0        0      965 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/battery.py
--rw-rw-rw-   0        0        0     3112 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/channel.py
--rw-rw-rw-   0        0        0      828 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/citation.py
--rw-rw-rw-   0        0        0      892 2023-09-26 20:16:48.000000 mt_metadata-0.3.4/mt_metadata/timeseries/copyright.py
--rw-rw-rw-   0        0        0     1542 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/data_logger.py
--rw-rw-rw-   0        0        0      962 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/data_quality.py
--rw-rw-rw-   0        0        0      995 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/declination.py
--rw-rw-rw-   0        0        0      834 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/diagnostic.py
--rw-rw-rw-   0        0        0     1745 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/electric.py
--rw-rw-rw-   0        0        0      997 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/electrode.py
--rw-rw-rw-   0        0        0    21016 2023-07-17 00:32:53.000000 mt_metadata-0.3.4/mt_metadata/timeseries/experiment.py
--rw-rw-rw-   0        0        0      822 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/fdsn.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:30.509601 mt_metadata-0.3.4/mt_metadata/timeseries/filters/
--rw-rw-rw-   0        0        0      474 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/__init__.py
--rw-rw-rw-   0        0        0    17297 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/channel_response.py
--rw-rw-rw-   0        0        0     3322 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/coefficient_filter.py
--rw-rw-rw-   0        0        0    12885 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/filter_base.py
--rw-rw-rw-   0        0        0     6979 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/filtered.py
--rw-rw-rw-   0        0        0     6767 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/fir_filter.py
--rw-rw-rw-   0        0        0     7396 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/frequency_response_table_filter.py
--rw-rw-rw-   0        0        0     4124 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/helper_functions.py
--rw-rw-rw-   0        0        0     5916 2023-07-18 00:34:28.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/obspy_stages.py
--rw-rw-rw-   0        0        0     6796 2023-04-21 23:00:09.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/plotting_helpers.py
--rw-rw-rw-   0        0        0     6724 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/pole_zero_filter.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:30.639195 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/__init__.py
--rw-rw-rw-   0        0        0      291 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/channel_response.json
--rw-rw-rw-   0        0        0      297 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/coefficient_filter.json
--rw-rw-rw-   0        0        0     2663 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/filter_base.json
--rw-rw-rw-   0        0        0     1582 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/fir_filter.json
--rw-rw-rw-   0        0        0     1506 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/frequency_response_table_filter.json
--rw-rw-rw-   0        0        0      994 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/pole_zero_filter.json
--rw-rw-rw-   0        0        0      327 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/time_delay_filter.json
--rw-rw-rw-   0        0        0     3257 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/filters/time_delay_filter.py
--rw-rw-rw-   0        0        0      841 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/funding_source.py
--rw-rw-rw-   0        0        0      851 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/geographic_location.py
--rw-rw-rw-   0        0        0      834 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/instrument.py
--rw-rw-rw-   0        0        0     7437 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/location.py
--rw-rw-rw-   0        0        0     1746 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/magnetic.py
--rw-rw-rw-   0        0        0      836 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/orientation.py
--rw-rw-rw-   0        0        0      971 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/person.py
--rw-rw-rw-   0        0        0     1605 2023-04-21 23:00:09.000000 mt_metadata-0.3.4/mt_metadata/timeseries/provenance.py
--rw-rw-rw-   0        0        0      826 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/rating.py
--rw-rw-rw-   0        0        0    14009 2023-09-13 20:58:32.000000 mt_metadata-0.3.4/mt_metadata/timeseries/run.py
--rw-rw-rw-   0        0        0     1224 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/software.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.048220 mt_metadata-0.3.4/mt_metadata/timeseries/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/__init__.py
--rw-rw-rw-   0        0        0     4746 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/auxiliary.json
--rw-rw-rw-   0        0        0     1408 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/battery.json
--rw-rw-rw-   0        0        0     5144 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/channel.json
--rw-rw-rw-   0        0        0     2030 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/citation.json
--rw-rw-rw-   0        0        0    12478 2023-11-09 00:17:46.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/copyright.json
--rw-rw-rw-   0        0        0     1506 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/data_quality.json
--rw-rw-rw-   0        0        0     1402 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/declination.json
--rw-rw-rw-   0        0        0      585 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/diagnostic.json
--rw-rw-rw-   0        0        0     2493 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/electric.json
--rw-rw-rw-   0        0        0     1949 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/fdsn.json
--rw-rw-rw-   0        0        0     1159 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/filtered.json
--rw-rw-rw-   0        0        0     1756 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/funding_source.json
--rw-rw-rw-   0        0        0     2223 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/geographic_location.json
--rw-rw-rw-   0        0        0     1533 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/instrument.json
--rw-rw-rw-   0        0        0     5294 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/location.json
--rw-rw-rw-   0        0        0     1291 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/magnetic.json
--rw-rw-rw-   0        0        0     1866 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/orientation.json
--rw-rw-rw-   0        0        0     1772 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/person.json
--rw-rw-rw-   0        0        0      981 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/provenance.json
--rw-rw-rw-   0        0        0     1029 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/rating.json
--rw-rw-rw-   0        0        0     2500 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/run.json
--rw-rw-rw-   0        0        0     1199 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/software.json
--rw-rw-rw-   0        0        0     2990 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/station.json
--rw-rw-rw-   0        0        0     3426 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/survey.json
--rw-rw-rw-   0        0        0      681 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/time_period.json
--rw-rw-rw-   0        0        0     1492 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/standards/timing_system.json
--rw-rw-rw-   0        0        0     9855 2023-09-13 20:51:05.000000 mt_metadata-0.3.4/mt_metadata/timeseries/station.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.198032 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/
--rw-rw-rw-   0        0        0      525 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/__init__.py
--rw-rw-rw-   0        0        0     9487 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/fdsn_tools.py
--rw-rw-rw-   0        0        0     7257 2023-08-18 20:44:09.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/utils.py
--rw-rw-rw-   0        0        0    20289 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_channel_mt_channel.py
--rw-rw-rw-   0        0        0     5151 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_equipment_mt_run.py
--rw-rw-rw-   0        0        0    13893 2023-07-18 00:34:28.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_inventory_mt_experiment.py
--rw-rw-rw-   0        0        0     7124 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_network_mt_survey.py
--rw-rw-rw-   0        0        0    11112 2023-08-18 21:16:21.000000 mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_station_mt_station.py
--rw-rw-rw-   0        0        0    11831 2023-09-13 20:49:58.000000 mt_metadata-0.3.4/mt_metadata/timeseries/survey.py
--rw-rw-rw-   0        0        0     1653 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/time_period.py
--rw-rw-rw-   0        0        0      839 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/timing_system.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.248420 mt_metadata-0.3.4/mt_metadata/timeseries/tools/
--rw-rw-rw-   0        0        0       78 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/tools/__init__.py
--rw-rw-rw-   0        0        0    14300 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/timeseries/tools/from_many_mt_files.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.279665 mt_metadata-0.3.4/mt_metadata/transfer_functions/
--rw-rw-rw-   0        0        0       42 2024-02-03 00:29:59.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/__init__.py
--rw-rw-rw-   0        0        0    79933 2024-02-27 19:19:47.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/core.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.317416 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/
--rw-rw-rw-   0        0        0      215 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.348665 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/
--rw-rw-rw-   0        0        0       61 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/__init__.py
--rw-rw-rw-   0        0        0    53305 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/edi.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.495769 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/
--rw-rw-rw-   0        0        0      395 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/__init__.py
--rw-rw-rw-   0        0        0     7751 2023-07-07 19:34:23.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/data_section.py
--rw-rw-rw-   0        0        0    16264 2024-01-22 22:32:08.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/define_measurement.py
--rw-rw-rw-   0        0        0     3138 2023-11-15 19:20:01.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/emeasurement.py
--rw-rw-rw-   0        0        0     9203 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/header.py
--rw-rw-rw-   0        0        0     2245 2023-09-05 19:26:53.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/hmeasurement.py
--rw-rw-rw-   0        0        0    17062 2023-08-31 17:14:39.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/information.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.580393 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/__init__.py
--rw-rw-rw-   0        0        0     3045 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/data_section.json
--rw-rw-rw-   0        0        0     2572 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/define_measurement.json
--rw-rw-rw-   0        0        0     3100 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/emeasurement.json
--rw-rw-rw-   0        0        0     6444 2023-04-21 23:00:09.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/header.json
--rw-rw-rw-   0        0        0     2450 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/hmeasurement.json
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:31.618145 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/
--rw-rw-rw-   0        0        0       73 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/__init__.py
--rw-rw-rw-   0        0        0    53432 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/emtfxml.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:32.297721 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/
--rw-rw-rw-   0        0        0     2364 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/__init__.py
--rw-rw-rw-   0        0        0     2459 2023-08-22 20:58:11.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/attachment.py
--rw-rw-rw-   0        0        0      889 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/channels.py
--rw-rw-rw-   0        0        0     1500 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/citation.py
--rw-rw-rw-   0        0        0     2409 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/comment.py
--rw-rw-rw-   0        0        0     1802 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/copyright.py
--rw-rw-rw-   0        0        0    14720 2023-09-27 22:58:29.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data.py
--rw-rw-rw-   0        0        0     2325 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_notes.py
--rw-rw-rw-   0        0        0     1769 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_warnings.py
--rw-rw-rw-   0        0        0     1919 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_type.py
--rw-rw-rw-   0        0        0     2349 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_types.py
--rw-rw-rw-   0        0        0     2414 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/dipole.py
--rw-rw-rw-   0        0        0     1952 2023-09-01 00:47:17.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/electric.py
--rw-rw-rw-   0        0        0     1398 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/electrode.py
--rw-rw-rw-   0        0        0      773 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/emtf.py
--rw-rw-rw-   0        0        0     2038 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/estimate.py
--rw-rw-rw-   0        0        0     1172 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/external_url.py
--rw-rw-rw-   0        0        0     1766 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/field_notes.py
--rw-rw-rw-   0        0        0     4494 2023-09-19 23:57:00.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/helpers.py
--rw-rw-rw-   0        0        0     1406 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/instrument.py
--rw-rw-rw-   0        0        0     9283 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/location.py
--rw-rw-rw-   0        0        0     1807 2023-09-01 00:47:17.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetic.py
--rw-rw-rw-   0        0        0     1343 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetometer.py
--rw-rw-rw-   0        0        0     2493 2023-08-15 19:40:16.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/orientation.py
--rw-rw-rw-   0        0        0     1633 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/period_range.py
--rw-rw-rw-   0        0        0      830 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/person.py
--rw-rw-rw-   0        0        0     1018 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/primary_data.py
--rw-rw-rw-   0        0        0     3208 2023-08-29 22:52:18.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/processing_info.py
--rw-rw-rw-   0        0        0     2425 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/provenance.py
--rw-rw-rw-   0        0        0     2291 2023-09-27 00:04:02.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_info.py
--rw-rw-rw-   0        0        0     1724 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_ref.py
--rw-rw-rw-   0        0        0     4848 2023-09-07 20:40:13.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/run.py
--rw-rw-rw-   0        0        0     4046 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/site.py
--rw-rw-rw-   0        0        0     6092 2023-09-27 00:25:52.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/site_layout.py
--rw-rw-rw-   0        0        0     1942 2023-08-29 22:52:18.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/software.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:32.814130 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/attachment.json
--rw-rw-rw-   0        0        0      565 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/channels.json
--rw-rw-rw-   0        0        0     2269 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/citation.json
--rw-rw-rw-   0        0        0      880 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/comment.json
--rw-rw-rw-   0        0        0     2477 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/copyright.json
--rw-rw-rw-   0        0        0      942 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_notes.json
--rw-rw-rw-   0        0        0      273 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_warnings.json
--rw-rw-rw-   0        0        0     2995 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_type.json
--rw-rw-rw-   0        0        0      284 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_types.json
--rw-rw-rw-   0        0        0      374 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/description.json
--rw-rw-rw-   0        0        0     1419 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/dipole.json
--rw-rw-rw-   0        0        0     2436 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electric.json
--rw-rw-rw-   0        0        0      958 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electrode.json
--rw-rw-rw-   0        0        0     1675 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/emtf.json
--rw-rw-rw-   0        0        0     2069 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/estimate.json
--rw-rw-rw-   0        0        0      638 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/external_url.json
--rw-rw-rw-   0        0        0     5294 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/location.json
--rw-rw-rw-   0        0        0     1483 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetic.json
--rw-rw-rw-   0        0        0     1814 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetometer.json
--rw-rw-rw-   0        0        0      675 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/orientation.json
--rw-rw-rw-   0        0        0      563 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/period_range.json
--rw-rw-rw-   0        0        0     1198 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/person.json
--rw-rw-rw-   0        0        0      319 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/primary_data.json
--rw-rw-rw-   0        0        0     1340 2023-08-29 22:52:18.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/processing_info.json
--rw-rw-rw-   0        0        0      707 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/provenance.json
--rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/remote_ref.json
--rw-rw-rw-   0        0        0     1486 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/run.json
--rw-rw-rw-   0        0        0     3240 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site.json
--rw-rw-rw-   0        0        0      696 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site_layout.json
--rw-rw-rw-   0        0        0      892 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/software.json
--rw-rw-rw-   0        0        0      298 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/statistical_estimates.json
--rw-rw-rw-   0        0        0     1097 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/value.json
--rw-rw-rw-   0        0        0     2429 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/statistical_estimates.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:32.851899 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/
--rw-rw-rw-   0        0        0       67 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/__init__.py
--rw-rw-rw-   0        0        0    13676 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/jfile.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:32.936518 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/
--rw-rw-rw-   0        0        0      265 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/__init__.py
--rw-rw-rw-   0        0        0      835 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_angles.py
--rw-rw-rw-   0        0        0      833 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_block.py
--rw-rw-rw-   0        0        0      843 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_parameters.py
--rw-rw-rw-   0        0        0     5207 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/header.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:32.999004 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/__init__.py
--rw-rw-rw-   0        0        0      830 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_angles.json
--rw-rw-rw-   0        0        0     1381 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_block.json
--rw-rw-rw-   0        0        0     6105 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_parameters.json
--rw-rw-rw-   0        0        0      846 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/header.json
--rw-rw-rw-   0        0        0     6024 2023-09-26 18:25:53.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.036763 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/
--rw-rw-rw-   0        0        0       61 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.068005 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/
--rw-rw-rw-   0        0        0       73 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/__init__.py
--rw-rw-rw-   0        0        0     2224 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/channel.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.099251 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/standards/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/standards/channel.json
--rw-rw-rw-   0        0        0    35850 2024-02-03 00:29:59.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/zmm.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.121376 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/
--rw-rw-rw-   0        0        0       77 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.421730 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/
--rw-rw-rw-   0        0        0      646 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/__init__.py
--rw-rw-rw-   0        0        0      801 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/auto.py
--rw-rw-rw-   0        0        0      795 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/ch.py
--rw-rw-rw-   0        0        0      804 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/d_plus.py
--rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/gdp.py
--rw-rw-rw-   0        0        0     1222 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/gps.py
--rw-rw-rw-   0        0        0     7700 2023-09-05 21:05:21.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/header.py
--rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/job.py
--rw-rw-rw-   0        0        0      799 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/line.py
--rw-rw-rw-   0        0        0     1173 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/mt_edit.py
--rw-rw-rw-   0        0        0      803 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/mtft24.py
--rw-rw-rw-   0        0        0      814 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/phase_slope.py
--rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/rx.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.669095 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/__init__.py
--rw-rw-rw-   0        0        0      330 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/auto.json
--rw-rw-rw-   0        0        0     2387 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/ch.json
--rw-rw-rw-   0        0        0      308 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/d_plus.json
--rw-rw-rw-   0        0        0     1145 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/gdp.json
--rw-rw-rw-   0        0        0     1113 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/gps.json
--rw-rw-rw-   0        0        0      267 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/header.json
--rw-rw-rw-   0        0        0      559 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/job.json
--rw-rw-rw-   0        0        0      548 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/line.json
--rw-rw-rw-   0        0        0      304 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/mt_edit.json
--rw-rw-rw-   0        0        0      304 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/mtft24.json
--rw-rw-rw-   0        0        0      681 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/phase_slope.json
--rw-rw-rw-   0        0        0     2961 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/rx.json
--rw-rw-rw-   0        0        0      276 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/stn.json
--rw-rw-rw-   0        0        0     1529 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/survey.json
--rw-rw-rw-   0        0        0      323 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/tx.json
--rw-rw-rw-   0        0        0      953 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/unit.json
--rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/stn.py
--rw-rw-rw-   0        0        0      772 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/survey.py
--rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/tx.py
--rw-rw-rw-   0        0        0      801 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/unit.py
--rw-rw-rw-   0        0        0    17203 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/zonge.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.669095 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/
--rw-rw-rw-   0        0        0        2 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:33.893976 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/
--rw-rw-rw-   0        0        0      668 2023-09-26 18:03:00.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/__init__.py
--rw-rw-rw-   0        0        0     8100 2023-09-27 15:25:49.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/band.py
--rw-rw-rw-   0        0        0      773 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/channel.py
--rw-rw-rw-   0        0        0     4264 2024-02-27 19:39:14.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/channel_nomenclature.py
--rw-rw-rw-   0        0        0      785 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/decimation.py
--rw-rw-rw-   0        0        0    10657 2023-09-27 22:58:29.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/decimation_level.py
--rw-rw-rw-   0        0        0      781 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/estimator.py
--rw-rw-rw-   0        0        0    10320 2024-02-23 20:26:16.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/processing.py
--rw-rw-rw-   0        0        0      783 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/regression.py
--rw-rw-rw-   0        0        0     4123 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/run.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.138726 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/
--rw-rw-rw-   0        0        0      135 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-09-26 18:03:01.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/band.json
--rw-rw-rw-   0        0        0      548 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/channel.json
--rw-rw-rw-   0        0        0     1798 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclature.json
--rw-rw-rw-   0        0        0      378 2023-10-23 19:47:34.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclatures.json
--rw-rw-rw-   0        0        0     1007 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/config.json
--rw-rw-rw-   0        0        0     1168 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/decimation.json
--rw-rw-rw-   0        0        0     4176 2023-09-01 00:47:17.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/decimation_level.json
--rw-rw-rw-   0        0        0      628 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/estimator.json
--rw-rw-rw-   0        0        0     1211 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/processing.json
--rw-rw-rw-   0        0        0      901 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/regression.json
--rw-rw-rw-   0        0        0     1423 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/run.json
--rw-rw-rw-   0        0        0     1173 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/station.json
--rw-rw-rw-   0        0        0      276 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/stations.json
--rw-rw-rw-   0        0        0     1892 2023-05-26 17:19:06.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/window.json
--rw-rw-rw-   0        0        0     5163 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/station.py
--rw-rw-rw-   0        0        0     4564 2024-02-23 20:28:07.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/stations.py
--rw-rw-rw-   0        0        0     1210 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/window.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.201212 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/
--rw-rw-rw-   0        0        0      134 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/__init__.py
--rw-rw-rw-   0        0        0    15679 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/decimation.py
--rw-rw-rw-   0        0        0    10450 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/fc.py
--rw-rw-rw-   0        0        0      926 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/fc_channel.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.254620 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/
--rw-rw-rw-   0        0        0      135 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-09-05 19:32:54.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/decimation.json
--rw-rw-rw-   0        0        0     1523 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc.json
--rw-rw-rw-   0        0        0     1873 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc_channel.json
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.364689 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/
--rw-rw-rw-   0        0        0     3890 2023-08-30 20:58:19.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-04-21 23:00:09.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/comment.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.439193 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/
--rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/__init__.py
--rw-rw-rw-   0        0        0      880 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/comment.json
--rw-rw-rw-   0        0        0     2972 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/station.json
--rw-rw-rw-   0        0        0     1917 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/statistical_estimate.json
--rw-rw-rw-   0        0        0     3426 2023-08-30 20:58:01.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/survey.json
--rw-rw-rw-   0        0        0     3220 2023-08-31 18:42:05.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/transfer_function.json
--rw-rw-rw-   0        0        0     9840 2023-09-13 20:50:49.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/station.py
--rw-rw-rw-   0        0        0      857 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/statistical_estimate.py
--rw-rw-rw-   0        0        0    12547 2023-09-13 20:50:32.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/survey.py
--rw-rw-rw-   0        0        0     5094 2024-02-27 23:44:07.000000 mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/transfer_function.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.570675 mt_metadata-0.3.4/mt_metadata/utils/
--rw-rw-rw-   0        0        0       35 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/utils/__init__.py
--rw-rw-rw-   0        0        0      462 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/mt_metadata/utils/exceptions.py
--rw-rw-rw-   0        0        0     7668 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/utils/list_dict.py
--rw-rw-rw-   0        0        0    18719 2023-11-09 00:17:46.000000 mt_metadata-0.3.4/mt_metadata/utils/mttime.py
--rw-rw-rw-   0        0        0     4109 2023-09-26 19:31:14.000000 mt_metadata-0.3.4/mt_metadata/utils/summarize.py
--rw-rw-rw-   0        0        0     6405 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/mt_metadata/utils/units.py
--rw-rw-rw-   0        0        0    16264 2023-07-17 00:32:53.000000 mt_metadata-0.3.4/mt_metadata/utils/validators.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:28.944264 mt_metadata-0.3.4/mt_metadata.egg-info/
--rw-rw-rw-   0        0        0    17146 2024-02-28 00:11:23.000000 mt_metadata-0.3.4/mt_metadata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    32618 2024-02-28 00:11:25.000000 mt_metadata-0.3.4/mt_metadata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 00:11:23.000000 mt_metadata-0.3.4/mt_metadata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-09 00:57:10.000000 mt_metadata-0.3.4/mt_metadata.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2024-02-28 00:11:23.000000 mt_metadata-0.3.4/mt_metadata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-28 00:11:23.000000 mt_metadata-0.3.4/mt_metadata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      462 2024-02-28 00:11:36.390235 mt_metadata-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-02-28 00:09:56.000000 mt_metadata-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.755217 mt_metadata-0.3.4/tests/
--rw-rw-rw-   0        0        0      449 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0    17262 2023-09-29 00:34:39.000000 mt_metadata-0.3.4/tests/test_helpers.py
--rw-rw-rw-   0        0        0     8706 2023-09-27 00:53:43.000000 mt_metadata-0.3.4/tests/test_list_dict.py
--rw-rw-rw-   0        0        0     4330 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/test_metadata.py
--rw-rw-rw-   0        0        0    11801 2023-11-09 00:17:46.000000 mt_metadata-0.3.4/tests/test_mttime.py
--rw-rw-rw-   0        0        0     6200 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/test_schema.py
--rw-rw-rw-   0        0        0     1512 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/test_standards_exist.py
--rw-rw-rw-   0        0        0     2775 2023-09-26 19:52:08.000000 mt_metadata-0.3.4/tests/test_summarize.py
--rw-rw-rw-   0        0        0     1488 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/test_units.py
--rw-rw-rw-   0        0        0     9201 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/test_validators.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.881149 mt_metadata-0.3.4/tests/tf/
--rw-rw-rw-   0        0        0       35 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:34.896771 mt_metadata-0.3.4/tests/tf/io/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.071514 mt_metadata-0.3.4/tests/tf/io/edi/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/edi/__init__.py
--rw-rw-rw-   0        0        0    19367 2023-09-05 19:40:11.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_cgg_edi.py
--rw-rw-rw-   0        0        0     7160 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_edi.py
--rw-rw-rw-   0        0        0     9801 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_edi_spectra.py
--rw-rw-rw-   0        0        0    21308 2023-09-05 19:39:04.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_empower_edi.py
--rw-rw-rw-   0        0        0     9148 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_metronix_edi.py
--rw-rw-rw-   0        0        0    10010 2024-02-28 00:09:56.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_no_error_edi.py
--rw-rw-rw-   0        0        0    12082 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_phoenix_edi.py
--rw-rw-rw-   0        0        0     9335 2023-07-07 19:34:23.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_quantec_edi.py
--rw-rw-rw-   0        0        0    13186 2023-04-24 19:02:54.000000 mt_metadata-0.3.4/tests/tf/io/edi/test_rho_only_edi.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.318885 mt_metadata-0.3.4/tests/tf/io/emtfxml/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/__init__.py
--rw-rw-rw-   0        0        0    29088 2023-09-27 01:00:58.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_emtfxml.py
--rw-rw-rw-   0        0        0    18967 2023-09-27 00:01:23.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_emtfxml_poor.py
--rw-rw-rw-   0        0        0     1702 2023-08-22 20:34:43.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_multiple_attachments.py
--rw-rw-rw-   0        0        0    27587 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read.py
--rw-rw-rw-   0        0        0    22989 2023-09-13 17:39:26.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_complete_remote_info.py
--rw-rw-rw-   0        0        0    12554 2023-09-13 17:40:22.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_derived_quantities.py
--rw-rw-rw-   0        0        0    12640 2023-09-13 17:41:06.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_no_site_layout.py
--rw-rw-rw-   0        0        0    14282 2023-09-13 17:42:00.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_poor.py
--rw-rw-rw-   0        0        0     8703 2023-09-07 18:36:05.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write.py
--rw-rw-rw-   0        0        0     8766 2023-09-07 18:43:17.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write_complete_remote_info.py
--rw-rw-rw-   0        0        0     7886 2023-09-07 18:36:41.000000 mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write_poor.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.356643 mt_metadata-0.3.4/tests/tf/io/jfile/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/jfile/__init__.py
--rw-rw-rw-   0        0        0     3537 2023-04-14 17:22:27.000000 mt_metadata-0.3.4/tests/tf/io/jfile/test_jfile.py
--rw-rw-rw-   0        0        0     8602 2023-09-13 18:03:05.000000 mt_metadata-0.3.4/tests/tf/io/jfile/test_tf_read.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.441239 mt_metadata-0.3.4/tests/tf/io/zmm/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/tf/io/zmm/__init__.py
--rw-rw-rw-   0        0        0    18065 2024-02-02 22:18:05.000000 mt_metadata-0.3.4/tests/tf/io/zmm/test_tf_read_zmm.py
--rw-rw-rw-   0        0        0    10338 2024-02-02 22:18:05.000000 mt_metadata-0.3.4/tests/tf/io/zmm/test_tf_read_zss.py
--rw-rw-rw-   0        0        0     8837 2024-02-03 00:29:59.000000 mt_metadata-0.3.4/tests/tf/io/zmm/test_zmm.py
--rw-rw-rw-   0        0        0     6612 2024-02-03 00:29:59.000000 mt_metadata-0.3.4/tests/tf/io/zmm/test_zss.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.557104 mt_metadata-0.3.4/tests/tf/io/zonge/
--rw-rw-rw-   0        0        0       16 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/tf/io/zonge/__init__.py
--rw-rw-rw-   0        0        0     8602 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read.py
--rw-rw-rw-   0        0        0     8646 2024-02-02 18:00:10.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read_newer.py
--rw-rw-rw-   0        0        0    16798 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read_tipper.py
--rw-rw-rw-   0        0        0     4078 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge.py
--rw-rw-rw-   0        0        0     3560 2023-09-26 18:17:45.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge_newer.py
--rw-rw-rw-   0        0        0    16644 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge_tipper.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:25.478215 mt_metadata-0.3.4/tests/tf/processing/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.757590 mt_metadata-0.3.4/tests/tf/processing/aurora/
--rw-rw-rw-   0        0        0        0 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/__init__.py
--rw-rw-rw-   0        0        0     8264 2023-09-27 15:42:38.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_band.py
--rw-rw-rw-   0        0        0     1671 2024-02-27 19:39:14.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_channel_nomenclature.py
--rw-rw-rw-   0        0        0     2489 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_dataset_dataframe.py
--rw-rw-rw-   0        0        0      707 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_decimation.py
--rw-rw-rw-   0        0        0      700 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_estimator.py
--rw-rw-rw-   0        0        0     1642 2023-09-27 22:58:29.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_frequency_bands.py
--rw-rw-rw-   0        0        0     4385 2024-02-23 21:21:05.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_processing.py
--rw-rw-rw-   0        0        0      707 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_regression.py
--rw-rw-rw-   0        0        0      714 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_station.py
--rw-rw-rw-   0        0        0     2558 2024-02-23 21:13:25.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_stations.py
--rw-rw-rw-   0        0        0     1205 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/aurora/test_window.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.820076 mt_metadata-0.3.4/tests/tf/processing/fcs/
--rw-rw-rw-   0        0        0        0 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/fcs/__init__.py
--rw-rw-rw-   0        0        0     7632 2023-09-27 22:58:29.000000 mt_metadata-0.3.4/tests/tf/processing/fcs/test_decimation.py
--rw-rw-rw-   0        0        0     4134 2023-07-18 00:25:46.000000 mt_metadata-0.3.4/tests/tf/processing/fcs/test_fc.py
--rw-rw-rw-   0        0        0     1062 2023-04-24 19:28:30.000000 mt_metadata-0.3.4/tests/tf/processing/fcs/test_fc_channel.py
--rw-rw-rw-   0        0        0    13784 2024-02-27 19:22:13.000000 mt_metadata-0.3.4/tests/tf/test_core_tf.py
--rw-rw-rw-   0        0        0     1150 2023-09-26 18:11:44.000000 mt_metadata-0.3.4/tests/tf/test_get_elevation.py
--rw-rw-rw-   0        0        0    17081 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/tf/test_run.py
--rw-rw-rw-   0        0        0    14129 2024-02-24 00:05:22.000000 mt_metadata-0.3.4/tests/tf/test_station.py
--rw-rw-rw-   0        0        0    11484 2023-09-13 20:55:40.000000 mt_metadata-0.3.4/tests/tf/test_survey.py
--rw-rw-rw-   0        0        0     4315 2023-08-29 22:52:18.000000 mt_metadata-0.3.4/tests/tf/test_tf_merge.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:35.979147 mt_metadata-0.3.4/tests/timeseries/
--rw-rw-rw-   0        0        0       35 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:36.158506 mt_metadata-0.3.4/tests/timeseries/filters/
--rw-rw-rw-   0        0        0       37 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/filters/__init__.py
--rw-rw-rw-   0        0        0    10817 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_channel_response.py
--rw-rw-rw-   0        0        0     3377 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_coefficient_filter.py
--rw-rw-rw-   0        0        0     5409 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_electric_unit.py
--rw-rw-rw-   0        0        0    10649 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_fap_filter.py
--rw-rw-rw-   0        0        0     2602 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_filter_base.py
--rw-rw-rw-   0        0        0     3456 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_filtered.py
--rw-rw-rw-   0        0        0     3961 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_magnetic_unit.py
--rw-rw-rw-   0        0        0     3438 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_time_delay_filter.py
--rw-rw-rw-   0        0        0     4319 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/filters/test_zpk_filter.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:11:36.390235 mt_metadata-0.3.4/tests/timeseries/stationxml/
--rw-rw-rw-   0        0        0       35 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_base_translator.py
--rw-rw-rw-   0        0        0    49588 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_channel.py
--rw-rw-rw-   0        0        0     7053 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_experiment_to_stationxml.py
--rw-rw-rw-   0        0        0     5846 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_fap.py
--rw-rw-rw-   0        0        0     5733 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_fdsn_tools.py
--rw-rw-rw-   0        0        0     3074 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_inventory.py
--rw-rw-rw-   0        0        0     7524 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_network.py
--rw-rw-rw-   0        0        0     2647 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_renaming_filters.py
--rw-rw-rw-   0        0        0     4466 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_run.py
--rw-rw-rw-   0        0        0    21799 2023-08-18 20:49:11.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_station.py
--rw-rw-rw-   0        0        0    11710 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_translations_electric.py
--rw-rw-rw-   0        0        0    13607 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/stationxml/test_translations_magnetic.py
--rw-rw-rw-   0        0        0     3288 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/test_channel.py
--rw-rw-rw-   0        0        0     3894 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/test_electric.py
--rw-rw-rw-   0        0        0     7404 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/test_experiment.py
--rw-rw-rw-   0        0        0     2264 2023-04-14 17:22:28.000000 mt_metadata-0.3.4/tests/timeseries/test_location.py
--rw-rw-rw-   0        0        0     3474 2024-01-22 22:32:29.000000 mt_metadata-0.3.4/tests/timeseries/test_magnetic.py
--rw-rw-rw-   0        0        0     7642 2023-09-13 20:57:37.000000 mt_metadata-0.3.4/tests/timeseries/test_run.py
--rw-rw-rw-   0        0        0     9240 2023-09-13 20:56:44.000000 mt_metadata-0.3.4/tests/timeseries/test_station.py
--rw-rw-rw-   0        0        0    11473 2023-09-13 20:53:46.000000 mt_metadata-0.3.4/tests/timeseries/test_survey.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.870858 mt_metadata-0.3.5/
+-rw-rw-rw-   0        0        0      706 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4330 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1080 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     1315 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    17146 2024-04-12 22:16:47.870858 mt_metadata-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11942 2024-04-12 21:44:56.000000 mt_metadata-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.182477 mt_metadata-0.3.5/docs/
+-rw-rw-rw-   0        0        0      625 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:38.898046 mt_metadata-0.3.5/docs/_build/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:38.898046 mt_metadata-0.3.5/docs/_build/doctrees/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.251480 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    32094 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_10_0.png
+-rw-rw-rw-   0        0        0    23186 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_14_0.png
+-rw-rw-rw-   0        0        0    19789 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_18_0.png
+-rw-rw-rw-   0        0        0    25725 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_23_1.png
+-rw-rw-rw-   0        0        0    57694 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_28_1.png
+-rw-rw-rw-   0        0        0    10774 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_6_0.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:38.913522 mt_metadata-0.3.5/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.367379 mt_metadata-0.3.5/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   541810 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/_build/html/_images/example_mt_file_structure.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.454939 mt_metadata-0.3.5/docs/_build/html/_images/math/
+-rw-rw-rw-   0        0        0      336 2023-09-28 23:30:27.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/000929b09e824936b9447ff8e01006701b495fba.png
+-rw-rw-rw-   0        0        0      359 2023-09-28 23:30:21.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/23f55551d151d663ccc7820ad914a1823ca8ec0f.png
+-rw-rw-rw-   0        0        0      135 2023-09-28 23:30:23.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/25f9afeac2f1f1f07e08db039b0d28955403ecc4.png
+-rw-rw-rw-   0        0        0      293 2023-09-28 23:30:26.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/49562190f3c3e1653c3689177a1258bec888cecc.png
+-rw-rw-rw-   0        0        0      203 2023-09-28 23:30:20.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/53bb25e8239563a86c5137ae758534125005551b.png
+-rw-rw-rw-   0        0        0      340 2023-09-28 23:30:24.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/73aec0fabc50fc9e5d700e44fa7b0238032cedc9.png
+-rw-rw-rw-   0        0        0      378 2023-09-28 23:30:22.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/c5a9382b989cdc1162ca003d6fe23230ff82fd5c.png
+-rw-rw-rw-   0        0        0      298 2023-09-28 23:30:25.000000 mt_metadata-0.3.5/docs/_build/html/_images/math/e2533258291b316cd7c9150be2f6f692e5cafbdd.png
+-rw-rw-rw-   0        0        0  1344293 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/_build/html/_images/reference_frame.png
+-rw-rw-rw-   0        0        0    32094 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_10_0.png
+-rw-rw-rw-   0        0        0    23186 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_14_0.png
+-rw-rw-rw-   0        0        0    19789 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_18_0.png
+-rw-rw-rw-   0        0        0    25725 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_23_1.png
+-rw-rw-rw-   0        0        0    57694 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_28_1.png
+-rw-rw-rw-   0        0        0    10774 2023-09-28 21:37:45.000000 mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_6_0.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.495576 mt_metadata-0.3.5/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-07-26 21:54:07.000000 mt_metadata-0.3.5/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mt_metadata-0.3.5/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/_build/html/_static/mt_metadata_logo.png
+-rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mt_metadata-0.3.5/docs/_build/html/_static/plus.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:39.495576 mt_metadata-0.3.5/docs/_static/
+-rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/_static/mt_metadata_logo.png
+-rw-rw-rw-   0        0        0       29 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/authors.rst
+-rw-rw-rw-   0        0        0     5566 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/contributing.rst
+-rw-rw-rw-   0        0        0      716 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/conventions.rst
+-rw-rw-rw-   0        0        0       29 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/history.rst
+-rw-rw-rw-   0        0        0     2559 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1755 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/make.bat
+-rw-rw-rw-   0        0        0    52229 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/mt_metadata_logo.png
+-rw-rw-rw-   0        0        0     1224 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/readme.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:41.957509 mt_metadata-0.3.5/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:41.988780 mt_metadata-0.3.5/docs/source/images/
+-rw-rw-rw-   0        0        0   541810 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/images/example_mt_file_structure.png
+-rw-rw-rw-   0        0        0  1344293 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/images/reference_frame.png
+-rw-rw-rw-   0        0        0       77 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      736 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.base.rst
+-rw-rw-rw-   0        0        0      265 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.data.rst
+-rw-rw-rw-   0        0        0      219 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.data.stationxml.rst
+-rw-rw-rw-   0        0        0      348 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.rst
+-rw-rw-rw-   0        0        0     3057 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.filters.rst
+-rw-rw-rw-   0        0        0      258 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.filters.standards.rst
+-rw-rw-rw-   0        0        0     5545 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.rst
+-rw-rw-rw-   0        0        0      234 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.standards.rst
+-rw-rw-rw-   0        0        0     2106 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.stationxml.rst
+-rw-rw-rw-   0        0        0      499 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.tools.rst
+-rw-rw-rw-   0        0        0     2101 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.edi.metadata.rst
+-rw-rw-rw-   0        0        0      308 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.edi.metadata.standards.rst
+-rw-rw-rw-   0        0        0      604 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.edi.rst
+-rw-rw-rw-   0        0        0     8784 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.rst
+-rw-rw-rw-   0        0        0      320 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.standards.rst
+-rw-rw-rw-   0        0        0      644 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.emtfxml.rst
+-rw-rw-rw-   0        0        0     1583 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.rst
+-rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.standards.rst
+-rw-rw-rw-   0        0        0      631 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.jfiles.rst
+-rw-rw-rw-   0        0        0      761 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.rst
+-rw-rw-rw-   0        0        0      701 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.rst
+-rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.standards.rst
+-rw-rw-rw-   0        0        0      625 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zfiles.rst
+-rw-rw-rw-   0        0        0     3091 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.rst
+-rw-rw-rw-   0        0        0      314 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.standards.rst
+-rw-rw-rw-   0        0        0      624 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zonge.rst
+-rw-rw-rw-   0        0        0      591 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.rst
+-rw-rw-rw-   0        0        0     1343 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.tf.rst
+-rw-rw-rw-   0        0        0      269 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.tf.standards.rst
+-rw-rw-rw-   0        0        0     1117 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/mt_metadata.utils.rst
+-rw-rw-rw-   0        0        0     6296 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/structure.rst
+-rw-rw-rw-   0        0        0    75115 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_auxiliary.rst
+-rw-rw-rw-   0        0        0     9860 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_battery.rst
+-rw-rw-rw-   0        0        0    75111 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_channel.rst
+-rw-rw-rw-   0        0        0    13746 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_citation.rst
+-rw-rw-rw-   0        0        0     5928 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_comment.rst
+-rw-rw-rw-   0        0        0     2046 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_copyright.rst
+-rw-rw-rw-   0        0        0    47501 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_data_logger.rst
+-rw-rw-rw-   0        0        0    15797 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_data_quality.rst
+-rw-rw-rw-   0        0        0     7895 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_declination.rst
+-rw-rw-rw-   0        0        0     3977 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_diagnostic.rst
+-rw-rw-rw-   0        0        0    21536 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_edi_data_section.rst
+-rw-rw-rw-   0        0        0    17690 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_edi_define_measurement.rst
+-rw-rw-rw-   0        0        0    19563 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_edi_e_measurement.rst
+-rw-rw-rw-   0        0        0    15671 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_edi_h_measurement.rst
+-rw-rw-rw-   0        0        0    79587 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_edi_header.rst
+-rw-rw-rw-   0        0        0      307 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_edi_index.rst
+-rw-rw-rw-   0        0        0       77 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_edi_information.rst
+-rw-rw-rw-   0        0        0   144298 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_electric.rst
+-rw-rw-rw-   0        0        0    27399 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_electrode.rst
+-rw-rw-rw-   0        0        0     3999 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_attachment.rst
+-rw-rw-rw-   0        0        0     3973 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_channels.rst
+-rw-rw-rw-   0        0        0    15713 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_citation.rst
+-rw-rw-rw-   0        0        0     5928 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_comment.rst
+-rw-rw-rw-   0        0        0    27446 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_copyright.rst
+-rw-rw-rw-   0        0        0    11901 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_data_quality_notes.rst
+-rw-rw-rw-   0        0        0     2044 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_data_quality_warnings.rst
+-rw-rw-rw-   0        0        0    17676 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_data_type.rst
+-rw-rw-rw-   0        0        0     2046 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_data_types.rst
+-rw-rw-rw-   0        0        0     9846 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_dipole.rst
+-rw-rw-rw-   0        0        0     9854 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_e_m_t_f.rst
+-rw-rw-rw-   0        0        0    15663 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_electric.rst
+-rw-rw-rw-   0        0        0     5946 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_electrode.rst
+-rw-rw-rw-   0        0        0    11815 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_estimate.rst
+-rw-rw-rw-   0        0        0     3991 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_external_url.rst
+-rw-rw-rw-   0        0        0       75 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_field_notes.rst
+-rw-rw-rw-   0        0        0     1100 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_index.rst
+-rw-rw-rw-   0        0        0    11803 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_instrument.rst
+-rw-rw-rw-   0        0        0    39355 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_location.rst
+-rw-rw-rw-   0        0        0     9822 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_magnetic.rst
+-rw-rw-rw-   0        0        0    11807 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_magnetometer.rst
+-rw-rw-rw-   0        0        0     4025 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_orientation.rst
+-rw-rw-rw-   0        0        0     3975 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_period_range.rst
+-rw-rw-rw-   0        0        0     7877 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_person.rst
+-rw-rw-rw-   0        0        0     2036 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_primary_data.rst
+-rw-rw-rw-   0        0        0    93909 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_processing_info.rst
+-rw-rw-rw-   0        0        0     5956 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_processing_software.rst
+-rw-rw-rw-   0        0        0    19787 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_provenance.rst
+-rw-rw-rw-   0        0        0    75668 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_remote_info.rst
+-rw-rw-rw-   0        0        0     2024 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_remote_ref.rst
+-rw-rw-rw-   0        0        0    27609 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_run.rst
+-rw-rw-rw-   0        0        0    75231 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_site.rst
+-rw-rw-rw-   0        0        0     4019 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_site_layout.rst
+-rw-rw-rw-   0        0        0     5936 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_software.rst
+-rw-rw-rw-   0        0        0     2066 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_statistical_estimates.rst
+-rw-rw-rw-   0        0        0       87 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_emtfxml_transfer_function.rst
+-rw-rw-rw-   0        0        0    11853 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_fdsn.rst
+-rw-rw-rw-   0        0        0    23643 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/tf_filter.rst
+-rw-rw-rw-   0        0        0    13782 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_filter_base.rst
+-rw-rw-rw-   0        0        0     5938 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_filtered.rst
+-rw-rw-rw-   0        0        0      715 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_index.rst
+-rw-rw-rw-   0        0        0     9844 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_instrument.rst
+-rw-rw-rw-   0        0        0     5936 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_jfile_birrp_angles.rst
+-rw-rw-rw-   0        0        0     9846 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_jfile_birrp_block.rst
+-rw-rw-rw-   0        0        0    43075 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_jfile_birrp_parameters.rst
+-rw-rw-rw-   0        0        0    45218 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_jfile_header.rst
+-rw-rw-rw-   0        0        0      265 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_jfile_index.rst
+-rw-rw-rw-   0        0        0    39355 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_location.rst
+-rw-rw-rw-   0        0        0    88902 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_magnetic.rst
+-rw-rw-rw-   0        0        0     7951 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_orientation.rst
+-rw-rw-rw-   0        0        0    11801 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_person.rst
+-rw-rw-rw-   0        0        0    13838 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_band.rst
+-rw-rw-rw-   0        0        0     3983 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_channel.rst
+-rw-rw-rw-   0        0        0     9828 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_channel_nomenclature.rst
+-rw-rw-rw-   0        0        0     7903 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_decimation.rst
+-rw-rw-rw-   0        0        0    53500 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_decimation_level.rst
+-rw-rw-rw-   0        0        0     4011 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_estimator.rst
+-rw-rw-rw-   0        0        0      593 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_index.rst
+-rw-rw-rw-   0        0        0    27803 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_processing.rst
+-rw-rw-rw-   0        0        0     6014 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_regression.rst
+-rw-rw-rw-   0        0        0     9884 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_run.rst
+-rw-rw-rw-   0        0        0     7883 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_station.rst
+-rw-rw-rw-   0        0        0     9888 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_stations.rst
+-rw-rw-rw-   0        0        0     9876 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_aurora_window.rst
+-rw-rw-rw-   0        0        0    11921 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_fcs_channel.rst
+-rw-rw-rw-   0        0        0    37582 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_fcs_decimation.rst
+-rw-rw-rw-   0        0        0    13850 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_fcs_f_c.rst
+-rw-rw-rw-   0        0        0      265 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_processing_fcs_index.rst
+-rw-rw-rw-   0        0        0    49368 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_provenance.rst
+-rw-rw-rw-   0        0        0     5930 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_rating.rst
+-rw-rw-rw-   0        0        0    83521 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_run.rst
+-rw-rw-rw-   0        0        0     7901 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_software.rst
+-rw-rw-rw-   0        0        0   203675 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_station.rst
+-rw-rw-rw-   0        0        0    11867 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_statistical_estimate.rst
+-rw-rw-rw-   0        0        0     4248 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_structure.rst
+-rw-rw-rw-   0        0        0    95093 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_survey.rst
+-rw-rw-rw-   0        0        0     3977 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_time_period.rst
+-rw-rw-rw-   0        0        0     9874 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_timing_system.rst
+-rw-rw-rw-   0        0        0    53534 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_transfer_function.rst
+-rw-rw-rw-   0        0        0     9836 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zmm_channel.rst
+-rw-rw-rw-   0        0        0      180 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zmm_index.rst
+-rw-rw-rw-   0        0        0     2026 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_auto.rst
+-rw-rw-rw-   0        0        0    15697 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_c_h.rst
+-rw-rw-rw-   0        0        0     2014 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_d_plus.rst
+-rw-rw-rw-   0        0        0     7873 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_g_d_p.rst
+-rw-rw-rw-   0        0        0     7875 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_g_p_s.rst
+-rw-rw-rw-   0        0        0    92430 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zonge_header.rst
+-rw-rw-rw-   0        0        0      485 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zonge_index.rst
+-rw-rw-rw-   0        0        0     3961 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zonge_job.rst
+-rw-rw-rw-   0        0        0     3969 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_line.rst
+-rw-rw-rw-   0        0        0     9922 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_m_t_edit.rst
+-rw-rw-rw-   0        0        0     2024 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_m_t_f_t24.rst
+-rw-rw-rw-   0        0        0     3989 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_phase_slope.rst
+-rw-rw-rw-   0        0        0    19607 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_rx.rst
+-rw-rw-rw-   0        0        0     2012 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_s_t_n.rst
+-rw-rw-rw-   0        0        0     9838 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_survey.rst
+-rw-rw-rw-   0        0        0     2010 2023-09-29 00:06:36.000000 mt_metadata-0.3.5/docs/source/tf_zonge_tx.rst
+-rw-rw-rw-   0        0        0     5908 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/tf_zonge_unit.rst
+-rw-rw-rw-   0        0        0    75115 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_auxiliary.rst
+-rw-rw-rw-   0        0        0     9860 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_battery.rst
+-rw-rw-rw-   0        0        0    75111 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_channel.rst
+-rw-rw-rw-   0        0        0    13746 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_citation.rst
+-rw-rw-rw-   0        0        0     2046 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_copyright.rst
+-rw-rw-rw-   0        0        0    47501 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_data_logger.rst
+-rw-rw-rw-   0        0        0    15797 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_data_quality.rst
+-rw-rw-rw-   0        0        0     7895 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_declination.rst
+-rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_diagnostic.rst
+-rw-rw-rw-   0        0        0   144298 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_electric.rst
+-rw-rw-rw-   0        0        0    27399 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_electrode.rst
+-rw-rw-rw-   0        0        0       75 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_experiment.rst
+-rw-rw-rw-   0        0        0    11853 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_fdsn.rst
+-rw-rw-rw-   0        0        0    13782 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_base.rst
+-rw-rw-rw-   0        0        0     2086 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_filter_channel_response_filter.rst
+-rw-rw-rw-   0        0        0    13796 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_coefficient_filter.rst
+-rw-rw-rw-   0        0        0    23653 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_f_i_r_filter.rst
+-rw-rw-rw-   0        0        0    21674 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_frequency_response_table_filter.rst
+-rw-rw-rw-   0        0        0      385 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_filter_index.rst
+-rw-rw-rw-   0        0        0    19679 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_pole_zero_filter.rst
+-rw-rw-rw-   0        0        0    15745 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filter_time_delay_filter.rst
+-rw-rw-rw-   0        0        0     5938 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_filtered.rst
+-rw-rw-rw-   0        0        0    11819 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_funding_source.rst
+-rw-rw-rw-   0        0        0    13784 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_geographic_location.rst
+-rw-rw-rw-   0        0        0      708 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_index.rst
+-rw-rw-rw-   0        0        0     9844 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_instrument.rst
+-rw-rw-rw-   0        0        0    39355 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_location.rst
+-rw-rw-rw-   0        0        0    88902 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_magnetic.rst
+-rw-rw-rw-   0        0        0    16149 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/source/ts_metadata_guide.rst
+-rw-rw-rw-   0        0        0     7951 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_orientation.rst
+-rw-rw-rw-   0        0        0    11801 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_person.rst
+-rw-rw-rw-   0        0        0    49368 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_provenance.rst
+-rw-rw-rw-   0        0        0     5930 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_rating.rst
+-rw-rw-rw-   0        0        0    83521 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_run.rst
+-rw-rw-rw-   0        0        0     7901 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_software.rst
+-rw-rw-rw-   0        0        0   150763 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_station.rst
+-rw-rw-rw-   0        0        0    95093 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_survey.rst
+-rw-rw-rw-   0        0        0     3977 2023-09-29 00:06:35.000000 mt_metadata-0.3.5/docs/source/ts_time_period.rst
+-rw-rw-rw-   0        0        0     9874 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/docs/source/ts_timing_system.rst
+-rw-rw-rw-   0        0        0     1965 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:41.988780 mt_metadata-0.3.5/mt_metadata/
+-rw-rw-rw-   0        0        0     5588 2024-04-12 21:44:56.000000 mt_metadata-0.3.5/mt_metadata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.127980 mt_metadata-0.3.5/mt_metadata/base/
+-rw-rw-rw-   0        0        0      184 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/base/__init__.py
+-rw-rw-rw-   0        0        0    19721 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/base/helpers.py
+-rw-rw-rw-   0        0        0    27145 2024-04-05 20:29:58.000000 mt_metadata-0.3.5/mt_metadata/base/metadata.py
+-rw-rw-rw-   0        0        0    12842 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/base/schema.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.144674 mt_metadata-0.3.5/mt_metadata/data/
+-rw-rw-rw-   0        0        0      217 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.207160 mt_metadata-0.3.5/mt_metadata/data/mt_xml/
+-rw-rw-rw-   0        0        0       26 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/mt_xml/__init__.py
+-rw-rw-rw-   0        0        0    57690 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/mt_xml/multi_run_experiment.xml
+-rw-rw-rw-   0        0        0   236665 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/mt_xml/multi_run_experiment_02.xml
+-rw-rw-rw-   0        0        0    86356 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/mt_xml/single_station_mt_experiment.xml
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.343197 mt_metadata-0.3.5/mt_metadata/data/stationxml/
+-rw-rw-rw-   0        0        0      217 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/__init__.py
+-rw-rw-rw-   0        0        0    12650 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/fdsn_no_mt_info.xml
+-rw-rw-rw-   0        0        0    13230 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_electrode_example.xml
+-rw-rw-rw-   0        0        0     9883 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_magnetometer_example.xml
+-rw-rw-rw-   0        0        0   117239 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_single_station.xml
+-rw-rw-rw-   0        0        0    76110 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/multiple_networks_example.xml
+-rw-rw-rw-   0        0        0   105469 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/station_xml_with_fap_example.xml
+-rw-rw-rw-   0        0        0   492319 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/stationxml/station_xml_with_fir_example.xml
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.775639 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/
+-rw-rw-rw-   0        0        0   102844 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/NMX20.xml
+-rw-rw-rw-   0        0        0    61145 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/PHXTest01.edi
+-rw-rw-rw-   0        0        0       26 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/__init__.py
+-rw-rw-rw-   0        0        0    31883 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/example.xml
+-rw-rw-rw-   0        0        0    32990 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/test.edi
+-rw-rw-rw-   0        0        0    13326 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg.avg
+-rw-rw-rw-   0        0        0    38811 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg_newer.avg
+-rw-rw-rw-   0        0        0    39033 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg_tipper.avg
+-rw-rw-rw-   0        0        0    46663 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_cgg.edi
+-rw-rw-rw-   0        0        0    39022 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_empower.edi
+-rw-rw-rw-   0        0        0    34562 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_metronix.edi
+-rw-rw-rw-   0        0        0    12987 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_no_error.edi
+-rw-rw-rw-   0        0        0    61195 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_phoenix.edi
+-rw-rw-rw-   0        0        0    31042 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_quantec.edi
+-rw-rw-rw-   0        0        0     4895 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_rho_only.edi
+-rw-rw-rw-   0        0        0    25251 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_spectra_in.edi
+-rw-rw-rw-   0        0        0    13446 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_spectra_out.edi
+-rw-rw-rw-   0        0        0    14251 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_jfile.j
+-rw-rw-rw-   0        0        0    30095 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_poor_xml.xml
+-rw-rw-rw-   0        0        0    92001 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml.xml
+-rw-rw-rw-   0        0        0    37102 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_bad_comments.xml
+-rw-rw-rw-   0        0        0    82850 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_complete_remote_info.xml
+-rw-rw-rw-   0        0        0    28104 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_emtf_xml_iris.xml
+-rw-rw-rw-   0        0        0    26903 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_multiple_attachments.xml
+-rw-rw-rw-   0        0        0    28593 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_no_site_layout.xml
+-rw-rw-rw-   0        0        0    96949 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_with_derived_quantities.xml
+-rw-rw-rw-   0        0        0    22671 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_zmm.zmm
+-rw-rw-rw-   0        0        0    16981 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_zss_tipper.zss
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.276994 mt_metadata-0.3.5/mt_metadata/timeseries/
+-rw-rw-rw-   0        0        0     3339 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/__init__.py
+-rw-rw-rw-   0        0        0      827 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/auxiliary.py
+-rw-rw-rw-   0        0        0      965 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/battery.py
+-rw-rw-rw-   0        0        0     3112 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/channel.py
+-rw-rw-rw-   0        0        0      828 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/citation.py
+-rw-rw-rw-   0        0        0      892 2023-09-26 20:16:48.000000 mt_metadata-0.3.5/mt_metadata/timeseries/copyright.py
+-rw-rw-rw-   0        0        0     1542 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/data_logger.py
+-rw-rw-rw-   0        0        0      962 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/data_quality.py
+-rw-rw-rw-   0        0        0      995 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/declination.py
+-rw-rw-rw-   0        0        0      834 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/diagnostic.py
+-rw-rw-rw-   0        0        0     1745 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/electric.py
+-rw-rw-rw-   0        0        0      997 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/electrode.py
+-rw-rw-rw-   0        0        0    21016 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/experiment.py
+-rw-rw-rw-   0        0        0      822 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/fdsn.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.493093 mt_metadata-0.3.5/mt_metadata/timeseries/filters/
+-rw-rw-rw-   0        0        0      474 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/__init__.py
+-rw-rw-rw-   0        0        0    17297 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/channel_response.py
+-rw-rw-rw-   0        0        0     3322 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/coefficient_filter.py
+-rw-rw-rw-   0        0        0    12885 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/filter_base.py
+-rw-rw-rw-   0        0        0     6979 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/filtered.py
+-rw-rw-rw-   0        0        0     6767 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/fir_filter.py
+-rw-rw-rw-   0        0        0     7396 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/frequency_response_table_filter.py
+-rw-rw-rw-   0        0        0     4124 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/helper_functions.py
+-rw-rw-rw-   0        0        0     5916 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/obspy_stages.py
+-rw-rw-rw-   0        0        0     6796 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/plotting_helpers.py
+-rw-rw-rw-   0        0        0     6724 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/pole_zero_filter.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.530845 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/__init__.py
+-rw-rw-rw-   0        0        0      291 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/channel_response.json
+-rw-rw-rw-   0        0        0      297 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/coefficient_filter.json
+-rw-rw-rw-   0        0        0     2663 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/filter_base.json
+-rw-rw-rw-   0        0        0     1582 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/fir_filter.json
+-rw-rw-rw-   0        0        0     1506 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/frequency_response_table_filter.json
+-rw-rw-rw-   0        0        0      994 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/pole_zero_filter.json
+-rw-rw-rw-   0        0        0      327 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/time_delay_filter.json
+-rw-rw-rw-   0        0        0     3257 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/filters/time_delay_filter.py
+-rw-rw-rw-   0        0        0      841 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/funding_source.py
+-rw-rw-rw-   0        0        0      851 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/geographic_location.py
+-rw-rw-rw-   0        0        0      834 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/instrument.py
+-rw-rw-rw-   0        0        0     7437 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/location.py
+-rw-rw-rw-   0        0        0     1746 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/magnetic.py
+-rw-rw-rw-   0        0        0      836 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/orientation.py
+-rw-rw-rw-   0        0        0      971 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/person.py
+-rw-rw-rw-   0        0        0     1605 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/provenance.py
+-rw-rw-rw-   0        0        0      826 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/rating.py
+-rw-rw-rw-   0        0        0    14009 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/run.py
+-rw-rw-rw-   0        0        0     1224 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/software.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.631089 mt_metadata-0.3.5/mt_metadata/timeseries/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/__init__.py
+-rw-rw-rw-   0        0        0     4746 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/auxiliary.json
+-rw-rw-rw-   0        0        0     1408 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/battery.json
+-rw-rw-rw-   0        0        0     5144 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/channel.json
+-rw-rw-rw-   0        0        0     2030 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/citation.json
+-rw-rw-rw-   0        0        0    12478 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/copyright.json
+-rw-rw-rw-   0        0        0     1506 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/data_quality.json
+-rw-rw-rw-   0        0        0     1402 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/declination.json
+-rw-rw-rw-   0        0        0      585 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/diagnostic.json
+-rw-rw-rw-   0        0        0     2493 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/electric.json
+-rw-rw-rw-   0        0        0     1949 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/fdsn.json
+-rw-rw-rw-   0        0        0     1159 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/filtered.json
+-rw-rw-rw-   0        0        0     1756 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/funding_source.json
+-rw-rw-rw-   0        0        0     2223 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/geographic_location.json
+-rw-rw-rw-   0        0        0     1533 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/instrument.json
+-rw-rw-rw-   0        0        0     5294 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/location.json
+-rw-rw-rw-   0        0        0     1291 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/magnetic.json
+-rw-rw-rw-   0        0        0     1866 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/orientation.json
+-rw-rw-rw-   0        0        0     1772 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/person.json
+-rw-rw-rw-   0        0        0      981 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/provenance.json
+-rw-rw-rw-   0        0        0     1029 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/rating.json
+-rw-rw-rw-   0        0        0     2500 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/run.json
+-rw-rw-rw-   0        0        0     1199 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/software.json
+-rw-rw-rw-   0        0        0     2990 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/station.json
+-rw-rw-rw-   0        0        0     3426 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/survey.json
+-rw-rw-rw-   0        0        0      681 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/time_period.json
+-rw-rw-rw-   0        0        0     1492 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/standards/timing_system.json
+-rw-rw-rw-   0        0        0     9855 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/station.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.777898 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/
+-rw-rw-rw-   0        0        0      525 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/__init__.py
+-rw-rw-rw-   0        0        0     9487 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/fdsn_tools.py
+-rw-rw-rw-   0        0        0     7257 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/utils.py
+-rw-rw-rw-   0        0        0    20289 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_channel_mt_channel.py
+-rw-rw-rw-   0        0        0     5151 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_equipment_mt_run.py
+-rw-rw-rw-   0        0        0    14036 2024-03-14 05:07:03.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_inventory_mt_experiment.py
+-rw-rw-rw-   0        0        0     7124 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_network_mt_survey.py
+-rw-rw-rw-   0        0        0    11112 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_station_mt_station.py
+-rw-rw-rw-   0        0        0    11831 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/timeseries/survey.py
+-rw-rw-rw-   0        0        0     1653 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/time_period.py
+-rw-rw-rw-   0        0        0      839 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/timing_system.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.809141 mt_metadata-0.3.5/mt_metadata/timeseries/tools/
+-rw-rw-rw-   0        0        0       78 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/timeseries/tools/__init__.py
+-rw-rw-rw-   0        0        0    14405 2024-03-01 22:13:10.000000 mt_metadata-0.3.5/mt_metadata/timeseries/tools/from_many_mt_files.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.846896 mt_metadata-0.3.5/mt_metadata/transfer_functions/
+-rw-rw-rw-   0        0        0       42 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/__init__.py
+-rw-rw-rw-   0        0        0    79933 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/core.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.893762 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/
+-rw-rw-rw-   0        0        0      215 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:43.931513 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/
+-rw-rw-rw-   0        0        0       61 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/__init__.py
+-rw-rw-rw-   0        0        0    53305 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/edi.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.047387 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/
+-rw-rw-rw-   0        0        0      395 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/__init__.py
+-rw-rw-rw-   0        0        0     7751 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/data_section.py
+-rw-rw-rw-   0        0        0    16264 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/define_measurement.py
+-rw-rw-rw-   0        0        0     3138 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/emeasurement.py
+-rw-rw-rw-   0        0        0     9203 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/header.py
+-rw-rw-rw-   0        0        0     2245 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/hmeasurement.py
+-rw-rw-rw-   0        0        0    17062 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/information.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.063011 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/__init__.py
+-rw-rw-rw-   0        0        0     3045 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/data_section.json
+-rw-rw-rw-   0        0        0     2572 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/define_measurement.json
+-rw-rw-rw-   0        0        0     3100 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/emeasurement.json
+-rw-rw-rw-   0        0        0     6444 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/header.json
+-rw-rw-rw-   0        0        0     2450 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/hmeasurement.json
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.109872 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/
+-rw-rw-rw-   0        0        0       73 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/__init__.py
+-rw-rw-rw-   0        0        0    53432 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/emtfxml.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.763619 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/
+-rw-rw-rw-   0        0        0     2364 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2459 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/attachment.py
+-rw-rw-rw-   0        0        0      889 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/channels.py
+-rw-rw-rw-   0        0        0     1500 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/citation.py
+-rw-rw-rw-   0        0        0     2409 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/comment.py
+-rw-rw-rw-   0        0        0     1802 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/copyright.py
+-rw-rw-rw-   0        0        0    14720 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data.py
+-rw-rw-rw-   0        0        0     2325 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_notes.py
+-rw-rw-rw-   0        0        0     1769 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_warnings.py
+-rw-rw-rw-   0        0        0     1919 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_type.py
+-rw-rw-rw-   0        0        0     2349 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_types.py
+-rw-rw-rw-   0        0        0     2414 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/dipole.py
+-rw-rw-rw-   0        0        0     1952 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/electric.py
+-rw-rw-rw-   0        0        0     1398 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/electrode.py
+-rw-rw-rw-   0        0        0      773 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/emtf.py
+-rw-rw-rw-   0        0        0     2038 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/estimate.py
+-rw-rw-rw-   0        0        0     1172 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/external_url.py
+-rw-rw-rw-   0        0        0     1766 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/field_notes.py
+-rw-rw-rw-   0        0        0     4494 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/helpers.py
+-rw-rw-rw-   0        0        0     1406 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/instrument.py
+-rw-rw-rw-   0        0        0     9283 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/location.py
+-rw-rw-rw-   0        0        0     1807 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetic.py
+-rw-rw-rw-   0        0        0     1343 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetometer.py
+-rw-rw-rw-   0        0        0     2493 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/orientation.py
+-rw-rw-rw-   0        0        0     1633 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/period_range.py
+-rw-rw-rw-   0        0        0      830 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/person.py
+-rw-rw-rw-   0        0        0     1018 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/primary_data.py
+-rw-rw-rw-   0        0        0     3208 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/processing_info.py
+-rw-rw-rw-   0        0        0     2425 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/provenance.py
+-rw-rw-rw-   0        0        0     2291 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_info.py
+-rw-rw-rw-   0        0        0     1724 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_ref.py
+-rw-rw-rw-   0        0        0     4848 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/run.py
+-rw-rw-rw-   0        0        0     4046 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/site.py
+-rw-rw-rw-   0        0        0     6092 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/site_layout.py
+-rw-rw-rw-   0        0        0     1942 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/software.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.879897 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/attachment.json
+-rw-rw-rw-   0        0        0      565 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/channels.json
+-rw-rw-rw-   0        0        0     2269 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/citation.json
+-rw-rw-rw-   0        0        0      880 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/comment.json
+-rw-rw-rw-   0        0        0     2477 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/copyright.json
+-rw-rw-rw-   0        0        0      942 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_notes.json
+-rw-rw-rw-   0        0        0      273 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_warnings.json
+-rw-rw-rw-   0        0        0     2995 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_type.json
+-rw-rw-rw-   0        0        0      284 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_types.json
+-rw-rw-rw-   0        0        0      374 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/description.json
+-rw-rw-rw-   0        0        0     1419 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/dipole.json
+-rw-rw-rw-   0        0        0     2436 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electric.json
+-rw-rw-rw-   0        0        0      958 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electrode.json
+-rw-rw-rw-   0        0        0     1675 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/emtf.json
+-rw-rw-rw-   0        0        0     2069 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/estimate.json
+-rw-rw-rw-   0        0        0      638 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/external_url.json
+-rw-rw-rw-   0        0        0     5294 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/location.json
+-rw-rw-rw-   0        0        0     1483 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetic.json
+-rw-rw-rw-   0        0        0     1814 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetometer.json
+-rw-rw-rw-   0        0        0      675 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/orientation.json
+-rw-rw-rw-   0        0        0      563 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/period_range.json
+-rw-rw-rw-   0        0        0     1198 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/person.json
+-rw-rw-rw-   0        0        0      319 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/primary_data.json
+-rw-rw-rw-   0        0        0     1340 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/processing_info.json
+-rw-rw-rw-   0        0        0      707 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/provenance.json
+-rw-rw-rw-   0        0        0      317 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/remote_ref.json
+-rw-rw-rw-   0        0        0     1486 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/run.json
+-rw-rw-rw-   0        0        0     3240 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site.json
+-rw-rw-rw-   0        0        0      696 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site_layout.json
+-rw-rw-rw-   0        0        0      892 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/software.json
+-rw-rw-rw-   0        0        0      298 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/statistical_estimates.json
+-rw-rw-rw-   0        0        0     1097 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/value.json
+-rw-rw-rw-   0        0        0     2429 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/statistical_estimates.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:44.911141 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/
+-rw-rw-rw-   0        0        0       67 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/__init__.py
+-rw-rw-rw-   0        0        0    13676 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/jfile.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.011387 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/
+-rw-rw-rw-   0        0        0      265 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_angles.py
+-rw-rw-rw-   0        0        0      833 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_block.py
+-rw-rw-rw-   0        0        0      843 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_parameters.py
+-rw-rw-rw-   0        0        0     5207 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/header.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.027007 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_angles.json
+-rw-rw-rw-   0        0        0     1381 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_block.json
+-rw-rw-rw-   0        0        0     6105 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_parameters.json
+-rw-rw-rw-   0        0        0      846 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/header.json
+-rw-rw-rw-   0        0        0     6024 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.064767 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/
+-rw-rw-rw-   0        0        0       61 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.096011 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/
+-rw-rw-rw-   0        0        0       73 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/channel.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.111631 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/standards/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/standards/channel.json
+-rw-rw-rw-   0        0        0    35850 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/zmm.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.149389 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/
+-rw-rw-rw-   0        0        0       77 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.412111 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/
+-rw-rw-rw-   0        0        0      646 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/auto.py
+-rw-rw-rw-   0        0        0      795 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/ch.py
+-rw-rw-rw-   0        0        0      804 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/d_plus.py
+-rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/gdp.py
+-rw-rw-rw-   0        0        0     1222 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/gps.py
+-rw-rw-rw-   0        0        0     7700 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/header.py
+-rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/job.py
+-rw-rw-rw-   0        0        0      799 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/line.py
+-rw-rw-rw-   0        0        0     1173 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/mt_edit.py
+-rw-rw-rw-   0        0        0      803 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/mtft24.py
+-rw-rw-rw-   0        0        0      814 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/phase_slope.py
+-rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/rx.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.465494 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/__init__.py
+-rw-rw-rw-   0        0        0      330 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/auto.json
+-rw-rw-rw-   0        0        0     2387 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/ch.json
+-rw-rw-rw-   0        0        0      308 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/d_plus.json
+-rw-rw-rw-   0        0        0     1145 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/gdp.json
+-rw-rw-rw-   0        0        0     1113 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/gps.json
+-rw-rw-rw-   0        0        0      267 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/header.json
+-rw-rw-rw-   0        0        0      559 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/job.json
+-rw-rw-rw-   0        0        0      548 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/line.json
+-rw-rw-rw-   0        0        0      304 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/mt_edit.json
+-rw-rw-rw-   0        0        0      304 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/mtft24.json
+-rw-rw-rw-   0        0        0      681 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/phase_slope.json
+-rw-rw-rw-   0        0        0     2961 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/rx.json
+-rw-rw-rw-   0        0        0      276 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/stn.json
+-rw-rw-rw-   0        0        0     1529 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/survey.json
+-rw-rw-rw-   0        0        0      323 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/tx.json
+-rw-rw-rw-   0        0        0      953 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/unit.json
+-rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/stn.py
+-rw-rw-rw-   0        0        0      772 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/survey.py
+-rw-rw-rw-   0        0        0      797 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/tx.py
+-rw-rw-rw-   0        0        0      801 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/unit.py
+-rw-rw-rw-   0        0        0    17203 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/zonge.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.465494 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/
+-rw-rw-rw-   0        0        0        2 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.697224 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/
+-rw-rw-rw-   0        0        0      668 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/__init__.py
+-rw-rw-rw-   0        0        0     8509 2024-04-05 20:29:58.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/band.py
+-rw-rw-rw-   0        0        0      773 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/channel.py
+-rw-rw-rw-   0        0        0     4264 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/channel_nomenclature.py
+-rw-rw-rw-   0        0        0      785 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/decimation.py
+-rw-rw-rw-   0        0        0    10657 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/decimation_level.py
+-rw-rw-rw-   0        0        0      781 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/estimator.py
+-rw-rw-rw-   0        0        0    10320 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/processing.py
+-rw-rw-rw-   0        0        0      783 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/regression.py
+-rw-rw-rw-   0        0        0     4123 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/run.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.750615 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/
+-rw-rw-rw-   0        0        0      135 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/__init__.py
+-rw-rw-rw-   0        0        0     2105 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/band.json
+-rw-rw-rw-   0        0        0      548 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/channel.json
+-rw-rw-rw-   0        0        0     1798 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclature.json
+-rw-rw-rw-   0        0        0      378 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclatures.json
+-rw-rw-rw-   0        0        0     1007 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/config.json
+-rw-rw-rw-   0        0        0     1168 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/decimation.json
+-rw-rw-rw-   0        0        0     4176 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/decimation_level.json
+-rw-rw-rw-   0        0        0      628 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/estimator.json
+-rw-rw-rw-   0        0        0     1211 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/processing.json
+-rw-rw-rw-   0        0        0      901 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/regression.json
+-rw-rw-rw-   0        0        0     1423 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/run.json
+-rw-rw-rw-   0        0        0     1173 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/station.json
+-rw-rw-rw-   0        0        0      276 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/stations.json
+-rw-rw-rw-   0        0        0     1892 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/window.json
+-rw-rw-rw-   0        0        0     5163 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/station.py
+-rw-rw-rw-   0        0        0     4564 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/stations.py
+-rw-rw-rw-   0        0        0     1210 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/window.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.836470 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/
+-rw-rw-rw-   0        0        0      134 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/__init__.py
+-rw-rw-rw-   0        0        0    15679 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/decimation.py
+-rw-rw-rw-   0        0        0    10450 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/fc.py
+-rw-rw-rw-   0        0        0      926 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/fc_channel.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.843524 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/
+-rw-rw-rw-   0        0        0      135 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/__init__.py
+-rw-rw-rw-   0        0        0     3772 2024-03-01 22:12:06.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/decimation.json
+-rw-rw-rw-   0        0        0     1523 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc.json
+-rw-rw-rw-   0        0        0     1873 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc_channel.json
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.951273 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/
+-rw-rw-rw-   0        0        0     3890 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/comment.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:45.982515 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/
+-rw-rw-rw-   0        0        0      135 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/__init__.py
+-rw-rw-rw-   0        0        0      880 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/comment.json
+-rw-rw-rw-   0        0        0     2972 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/station.json
+-rw-rw-rw-   0        0        0     1917 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/statistical_estimate.json
+-rw-rw-rw-   0        0        0     3426 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/survey.json
+-rw-rw-rw-   0        0        0     3220 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/transfer_function.json
+-rw-rw-rw-   0        0        0     9840 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/station.py
+-rw-rw-rw-   0        0        0      857 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/statistical_estimate.py
+-rw-rw-rw-   0        0        0    12547 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/survey.py
+-rw-rw-rw-   0        0        0     5094 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/transfer_function.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.098383 mt_metadata-0.3.5/mt_metadata/utils/
+-rw-rw-rw-   0        0        0       35 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/utils/__init__.py
+-rw-rw-rw-   0        0        0      462 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/mt_metadata/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7668 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/utils/list_dict.py
+-rw-rw-rw-   0        0        0    18719 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/utils/mttime.py
+-rw-rw-rw-   0        0        0     4109 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/utils/summarize.py
+-rw-rw-rw-   0        0        0     6405 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/utils/units.py
+-rw-rw-rw-   0        0        0    16264 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/mt_metadata/utils/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:42.042158 mt_metadata-0.3.5/mt_metadata.egg-info/
+-rw-rw-rw-   0        0        0    17146 2024-04-12 22:16:36.000000 mt_metadata-0.3.5/mt_metadata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    32618 2024-04-12 22:16:38.000000 mt_metadata-0.3.5/mt_metadata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 22:16:36.000000 mt_metadata-0.3.5/mt_metadata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 22:16:36.000000 mt_metadata-0.3.5/mt_metadata.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2024-04-12 22:16:36.000000 mt_metadata-0.3.5/mt_metadata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-12 22:16:36.000000 mt_metadata-0.3.5/mt_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      462 2024-04-12 22:16:47.870858 mt_metadata-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2024-04-12 21:44:56.000000 mt_metadata-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.267631 mt_metadata-0.3.5/tests/
+-rw-rw-rw-   0        0        0      449 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/__init__.py
+-rw-rw-rw-   0        0        0    17262 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     8706 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/test_list_dict.py
+-rw-rw-rw-   0        0        0     4330 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/test_metadata.py
+-rw-rw-rw-   0        0        0    11801 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/test_mttime.py
+-rw-rw-rw-   0        0        0     6200 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/test_schema.py
+-rw-rw-rw-   0        0        0     1571 2024-03-14 05:21:54.000000 mt_metadata-0.3.5/tests/test_standards_exist.py
+-rw-rw-rw-   0        0        0     2775 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/test_summarize.py
+-rw-rw-rw-   0        0        0     1488 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/test_units.py
+-rw-rw-rw-   0        0        0     9201 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/test_validators.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.391842 mt_metadata-0.3.5/tests/tf/
+-rw-rw-rw-   0        0        0       35 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.407463 mt_metadata-0.3.5/tests/tf/io/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.583711 mt_metadata-0.3.5/tests/tf/io/edi/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/edi/__init__.py
+-rw-rw-rw-   0        0        0    19367 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_cgg_edi.py
+-rw-rw-rw-   0        0        0     7160 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_edi.py
+-rw-rw-rw-   0        0        0     9801 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_edi_spectra.py
+-rw-rw-rw-   0        0        0    21308 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_empower_edi.py
+-rw-rw-rw-   0        0        0     9148 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_metronix_edi.py
+-rw-rw-rw-   0        0        0    10010 2024-04-12 21:44:56.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_no_error_edi.py
+-rw-rw-rw-   0        0        0    12082 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_phoenix_edi.py
+-rw-rw-rw-   0        0        0     9335 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_quantec_edi.py
+-rw-rw-rw-   0        0        0    13186 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/edi/test_rho_only_edi.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.799827 mt_metadata-0.3.5/tests/tf/io/emtfxml/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/__init__.py
+-rw-rw-rw-   0        0        0    29088 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_emtfxml.py
+-rw-rw-rw-   0        0        0    18967 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_emtfxml_poor.py
+-rw-rw-rw-   0        0        0     1702 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_multiple_attachments.py
+-rw-rw-rw-   0        0        0    27587 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read.py
+-rw-rw-rw-   0        0        0    22989 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_complete_remote_info.py
+-rw-rw-rw-   0        0        0    12554 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_derived_quantities.py
+-rw-rw-rw-   0        0        0    12640 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_no_site_layout.py
+-rw-rw-rw-   0        0        0    14282 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_poor.py
+-rw-rw-rw-   0        0        0     8703 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write.py
+-rw-rw-rw-   0        0        0     8766 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write_complete_remote_info.py
+-rw-rw-rw-   0        0        0     7886 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write_poor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.837582 mt_metadata-0.3.5/tests/tf/io/jfile/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/jfile/__init__.py
+-rw-rw-rw-   0        0        0     3537 2023-04-14 17:22:27.000000 mt_metadata-0.3.5/tests/tf/io/jfile/test_jfile.py
+-rw-rw-rw-   0        0        0     8602 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/jfile/test_tf_read.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:46.925222 mt_metadata-0.3.5/tests/tf/io/zmm/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/tf/io/zmm/__init__.py
+-rw-rw-rw-   0        0        0    18065 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zmm/test_tf_read_zmm.py
+-rw-rw-rw-   0        0        0    10338 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zmm/test_tf_read_zss.py
+-rw-rw-rw-   0        0        0     8837 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zmm/test_zmm.py
+-rw-rw-rw-   0        0        0     6612 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zmm/test_zss.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.053602 mt_metadata-0.3.5/tests/tf/io/zonge/
+-rw-rw-rw-   0        0        0       16 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/tf/io/zonge/__init__.py
+-rw-rw-rw-   0        0        0     8602 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read.py
+-rw-rw-rw-   0        0        0     8646 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read_newer.py
+-rw-rw-rw-   0        0        0    16798 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read_tipper.py
+-rw-rw-rw-   0        0        0     4078 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge.py
+-rw-rw-rw-   0        0        0     3560 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge_newer.py
+-rw-rw-rw-   0        0        0    16644 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge_tipper.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:38.946780 mt_metadata-0.3.5/tests/tf/processing/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.238473 mt_metadata-0.3.5/tests/tf/processing/aurora/
+-rw-rw-rw-   0        0        0        0 2023-04-24 19:28:30.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/__init__.py
+-rw-rw-rw-   0        0        0     8468 2024-04-05 20:29:58.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_band.py
+-rw-rw-rw-   0        0        0     1671 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_channel_nomenclature.py
+-rw-rw-rw-   0        0        0     2489 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_dataset_dataframe.py
+-rw-rw-rw-   0        0        0      707 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_decimation.py
+-rw-rw-rw-   0        0        0      700 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_estimator.py
+-rw-rw-rw-   0        0        0     1642 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_frequency_bands.py
+-rw-rw-rw-   0        0        0     4385 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_processing.py
+-rw-rw-rw-   0        0        0      707 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_regression.py
+-rw-rw-rw-   0        0        0      714 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_station.py
+-rw-rw-rw-   0        0        0     2558 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_stations.py
+-rw-rw-rw-   0        0        0     1205 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/aurora/test_window.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.300964 mt_metadata-0.3.5/tests/tf/processing/fcs/
+-rw-rw-rw-   0        0        0        0 2023-04-24 19:28:30.000000 mt_metadata-0.3.5/tests/tf/processing/fcs/__init__.py
+-rw-rw-rw-   0        0        0     7632 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/fcs/test_decimation.py
+-rw-rw-rw-   0        0        0     4134 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/fcs/test_fc.py
+-rw-rw-rw-   0        0        0     1062 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/processing/fcs/test_fc_channel.py
+-rw-rw-rw-   0        0        0    13784 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_core_tf.py
+-rw-rw-rw-   0        0        0     1150 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_get_elevation.py
+-rw-rw-rw-   0        0        0    17081 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_run.py
+-rw-rw-rw-   0        0        0    14129 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_station.py
+-rw-rw-rw-   0        0        0    11484 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_survey.py
+-rw-rw-rw-   0        0        0     4315 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/tf/test_tf_merge.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.454480 mt_metadata-0.3.5/tests/timeseries/
+-rw-rw-rw-   0        0        0       35 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.622489 mt_metadata-0.3.5/tests/timeseries/filters/
+-rw-rw-rw-   0        0        0       37 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/filters/__init__.py
+-rw-rw-rw-   0        0        0    10817 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_channel_response.py
+-rw-rw-rw-   0        0        0     3377 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_coefficient_filter.py
+-rw-rw-rw-   0        0        0     5409 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_electric_unit.py
+-rw-rw-rw-   0        0        0    10649 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_fap_filter.py
+-rw-rw-rw-   0        0        0     2602 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_filter_base.py
+-rw-rw-rw-   0        0        0     3456 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_filtered.py
+-rw-rw-rw-   0        0        0     3961 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_magnetic_unit.py
+-rw-rw-rw-   0        0        0     3438 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_time_delay_filter.py
+-rw-rw-rw-   0        0        0     4319 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/filters/test_zpk_filter.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:16:47.855238 mt_metadata-0.3.5/tests/timeseries/stationxml/
+-rw-rw-rw-   0        0        0       35 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_base_translator.py
+-rw-rw-rw-   0        0        0    49588 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_channel.py
+-rw-rw-rw-   0        0        0     7424 2024-03-14 05:17:20.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_experiment_to_stationxml.py
+-rw-rw-rw-   0        0        0     5846 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_fap.py
+-rw-rw-rw-   0        0        0     5733 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_fdsn_tools.py
+-rw-rw-rw-   0        0        0     3074 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_inventory.py
+-rw-rw-rw-   0        0        0     7524 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_network.py
+-rw-rw-rw-   0        0        0     2647 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_renaming_filters.py
+-rw-rw-rw-   0        0        0     4466 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_run.py
+-rw-rw-rw-   0        0        0    21799 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_station.py
+-rw-rw-rw-   0        0        0    11710 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_translations_electric.py
+-rw-rw-rw-   0        0        0    13607 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/stationxml/test_translations_magnetic.py
+-rw-rw-rw-   0        0        0     3288 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_channel.py
+-rw-rw-rw-   0        0        0     3894 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_electric.py
+-rw-rw-rw-   0        0        0     7395 2024-03-14 05:11:32.000000 mt_metadata-0.3.5/tests/timeseries/test_experiment.py
+-rw-rw-rw-   0        0        0     2264 2023-04-14 17:22:28.000000 mt_metadata-0.3.5/tests/timeseries/test_location.py
+-rw-rw-rw-   0        0        0     3474 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_magnetic.py
+-rw-rw-rw-   0        0        0     7642 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_run.py
+-rw-rw-rw-   0        0        0     9240 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_station.py
+-rw-rw-rw-   0        0        0    11473 2024-02-29 19:37:31.000000 mt_metadata-0.3.5/tests/timeseries/test_survey.py
```

### Comparing `mt_metadata-0.3.4/AUTHORS.rst` & `mt_metadata-0.3.5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/CONTRIBUTING.rst` & `mt_metadata-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/HISTORY.rst` & `mt_metadata-0.3.5/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/LICENSE` & `mt_metadata-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/MANIFEST.in` & `mt_metadata-0.3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/PKG-INFO` & `mt_metadata-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mt_metadata
-Version: 0.3.4
+Version: 0.3.5
 Summary: Metadata for magnetotelluric data
 Home-page: https://github.com/kujaku11/mt_metadata
 Author: Jared Peacock
 Author-email: jpeacock@usgs.gov
 License: MIT license
 Keywords: mt_metadata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# mt_metadata version 0.3.4
+# mt_metadata version 0.3.5
  Standard MT metadata
 
 [![PyPi version](https://img.shields.io/pypi/v/mt_metadata.svg)](https://pypi.python.org/pypi/mt-metadata)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mt-metadata.svg)](https://anaconda.org/conda-forge/mt-metadata)
 [![codecov](https://codecov.io/gh/kujaku11/mt_metadata/branch/main/graph/badge.svg?token=1WYF0G1L3D)](https://codecov.io/gh/kujaku11/mt_metadata)
 ![example workflow name](https://github.com/kujaku11/mt_metadata/workflows/TestingInConda/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -48,15 +48,15 @@
         - **ZMM** (Egberts EMTF output)
         - **JFILE** (BIRRP output)
         - **EMTFXML** (Kelbert's format)
         - **AVG** (Zonge output)
 
 Most people will be using the transfer functions, but a lot of that metadata comes from the time series metadata.  This module supports both and has tried to make them more or less seamless to reduce complication.
 
-* **Version**: 0.3.4
+* **Version**: 0.3.5
 * **Free software**: MIT license
 * **Documentation**: https://mt-metadata.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **mt_metadata/examples/notebooks** and **docs/source/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 # Installation
```

### Comparing `mt_metadata-0.3.4/README.md` & `mt_metadata-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mt_metadata version 0.3.4
+# mt_metadata version 0.3.5
  Standard MT metadata
 
 [![PyPi version](https://img.shields.io/pypi/v/mt_metadata.svg)](https://pypi.python.org/pypi/mt-metadata)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mt-metadata.svg)](https://anaconda.org/conda-forge/mt-metadata)
 [![codecov](https://codecov.io/gh/kujaku11/mt_metadata/branch/main/graph/badge.svg?token=1WYF0G1L3D)](https://codecov.io/gh/kujaku11/mt_metadata)
 ![example workflow name](https://github.com/kujaku11/mt_metadata/workflows/TestingInConda/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -24,15 +24,15 @@
         - **ZMM** (Egberts EMTF output)
         - **JFILE** (BIRRP output)
         - **EMTFXML** (Kelbert's format)
         - **AVG** (Zonge output)
 
 Most people will be using the transfer functions, but a lot of that metadata comes from the time series metadata.  This module supports both and has tried to make them more or less seamless to reduce complication.
 
-* **Version**: 0.3.4
+* **Version**: 0.3.5
 * **Free software**: MIT license
 * **Documentation**: https://mt-metadata.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **mt_metadata/examples/notebooks** and **docs/source/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 # Installation
```

### Comparing `mt_metadata-0.3.4/docs/Makefile` & `mt_metadata-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_10_0.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_10_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_14_0.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_18_0.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_18_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_23_1.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_23_1.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_28_1.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_28_1.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_6_0.png` & `mt_metadata-0.3.5/docs/_build/doctrees/nbsphinx/source_notebooks_filters_example_6_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/example_mt_file_structure.png` & `mt_metadata-0.3.5/docs/_build/html/_images/example_mt_file_structure.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/reference_frame.png` & `mt_metadata-0.3.5/docs/_build/html/_images/reference_frame.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_10_0.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_10_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_14_0.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_18_0.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_18_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_23_1.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_23_1.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_28_1.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_28_1.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_images/source_notebooks_filters_example_6_0.png` & `mt_metadata-0.3.5/docs/_build/html/_images/source_notebooks_filters_example_6_0.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_build/html/_static/mt_metadata_logo.png` & `mt_metadata-0.3.5/docs/_build/html/_static/mt_metadata_logo.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/_static/mt_metadata_logo.png` & `mt_metadata-0.3.5/docs/_static/mt_metadata_logo.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/conf.py` & `mt_metadata-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/conventions.rst` & `mt_metadata-0.3.5/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/index.rst` & `mt_metadata-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/installation.rst` & `mt_metadata-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/make.bat` & `mt_metadata-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/mt_metadata_logo.png` & `mt_metadata-0.3.5/docs/mt_metadata_logo.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/readme.rst` & `mt_metadata-0.3.5/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/images/example_mt_file_structure.png` & `mt_metadata-0.3.5/docs/source/images/example_mt_file_structure.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/images/reference_frame.png` & `mt_metadata-0.3.5/docs/source/images/reference_frame.png`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.base.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.base.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.filters.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.filters.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.timeseries.stationxml.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.timeseries.stationxml.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.edi.metadata.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.edi.metadata.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.edi.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.edi.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.emtfxml.metadata.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.emtfxml.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.emtfxml.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.jfiles.metadata.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.jfiles.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.jfiles.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zfiles.metadata.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zfiles.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zfiles.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zonge.metadata.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.io.zonge.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.io.zonge.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.transfer_functions.tf.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.transfer_functions.tf.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/mt_metadata.utils.rst` & `mt_metadata-0.3.5/docs/source/mt_metadata.utils.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/structure.rst` & `mt_metadata-0.3.5/docs/source/structure.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_auxiliary.rst` & `mt_metadata-0.3.5/docs/source/tf_auxiliary.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_battery.rst` & `mt_metadata-0.3.5/docs/source/tf_battery.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_channel.rst` & `mt_metadata-0.3.5/docs/source/tf_channel.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_citation.rst` & `mt_metadata-0.3.5/docs/source/tf_citation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_comment.rst` & `mt_metadata-0.3.5/docs/source/tf_comment.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_copyright.rst` & `mt_metadata-0.3.5/docs/source/tf_copyright.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_data_logger.rst` & `mt_metadata-0.3.5/docs/source/tf_data_logger.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_data_quality.rst` & `mt_metadata-0.3.5/docs/source/tf_data_quality.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_declination.rst` & `mt_metadata-0.3.5/docs/source/tf_declination.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_diagnostic.rst` & `mt_metadata-0.3.5/docs/source/tf_diagnostic.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_edi_data_section.rst` & `mt_metadata-0.3.5/docs/source/tf_edi_data_section.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_edi_define_measurement.rst` & `mt_metadata-0.3.5/docs/source/tf_edi_define_measurement.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_edi_e_measurement.rst` & `mt_metadata-0.3.5/docs/source/tf_edi_e_measurement.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_edi_h_measurement.rst` & `mt_metadata-0.3.5/docs/source/tf_edi_h_measurement.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_edi_header.rst` & `mt_metadata-0.3.5/docs/source/tf_edi_header.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_electric.rst` & `mt_metadata-0.3.5/docs/source/tf_electric.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_electrode.rst` & `mt_metadata-0.3.5/docs/source/tf_electrode.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_attachment.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_attachment.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_channels.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_channels.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_citation.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_citation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_comment.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_comment.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_copyright.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_copyright.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_data_quality_notes.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_data_quality_notes.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_data_quality_warnings.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_data_quality_warnings.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_data_type.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_data_type.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_data_types.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_data_types.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_dipole.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_dipole.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_e_m_t_f.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_e_m_t_f.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_electric.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_electric.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_electrode.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_electrode.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_estimate.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_estimate.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_external_url.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_external_url.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_index.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_index.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_instrument.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_instrument.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_location.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_location.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_magnetic.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_magnetic.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_magnetometer.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_magnetometer.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_orientation.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_orientation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_period_range.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_period_range.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_person.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_person.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_primary_data.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_primary_data.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_processing_info.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_processing_info.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_processing_software.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_processing_software.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_provenance.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_provenance.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_remote_info.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_remote_info.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_remote_ref.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_remote_ref.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_run.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_run.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_site.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_site.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_site_layout.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_site_layout.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_software.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_software.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_emtfxml_statistical_estimates.rst` & `mt_metadata-0.3.5/docs/source/tf_emtfxml_statistical_estimates.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_fdsn.rst` & `mt_metadata-0.3.5/docs/source/tf_fdsn.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_filter.rst` & `mt_metadata-0.3.5/docs/source/tf_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_filter_base.rst` & `mt_metadata-0.3.5/docs/source/tf_filter_base.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_filtered.rst` & `mt_metadata-0.3.5/docs/source/tf_filtered.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_index.rst` & `mt_metadata-0.3.5/docs/source/tf_index.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_instrument.rst` & `mt_metadata-0.3.5/docs/source/tf_instrument.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_jfile_birrp_angles.rst` & `mt_metadata-0.3.5/docs/source/tf_jfile_birrp_angles.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_jfile_birrp_block.rst` & `mt_metadata-0.3.5/docs/source/tf_jfile_birrp_block.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_jfile_birrp_parameters.rst` & `mt_metadata-0.3.5/docs/source/tf_jfile_birrp_parameters.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_jfile_header.rst` & `mt_metadata-0.3.5/docs/source/tf_jfile_header.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_location.rst` & `mt_metadata-0.3.5/docs/source/tf_location.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_magnetic.rst` & `mt_metadata-0.3.5/docs/source/tf_magnetic.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_orientation.rst` & `mt_metadata-0.3.5/docs/source/tf_orientation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_person.rst` & `mt_metadata-0.3.5/docs/source/tf_person.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_band.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_band.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_channel.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_channel.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_channel_nomenclature.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_channel_nomenclature.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_decimation.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_decimation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_decimation_level.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_decimation_level.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_estimator.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_estimator.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_index.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_index.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_processing.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_processing.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_regression.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_regression.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_run.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_run.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_station.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_station.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_stations.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_stations.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_aurora_window.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_aurora_window.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_fcs_channel.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_fcs_channel.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_fcs_decimation.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_fcs_decimation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_processing_fcs_f_c.rst` & `mt_metadata-0.3.5/docs/source/tf_processing_fcs_f_c.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_provenance.rst` & `mt_metadata-0.3.5/docs/source/tf_provenance.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_rating.rst` & `mt_metadata-0.3.5/docs/source/tf_rating.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_run.rst` & `mt_metadata-0.3.5/docs/source/tf_run.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_software.rst` & `mt_metadata-0.3.5/docs/source/tf_software.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_station.rst` & `mt_metadata-0.3.5/docs/source/tf_station.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_statistical_estimate.rst` & `mt_metadata-0.3.5/docs/source/tf_statistical_estimate.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_structure.rst` & `mt_metadata-0.3.5/docs/source/tf_structure.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_survey.rst` & `mt_metadata-0.3.5/docs/source/tf_survey.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_time_period.rst` & `mt_metadata-0.3.5/docs/source/tf_time_period.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_timing_system.rst` & `mt_metadata-0.3.5/docs/source/tf_timing_system.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_transfer_function.rst` & `mt_metadata-0.3.5/docs/source/tf_transfer_function.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zmm_channel.rst` & `mt_metadata-0.3.5/docs/source/tf_zmm_channel.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_auto.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_auto.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_c_h.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_c_h.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_d_plus.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_d_plus.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_g_d_p.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_g_d_p.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_g_p_s.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_g_p_s.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_header.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_header.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_job.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_job.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_line.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_line.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_m_t_edit.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_m_t_edit.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_m_t_f_t24.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_m_t_f_t24.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_phase_slope.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_phase_slope.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_rx.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_rx.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_s_t_n.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_s_t_n.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_survey.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_survey.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_tx.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_tx.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/tf_zonge_unit.rst` & `mt_metadata-0.3.5/docs/source/tf_zonge_unit.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_auxiliary.rst` & `mt_metadata-0.3.5/docs/source/ts_auxiliary.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_battery.rst` & `mt_metadata-0.3.5/docs/source/ts_battery.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_channel.rst` & `mt_metadata-0.3.5/docs/source/ts_channel.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_citation.rst` & `mt_metadata-0.3.5/docs/source/ts_citation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_copyright.rst` & `mt_metadata-0.3.5/docs/source/ts_copyright.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_data_logger.rst` & `mt_metadata-0.3.5/docs/source/ts_data_logger.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_data_quality.rst` & `mt_metadata-0.3.5/docs/source/ts_data_quality.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_declination.rst` & `mt_metadata-0.3.5/docs/source/ts_declination.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_diagnostic.rst` & `mt_metadata-0.3.5/docs/source/ts_diagnostic.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_electric.rst` & `mt_metadata-0.3.5/docs/source/ts_electric.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_electrode.rst` & `mt_metadata-0.3.5/docs/source/ts_electrode.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_fdsn.rst` & `mt_metadata-0.3.5/docs/source/ts_fdsn.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_base.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_base.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_channel_response_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_channel_response_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_coefficient_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_coefficient_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_f_i_r_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_f_i_r_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_frequency_response_table_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_frequency_response_table_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_pole_zero_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_pole_zero_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filter_time_delay_filter.rst` & `mt_metadata-0.3.5/docs/source/ts_filter_time_delay_filter.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_filtered.rst` & `mt_metadata-0.3.5/docs/source/ts_filtered.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_funding_source.rst` & `mt_metadata-0.3.5/docs/source/ts_funding_source.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_geographic_location.rst` & `mt_metadata-0.3.5/docs/source/ts_geographic_location.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_index.rst` & `mt_metadata-0.3.5/docs/source/ts_index.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_instrument.rst` & `mt_metadata-0.3.5/docs/source/ts_instrument.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_location.rst` & `mt_metadata-0.3.5/docs/source/ts_location.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_magnetic.rst` & `mt_metadata-0.3.5/docs/source/ts_magnetic.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_metadata_guide.rst` & `mt_metadata-0.3.5/docs/source/ts_metadata_guide.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_orientation.rst` & `mt_metadata-0.3.5/docs/source/ts_orientation.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_person.rst` & `mt_metadata-0.3.5/docs/source/ts_person.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_provenance.rst` & `mt_metadata-0.3.5/docs/source/ts_provenance.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_rating.rst` & `mt_metadata-0.3.5/docs/source/ts_rating.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_run.rst` & `mt_metadata-0.3.5/docs/source/ts_run.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_software.rst` & `mt_metadata-0.3.5/docs/source/ts_software.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_station.rst` & `mt_metadata-0.3.5/docs/source/ts_station.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_survey.rst` & `mt_metadata-0.3.5/docs/source/ts_survey.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_time_period.rst` & `mt_metadata-0.3.5/docs/source/ts_time_period.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/source/ts_timing_system.rst` & `mt_metadata-0.3.5/docs/source/ts_timing_system.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/docs/usage.rst` & `mt_metadata-0.3.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/__init__.py` & `mt_metadata-0.3.5/mt_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # =============================================================================
 # Package details
 # =============================================================================
 
 
 __author__ = """Jared Peacock"""
 __email__ = "jpeacock@usgs.gov"
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 # =============================================================================
 # Imports
 # =============================================================================
 import sys
 from pathlib import Path
```

### Comparing `mt_metadata-0.3.4/mt_metadata/base/helpers.py` & `mt_metadata-0.3.5/mt_metadata/base/helpers.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/base/metadata.py` & `mt_metadata-0.3.5/mt_metadata/base/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,44 +296,44 @@
 
         try:
             return validate_value_type(value, v_type, style=style)
         except MTSchemaError as error:
             self.logger.exception(error)
             raise MTSchemaError(error)
 
-    def _validate_option(self, name, option_list):
+    def _validate_option(self, name, value, option_list):
         """
         validate the given attribute name agains possible options and check
         for aliases
 
         :param name: DESCRIPTION
         :type name: TYPE
         :param option_list: DESCRIPTION
         :type option_list: TYPE
         :param alias_list: DESCRIPTION
         :type alias_list: TYPE
         :return: DESCRIPTION
         :rtype: TYPE
 
         """
-        if name is None:
+        if value is None:
             return True, False, None
         options = [ss.lower() for ss in option_list]
         other_possible = False
         if "other" in options:
             other_possible = True
-        if name.lower() in options:
+        if value.lower() in options:
             return True, other_possible, None
-        elif name.lower() not in options and other_possible:
+        elif value.lower() not in options and other_possible:
             msg = (
-                "{0} not found in options list {1}, but other options"
-                + " are allowed.  Allowing {2} to be set to {0}."
+                f"Value '{value}' not found for metadata field '{name}' in options list {option_list}, but other options"
+                + f" are allowed.  Allowing {option_list} to be set to {value}."
             )
             return True, other_possible, msg
-        return False, other_possible, "{0} not found in options list {1}"
+        return False, other_possible, f"Value '{value}' for metadata field '{name}' not found in options list {option_list}"
 
     def __setattr__(self, name, value):
         """
         set attribute based on metadata standards
 
         Something here doesnt allow other objects to be set as attributes
 
@@ -395,15 +395,15 @@
             try:
                 v_dict = self._attr_dict[name]
                 v_type = self._get_standard_type(name)
                 value = self._validate_type(value, v_type, v_dict["style"])
                 # check options
                 if v_dict["style"] == "controlled vocabulary":
                     options = v_dict["options"]
-                    accept, other, msg = self._validate_option(value, options)
+                    accept, other, msg = self._validate_option(name, value, options)
                     if not accept:
                         self.logger.error(msg.format(value, options))
                         raise MTSchemaError(msg.format(value, options))
                     if other and not accept:
                         self.logger.warning(msg.format(value, options, name))
                 super().__setattr__(name, value)
             except KeyError as error:
```

### Comparing `mt_metadata-0.3.4/mt_metadata/base/schema.py` & `mt_metadata-0.3.5/mt_metadata/base/schema.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/mt_xml/multi_run_experiment.xml` & `mt_metadata-0.3.5/mt_metadata/data/mt_xml/multi_run_experiment.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/mt_xml/multi_run_experiment_02.xml` & `mt_metadata-0.3.5/mt_metadata/data/mt_xml/multi_run_experiment_02.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/mt_xml/single_station_mt_experiment.xml` & `mt_metadata-0.3.5/mt_metadata/data/mt_xml/single_station_mt_experiment.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/fdsn_no_mt_info.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/fdsn_no_mt_info.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_electrode_example.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_electrode_example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_magnetometer_example.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_magnetometer_example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/mtml_single_station.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/mtml_single_station.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/multiple_networks_example.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/multiple_networks_example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/station_xml_with_fap_example.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/station_xml_with_fap_example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/stationxml/station_xml_with_fir_example.xml` & `mt_metadata-0.3.5/mt_metadata/data/stationxml/station_xml_with_fir_example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/NMX20.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/NMX20.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/PHXTest01.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/PHXTest01.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/example.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/example.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/test.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/test.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg.avg` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg.avg`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg_newer.avg` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg_newer.avg`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_avg_tipper.avg` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_avg_tipper.avg`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_cgg.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_cgg.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_empower.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_empower.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_metronix.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_metronix.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_no_error.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_no_error.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_phoenix.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_phoenix.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_quantec.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_quantec.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_rho_only.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_rho_only.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_spectra_in.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_spectra_in.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_edi_spectra_out.edi` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_edi_spectra_out.edi`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_jfile.j` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_jfile.j`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_poor_xml.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_poor_xml.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_bad_comments.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_bad_comments.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_complete_remote_info.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_complete_remote_info.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_emtf_xml_iris.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_emtf_xml_iris.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_multiple_attachments.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_multiple_attachments.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_no_site_layout.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_no_site_layout.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_xml_with_derived_quantities.xml` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_xml_with_derived_quantities.xml`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_zmm.zmm` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_zmm.zmm`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/data/transfer_functions/tf_zss_tipper.zss` & `mt_metadata-0.3.5/mt_metadata/data/transfer_functions/tf_zss_tipper.zss`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/__init__.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/auxiliary.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/auxiliary.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/battery.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/battery.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/channel.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/citation.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/citation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/copyright.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/copyright.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/data_logger.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/data_logger.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/data_quality.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/data_quality.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/declination.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/declination.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/diagnostic.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/diagnostic.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/electric.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/electric.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/electrode.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/electrode.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/experiment.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/experiment.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/fdsn.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/fdsn.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/channel_response.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/channel_response.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/coefficient_filter.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/coefficient_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/filter_base.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/filter_base.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/filtered.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/filtered.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/fir_filter.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/fir_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/frequency_response_table_filter.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/frequency_response_table_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/helper_functions.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/helper_functions.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/obspy_stages.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/obspy_stages.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/plotting_helpers.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/pole_zero_filter.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/pole_zero_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/filter_base.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/filter_base.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/fir_filter.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/fir_filter.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/frequency_response_table_filter.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/frequency_response_table_filter.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/standards/pole_zero_filter.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/standards/pole_zero_filter.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/filters/time_delay_filter.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/filters/time_delay_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/funding_source.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/funding_source.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/geographic_location.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/geographic_location.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/instrument.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/instrument.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/location.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/location.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/magnetic.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/magnetic.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/orientation.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/orientation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/person.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/person.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/provenance.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/provenance.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/rating.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/rating.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/run.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/software.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/software.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/auxiliary.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/auxiliary.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/battery.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/battery.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/channel.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/channel.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/citation.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/citation.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/copyright.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/copyright.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/data_quality.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/data_quality.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/declination.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/declination.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/diagnostic.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/diagnostic.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/electric.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/electric.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/fdsn.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/fdsn.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/filtered.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/filtered.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/funding_source.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/funding_source.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/geographic_location.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/geographic_location.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/instrument.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/instrument.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/location.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/location.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/magnetic.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/magnetic.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/orientation.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/orientation.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/person.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/person.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/provenance.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/provenance.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/rating.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/rating.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/run.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/run.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/software.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/software.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/station.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/station.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/survey.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/survey.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/time_period.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/time_period.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/standards/timing_system.json` & `mt_metadata-0.3.5/mt_metadata/timeseries/standards/timing_system.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/station.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/__init__.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/fdsn_tools.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/fdsn_tools.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/utils.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/utils.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_channel_mt_channel.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_channel_mt_channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_equipment_mt_run.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_equipment_mt_run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_inventory_mt_experiment.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_inventory_mt_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,18 @@
             self.logger.error(msg)
             raise ValueError(msg)
         xml_inventory = inventory.Inventory()
         for mt_survey in mt_experiment.surveys:
             xml_network = self.network_translator.mt_to_xml(mt_survey)
             for mt_station in mt_survey.stations:
                 xml_station = self.station_translator.mt_to_xml(mt_station)
-                xml_station.site.country = mt_survey.country
+                if mt_survey.country is not None:
+                    xml_station.site.country = ",".join(
+                        [str(country) for country in mt_survey.country]
+                    )
                 for mt_run in mt_station.runs:
                     xml_station = self.add_run(
                         xml_station, mt_run, mt_survey.filters
                     )
                 xml_network.stations.append(xml_station)
             xml_inventory.networks.append(xml_network)
         if stationxml_fn:
```

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_network_mt_survey.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_network_mt_survey.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/stationxml/xml_station_mt_station.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/stationxml/xml_station_mt_station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/survey.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/survey.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/time_period.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/time_period.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/timing_system.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/timing_system.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/timeseries/tools/from_many_mt_files.py` & `mt_metadata-0.3.5/mt_metadata/timeseries/tools/from_many_mt_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,32 @@
 # =============================================================================
 # Imports
 # =============================================================================
 from pathlib import Path
 import pandas as pd
 from xml.etree import cElementTree as et
 
-from mt_metadata.timeseries import Experiment, Survey, Station, Run, Electric, Magnetic
+from mt_metadata.timeseries import (
+    Experiment,
+    Survey,
+    Station,
+    Run,
+    Electric,
+    Magnetic,
+)
 
 from mt_metadata.timeseries.filters import (
     PoleZeroFilter,
     CoefficientFilter,
     TimeDelayFilter,
     FIRFilter,
 )
 from mt_metadata.timeseries.stationxml import XMLInventoryMTExperiment
 
+
 # =============================================================================
 # Useful Class
 # =============================================================================
 class MT2StationXML(XMLInventoryMTExperiment):
     """
     A class to convert multiple MT xml files into a stationXML (MTML)
 
@@ -178,29 +186,33 @@
                 & (self.df.is_channel == True)
             ].fn
         )
 
         channels_list = []
         for ch in order:
             for fn in rdf:
-                if ch in fn.name.lower():
+                if ch in fn.name[len(station) :].lower():
                     channels_list.append(fn)
                     break
 
         return channels_list
 
     def sort_by_station(self, stations=None):
         """
         sort the file into station, runs and channels
 
         :return: DESCRIPTION
         :rtype: TYPE
 
         """
-        fn_dict = {"survey": self.survey, "filters": self.filters, "stations": []}
+        fn_dict = {
+            "survey": self.survey,
+            "filters": self.filters,
+            "stations": [],
+        }
         if stations in [None, []]:
             station_iterator = self.stations
         else:
             if isinstance(stations, str):
                 stations = [stations]
             if not isinstance(stations, list):
                 raise ValueError("stations must be a list of stations")
```

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/core.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/core.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/edi.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/data_section.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/data_section.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/define_measurement.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/define_measurement.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/emeasurement.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/emeasurement.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/header.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/header.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/hmeasurement.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/hmeasurement.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/information.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/information.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/data_section.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/data_section.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/define_measurement.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/define_measurement.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/emeasurement.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/emeasurement.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/header.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/header.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/edi/metadata/standards/hmeasurement.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/edi/metadata/standards/hmeasurement.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/emtfxml.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/emtfxml.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/__init__.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/attachment.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/attachment.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/channels.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/channels.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/citation.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/citation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/comment.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/comment.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/copyright.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/copyright.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_notes.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_notes.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_warnings.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_quality_warnings.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_type.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_type.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/data_types.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/data_types.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/dipole.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/dipole.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/electric.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/electric.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/electrode.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/electrode.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/emtf.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/emtf.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/estimate.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/estimate.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/external_url.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/external_url.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/field_notes.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/field_notes.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/helpers.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/helpers.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/instrument.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/instrument.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/location.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/location.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetic.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetic.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetometer.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/magnetometer.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/orientation.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/orientation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/period_range.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/period_range.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/person.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/person.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/primary_data.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/primary_data.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/processing_info.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/processing_info.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/provenance.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/provenance.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_info.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_info.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_ref.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/remote_ref.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/run.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/site.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/site.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/site_layout.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/site_layout.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/software.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/software.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/attachment.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/attachment.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/channels.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/channels.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/citation.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/citation.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/comment.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/comment.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/copyright.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/copyright.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_notes.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_quality_notes.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_type.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/data_type.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/dipole.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/dipole.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electric.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electric.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electrode.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/electrode.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/emtf.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/emtf.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/estimate.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/estimate.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/external_url.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/external_url.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/location.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/location.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetic.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetic.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetometer.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/magnetometer.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/orientation.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/orientation.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/period_range.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/period_range.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/person.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/person.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/processing_info.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/processing_info.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/provenance.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/provenance.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/run.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/run.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site_layout.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/site_layout.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/software.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/software.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/value.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/standards/value.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/emtfxml/metadata/statistical_estimates.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/emtfxml/metadata/statistical_estimates.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/jfile.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/jfile.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_angles.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_angles.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_block.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_block.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_parameters.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/birrp_parameters.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/header.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/header.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_angles.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_angles.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_block.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_block.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_parameters.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/birrp_parameters.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/jfiles/metadata/standards/header.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/jfiles/metadata/standards/header.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/tools.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/tools.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/channel.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/metadata/standards/channel.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/metadata/standards/channel.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zfiles/zmm.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zfiles/zmm.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/__init__.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/auto.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/auto.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/ch.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/ch.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/d_plus.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/d_plus.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/gdp.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/gdp.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/gps.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/gps.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/header.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/header.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/job.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/job.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/line.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/line.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/mt_edit.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/mt_edit.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/mtft24.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/mtft24.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/phase_slope.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/phase_slope.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/rx.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/rx.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/ch.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/ch.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/gdp.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/gdp.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/gps.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/gps.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/job.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/job.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/line.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/line.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/phase_slope.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/phase_slope.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/rx.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/rx.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/survey.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/survey.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/standards/unit.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/standards/unit.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/stn.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/stn.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/survey.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/survey.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/tx.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/tx.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/metadata/unit.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/metadata/unit.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/io/zonge/zonge.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/io/zonge/zonge.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/__init__.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/band.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/band.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # =============================================================================
 class Band(Base):
     __doc__ = write_lines(attr_dict)
 
     def __init__(self, **kwargs):
 
         super().__init__(attr_dict=attr_dict, **kwargs)
+        self._name = None
 
     @property
     def lower_bound(self):
         return self.frequency_min
 
     @property
     def upper_bound(self):
@@ -37,14 +38,29 @@
     def lower_closed(self):
         return self.to_interval().closed_left
 
     @property
     def upper_closed(self):
         return self.to_interval().closed_right
 
+    @property
+    def name(self):
+        """
+        :return: The name of the frequency band (currently defaults to fstring with 6 decimal places.
+        :rtype: str
+        """
+        if self._name is None:
+            self._name = f"{self.center_frequency:.6f}"
+        return self._name
+
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
     def _indices_from_frequencies(self, frequencies):
         """
 
         Parameters
         ----------
         frequencies: numpy array
             Intended to represent the one-sided (positive) frequency axis of
```

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/channel.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/channel_nomenclature.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/channel_nomenclature.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/decimation.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/decimation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/decimation_level.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/decimation_level.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/estimator.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/estimator.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/processing.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/processing.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/regression.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/regression.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/run.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/band.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/band.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/channel.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/channel.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclature.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/channel_nomenclature.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/config.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/config.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/decimation.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/decimation.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/decimation_level.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/decimation_level.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/estimator.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/estimator.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/processing.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/processing.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/regression.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/regression.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/run.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/run.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/station.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/station.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/standards/window.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/standards/window.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/station.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/stations.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/stations.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/aurora/window.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/aurora/window.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/decimation.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/decimation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/fc.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/fc.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/fc_channel.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/fc_channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/decimation.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/decimation.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976851851851851%*

 * *Differences: {"'decimation_level'": "{'description': 'Decimation level, must be a non-negative integer starting "*

 * *                       "at 0'}"}*

```diff
@@ -31,15 +31,15 @@
         "style": "number",
         "type": "integer",
         "units": null
     },
     "decimation_level": {
         "alias": [],
         "default": null,
-        "description": "Decimation level, must be a positive integer starting at 0.",
+        "description": "Decimation level, must be a non-negative integer starting at 0",
         "example": "1",
         "options": [],
         "required": true,
         "style": "number",
         "type": "integer",
         "units": null
     },
```

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc_channel.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/processing/fourier_coefficients/standards/fc_channel.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/__init__.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/comment.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/comment.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/comment.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/comment.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/station.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/station.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/statistical_estimate.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/statistical_estimate.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/survey.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/survey.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/standards/transfer_function.json` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/standards/transfer_function.json`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/station.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/statistical_estimate.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/statistical_estimate.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/survey.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/survey.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/transfer_functions/tf/transfer_function.py` & `mt_metadata-0.3.5/mt_metadata/transfer_functions/tf/transfer_function.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/utils/list_dict.py` & `mt_metadata-0.3.5/mt_metadata/utils/list_dict.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/utils/mttime.py` & `mt_metadata-0.3.5/mt_metadata/utils/mttime.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/utils/summarize.py` & `mt_metadata-0.3.5/mt_metadata/utils/summarize.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/utils/units.py` & `mt_metadata-0.3.5/mt_metadata/utils/units.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata/utils/validators.py` & `mt_metadata-0.3.5/mt_metadata/utils/validators.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/mt_metadata.egg-info/PKG-INFO` & `mt_metadata-0.3.5/mt_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mt-metadata
-Version: 0.3.4
+Version: 0.3.5
 Summary: Metadata for magnetotelluric data
 Home-page: https://github.com/kujaku11/mt_metadata
 Author: Jared Peacock
 Author-email: jpeacock@usgs.gov
 License: MIT license
 Keywords: mt_metadata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# mt_metadata version 0.3.4
+# mt_metadata version 0.3.5
  Standard MT metadata
 
 [![PyPi version](https://img.shields.io/pypi/v/mt_metadata.svg)](https://pypi.python.org/pypi/mt-metadata)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mt-metadata.svg)](https://anaconda.org/conda-forge/mt-metadata)
 [![codecov](https://codecov.io/gh/kujaku11/mt_metadata/branch/main/graph/badge.svg?token=1WYF0G1L3D)](https://codecov.io/gh/kujaku11/mt_metadata)
 ![example workflow name](https://github.com/kujaku11/mt_metadata/workflows/TestingInConda/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -48,15 +48,15 @@
         - **ZMM** (Egberts EMTF output)
         - **JFILE** (BIRRP output)
         - **EMTFXML** (Kelbert's format)
         - **AVG** (Zonge output)
 
 Most people will be using the transfer functions, but a lot of that metadata comes from the time series metadata.  This module supports both and has tried to make them more or less seamless to reduce complication.
 
-* **Version**: 0.3.4
+* **Version**: 0.3.5
 * **Free software**: MIT license
 * **Documentation**: https://mt-metadata.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **mt_metadata/examples/notebooks** and **docs/source/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 # Installation
```

### Comparing `mt_metadata-0.3.4/mt_metadata.egg-info/SOURCES.txt` & `mt_metadata-0.3.5/mt_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/setup.py` & `mt_metadata-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     keywords="mt_metadata",
     name="mt_metadata",
     packages=find_packages(include=["mt_metadata", "mt_metadata.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/kujaku11/mt_metadata",
-    version="0.3.4",
+    version="0.3.5",
     zip_safe=False,
     package_data={
         "": [
             "data/mt_xml/*.xml",
             "data/stationxml/*.xml",
             "data/transfer_functions/*.edi",
         ]
```

### Comparing `mt_metadata-0.3.4/tests/test_helpers.py` & `mt_metadata-0.3.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_list_dict.py` & `mt_metadata-0.3.5/tests/test_list_dict.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_metadata.py` & `mt_metadata-0.3.5/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_mttime.py` & `mt_metadata-0.3.5/tests/test_mttime.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_schema.py` & `mt_metadata-0.3.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_standards_exist.py` & `mt_metadata-0.3.5/tests/test_standards_exist.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 """
 
 import unittest
 from pathlib import Path
 
 
 def get_standard_dirs(dir_path):
-    existing_dirs = list(set([fn.parent.as_posix() for fn in dir_path.rglob("*.json")]))
+    existing_dirs = list(
+        set([fn.parent.as_posix() for fn in dir_path.rglob("*.json")])
+    )
     existing_dirs = [
-        fn[fn.rfind("mt_metadata") :] for fn in existing_dirs if ".git" not in fn
+        fn[fn.rfind("mt_metadata") :]
+        for fn in existing_dirs
+        if ".git" not in fn
     ]
 
     return sorted(set(existing_dirs))
 
 
 def read_manifest(fn):
     lines = fn.read_text().split("\n")
@@ -37,15 +41,15 @@
         self.maxDiff = None
         self.home = Path(__file__).parent.parent
         self.manifest_fn = self.home.joinpath("MANIFEST.in")
         if not self.manifest_fn.exists():
             self.manifest_fn = self.home.parent.joinpath("MANIFEST.in")
 
     def test_standards_exist(self):
-        existing_dirs = get_standard_dirs(self.home)
+        existing_dirs = get_standard_dirs(self.home.joinpath(self.home.name))
         manifest_dirs = read_manifest(self.manifest_fn)
         self.assertListEqual(existing_dirs, manifest_dirs)
 
 
 # =============================================================================
 # run
 # =============================================================================
```

### Comparing `mt_metadata-0.3.4/tests/test_summarize.py` & `mt_metadata-0.3.5/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_units.py` & `mt_metadata-0.3.5/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/test_validators.py` & `mt_metadata-0.3.5/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_cgg_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_cgg_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_edi_spectra.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_edi_spectra.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_empower_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_empower_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_metronix_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_metronix_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_no_error_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_no_error_edi.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 ("enddate", "2020-04-28T00:00:00+00:00"),
                 ("fileby", "PSJ"),
                 ("filedate", "2021-03-25"),
                 ("latitude", 0.0),
                 ("longitude", 0.0),
                 ("progdate", "2013-07-03"),
                 ("progname", "mt_metadata"),
-                ("progvers", "0.3.4"),
+                ("progvers", "0.3.5"),
                 ("stdvers", "SEG 1.0"),
                 ("units", "millivolts_per_kilometer_per_nanotesla"),
             ]
         )
 
         for key, value in head.items():
             with self.subTest(key):
```

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_phoenix_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_phoenix_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_quantec_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_quantec_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/edi/test_rho_only_edi.py` & `mt_metadata-0.3.5/tests/tf/io/edi/test_rho_only_edi.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_emtfxml.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_emtfxml.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_emtfxml_poor.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_emtfxml_poor.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_multiple_attachments.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_multiple_attachments.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_complete_remote_info.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_complete_remote_info.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_derived_quantities.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_derived_quantities.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_no_site_layout.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_no_site_layout.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_read_poor.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_read_poor.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write_complete_remote_info.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write_complete_remote_info.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/emtfxml/test_tf_write_poor.py` & `mt_metadata-0.3.5/tests/tf/io/emtfxml/test_tf_write_poor.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/jfile/test_jfile.py` & `mt_metadata-0.3.5/tests/tf/io/jfile/test_jfile.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/jfile/test_tf_read.py` & `mt_metadata-0.3.5/tests/tf/io/jfile/test_tf_read.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zmm/test_tf_read_zmm.py` & `mt_metadata-0.3.5/tests/tf/io/zmm/test_tf_read_zmm.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zmm/test_tf_read_zss.py` & `mt_metadata-0.3.5/tests/tf/io/zmm/test_tf_read_zss.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zmm/test_zmm.py` & `mt_metadata-0.3.5/tests/tf/io/zmm/test_zmm.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zmm/test_zss.py` & `mt_metadata-0.3.5/tests/tf/io/zmm/test_zss.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read_newer.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read_newer.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_tf_read_tipper.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_tf_read_tipper.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge_newer.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge_newer.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/io/zonge/test_zonge_tipper.py` & `mt_metadata-0.3.5/tests/tf/io/zonge/test_zonge_tipper.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_band.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_band.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         self.freqs = 0.1 * np.arange(100)  # 0-10Hz
         self.min_freq = 2.0
         self.max_freq = 3.0
         self.band = Band(
             frequency_min=self.min_freq, frequency_max=self.max_freq
         )
 
+    def test_copy(self):
+        cloned = self.band.copy()
+        self.assertEqual(self.band, cloned)
+        
     def test_lower_bound(self):
         self.assertEqual(self.band.lower_bound, self.min_freq)
 
     def test_upper_bound(self):
         self.assertEqual(self.band.upper_bound, self.max_freq)
 
     def test_lower_closed(self):
@@ -92,14 +96,18 @@
     def test_center_frequency_arithmetic(self):
         self.band.center_averaging_type = "arithmetic"
         with self.subTest("frequency"):
             self.assertAlmostEqual(self.band.center_frequency, 2.5)
         with self.subTest("period"):
             self.assertAlmostEqual(self.band.center_period, 1.0 / 2.5)
 
+    def test_name(self):
+        self.assertTrue(isinstance(self.band.name, str))
+
+
 
 class TestBandClosedRight(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         self.freqs = 0.1 * np.arange(100)  # 0-10Hz
         self.min_freq = 2.0
         self.max_freq = 3.0
```

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_channel_nomenclature.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_channel_nomenclature.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_dataset_dataframe.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_dataset_dataframe.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_decimation.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_decimation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_estimator.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_estimator.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_frequency_bands.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_frequency_bands.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_processing.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_processing.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_regression.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_regression.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_station.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_stations.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_stations.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/aurora/test_window.py` & `mt_metadata-0.3.5/tests/tf/processing/aurora/test_window.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/fcs/test_decimation.py` & `mt_metadata-0.3.5/tests/tf/processing/fcs/test_decimation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/fcs/test_fc.py` & `mt_metadata-0.3.5/tests/tf/processing/fcs/test_fc.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/processing/fcs/test_fc_channel.py` & `mt_metadata-0.3.5/tests/tf/processing/fcs/test_fc_channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_core_tf.py` & `mt_metadata-0.3.5/tests/tf/test_core_tf.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_get_elevation.py` & `mt_metadata-0.3.5/tests/tf/test_get_elevation.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_run.py` & `mt_metadata-0.3.5/tests/tf/test_run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_station.py` & `mt_metadata-0.3.5/tests/tf/test_station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_survey.py` & `mt_metadata-0.3.5/tests/tf/test_survey.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/tf/test_tf_merge.py` & `mt_metadata-0.3.5/tests/tf/test_tf_merge.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_channel_response.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_channel_response.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_coefficient_filter.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_coefficient_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_electric_unit.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_electric_unit.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_fap_filter.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_fap_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_filter_base.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_filter_base.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_filtered.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_filtered.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_magnetic_unit.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_magnetic_unit.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_time_delay_filter.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_time_delay_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/filters/test_zpk_filter.py` & `mt_metadata-0.3.5/tests/timeseries/filters/test_zpk_filter.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_base_translator.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_base_translator.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_channel.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_experiment_to_stationxml.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_experiment_to_stationxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,13 +178,24 @@
                 self.inventory.networks[0].start_date <= min(c_start)
             )
 
         with self.subTest("test station end time period in channels"):
             c_end = [c.end_date for c in self.inventory.networks[0].stations]
             self.assertTrue(self.inventory.networks[0].end_date >= max(c_end))
 
+    def test_country_is_string(self):
+        with self.subTest("is string"):
+            self.assertIsInstance(
+                self.inventory.networks[0].stations[0].site.country, str
+            )
+
+        with self.subTest("is equal"):
+            self.assertEqual(
+                self.inventory.networks[0].stations[0].site.country, "USA"
+            )
+
 
 # =============================================================================
 # Run
 # =============================================================================
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_fap.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_fap.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_fdsn_tools.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_fdsn_tools.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_inventory.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_inventory.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_network.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_network.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_renaming_filters.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_renaming_filters.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_run.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_station.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_translations_electric.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_translations_electric.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/stationxml/test_translations_magnetic.py` & `mt_metadata-0.3.5/tests/timeseries/stationxml/test_translations_magnetic.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_channel.py` & `mt_metadata-0.3.5/tests/timeseries/test_channel.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_electric.py` & `mt_metadata-0.3.5/tests/timeseries/test_electric.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_experiment.py` & `mt_metadata-0.3.5/tests/timeseries/test_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         self.experiment = Experiment()
         self.start = "2020-01-01T00:00:00+00:00"
         self.end = "2021-01-01T12:00:00+00:00"
 
         kwargs = {"time_period.start": self.start, "time_period.end": self.end}
 
         for survey in ["One", "Two"]:
-            survey_obj = Survey(id=survey)
+            survey_obj = Survey(id=survey, country="USA")
             survey_obj.filters = {}
             for station in ["mt01", "mt02"]:
                 station_obj = Station(id=station, **kwargs)
                 for run in ["mt01a", "mt01b"]:
                     run_obj = Run(id=run, **kwargs)
                     for ch in ["ex", "ey"]:
                         ch_obj = Electric(component=ch, **kwargs)
@@ -117,17 +117,16 @@
                 survey_obj.update_time_period()
             self.experiment.surveys.append(survey_obj)
 
     def test_write_xml(self):
         experiment_xml = self.experiment.to_xml(required=True)
         experiment_02 = Experiment()
         experiment_02.from_xml(element=experiment_xml)
-        self.assertDictEqual(
-            self.experiment.to_dict(), experiment_02.to_dict()
-        )
+
+        self.assertDictEqual(self.experiment.to_dict(), experiment_02.to_dict())
 
     def test_survey_time_period(self):
         with self.subTest("start"):
             self.assertEqual(
                 self.start, self.experiment.surveys[0].time_period.start
             )
         with self.subTest("end"):
@@ -196,15 +195,14 @@
                     d["experiment"]["surveys"][0]["stations"][0]["runs"][0][
                         "channels"
                     ]
                 ),
             )
 
     def test_from_dict(self):
-
         d = self.experiment.to_dict()
         ex = Experiment()
         ex.from_dict(d, skip_none=False)
 
         self.assertDictEqual(ex.to_dict(), self.experiment.to_dict())
 
     def test_from_dict_fail(self):
```

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_location.py` & `mt_metadata-0.3.5/tests/timeseries/test_location.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_magnetic.py` & `mt_metadata-0.3.5/tests/timeseries/test_magnetic.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_run.py` & `mt_metadata-0.3.5/tests/timeseries/test_run.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_station.py` & `mt_metadata-0.3.5/tests/timeseries/test_station.py`

 * *Files identical despite different names*

### Comparing `mt_metadata-0.3.4/tests/timeseries/test_survey.py` & `mt_metadata-0.3.5/tests/timeseries/test_survey.py`

 * *Files identical despite different names*

