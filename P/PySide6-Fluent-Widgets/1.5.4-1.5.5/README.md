# Comparing `tmp/PySide6-Fluent-Widgets-1.5.4.tar.gz` & `tmp/PySide6-Fluent-Widgets-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.4.tar", last modified: Sat Mar 23 05:56:46 2024, max compression
+gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.5.tar", last modified: Sat Apr 13 06:40:11 2024, max compression
```

## Comparing `PySide6-Fluent-Widgets-1.5.4.tar` & `PySide6-Fluent-Widgets-1.5.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.621992 PySide6-Fluent-Widgets-1.5.4/
--rw-rw-rw-   0        0        0    35823 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     5183 2024-03-23 05:56:46.619769 PySide6-Fluent-Widgets-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.356802 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5183 2024-03-23 05:56:46.000000 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4929 2024-03-23 05:56:46.000000 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 05:56:46.000000 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-03-23 05:56:46.000000 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-23 05:56:46.000000 PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4399 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.362443 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/
--rw-rw-rw-   0        0        0      566 2024-03-23 05:51:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.366256 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3307370 2024-03-23 05:52:30.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.411842 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15208 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1589 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11172 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13725 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5554 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      664 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4862 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14413 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.413720 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.430020 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2329 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21813 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7630 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19331 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6406 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.445069 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14892 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5896 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11413 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3179 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2873 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2425 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.454916 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2716 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7104 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.474322 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3129 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3542 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6778 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1187 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1310 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.494736 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9884 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12954 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8771 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24105 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19604 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6823 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5205 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.513362 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5280 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11031 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4644 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2841 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14031 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.596473 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3316 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     7971 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    29945 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7688 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5808 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    16342 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19812 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7934 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13111 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17080 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2229 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1496 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16653 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18932 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14700 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    13969 2024-03-23 05:49:49.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4579 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40995 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11197 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9173 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7029 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2720 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17861 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1167 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10310 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8563 2024-03-23 05:55:20.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6535 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5854 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8597 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26330 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11774 2024-03-23 05:50:01.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22912 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10581 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4555 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.606269 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11597 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3887 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2849 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-03-23 05:56:46.618029 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      164 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12202 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2827 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1660 2024-03-23 05:49:50.000000 PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-03-23 05:56:46.621992 PySide6-Fluent-Widgets-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1219 2024-03-23 05:51:57.000000 PySide6-Fluent-Widgets-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.391186 PySide6-Fluent-Widgets-1.5.5/
+-rw-rw-rw-   0        0        0    35823 2024-04-13 06:31:05.000000 PySide6-Fluent-Widgets-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     5183 2024-04-13 06:40:11.390162 PySide6-Fluent-Widgets-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.188526 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5183 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4399 2024-04-13 06:31:05.000000 PySide6-Fluent-Widgets-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.190908 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/
+-rw-rw-rw-   0        0        0      566 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.194044 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3307370 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.230411 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15208 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1589 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11172 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13725 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5554 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      664 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4862 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14471 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.232893 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.242789 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2329 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21813 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7630 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19331 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6406 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.256229 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14892 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5896 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11413 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3179 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2873 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2425 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.263592 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2716 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7104 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.276958 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3129 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3542 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6778 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1187 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1310 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.293112 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9884 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12954 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8771 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24105 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    19679 2024-04-13 06:32:17.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6823 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5205 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.306148 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5280 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11031 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4644 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2841 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14031 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.372345 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3316 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     7971 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    29986 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7688 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5808 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    16342 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19812 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7934 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13111 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17080 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2229 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1496 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16653 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18932 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14700 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14221 2024-04-13 06:32:27.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4579 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40995 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11197 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9173 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7029 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2720 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17861 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1167 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10310 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8563 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6535 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5854 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8597 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26330 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11774 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22912 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10581 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4555 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.379368 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11597 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3887 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2849 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.386859 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12940 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2827 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1660 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 06:40:11.391186 PySide6-Fluent-Widgets-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2024-04-13 06:31:33.000000 PySide6-Fluent-Widgets-1.5.5/setup.py
```

### Comparing `PySide6-Fluent-Widgets-1.5.4/LICENSE` & `PySide6-Fluent-Widgets-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.4
+Version: 1.5.5
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.4 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.5 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.4
+Version: 1.5.5
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.4 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.5 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide6-Fluent-Widgets-1.5.4/PySide6_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/README.md` & `PySide6-Fluent-Widgets-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6/examples.
 
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

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/_rc/resource.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/animation.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/auto_wrap.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/color.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/config.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/exception_handler.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/font.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/icon.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/image_utils.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/overload.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/router.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/screen.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/smooth_scroll.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/common/style_sheet.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding:utf-8
 from enum import Enum
 from string import Template
 from typing import List, Union
 import weakref
 
-from PySide6.QtCore import QFile, QObject, QEvent
+from PySide6.QtCore import QFile, QObject, QEvent, QDynamicPropertyChangeEvent
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QWidget
 
 from .config import qconfig, Theme, isDarkTheme
 
 
 class StyleSheetManager(QObject):
@@ -208,15 +208,15 @@
 class CustomStyleSheetWatcher(QObject):
     """ Custom style sheet watcher """
 
     def eventFilter(self, obj: QWidget, e: QEvent):
         if e.type() != QEvent.DynamicPropertyChange:
             return super().eventFilter(obj, e)
 
-        name = e.propertyName().data().decode()
+        name = QDynamicPropertyChangeEvent(e).propertyName().data().decode()
         if name in [CustomStyleSheet.LIGHT_QSS_KEY, CustomStyleSheet.DARK_QSS_KEY]:
             addStyleSheet(obj, CustomStyleSheet(obj))
 
         return super().eventFilter(obj, e)
 
 
 class DirtyStyleSheetWatcher(QObject):
```

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/calendar_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/date_picker.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/picker_base.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/date_time/time_picker.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/dialog.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_box_base.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/expand_layout.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/flow_layout.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/layout/v_box_layout.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_combo_box.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_flyout.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_line_edit.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_menu.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/material/acrylic_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/breadcrumb.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding:utf-8
 from typing import Union, List
 
 from PySide6.QtCore import (Qt, Signal, QRect, QRectF, QPropertyAnimation, Property, QMargins,
-                          QEasingCurve, QPoint, QEvent, QSize)
+                          QEasingCurve, QPoint, QEvent)
 from PySide6.QtGui import QColor, QPainter, QPen, QIcon, QCursor, QFont, QBrush, QPixmap, QImage
 from PySide6.QtWidgets import QWidget, QVBoxLayout
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

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/pivot.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/options_setting_card.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/settings/setting_card_group.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/button.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/card_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/check_box.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/combo_box.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/command_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flip_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/flyout.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/frameless_window.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/icon_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_badge.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/info_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/label.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/line_edit.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,8 +423,15 @@
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
     passwordVisible = Property(bool, isPasswordVisible, setPasswordVisible)
```

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/list_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/menu.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/pips_pager.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/progress_ring.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_area.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/separator.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/slider.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/spin_box.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/switch_button.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tab_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/table_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tool_tip.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/components/widgets/tree_view.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_play_bar.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/media_player.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/multimedia/video_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/fluent_window.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/splash_screen.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/qfluentwidgets/window/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.4/setup.py` & `PySide6-Fluent-Widgets-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Fluent-Widgets",
-    version="1.5.4",
+    version="1.5.5",
     keywords="pyside6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

