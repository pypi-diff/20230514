# Comparing `tmp/magic_class-0.7.0rc0.tar.gz` & `tmp/magic_class-0.7.0rc1.tar.gz`

## Comparing `magic_class-0.7.0rc0.tar` & `magic_class-0.7.0rc1.tar`

### file list

```diff
@@ -1,132 +1,133 @@
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_app.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_register_types.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/command_palette.py
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/core.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/core.pyi
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/help.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/plot_api.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/signature.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/testing.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/undo.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/__init__.py
--rw-r--r--   0        0        0    46951 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_base.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_dock_widget.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_function_gui.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_gui_modes.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_icon.py
--rw-r--r--   0        0        0    21659 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_macro.py
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_macro_utils.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_message_box.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_napari_type.py
--rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/class_gui.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/keybinding.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/menu_gui.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/mgui_ext.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/runner.py
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/toolbar.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/_doc.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/_shared_utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/__init__.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/progress.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/resource.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/__init__.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/_magicgui.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/types.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/utils.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/viewer.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/widgets.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/tests/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/tests/test_viewer.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/tests/test_viewer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/_const.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/components.py
--rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/graph_items.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/mouse_event.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/plot_api.py
--rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/_qt.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/widgets.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/_base.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/camera.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layer2d.py
--rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layer3d.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layerlist.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/plot_api.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/widgets2d.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/widgets3d.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/tests/__init__.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/tests/test_vispy2d.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/__init__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/components.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/const.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/volume.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/widgets.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_define.py
--rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_fields.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_group.py
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_property.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/__init__.py
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_dispatch.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_partial.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_wraps.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/logging/__init__.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/logging/core.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/stylesheets/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_bound.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_choices.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_const.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_expr.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_optional.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_path.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_union.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/__init__.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_click.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_functions.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_recent.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qt.py
--rw-r--r--   0        0        0    31513 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qthreading.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qtsignal.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/__init__.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/_mpl_canvas.py
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/codeedit.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/color.py
--rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/containers.py
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/eval.py
--rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/logger.py
--rw-r--r--   0        0        0    18103 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/misc.py
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/plot.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/separator.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/toggle_switch.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/utils.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/__init__.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/dict.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/list.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/object.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/tests/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/tests/test_eval.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_abstractapi.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_confirm.py
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_misc.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_preview.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/LICENSE
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/README.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/pyproject.toml
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_app.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_register_types.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/command_palette.py
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/core.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/core.pyi
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/help.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/plot_api.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/signature.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/testing.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/undo.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/__init__.py
+-rw-r--r--   0        0        0    46952 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_base.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_dock_widget.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_function_gui.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_gui_modes.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_icon.py
+-rw-r--r--   0        0        0    21903 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_macro.py
+-rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_macro_utils.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_message_box.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_napari_type.py
+-rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/class_gui.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/keybinding.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/menu_gui.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/mgui_ext.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/runner.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/toolbar.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/_doc.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/_shared_utils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/__init__.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/progress.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/resource.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/_magicgui.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/types.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/utils.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/viewer.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/widgets.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/tests/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/tests/test_viewer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/__init__.py
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/tests/test_viewer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/_const.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/components.py
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/graph_items.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/mouse_event.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/plot_api.py
+-rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/_qt.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/widgets.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/_base.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/camera.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layer2d.py
+-rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layer3d.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layerlist.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/plot_api.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/widgets2d.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/widgets3d.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/tests/test_vispy2d.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/__init__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/components.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/const.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/volume.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/widgets.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_define.py
+-rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_fields.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_group.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_property.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/__init__.py
+-rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_dispatch.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_partial.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_wraps.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/logging/__init__.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/logging/core.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/stylesheets/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_bound.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_choices.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_const.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_expr.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_optional.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_path.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_union.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/__init__.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_click.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_functions.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_recent.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qt.py
+-rw-r--r--   0        0        0    31513 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qthreading.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qtsignal.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/__init__.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/_html.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/_mpl_canvas.py
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/codeedit.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/color.py
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/containers.py
+-rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/eval.py
+-rw-r--r--   0        0        0    19319 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/logger.py
+-rw-r--r--   0        0        0    18103 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/misc.py
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/plot.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/separator.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/toggle_switch.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/utils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/__init__.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/dict.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/list.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/object.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/tests/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/tests/test_eval.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_abstractapi.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_confirm.py
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_misc.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_preview.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/README.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/PKG-INFO
```

### Comparing `magic_class-0.7.0rc0/magicclass/__init__.py` & `magic_class-0.7.0rc1/magicclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0rc0"
+__version__ = "0.7.0rc1"
 
 from .core import (
     magicclass,
     magicmenu,
     magiccontext,
     magictoolbar,
     Parameters,
```

### Comparing `magic_class-0.7.0rc0/magicclass/_app.py` & `magic_class-0.7.0rc1/magicclass/_app.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_register_types.py` & `magic_class-0.7.0rc1/magicclass/_register_types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/command_palette.py` & `magic_class-0.7.0rc1/magicclass/command_palette.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/core.py` & `magic_class-0.7.0rc1/magicclass/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/core.pyi` & `magic_class-0.7.0rc1/magicclass/core.pyi`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/help.py` & `magic_class-0.7.0rc1/magicclass/help.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/plot_api.py` & `magic_class-0.7.0rc1/magicclass/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/signature.py` & `magic_class-0.7.0rc1/magicclass/signature.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/testing.py` & `magic_class-0.7.0rc1/magicclass/testing.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/undo.py` & `magic_class-0.7.0rc1/magicclass/undo.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_base.py` & `magic_class-0.7.0rc1/magicclass/_gui/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,19 +159,19 @@
 _F = TypeVar("_F", bound=Callable)
 
 
 class _MagicTemplateMeta(ABCMeta):
     """This metaclass enables type checking of nested magicclasses."""
 
     @overload
-    def __get__(self: type[_T], obj: Any, objtype=None) -> _T:
+    def __get__(self: type[_T], obj: MagicTemplate, objtype=None) -> _T:
         ...
 
     @overload
-    def __get__(self: type[_T], obj: Literal[None], objtype=None) -> type[_T]:
+    def __get__(self: type[_T], obj: None, objtype=None) -> type[_T]:
         ...
 
     def __get__(self, obj, objtype=None):
         return self
 
 
 _W = TypeVar("_W", bound=Widget)
```

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_dock_widget.py` & `magic_class-0.7.0rc1/magicclass/_gui/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_function_gui.py` & `magic_class-0.7.0rc1/magicclass/_gui/_function_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_gui_modes.py` & `magic_class-0.7.0rc1/magicclass/_gui/_gui_modes.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_icon.py` & `magic_class-0.7.0rc1/magicclass/_gui/_icon.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_macro.py` & `magic_class-0.7.0rc1/magicclass/_gui/_macro.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,72 +306,75 @@
         self._recorded_macro = None
 
     def _set_menubar(self):
         self._menubar = QtW.QMenuBar(self.native)
         self.native.layout().setMenuBar(self._menubar)
 
         # fmt: off
-        self._file_menu = QtW.QMenu("File", self.native)
-        self._file_menu.setToolTipsVisible(True)
-        self._menubar.addMenu(self._file_menu)
-
-        self._file_menu.addAction(_action("New window", self._new_window, tooltip="Open a new macro editor"))
-        self._file_menu.addSeparator()
-        self._file_menu.addAction(_action("Open file", self._load, "Ctrl+O", tooltip="Open a python file"))
-        self._file_menu.addAction(_action("Save", self._save, "Ctrl+S", tooltip="Save the macro as a python file"))
-        self._file_menu.addSeparator()
-        self._file_menu.addAction(_action("Close", self._close, tooltip="Close this macro editor"))
-
-        self._tab_menu = QtW.QMenu("Tab", self.native)
-        self._tab_menu.setToolTipsVisible(True)
-        self._menubar.addMenu(self._tab_menu)
-        self._tab_menu.addAction(_action("New tab", self._new_tab, "Ctrl+T", tooltip="Open a new empty tab"))
-        self._tab_menu.addAction(_action("Duplicate tab", self._duplicate_tab, "Ctrl+D", tooltip="Duplicate current tab as a new tab"))
-        self._tab_menu.addAction(_action("Current macro in new tab", self._create_native_duplicate, tooltip="Duplicate current GUI macro in a new tab"))
-        self._tab_menu.addAction(_action("Delete tab", self._delete_tab, "Ctrl+W", tooltip="Delete current tab"))
-        self._tab_menu.addSeparator()
-        self._tab_menu.addAction(_action("Zoom in", self._zoom_in, "Ctrl+Shift+.", tooltip="Zoom in the text"))
-        self._tab_menu.addAction(_action("Zoom out", self._zoom_out, "Ctrl+Shift+,", tooltip="Zoom out the text"))
+        _file_menu = QtW.QMenu("File", self.native)
+        _file_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(_file_menu)
+
+        _file_menu.addAction(_action("New window", self._new_window, tooltip="Open a new macro editor", parent=_file_menu))
+        _file_menu.addSeparator()
+        _file_menu.addAction(_action("Open file", self._load, "Ctrl+O", tooltip="Open a python file", parent=_file_menu))
+        _file_menu.addAction(_action("Save", self._save, "Ctrl+S", tooltip="Save the macro as a python file", parent=_file_menu))
+        _file_menu.addSeparator()
+        _file_menu.addAction(_action("Close", self._close, tooltip="Close this macro editor", parent=_file_menu))
+
+        _tab_menu = QtW.QMenu("Tab", self.native)
+        _tab_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(_tab_menu)
+        _tab_menu.addAction(_action("New tab", self._new_tab, "Ctrl+T", tooltip="Open a new empty tab", parent=_tab_menu))
+        _tab_menu.addAction(_action("Duplicate tab", self._duplicate_tab, "Ctrl+D", tooltip="Duplicate current tab as a new tab", parent=_tab_menu))
+        _tab_menu.addAction(_action("Current macro in new tab", self._create_native_duplicate, tooltip="Duplicate current GUI macro in a new tab", parent=_tab_menu))
+        _tab_menu.addAction(_action("Delete tab", self._delete_tab, "Ctrl+W", tooltip="Delete current tab", parent=_tab_menu))
+        _tab_menu.addSeparator()
+        _tab_menu.addAction(_action("Zoom in", self._zoom_in, "Ctrl+Shift+.", tooltip="Zoom in the text", parent=_tab_menu))
+        _tab_menu.addAction(_action("Zoom out", self._zoom_out, "Ctrl+Shift+,", tooltip="Zoom out the text", parent=_tab_menu))
 
 
         # set macro menu
-        self._macro_menu = QtW.QMenu("Macro", self.native)
-        self._macro_menu.setToolTipsVisible(True)
-        self._menubar.addMenu(self._macro_menu)
-
-        self._macro_menu.addAction(_action("Execute", self.execute, "Ctrl+F5", tooltip="Execute the entire script of the current tab"))
-        self._macro_menu.addAction(_action("Execute selected lines", self._execute_selected, "Ctrl+Shift+F5", tooltip="Execute the selected lines of the current tab"))
-        self._macro_menu.addSeparator()
-        _action_start = _action("Start recording", self._start_recording, tooltip="Open a new tab and start recording GUI operations in it")
-        self._macro_menu.addAction(_action_start)
-        _action_finish = _action("Finish recording", self._finish_recording, tooltip="Finish the recording task started by 'Start recording' menu")
-        self._macro_menu.addAction(_action_finish)
-
+        _macro_menu = QtW.QMenu("Macro", self.native)
+        _macro_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(_macro_menu)
+
+        _macro_menu.addAction(_action("Execute", self.execute, "Ctrl+F5", tooltip="Execute the entire script of the current tab", parent=_macro_menu))
+        _macro_menu.addAction(_action("Execute selected lines", self._execute_selected, "Ctrl+Shift+F5", tooltip="Execute the selected lines of the current tab", parent=_macro_menu))
+        _macro_menu.addSeparator()
+        _action_start = _action("Start recording", self._start_recording, tooltip="Open a new tab and start recording GUI operations in it", parent=_macro_menu)
+        _macro_menu.addAction(_action_start)
+        _action_finish = _action("Finish recording", self._finish_recording, tooltip="Finish the recording task started by 'Start recording' menu", parent=_macro_menu)
+        _macro_menu.addAction(_action_finish)
         _action_finish.setEnabled(False)
         _action_start.triggered.connect(lambda: _action_finish.setEnabled(True))
         _action_finish.triggered.connect(lambda: _action_finish.setEnabled(False))
 
         self._command_menu = CommandRunnerMenu(
             "Command",
             parent=self.native,
             magicclass_parent=self._search_parent_magicclass(),
         )
         self._command_menu.native.setToolTipsVisible(True)
         self._menubar.addMenu(self._command_menu.native)
-        self._command_menu.native.addAction(_action("Create command", self._create_command, tooltip="Create a command using the selected lines"))
-        self._command_menu.native.addAction(_action("Rename command", self._rename_command, tooltip="Rename regeistered commands."))
+        self._command_menu.native.addAction(_action("Create command", self._create_command, tooltip="Create a command using the selected lines", parent=self._command_menu.native))
+        self._command_menu.native.addAction(_action("Rename command", self._rename_command, tooltip="Rename regeistered commands.", parent=self._command_menu.native))
         self._command_menu.native.addSeparator()
         # fmt: on
 
 
 def _action(
-    text: str, slot: Callable, shortcut: str | None = None, tooltip: str | None = None
+    text: str,
+    slot: Callable,
+    shortcut: str | None = None,
+    tooltip: str | None = None,
+    parent=None,
 ):
     """Create a QAction object. Backend compatible."""
-    action = QtW.QAction(text)
+    action = QtW.QAction(text, parent=parent)
     action.triggered.connect(slot)
     if shortcut:
         action.setShortcut(shortcut)
     if tooltip:
         action.setToolTip(tooltip)
     return action
```

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_macro_utils.py` & `magic_class-0.7.0rc1/magicclass/_gui/_macro_utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_message_box.py` & `magic_class-0.7.0rc1/magicclass/_gui/_message_box.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/_napari_type.py` & `magic_class-0.7.0rc1/magicclass/_gui/_napari_type.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/class_gui.py` & `magic_class-0.7.0rc1/magicclass/_gui/class_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/keybinding.py` & `magic_class-0.7.0rc1/magicclass/_gui/keybinding.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/menu_gui.py` & `magic_class-0.7.0rc1/magicclass/_gui/menu_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/mgui_ext.py` & `magic_class-0.7.0rc1/magicclass/_gui/mgui_ext.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/runner.py` & `magic_class-0.7.0rc1/magicclass/_gui/runner.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/toolbar.py` & `magic_class-0.7.0rc1/magicclass/_gui/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from .menu_gui import ContextMenuGui, MenuGui, MenuGuiBase, insert_action_like
 from ._macro_utils import inject_recorder, nested_function_gui_callback
 
 from magicclass.signature import get_additional_option
 from magicclass.fields import MagicField
 from magicclass.widgets import FreeWidget, Separator
 from magicclass.utils import iter_members, Tooltips
-from magicclass.wrappers import abstractapi
 
 if TYPE_CHECKING:
     import napari
 
 
 def _check_popupmode(popup_mode: PopUpMode):
     if popup_mode in (PopUpMode.above, PopUpMode.below, PopUpMode.first):
```

### Comparing `magic_class-0.7.0rc0/magicclass/_gui/utils.py` & `magic_class-0.7.0rc1/magicclass/_gui/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/_doc.py` & `magic_class-0.7.0rc1/magicclass/ext/_doc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/dask/progress.py` & `magic_class-0.7.0rc1/magicclass/ext/dask/progress.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/dask/resource.py` & `magic_class-0.7.0rc1/magicclass/ext/dask/resource.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/napari/_magicgui.py` & `magic_class-0.7.0rc1/magicclass/ext/napari/_magicgui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/napari/types.py` & `magic_class-0.7.0rc1/magicclass/ext/napari/types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/napari/utils.py` & `magic_class-0.7.0rc1/magicclass/ext/napari/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/napari/viewer.py` & `magic_class-0.7.0rc1/magicclass/ext/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/napari/widgets.py` & `magic_class-0.7.0rc1/magicclass/ext/napari/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pandas/_viewer.py` & `magic_class-0.7.0rc1/magicclass/ext/pandas/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pandas/tests/test_viewer.py` & `magic_class-0.7.0rc1/magicclass/ext/pandas/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/polars/_viewer.py` & `magic_class-0.7.0rc1/magicclass/ext/polars/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/polars/tests/test_viewer.py` & `magic_class-0.7.0rc1/magicclass/ext/polars/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/__init__.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/components.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/graph_items.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/graph_items.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/mouse_event.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/mouse_event.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/plot_api.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/widgets.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/test_qtgraph.py` & `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/qtconsole/__init__.py` & `magic_class-0.7.0rc1/magicclass/ext/qtconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/qtconsole/_qt.py` & `magic_class-0.7.0rc1/magicclass/ext/qtconsole/_qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/qtconsole/widgets.py` & `magic_class-0.7.0rc1/magicclass/ext/qtconsole/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/_base.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/_base.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/camera.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/camera.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/layer2d.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/layer2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/layer3d.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/layer3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/layerlist.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/layerlist.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/plot_api.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/widgets2d.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/widgets2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/widgets3d.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/widgets3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vispy/tests/test_vispy2d.py` & `magic_class-0.7.0rc1/magicclass/ext/vispy/tests/test_vispy2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vtk/components.py` & `magic_class-0.7.0rc1/magicclass/ext/vtk/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vtk/const.py` & `magic_class-0.7.0rc1/magicclass/ext/vtk/const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vtk/volume.py` & `magic_class-0.7.0rc1/magicclass/ext/vtk/volume.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/ext/vtk/widgets.py` & `magic_class-0.7.0rc1/magicclass/ext/vtk/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/fields/_define.py` & `magic_class-0.7.0rc1/magicclass/fields/_define.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/fields/_fields.py` & `magic_class-0.7.0rc1/magicclass/fields/_fields.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/fields/_group.py` & `magic_class-0.7.0rc1/magicclass/fields/_group.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/fields/_property.py` & `magic_class-0.7.0rc1/magicclass/fields/_property.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/functools/_dispatch.py` & `magic_class-0.7.0rc1/magicclass/functools/_dispatch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/functools/_partial.py` & `magic_class-0.7.0rc1/magicclass/functools/_partial.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/functools/_wraps.py` & `magic_class-0.7.0rc1/magicclass/functools/_wraps.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/logging/core.py` & `magic_class-0.7.0rc1/magicclass/logging/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,18 @@
             arr, vmin=vmin, vmax=vmax, cmap=cmap, norm=norm, width=width, height=height
         )
 
     def print_figure(self, fig):
         """Print matplotlib Figure object like inline plot."""
         self._widget.print_figure(fig)
 
+    def print_link(self, text: str, href: str):
+        """Print a hypter link in the logger widget."""
+        self._widget.print_link(text, href)
+
     def set_stdout(self):
         """A context manager for printing things in this widget."""
         return self._widget.set_stdout()
 
     def set_logger(self, clear: bool = True):
         """A context manager for logging things in this widget."""
         return self._widget.set_logger(self.name, clear=clear)
```

### Comparing `magic_class-0.7.0rc0/magicclass/stylesheets/__init__.py` & `magic_class-0.7.0rc1/magicclass/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/__init__.py` & `magic_class-0.7.0rc1/magicclass/types/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_bound.py` & `magic_class-0.7.0rc1/magicclass/types/_bound.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_choices.py` & `magic_class-0.7.0rc1/magicclass/types/_choices.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_const.py` & `magic_class-0.7.0rc1/magicclass/types/_const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_expr.py` & `magic_class-0.7.0rc1/magicclass/types/_expr.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_optional.py` & `magic_class-0.7.0rc1/magicclass/types/_optional.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_path.py` & `magic_class-0.7.0rc1/magicclass/types/_path.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/types/_union.py` & `magic_class-0.7.0rc1/magicclass/types/_union.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/__init__.py` & `magic_class-0.7.0rc1/magicclass/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/_click.py` & `magic_class-0.7.0rc1/magicclass/utils/_click.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/_functions.py` & `magic_class-0.7.0rc1/magicclass/utils/_functions.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/_recent.py` & `magic_class-0.7.0rc1/magicclass/utils/_recent.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/qt.py` & `magic_class-0.7.0rc1/magicclass/utils/qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/utils/qthreading.py` & `magic_class-0.7.0rc1/magicclass/utils/qthreading.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/__init__.py` & `magic_class-0.7.0rc1/magicclass/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/_mpl_canvas.py` & `magic_class-0.7.0rc1/magicclass/widgets/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/codeedit.py` & `magic_class-0.7.0rc1/magicclass/widgets/codeedit.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/color.py` & `magic_class-0.7.0rc1/magicclass/widgets/color.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/containers.py` & `magic_class-0.7.0rc1/magicclass/widgets/containers.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/eval.py` & `magic_class-0.7.0rc1/magicclass/widgets/eval.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/logger.py` & `magic_class-0.7.0rc1/magicclass/widgets/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 import sys
 import logging
 from pathlib import Path
 from contextlib import contextmanager, suppress
+
 from qtpy import QtWidgets as QtW, QtGui, QtCore
 from qtpy.QtCore import Qt, Signal
 from magicgui.backends._qtpy.widgets import QBaseWidget
 from magicgui.widgets import Widget
 import logging
-from typing import TYPE_CHECKING, Any, Union, overload
+from typing import TYPE_CHECKING, Any, Union, overload, NamedTuple
 
 from magicclass.utils import rst_to_html
 
 if TYPE_CHECKING:
     import numpy as np
     from matplotlib.figure import Figure as mpl_Figure
 
@@ -46,17 +47,68 @@
 
 class Output:
     """Logger output types."""
 
     TEXT = 0
     HTML = 1
     IMAGE = 2
+    LINK = 3
+
+
+class linkedStr(NamedTuple):
+    text: str
+    link: str
+
+
+Printable = Union[str, QtGui.QImage, linkedStr]
+# HREF_PATTERN = re.compile(r"<a href=.+>.+</a>")
 
 
-Printable = Union[str, QtGui.QImage]
+class QFinderWidget(QtW.QWidget):
+    def __init__(self):
+        super().__init__()
+        _layout = QtW.QHBoxLayout(self)
+        _layout.setContentsMargins(2, 2, 2, 2)
+        self.setLayout(_layout)
+        _line = QtW.QLineEdit()
+        _btn_prev = QtW.QPushButton("▲")
+        _btn_next = QtW.QPushButton("▼")
+        _btn_prev.setFixedSize(20, 20)
+        _btn_next.setFixedSize(20, 20)
+        _layout.addWidget(_line)
+        _layout.addWidget(_btn_prev)
+        _layout.addWidget(_btn_next)
+        _btn_prev.clicked.connect(self._find_prev)
+        _btn_next.clicked.connect(self._find_next)
+        _line.editingFinished.connect(self._find_next)
+        self._line_edit = _line
+
+    if TYPE_CHECKING:
+
+        def parentWidget(self) -> QtLogger:
+            ...  # fmt: skip
+
+    def _find_prev(self):
+        qlogger = self.parentWidget()
+        flag = QtGui.QTextDocument.FindFlag.FindBackward
+        found = qlogger.find(self._line_edit.text(), flag)
+        if not found:
+            qlogger.moveCursor(QtGui.QTextCursor.MoveOperation.End)
+            exists = qlogger.find(self._line_edit.text(), flag)
+            if not exists:
+                QtW.QMessageBox.information(self, "Find", "No text matches.")
+
+    def _find_next(self):
+        qlogger = self.parentWidget()
+        found = qlogger.find(self._line_edit.text())
+        if not found:
+            qlogger.moveCursor(QtGui.QTextCursor.MoveOperation.Start)
+            exists = qlogger.find(self._line_edit.text())
+            if not exists:
+                QtW.QMessageBox.information(self, "Find", "No text matches.")
 
 
 class QtLogger(QtW.QTextEdit):
     process = Signal(tuple)
 
     def __init__(self, parent=None, max_history: int = 500):
         super().__init__(parent=parent)
@@ -71,14 +123,16 @@
         @self.customContextMenuRequested.connect
         def rightClickContextMenu(point):
             menu = self._make_contextmenu(point)
             if menu:
                 menu.exec_(self.mapToGlobal(point))
 
         self._last_save_path = None
+        self._finder_widget = None
+        self._anchor = None
 
     def update(self, output: tuple[int, Printable]):
         output_type, obj = output
         if output_type == Output.TEXT:
             self.moveCursor(QtGui.QTextCursor.MoveOperation.End)
             self.insertPlainText(obj)
             self.moveCursor(QtGui.QTextCursor.MoveOperation.End)
@@ -87,14 +141,23 @@
             self.insertHtml(obj)
             self.moveCursor(QtGui.QTextCursor.MoveOperation.End)
         elif output_type == Output.IMAGE:
             cursor = self.textCursor()
             cursor.insertImage(obj)
             self.insertPlainText("\n\n")
             self.verticalScrollBar().setValue(self.verticalScrollBar().maximum())
+        elif output_type == Output.LINK:
+            linkedstr = linkedStr(*obj)
+            cursor = self.textCursor()
+            linkFormat = cursor.charFormat()
+            linkFormat.setAnchor(True)
+            linkFormat.setAnchorHref(linkedstr.link)
+            linkFormat.setFontUnderline(True)
+            linkFormat.setForeground(QtGui.QBrush(QtGui.QColor("blue")))
+            cursor.insertText(linkedstr.text, linkFormat)
         else:
             raise TypeError("Wrong type.")
         self._post_append()
         return None
 
     def appendText(self, text: str):
         """Append text in the main thread."""
@@ -104,14 +167,18 @@
         """Append HTML in the main thread."""
         self._emit_output(Output.HTML, html)
 
     def appendImage(self, qimage: QtGui.QImage):
         """Append image in the main thread."""
         self._emit_output(Output.IMAGE, qimage)
 
+    def appendHref(self, text: str, link: str):
+        """Append link in the main thread."""
+        self._emit_output(Output.LINK, linkedStr(text, link))
+
     def _emit_output(self, output: int, obj: Printable):
         with suppress(RuntimeError):
             self.process.emit((output, obj))
 
     def _post_append(self):
         """Check the history length."""
         if self._n_lines < self._max_history:
@@ -131,22 +198,24 @@
         return self.palette().color(self.backgroundRole()).getRgb()
 
     # These methods below are modified from qtconsole.rich_jupyter_widget.py
 
     def _make_contextmenu(self, pos):
         """Reimplemented to return a custom context menu for images."""
         format = self.cursorForPosition(pos).charFormat()
-        name = format.stringProperty(QtGui.QTextFormat.Property.ImageName)
-        if name:
-            menu = QtW.QMenu(self)
-
+        menu = QtW.QMenu(self)
+        menu.addAction("Find ...", self._find_string)
+        menu.addAction("Export as HTML", self._export_as_html)
+        menu.addSeparator()
+        if name := format.stringProperty(QtGui.QTextFormat.Property.ImageName):
             menu.addAction("Copy Image", lambda: self._copy_image(name))
             menu.addAction("Save Image As...", lambda: self._save_image(name))
-            menu.addSeparator()
-            return menu
+        if name := format.stringProperty(QtGui.QTextFormat.Property.AnchorName):
+            menu.addAction("Copy Link", lambda: self._copy_link(name))
+        return menu
 
     def _copy_image(self, name):
         image = self._get_image(name)
         return QtW.QApplication.clipboard().setImage(image)
 
     def _save_image(self, name, format="PNG"):
         """Shows a save dialog for the ImageResource with 'name'."""
@@ -160,22 +229,57 @@
         if dialog.exec_():
             filename = dialog.selectedFiles()[0]
             image = self._get_image(name)
             image.save(filename, format)
             self._last_save_path = Path(filename).parent
         return None
 
+    def _find_string(self):
+        if self._finder_widget is None:
+            self._finder_widget = QFinderWidget()
+        self._finder_widget.setParent(self, self.windowFlags())
+        self._finder_widget.show()
+
+    def _export_as_html(self):
+        from ._html import HtmlExporter
+
+        HtmlExporter(self).export()
+
     def _get_image(self, name):
         """Returns the QImage stored as the ImageResource with 'name'."""
         document = self.document()
         image = document.resource(
             QtGui.QTextDocument.ResourceType.ImageResource, QtCore.QUrl(name)
         )
         return image
 
+    def mousePressEvent(self, e: QtGui.QMouseEvent):
+        self._anchor = self.anchorAt(e.pos())
+        self.viewport().setCursor(
+            Qt.CursorShape.PointingHandCursor
+            if self._anchor
+            else Qt.CursorShape.IBeamCursor
+        )
+        return super().mousePressEvent(e)
+
+    def mouseMoveEvent(self, e: QtGui.QMouseEvent) -> None:
+        super().mouseMoveEvent(e)
+        _anchor = self.anchorAt(e.pos())
+        self.viewport().setCursor(
+            Qt.CursorShape.PointingHandCursor if _anchor else Qt.CursorShape.IBeamCursor
+        )
+        return None
+
+    def mouseReleaseEvent(self, e: QtGui.QMouseEvent):
+        _anchor = self.anchorAt(e.pos())
+        if self._anchor == _anchor:
+            QtGui.QDesktopServices.openUrl(QtCore.QUrl(self._anchor))
+        self._anchor = None
+        return super().mouseReleaseEvent(e)
+
 
 class Logger(Widget, logging.Handler):
     """
     A widget for logging.
 
     Examples
     --------
@@ -340,14 +444,19 @@
             image = image.scaledToWidth(
                 width, Qt.TransformationMode.SmoothTransformation
             )
 
         self.native.appendImage(image)
         return None
 
+    def print_link(self, text: str, href: str):
+        """Print a link in the logger widget."""
+        self.native.appendHref(text, href)
+        return None
+
     def print_figure(self, fig: mpl_Figure) -> None:
         """Print matplotlib Figure object like inline plot."""
         import numpy as np
 
         fig.canvas.draw()
         data = np.asarray(fig.canvas.renderer.buffer_rgba(), dtype=np.uint8)
         self.print_image(data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/misc.py` & `magic_class-0.7.0rc1/magicclass/widgets/misc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/plot.py` & `magic_class-0.7.0rc1/magicclass/widgets/plot.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/separator.py` & `magic_class-0.7.0rc1/magicclass/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/toggle_switch.py` & `magic_class-0.7.0rc1/magicclass/widgets/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/utils.py` & `magic_class-0.7.0rc1/magicclass/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/__init__.py` & `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/dict.py` & `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/dict.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/list.py` & `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/list.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/object.py` & `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/object.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/tree.py` & `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/tree.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/wrappers/__init__.py` & `magic_class-0.7.0rc1/magicclass/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/wrappers/_abstractapi.py` & `magic_class-0.7.0rc1/magicclass/wrappers/_abstractapi.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/wrappers/_confirm.py` & `magic_class-0.7.0rc1/magicclass/wrappers/_confirm.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/wrappers/_misc.py` & `magic_class-0.7.0rc1/magicclass/wrappers/_misc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/magicclass/wrappers/_preview.py` & `magic_class-0.7.0rc1/magicclass/wrappers/_preview.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/.gitignore` & `magic_class-0.7.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/LICENSE` & `magic_class-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/README.md` & `magic_class-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/pyproject.toml` & `magic_class-0.7.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc0/PKG-INFO` & `magic_class-0.7.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-class
-Version: 0.7.0rc0
+Version: 0.7.0rc1
 Summary: Generate multifunctional GUIs from classes
 Project-URL: Download, https://github.com/hanjinliu/magic-class
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
```

