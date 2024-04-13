# Comparing `tmp/PyQt-Fluent-Widgets-1.5.4.tar.gz` & `tmp/PyQt-Fluent-Widgets-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.5.4.tar", last modified: Sat Mar 23 06:15:48 2024, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.5.5.tar", last modified: Sat Apr 13 06:44:26 2024, max compression
```

## Comparing `PyQt-Fluent-Widgets-1.5.4.tar` & `PyQt-Fluent-Widgets-1.5.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.332369 PyQt-Fluent-Widgets-1.5.4/
--rw-rw-rw-   0        0        0    35825 2024-03-23 06:08:38.000000 PyQt-Fluent-Widgets-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     5676 2024-03-23 06:15:48.331273 PyQt-Fluent-Widgets-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.048448 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5676 2024-03-23 06:15:47.000000 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2024-03-23 06:15:47.000000 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 06:15:47.000000 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-03-23 06:15:47.000000 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-23 06:15:47.000000 PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4913 2024-03-23 06:12:35.000000 PyQt-Fluent-Widgets-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.049977 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/
--rw-rw-rw-   0        0        0      549 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.055578 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  6506729 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.100557 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1587 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11192 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      803 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13751 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5537 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      658 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4851 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14407 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.112300 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.128637 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2341 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21800 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7629 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19337 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6439 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.142946 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14788 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5860 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11337 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3173 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2879 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2500 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.154159 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2750 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7112 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.173234 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3006 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3536 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6276 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1181 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1431 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.195100 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9905 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12968 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8773 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24107 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19630 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6825 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5211 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.211183 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5282 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11031 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4648 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2843 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14036 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1586 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.308182 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3328 2024-03-23 06:08:38.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     7973 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    29975 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7700 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5802 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    15825 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19594 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7881 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13091 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17086 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2223 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1498 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16647 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18934 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14724 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    13887 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4812 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40458 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11189 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9199 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7033 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2718 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17887 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1204 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10220 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8555 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6534 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8631 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26348 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11538 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22906 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10563 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4484 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.319331 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11617 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3585 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2845 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 06:15:48.328367 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      164 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12196 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2846 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1664 2024-03-23 06:12:36.000000 PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-03-23 06:15:48.332369 PyQt-Fluent-Widgets-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1193 2024-03-23 06:13:17.000000 PyQt-Fluent-Widgets-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.923461 PyQt-Fluent-Widgets-1.5.5/
+-rw-rw-rw-   0        0        0    35825 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     5676 2024-04-13 06:44:26.921955 PyQt-Fluent-Widgets-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.723423 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5676 2024-04-13 06:44:26.000000 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4914 2024-04-13 06:44:26.000000 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:44:26.000000 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-13 06:44:26.000000 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-13 06:44:26.000000 PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4913 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.725455 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/
+-rw-rw-rw-   0        0        0      549 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.728552 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  6506729 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.770568 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1587 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11192 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      803 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13751 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5537 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      658 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4851 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14407 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.771576 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.782608 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2341 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21800 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7629 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19337 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6439 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.795221 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14788 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5860 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11337 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3173 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2879 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2500 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.802030 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2750 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7112 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.815609 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3006 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3536 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6276 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1181 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1431 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.829656 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9905 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12968 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8773 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24107 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    19705 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6825 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5211 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.841872 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5282 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11031 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4648 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2843 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14036 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1586 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.906018 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3328 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     7973 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    30016 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7700 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5802 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    15825 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19594 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7881 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13091 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17086 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2223 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1498 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16647 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18934 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14724 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14139 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4812 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40458 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11189 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9199 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7033 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2718 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17887 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1204 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10220 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8555 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6534 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8631 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26348 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11538 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22906 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10563 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4484 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.912987 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11617 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3585 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2845 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:44:26.919533 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:31:18.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12934 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2846 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1664 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 06:44:26.923461 PyQt-Fluent-Widgets-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2024-04-13 06:44:21.000000 PyQt-Fluent-Widgets-1.5.5/setup.py
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/LICENSE` & `PyQt-Fluent-Widgets-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/PKG-INFO` & `PyQt-Fluent-Widgets-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.5.4
+Version: 1.5.5
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.4 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.5 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL:
 Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords:
 pyqt fluent widgets Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.5.4
+Version: 1.5.5
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.4 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.5 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL:
 Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords:
 pyqt fluent widgets Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-1.5.5/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/README.md` & `PyQt-Fluent-Widgets-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3 for non-commercial project, see README for more details.
 """
 
-__version__ = "1.5.4"
+__version__ = "1.5.5"
 __author__ = "zhiyiYo"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/animation.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/color.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/font.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/overload.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/router.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/screen.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_box_base.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_combo_box.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_flyout.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_line_edit.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_menu.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/breadcrumb.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding:utf-8
 from typing import Union, List
 
 from PyQt5.QtCore import (Qt, pyqtSignal, QRect, QRectF, QPropertyAnimation, pyqtProperty, QMargins,
-                          QEasingCurve, QPoint, QEvent, QSize)
+                          QEasingCurve, QPoint, QEvent)
 from PyQt5.QtGui import QColor, QPainter, QPen, QIcon, QCursor, QFont, QBrush, QPixmap, QImage
 from PyQt5.QtWidgets import QWidget, QVBoxLayout
 from collections import deque
 
 from ...common.config import isDarkTheme
 from ...common.style_sheet import themeColor
 from ...common.icon import drawIcon, toQIcon
@@ -345,14 +345,15 @@
         self.vBoxLayout.setContentsMargins(0, 0, 0, 0)
         self.vBoxLayout.addWidget(self.itemWidget, 0, Qt.AlignTop)
 
         self.itemWidget.itemClicked.connect(self._onClicked)
         self.setAttribute(Qt.WA_TranslucentBackground)
         self.expandAni.valueChanged.connect(lambda g: self.setFixedSize(g.size()))
         self.expandAni.valueChanged.connect(self.expanded)
+        self.expandAni.finished.connect(self.parentWidget().layout().invalidate)
 
     def addChild(self, child):
         self.insertChild(-1, child)
 
     def text(self):
         return self.itemWidget.text()
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/pivot.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,22 @@
         elif self.isPressed:
             painter.setOpacity(0.786)
 
         w, h = self.iconSize().width(), self.iconSize().height()
         y = (self.height() - h) / 2
         mw = self.minimumSizeHint().width()
         if mw > 0:
-            self._drawIcon(self._icon, painter, QRectF(
-                12+(self.width()-mw)//2, y, w, h))
+            x = 12 + (self.width() - mw) // 2
         else:
-            self._drawIcon(self._icon, painter, QRectF(12, y, w, h))
+            x = 12
+
+        if self.isRightToLeft():
+            x = self.width() - w - x
+            
+        self._drawIcon(self._icon, painter, QRectF(x, y, w, h))
 
 
 class PrimaryPushButton(PushButton):
     """ Primary color push button
 
     Constructors
     ------------
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/card_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/check_box.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/command_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flip_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flyout.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_badge.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,8 +422,15 @@
         if e.type() == QEvent.MouseButtonPress:
             self.setPasswordVisible(True)
         elif e.type() == QEvent.MouseButtonRelease:
             self.setPasswordVisible(False)
 
         return super().eventFilter(obj, e)
 
+    def inputMethodQuery(self, query: Qt.InputMethodQuery):
+        # Disable IME for PasswordLineEdit
+        if query == Qt.InputMethodQuery.ImEnabled:
+            return False
+        else:
+            return super().inputMethodQuery(query)
+
     passwordVisible = pyqtProperty(bool, isPasswordVisible, setPasswordVisible)
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/list_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/pips_pager.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/separator.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tab_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/table_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_play_bar.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_player.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/video_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/fluent_window.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 
 class FluentWindowBase(BackgroundAnimationWidget, FramelessWindow):
     """ Fluent window base class """
 
     def __init__(self, parent=None):
         self._isMicaEnabled = False
+        self._lightBackgroundColor = QColor(243, 243, 243)
+        self._darkBackgroundColor = QColor(32, 32, 32)
         super().__init__(parent=parent)
 
         self.hBoxLayout = QHBoxLayout(self)
         self.stackedWidget = StackedWidget(self)
         self.navigationInterface = None
 
         # initialize layout
@@ -60,17 +62,29 @@
         isTransparent = self.stackedWidget.currentWidget().property("isStackedTransparent")
         if bool(self.stackedWidget.property("isTransparent")) == isTransparent:
             return
         
         self.stackedWidget.setProperty("isTransparent", isTransparent)
         self.stackedWidget.setStyle(QApplication.style())
 
+    def setCustomBackgroundColor(self, light, dark):
+        """ set custom background color
+
+        Parameters
+        ----------
+        light, dark: QColor | Qt.GlobalColor | str
+            background color in light/dark theme mode
+        """
+        self._lightBackgroundColor = QColor(light)
+        self._darkBackgroundColor = QColor(dark)
+        self._updateBackgroundColor()
+
     def _normalBackgroundColor(self):
         if not self.isMicaEffectEnabled():
-            return QColor(32, 32, 32) if isDarkTheme() else QColor(243, 243, 243)
+            return self._darkBackgroundColor if isDarkTheme() else self._lightBackgroundColor
 
         return QColor(0, 0, 0, 0)
 
     def _onThemeChangedFinished(self):
         if self.isMicaEffectEnabled():
             self.windowEffect.setMicaEffect(self.winId(), isDarkTheme())
 
@@ -332,7 +346,13 @@
         super().__init__(parent)
         self.setTitleBar(SplitTitleBar(self))
 
         self.widgetLayout.setContentsMargins(0, 0, 0, 0)
 
         self.titleBar.raise_()
         self.navigationInterface.displayModeChanged.connect(self.titleBar.raise_)
+
+
+class FluentBackgroundTheme:
+    """ Fluent background theme """
+    DEFAULT = (QColor(243, 243, 243), QColor(32, 32, 32))   # light, dark
+    DEFAULT_BLUE = (QColor(240, 244, 249), QColor(25, 33, 42))
```

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/splash_screen.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/qfluentwidgets/window/stacked_widget.py` & `PyQt-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.4/setup.py` & `PyQt-Fluent-Widgets-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="1.5.4",
+    version="1.5.5",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

