# Comparing `tmp/GridCal-5.1.5.tar.gz` & `tmp/GridCal-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCal-5.1.5.tar", last modified: Thu Apr 11 17:55:34 2024, max compression
+gzip compressed data, was "GridCal-5.1.6.tar", last modified: Sat Apr 13 14:14:26 2024, max compression
```

## Comparing `GridCal-5.1.5.tar` & `GridCal-5.1.6.tar`

### file list

```diff
@@ -1,227 +1,227 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-11 15:31:05.578472 GridCal-5.1.5/GridCal/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/ExecuteGridCal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.5/GridCal/update.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/templates.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.5/GridCal/Session/results_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/export_results_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/session.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/synchronization_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Session/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.5/GridCal/Session/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.5/GridCal/data/cables.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.5/GridCal/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-11 15:31:05.578472 GridCal-5.1.5/GridCal/data/sequence_lines.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.5/GridCal/data/transformers.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.5/GridCal/data/wires.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.5/GridCal/Gui/GeneralDialogues.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/update_gui_all.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/messages.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/themes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.5/GridCal/Gui/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    85064 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/GuiFunctions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/plot_config.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/update_gui_common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/Widgets/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Widgets/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/Widgets/custom_qrangeslider.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/TowerBuilder/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/TowerBuilder/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/Gui/TowerBuilder/table_models.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TowerBuilder/test_.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/TowerBuilder/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/TowerBuilder/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/graphics_manager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.5/GridCal/Gui/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/diagrams_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   186520 2024-04-11 16:03:35.834534 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6687 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6203 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16999 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13480 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4212 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12258 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4852 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9421 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-11 15:31:05.570472 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4683 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32907 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30218 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21562 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30410 2024-04-08 13:34:15.959164 GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   160182 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/node_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20956 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4966 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2159 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4975 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1917 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/AboutDialogue/about_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.5/GridCal/Gui/AboutDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.5/GridCal/Gui/AboutDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.5/GridCal/Gui/AboutDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/AboutDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_dialog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.5/GridCal/Gui/ProfilesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/ProfilesInput/models_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profile_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.5/GridCal/Gui/Analysis/AnalysisDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/Analysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.5/GridCal/Gui/Analysis/object_plot_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/CascadingSteps/cascading_steps.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.5/GridCal/Gui/CascadingSteps/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.5/GridCal/Gui/Main/ConsoleLogController.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.5/GridCal/Gui/Main/GridCalMain.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   277012 2024-04-11 17:39:50.574328 GridCal-5.1.5/GridCal/Gui/Main/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.5/GridCal/Gui/Main/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-11 17:39:50.802328 GridCal-5.1.5/GridCal/Gui/Main/ConsoleLog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   762396 2024-04-11 17:39:50.342328 GridCal-5.1.5/GridCal/Gui/Main/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Main/object_select_window.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/README.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/simulations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33887 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/io.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/base_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17930 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/configuration.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45640 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/objects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21114 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/time_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    71734 2024-04-11 15:31:05.574472 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/diagrams.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/Visualization/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Visualization/visualization.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/Visualization/palettes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SyncDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SyncDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SyncDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/SyncDialogue/sync_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SyncDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/RosetaExplorer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/LoadDesigner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/WindPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.5/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.5/GridCal/Gui/GridGenerator/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.5/GridCal/Gui/GridGenerator/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.5/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/GridGenerator/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.5/GridCal/Gui/GridGenerator/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4923 2024-04-11 17:44:56.522321 GridCal-5.1.5/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-11 17:55:34.142307 GridCal-5.1.5/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-11 17:55:34.142307 GridCal-5.1.5/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-12 12:41:14.151810 GridCal-5.1.6/GridCal/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/ExecuteGridCal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.6/GridCal/update.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/templates.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.6/GridCal/Session/results_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/export_results_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/session.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/synchronization_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.6/GridCal/Session/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.6/GridCal/data/cables.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.6/GridCal/data/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-11 15:31:05.578472 GridCal-5.1.6/GridCal/data/sequence_lines.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.6/GridCal/data/transformers.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.6/GridCal/data/wires.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.6/GridCal/Gui/GeneralDialogues.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/update_gui_all.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/messages.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/themes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.6/GridCal/Gui/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    85249 2024-04-12 16:08:47.131984 GridCal-5.1.6/GridCal/Gui/GuiFunctions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/plot_config.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/update_gui_common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/Widgets/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Widgets/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/Widgets/custom_qrangeslider.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/TowerBuilder/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/TowerBuilder/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/Gui/TowerBuilder/table_models.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TowerBuilder/test_.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/TowerBuilder/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/TowerBuilder/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/graphics_manager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.6/GridCal/Gui/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/diagrams_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   198492 2024-04-12 14:20:56.563894 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7195 2024-04-12 14:37:07.823907 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6253 2024-04-12 14:15:42.503889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17195 2024-04-12 14:15:42.515889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13617 2024-04-12 14:15:42.539889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-04-12 14:20:56.579894 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12367 2024-04-12 14:15:42.579889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4961 2024-04-12 14:15:42.475889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4480 2024-04-12 14:15:42.547889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9547 2024-04-12 14:15:42.571889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-11 15:31:05.570472 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4792 2024-04-12 14:15:42.555889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-12 14:04:34.963880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32985 2024-04-12 14:15:42.563889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30364 2024-04-12 14:04:34.939880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21549 2024-04-12 14:04:34.795880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30526 2024-04-12 14:15:42.495889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   160182 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/node_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21089 2024-04-12 14:39:32.843909 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4966 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2159 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4975 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1917 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/AboutDialogue/about_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.6/GridCal/Gui/AboutDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.6/GridCal/Gui/AboutDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.6/GridCal/Gui/AboutDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/AboutDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_dialog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.6/GridCal/Gui/ProfilesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/ProfilesInput/models_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profile_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/Analysis/AnalysisDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.6/GridCal/Gui/Analysis/object_plot_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/CascadingSteps/cascading_steps.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.6/GridCal/Gui/Main/ConsoleLogController.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.6/GridCal/Gui/Main/GridCalMain.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   276874 2024-04-12 06:51:51.955518 GridCal-5.1.6/GridCal/Gui/Main/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/Main/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-12 06:51:51.955518 GridCal-5.1.6/GridCal/Gui/Main/ConsoleLog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   807433 2024-04-12 06:51:51.959518 GridCal-5.1.6/GridCal/Gui/Main/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Main/object_select_window.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/README.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/simulations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33887 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/io.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/base_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17930 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/configuration.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45640 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/objects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21114 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/time_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    72028 2024-04-12 10:06:43.207681 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/diagrams.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/Visualization/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Visualization/visualization.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Visualization/palettes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SyncDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SyncDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SyncDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/SyncDialogue/sync_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SyncDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/LoadDesigner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/GridGenerator/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.6/GridCal/Gui/GridGenerator/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/GridGenerator/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/GridGenerator/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4923 2024-04-11 18:07:34.878291 GridCal-5.1.6/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-13 14:14:26.922700 GridCal-5.1.6/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-13 14:14:26.922700 GridCal-5.1.6/setup.cfg
```

### Comparing `GridCal-5.1.5/GridCal/__version__.py` & `GridCal-5.1.6/GridCal/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCal_VERSION__ = "5.1.5"
+__GridCal_VERSION__ = "5.1.6"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCal_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCal-5.1.5/GridCal/__init__.py` & `GridCal-5.1.6/GridCal/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/ExecuteGridCal.py` & `GridCal-5.1.6/GridCal/ExecuteGridCal.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/LICENSE.txt` & `GridCal-5.1.6/GridCal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/update.py` & `GridCal-5.1.6/GridCal/update.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/templates.py` & `GridCal-5.1.6/GridCal/templates.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Session/results_model.py` & `GridCal-5.1.6/GridCal/Session/results_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Session/export_results_driver.py` & `GridCal-5.1.6/GridCal/Session/export_results_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Session/session.py` & `GridCal-5.1.6/GridCal/Session/session.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Session/synchronization_driver.py` & `GridCal-5.1.6/GridCal/Session/synchronization_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Session/file_handler.py` & `GridCal-5.1.6/GridCal/Session/file_handler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/data/cables.csv` & `GridCal-5.1.6/GridCal/data/cables.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/data/transformers.csv` & `GridCal-5.1.6/GridCal/data/transformers.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/data/wires.csv` & `GridCal-5.1.6/GridCal/data/wires.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/GeneralDialogues.py` & `GridCal-5.1.6/GridCal/Gui/GeneralDialogues.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/update_gui_all.py` & `GridCal-5.1.6/GridCal/Gui/update_gui_all.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/messages.py` & `GridCal-5.1.6/GridCal/Gui/messages.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/themes.py` & `GridCal-5.1.6/GridCal/Gui/themes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ConsoleWidget.py` & `GridCal-5.1.6/GridCal/Gui/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/GuiFunctions.py` & `GridCal-5.1.6/GridCal/Gui/GuiFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1349,26 +1349,26 @@
             attr_idx = index.column()
 
         if self.editable and self.attributes[attr_idx] not in self.non_editable_attributes:
             return QtCore.Qt.ItemFlag.ItemIsEditable | QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
         else:
             return QtCore.Qt.ItemFlag.ItemIsEnabled
 
-    def rowCount(self, parent=None):
+    def rowCount(self, parent: QtCore.QModelIndex = None) -> int:
         """
         Get number of rows
         :param parent:
         :return:
         """
         if self.transposed:
             return self.c
         else:
             return self.r
 
-    def columnCount(self, parent=None):
+    def columnCount(self, parent: QtCore.QModelIndex = None) -> int:
         """
         Get number of columns
         :param parent:
         :return:
         """
         if self.transposed:
             return self.r
@@ -1431,15 +1431,15 @@
                 return str(self.data_with_type(index))
             elif role == QtCore.Qt.ItemDataRole.BackgroundRole:
                 if 'color' in self.attributes[index.column()]:
                     return QtGui.QColor(str(self.data_with_type(index)))
 
         return None
 
-    def setData(self, index, value, role=None):
+    def setData(self, index: QtCore.QModelIndex, value: Union[float, str], role: Union[int, None] = None) -> bool:
         """
         Set data by simple editor (whatever text)
         :param index:
         :param value:
         :param role:
         :return:
         """
@@ -1505,15 +1505,15 @@
             return None
 
         if role == QtCore.Qt.ItemDataRole.DisplayRole:
 
             if self.transposed:
                 # for the properties in the schematic view
                 if orientation == QtCore.Qt.Orientation.Horizontal:
-                    return 'Value'
+                    return self.objects[0].device_type.value if len(self.objects) else 'Value'
                 elif orientation == QtCore.Qt.Orientation.Vertical:
                     if self.units[section] != '':
                         return self.attributes[section] + ' [' + self.units[section] + ']'
                     else:
                         return self.attributes[section]
             else:
                 # Normal
```

### Comparing `GridCal-5.1.5/GridCal/Gui/plot_config.py` & `GridCal-5.1.6/GridCal/Gui/plot_config.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/update_gui_common.py` & `GridCal-5.1.6/GridCal/Gui/update_gui_common.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Widgets/matplotlibwidget.py` & `GridCal-5.1.6/GridCal/Gui/Widgets/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Widgets/custom_qrangeslider.py` & `GridCal-5.1.6/GridCal/Gui/Widgets/custom_qrangeslider.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ContingencyPlanner/gui.py` & `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/gui.py` & `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TowerBuilder/table_models.py` & `GridCal-5.1.6/GridCal/Gui/TowerBuilder/table_models.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TowerBuilder/test_.py` & `GridCal-5.1.6/GridCal/Gui/TowerBuilder/test_.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TowerBuilder/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/TowerBuilder/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TowerBuilder/gui.py` & `GridCal-5.1.6/GridCal/Gui/TowerBuilder/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py` & `GridCal-5.1.6/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/graphics_manager.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/graphics_manager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/diagrams_model.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/diagrams_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from PySide6.QtCore import (Qt, QPoint, QSize, QPointF, QRect, QRectF, QMimeData, QIODevice, QByteArray,
                             QDataStream, QModelIndex)
 from PySide6.QtGui import (QIcon, QPixmap, QImage, QPainter, QStandardItemModel, QStandardItem, QColor, QPen,
                            QDragEnterEvent, QDragMoveEvent, QDropEvent, QWheelEvent, QKeyEvent, QMouseEvent,
                            QContextMenuEvent)
 from PySide6.QtWidgets import (QGraphicsView, QListView, QTableView, QVBoxLayout, QHBoxLayout, QFrame,
                                QSplitter, QMessageBox, QAbstractItemView, QGraphicsScene, QGraphicsSceneMouseEvent,
-                               QGraphicsItem, QGraphicsTextItem, QMenu, QWidget)
+                               QGraphicsItem)
 from PySide6.QtSvg import QSvgGenerator
 
 from GridCalEngine.Devices.types import ALL_DEV_TYPES, INJECTION_DEVICE_TYPES, FLUID_TYPES
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Devices.Substation.bus import Bus
 from GridCalEngine.Devices.Substation.substation import Substation
 from GridCalEngine.Devices.Substation.voltage_level import VoltageLevel
@@ -80,15 +80,15 @@
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.generic_graphics import ACTIVE
 from GridCal.Gui.GeneralDialogues import InputNumberDialogue
 import GridCal.Gui.Visualization.visualization as viz
 import GridCal.Gui.Visualization.palettes as palettes
-from GridCal.Gui.GuiFunctions import ObjectsModel, add_menu_entry
+from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import info_msg, error_msg, warning_msg, yes_no_question
 from matplotlib import pyplot as plt
 
 BRANCH_GRAPHICS = Union[
     LineGraphicItem,
     WindingGraphicItem,
     DcLineGraphicItem,
@@ -446,28 +446,28 @@
         #                icon_path=":/Icons/icons/bus_icon.svg",
         #                function_ptr=lambda x: self.parent_.clear_big_bus_markers())
         #
         # # launch the menu
         # context_menu.exec(event.globalPos())
 
 
-def find_my_node(idtag_: str,
-                 bus_dict: Dict[str, BusGraphicItem],
-                 fluid_node_dict: Dict[str, FluidNodeGraphicItem]):
-    """
-    Function to look for the bus or fluid node
-    :param idtag_: bus or fluidnode idtag
-    :param bus_dict:
-    :param fluid_node_dict:
-    :return: Matching graphic object
-    """
-    graphic_obj = bus_dict.get(idtag_, None)
-    if graphic_obj is None:
-        graphic_obj = fluid_node_dict.get(idtag_, None)
-    return graphic_obj
+# def find_my_node(idtag_: str,
+#                  bus_dict: Dict[str, BusGraphicItem],
+#                  fluid_node_dict: Dict[str, FluidNodeGraphicItem]):
+#     """
+#     Function to look for the bus or fluid node
+#     :param idtag_: bus or fluidnode idtag
+#     :param bus_dict:
+#     :param fluid_node_dict:
+#     :return: Matching graphic object
+#     """
+#     graphic_obj = bus_dict.get(idtag_, None)
+#     if graphic_obj is None:
+#         graphic_obj = fluid_node_dict.get(idtag_, None)
+#     return graphic_obj
 
 
 class DiagramEditorWidget(QSplitter):
     """
     DiagramEditorWidget
     This is the bus-branch editor
     """
@@ -678,14 +678,15 @@
             # add to the diagram list
             self.update_diagram_element(device=obj,
                                         x=x0,
                                         y=y0,
                                         w=graphic_object.w,
                                         h=graphic_object.h,
                                         r=0,
+                                        draw_labels=graphic_object.draw_labels,
                                         graphic_object=graphic_object)
 
     def graphicsWheelEvent(self, event: QWheelEvent) -> None:
         """
         Zoom
         @param event:
         @return:
@@ -722,57 +723,63 @@
     def zoom_out(self, scale_factor: float = 1.15) -> None:
         """
 
         :param scale_factor:
         """
         self.editor_graphics_view.scale(1.0 / scale_factor, 1.0 / scale_factor)
 
-    def create_bus_graphics(self, bus: Bus, x: int, y: int, h: int, w: int) -> BusGraphicItem:
+    def create_bus_graphics(self, bus: Bus, x: int, y: int, h: int, w: int,
+                            draw_labels: bool = True) -> BusGraphicItem:
         """
         create the Bus graphics
         :param bus: GridCal Bus object
         :param x: x coordinate
         :param y: y coordinate
         :param h: height (px)
         :param w: width (px)
+        :param draw_labels: Draw labels?
         :return: BusGraphicItem
         """
 
         graphic_object = BusGraphicItem(editor=self,
                                         bus=bus,
                                         x=x,
                                         y=y,
                                         h=h,
-                                        w=w)
+                                        w=w,
+                                        draw_labels=draw_labels)
         return graphic_object
 
     def create_transformer_3w_graphics(self, elm: Transformer3W, x: int, y: int) -> Transformer3WGraphicItem:
         """
         Add Transformer3W to the graphics
         :param elm: Transformer3W
         :param x: x coordinate
         :param y: y coordinate
         :return: Transformer3WGraphicItem
         """
         graphic_object = Transformer3WGraphicItem(editor=self, elm=elm)
         graphic_object.setPos(QPoint(x, y))
         return graphic_object
 
-    def create_fluid_node_graphics(self, node: FluidNode, x: int, y: int, h: int, w: int) -> FluidNodeGraphicItem:
+    def create_fluid_node_graphics(self, node: FluidNode, x: int, y: int, h: int, w: int,
+                                   draw_labels: bool = True) -> FluidNodeGraphicItem:
         """
         Add fluid node to graphics
         :param node: GridCal FluidNode object
         :param x: x coordinate
         :param y: y coordinate
         :param h: height (px)
         :param w: width (px)
+        :param draw_labels: Draw labels?
         :return: FluidNodeGraphicItem
         """
 
-        graphic_object = FluidNodeGraphicItem(editor=self, fluid_node=node, x=x, y=y, h=h, w=w)
+        graphic_object = FluidNodeGraphicItem(editor=self, fluid_node=node, x=x, y=y, h=h, w=w,
+                                              draw_labels=draw_labels)
         return graphic_object
 
     def create_connectivity_node_graphics(self, node: ConnectivityNode, x: int, y: int, h: int,
                                           w: int) -> CnGraphicItem:
         """
         Add connectivity node to graphics
         :param node: GridCal connectivity node object
@@ -807,275 +814,384 @@
         :param diagram: SchematicDiagram
         """
         self.clear()
         self.circuit = circuit
         self.diagram = diagram
         self.draw()
 
-    def draw(self) -> None:
+    def draw_additional_diagram(self, diagram: SchematicDiagram) -> None:
         """
-        Draw diagram
-        :return:
+        Draw a new diagram
+        :param diagram: SchematicDiagram
         """
         inj_dev_by_bus = self.circuit.get_injection_devices_grouped_by_bus()
         inj_dev_by_fluid_node = self.circuit.get_injection_devices_grouped_by_fluid_node()
 
         # add buses first
-        bus_dict: Dict[str, BusGraphicItem] = dict()
-        fluid_node_dict: Dict[str, FluidNodeGraphicItem] = dict()
-        windings_dict: Dict[str, WindingGraphicItem] = dict()
-        for category, points_group in self.diagram.data.items():
+        for category, points_group in diagram.data.items():
 
             if category == DeviceType.BusDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    # add the graphic object to the diagram view
-                    graphic_object = self.create_bus_graphics(bus=location.api_object,
-                                                              x=location.x,
-                                                              y=location.y,
-                                                              h=location.h,
-                                                              w=location.w)
-                    self.add_to_scene(graphic_object=graphic_object)
-
-                    # create the bus children
-                    graphic_object.create_children_widgets(
-                        injections_by_tpe=inj_dev_by_bus.get(location.api_object, dict())
-                    )
-
-                    graphic_object.change_size(w=location.w)
-
-                    # add buses reference for later
-                    bus_dict[idtag] = graphic_object
-                    self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+                        # add the graphic object to the diagram view
+                        graphic_object = self.create_bus_graphics(bus=location.api_object,
+                                                                  x=location.x,
+                                                                  y=location.y,
+                                                                  h=location.h,
+                                                                  w=location.w,
+                                                                  draw_labels=location.draw_labels)
+                        self.add_to_scene(graphic_object=graphic_object)
+
+                        # create the bus children
+                        graphic_object.create_children_widgets(
+                            injections_by_tpe=inj_dev_by_bus.get(location.api_object, dict())
+                        )
+
+                        graphic_object.change_size(w=location.w)
+
+                        # add buses reference for later
+                        # bus_dict[idtag] = graphic_object
+                        self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.Transformer3WDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    elm: Transformer3W = location.api_object
 
-                    graphic_object = self.create_transformer_3w_graphics(elm=elm,
-                                                                         x=location.x,
-                                                                         y=location.y)
-                    self.add_to_scene(graphic_object=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+                        elm: Transformer3W = location.api_object
 
-                    bus_1_graphic = bus_dict[elm.bus1.idtag]
-                    bus_2_graphic = bus_dict[elm.bus2.idtag]
-                    bus_3_graphic = bus_dict[elm.bus3.idtag]
-
-                    conn1 = WindingGraphicItem(from_port=graphic_object.terminals[0],
-                                               to_port=bus_1_graphic.get_terminal(),
-                                               editor=self)
-
-                    graphic_object.set_connection(i=0, bus=elm.bus1, conn=conn1)
-
-                    conn2 = WindingGraphicItem(from_port=graphic_object.terminals[1],
-                                               to_port=bus_2_graphic.get_terminal(),
-                                               editor=self)
-                    graphic_object.set_connection(i=1, bus=elm.bus2, conn=conn2)
-
-                    conn3 = WindingGraphicItem(from_port=graphic_object.terminals[2],
-                                               to_port=bus_3_graphic.get_terminal(),
-                                               editor=self)
-                    graphic_object.set_connection(i=2, bus=elm.bus3, conn=conn3)
-
-                    graphic_object.set_position(x=location.x, y=location.y)
-                    graphic_object.change_size(h=location.h, w=location.w)
-
-                    self.add_to_scene(graphic_object=conn1)
-                    self.add_to_scene(graphic_object=conn2)
-                    self.add_to_scene(graphic_object=conn3)
-
-                    graphic_object.update_conn()
-                    self.graphics_manager.add_device(elm=elm, graphic=graphic_object)
-                    self.graphics_manager.add_device(elm=elm.winding1, graphic=conn1)
-                    self.graphics_manager.add_device(elm=elm.winding2, graphic=conn2)
-                    self.graphics_manager.add_device(elm=elm.winding3, graphic=conn3)
-
-                    # register the windings for the branches pass
-                    windings_dict[elm.winding1.idtag] = conn1
-                    windings_dict[elm.winding2.idtag] = conn2
-                    windings_dict[elm.winding3.idtag] = conn3
+                        graphic_object = self.create_transformer_3w_graphics(elm=elm,
+                                                                             x=location.x,
+                                                                             y=location.y)
+                        self.add_to_scene(graphic_object=graphic_object)
+
+                        bus_1_graphic = self.graphics_manager.query(elm.bus1)
+                        bus_2_graphic = self.graphics_manager.query(elm.bus2)
+                        bus_3_graphic = self.graphics_manager.query(elm.bus3)
+
+                        conn1 = WindingGraphicItem(from_port=graphic_object.terminals[0],
+                                                   to_port=bus_1_graphic.get_terminal(),
+                                                   editor=self)
+
+                        graphic_object.set_connection(i=0, bus=elm.bus1, conn=conn1)
+
+                        conn2 = WindingGraphicItem(from_port=graphic_object.terminals[1],
+                                                   to_port=bus_2_graphic.get_terminal(),
+                                                   editor=self)
+                        graphic_object.set_connection(i=1, bus=elm.bus2, conn=conn2)
+
+                        conn3 = WindingGraphicItem(from_port=graphic_object.terminals[2],
+                                                   to_port=bus_3_graphic.get_terminal(),
+                                                   editor=self)
+                        graphic_object.set_connection(i=2, bus=elm.bus3, conn=conn3)
+
+                        graphic_object.set_position(x=location.x, y=location.y)
+                        graphic_object.change_size(h=location.h, w=location.w)
+
+                        self.add_to_scene(graphic_object=conn1)
+                        self.add_to_scene(graphic_object=conn2)
+                        self.add_to_scene(graphic_object=conn3)
+
+                        graphic_object.update_conn()
+                        self.graphics_manager.add_device(elm=elm, graphic=graphic_object)
+                        self.graphics_manager.add_device(elm=elm.winding1, graphic=conn1)
+                        self.graphics_manager.add_device(elm=elm.winding2, graphic=conn2)
+                        self.graphics_manager.add_device(elm=elm.winding3, graphic=conn3)
+
+                        # register the windings for the branches pass
+                        # windings_dict[elm.winding1.idtag] = conn1
+                        # windings_dict[elm.winding2.idtag] = conn2
+                        # windings_dict[elm.winding3.idtag] = conn3
 
-            if category == DeviceType.FluidNodeDevice.value:
+            elif category == DeviceType.FluidNodeDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    # add the graphic object to the diagram view
-                    graphic_object = self.create_fluid_node_graphics(node=location.api_object,
-                                                                     x=location.x,
-                                                                     y=location.y,
-                                                                     h=location.h,
-                                                                     w=location.w)
-                    self.add_to_scene(graphic_object=graphic_object)
-
-                    # create the bus children
-                    graphic_object.create_children_widgets(
-                        injections_by_tpe=inj_dev_by_fluid_node.get(location.api_object, dict()))
-
-                    graphic_object.change_size(h=location.h,
-                                               w=location.w)
-
-                    # add fluid node reference for later
-                    fluid_node_dict[idtag] = graphic_object
-                    self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
-
-                    # map the internal bus
-                    # if location.api_object.bus is not None:
-                    #     bus_dict[location.api_object.bus.idtag] = graphic_object
+
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+                        # add the graphic object to the diagram view
+                        graphic_object = self.create_fluid_node_graphics(node=location.api_object,
+                                                                         x=location.x,
+                                                                         y=location.y,
+                                                                         h=location.h,
+                                                                         w=location.w,
+                                                                         draw_labels=location.draw_labels)
+                        self.add_to_scene(graphic_object=graphic_object)
+
+                        # create the bus children
+                        graphic_object.create_children_widgets(
+                            injections_by_tpe=inj_dev_by_fluid_node.get(location.api_object, dict()))
+
+                        graphic_object.change_size(h=location.h,
+                                                   w=location.w)
+
+                        # add fluid node reference for later
+                        # fluid_node_dict[idtag] = graphic_object
+                        self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                        self.graphics_manager.add_device(elm=location.api_object.bus, graphic=graphic_object)
+
+                        # map the internal bus
+                        # if location.api_object.bus is not None:
+                        #     bus_dict[location.api_object.bus.idtag] = graphic_object
 
             else:
                 # pass for now...
                 pass
 
         # add the rest of the branches
-        for category, points_group in self.diagram.data.items():
+        for category, points_group in diagram.data.items():
 
             if category == DeviceType.LineDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: Line = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = LineGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                             to_port=bus_t_graphic_obj.get_terminal(),
-                                                             editor=self,
-                                                             api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: Line = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = LineGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                 to_port=bus_t_graphic_obj.get_terminal(),
+                                                                 editor=self,
+                                                                 api_object=branch,
+                                                                 draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.DCLineDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: DcLine = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = DcLineGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                               to_port=bus_t_graphic_obj.get_terminal(),
-                                                               editor=self,
-                                                               api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: DcLine = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = DcLineGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                   to_port=bus_t_graphic_obj.get_terminal(),
+                                                                   editor=self,
+                                                                   api_object=branch,
+                                                                   draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.HVDCLineDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: HvdcLine = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = HvdcGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                             to_port=bus_t_graphic_obj.get_terminal(),
-                                                             editor=self,
-                                                             api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: HvdcLine = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = HvdcGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                 to_port=bus_t_graphic_obj.get_terminal(),
+                                                                 editor=self,
+                                                                 api_object=branch,
+                                                                 draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.VscDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: VSC = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = VscGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                            to_port=bus_t_graphic_obj.get_terminal(),
-                                                            editor=self,
-                                                            api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: VSC = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = VscGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                to_port=bus_t_graphic_obj.get_terminal(),
+                                                                editor=self,
+                                                                api_object=branch,
+                                                                draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.UpfcDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: UPFC = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = UpfcGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                             to_port=bus_t_graphic_obj.get_terminal(),
-                                                             editor=self,
-                                                             api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: UPFC = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = UpfcGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                 to_port=bus_t_graphic_obj.get_terminal(),
+                                                                 editor=self,
+                                                                 api_object=branch,
+                                                                 draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.Transformer2WDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: Transformer2W = location.api_object
-                    if branch.bus_from is not None and branch.bus_to is not None:
-                        bus_f_graphic_obj = find_my_node(branch.bus_from.idtag, bus_dict, fluid_node_dict)
-                        bus_t_graphic_obj = find_my_node(branch.bus_to.idtag, bus_dict, fluid_node_dict)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = TransformerGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                                    to_port=bus_t_graphic_obj.get_terminal(),
-                                                                    editor=self,
-                                                                    api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: Transformer2W = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = TransformerGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                        to_port=bus_t_graphic_obj.get_terminal(),
+                                                                        editor=self,
+                                                                        api_object=branch,
+                                                                        draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+
+            elif category == DeviceType.SeriesReactanceDevice.value:
+
+                for idtag, location in points_group.locations.items():
+
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: SeriesReactance = location.api_object
+                        if branch.bus_from is not None and branch.bus_to is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.bus_from)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.bus_to)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = SeriesReactanceGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                            to_port=bus_t_graphic_obj.get_terminal(),
+                                                                            editor=self,
+                                                                            api_object=branch,
+                                                                            draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.WindingDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    # branch: Winding = location.api_object
-                    graphic_object = windings_dict[idtag]
-                    graphic_object.redraw()
-                    self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is not None:
+                        graphic_object.redraw()
+                        self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             elif category == DeviceType.FluidPathDevice.value:
 
                 for idtag, location in points_group.locations.items():
-                    branch: FluidPath = location.api_object
-                    if branch.source is not None and branch.target is not None:
-                        bus_f_graphic_obj = fluid_node_dict.get(branch.source.idtag, None)
-                        bus_t_graphic_obj = fluid_node_dict.get(branch.target.idtag, None)
-
-                        if bus_f_graphic_obj and bus_t_graphic_obj:
-                            graphic_object = FluidPathGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
-                                                                  to_port=bus_t_graphic_obj.get_terminal(),
-                                                                  editor=self,
-                                                                  api_object=branch)
-                            self.add_to_scene(graphic_object=graphic_object)
 
-                            graphic_object.redraw()
-                            self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
+                    # search for the api object, because it may be created already
+                    graphic_object = self.graphics_manager.query(elm=location.api_object)
+
+                    if graphic_object is None:
+
+                        branch: FluidPath = location.api_object
+                        if branch.source is not None and branch.target is not None:
+                            bus_f_graphic_obj = self.graphics_manager.query(branch.source)
+                            bus_t_graphic_obj = self.graphics_manager.query(branch.target)
+
+                            if bus_f_graphic_obj and bus_t_graphic_obj:
+                                graphic_object = FluidPathGraphicItem(from_port=bus_f_graphic_obj.get_terminal(),
+                                                                      to_port=bus_t_graphic_obj.get_terminal(),
+                                                                      editor=self,
+                                                                      api_object=branch,
+                                                                      draw_labels=location.draw_labels)
+                                self.add_to_scene(graphic_object=graphic_object)
+
+                                graphic_object.redraw()
+                                self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
 
             else:
                 pass
                 # print('draw: Unrecognized category: {}'.format(category))
 
         # last pass: arange children
         for category in [DeviceType.BusDevice, DeviceType.FluidNodeDevice]:
             graphics_dict = self.graphics_manager.get_device_type_dict(device_type=category)
             for idtag, graphic in graphics_dict.items():
                 graphic.arrange_children()
 
+    def draw(self) -> None:
+        """
+        Draw the stored diagram
+        """
+        self.draw_additional_diagram(diagram=self.diagram)
+
+    def expand_diagram_from_bus(self, root_bus: Bus) -> None:
+        """
+        Expand the diagram from one bus
+        :param root_bus: Root bus to expand from
+        """
+        extra_diagram = make_vecinity_diagram(circuit=self.circuit,
+                                              root_bus=root_bus,
+                                              max_level=1)
+
+        self.draw_additional_diagram(diagram=extra_diagram)
+
     @property
     def name(self):
         """
         Get the diagram name
         :return:
         """
         return self.diagram.name
@@ -1087,35 +1203,49 @@
         :param val:
         :return:
         """
         self.diagram.name = val
 
     def update_diagram_element(self, device: ALL_DEV_TYPES,
                                x: int = 0, y: int = 0, w: int = 0, h: int = 0, r: float = 0,
+                               draw_labels: bool = True,
                                graphic_object: QGraphicsItem = None) -> None:
         """
         Set the position of a device in the diagram
         :param device: EditableDevice
         :param x: x position (px)
         :param y: y position (px)
         :param h: height (px)
         :param w: width (px)
         :param r: rotation (deg)
+        :param draw_labels: Draw the labels?
         :param graphic_object: Graphic object associated
         """
         self.diagram.set_point(device=device,
                                location=GraphicLocation(x=x,
                                                         y=y,
                                                         h=h,
                                                         w=w,
                                                         r=r,
+                                                        draw_labels=draw_labels,
                                                         api_object=device))
 
         self.graphics_manager.add_device(elm=device, graphic=graphic_object)
 
+    def update_label_drwaing_status(self, device: ALL_DEV_TYPES, draw_labels: bool) -> None:
+        """
+        Update the label drawing flag
+        :param device: Any database device
+        :param draw_labels: Draw labels?
+        """
+        location = self.diagram.query_point(device=device)
+
+        if location is not None:
+            location.draw_labels = draw_labels
+
     def add_to_scene(self, graphic_object: QGraphicsItem = None) -> None:
         """
         Add item to the diagram and the diagram scene
         :param graphic_object: Graphic object associated
         """
 
         self.diagram_scene.addItem(graphic_object)
@@ -1304,14 +1434,15 @@
                                          to_port=to_port,
                                          editor=self,
                                          api_object=obj)
 
         self.add_to_scene(graphic_object=graphic_object)
 
         self.update_diagram_element(device=obj,
+                                    draw_labels=graphic_object.draw_labels,
                                     graphic_object=graphic_object)
 
         # add the new object to the circuit
         self.circuit.add_branch(obj)
 
         # update the connection placement
         graphic_object.update_ports()
@@ -1336,15 +1467,17 @@
         graphic_object = DcLineGraphicItem(from_port=from_port,
                                            to_port=to_port,
                                            editor=self,
                                            api_object=obj)
 
         self.add_to_scene(graphic_object=graphic_object)
 
-        self.update_diagram_element(device=obj, graphic_object=graphic_object)
+        self.update_diagram_element(device=obj,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
         # add the new object to the circuit
         self.circuit.add_branch(obj)
 
         # update the connection placement
         graphic_object.update_ports()
 
@@ -1364,14 +1497,15 @@
                                               to_port=to_port,
                                               editor=self,
                                               api_object=api_object)
 
         self.add_to_scene(graphic_object=winding_graphics)
 
         self.update_diagram_element(device=winding_graphics.api_object,
+                                    draw_labels=winding_graphics.draw_labels,
                                     graphic_object=winding_graphics)
 
         self.started_branch.update_ports()
 
         # set the connection placement
         winding_graphics.setZValue(-1)
 
@@ -1394,15 +1528,17 @@
         graphic_object = TransformerGraphicItem(from_port=from_port,
                                                 to_port=to_port,
                                                 editor=self,
                                                 api_object=obj)
 
         self.add_to_scene(graphic_object=graphic_object)
 
-        self.update_diagram_element(device=obj, graphic_object=graphic_object)
+        self.update_diagram_element(device=obj,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
         # add the new object to the circuit
         self.circuit.add_branch(obj)
 
         # update the connection placement
         graphic_object.update_ports()
 
@@ -1426,15 +1562,17 @@
         graphic_object = VscGraphicItem(from_port=from_port,
                                         to_port=to_port,
                                         editor=self,
                                         api_object=obj)
 
         self.add_to_scene(graphic_object=graphic_object)
 
-        self.update_diagram_element(device=obj, graphic_object=graphic_object)
+        self.update_diagram_element(device=obj,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
         # add the new object to the circuit
         self.circuit.add_branch(obj)
 
         # update the connection placement
         graphic_object.update_ports()
 
@@ -1459,15 +1597,17 @@
         graphic_object = FluidPathGraphicItem(from_port=from_port,
                                               to_port=to_port,
                                               editor=self,
                                               api_object=obj)
 
         self.add_to_scene(graphic_object=graphic_object)
 
-        self.update_diagram_element(device=obj, graphic_object=graphic_object)
+        self.update_diagram_element(device=obj,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
         # update the connection placement
         graphic_object.update_ports()
 
         # set the connection placement
         graphic_object.setZValue(-1)
 
@@ -2007,14 +2147,15 @@
 
         self.update_diagram_element(device=bus,
                                     x=x,
                                     y=y,
                                     w=bus.w,
                                     h=bus.h,
                                     r=0,
+                                    draw_labels=graphic_object.draw_labels,
                                     graphic_object=graphic_object)
 
         return graphic_object
 
     def add_api_line(self, branch: Line,
                      bus_f_graphic0: Union[None, BusGraphicItem] = None,
                      bus_t_graphic0: Union[None, BusGraphicItem] = None) -> Union[None, LineGraphicItem]:
@@ -2038,15 +2179,17 @@
 
         graphic_object = LineGraphicItem(from_port=bus_f_graphic0.get_terminal(),
                                          to_port=bus_t_graphic0.get_terminal(),
                                          editor=self,
                                          api_object=branch)
 
         graphic_object.redraw()
-        self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+        self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
         return graphic_object
 
     def add_api_line_between_fluid_graphics(self, branch: Line,
                                             bus_f_graphic: FluidNodeGraphicItem,
                                             bus_t_graphic: FluidNodeGraphicItem):
         """
         add API branch to the Scene
@@ -2058,15 +2201,17 @@
 
         graphic_object = LineGraphicItem(from_port=bus_f_graphic.get_terminal(),
                                          to_port=bus_t_graphic.get_terminal(),
                                          editor=self,
                                          api_object=branch)
 
         graphic_object.redraw()
-        self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+        self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
         return graphic_object
 
     def add_api_dc_line(self, branch: DcLine):
         """
         add API branch to the Scene
         :param branch: Branch instance
         """
@@ -2077,15 +2222,17 @@
 
             graphic_object = DcLineGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                                to_port=bus_t_graphics.get_terminal(),
                                                editor=self,
                                                api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_hvdc(self, branch: HvdcLine):
         """
@@ -2099,15 +2246,17 @@
 
             graphic_object = HvdcGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                              to_port=bus_t_graphics.get_terminal(),
                                              editor=self,
                                              api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_vsc(self, branch: VSC):
         """
@@ -2121,15 +2270,17 @@
 
             graphic_object = VscGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                             to_port=bus_t_graphics.get_terminal(),
                                             editor=self,
                                             api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_upfc(self, branch: UPFC):
         """
@@ -2143,15 +2294,17 @@
 
             graphic_object = UpfcGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                              to_port=bus_t_graphics.get_terminal(),
                                              editor=self,
                                              api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_series_reactance(self, branch: SeriesReactance):
         """
@@ -2165,15 +2318,17 @@
 
             graphic_object = SeriesReactanceGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                                         to_port=bus_t_graphics.get_terminal(),
                                                         editor=self,
                                                         api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_transformer(self, branch: Transformer2W):
         """
@@ -2187,15 +2342,17 @@
 
             graphic_object = TransformerGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                                     to_port=bus_t_graphics.get_terminal(),
                                                     editor=self,
                                                     api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's buses were not found in the diagram :(")
             return None
 
     def add_api_transformer_3w(self, elm: Transformer3W):
         """
@@ -2228,14 +2385,15 @@
 
         self.update_diagram_element(device=elm,
                                     x=elm.x,
                                     y=elm.y,
                                     w=80,
                                     h=80,
                                     r=0,
+                                    draw_labels=True,
                                     graphic_object=tr3_graphic_object)
 
         self.update_diagram_element(device=conn1.api_object, graphic_object=conn1)
         self.update_diagram_element(device=conn2.api_object, graphic_object=conn2)
         self.update_diagram_element(device=conn3.api_object, graphic_object=conn3)
 
         return tr3_graphic_object
@@ -2261,14 +2419,15 @@
 
         self.update_diagram_element(device=node,
                                     x=x,
                                     y=y,
                                     w=graphic_object.w,
                                     h=graphic_object.h,
                                     r=0,
+                                    draw_labels=graphic_object.draw_labels,
                                     graphic_object=graphic_object)
 
         return graphic_object
 
     def add_api_fluid_path(self, branch: FluidPath):
         """
         add API branch to the Scene
@@ -2281,15 +2440,17 @@
 
             graphic_object = FluidPathGraphicItem(from_port=bus_f_graphics.get_terminal(),
                                                   to_port=bus_t_graphics.get_terminal(),
                                                   editor=self,
                                                   api_object=branch)
 
             graphic_object.redraw()
-            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+            self.update_diagram_element(device=branch, x=0, y=0, w=0, h=0, r=0,
+                                        draw_labels=graphic_object.draw_labels,
+                                        graphic_object=graphic_object)
             return graphic_object
         else:
             print("Branch's fluid nodes were not found in the diagram :(")
             return None
 
     def convert_line_to_hvdc(self, line: Line, line_graphic: LineGraphicItem):
         """
@@ -2306,16 +2467,17 @@
 
         # update position
         graphic_object.update_ports()
 
         # delete from the schematic
         self.remove_from_scene(line_graphic)
 
-        self.update_diagram_element(device=hvdc, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
-        # self.delete_diagram_element(device=line)
+        self.update_diagram_element(device=hvdc, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
     def convert_line_to_transformer(self, line: Line, line_graphic: LineGraphicItem):
         """
         Convert a line to Transformer
         :param line: Line instance
         :param line_graphic: LineGraphicItem
         :return: Nothing
@@ -2328,15 +2490,17 @@
 
         # update position
         graphic_object.update_ports()
 
         # delete from the schematic
         self.remove_from_scene(line_graphic)
 
-        self.update_diagram_element(device=transformer, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+        self.update_diagram_element(device=transformer, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
         # self.delete_diagram_element(device=line)
 
     def convert_line_to_vsc(self, line: Line, line_graphic: LineGraphicItem):
         """
         Convert a line to voltage source converter
         :param line: Line instance
         :param line_graphic: LineGraphicItem
@@ -2350,16 +2514,17 @@
 
         # update position
         graphic_object.update_ports()
 
         # delete from the schematic
         self.remove_from_scene(line_graphic)
 
-        self.update_diagram_element(device=vsc, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
-        # self.delete_diagram_element(device=line)
+        self.update_diagram_element(device=vsc, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
     def convert_line_to_upfc(self, line: Line, line_graphic: LineGraphicItem):
         """
         Convert a line to UPFC
         :param line: Line instance
         :param line_graphic: LineGraphicItem
         :return: Nothing
@@ -2372,15 +2537,17 @@
 
         # update position
         graphic_object.update_ports()
 
         # delete from the schematic
         self.remove_from_scene(line_graphic)
 
-        self.update_diagram_element(device=upfc, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+        self.update_diagram_element(device=upfc, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
     def convert_line_to_series_reactance(self, line: Line, line_graphic: LineGraphicItem):
         """
         Convert a line to convert_line_to_series_reactance
         :param line: Line instance
         :param line_graphic: LineGraphicItem
         :return: Nothing
@@ -2393,15 +2560,17 @@
 
         # update position
         graphic_object.update_ports()
 
         # delete from the schematic
         self.remove_from_scene(line_graphic)
 
-        self.update_diagram_element(device=series_reactance, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
+        self.update_diagram_element(device=series_reactance, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
     def convert_fluid_path_to_line(self, element: FluidPath, item_graphic: FluidPathGraphicItem):
         """
         Convert a fluid node to an electrical line
         :param element: FluidPath instance
         :param item_graphic: FluidPathGraphicItem
         :return: Nothing
@@ -2424,16 +2593,17 @@
         # update position
         fl_from.get_terminal().update()
         fl_to.get_terminal().update()
 
         # delete from the schematic
         self.remove_from_scene(item_graphic)
 
-        self.update_diagram_element(device=line, x=0, y=0, w=0, h=0, r=0, graphic_object=graphic_object)
-        # self.delete_diagram_element(device=element)
+        self.update_diagram_element(device=line, x=0, y=0, w=0, h=0, r=0,
+                                    draw_labels=graphic_object.draw_labels,
+                                    graphic_object=graphic_object)
 
     def convert_generator_to_battery(self, gen: Generator, graphic_object: GeneratorGraphicItem):
         """
         Convert a generator to a battery
         :param gen: Generator instance
         :param graphic_object: GeneratorGraphicItem
         :return: Nothing
@@ -3264,14 +3434,15 @@
 
                 self.update_diagram_element(device=bus,
                                             x=x_m,
                                             y=y_m,
                                             w=graphic_object.w,
                                             h=graphic_object.h,
                                             r=0,
+                                            draw_labels=graphic_object.draw_labels,
                                             graphic_object=graphic_object)
                 graphic_object.set_position(x=x_m, y=y_m)
 
         return
 
     def get_boundaries(self):
         """
@@ -3573,30 +3744,30 @@
 
                 plt.legend()
                 fig.suptitle(api_object.name, fontsize=20)
 
                 # plot the profiles
                 plt.show()
 
-    def set_rate_to_profile(self, api_object):
+    def set_rate_to_profile(self, api_object: ALL_DEV_TYPES):
         """
 
         :param api_object:
         """
         if api_object is not None:
             if api_object.rate_prof.size():
                 quit_msg = (f"{api_object.name}\nAre you sure that you want to overwrite the "
                             f"rates profile with the snapshot value?")
                 reply = QMessageBox.question(self, 'Overwrite the profile', quit_msg,
                                              QMessageBox.StandardButton.Yes, QMessageBox.StandardButton.No)
 
                 if reply == QMessageBox.StandardButton.Yes.value:
                     api_object.rate_prof.fill(api_object.rate)
 
-    def set_active_status_to_profile(self, api_object, override_question=False):
+    def set_active_status_to_profile(self, api_object: ALL_DEV_TYPES, override_question=False):
         """
 
         :param api_object:
         :param override_question:
         :return:
         """
         if api_object is not None:
@@ -3718,18 +3889,21 @@
             self.circuit.add_bus(mid_bus)
             self.circuit.add_line(br1)
             self.circuit.add_line(br2)
 
             # add new stuff as new investment
             inv_group = InvestmentsGroup(name=line.name + ' split', category='Line split')
             self.circuit.add_investments_group(inv_group)
-            self.circuit.add_investment(
-                Investment(name=mid_bus.name, device_idtag=mid_bus.idtag, group=inv_group))
+            self.circuit.add_investment(Investment(name=mid_bus.name, device_idtag=mid_bus.idtag, group=inv_group))
             self.circuit.add_investment(Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
             self.circuit.add_investment(Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
+            # include the deactivation of the original line
+            self.circuit.add_investment(Investment(name=line_graphics.api_object.name,
+                                                   device_idtag=line_graphics.api_object.idtag,
+                                                   status=False, group=inv_group))
 
             # add to the schematic the new 2 lines and the bus
             middle_bus_graphics = self.add_api_bus(bus=mid_bus,
                                                    injections_by_tpe=dict(),
                                                    x0=middle_bus_x,
                                                    y0=middle_bus_y)
             br1_graphics = self.add_api_line(branch=br1,
@@ -3834,17 +4008,17 @@
                                     return None
                                 if bus_t_graphic_obj is None:
                                     error_msg(f"{line.bus_to} was not found in the graphics manager")
                                     return None
 
                                 # C(x, y) = (x1 + t * (x2 - x1), y1 + t * (y2 - y1))
                                 mid_x = bus_f_graphics_data.x + (
-                                            bus_t_graphics_data.x - bus_f_graphics_data.x) * position
+                                        bus_t_graphics_data.x - bus_f_graphics_data.x) * position
                                 mid_y = bus_f_graphics_data.y + (
-                                            bus_t_graphics_data.y - bus_f_graphics_data.y) * position
+                                        bus_t_graphics_data.y - bus_f_graphics_data.y) * position
 
                                 B1 = Bus(name=line.name + ' split bus 1',
                                          vnom=line.bus_from.Vnom,
                                          vmin=line.bus_from.Vmin,
                                          vmax=line.bus_from.Vmax,
                                          area=line.bus_from.area,
                                          zone=line.bus_from.zone,
@@ -3962,27 +4136,32 @@
                                 self.circuit.add_line(br3)
                                 self.circuit.add_line(br4)
 
                                 # add new stuff as new investment
                                 inv_group = InvestmentsGroup(name=line.name + ' in/out', category='Line in/out')
                                 self.circuit.add_investments_group(inv_group)
                                 self.circuit.add_investment(
-                                    Investment(name=B1.name, device_idtag=B1.idtag, group=inv_group))
+                                    Investment(name=B1.name, device_idtag=B1.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=B2.name, device_idtag=B2.idtag, group=inv_group))
+                                    Investment(name=B2.name, device_idtag=B2.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=B3.name, device_idtag=B3.idtag, group=inv_group))
+                                    Investment(name=B3.name, device_idtag=B3.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=br1.name, device_idtag=br1.idtag, group=inv_group))
+                                    Investment(name=br1.name, device_idtag=br1.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=br2.name, device_idtag=br2.idtag, group=inv_group))
+                                    Investment(name=br2.name, device_idtag=br2.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=br3.name, device_idtag=br3.idtag, group=inv_group))
+                                    Investment(name=br3.name, device_idtag=br3.idtag, status=True, group=inv_group))
                                 self.circuit.add_investment(
-                                    Investment(name=br4.name, device_idtag=br4.idtag, group=inv_group))
+                                    Investment(name=br4.name, device_idtag=br4.idtag, status=True, group=inv_group))
+
+                                # include the deactivation of the original line
+                                self.circuit.add_investment(Investment(name=line_graphics.api_object.name,
+                                                                       device_idtag=line_graphics.api_object.idtag,
+                                                                       status=False, group=inv_group))
 
                                 # add to the schematic the new 2 lines and the bus
                                 B1_graphics = self.add_api_bus(bus=B1,
                                                                injections_by_tpe=dict(),
                                                                x0=mid_x,
                                                                y0=mid_y)
 
@@ -4114,14 +4293,15 @@
                                 dc_lines: List[DcLine],
                                 transformers2w: List[Transformer2W],
                                 transformers3w: List[Transformer3W],
                                 windings: List[Winding],
                                 hvdc_lines: List[HvdcLine],
                                 vsc_devices: List[VSC],
                                 upfc_devices: List[UPFC],
+                                series_reactances: List[SeriesReactance],
                                 fluid_nodes: List[FluidNode],
                                 fluid_paths: List[FluidPath],
                                 explode_factor=1.0,
                                 prog_func: Union[Callable, None] = None,
                                 text_func: Union[Callable, None] = None,
                                 name='Bus branch diagram') -> SchematicDiagram:
     """
@@ -4131,16 +4311,17 @@
     :param dc_lines: list of DcLine objects
     :param transformers2w: list of Transformer Objects
     :param transformers3w: list of Transformer3W Objects
     :param windings: list of Winding objects
     :param hvdc_lines: list of HvdcLine objects
     :param vsc_devices: list Vsc objects
     :param upfc_devices: List of UPFC devices
-    :param fluid_nodes:
-    :param fluid_paths:
+    :param series_reactances: List of SeriesReactance
+    :param fluid_nodes: List of FluidNode
+    :param fluid_paths: List of FluidPath
     :param explode_factor: factor of "explosion": Separation of the nodes factor
     :param prog_func: progress report function
     :param text_func: Text report function
     :param name: name of the diagram
     """
 
     diagram = SchematicDiagram(name=name)
@@ -4213,14 +4394,26 @@
         if prog_func is not None:
             prog_func((i + 1) / nn * 100.0)
 
         diagram.set_point(device=branch, location=GraphicLocation())
 
     # --------------------------------------------------------------------------------------------------------------
     if text_func is not None:
+        text_func('Creating schematic series reactances devices')
+
+    nn = len(series_reactances)
+    for i, branch in enumerate(series_reactances):
+
+        if prog_func is not None:
+            prog_func((i + 1) / nn * 100.0)
+
+        diagram.set_point(device=branch, location=GraphicLocation())
+
+    # --------------------------------------------------------------------------------------------------------------
+    if text_func is not None:
         text_func('Creating schematic transformer3w devices')
 
     nn = len(transformers3w)
     for i, elm in enumerate(transformers3w):
 
         if prog_func is not None:
             prog_func((i + 1) / nn * 100.0)
@@ -4291,17 +4484,31 @@
             prog_func((i + 1) / nn * 100.0)
 
         diagram.set_point(device=elm, location=GraphicLocation())
 
     return diagram
 
 
-def make_vecinity_diagram(circuit: MultiCircuit, root_bus: Bus, max_level: int = 1):
+def get_devices_to_expand(circuit: MultiCircuit,
+                          root_bus: Bus,
+                          max_level: int = 1) -> Tuple[
+    List[Bus],
+    List[Line],
+    List[DcLine],
+    List[Transformer2W],
+    List[Transformer3W],
+    List[Winding],
+    List[HvdcLine],
+    List[VSC],
+    List[UPFC],
+    List[SeriesReactance],
+    List[FluidNode],
+    List[FluidPath]]:
     """
-    Create a vecinity diagram
+    get lists of devices to expand given a root bus
     :param circuit: MultiCircuit
     :param root_bus: Bus
     :param max_level: max expansion level
     :return:
     """
 
     branch_idx = list()
@@ -4342,23 +4549,24 @@
                     bus_pool.append((br.bus_from, level + 1))
                     selected_branches.add(br)
 
                 else:
                     pass
 
     # sort Branches
-    lines = list()
-    dc_lines = list()
-    transformers2w = list()
-    transformers3w = list()
-    windings = list()
-    hvdc_lines = list()
-    vsc_converters = list()
-    upfc_devices = list()
-    fluid_paths = list()
+    lines: List[Line] = list()
+    dc_lines: List[DcLine] = list()
+    transformers2w: List[Transformer2W] = list()
+    transformers3w: List[Transformer3W] = list()
+    windings: List[Winding] = list()
+    hvdc_lines: List[HvdcLine] = list()
+    vsc_converters: List[VSC] = list()
+    upfc_devices: List[UPFC] = list()
+    series_reactances: List[SeriesReactance] = list()
+    fluid_paths: List[FluidPath] = list()
 
     for obj in selected_branches:
 
         branch_idx.append(branch_dict[obj])
 
         if obj.device_type == DeviceType.LineDevice:
             lines.append(obj)
@@ -4383,24 +4591,44 @@
 
         elif obj.device_type == DeviceType.UpfcDevice:
             upfc_devices.append(obj)
 
         else:
             raise Exception('Unrecognized branch type ' + obj.device_type.value)
 
+    return (list(buses), lines, dc_lines, transformers2w, transformers3w, windings, hvdc_lines,
+            vsc_converters, upfc_devices, series_reactances, list(fluid_nodes), fluid_paths)
+
+
+def make_vecinity_diagram(circuit: MultiCircuit, root_bus: Bus, max_level: int = 1):
+    """
+    Create a vecinity diagram
+    :param circuit: MultiCircuit
+    :param root_bus: Bus
+    :param max_level: max expansion level
+    :return:
+    """
+
+    (buses, lines, dc_lines, transformers2w,
+     transformers3w, windings, hvdc_lines,
+     vsc_converters, upfc_devices,
+     series_reactances,
+     fluid_nodes, fluid_paths) = get_devices_to_expand(circuit=circuit, root_bus=root_bus, max_level=max_level)
+
     # Draw schematic subset
     diagram = generate_bus_branch_diagram(buses=list(buses),
                                           lines=lines,
                                           dc_lines=dc_lines,
                                           transformers2w=transformers2w,
                                           transformers3w=transformers3w,
                                           windings=windings,
                                           hvdc_lines=hvdc_lines,
                                           vsc_devices=vsc_converters,
                                           upfc_devices=upfc_devices,
+                                          series_reactances=series_reactances,
                                           fluid_nodes=list(fluid_nodes),
                                           fluid_paths=fluid_paths,
                                           explode_factor=1.0,
                                           prog_func=None,
                                           text_func=print,
                                           name=root_bus.name + 'vecinity')
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,20 +186,39 @@
 
         self.parent = parent
 
         self.api_object: ALL_DEV_TYPES = api_object
 
         self.editor: DiagramEditorWidget = editor
 
-        self.draw_labels: bool = draw_labels
+        self._draw_labels: bool = draw_labels
 
         # color
         self.color = ACTIVE['color']
         self.style = ACTIVE['style']
 
+    @property
+    def draw_labels(self) -> bool:
+        """
+        draw labels getter
+        :return: Bool
+        """
+        return self._draw_labels
+
+    @draw_labels.setter
+    def draw_labels(self, value: bool):
+        """
+        Draw labels setter, it updates the diagram
+        :param value: boolean
+        """
+        self._draw_labels = value
+
+        # update editor diagram position
+        self.editor.update_label_drwaing_status(device=self.api_object, draw_labels=self._draw_labels)
+
     def recolour_mode(self) -> None:
         """
         Change the colour according to the system theme
         """
         if self.api_object is not None:
             if hasattr(self.api_object, 'active'):
                 if self.api_object.active:
@@ -231,7 +250,9 @@
 
     def enable_disable_label_drawing(self):
         """
 
         :return:
         """
         self.draw_labels = not self.draw_labels
+
+
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,25 +37,26 @@
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem, None],
                  editor: DiagramEditorWidget,
                  width=10,
                  api_object: FluidPath = None,
-                 arrow_size=15):
+                 arrow_size=15,
+                 draw_labels: bool = True):
         """
         
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         :param arrow_size:
         """
-        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=True)
+        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=draw_labels)
         LineGraphicTemplateItem.__init__(self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
                                          api_object=api_object,
                                          arrow_size=arrow_size)
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,18 @@
 
       - in and output ports
       - parameters
       - description
     """
 
     def __init__(self, editor: DiagramEditorWidget, fluid_node: FluidNode,
-                 parent=None, index=0, h: int = 20, w: int = 80, x: int = 0, y: int = 0):
+                 parent=None, index=0, h: int = 20, w: int = 80, x: int = 0, y: int = 0,
+                 draw_labels: bool = True):
 
-        GenericDBWidget.__init__(self, parent=parent, api_object=fluid_node, editor=editor, draw_labels=True)
+        GenericDBWidget.__init__(self, parent=parent, api_object=fluid_node, editor=editor, draw_labels=draw_labels)
         QtWidgets.QGraphicsRectItem.__init__(self, parent)
 
         self.min_w = 180.0
         self.min_h = 40.0
         self.offset = 20
         self.h = h if h >= self.min_h else self.min_h
         self.w = w if w >= self.min_w else self.min_w
@@ -177,14 +178,15 @@
 
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=self.h,
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
     def set_position(self, x, y):
         """
         Set the bus x, y position
         :param x: x in pixels
         :param y: y in pixels
@@ -258,14 +260,15 @@
         # update editor diagram position
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=int(self.min_h),
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
         return self.w, self.min_h
 
     def arrange_children(self):
         """
         This function sorts the load and generators icons
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,32 @@
     """
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem, None],
                  editor: DiagramEditorWidget,
                  width=5,
-                 api_object: Line = None):
+                 api_object: Line = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
+        :param draw_labels:
         """
         LineGraphicTemplateItem.__init__(self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def remove_symbol(self) -> None:
         """
         Remove all symbols
         """
         for elm in [self.symbol]:
             if elm is not None:
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,29 +28,31 @@
 
 class SeriesReactanceGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem],
                  editor: DiagramEditorWidget, width=5,
-                 api_object: SeriesReactance = None):
+                 api_object: SeriesReactance = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,29 +229,31 @@
 
 class DcLineGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem],
                  editor: DiagramEditorWidget,
-                 width=5, api_object: DcLine = None):
+                 width=5, api_object: DcLine = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,31 @@
 class HvdcGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem],
                  editor: DiagramEditorWidget,
                  width=5,
-                 api_object: HvdcLine = None):
+                 api_object: HvdcLine = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,31 @@
     from GridCal.Gui.Diagrams.DiagramEditorWidget.diagram_editor_widget import DiagramEditorWidget
 
 
 class UpfcGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self, from_port: BarTerminalItem, to_port: BarTerminalItem,
                  editor: DiagramEditorWidget, width=5,
-                 api_object: UPFC = None):
+                 api_object: UPFC = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,33 @@
     """
     TransformerGraphicItem
     """
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem],
-                 editor: DiagramEditorWidget, width=5,
-                 api_object: Transformer2W = None):
+                 editor: DiagramEditorWidget,
+                 width=5,
+                 api_object: Transformer2W = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,29 +32,31 @@
     Graphics item for the VSC converter
     """
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem],
                  editor: DiagramEditorWidget, width=5,
-                 api_object: VSC = None):
+                 api_object: VSC = None,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         """
         LineGraphicTemplateItem.__init__(self=self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
-                                         api_object=api_object)
+                                         api_object=api_object,
+                                         draw_labels=draw_labels)
 
     def contextMenuEvent(self, event):
         """
         Show context menu
         @param event:
         @return:
         """
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,25 +420,27 @@
 
     def __init__(self,
                  from_port: Union[BarTerminalItem, RoundTerminalItem],
                  to_port: Union[BarTerminalItem, RoundTerminalItem, None],
                  editor: DiagramEditorWidget,
                  width=5,
                  api_object: Union[Line, Transformer2W, VSC, UPFC, HvdcLine, DcLine, FluidPath, None] = None,
-                 arrow_size=10):
+                 arrow_size=10,
+                 draw_labels: bool = True):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         :param arrow_size:
+        :param draw_labels:
         """
-        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=True)
+        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=draw_labels)
         QGraphicsLineItem.__init__(self)
 
         if isinstance(api_object, Transformer2W):
             if isinstance(api_object, Winding):  # Winding is a sublass of Transformer
                 self.symbol = None
             else:
                 self.symbol = TransformerSymbol(parent=self, pen_width=width, h=80, w=80)
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         super().mouseMoveEvent(event)
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=self.h,
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
     def add_big_marker(self, color: Union[None, QColor] = Qt.red, tool_tip_text: str = ""):
         """
         Add a big marker to the bus
         :param color: Qt Color ot the marker
         :param tool_tip_text: tool tip text to display
@@ -253,14 +254,15 @@
         # update editor diagram position
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=w,
                                            h=int(self.min_h),
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
         return w, self.min_h
 
     def arrange_children(self) -> None:
         """
         This function sorts the load and generators icons
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     CurrentInjection)
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Injections.controllable_shunt_graphics import (
     ControllableShuntGraphicItem,
     ControllableShunt)
 
 from GridCalEngine.enumerations import DeviceType, FaultType
 from GridCalEngine.Devices.types import INJECTION_DEVICE_TYPES
-from GridCalEngine.Simulations.Topology.topology_reduction_driver import reduce_buses
 from GridCalEngine.Devices.Substation.connectivity_node import ConnectivityNode
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
     from GridCal.Gui.Diagrams.DiagramEditorWidget.diagram_editor_widget import DiagramEditorWidget
 
 
 class CnGraphicItem(GenericDBWidget, QtWidgets.QGraphicsRectItem):
@@ -142,14 +141,15 @@
         super().mouseMoveEvent(event)
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=self.h,
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
     def set_position(self, x: int, y: int) -> None:
         """
         Set the bus x, y position
         :param x: x in pixels
         :param y: y in pixels
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,27 +66,28 @@
                  parent=None,
                  index=0,
                  editor: DiagramEditorWidget = None,
                  bus: Bus = None,
                  h: int = 40,
                  w: int = 80,
                  x: int = 0,
-                 y: int = 0):
+                 y: int = 0,
+                 draw_labels: bool = True):
         """
 
         :param parent:
         :param index:
         :param editor:
         :param bus:
         :param h:
         :param w:
         :param x:
         :param y:
         """
-        GenericDBWidget.__init__(self, parent=parent, api_object=bus, editor=editor, draw_labels=True)
+        GenericDBWidget.__init__(self, parent=parent, api_object=bus, editor=editor, draw_labels=draw_labels)
         QtWidgets.QGraphicsRectItem.__init__(self, parent)
 
         self.min_w = 180.0
         self.min_h = 40.0
         self.offset = 20
         self.h = h if h >= self.min_h else self.min_h
         self.w = w if w >= self.min_w else self.min_w
@@ -156,14 +157,15 @@
         super().mouseMoveEvent(event)
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=self.h,
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
     def add_big_marker(self, color: Union[None, QColor] = Qt.red, tool_tip_text: str = ""):
         """
         Add a big marker to the bus
         :param color: Qt Color ot the marker
         :param tool_tip_text: tool tip text to display
@@ -254,14 +256,15 @@
         # update editor diagram position
         self.editor.update_diagram_element(device=self.api_object,
                                            x=self.pos().x(),
                                            y=self.pos().y(),
                                            w=self.w,
                                            h=int(self.min_h),
                                            r=self.rotation(),
+                                           draw_labels=self.draw_labels,
                                            graphic_object=self)
 
         return self.w, self.min_h
 
     def arrange_children(self) -> None:
         """
         This function sorts the load and generators icons
@@ -427,19 +430,19 @@
 
         da = menu.addAction('Delete')
         del_icon = QIcon()
         del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
         da.setIcon(del_icon)
         da.triggered.connect(self.remove)
 
-        re = menu.addAction('Reduce')
+        re = menu.addAction('Expand schematic')
         re_icon = QIcon()
-        re_icon.addPixmap(QPixmap(":/Icons/icons/grid_reduction.svg"))
+        re_icon.addPixmap(QPixmap(":/Icons/icons/grid_icon.svg"))
         re.setIcon(re_icon)
-        re.triggered.connect(self.reduce)
+        re.triggered.connect(self.expand_diagram_from_bus)
 
         menu.addSection("Add")
 
         al = menu.addAction('Load')
         al_icon = QIcon()
         al_icon.addPixmap(QPixmap(":/Icons/icons/add_load.svg"))
         al.setIcon(al_icon)
@@ -497,24 +500,14 @@
 
     def delete_all_connections(self) -> None:
         """
         Delete all bus connections
         """
         self._terminal.remove_all_connections()
 
-    def reduce(self):
-        """
-        Reduce this bus
-        :return:
-        """
-        ok = yes_no_question('Are you sure that you want to reduce this bus', 'Reduce bus')
-        if ok:
-            reduce_buses(self.editor.circuit, [self.api_object])
-            self.remove()
-
     def remove(self, ask: bool = True) -> None:
         """
         Remove this element
         @return:
         """
         if ask:
             ok = yes_no_question('Are you sure that you want to remove this bus', 'Remove bus')
@@ -534,14 +527,20 @@
         Update the colour
         """
         if self.api_object.active:
             self.set_tile_color(QBrush(ACTIVE['color']))
         else:
             self.set_tile_color(QBrush(DEACTIVATED['color']))
 
+    def expand_diagram_from_bus(self) -> None:
+        """
+        Expands the diagram from this bus
+        """
+        self.editor.expand_diagram_from_bus(root_bus=self.api_object)
+
     def enable_disable_toggle(self):
         """
         Toggle bus element state
         @return:
         """
         if self.api_object is not None:
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_widget.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/node_widget.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/node_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/map_events.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,17 @@
                         nodSiz = len(self.schema_Manager.CurrentLine.Nodes)
                         if(nodSiz > 1):
                             i1 = nodSiz - 1
                             i2 = nodSiz - 2
                             self.schema_Manager.CurrentLine.CreateConnector(i1, i2)
             elif category == DeviceType.VoltageLevelDevice.value:
                 for idtag, location in points_group.locations.items():
-                    self.schema_Manager.CreateSubstation(location.latitude, location.longitude)
+                    if(location.api_object.substation):
+                        objectSubs = location.api_object.substation
+                        self.schema_Manager.CreateSubstation(objectSubs.longitude, -objectSubs.latitude)
 
     def colour_results(self,
                        buses: List[Bus],
                        branches: List[BRANCH_TYPES],
                        hvdc_lines: List[HvdcLine],
                        Sbus: CxVec,
                        bus_active: IntVec,
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py` & `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/AboutDialogue/about_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/AboutDialogue/about_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/AboutDialogue/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/AboutDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/AboutDialogue/gui.py` & `GridCal-5.1.6/GridCal/Gui/AboutDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_dialog.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_dialog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/models_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/models_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profile_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profile_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/ProfilesInput/excel_sheet_selection.py` & `GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_sheet_selection.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Analysis/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/Analysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Analysis/AnalysisDialogue.py` & `GridCal-5.1.6/GridCal/Gui/Analysis/AnalysisDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Analysis/gui.py` & `GridCal-5.1.6/GridCal/Gui/Analysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Analysis/object_plot_analysis.py` & `GridCal-5.1.6/GridCal/Gui/Analysis/object_plot_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/CascadingSteps/cascading_steps.py` & `GridCal-5.1.6/GridCal/Gui/CascadingSteps/cascading_steps.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/CascadingSteps/gui.py` & `GridCal-5.1.6/GridCal/Gui/CascadingSteps/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/ConsoleLogController.py` & `GridCal-5.1.6/GridCal/Gui/Main/ConsoleLogController.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/GridCalMain.py` & `GridCal-5.1.6/GridCal/Gui/Main/GridCalMain.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/MainWindow.py` & `GridCal-5.1.6/GridCal/Gui/Main/MainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'MainWindow.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.7.0
+## Created by: Qt User Interface Compiler version 6.6.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -1579,15 +1579,15 @@
         brush2.setStyle(Qt.SolidPattern)
         palette2.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette2.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette2.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_14.setPalette(palette2)
         self.line_14.setFrameShadow(QFrame.Plain)
         self.line_14.setLineWidth(4)
-        self.line_14.setFrameShape(QFrame.Shape.HLine)
+        self.line_14.setFrameShape(QFrame.HLine)
 
         self.gridLayout_9.addWidget(self.line_14, 1, 0, 1, 2)
 
         self.frame_20 = QFrame(self.frame_13)
         self.frame_20.setObjectName(u"frame_20")
         self.frame_20.setFrameShape(QFrame.NoFrame)
         self.frame_20.setFrameShadow(QFrame.Raised)
@@ -1676,15 +1676,15 @@
         palette4 = QPalette()
         palette4.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette4.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette4.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_17.setPalette(palette4)
         self.line_17.setFrameShadow(QFrame.Plain)
         self.line_17.setLineWidth(4)
-        self.line_17.setFrameShape(QFrame.Shape.HLine)
+        self.line_17.setFrameShape(QFrame.HLine)
 
         self.gridLayout_2.addWidget(self.line_17, 1, 0, 1, 3)
 
         self.vs_departure_comboBox = QComboBox(self.frame_21)
         self.vs_departure_comboBox.setObjectName(u"vs_departure_comboBox")
 
         self.gridLayout_2.addWidget(self.vs_departure_comboBox, 11, 1, 1, 2)
@@ -1970,15 +1970,15 @@
         palette7 = QPalette()
         palette7.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette7.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette7.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_16.setPalette(palette7)
         self.line_16.setFrameShadow(QFrame.Plain)
         self.line_16.setLineWidth(4)
-        self.line_16.setFrameShape(QFrame.Shape.HLine)
+        self.line_16.setFrameShape(QFrame.HLine)
 
         self.gridLayout_10.addWidget(self.line_16, 2, 0, 1, 5)
 
         self.groupBox_2 = QGroupBox(self.tab_4)
         self.groupBox_2.setObjectName(u"groupBox_2")
         self.groupBox_2.setFont(font3)
         self.gridLayout_26 = QGridLayout(self.groupBox_2)
@@ -2106,15 +2106,15 @@
         palette9 = QPalette()
         palette9.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette9.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette9.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_27.setPalette(palette9)
         self.line_27.setFrameShadow(QFrame.Plain)
         self.line_27.setLineWidth(4)
-        self.line_27.setFrameShape(QFrame.Shape.HLine)
+        self.line_27.setFrameShape(QFrame.HLine)
 
         self.gridLayout_13.addWidget(self.line_27, 1, 0, 1, 4)
 
         self.groupBox_4 = QGroupBox(self.tab_12)
         self.groupBox_4.setObjectName(u"groupBox_4")
         self.gridLayout_20 = QGridLayout(self.groupBox_4)
         self.gridLayout_20.setObjectName(u"gridLayout_20")
@@ -2254,15 +2254,15 @@
         palette10 = QPalette()
         palette10.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette10.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette10.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_26.setPalette(palette10)
         self.line_26.setFrameShadow(QFrame.Plain)
         self.line_26.setLineWidth(4)
-        self.line_26.setFrameShape(QFrame.Shape.HLine)
+        self.line_26.setFrameShape(QFrame.HLine)
 
         self.gridLayout_4.addWidget(self.line_26, 1, 0, 1, 2)
 
         self.label_95 = QLabel(self.frame_40)
         self.label_95.setObjectName(u"label_95")
         palette11 = QPalette()
         palette11.setBrush(QPalette.Active, QPalette.WindowText, brush3)
@@ -2375,15 +2375,15 @@
         palette12 = QPalette()
         palette12.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette12.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette12.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_22.setPalette(palette12)
         self.line_22.setFrameShadow(QFrame.Plain)
         self.line_22.setLineWidth(4)
-        self.line_22.setFrameShape(QFrame.Shape.HLine)
+        self.line_22.setFrameShape(QFrame.HLine)
 
         self.gridLayout_14.addWidget(self.line_22, 1, 0, 1, 2)
 
         self.verticalSpacer_12 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.gridLayout_14.addItem(self.verticalSpacer_12, 8, 0, 1, 1)
 
@@ -2559,15 +2559,15 @@
         palette15 = QPalette()
         palette15.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette15.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette15.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_25.setPalette(palette15)
         self.line_25.setFrameShadow(QFrame.Plain)
         self.line_25.setLineWidth(4)
-        self.line_25.setFrameShape(QFrame.Shape.HLine)
+        self.line_25.setFrameShape(QFrame.HLine)
 
         self.gridLayout_28.addWidget(self.line_25, 2, 0, 1, 2)
 
         self.label_1322 = QLabel(self.frame_76)
         self.label_1322.setObjectName(u"label_1322")
 
         self.gridLayout_28.addWidget(self.label_1322, 12, 0, 1, 1)
@@ -2608,15 +2608,15 @@
         palette16 = QPalette()
         palette16.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette16.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette16.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_24.setPalette(palette16)
         self.line_24.setFrameShadow(QFrame.Plain)
         self.line_24.setLineWidth(4)
-        self.line_24.setFrameShape(QFrame.Shape.HLine)
+        self.line_24.setFrameShape(QFrame.HLine)
 
         self.gridLayout_21.addWidget(self.line_24, 14, 0, 1, 2)
 
         self.label_44 = QLabel(self.frame_18)
         self.label_44.setObjectName(u"label_44")
 
         self.gridLayout_21.addWidget(self.label_44, 17, 0, 1, 2)
@@ -2660,15 +2660,15 @@
         palette18 = QPalette()
         palette18.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette18.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette18.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_30.setPalette(palette18)
         self.line_30.setFrameShadow(QFrame.Plain)
         self.line_30.setLineWidth(4)
-        self.line_30.setFrameShape(QFrame.Shape.HLine)
+        self.line_30.setFrameShape(QFrame.HLine)
 
         self.gridLayout_21.addWidget(self.line_30, 19, 0, 1, 2)
 
         self.investment_evaluation_method_ComboBox = QComboBox(self.frame_18)
         self.investment_evaluation_method_ComboBox.setObjectName(u"investment_evaluation_method_ComboBox")
 
         self.gridLayout_21.addWidget(self.investment_evaluation_method_ComboBox, 21, 0, 1, 2)
@@ -2730,15 +2730,15 @@
         palette20 = QPalette()
         palette20.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette20.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette20.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_29.setPalette(palette20)
         self.line_29.setFrameShadow(QFrame.Plain)
         self.line_29.setLineWidth(4)
-        self.line_29.setFrameShape(QFrame.Shape.HLine)
+        self.line_29.setFrameShape(QFrame.HLine)
 
         self.gridLayout_21.addWidget(self.line_29, 9, 0, 1, 3)
 
         self.label_51 = QLabel(self.frame_18)
         self.label_51.setObjectName(u"label_51")
 
         self.gridLayout_21.addWidget(self.label_51, 22, 0, 1, 2)
@@ -2850,15 +2850,15 @@
         palette24 = QPalette()
         palette24.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette24.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette24.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_4.setPalette(palette24)
         self.line_4.setFrameShadow(QFrame.Plain)
         self.line_4.setLineWidth(4)
-        self.line_4.setFrameShape(QFrame.Shape.HLine)
+        self.line_4.setFrameShape(QFrame.HLine)
 
         self.gridLayout_6.addWidget(self.line_4, 1, 0, 1, 3)
 
         self.label_138 = QLabel(self.frame_15)
         self.label_138.setObjectName(u"label_138")
 
         self.gridLayout_6.addWidget(self.label_138, 7, 0, 1, 3)
@@ -2868,15 +2868,15 @@
         palette25 = QPalette()
         palette25.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette25.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette25.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_10.setPalette(palette25)
         self.line_10.setFrameShadow(QFrame.Plain)
         self.line_10.setLineWidth(4)
-        self.line_10.setFrameShape(QFrame.Shape.HLine)
+        self.line_10.setFrameShape(QFrame.HLine)
 
         self.gridLayout_6.addWidget(self.line_10, 9, 0, 1, 3)
 
         self.max_iterations_stochastic_spinBox = QSpinBox(self.frame_15)
         self.max_iterations_stochastic_spinBox.setObjectName(u"max_iterations_stochastic_spinBox")
         self.max_iterations_stochastic_spinBox.setMinimum(10)
         self.max_iterations_stochastic_spinBox.setMaximum(99999999)
@@ -2973,15 +2973,15 @@
         palette27 = QPalette()
         palette27.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette27.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette27.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_21.setPalette(palette27)
         self.line_21.setFrameShadow(QFrame.Plain)
         self.line_21.setLineWidth(4)
-        self.line_21.setFrameShape(QFrame.Shape.HLine)
+        self.line_21.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_36.addWidget(self.line_21)
 
         self.label_24 = QLabel(self.frame_39)
         self.label_24.setObjectName(u"label_24")
         self.label_24.setTextFormat(Qt.PlainText)
         self.label_24.setScaledContents(True)
@@ -3005,15 +3005,15 @@
         palette28 = QPalette()
         palette28.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette28.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette28.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_13.setPalette(palette28)
         self.line_13.setFrameShadow(QFrame.Plain)
         self.line_13.setLineWidth(4)
-        self.line_13.setFrameShape(QFrame.Shape.HLine)
+        self.line_13.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_36.addWidget(self.line_13)
 
         self.label_60 = QLabel(self.frame_39)
         self.label_60.setObjectName(u"label_60")
 
         self.verticalLayout_36.addWidget(self.label_60)
@@ -3086,15 +3086,15 @@
         palette30 = QPalette()
         palette30.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette30.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette30.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_8.setPalette(palette30)
         self.line_8.setFrameShadow(QFrame.Plain)
         self.line_8.setLineWidth(4)
-        self.line_8.setFrameShape(QFrame.Shape.HLine)
+        self.line_8.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_25.addWidget(self.line_8)
 
         self.frame_23 = QFrame(self.frame_31)
         self.frame_23.setObjectName(u"frame_23")
         self.frame_23.setFrameShape(QFrame.NoFrame)
         self.frame_23.setFrameShadow(QFrame.Raised)
@@ -3175,15 +3175,15 @@
         palette32 = QPalette()
         palette32.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette32.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette32.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_20.setPalette(palette32)
         self.line_20.setFrameShadow(QFrame.Plain)
         self.line_20.setLineWidth(4)
-        self.line_20.setFrameShape(QFrame.Shape.HLine)
+        self.line_20.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_21.addWidget(self.line_20)
 
         self.label_59 = QLabel(self.frame_27)
         self.label_59.setObjectName(u"label_59")
 
         self.verticalLayout_21.addWidget(self.label_59)
@@ -3261,15 +3261,15 @@
         palette34 = QPalette()
         palette34.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette34.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette34.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_9.setPalette(palette34)
         self.line_9.setFrameShadow(QFrame.Plain)
         self.line_9.setLineWidth(4)
-        self.line_9.setFrameShape(QFrame.Shape.HLine)
+        self.line_9.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_31.addWidget(self.line_9)
 
         self.frame_70 = QFrame(self.frame_46)
         self.frame_70.setObjectName(u"frame_70")
         self.frame_70.setFrameShape(QFrame.NoFrame)
         self.frame_70.setFrameShadow(QFrame.Raised)
@@ -3537,15 +3537,15 @@
         palette40 = QPalette()
         palette40.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette40.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette40.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_6.setPalette(palette40)
         self.line_6.setFrameShadow(QFrame.Plain)
         self.line_6.setLineWidth(4)
-        self.line_6.setFrameShape(QFrame.Shape.HLine)
+        self.line_6.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_7.addWidget(self.line_6)
 
         self.frame_24 = QFrame(self.frame_3)
         self.frame_24.setObjectName(u"frame_24")
         self.frame_24.setFrameShape(QFrame.NoFrame)
         self.frame_24.setFrameShadow(QFrame.Raised)
@@ -3636,15 +3636,15 @@
         palette42 = QPalette()
         palette42.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette42.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette42.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_28.setPalette(palette42)
         self.line_28.setFrameShadow(QFrame.Plain)
         self.line_28.setLineWidth(4)
-        self.line_28.setFrameShape(QFrame.Shape.HLine)
+        self.line_28.setFrameShape(QFrame.HLine)
 
         self.gridLayout_11.addWidget(self.line_28, 1, 0, 1, 2)
 
         self.saveResultsCheckBox = QCheckBox(self.frame_77)
         self.saveResultsCheckBox.setObjectName(u"saveResultsCheckBox")
 
         self.gridLayout_11.addWidget(self.saveResultsCheckBox, 6, 0, 1, 2)
@@ -3712,15 +3712,15 @@
         palette44 = QPalette()
         palette44.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette44.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette44.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_31.setPalette(palette44)
         self.line_31.setFrameShadow(QFrame.Plain)
         self.line_31.setLineWidth(4)
-        self.line_31.setFrameShape(QFrame.Shape.HLine)
+        self.line_31.setFrameShape(QFrame.HLine)
 
         self.gridLayout_5.addWidget(self.line_31, 1, 0, 1, 3)
 
         self.label_137 = QLabel(self.frame_79)
         self.label_137.setObjectName(u"label_137")
         self.label_137.setMinimumSize(QSize(24, 24))
         self.label_137.setMaximumSize(QSize(24, 24))
@@ -3797,15 +3797,15 @@
         palette46 = QPalette()
         palette46.setBrush(QPalette.Active, QPalette.WindowText, brush2)
         palette46.setBrush(QPalette.Inactive, QPalette.WindowText, brush2)
         palette46.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.line_5.setPalette(palette46)
         self.line_5.setFrameShadow(QFrame.Plain)
         self.line_5.setLineWidth(4)
-        self.line_5.setFrameShape(QFrame.Shape.HLine)
+        self.line_5.setFrameShape(QFrame.HLine)
 
         self.verticalLayout_12.addWidget(self.line_5)
 
         self.frame_25 = QFrame(self.frame_7)
         self.frame_25.setObjectName(u"frame_25")
         self.frame_25.setFrameShape(QFrame.NoFrame)
         self.frame_25.setFrameShadow(QFrame.Raised)
@@ -3965,15 +3965,15 @@
         font6 = QFont()
         font6.setPointSize(8)
         self.toolBar.setFont(font6)
         self.toolBar.setMovable(False)
         self.toolBar.setIconSize(QSize(26, 26))
         self.toolBar.setToolButtonStyle(Qt.ToolButtonIconOnly)
         self.toolBar.setFloatable(False)
-        mainWindow.addToolBar(Qt.ToolBarArea.TopToolBarArea, self.toolBar)
+        mainWindow.addToolBar(Qt.TopToolBarArea, self.toolBar)
 
         self.menuBar.addAction(self.menuProject.menuAction())
         self.menuBar.addAction(self.menuActions.menuAction())
         self.menuBar.addAction(self.menuDiagrams.menuAction())
         self.menuBar.addAction(self.menuModel.menuAction())
         self.menuBar.addAction(self.menuSimulations.menuAction())
         self.menuBar.addAction(self.menuAbout.menuAction())
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/update_gui_file.py` & `GridCal-5.1.6/GridCal/Gui/Main/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/ConsoleLog.py` & `GridCal-5.1.6/GridCal/Gui/Main/ConsoleLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ConsoleLog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.7.0
+## Created by: Qt User Interface Compiler version 6.6.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/object_select_window.py` & `GridCal-5.1.6/GridCal/Gui/Main/object_select_window.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/simulations.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/simulations.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/io.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/io.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/base_gui.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/base_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Scripting/scripting.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/scripting.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Settings/configuration.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/configuration.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/objects.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/objects.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/time_events.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/time_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/diagrams.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/diagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from pandas.plotting import register_matplotlib_converters
 
 import GridCalEngine.Devices as dev
 import GridCalEngine.Simulations as sim
 import GridCal.Gui.GuiFunctions as gf
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCalEngine.IO.file_system import get_create_gridcal_folder
-from GridCal.Gui.GeneralDialogues import CheckListDialogue, StartEndSelectionDialogue, InputSearchDialogue, \
-    InputNumberDialogue
+from GridCal.Gui.GeneralDialogues import (CheckListDialogue, StartEndSelectionDialogue, InputSearchDialogue,
+                                          InputNumberDialogue)
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
 from GridCal.Gui.Diagrams.DiagramEditorWidget.diagram_editor_widget import (DiagramEditorWidget,
                                                                             BusGraphicItem,
                                                                             generate_bus_branch_diagram,
                                                                             make_vecinity_diagram)
 from GridCal.Gui.Diagrams.MapWidget.grid_map_widget import GridMapWidget, generate_map_diagram
@@ -766,25 +766,26 @@
         """
         diagram_widget = self.get_selected_diagram_widget()
 
         if diagram_widget:
 
             if isinstance(diagram_widget, DiagramEditorWidget):
                 # set pointer to the circuit
-                diagram = generate_bus_branch_diagram(buses=self.circuit.buses,
-                                                      lines=self.circuit.lines,
-                                                      dc_lines=self.circuit.dc_lines,
-                                                      transformers2w=self.circuit.transformers2w,
-                                                      transformers3w=self.circuit.transformers3w,
-                                                      windings=self.circuit.windings,
-                                                      hvdc_lines=self.circuit.hvdc_lines,
-                                                      vsc_devices=self.circuit.vsc_devices,
-                                                      upfc_devices=self.circuit.upfc_devices,
-                                                      fluid_nodes=self.circuit.fluid_nodes,
-                                                      fluid_paths=self.circuit.fluid_paths,
+                diagram = generate_bus_branch_diagram(buses=self.circuit.get_buses(),
+                                                      lines=self.circuit.get_lines(),
+                                                      dc_lines=self.circuit.get_dc_lines(),
+                                                      transformers2w=self.circuit.get_transformers2w(),
+                                                      transformers3w=self.circuit.get_transformers3w(),
+                                                      windings=self.circuit.get_windings(),
+                                                      hvdc_lines=self.circuit.get_hvdc(),
+                                                      vsc_devices=self.circuit.get_vsc(),
+                                                      upfc_devices=self.circuit.get_upfc(),
+                                                      series_reactances=self.circuit.get_series_reactances(),
+                                                      fluid_nodes=self.circuit.get_fluid_nodes(),
+                                                      fluid_paths=self.circuit.get_fluid_paths(),
                                                       explode_factor=1.0,
                                                       prog_func=None,
                                                       text_func=None)
 
                 diagram_widget.set_data(circuit=self.circuit,
                                         diagram=diagram)
 
@@ -807,14 +808,15 @@
                                               dc_lines=self.circuit.get_dc_lines(),
                                               transformers2w=self.circuit.get_transformers2w(),
                                               transformers3w=self.circuit.get_transformers3w(),
                                               windings=self.circuit.get_windings(),
                                               hvdc_lines=self.circuit.get_hvdc(),
                                               vsc_devices=self.circuit.get_vsc(),
                                               upfc_devices=self.circuit.get_upfc(),
+                                              series_reactances=self.circuit.get_series_reactances(),
                                               fluid_nodes=self.circuit.get_fluid_nodes(),
                                               fluid_paths=self.circuit.get_fluid_paths(),
                                               explode_factor=1.0,
                                               prog_func=None,
                                               text_func=None,
                                               name=name)
```

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Main/SubClasses/Results/results.py` & `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/results.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Visualization/visualization.py` & `GridCal-5.1.6/GridCal/Gui/Visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/Visualization/palettes.py` & `GridCal-5.1.6/GridCal/Gui/Visualization/palettes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SyncDialogue/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/SyncDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SyncDialogue/sync_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/SyncDialogue/sync_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SyncDialogue/gui.py` & `GridCal-5.1.6/GridCal/Gui/SyncDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py` & `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SolarPowerWizard/gui.py` & `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/MainWindow.py` & `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/update_gui_file.py` & `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/RosetaExplorer.py` & `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/RosetaExplorer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/ConsoleWidget.py` & `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/RosetaExplorer/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer.py` & `GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/LoadDesigner/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/LoadDesigner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/LoadDesigner/load_designer_ui.py` & `GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py` & `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/WindPowerWizard/gui.py` & `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler.py` & `GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SystemScaler/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/SystemScaler/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SystemScaler/system_scaler_ui.py` & `GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/MainWindow.py` & `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/update_gui_file.py` & `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/TreeModelViewer/TreeModelViewer.py` & `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/TreeModelViewer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/gui.py` & `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/GridGenerator/grid_generator_dialogue.py` & `GridCal-5.1.6/GridCal/Gui/GridGenerator/grid_generator_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/GridGenerator/icons_rc.py` & `GridCal-5.1.6/GridCal/Gui/GridGenerator/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/GridCal/Gui/GridGenerator/gui.py` & `GridCal-5.1.6/GridCal/Gui/GridGenerator/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/setup.py` & `GridCal-5.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.5/PKG-INFO` & `GridCal-5.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCal
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

