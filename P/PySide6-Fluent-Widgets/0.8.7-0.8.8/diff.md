# Comparing `tmp/PySide6-Fluent-Widgets-0.8.7.tar.gz` & `tmp/PySide6-Fluent-Widgets-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Fluent-Widgets-0.8.7.tar", last modified: Wed May 10 06:17:11 2023, max compression
+gzip compressed data, was "dist\PySide6-Fluent-Widgets-0.8.8.tar", last modified: Sun May 14 14:32:04 2023, max compression
```

## Comparing `PySide6-Fluent-Widgets-0.8.7.tar` & `PySide6-Fluent-Widgets-0.8.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.588488 PySide6-Fluent-Widgets-0.8.7/
--rw-rw-rw-   0        0        0     7815 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/LICENSE
--rw-rw-rw-   0        0        0     3604 2023-05-10 06:17:11.586981 PySide6-Fluent-Widgets-0.8.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.465072 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     3604 2023-05-10 06:17:11.000000 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3259 2023-05-10 06:17:11.000000 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 06:17:11.000000 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-05-10 06:17:11.000000 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 06:17:11.000000 PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2785 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.467344 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/
--rw-rw-rw-   0        0        0      502 2023-05-10 03:31:14.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.470895 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5113609 2023-05-10 03:36:39.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.497258 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      440 2023-04-28 08:31:54.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10580 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     8794 2023-05-10 03:31:14.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4785 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     4862 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7052 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2023-05-10 03:31:14.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.499775 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.506889 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     7464 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19071 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5675 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.517744 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14828 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5392 2023-05-10 03:43:03.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11413 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3244 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2425 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.524751 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.531433 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    16710 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0     4873 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_widget.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.544175 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5314 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8036 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6028 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2838 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13114 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1516 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:17:11.585983 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     1492 2023-05-10 03:31:14.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4596 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    13941 2023-05-10 03:39:10.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     1615 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13562 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7934 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     1327 2023-05-10 03:33:28.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18492 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0      845 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     5548 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3983 2023-05-10 03:34:05.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    23753 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7288 2023-05-10 03:37:48.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1875 2023-05-10 03:40:23.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2451 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17679 2023-05-10 03:31:14.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5266 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4631 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6335 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5854 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8931 2023-05-10 03:34:26.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     9123 2023-05-10 03:36:02.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    10402 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2194 2023-05-10 03:30:43.000000 PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tree_view.py
--rw-rw-rw-   0        0        0       42 2023-05-10 06:17:11.589012 PySide6-Fluent-Widgets-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1269 2023-05-10 03:31:37.000000 PySide6-Fluent-Widgets-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.099609 PySide6-Fluent-Widgets-0.8.8/
+-rw-rw-rw-   0        0        0     7815 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     3604 2023-05-14 14:32:04.098248 PySide6-Fluent-Widgets-0.8.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:03.955650 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     3604 2023-05-14 14:32:03.000000 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3259 2023-05-14 14:32:03.000000 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:32:03.000000 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-14 14:32:03.000000 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 14:32:03.000000 PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2785 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:03.957656 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/
+-rw-rw-rw-   0        0        0      502 2023-05-14 14:16:32.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:03.961656 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5113609 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:03.998935 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      440 2023-04-28 08:31:54.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10580 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0     8794 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4785 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     4862 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7052 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.000944 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.007894 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     7464 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19071 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5675 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.017547 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14828 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5363 2023-05-14 14:30:28.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11413 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3244 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2425 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.024589 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.030530 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     4843 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    16710 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0     4873 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_widget.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.044296 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5314 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8036 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6028 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2838 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13114 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1516 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:32:04.097251 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     1492 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    13941 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     1615 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13620 2023-05-14 14:16:32.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7934 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     1327 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18492 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0      845 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     5617 2023-05-14 14:16:32.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3983 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    23753 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7288 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1875 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2451 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17679 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5266 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4631 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6335 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5854 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8931 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     9123 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    10402 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2194 2023-05-14 14:16:18.000000 PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tree_view.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:32:04.099609 PySide6-Fluent-Widgets-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-05-14 14:17:26.000000 PySide6-Fluent-Widgets-0.8.8/setup.py
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/LICENSE` & `PySide6-Fluent-Widgets-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/PKG-INFO` & `PySide6-Fluent-Widgets-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 0.8.7
+Version: 0.8.8
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/PKG-INFO` & `PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 0.8.7
+Version: 0.8.8
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/PySide6_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide6-Fluent-Widgets-0.8.8/PySide6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/README.md` & `PySide6-Fluent-Widgets-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/resource.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/animation.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/auto_wrap.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/config.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/exception_handler.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/icon.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/image_utils.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/overload.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/smooth_scroll.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/common/style_sheet.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/date_picker.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/picker_base.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/time_picker.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/dialog.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class Ui_MessageBox:
     """ Ui of message box """
 
     yesSignal = Signal()
     cancelSignal = Signal()
 
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        pass
 
     def _setUpUi(self, title, content, parent):
         self.content = content
         self.titleLabel = QLabel(title, parent)
         self.contentLabel = QLabel(content, parent)
 
         self.buttonGroup = QFrame(parent)
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/expand_layout.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/flow_layout.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/v_box_layout.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/__init__.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/options_setting_card.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card_group.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/__init__.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/button.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/check_box.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/combo_box.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/combo_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,14 +373,17 @@
         self.returnPressed.connect(self._onReturnPressed)
 
         FluentStyleSheet.LINE_EDIT.apply(self)
 
     def currentText(self):
         return self.text()
 
+    def clear(self):
+        ComboBoxBase.clear(self)
+
     def _onReturnPressed(self):
         if not self.text():
             return
 
         index = self.findText(self.text())
         if index >= 0 and index != self.currentIndex():
             self._currentIndex = index
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/icon_widget.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/info_bar.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/label.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/line_edit.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/line_edit.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,20 +107,21 @@
         if not self.hasFocus():
             return
 
         painter = QPainter(self)
         painter.setRenderHints(QPainter.Antialiasing)
         painter.setPen(Qt.NoPen)
 
+        m = self.contentsMargins()
         path = QPainterPath()
-        w, h = self.width(), self.height()
-        path.addRoundedRect(QRectF(0, h-10, w, 10), 5, 5)
+        w, h = self.width()-m.left()-m.right(), self.height()
+        path.addRoundedRect(QRectF(m.left(), h-10, w, 10), 5, 5)
 
         rectPath = QPainterPath()
-        rectPath.addRect(0, h-10, w, 8)
+        rectPath.addRect(m.left(), h-10, w, 8)
         path = path.subtracted(rectPath)
 
         painter.fillPath(path, themeColor())
 
 
 class SearchLineEdit(LineEdit):
     """ Search line edit """
```

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/list_view.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/menu.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_bar.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_ring.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_area.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/slider.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/spin_box.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/switch_button.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/table_view.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tool_tip.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tree_view.py` & `PySide6-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.8.7/setup.py` & `PySide6-Fluent-Widgets-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Fluent-Widgets",
-    version="0.8.7",
+    version="0.8.8",
     keywords="pyside6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

