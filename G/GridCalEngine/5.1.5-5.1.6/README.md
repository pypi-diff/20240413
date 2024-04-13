# Comparing `tmp/GridCalEngine-5.1.5.tar.gz` & `tmp/GridCalEngine-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalEngine-5.1.5.tar", last modified: Thu Apr 11 17:55:28 2024, max compression
+gzip compressed data, was "GridCalEngine-5.1.6.tar", last modified: Sat Apr 13 14:14:19 2024, max compression
```

## Comparing `GridCalEngine-5.1.5.tar` & `GridCalEngine-5.1.6.tar`

### file list

```diff
@@ -1,678 +1,678 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)    11061 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/data_logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39202 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/enumerations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23740 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/basic_structures.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/api.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/objects_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/timeseries_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9944 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/results_table_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/iwamoto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/ips.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/powell.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/autodiff.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc_numba.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/selected_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/ortools_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/pulp_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/highs.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Topology/topology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/simulation_indices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10513 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/topology_substation_reduction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4490 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Topology/detect_substations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.5/GridCalEngine/Topology/admittance_matrices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21419 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/units.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/base/base_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/dgs/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/dgs/dgs_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/raw/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/gridcal_to_raw.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/gne_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/switched_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/system_switching_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/facts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/owner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/inter_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/vsc_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/induction_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/fixed_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_storage_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_gen_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_bus_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_branch_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    53833 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/pack_unpack.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16095 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/zip_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/json_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/generic_io_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/h5_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    47307 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/excel_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/sqlite_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/contingency_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/epc/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/epc/epc_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/IO/others/dpx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.5/GridCalEngine/IO/others/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/IO/others/ipa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.5/GridCalEngine/IO/others/pypsa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/IO/others/plx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    50379 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2227 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29743 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/base.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12411 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_export.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26404 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    82071 2024-04-11 15:31:24.470472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2416 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4230 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_devices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/base_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/psse_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/db_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/sparse_array.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/Devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   195588 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/multi_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Devices/profile.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/municipality.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2579 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3864 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2641 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/emission_gas.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/country.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/modelling_authority.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2536 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2069 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1940 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1864 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investments_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3232 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/community.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/branch_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_path.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_turbine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_injection_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_p2x.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/underground_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/series_reactance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/wire.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5553 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line_locations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/sequence_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/overhead_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/vsc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/upfc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20073 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/hvdc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/winding.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20777 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer3w.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/static_generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/external_grid.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/current_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/battery.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator_q_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/controllable_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2203 2024-04-01 07:29:23.256927 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/graphic_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/schematic_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12374 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/base_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/injection_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23830 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/editable_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6781 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/generator_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/controllable_branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5952 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/load_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7415 2024-04-11 15:31:05.586472 GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/shunt_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2339 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_emission.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2392 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2260 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/load_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.5/GridCalEngine/DataStructures/bus_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/branch_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_turbine_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_p2x_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-11 15:31:05.582472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/numerical_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/DataStructures/generator_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_pump_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/battery_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_path_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.5/GridCalEngine/DataStructures/hvdc_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/DataStructures/shunt_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_node_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_newton_pa.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_bentayga.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-11 15:31:05.578472 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_optimods.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_pgm.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/results_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/results_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_processor_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/node_groups_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/blackout_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29395 2024-03-28 10:16:48.984877 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_estimation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26711 2024-03-28 10:16:48.988877 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-08 13:34:15.975164 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/linear_opf_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4258 2024-04-11 15:31:05.594472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44173 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54464 2024-04-11 15:31:05.590472 GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.5/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-11 17:55:28.778307 GridCalEngine-5.1.5/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-11 17:55:28.778307 GridCalEngine-5.1.5/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-12 12:41:14.135810 GridCalEngine-5.1.6/GridCalEngine/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11061 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/data_logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39202 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/enumerations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23740 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/basic_structures.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.6/GridCalEngine/api.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/objects_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/timeseries_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9944 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/results_table_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/iwamoto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/ips.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/powell.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/autodiff.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc_numba.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/selected_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/ortools_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/pulp_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/highs.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Topology/topology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21322 2024-04-11 15:31:05.594472 GridCalEngine-5.1.6/GridCalEngine/Topology/simulation_indices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10513 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Topology/topology_substation_reduction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4490 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Topology/detect_substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.6/GridCalEngine/Topology/admittance_matrices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21396 2024-04-12 07:37:45.923557 GridCalEngine-5.1.6/GridCalEngine/IO/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/units.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/base/base_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/dgs/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/dgs/dgs_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/raw/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/gridcal_to_raw.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/gne_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/switched_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/system_switching_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/facts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/owner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/inter_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/vsc_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/induction_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/fixed_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_storage_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_gen_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_bus_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_branch_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    53833 2024-04-12 14:26:56.903899 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/pack_unpack.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16095 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/zip_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    98239 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/json_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/generic_io_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/h5_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46676 2024-04-13 08:34:01.782415 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/excel_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/sqlite_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/contingency_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/epc/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/epc/epc_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/IO/others/dpx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.6/GridCalEngine/IO/others/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/IO/others/ipa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.6/GridCalEngine/IO/others/pypsa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/IO/others/plx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    50379 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2227 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30700 2024-04-12 14:39:07.187909 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/base.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12402 2024-04-12 07:37:45.923557 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_export.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26404 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    82071 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2416 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4230 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_devices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/base_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/psse_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/db_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8637 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/Devices/sparse_array.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/Devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   195588 2024-04-12 14:26:56.931899 GridCalEngine-5.1.6/GridCalEngine/Devices/multi_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14901 2024-04-11 15:31:05.590472 GridCalEngine-5.1.6/GridCalEngine/Devices/profile.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/municipality.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2579 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3864 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2641 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/emission_gas.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/country.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/modelling_authority.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2536 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2069 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1940 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1864 2024-04-11 18:07:34.878291 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investments_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3564 2024-04-12 08:49:11.587616 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/community.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/branch_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_path.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8074 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_turbine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_injection_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_p2x.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10753 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/underground_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10243 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/series_reactance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/wire.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5543 2024-04-12 14:41:25.899911 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line_locations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/sequence_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/overhead_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/vsc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/upfc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20073 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/hvdc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15880 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9392 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/winding.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20777 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11768 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer3w.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/static_generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5947 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/external_grid.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5295 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/current_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/battery.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15440 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator_q_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6879 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/controllable_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6848 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2399 2024-04-12 14:04:34.955880 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/graphic_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1078 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/schematic_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12487 2024-04-12 14:04:34.831880 GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/base_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14140 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7381 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/injection_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23830 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/editable_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6781 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/generator_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17133 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/controllable_branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5952 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/load_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17273 2024-04-11 15:31:05.586472 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7415 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/shunt_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2339 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_emission.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2392 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2260 2024-04-11 18:07:34.882291 GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/load_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.6/GridCalEngine/DataStructures/bus_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/branch_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_turbine_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_p2x_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    67032 2024-04-11 15:31:05.582472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/numerical_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/DataStructures/generator_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_pump_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/battery_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_path_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.6/GridCalEngine/DataStructures/hvdc_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/DataStructures/shunt_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_node_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_newton_pa.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_bentayga.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44207 2024-04-11 15:31:05.578472 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_optimods.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_pgm.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/results_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/results_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_processor_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/node_groups_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/blackout_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29937 2024-04-13 08:56:44.442434 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_estimation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26878 2024-04-12 06:51:51.959518 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-12 06:58:44.963524 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/linear_opf_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4258 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44173 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54464 2024-04-11 18:07:34.886291 GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.6/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-13 14:14:19.882700 GridCalEngine-5.1.6/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-13 14:14:19.882700 GridCalEngine-5.1.6/setup.cfg
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/__version__.py` & `GridCalEngine-5.1.6/GridCalEngine/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCalEngine_VERSION__ = "5.1.5"
+__GridCalEngine_VERSION__ = "5.1.6"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCalEngine_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/LICENSE.txt` & `GridCalEngine-5.1.6/GridCalEngine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/data_logger.py` & `GridCalEngine-5.1.6/GridCalEngine/data_logger.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/enumerations.py` & `GridCalEngine-5.1.6/GridCalEngine/enumerations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/basic_structures.py` & `GridCalEngine-5.1.6/GridCalEngine/basic_structures.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/api.py` & `GridCalEngine-5.1.6/GridCalEngine/api.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/objects_filtering.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/objects_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/timeseries_filtering.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/timeseries_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/filtering.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Filtering/results_table_filtering.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Filtering/results_table_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/common.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/common.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/ips.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/ips.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/powell.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/powell.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/autodiff.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/autodiff.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/NumericalMethods/sparse_solve.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/NumericalMethods/sparse_solve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc_numba.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc_numba.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/csc.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/csc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/Sparse/utils.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/Sparse/utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/selected_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/selected_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/ortools_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/ortools_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/pulp_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/pulp_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Utils/MIP/SimpleMip/highs.py` & `GridCalEngine-5.1.6/GridCalEngine/Utils/MIP/SimpleMip/highs.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Topology/topology.py` & `GridCalEngine-5.1.6/GridCalEngine/Topology/topology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Topology/simulation_indices.py` & `GridCalEngine-5.1.6/GridCalEngine/Topology/simulation_indices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Topology/topology_substation_reduction.py` & `GridCalEngine-5.1.6/GridCalEngine/Topology/topology_substation_reduction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Topology/detect_substations.py` & `GridCalEngine-5.1.6/GridCalEngine/Topology/detect_substations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Topology/admittance_matrices.py` & `GridCalEngine-5.1.6/GridCalEngine/Topology/admittance_matrices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/file_handler.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/file_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
         if isinstance(self.file_name, list):
 
             for f in self.file_name:
                 _, file_extension = os.path.splitext(f)
                 if file_extension.lower() not in ['.xml', '.zip']:
                     raise Exception('Loading multiple files that are not XML/Zip (xml or zip is for CIM or CGMES)')
-            import time
+
             data_parser = CgmesDataParser(text_func=text_func, progress_func=progress_func, logger=self.cgmes_logger)
             data_parser.load_files(files=self.file_name)
             self.cgmes_circuit = CgmesCircuit(cgmes_version=data_parser.cgmes_version, text_func=text_func,
                                               progress_func=progress_func, logger=self.cgmes_logger)
             self.cgmes_circuit.parse_files(data_parser=data_parser)
             self.circuit = cgmes_to_gridcal(cgmes_model=self.cgmes_circuit, logger=self.cgmes_logger)
         else:
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/base/units.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/base/units.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/base/base_property.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/base/base_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/dgs/dgs_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/dgs/dgs_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_legacy.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_functions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_writer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_parser_writer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/raw_to_gridcal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/raw_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/rawx_parser_legacy.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/rawx_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/gne_device.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/gne_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/switched_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/switched_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/system_switching_device.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/system_switching_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_object.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/facts.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/facts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/owner.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/owner.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/inter_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/inter_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_property.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/generator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/psse_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/psse_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/bus.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/vsc_dc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/vsc_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/induction_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/induction_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/fixed_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/fixed_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/load.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/zone.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/branch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/raw/devices/substation.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/raw/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_storage_definitions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_storage_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_gen_definitions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_gen_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_bus_definitions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_bus_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/matpower/matpower_branch_definitions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/matpower/matpower_branch_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/pack_unpack.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/pack_unpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1311,15 +1311,15 @@
 
     # create diagrams --------------------------------------------------------------------------------------------------
     if text_func is not None:
         text_func("Parsing diagrams...")
     if 'diagrams' in data.keys():
 
         if len(data['diagrams']):
-            obj_dict = circuit.gat_all_elements_dict_by_type()
+            obj_dict = circuit.get_all_elements_dict_by_type()
 
             for diagram_dict in data['diagrams']:
 
                 if diagram_dict['type'] in [DiagramType.Schematic.value, "bus-branch"]:
                     diagram = dev.SchematicDiagram()
                     diagram.parse_data(data=diagram_dict, obj_dict=obj_dict, logger=logger)
                     circuit.add_diagram(diagram)
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/zip_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/zip_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/json_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/json_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/generic_io_functions.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/generic_io_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/h5_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/h5_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/excel_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/excel_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 # just pick the DataFrame
                 df = xl.parse(name, index_col=0)
 
                 if allowed_data_sheets[name] == complex:
                     # pandas does not read complex numbers right,
                     # so when we expect a complex number input, parse directly
                     for c in df.columns.values:
-                        df[c] = df[c].apply(lambda x: np.complex(x))
+                        df[c] = df[c].apply(lambda x: complex(x))
 
                 data[name] = df
 
     else:
         raise Exception('This excel file is not in GridCal Format')
 
     return data
@@ -242,24 +242,31 @@
             if attr == 'is_enabled':
                 attr = 'active'
 
             if attr == 'type_obj':
                 attr = 'template'
 
             if hasattr(obj_, attr):
-                conv = obj_.registered_properties[attr].tpe  # get the type converter
-                if conv is None:
-                    setattr(obj_, attr, values[a])
-                elif conv is dev.BranchType:
-                    # cbr = BranchTypeConverter(None)
-                    setattr(obj_, attr, dev.BranchType(values[a]))
-                elif isinstance(conv, DeviceType):
-                    pass
+
+                prop = obj_.registered_properties.get(attr, None)
+
+                if prop is not None:
+                    conv = prop.tpe  # get the type converter
+                    if conv is None:
+                        setattr(obj_, attr, values[a])
+                    elif conv is dev.BranchType:
+                        # cbr = BranchTypeConverter(None)
+                        setattr(obj_, attr, dev.BranchType(values[a]))
+                    elif isinstance(conv, DeviceType):
+                        pass
+                    else:
+                        setattr(obj_, attr, conv(values[a]))
                 else:
-                    setattr(obj_, attr, conv(values[a]))
+                    # the property wasn't found
+                    pass
             else:
 
                 if attr in ['Y', 'Z', 'I', 'S', 'seq_resistance', 'seq_admittance', 'Zf']:
 
                     if attr == 'Z':
                         val = complex(values[a])
                         re = 1 / val.real if val.real != 0.0 else 0
@@ -311,15 +318,14 @@
         hdr = lst.columns.values
         vals = lst.values
         for i in range(len(lst)):
             obj = dev.Bus()
             set_object_attributes(obj, hdr, vals[i, :])
             bus_dict[obj.name] = obj
             circuit.add_bus(obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No buses in the file!')
 
     # add the loads ################################################################################################
     if 'load' in data.keys():
         lst = data['load']
         bus_from = lst['bus'].values
@@ -368,15 +374,14 @@
             except KeyError as ex:
                 raise Exception(str(i) + ': Load bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'Load':
                 obj.name += f"{circuit.get_loads_number()} @{bus.name}"
 
             circuit.add_load(bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No loads in the file!')
 
     # add the controlled generators ################################################################################
     if 'controlled_generator' in data.keys():
         lst = data['controlled_generator']
         bus_from = lst['bus'].values
@@ -410,15 +415,14 @@
                 raise Exception(str(i) + ': Controlled generator bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'gen':
                 obj.name += str(circuit.get_generators_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_generator(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No controlled generator in the file!')
 
     # add the batteries ############################################################################################
     if 'battery' in data.keys():
         lst = data['battery']
         bus_from = lst['bus'].values
@@ -450,15 +454,14 @@
             except KeyError as ex:
                 raise Exception(str(i) + ': Battery bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'batt':
                 obj.name += str(circuit.get_batteries_number() + 1) + '@' + bus.name
 
             circuit.add_battery(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No battery in the file!')
 
     # add the static generators ####################################################################################
     if 'static_generator' in data.keys():
         lst = data['static_generator']
         bus_from = lst['bus'].values
@@ -491,15 +494,14 @@
                 raise Exception(str(i) + ': Static generator bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'StaticGen':
                 obj.name += str(circuit.get_static_generators_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_static_generator(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No static generator in the file!')
 
     # add the shunts ###############################################################################################
     if 'shunt' in data.keys():
         lst = data['shunt']
         bus_from = lst['bus'].values
@@ -521,15 +523,14 @@
                 raise Exception(str(i) + ': Shunt bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'shunt':
                 obj.name += str(circuit.get_shunts_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_shunt(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No shunt in the file!')
 
     # Add the wires ################################################################################################
     if 'wires' in data.keys():
         lst = data['wires']
         hdr = lst.columns.values
@@ -631,15 +632,14 @@
             template_name = str(obj.template)
             if template_name in branch_types.keys():
                 obj.template = branch_types[template_name]
                 print(template_name, 'updated!')
 
             # set the branch
             circuit.add_branch(obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
 
     else:
         circuit.logger.add_warning('No Branches in the file!')
 
     # Other actions ################################################################################################
     circuit.logger += circuit.apply_all_branch_types()
 
@@ -728,15 +728,14 @@
         hdr = df.columns.values
         vals = df.values
         for i in range(len(df)):
             obj = dev.Bus()
             set_object_attributes(obj, hdr, vals[i, :])
             bus_dict[obj.name] = obj
             circuit.add_bus(obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No buses in the file!')
 
     # add the loads ################################################################################################
     if 'load' in data.keys():
         df = data['load']
         bus_from = df['bus'].values
@@ -774,15 +773,14 @@
                 raise Exception(str(i) + ': Load bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'Load':
                 obj.name += f"{circuit.get_loads_number()} @{bus.name}"
 
             obj.bus = bus
             circuit.add_load(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No loads in the file!')
 
     # add the controlled generators ################################################################################
     if 'generator' in data.keys():
         df = data['generator']
         bus_from = df['bus'].values
@@ -829,15 +827,14 @@
                 raise Exception(str(i) + ': Controlled generator bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'gen':
                 obj.name += str(circuit.get_generators_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_generator(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No controlled generator in the file!')
 
     # add the batteries ############################################################################################
     if 'battery' in data.keys():
         df = data['battery']
         bus_from = df['bus'].values
@@ -876,15 +873,14 @@
                 raise Exception(str(i) + ': Battery bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'batt':
                 obj.name += str(circuit.get_batteries_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_battery(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No battery in the file!')
 
     # add the static generators ####################################################################################
     if 'static_generator' in data.keys():
         df = data['static_generator']
         bus_from = df['bus'].values
@@ -927,15 +923,14 @@
                 raise Exception(str(i) + ': Static generator bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'StaticGen':
                 obj.name += str(circuit.get_static_generators_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_static_generator(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No static generator in the file!')
 
     # add the shunts ###############################################################################################
     if 'shunt' in data.keys():
         df = data['shunt']
         bus_from = df['bus'].values
@@ -978,15 +973,14 @@
                 raise Exception(str(i) + ': Shunt bus is not in the buses list.\n' + str(ex))
 
             if obj.name == 'shunt':
                 obj.name += str(circuit.get_shunts_number() + 1) + '@' + bus.name
 
             obj.bus = bus
             circuit.add_shunt(bus=bus, api_obj=obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
     else:
         circuit.logger.add_warning('No shunt in the file!')
 
     # Add the wires ################################################################################################
     if 'wires' in data.keys():
         df = data['wires']
         hdr = df.columns.values
@@ -1095,15 +1089,14 @@
             except KeyError as ex:
                 raise Exception(str(i) + ': Branch bus is not in the buses list.\n' + str(ex))
 
             set_object_attributes(obj, hdr, vals[i, :])
 
             # set the branch
             circuit.add_branch(obj)
-            obj.ensure_profiles_exist(circuit.time_profile)
 
             if 'branch_active_prof' in data.keys():
                 val = data['branch_active_prof'].values[:, i]
                 idx = data['branch_active_prof'].index
                 obj.set_profile_array(magnitude='active', arr=val)
 
             if 'branch_Cost_prof' in data.keys():
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/sqlite_interface.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/gridcal/contingency_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/gridcal/contingency_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/epc/epc_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/epc/epc_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/others/dpx_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/others/dpx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/others/ipa_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/others/ipa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/others/pypsa_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/others/pypsa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/others/plx_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/others/plx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_enums.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_writer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from GridCalEngine.Devices import MultiCircuit
 from GridCalEngine.Devices.Substation.bus import Bus
-from GridCalEngine.IO.cim.cgmes.base import get_new_rdfid, form_rdfid
+from GridCalEngine.IO.cim.cgmes.base import get_new_rdfid, form_rdfid, rfid2uuid
 from GridCalEngine.IO.cim.cgmes.cgmes_circuit import CgmesCircuit
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.full_model import FullModel
 from GridCalEngine.IO.cim.cgmes.base import Base
 import GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices as cgmes
 import GridCalEngine.Devices as gcdev
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices import GeneratingUnit, \
     ThermalGeneratingUnit, HydroGeneratingUnit, SolarGeneratingUnit, \
@@ -34,41 +34,44 @@
             tpe_dict[cgmes_obj.rdfid] = cgmes_obj
 
 
 # def find_terms_connections():
 #     pass   # TODO
 
 
-def find_object_by_uuid(object_list, target_uuid):  # TODO move to CGMES utils
+def find_object_by_uuid(cgmes_model: CgmesCircuit, object_list, target_uuid):  # TODO move to CGMES utils
     """
     Finds an object with the specified uuid
      in the given object_list from a CGMES Circuit.
 
     Args:
+        cgmes_model:
         object_list (list[MyObject]): List of MyObject instances.
         target_uuid (str): The uuid to search for.
 
     Returns:
         MyObject or None: The found object or None if not found.
     """
+    boundary_obj_dict = cgmes_model.all_objects_dict_boundary
+    if boundary_obj_dict is not None:
+        for k, obj in boundary_obj_dict.items():
+            if rfid2uuid(k) == target_uuid:
+                return obj
     for obj in object_list:
         if obj.uuid == target_uuid:
             return obj
     return None
 
 
-def find_object_by_tn_uuid(object_list: List[cgmes.VoltageLevel], target_uuid):
-    """ for Voltage Levels.. """
-    for obj in object_list:
-        if obj.TopologicalNode.uuid == target_uuid:
-            return obj
-    return None
-
-
-def find_object_by_vnom(object_list: List[cgmes.BaseVoltage], target_vnom):
+def find_object_by_vnom(cgmes_model: CgmesCircuit, object_list: List[cgmes.BaseVoltage], target_vnom):
+    boundary_obj_list = cgmes_model.elements_by_type_boundary.get("BaseVoltage")
+    if boundary_obj_list is not None:
+        for obj in boundary_obj_list:
+            if obj.nominalVoltage == target_vnom:
+                return obj
     for obj in object_list:
         if obj.nominalVoltage == target_vnom:
             return obj
     return None
 
 
 def find_object_by_attribute(object_list: List, target_attr_name, target_value):
@@ -170,20 +173,19 @@
                     "http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU" in bd.profile):
                 eqbd_id = bd.rdfid
             if "http://entsoe.eu/CIM/TopologyBoundary/3/1" in bd.profile:  # no TPBD in 3.0
                 tpbd_id = bd.rdfid
 
         fm_list[0].DependentOn = [eqbd_id]
         fm_list[1].DependentOn = [fm_list[0].rdfid]
+        fm_list[2].DependentOn = [fm_list[0].rdfid]
         if tpbd_id != "":
-            fm_list[2].DependentOn = [eqbd_id, tpbd_id, fm_list[0].rdfid]
-            fm_list[3].DependentOn = [tpbd_id, fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
+            fm_list[3].DependentOn = [tpbd_id, fm_list[1].rdfid, fm_list[2].rdfid]
         else:
-            fm_list[2].DependentOn = [eqbd_id, fm_list[0].rdfid]
-            fm_list[3].DependentOn = [fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
+            fm_list[3].DependentOn = [fm_list[1].rdfid, fm_list[2].rdfid]
     except TypeError:
         print("Missing default boundary files")
         fm_list[1].DependentOn = [fm_list[0].rdfid]
         fm_list[2].DependentOn = [fm_list[0].rdfid]
         fm_list[3].DependentOn = [fm_list[0].rdfid, fm_list[1].rdfid, fm_list[2].rdfid]
 
     cgmes_model.FullModel_list = fm_list
@@ -199,14 +201,15 @@
     new_rdf_id = get_new_rdfid()
     term = cgmes.Terminal(new_rdf_id)
     term.name = bus.name
     # term.phases =
     # term.ConductingEquipment = BusBarSection
     term.connected = True
     tn = find_object_by_uuid(
+        cgmes_model=cgmes_model,
         object_list=cgmes_model.TopologicalNode_list,
         target_uuid=bus.idtag
     )
 
     if isinstance(tn, cgmes.TopologicalNode):
         term.TopologicalNode = tn
     else:
@@ -323,21 +326,30 @@
 
 def get_cgmes_subgeograpical_regions(multi_circuit_model: MultiCircuit,
                                      cgmes_model: CgmesCircuit,
                                      logger: DataLogger):
     pass
 
 
+def get_base_voltage_from_boundary(cgmes_model: CgmesCircuit, vnom: float):
+    bv_list = cgmes_model.elements_by_type_boundary.get("BaseVoltage")
+    if bv_list is not None:
+        for bv in bv_list:
+            if bv.nominalVoltage == vnom:
+                return bv
+    return None
+
+
 def get_cgmes_base_voltages(multi_circuit_model: MultiCircuit,
                             cgmes_model: CgmesCircuit,
                             logger: DataLogger) -> None:
     base_volt_set = set()
     for bus in multi_circuit_model.buses:
 
-        if bus.Vnom not in base_volt_set:
+        if bus.Vnom not in base_volt_set and get_base_voltage_from_boundary(cgmes_model, vnom=bus.Vnom) is None:
             base_volt_set.add(bus.Vnom)
 
             new_rdf_id = get_new_rdfid()
             base_volt = cgmes.BaseVoltage(rdfid=new_rdf_id)
             base_volt.name = f'_BV_{int(bus.Vnom)}'
             base_volt.nominalVoltage = bus.Vnom
 
@@ -348,14 +360,15 @@
 def get_cgmes_substations(multi_circuit_model: MultiCircuit,
                           cgmes_model: CgmesCircuit,
                           logger: DataLogger) -> None:
     for mc_elm in multi_circuit_model.substations:
         substation = cgmes.Substation(rdfid=form_rdfid(mc_elm.idtag))
         substation.name = mc_elm.name
         substation.Region = find_object_by_uuid(
+            cgmes_model=cgmes_model,
             object_list=cgmes_model.SubGeographicalRegion_list,
             target_uuid=mc_elm.idtag  # TODO Community.idtag!
         )
 
         cgmes_model.add(substation)
 
 
@@ -363,22 +376,24 @@
                              cgmes_model: CgmesCircuit,
                              logger: DataLogger) -> None:
     for mc_elm in multi_circuit_model.voltage_levels:
 
         vl = cgmes.VoltageLevel(rdfid=form_rdfid(mc_elm.idtag))
         vl.name = mc_elm.name
         vl.BaseVoltage = find_object_by_vnom(
+            cgmes_model=cgmes_model,
             object_list=cgmes_model.BaseVoltage_list,
             target_vnom=mc_elm.Vnom
         )
         # vl.Bays = later
         # vl.TopologicalNode added at tn_nodes func
 
         if mc_elm.substation is not None:
             substation: cgmes.Substation = find_object_by_uuid(
+                cgmes_model=cgmes_model,
                 object_list=cgmes_model.Substation_list,
                 target_uuid=mc_elm.substation.idtag
             )
             if substation:
                 vl.Substation = substation
 
                 # link back
@@ -393,20 +408,22 @@
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
     for bus in multi_circuit_model.buses:
 
         tn = cgmes.TopologicalNode(rdfid=bus.idtag)
         tn.name = bus.name
         tn.BaseVoltage = find_object_by_vnom(
+            cgmes_model=cgmes_model,
             object_list=cgmes_model.BaseVoltage_list,
             target_vnom=bus.Vnom
         )
 
         if bus.voltage_level is not None:  # VoltageLevel
             vl: cgmes.VoltageLevel = find_object_by_uuid(
+                cgmes_model=cgmes_model,
                 object_list=cgmes_model.VoltageLevel_list,
                 target_uuid=bus.voltage_level.idtag
             )
             tn.ConnectivityNodeContainer = vl
             # link back
             vl.TopologicalNode = tn
         else:
@@ -422,32 +439,32 @@
 def get_cgmes_cn_nodes(multi_circuit_model: MultiCircuit,
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
     for mc_elm in multi_circuit_model.connectivity_nodes:
 
         cn = cgmes.ConnectivityNode(rdfid=form_rdfid(mc_elm.idtag))
         cn.name = mc_elm.name
-        tn = None
         if mc_elm.default_bus is not None:
             tn: cgmes.TopologicalNode = find_object_by_uuid(
+                cgmes_model=cgmes_model,
                 object_list=cgmes_model.TopologicalNode_list,
                 target_uuid=mc_elm.default_bus.idtag
             )
             if tn is not None:
                 cn.TopologicalNode = tn
                 cn.ConnectivityNodeContainer = tn.ConnectivityNodeContainer
                 tn.ConnectivityNodes = cn  # link back
             else:
                 logger.add_error(msg='No TopologinalNode found',
-                                 device=cn,
+                                 device=cn.name,
                                  device_class=cn.tpe)
         else:
             logger.add_error(msg='Connectivity Node has no default bus',
-                             device=mc_elm,
-                             device_class=gcdev.ConnectivityNode)
+                             device=mc_elm.name,
+                             device_class=gcdev.ConnectivityNode.type_name)
             # print(f'Topological node not found for cn: {cn.name}')
 
         cgmes_model.add(cn)
 
     return
 
 
@@ -531,16 +548,17 @@
 
     for mc_elm in multicircuit_model.external_grids:
         ei = cgmes.EquivalentInjection(rdfid=form_rdfid(mc_elm.idtag))
         ei.description = mc_elm.code
         ei.name = mc_elm.name
         ei.p = mc_elm.P
         ei.q = mc_elm.Q
-        ei.BaseVoltage = find_object_by_attribute(cgmes_model.BaseVoltage_list, "nominalVoltage",
-                                                  mc_elm.bus.Vnom)
+        ei.BaseVoltage = find_object_by_vnom(cgmes_model=cgmes_model,
+                                             object_list=cgmes_model.BaseVoltage_list,
+                                             target_vnom=mc_elm.bus.Vnom)
 
         cgmes_model.add(ei)
 
 
 def get_cgmes_ac_line_segments(multicircuit_model: MultiCircuit,
                                cgmes_model: CgmesCircuit,
                                logger: DataLogger):
@@ -554,19 +572,18 @@
     :return:
     """
     sbase = multicircuit_model.Sbase
     for mc_elm in multicircuit_model.lines:
         line = cgmes.ACLineSegment(rdfid=form_rdfid(mc_elm.idtag))
         line.description = mc_elm.code
         line.name = mc_elm.name
-        line.BaseVoltage = find_object_by_attribute(
-            object_list=cgmes_model.BaseVoltage_list,
-            target_attr_name="nominalVoltage",
-            target_value=mc_elm.get_max_bus_nominal_voltage()
-        )  # which Vnom we need?
+        line.BaseVoltage = find_object_by_vnom(cgmes_model=cgmes_model,
+                                               object_list=cgmes_model.BaseVoltage_list,
+                                               target_vnom=mc_elm.get_max_bus_nominal_voltage()
+                                               )  # which Vnom we need?
         vnom = line.BaseVoltage.nominalVoltage
 
         if vnom is not None:
             # Calculate Zbase
             zbase = (vnom * vnom) / sbase
             ybase = 1.0 / zbase
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/base.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/base.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_export.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                         "modelingAuthoritySet": "str",
                         "DependentOn": "Association",
                         "longDependentOnPF": "str",
                         "Supersedes": "str",
                         "description": "str"}
 
         for instance in self.cgmes_circuit.FullModel_list:
-            instance_dict = instance.parsed_properties
+            instance_dict = instance.__dict__
             if self.is_in_profile(instance_profiles=instance_dict.get("profile"), model_profile=profile):
                 element = Et.Element("md:FullModel", {"rdf:about": "urn:uuid:" + instance.rdfid})
                 for attr_name, attr_value in instance_dict.items():
                     if attr_name not in filter_props or attr_value is None:
                         continue
                     child = Et.Element(f"md:Model.{attr_name}")
                     if filter_props.get(attr_name) == "Association":
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_utils.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_devices.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_devices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_enums.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/cim16/cim_data_parser.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/cim16/cim_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/base_db.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/base_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/cgmes_lookup_db.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/cgmes_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/file_system.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/file_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/psse_lookup_db.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/psse_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/IO/cim/db/db_handler.py` & `GridCalEngine-5.1.6/GridCalEngine/IO/cim/db/db_handler.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/types.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/sparse_array.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/sparse_array.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/multi_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/multi_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2433,15 +2433,15 @@
             elements = self.get_elements_by_type(device_type=tpe)
 
             for elm in elements:
                 data[elm.idtag] = elm
 
         return data
 
-    def gat_all_elements_dict_by_type(self) -> dict[Callable[[], Any], Union[dict[str, ALL_DEV_TYPES], Any]]:
+    def get_all_elements_dict_by_type(self) -> dict[Callable[[], Any], Union[dict[str, ALL_DEV_TYPES], Any]]:
         """
         Get a dictionary of all elements by type
         :return:
         """
 
         data = dict()
         for key, tpe in self.device_type_name_dict.items():
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/measurement.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/profile.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/profile.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/municipality.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/municipality.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency_group.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/fuel.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/contingency.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/contingency.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/emission_gas.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/emission_gas.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/country.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/country.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/modelling_authority.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/modelling_authority.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/region.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/area.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/technology.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/zone.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investments_group.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investments_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/investment.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/investment.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,23 +28,25 @@
     def __init__(self,
                  idtag: Union[str, None] = None,
                  device_idtag: Union[str, None] = None,
                  name="Investment",
                  code='',
                  CAPEX=0.0,
                  OPEX=0.0,
+                 status: bool = True,
                  group: InvestmentsGroup = None,
                  comment: str = ""):
         """
-        Contingency
+        Investment
         :param idtag: String. Element unique identifier
         :param name: String. Contingency name
         :param code: String. Contingency code name
         :param CAPEX: Float. Capital expenditures
         :param OPEX: Float. Operating expenditures
+        :param status: If true the investment activates when applied, otherwise is deactivated
         :param group: ContingencyGroup. Contingency group
         :param comment: Comment
         """
 
         EditableDevice.__init__(self,
                                 idtag=idtag,
                                 code=code,
@@ -53,20 +55,23 @@
                                 comment=comment)
 
         # Contingency type
         self.device_idtag = device_idtag
         self.CAPEX = CAPEX
         self.OPEX = OPEX
         self._group: InvestmentsGroup = group
+        self.status: bool = status
 
         self.register(key='device_idtag', units='', tpe=str, definition='Unique ID')
         self.register(key='CAPEX', units='Me', tpe=float,
                       definition='Capital expenditures. This is the initial investment.')
         self.register(key='OPEX', units='Me', tpe=float,
                       definition='Operation expenditures. Maintenance costs among other recurrent costs.')
+        self.register(key='status', units='', tpe=bool,
+                      definition='If true the investment activates when applied, otherwise is deactivated.')
         self.register(key='group', units='', tpe=DeviceType.InvestmentsGroupDevice, definition='Investment group')
 
     @property
     def group(self) -> InvestmentsGroup:
         """
         Group of investments
         :return:
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/community.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/community.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Aggregation/branch_group.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Aggregation/branch_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_path.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_path.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_pump.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_node.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_turbine.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_turbine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_injection_template.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_injection_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Fluid/fluid_p2x.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Fluid/fluid_p2x.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/dc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/underground_line_type.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/underground_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/series_reactance.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/series_reactance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/wire.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/wire.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line_locations.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         Parse Json data
         :param data: List of lists with (latitude, longitude, altitude)
         """
         if len(data) > 0:
             values = np.array(data)
             self.set(data=values)
         else:
-            self.data = np.zeros((0, 4))
+            self.data = list()
 
     def set(self, data: np.ndarray):
         """
         Parse Json data
         :param data: List of lists with (sequence, latitude, longitude, altitude)
         """
         if data.ndim == 2:
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/sequence_line_type.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/sequence_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/overhead_line_type.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/overhead_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/switch.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/vsc.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/vsc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/upfc.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/upfc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/hvdc_line.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/hvdc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/line.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/tap_changer.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/winding.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/winding.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/branch.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer_type.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Branches/transformer3w.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Branches/transformer3w.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/static_generator.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/static_generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/external_grid.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/external_grid.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/current_injection.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/current_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/battery.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/battery.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/generator_q_curve.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/generator_q_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/controllable_shunt.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/controllable_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Injections/load.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Injections/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/graphic_location.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/graphic_location.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,53 +11,57 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from typing import Dict, List, Tuple, Union
-from GridCalEngine.Devices.Parents.editable_device import EditableDevice
+from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
 
 class GraphicLocation:
     """
     GraphicLocation
     """
 
     def __init__(self,
                  x: int = 0,
                  y: int = 0,
                  h: int = 80,
                  w: int = 80,
                  r: float = 0,
-                 poly_line: List[Tuple[int, int]] = list(),
-                 api_object: EditableDevice = None):
+                 poly_line: Union[None, List[Tuple[int, int]]] = None,
+                 draw_labels: bool = True,
+                 api_object: ALL_DEV_TYPES = None):
         """
         GraphicLocation
         :param x: x position (px)
         :param y: y position (px)
         :param h: height (px)
         :param w: width (px)
         :param r: rotation (deg)
         :param poly_line: List of poits to represent a polyline, if this object is to use one
+        :param draw_labels: Draw labels?
         :param api_object: object to be linked to this representation
         """
         self.x = x
         self.y = y
         self.h = h
         self.w = w
         self.r = r
-        self.poly_line = poly_line
+        self.poly_line = list() if poly_line is None else poly_line
+        self.draw_labels = draw_labels
         self.api_object = api_object
 
     def get_properties_dict(self) -> Dict[str, Union[int, str]]:
         """
         get as a dictionary point
         :return:
         """
         return {'x': self.x,
                 'y': self.y,
                 'h': self.h,
                 'w': self.w,
                 'r': self.r,
                 'poly_line': self.poly_line,
+                'draw_labels': self.draw_labels,
                 'api_object': self.api_object.idtag if self.api_object else ''}
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_diagram.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/map_location.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/map_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/schematic_diagram.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/schematic_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Diagrams/base_diagram.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Diagrams/base_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         :return:
         """
         points = {idtag: location.get_properties_dict() for idtag, location in self.locations.items()}
 
         return points
 
     def parse_data(self,
-                   data: Dict[str, Dict[str, Union[int, float, List[Tuple[float, float]]]]],
+                   data: Dict[str, Dict[str, Union[int, float, bool, List[Tuple[float, float]]]]],
                    obj_dict: Dict[str, ALL_DEV_TYPES],
                    logger: Logger,
                    category: str = "") -> None:
         """
         Parse file data ito this class
         :param data: json dictionary
         :param obj_dict: dicrtionary of relevant objects (idtag, object)
@@ -107,14 +107,15 @@
             else:
                 if 'x' in location:
                     self.locations[idtag] = GraphicLocation(x=location['x'],
                                                             y=location['y'],
                                                             w=location['w'],
                                                             h=location['h'],
                                                             r=location['r'],
+                                                            draw_labels=location.get('draw_labels', True),
                                                             api_object=api_object)
                 if 'latitude' in location:
                     self.locations[idtag] = MapLocation(latitude=location['latitude'],
                                                         longitude=location['longitude'],
                                                         altitude=location['altitude'],
                                                         api_object=api_object)
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/connectivity_node.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/voltage_level.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/bus.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/busbar.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Substation/substation.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Substation/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/injection_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/injection_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/editable_device.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/editable_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/generator_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/generator_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/controllable_branch_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/controllable_branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/load_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/load_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/branch_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Parents/shunt_parent.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Parents/shunt_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_emission.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_emission.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_technology.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Devices/Associations/generator_fuel.py` & `GridCalEngine-5.1.6/GridCalEngine/Devices/Associations/generator_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/load_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/load_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/bus_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/bus_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/branch_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/branch_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_turbine_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_turbine_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_p2x_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_p2x_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/numerical_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/numerical_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/generator_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/generator_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_pump_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_pump_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/battery_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/battery_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_path_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_path_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/hvdc_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/hvdc_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/shunt_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/shunt_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/DataStructures/fluid_node_data.py` & `GridCalEngine-5.1.6/GridCalEngine/DataStructures/fluid_node_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_newton_pa.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_newton_pa.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_bentayga.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_bentayga.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_data.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_optimods.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_optimods.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Compilers/circuit_to_pgm.py` & `GridCalEngine-5.1.6/GridCalEngine/Compilers/circuit_to_pgm.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/results_template.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/results_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/results_table.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/results_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_types.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/driver_template.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/driver_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_reduction_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_reduction_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/topology_processor_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/topology_processor_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Topology/node_groups_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Topology/node_groups_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/reliability_iterable.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/reliability_iterable.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/blackout_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/blackout_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/grid_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/grid_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Dynamics/dynamic_modules.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Dynamics/dynamic_modules.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_opf.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_opf.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/NTC/ntc_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/NTC/ntc_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -390,30 +390,32 @@
             condlist=[(df["Contingency"] == "Base"),
                       (df["Contingency"] != "Base") & (df["SRAP availability"] == "SRAP applicable"),
                       (df["Contingency"] != "Base") & (df["SRAP availability"] != "SRAP applicable")],
             choicelist=[df["Base loading (pu)"], df["Post-SRAP loading (pu)"], df["Post-Contingency loading (pu)"]],
             default=-999999
         )
 
-        df["Overload for reporting weighted with cluster"] = df["Overload for reporting"]*df["Probability cluster"]
+        df["Overload for reporting weighted with cluster"] = df["Overload for reporting"] * df["Probability cluster"]
 
         # Count the number of Hours the monitored line appears
 
         df_ = df[["Time idx", "Monitored", "Probability cluster"]].drop_duplicates()
         df_monit_time_pu = pd.pivot_table(df_, values='Probability cluster', index="Monitored", aggfunc="sum")
         df_monit_time_clust = pd.pivot_table(df_, values='Probability cluster', index="Monitored", aggfunc="count")
 
-        df['Time this line is monitored by any contingency (pu)'] = df['Monitored'].map(df_monit_time_pu['Probability cluster'])
-        df['Number of clusters this line is monitored'] = df['Monitored'].map(df_monit_time_clust['Probability cluster'])
-
+        df['Time this line is monitored by any contingency (pu)'] = df['Monitored'].map(
+            df_monit_time_pu['Probability cluster'])
+        df['Number of clusters this line is monitored'] = df['Monitored'].map(
+            df_monit_time_clust['Probability cluster'])
 
         # Group de columns by Area1, Area2, Monitored, Contingency
         df_grp = df.groupby(
             ["Area 1", "Area 2", "Monitored", "Contingency", "Base rating (MW)", "Contingency rating (MW)",
-             "SRAP rating (MW)","Time this line is monitored by any contingency (pu)","Number of clusters this line is monitored"])
+             "SRAP rating (MW)", "Time this line is monitored by any contingency (pu)",
+             "Number of clusters this line is monitored"])
 
         # Compute the columns
         ov_max = df_grp["Overload for reporting"].max()
         ov_max_date = df.loc[df_grp["Overload for reporting"].idxmax(), "Time idx"]
         ov_avg = df_grp["Overload for reporting"].mean()
 
         ov_desvest = df_grp["Overload for reporting"].std()
@@ -424,31 +426,31 @@
         ov_time_pu = df_grp["Probability cluster"].sum()
 
         if time_array is not None:
             ov_max_dates = [time_array[t].strftime(time_format) for t in ov_max_date.values]
         else:
             ov_max_dates = ov_max_date.values
 
-        #new, work in progress
-        ov_avg_clust = df_grp["Overload for reporting weighted with cluster"].sum()/df_grp["Probability cluster"].sum() #checked
-        ov_desvest_clust = df_grp["Overload for reporting weighted with cluster"].std()/df_grp["Probability cluster"].sum()
-
+        # new, work in progress
+        ov_avg_clust = df_grp["Overload for reporting weighted with cluster"].sum() / df_grp[
+            "Probability cluster"].sum()  # checked
+        ov_desvest_clust = df_grp["Overload for reporting weighted with cluster"].std() / df_grp[
+            "Probability cluster"].sum()
 
         # Create the new dataframe with the columns we need
         df_summary = pd.DataFrame({
             "Area 1": ov_max.index.get_level_values("Area 1"),
             "Area 2": ov_max.index.get_level_values("Area 2"),
             "Monitored": ov_max.index.get_level_values("Monitored"),
             "Contingency": ov_max.index.get_level_values("Contingency"),
 
-            "Area 1": ov_max.index.get_level_values("Area 1"),
-            "Area 2": ov_max.index.get_level_values("Area 2"),
-
-            "Monitored": ov_max.index.get_level_values("Monitored"),
-            "Contingency": ov_max.index.get_level_values("Contingency"),
+            # "Area 1": ov_max.index.get_level_values("Area 1"),
+            # "Area 2": ov_max.index.get_level_values("Area 2"),
+            # "Monitored": ov_max.index.get_level_values("Monitored"),
+            # "Contingency": ov_max.index.get_level_values("Contingency"),
 
             "Base rating (MW)": ov_max.index.get_level_values("Base rating (MW)"),
             "Contingency rating (MW)": ov_max.index.get_level_values("Contingency rating (MW)"),
             "SRAP rating (MW)": ov_max.index.get_level_values("SRAP rating (MW)"),
 
             "Overload max (pu)": ov_max.values,
             "Date Overload max": ov_max_dates,
@@ -465,19 +467,22 @@
             "Standard deviation for clusters(pu)": ov_desvest.values,
             "Number of clusters with this overload (h)": ov_count_clusters.values.astype(int)
 
         })
 
         df_summary = df_summary.sort_values(by="Contingency", ascending=False)
 
-        cols_1dec = ["Number of clusters this line is monitored","Number of clusters with this overload (h)"]
-        cols_2dec = ["Base rating (MW)","Contingency rating (MW)","SRAP rating (MW)"]
-        cols_4dec = ["Overload max (pu)","Overload average weighting time (pu)","Annual time the Monitored line is overloaded by this contingency (pu)","Time this line is monitored by any contingency (pu)","Overload average for clusters(pu)","Standard deviation for clusters(pu)"]
+        cols_1dec = ["Number of clusters this line is monitored", "Number of clusters with this overload (h)"]
+        cols_2dec = ["Base rating (MW)", "Contingency rating (MW)", "SRAP rating (MW)"]
+        cols_4dec = ["Overload max (pu)", "Overload average weighting time (pu)",
+                     "Annual time the Monitored line is overloaded by this contingency (pu)",
+                     "Time this line is monitored by any contingency (pu)", "Overload average for clusters(pu)",
+                     "Standard deviation for clusters(pu)"]
 
-        df_summary[cols_1dec]=df_summary[cols_1dec].map(lambda x:f'{x:.1f}')
+        df_summary[cols_1dec] = df_summary[cols_1dec].map(lambda x: f'{x:.1f}')
         df_summary[cols_2dec] = df_summary[cols_2dec].map(lambda x: f'{x:.2f}')
         df_summary[cols_4dec] = df_summary[cols_4dec].map(lambda x: f'{x:.4f}')
 
         return df_summary
 
     def __iadd__(self, other: "ContingencyResultsReport"):
         """
@@ -546,21 +551,27 @@
         :param detailed_massive_report: Generate massive report
         """
 
         # Reporting base case
         if contingency_idx == 0:  # only doing it once per hour
 
             for m in mon_idx:
+                if len(area_names):
+                    area_from = area_names[bus_area_indices[F[m]]]
+                    area_to = area_names[bus_area_indices[T[m]]]
+                else:
+                    area_from = ""
+                    area_to = ""
 
                 if abs(base_flow[m]) > numerical_circuit.rates[m]:  # only add if overloaded
 
                     self.add(time_index=t if t is not None else 0,
-                             t_prob = t_prob,
-                             area_from=area_names[bus_area_indices[F[m]]],
-                             area_to=area_names[bus_area_indices[T[m]]],
+                             t_prob=t_prob,
+                             area_from=area_from,
+                             area_to=area_to,
                              base_name=numerical_circuit.branch_data.names[m],
                              contingency_name='Base',
                              base_rating=numerical_circuit.branch_data.rates[m],
                              contingency_rating=numerical_circuit.branch_data.contingency_rates[m],
                              srap_rating=srap_ratings[m],
                              base_flow=abs(base_flow[m]),
                              post_contingency_flow=0.0,
@@ -572,14 +583,21 @@
                              msg_srap='SRAP not applicable',
                              srap_power=0.0,
                              solved_by_srap=False)
 
         # Now evalueting the effect of contingencies
         for m in mon_idx:  # for each monitored branch ...
 
+            if len(area_names):
+                area_from = area_names[bus_area_indices[F[m]]]
+                area_to = area_names[bus_area_indices[T[m]]]
+            else:
+                area_from = ""
+                area_to = ""
+
             c_flow = abs(contingency_flows[m])
             b_flow = abs(base_flow[m])
 
             c_load = abs(contingency_loadings[m])
 
             rate_nx_pu = numerical_circuit.contingency_rates[m] / (numerical_circuit.rates[m] + 1e-9)
             rate_srap_pu = srap_ratings[m] / (numerical_circuit.rates[m] + 1e-9)
@@ -677,16 +695,16 @@
                         msg_ov = 'Overload acceptable'
                     else:
                         msg_ov = 'Overload not acceptable'
 
                 if detailed_massive_report:
                     self.add(time_index=t if t is not None else 0,
                              t_prob=t_prob,
-                             area_from=area_names[bus_area_indices[F[m]]],
-                             area_to=area_names[bus_area_indices[T[m]]],
+                             area_from=area_from,
+                             area_to=area_to,
                              base_name=numerical_circuit.branch_data.names[m],
                              contingency_name=contingency_group.name,
                              base_rating=numerical_circuit.branch_data.rates[m],
                              contingency_rating=numerical_circuit.branch_data.contingency_rates[m],
                              srap_rating=srap_ratings[m],
                              base_flow=abs(b_flow),
                              post_contingency_flow=abs(c_flow),
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/Clustering/clustering_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/Clustering/clustering_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/StateEstimation/state_estimation.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/StateEstimation/state_estimation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,21 @@
         n = len(groups)
         i = 1
         energy_0: Union[Vec, None] = None  # at the beginning
 
         while i < n and not self.__cancel__:
             start_ = groups[i - 1]
             end_ = groups[i]
-            time_indices = np.arange(start_, end_)
+
+            # Grab the last time index in the last group
+            if i == n - 1:
+                time_indices = np.arange(start_, end_ + 1)
+            else:
+                time_indices = np.arange(start_, end_)
+
             # show progress message
             print(start_, ':', end_, ' [', end_ - start_, ']')
             self.report_text('Running OPF for the time group {0} '
                              'start {1} - end {2} in external solver...'.format(i, start_, end_))
 
             # run an opf for the group interval only if the group is within the start:end boundaries
             # DC optimal power flow
```

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_ts_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/linear_opf_ts.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/linear_opf_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/opf_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/opf_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/__init__.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py` & `GridCalEngine-5.1.6/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/setup.py` & `GridCalEngine-5.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.5/PKG-INFO` & `GridCalEngine-5.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCalEngine
-Version: 5.1.5
+Version: 5.1.6
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

