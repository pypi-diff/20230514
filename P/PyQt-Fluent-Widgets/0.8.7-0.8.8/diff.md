# Comparing `tmp/PyQt-Fluent-Widgets-0.8.7.tar.gz` & `tmp/PyQt-Fluent-Widgets-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.8.7.tar", last modified: Wed May 10 03:28:43 2023, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.8.8.tar", last modified: Sun May 14 14:02:15 2023, max compression
```

## Comparing `PyQt-Fluent-Widgets-0.8.7.tar` & `PyQt-Fluent-Widgets-0.8.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.623346 PyQt-Fluent-Widgets-0.8.7/
--rw-rw-rw-   0        0        0    35823 2023-05-07 08:43:45.000000 PyQt-Fluent-Widgets-0.8.7/LICENSE
--rw-rw-rw-   0        0        0     4982 2023-05-10 03:28:43.622345 PyQt-Fluent-Widgets-0.8.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.501651 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4982 2023-05-10 03:28:43.000000 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3244 2023-05-10 03:28:43.000000 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:28:43.000000 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-10 03:28:43.000000 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 03:28:43.000000 PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4206 2023-05-10 03:27:45.000000 PyQt-Fluent-Widgets-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.503821 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/
--rw-rw-rw-   0        0        0      492 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.506355 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5113607 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.533968 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      440 2023-04-28 08:31:54.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10596 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     8814 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4783 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     4851 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7046 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.534975 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.541793 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     7455 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19077 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.553454 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14724 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5327 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11337 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3238 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2500 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.560190 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5433 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.566683 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     4845 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    16716 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0     4875 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_widget.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.579509 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8027 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6034 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13119 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1512 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:28:43.620219 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     1504 2023-05-10 02:05:16.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4598 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    13971 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     1609 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13109 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7881 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     1329 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18494 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0      835 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     5542 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4204 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    23712 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7314 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1866 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2449 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17705 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5132 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4625 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6334 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8973 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8903 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    10384 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2150 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tree_view.py
--rw-rw-rw-   0        0        0       42 2023-05-10 03:28:43.623346 PyQt-Fluent-Widgets-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-05-10 03:05:37.000000 PyQt-Fluent-Widgets-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.301430 PyQt-Fluent-Widgets-0.8.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-11 05:36:47.000000 PyQt-Fluent-Widgets-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     4982 2023-05-14 14:02:15.301430 PyQt-Fluent-Widgets-0.8.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.176886 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4982 2023-05-14 14:02:14.000000 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3244 2023-05-14 14:02:15.000000 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:02:14.000000 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-14 14:02:14.000000 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 14:02:14.000000 PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4206 2023-05-11 14:18:13.000000 PyQt-Fluent-Widgets-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.178892 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/
+-rw-rw-rw-   0        0        0      492 2023-05-14 13:58:20.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.182445 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5113607 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.209213 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      440 2023-04-28 08:31:54.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10596 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0     8814 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4783 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-04-23 05:13:06.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     4851 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7046 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.211418 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.218021 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     7455 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19077 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.228814 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14724 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5327 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11337 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3238 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2500 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.236329 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5433 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.243331 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     4845 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    16716 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0     4875 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_widget.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.256602 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5316 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8027 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6034 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13119 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1512 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:02:15.299431 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     1504 2023-05-11 05:36:49.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4598 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    13971 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     1609 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13167 2023-05-14 13:21:44.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7881 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     1329 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18494 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0      835 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     5611 2023-05-14 13:37:21.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4204 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    23712 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7314 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1866 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2449 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17705 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5132 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4625 2023-05-14 13:50:25.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6334 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8973 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8903 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    10384 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2150 2023-05-11 14:18:14.000000 PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tree_view.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:02:15.302432 PyQt-Fluent-Widgets-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-05-14 13:58:15.000000 PyQt-Fluent-Widgets-0.8.8/setup.py
```

### Comparing `PyQt-Fluent-Widgets-0.8.7/LICENSE` & `PyQt-Fluent-Widgets-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/PKG-INFO` & `PyQt-Fluent-Widgets-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.8.7
+Version: 0.8.8
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.8.7 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.8.8 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.8.7
+Version: 0.8.8
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.8.7 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.8.8 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `PyQt-Fluent-Widgets-0.8.7/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-0.8.8/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/README.md` & `PyQt-Fluent-Widgets-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/animation.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/overload.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/check_box.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/combo_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,14 +369,17 @@
         self.dropButton.clicked.connect(self._toggleComboMenu)
         self.textEdited.connect(self._onTextEdited)
         self.returnPressed.connect(self._onReturnPressed)
 
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

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/line_edit.py`

 * *Files 2% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/list_view.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/table_view.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-0.8.8/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.8.7/setup.py` & `PyQt-Fluent-Widgets-0.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="0.8.7",
+    version="0.8.8",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

