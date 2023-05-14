# Comparing `tmp/nicegui-1.2.8.tar.gz` & `tmp/nicegui-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegui-1.2.8.tar", max compression
+gzip compressed data, was "nicegui-1.2.9.tar", max compression
```

## Comparing `nicegui-1.2.8.tar` & `nicegui-1.2.9.tar`

### file list

```diff
@@ -1,416 +1,421 @@
--rw-r--r--   0        0        0     1072 2023-04-17 09:38:33.882799 nicegui-1.2.8/LICENSE
--rw-r--r--   0        0        0     5751 2023-04-17 09:38:33.882799 nicegui-1.2.8/README.md
--rw-r--r--   0        0        0      288 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/__init__.py
--rw-r--r--   0        0        0     3118 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/app.py
--rw-r--r--   0        0        0     2056 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/background_tasks.py
--rw-r--r--   0        0        0     4599 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/binding.py
--rw-r--r--   0        0        0     6050 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/client.py
--rw-r--r--   0        0        0     1291 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/colors.py
--rw-r--r--   0        0        0     3030 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/dependencies.py
--rw-r--r--   0        0        0      457 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/deprecation.py
--rw-r--r--   0        0        0    11039 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/element.py
--rw-r--r--   0        0        0     2958 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/aggrid.js
--rw-r--r--   0        0        0     2975 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/aggrid.py
--rw-r--r--   0        0        0      212 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/audio.js
--rw-r--r--   0        0        0     1487 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/audio.py
--rw-r--r--   0        0        0     1827 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/avatar.py
--rw-r--r--   0        0        0     1095 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/badge.py
--rw-r--r--   0        0        0     1454 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/button.py
--rw-r--r--   0        0        0     1124 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/card.py
--rw-r--r--   0        0        0      990 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/chart.js
--rw-r--r--   0        0        0     4840 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/chart.py
--rw-r--r--   0        0        0      622 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/checkbox.py
--rw-r--r--   0        0        0     1075 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/choice_element.py
--rw-r--r--   0        0        0     1361 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/color_input.py
--rw-r--r--   0        0        0      915 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/color_picker.py
--rw-r--r--   0        0        0      335 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/colors.js
--rw-r--r--   0        0        0     1062 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/colors.py
--rw-r--r--   0        0        0      269 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/column.py
--rw-r--r--   0        0        0     1216 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/date.py
--rw-r--r--   0        0        0     1441 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/dialog.py
--rw-r--r--   0        0        0      782 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/expansion.py
--rw-r--r--   0        0        0      543 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/html.py
--rw-r--r--   0        0        0      947 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/icon.py
--rw-r--r--   0        0        0      321 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/image.py
--rw-r--r--   0        0        0     2830 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/input.py
--rw-r--r--   0        0        0     2004 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/interactive_image.js
--rw-r--r--   0        0        0     2600 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/interactive_image.py
--rw-r--r--   0        0        0     2370 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/joystick.py
--rw-r--r--   0        0        0      622 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/joystick.vue
--rw-r--r--   0        0        0      792 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/keyboard.js
--rw-r--r--   0        0        0     2397 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/keyboard.py
--rw-r--r--   0        0        0     2246 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/knob.py
--rw-r--r--   0        0        0      274 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/label.py
--rw-r--r--   0        0        0     4673 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/lib/CSS2DRenderer.js
--rw-r--r--   0        0        0     8988 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/lib/CSS3DRenderer.js
--rw-r--r--   0        0        0    29354 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/lib/OrbitControls.js
--rw-r--r--   0        0        0    10612 2023-04-17 09:38:33.898800 nicegui-1.2.8/nicegui/elements/lib/STLLoader.js
--rw-r--r--   0        0        0  1570067 2023-04-17 09:38:33.906801 nicegui-1.2.8/nicegui/elements/lib/ag-grid-community.min.js
--rw-r--r--   0        0        0    49248 2023-04-17 09:38:33.906801 nicegui-1.2.8/nicegui/elements/lib/highcharts-3d.js
--rw-r--r--   0        0        0   106326 2023-04-17 09:38:33.906801 nicegui-1.2.8/nicegui/elements/lib/highcharts-more.js
--rw-r--r--   0        0        0   303628 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts.js
--rw-r--r--   0        0        0   130976 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/accessibility.js
--rw-r--r--   0        0        0    98853 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/annotations-advanced.js
--rw-r--r--   0        0        0    65315 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/annotations.js
--rw-r--r--   0        0        0     7406 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/arc-diagram.js
--rw-r--r--   0        0        0     1211 2023-04-17 09:38:33.910801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/arrow-symbols.js
--rw-r--r--   0        0        0    43377 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/boost-canvas.js
--rw-r--r--   0        0        0    47427 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/boost.js
--rw-r--r--   0        0        0     5884 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/broken-axis.js
--rw-r--r--   0        0        0     4029 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/bullet.js
--rw-r--r--   0        0        0    12125 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/coloraxis.js
--rw-r--r--   0        0        0     1770 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/current-date-indicator.js
--rw-r--r--   0        0        0     5056 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/cylinder.js
--rw-r--r--   0        0        0    16507 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/data.js
--rw-r--r--   0        0        0    11360 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/datagrouping.js
--rw-r--r--   0        0        0    15051 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/debugger.js
--rw-r--r--   0        0        0     5733 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dependency-wheel.js
--rw-r--r--   0        0        0     2652 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dotplot.js
--rw-r--r--   0        0        0     4560 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/drag-panes.js
--rw-r--r--   0        0        0    17196 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/draggable-points.js
--rw-r--r--   0        0        0    18352 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/drilldown.js
--rw-r--r--   0        0        0     8141 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dumbbell.js
--rw-r--r--   0        0        0    12791 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/export-data.js
--rw-r--r--   0        0        0    19692 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/exporting.js
--rw-r--r--   0        0        0     3491 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/full-screen.js
--rw-r--r--   0        0        0     5606 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/funnel.js
--rw-r--r--   0        0        0    10167 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/funnel3d.js
--rw-r--r--   0        0        0   112925 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/gantt.js
--rw-r--r--   0        0        0    11206 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/grid-axis.js
--rw-r--r--   0        0        0    19983 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/heatmap.js
--rw-r--r--   0        0        0     3869 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/heikinashi.js
--rw-r--r--   0        0        0     6199 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js
--rw-r--r--   0        0        0     3983 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js
--rw-r--r--   0        0        0     5636 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/item-series.js
--rw-r--r--   0        0        0     3063 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/lollipop.js
--rw-r--r--   0        0        0    17955 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/marker-clusters.js
--rw-r--r--   0        0        0    27952 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/networkgraph.js
--rw-r--r--   0        0        0     1947 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/no-data-to-display.js
--rw-r--r--   0        0        0     9627 2023-04-17 09:38:33.914801 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/offline-exporting.js
--rw-r--r--   0        0        0     3042 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js
--rw-r--r--   0        0        0    14679 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/oldie.js
--rw-r--r--   0        0        0     8553 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/organization.js
--rw-r--r--   0        0        0      741 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js
--rw-r--r--   0        0        0     5234 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js
--rw-r--r--   0        0        0     3180 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pareto.js
--rw-r--r--   0        0        0    15251 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pathfinder.js
--rw-r--r--   0        0        0     7026 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pattern-fill.js
--rw-r--r--   0        0        0     2151 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/price-indicator.js
--rw-r--r--   0        0        0     1640 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pyramid3d.js
--rw-r--r--   0        0        0    16340 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sankey.js
--rw-r--r--   0        0        0     9424 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/series-label.js
--rw-r--r--   0        0        0     3792 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/series-on-point.js
--rw-r--r--   0        0        0     4944 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/solid-gauge.js
--rw-r--r--   0        0        0    29682 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sonification.js
--rw-r--r--   0        0        0     1837 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/static-scale.js
--rw-r--r--   0        0        0    55798 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/stock-tools.js
--rw-r--r--   0        0        0   108215 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/stock.js
--rw-r--r--   0        0        0     1698 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/streamgraph.js
--rw-r--r--   0        0        0    37904 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sunburst.js
--rw-r--r--   0        0        0     8257 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/tilemap.js
--rw-r--r--   0        0        0     8804 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/timeline.js
--rw-r--r--   0        0        0    18184 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treegraph.js
--rw-r--r--   0        0        0    28748 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treegrid.js
--rw-r--r--   0        0        0    27334 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treemap.js
--rw-r--r--   0        0        0     4254 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/variable-pie.js
--rw-r--r--   0        0        0     5739 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/variwide.js
--rw-r--r--   0        0        0     3265 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/vector.js
--rw-r--r--   0        0        0    15068 2023-04-17 09:38:33.918802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/venn.js
--rw-r--r--   0        0        0     7390 2023-04-17 09:38:33.922802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/windbarb.js
--rw-r--r--   0        0        0    11231 2023-04-17 09:38:33.922802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/wordcloud.js
--rw-r--r--   0        0        0     8508 2023-04-17 09:38:33.922802 nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/xrange.js
--rw-r--r--   0        0        0  2777841 2023-04-17 09:38:33.938803 nicegui-1.2.8/nicegui/elements/lib/mermaid.min.js
--rw-r--r--   0        0        0    20547 2023-04-17 09:38:33.938803 nicegui-1.2.8/nicegui/elements/lib/nipplejs.min.js
--rw-r--r--   0        0        0  3579005 2023-04-17 09:38:33.962805 nicegui-1.2.8/nicegui/elements/lib/plotly.min.js
--rw-r--r--   0        0        0   613740 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/lib/three.min.js
--rw-r--r--   0        0        0    10633 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/lib/tween.umd.min.js
--rw-r--r--   0        0        0     2298 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/line_plot.py
--rw-r--r--   0        0        0      533 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/link.js
--rw-r--r--   0        0        0     1395 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/link.py
--rw-r--r--   0        0        0      997 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/log.js
--rw-r--r--   0        0        0     1168 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/log.py
--rw-r--r--   0        0        0      933 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/markdown.js
--rw-r--r--   0        0        0     2701 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/markdown.py
--rw-r--r--   0        0        0     1593 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/menu.py
--rw-r--r--   0        0        0      274 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mermaid.js
--rw-r--r--   0        0        0      861 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mermaid.py
--rw-r--r--   0        0        0     3327 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/content_element.py
--rw-r--r--   0        0        0     3131 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/filter_element.py
--rw-r--r--   0        0        0     3055 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/source_element.py
--rw-r--r--   0        0        0     3058 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/text_element.py
--rw-r--r--   0        0        0     4204 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/value_element.py
--rw-r--r--   0        0        0     3850 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/mixins/visibility.py
--rw-r--r--   0        0        0     2475 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/number.py
--rw-r--r--   0        0        0     2047 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/plotly.py
--rw-r--r--   0        0        0     2622 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/plotly.vue
--rw-r--r--   0        0        0     2741 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/progress.py
--rw-r--r--   0        0        0     1471 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/pyplot.py
--rw-r--r--   0        0        0     1158 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/query.js
--rw-r--r--   0        0        0     2751 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/query.py
--rw-r--r--   0        0        0     1021 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/radio.py
--rw-r--r--   0        0        0      257 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/row.py
--rw-r--r--   0        0        0    13006 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/scene.js
--rw-r--r--   0        0        0     5765 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/scene.py
--rw-r--r--   0        0        0     4047 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/scene_object3d.py
--rw-r--r--   0        0        0     5066 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/scene_objects.py
--rw-r--r--   0        0        0      924 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/select.js
--rw-r--r--   0        0        0     2065 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/select.py
--rw-r--r--   0        0        0      280 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/separator.py
--rw-r--r--   0        0        0      852 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/slider.py
--rw-r--r--   0        0        0     1461 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/spinner.py
--rw-r--r--   0        0        0     1704 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/splitter.py
--rw-r--r--   0        0        0      634 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/switch.py
--rw-r--r--   0        0        0     3281 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/table.py
--rw-r--r--   0        0        0     2867 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/tabs.py
--rw-r--r--   0        0        0     1125 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/textarea.py
--rw-r--r--   0        0        0      813 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/time.py
--rw-r--r--   0        0        0     1019 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/toggle.py
--rw-r--r--   0        0        0      335 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/tooltip.py
--rw-r--r--   0        0        0     2634 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/tree.py
--rw-r--r--   0        0        0     2827 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/upload.py
--rw-r--r--   0        0        0      212 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/video.js
--rw-r--r--   0        0        0     1487 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/elements/video.py
--rw-r--r--   0        0        0     1046 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/error.py
--rw-r--r--   0        0        0     1102 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/event_listener.py
--rw-r--r--   0        0        0     6093 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/events.py
--rw-r--r--   0        0        0     1987 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/favicon.py
--rw-r--r--   0        0        0      384 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/download.py
--rw-r--r--   0        0        0      203 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/html.py
--rw-r--r--   0        0        0     1230 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/javascript.py
--rw-r--r--   0        0        0     1408 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/notify.py
--rw-r--r--   0        0        0      669 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/open.py
--rw-r--r--   0        0        0     3992 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/timer.py
--rw-r--r--   0        0        0      126 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/functions/update.py
--rw-r--r--   0        0        0     2262 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/globals.py
--rw-r--r--   0        0        0     2900 2023-04-17 09:38:33.966805 nicegui-1.2.8/nicegui/helpers.py
--rw-r--r--   0        0        0      387 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/ids.py
--rw-r--r--   0        0        0      788 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/json/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/json/builtin_wrapper.py
--rw-r--r--   0        0        0     1758 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/json/orjson_wrapper.py
--rw-r--r--   0        0        0      220 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/native.py
--rw-r--r--   0        0        0     2074 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/native_mode.py
--rw-r--r--   0        0        0     6390 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/nicegui.py
--rw-r--r--   0        0        0     1609 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/outbox.py
--rw-r--r--   0        0        0     4378 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/page.py
--rw-r--r--   0        0        0     8064 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/page_layout.py
--rw-r--r--   0        0        0     5972 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/run.py
--rw-r--r--   0        0        0      895 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/run_with.py
--rw-r--r--   0        0        0      611 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/slot.py
--rw-r--r--   0        0        0    15086 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/favicon.ico
--rw-r--r--   0        0        0      756 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0    10144 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     7668 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     3360 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0    10972 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2
--rw-r--r--   0        0        0     4960 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     6384 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2
--rw-r--r--   0        0        0     6632 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11072 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4796 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      768 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10352 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7676 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3472 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6480 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11160 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4928 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      756 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10412 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7840 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3448 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6620 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    11040 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4796 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      756 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10256 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7676 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3468 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     6612 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10992 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2
--rw-r--r--   0        0        0     4756 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0      772 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2
--rw-r--r--   0        0        0    10188 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     7608 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     3388 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2
--rw-r--r--   0        0        0     4864 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0    11028 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2
--rw-r--r--   0        0        0     6460 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0    10352 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2
--rw-r--r--   0        0        0     7736 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0     3496 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0      748 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2
--rw-r--r--   0        0        0   128616 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0        0        0    11484 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/fonts.css
--rw-r--r--   0        0        0     1913 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/nicegui.css
--rw-r--r--   0        0        0   198973 2023-04-17 09:38:33.970806 nicegui-1.2.8/nicegui/static/quasar.prod.css
--rw-r--r--   0        0        0   509631 2023-04-17 09:38:33.974806 nicegui-1.2.8/nicegui/static/quasar.umd.prod.js
--rw-r--r--   0        0        0     1510 2023-04-17 09:38:33.974806 nicegui-1.2.8/nicegui/static/sad_face.svg
--rw-r--r--   0        0        0    45896 2023-04-17 09:38:33.974806 nicegui-1.2.8/nicegui/static/socket.io.min.js
--rw-r--r--   0        0        0   350399 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/static/tailwindcss.min.js
--rw-r--r--   0        0        0   128872 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/static/vue.global.prod.js
--rw-r--r--   0        0        0   107302 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/static/vue.min.js
--rw-r--r--   0        0        0    44035 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind.py
--rw-r--r--   0        0        0     4232 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/accent_color.py
--rw-r--r--   0        0        0      191 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/align_content.py
--rw-r--r--   0        0        0      132 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/align_items.py
--rw-r--r--   0        0        0      143 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/align_self.py
--rw-r--r--   0        0        0      125 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/animation.py
--rw-r--r--   0        0        0       75 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/appearance.py
--rw-r--r--   0        0        0      103 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/aspect_ratio.py
--rw-r--r--   0        0        0      147 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_blur.py
--rw-r--r--   0        0        0      186 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_brightness.py
--rw-r--r--   0        0        0      142 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_contrast.py
--rw-r--r--   0        0        0       87 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_grayscale.py
--rw-r--r--   0        0        0      130 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_hue_rotate.py
--rw-r--r--   0        0        0       84 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_invert.py
--rw-r--r--   0        0        0      217 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_opacity.py
--rw-r--r--   0        0        0      121 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_saturate.py
--rw-r--r--   0        0        0       83 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/backdrop_sepia.py
--rw-r--r--   0        0        0      113 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_attachment.py
--rw-r--r--   0        0        0      328 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_blend_mode.py
--rw-r--r--   0        0        0      123 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_clip.py
--rw-r--r--   0        0        0     4224 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_color.py
--rw-r--r--   0        0        0      252 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_image.py
--rw-r--r--   0        0        0      113 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_origin.py
--rw-r--r--   0        0        0      207 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_position.py
--rw-r--r--   0        0        0      172 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_repeat.py
--rw-r--r--   0        0        0      107 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/background_size.py
--rw-r--r--   0        0        0      139 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/blur.py
--rw-r--r--   0        0        0       99 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_collapse.py
--rw-r--r--   0        0        0    41420 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_color.py
--rw-r--r--   0        0        0     1785 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_radius.py
--rw-r--r--   0        0        0     1238 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_spacing.py
--rw-r--r--   0        0        0      145 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_style.py
--rw-r--r--   0        0        0      532 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/border_width.py
--rw-r--r--   0        0        0       97 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/box_decoration_break.py
--rw-r--r--   0        0        0      146 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/box_shadow.py
--rw-r--r--   0        0        0     4223 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/box_shadow_color.py
--rw-r--r--   0        0        0       91 2023-04-17 09:38:33.978806 nicegui-1.2.8/nicegui/tailwind_types/box_sizing.py
--rw-r--r--   0        0        0      168 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/break_after.py
--rw-r--r--   0        0        0      169 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/break_before.py
--rw-r--r--   0        0        0      127 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/break_inside.py
--rw-r--r--   0        0        0      178 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/brightness.py
--rw-r--r--   0        0        0       89 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/caption_side.py
--rw-r--r--   0        0        0     4219 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/caret_color.py
--rw-r--r--   0        0        0      107 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/clear.py
--rw-r--r--   0        0        0      321 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/columns.py
--rw-r--r--   0        0        0       72 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/content.py
--rw-r--r--   0        0        0      134 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/contrast.py
--rw-r--r--   0        0        0      623 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/cursor.py
--rw-r--r--   0        0        0      443 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/display.py
--rw-r--r--   0        0        0     4220 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/divide_color.py
--rw-r--r--   0        0        0      131 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/divide_style.py
--rw-r--r--   0        0        0      204 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/divide_width.py
--rw-r--r--   0        0        0      134 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/drop_shadow.py
--rw-r--r--   0        0        0     4225 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/fill.py
--rw-r--r--   0        0        0      105 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex.py
--rw-r--r--   0        0        0      729 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex_basis.py
--rw-r--r--   0        0        0      126 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex_direction.py
--rw-r--r--   0        0        0       78 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex_grow.py
--rw-r--r--   0        0        0       80 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex_shrink.py
--rw-r--r--   0        0        0      107 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/flex_wrap.py
--rw-r--r--   0        0        0       96 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/floats.py
--rw-r--r--   0        0        0      100 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_family.py
--rw-r--r--   0        0        0      201 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_size.py
--rw-r--r--   0        0        0      113 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_smoothing.py
--rw-r--r--   0        0        0       94 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_style.py
--rw-r--r--   0        0        0      261 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_variant_numeric.py
--rw-r--r--   0        0        0      192 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/font_weight.py
--rw-r--r--   0        0        0     1228 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/gap.py
--rw-r--r--   0        0        0    16445 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/gradient_color_stops.py
--rw-r--r--   0        0        0       79 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grayscale.py
--rw-r--r--   0        0        0      112 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_auto_columns.py
--rw-r--r--   0        0        0      134 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_auto_flow.py
--rw-r--r--   0        0        0      109 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_auto_rows.py
--rw-r--r--   0        0        0      677 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_column_start_end.py
--rw-r--r--   0        0        0      411 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_row_start_end.py
--rw-r--r--   0        0        0      195 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_template_columns.py
--rw-r--r--   0        0        0      135 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/grid_template_rows.py
--rw-r--r--   0        0        0      639 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/height.py
--rw-r--r--   0        0        0      122 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/hue_rotate.py
--rw-r--r--   0        0        0       98 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/hyphens.py
--rw-r--r--   0        0        0       76 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/invert.py
--rw-r--r--   0        0        0       99 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/isolation.py
--rw-r--r--   0        0        0      177 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/justify_content.py
--rw-r--r--   0        0        0      118 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/justify_items.py
--rw-r--r--   0        0        0      129 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/justify_self.py
--rw-r--r--   0        0        0      147 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/letter_spacing.py
--rw-r--r--   0        0        0      128 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/line_clamp.py
--rw-r--r--   0        0        0      215 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/line_height.py
--rw-r--r--   0        0        0       79 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/list_style_image.py
--rw-r--r--   0        0        0       99 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/list_style_position.py
--rw-r--r--   0        0        0      105 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/list_style_type.py
--rw-r--r--   0        0        0     4199 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/margin.py
--rw-r--r--   0        0        0      477 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/max_height.py
--rw-r--r--   0        0        0      342 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/max_width.py
--rw-r--r--   0        0        0      130 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/min_height.py
--rw-r--r--   0        0        0      115 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/min_width.py
--rw-r--r--   0        0        0      341 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/mix_blend_mode.py
--rw-r--r--   0        0        0      132 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/object_fit.py
--rw-r--r--   0        0        0      203 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/object_position.py
--rw-r--r--   0        0        0      209 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/opacity.py
--rw-r--r--   0        0        0      206 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/order.py
--rw-r--r--   0        0        0     4221 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/outline_color.py
--rw-r--r--   0        0        0      111 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/outline_offset.py
--rw-r--r--   0        0        0      127 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/outline_style.py
--rw-r--r--   0        0        0      110 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/outline_width.py
--rw-r--r--   0        0        0      282 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/overflow.py
--rw-r--r--   0        0        0      200 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/overscroll_behavior.py
--rw-r--r--   0        0        0     4066 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/padding.py
--rw-r--r--   0        0        0      177 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/place_content.py
--rw-r--r--   0        0        0      132 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/place_items.py
--rw-r--r--   0        0        0      127 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/place_self.py
--rw-r--r--   0        0        0       90 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/pointer_events.py
--rw-r--r--   0        0        0      134 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/position.py
--rw-r--r--   0        0        0       97 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/resize.py
--rw-r--r--   0        0        0     4218 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/ring_color.py
--rw-r--r--   0        0        0     4224 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/ring_offset_color.py
--rw-r--r--   0        0        0      113 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/ring_offset_width.py
--rw-r--r--   0        0        0      128 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/ring_width.py
--rw-r--r--   0        0        0      145 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/rotate.py
--rw-r--r--   0        0        0      113 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/saturate.py
--rw-r--r--   0        0        0      410 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scale.py
--rw-r--r--   0        0        0      100 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/screen_readers.py
--rw-r--r--   0        0        0       93 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_behavior.py
--rw-r--r--   0        0        0     4071 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_margin.py
--rw-r--r--   0        0        0     4072 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_padding.py
--rw-r--r--   0        0        0      124 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_snap_align.py
--rw-r--r--   0        0        0       95 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_snap_stop.py
--rw-r--r--   0        0        0      143 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/scroll_snap_type.py
--rw-r--r--   0        0        0       75 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/sepia.py
--rw-r--r--   0        0        0      191 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/skew.py
--rw-r--r--   0        0        0      927 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/space_between.py
--rw-r--r--   0        0        0     4227 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/stroke.py
--rw-r--r--   0        0        0       91 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/stroke_width.py
--rw-r--r--   0        0        0       89 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/table_layout.py
--rw-r--r--   0        0        0      140 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_align.py
--rw-r--r--   0        0        0     4218 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_color.py
--rw-r--r--   0        0        0      140 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_decoration.py
--rw-r--r--   0        0        0     4228 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_decoration_color.py
--rw-r--r--   0        0        0      139 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_decoration_style.py
--rw-r--r--   0        0        0      150 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_decoration_thickness.py
--rw-r--r--   0        0        0      407 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_indent.py
--rw-r--r--   0        0        0      119 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_overflow.py
--rw-r--r--   0        0        0      137 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_transform.py
--rw-r--r--   0        0        0      129 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/text_underline_offset.py
--rw-r--r--   0        0        0     6299 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/top_right_bottom_left.py
--rw-r--r--   0        0        0      215 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/touch_action.py
--rw-r--r--   0        0        0      204 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/transform_origin.py
--rw-r--r--   0        0        0      165 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/transition_delay.py
--rw-r--r--   0        0        0      168 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/transition_duration.py
--rw-r--r--   0        0        0      162 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/transition_property.py
--rw-r--r--   0        0        0      126 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/transition_timing_function.py
--rw-r--r--   0        0        0     1074 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/translate.py
--rw-r--r--   0        0        0      110 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/user_select.py
--rw-r--r--   0        0        0      180 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/vertical_align.py
--rw-r--r--   0        0        0      111 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/visibility.py
--rw-r--r--   0        0        0      154 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/whitespace.py
--rw-r--r--   0        0        0      772 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/width.py
--rw-r--r--   0        0        0      122 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/will_change.py
--rw-r--r--   0        0        0      112 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/word_break.py
--rw-r--r--   0        0        0      130 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/tailwind_types/z_index.py
--rw-r--r--   0        0        0     7912 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/templates/index.html
--rw-r--r--   0        0        0     3758 2023-04-17 09:38:33.982807 nicegui-1.2.8/nicegui/ui.py
--rw-r--r--   0        0        0     1685 2023-04-17 09:38:47.919894 nicegui-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     7464 1970-01-01 00:00:00.000000 nicegui-1.2.8/setup.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 nicegui-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-21 13:32:27.550473 nicegui-1.2.9/LICENSE
+-rw-r--r--   0        0        0     5751 2023-04-21 13:32:27.550473 nicegui-1.2.9/README.md
+-rw-r--r--   0        0        0      288 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/__init__.py
+-rw-r--r--   0        0        0     3118 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/app.py
+-rw-r--r--   0        0        0     2056 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/background_tasks.py
+-rw-r--r--   0        0        0     4599 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/binding.py
+-rw-r--r--   0        0        0     6050 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/client.py
+-rw-r--r--   0        0        0     1291 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/colors.py
+-rw-r--r--   0        0        0     3030 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/dependencies.py
+-rw-r--r--   0        0        0      457 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/deprecation.py
+-rw-r--r--   0        0        0    11051 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/element.py
+-rw-r--r--   0        0        0     2958 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/aggrid.js
+-rw-r--r--   0        0        0     2975 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/aggrid.py
+-rw-r--r--   0        0        0      212 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/audio.js
+-rw-r--r--   0        0        0     1487 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/audio.py
+-rw-r--r--   0        0        0     1827 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/avatar.py
+-rw-r--r--   0        0        0     1095 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/badge.py
+-rw-r--r--   0        0        0     1533 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/button.py
+-rw-r--r--   0        0        0     1124 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/card.py
+-rw-r--r--   0        0        0      990 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/chart.js
+-rw-r--r--   0        0        0     4840 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/chart.py
+-rw-r--r--   0        0        0      701 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/checkbox.py
+-rw-r--r--   0        0        0     1075 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/choice_element.py
+-rw-r--r--   0        0        0     1440 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/color_input.py
+-rw-r--r--   0        0        0      915 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/color_picker.py
+-rw-r--r--   0        0        0      335 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/colors.js
+-rw-r--r--   0        0        0     1062 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/colors.py
+-rw-r--r--   0        0        0      269 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/column.py
+-rw-r--r--   0        0        0      455 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/dark_mode.js
+-rw-r--r--   0        0        0     1415 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/dark_mode.py
+-rw-r--r--   0        0        0     1295 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/date.py
+-rw-r--r--   0        0        0     1441 2023-04-21 13:32:27.562473 nicegui-1.2.9/nicegui/elements/dialog.py
+-rw-r--r--   0        0        0      861 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/expansion.py
+-rw-r--r--   0        0        0      543 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/html.py
+-rw-r--r--   0        0        0      947 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/icon.py
+-rw-r--r--   0        0        0      321 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/image.py
+-rw-r--r--   0        0        0     2909 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/input.py
+-rw-r--r--   0        0        0     2004 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/interactive_image.js
+-rw-r--r--   0        0        0     2600 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/interactive_image.py
+-rw-r--r--   0        0        0     2370 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/joystick.py
+-rw-r--r--   0        0        0      622 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/joystick.vue
+-rw-r--r--   0        0        0      792 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/keyboard.js
+-rw-r--r--   0        0        0     2397 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/keyboard.py
+-rw-r--r--   0        0        0     2325 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/knob.py
+-rw-r--r--   0        0        0      274 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/label.py
+-rw-r--r--   0        0        0     4673 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/lib/CSS2DRenderer.js
+-rw-r--r--   0        0        0     8988 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/lib/CSS3DRenderer.js
+-rw-r--r--   0        0        0    29354 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/lib/OrbitControls.js
+-rw-r--r--   0        0        0    10612 2023-04-21 13:32:27.566473 nicegui-1.2.9/nicegui/elements/lib/STLLoader.js
+-rw-r--r--   0        0        0  1570067 2023-04-21 13:32:27.570473 nicegui-1.2.9/nicegui/elements/lib/ag-grid-community.min.js
+-rw-r--r--   0        0        0    49248 2023-04-21 13:32:27.574473 nicegui-1.2.9/nicegui/elements/lib/highcharts-3d.js
+-rw-r--r--   0        0        0   106326 2023-04-21 13:32:27.574473 nicegui-1.2.9/nicegui/elements/lib/highcharts-more.js
+-rw-r--r--   0        0        0   303628 2023-04-21 13:32:27.574473 nicegui-1.2.9/nicegui/elements/lib/highcharts.js
+-rw-r--r--   0        0        0   130976 2023-04-21 13:32:27.574473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/accessibility.js
+-rw-r--r--   0        0        0    98853 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/annotations-advanced.js
+-rw-r--r--   0        0        0    65315 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/annotations.js
+-rw-r--r--   0        0        0     7406 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/arc-diagram.js
+-rw-r--r--   0        0        0     1211 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/arrow-symbols.js
+-rw-r--r--   0        0        0    43377 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/boost-canvas.js
+-rw-r--r--   0        0        0    47427 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/boost.js
+-rw-r--r--   0        0        0     5884 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/broken-axis.js
+-rw-r--r--   0        0        0     4029 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/bullet.js
+-rw-r--r--   0        0        0    12125 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/coloraxis.js
+-rw-r--r--   0        0        0     1770 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/current-date-indicator.js
+-rw-r--r--   0        0        0     5056 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/cylinder.js
+-rw-r--r--   0        0        0    16507 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/data.js
+-rw-r--r--   0        0        0    11360 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/datagrouping.js
+-rw-r--r--   0        0        0    15051 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/debugger.js
+-rw-r--r--   0        0        0     5733 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dependency-wheel.js
+-rw-r--r--   0        0        0     2652 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dotplot.js
+-rw-r--r--   0        0        0     4560 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/drag-panes.js
+-rw-r--r--   0        0        0    17196 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/draggable-points.js
+-rw-r--r--   0        0        0    18352 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/drilldown.js
+-rw-r--r--   0        0        0     8141 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dumbbell.js
+-rw-r--r--   0        0        0    12791 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/export-data.js
+-rw-r--r--   0        0        0    19692 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/exporting.js
+-rw-r--r--   0        0        0     3491 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/full-screen.js
+-rw-r--r--   0        0        0     5606 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/funnel.js
+-rw-r--r--   0        0        0    10167 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/funnel3d.js
+-rw-r--r--   0        0        0   112925 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/gantt.js
+-rw-r--r--   0        0        0    11206 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/grid-axis.js
+-rw-r--r--   0        0        0    19983 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/heatmap.js
+-rw-r--r--   0        0        0     3869 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/heikinashi.js
+-rw-r--r--   0        0        0     6199 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js
+-rw-r--r--   0        0        0     3983 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js
+-rw-r--r--   0        0        0     5636 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/item-series.js
+-rw-r--r--   0        0        0     3063 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/lollipop.js
+-rw-r--r--   0        0        0    17955 2023-04-21 13:32:27.578473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/marker-clusters.js
+-rw-r--r--   0        0        0    27952 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/networkgraph.js
+-rw-r--r--   0        0        0     1947 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/no-data-to-display.js
+-rw-r--r--   0        0        0     9627 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/offline-exporting.js
+-rw-r--r--   0        0        0     3042 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js
+-rw-r--r--   0        0        0    14679 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/oldie.js
+-rw-r--r--   0        0        0     8553 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/organization.js
+-rw-r--r--   0        0        0      741 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js
+-rw-r--r--   0        0        0     5234 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js
+-rw-r--r--   0        0        0     3180 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pareto.js
+-rw-r--r--   0        0        0    15251 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pathfinder.js
+-rw-r--r--   0        0        0     7026 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pattern-fill.js
+-rw-r--r--   0        0        0     2151 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/price-indicator.js
+-rw-r--r--   0        0        0     1640 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pyramid3d.js
+-rw-r--r--   0        0        0    16340 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sankey.js
+-rw-r--r--   0        0        0     9424 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/series-label.js
+-rw-r--r--   0        0        0     3792 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/series-on-point.js
+-rw-r--r--   0        0        0     4944 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/solid-gauge.js
+-rw-r--r--   0        0        0    29682 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sonification.js
+-rw-r--r--   0        0        0     1837 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/static-scale.js
+-rw-r--r--   0        0        0    55798 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/stock-tools.js
+-rw-r--r--   0        0        0   108215 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/stock.js
+-rw-r--r--   0        0        0     1698 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/streamgraph.js
+-rw-r--r--   0        0        0    37904 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sunburst.js
+-rw-r--r--   0        0        0     8257 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/tilemap.js
+-rw-r--r--   0        0        0     8804 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/timeline.js
+-rw-r--r--   0        0        0    18184 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treegraph.js
+-rw-r--r--   0        0        0    28748 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treegrid.js
+-rw-r--r--   0        0        0    27334 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treemap.js
+-rw-r--r--   0        0        0     4254 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/variable-pie.js
+-rw-r--r--   0        0        0     5739 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/variwide.js
+-rw-r--r--   0        0        0     3265 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/vector.js
+-rw-r--r--   0        0        0    15068 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/venn.js
+-rw-r--r--   0        0        0     7390 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/windbarb.js
+-rw-r--r--   0        0        0    11231 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/wordcloud.js
+-rw-r--r--   0        0        0     8508 2023-04-21 13:32:27.582473 nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/xrange.js
+-rw-r--r--   0        0        0  2777841 2023-04-21 13:32:27.602473 nicegui-1.2.9/nicegui/elements/lib/mermaid.min.js
+-rw-r--r--   0        0        0    20547 2023-04-21 13:32:27.602473 nicegui-1.2.9/nicegui/elements/lib/nipplejs.min.js
+-rw-r--r--   0        0        0  3579005 2023-04-21 13:32:27.622473 nicegui-1.2.9/nicegui/elements/lib/plotly.min.js
+-rw-r--r--   0        0        0   613740 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/lib/three.min.js
+-rw-r--r--   0        0        0    10633 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/lib/tween.umd.min.js
+-rw-r--r--   0        0        0     2298 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/line_plot.py
+-rw-r--r--   0        0        0      533 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/link.js
+-rw-r--r--   0        0        0     1395 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/link.py
+-rw-r--r--   0        0        0      997 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/log.js
+-rw-r--r--   0        0        0     1168 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/log.py
+-rw-r--r--   0        0        0      933 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/markdown.js
+-rw-r--r--   0        0        0     2701 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/markdown.py
+-rw-r--r--   0        0        0     1593 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/menu.py
+-rw-r--r--   0        0        0      274 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mermaid.js
+-rw-r--r--   0        0        0      861 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mermaid.py
+-rw-r--r--   0        0        0     3327 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/content_element.py
+-rw-r--r--   0        0        0      864 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/disableable_element.py
+-rw-r--r--   0        0        0     3131 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/filter_element.py
+-rw-r--r--   0        0        0     3055 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/source_element.py
+-rw-r--r--   0        0        0     3058 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/text_element.py
+-rw-r--r--   0        0        0     4204 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/value_element.py
+-rw-r--r--   0        0        0     3850 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/mixins/visibility.py
+-rw-r--r--   0        0        0     3663 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/number.py
+-rw-r--r--   0        0        0     2047 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/plotly.py
+-rw-r--r--   0        0        0     2622 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/plotly.vue
+-rw-r--r--   0        0        0     2741 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/progress.py
+-rw-r--r--   0        0        0     1471 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/pyplot.py
+-rw-r--r--   0        0        0     1158 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/query.js
+-rw-r--r--   0        0        0     2751 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/query.py
+-rw-r--r--   0        0        0     1100 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/radio.py
+-rw-r--r--   0        0        0      257 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/row.py
+-rw-r--r--   0        0        0    13006 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/scene.js
+-rw-r--r--   0        0        0     5765 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/scene.py
+-rw-r--r--   0        0        0     4047 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/scene_object3d.py
+-rw-r--r--   0        0        0     5066 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/scene_objects.py
+-rw-r--r--   0        0        0      924 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/select.js
+-rw-r--r--   0        0        0     2144 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/select.py
+-rw-r--r--   0        0        0      280 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/separator.py
+-rw-r--r--   0        0        0      931 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/slider.py
+-rw-r--r--   0        0        0     1461 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/spinner.py
+-rw-r--r--   0        0        0     1784 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/splitter.py
+-rw-r--r--   0        0        0      713 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/switch.py
+-rw-r--r--   0        0        0     3281 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/table.py
+-rw-r--r--   0        0        0     2926 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/tabs.py
+-rw-r--r--   0        0        0     1125 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/textarea.py
+-rw-r--r--   0        0        0      892 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/time.py
+-rw-r--r--   0        0        0     1098 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/toggle.py
+-rw-r--r--   0        0        0      335 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/tooltip.py
+-rw-r--r--   0        0        0     2634 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/tree.py
+-rw-r--r--   0        0        0      627 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/upload.js
+-rw-r--r--   0        0        0     2966 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/upload.py
+-rw-r--r--   0        0        0      212 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/video.js
+-rw-r--r--   0        0        0     1487 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/elements/video.py
+-rw-r--r--   0        0        0     1046 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/error.py
+-rw-r--r--   0        0        0     1102 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/event_listener.py
+-rw-r--r--   0        0        0     6093 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/events.py
+-rw-r--r--   0        0        0     1987 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/favicon.py
+-rw-r--r--   0        0        0      384 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/download.py
+-rw-r--r--   0        0        0      203 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/html.py
+-rw-r--r--   0        0        0     1230 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/javascript.py
+-rw-r--r--   0        0        0     1408 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/notify.py
+-rw-r--r--   0        0        0      669 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/open.py
+-rw-r--r--   0        0        0     1027 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/refreshable.py
+-rw-r--r--   0        0        0     3992 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/timer.py
+-rw-r--r--   0        0        0      126 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/functions/update.py
+-rw-r--r--   0        0        0     2262 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/globals.py
+-rw-r--r--   0        0        0     2900 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/helpers.py
+-rw-r--r--   0        0        0      387 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/ids.py
+-rw-r--r--   0        0        0      788 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/json/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/json/builtin_wrapper.py
+-rw-r--r--   0        0        0     1758 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/json/orjson_wrapper.py
+-rw-r--r--   0        0        0      220 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/native.py
+-rw-r--r--   0        0        0     2074 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/native_mode.py
+-rw-r--r--   0        0        0     6307 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/nicegui.py
+-rw-r--r--   0        0        0     1609 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/outbox.py
+-rw-r--r--   0        0        0     4376 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/page.py
+-rw-r--r--   0        0        0     8064 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/page_layout.py
+-rw-r--r--   0        0        0     5972 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/run.py
+-rw-r--r--   0        0        0      895 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/run_with.py
+-rw-r--r--   0        0        0      611 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/slot.py
+-rw-r--r--   0        0        0    15086 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/favicon.ico
+-rw-r--r--   0        0        0      756 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0    10144 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     7668 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     3360 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0    10972 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2
+-rw-r--r--   0        0        0     4960 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     6384 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2
+-rw-r--r--   0        0        0     6632 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11072 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4796 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      768 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10352 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7676 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3472 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6480 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11160 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4928 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      756 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10412 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7840 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3448 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6620 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    11040 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4796 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      756 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10256 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7676 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3468 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     6612 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10992 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2
+-rw-r--r--   0        0        0     4756 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0      772 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0    10188 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     7608 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     3388 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2
+-rw-r--r--   0        0        0     4864 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0    11028 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2
+-rw-r--r--   0        0        0     6460 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0    10352 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0     7736 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0     3496 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0      748 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2
+-rw-r--r--   0        0        0   128616 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0        0        0    11484 2023-04-21 13:32:27.626473 nicegui-1.2.9/nicegui/static/fonts.css
+-rw-r--r--   0        0        0     1913 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/nicegui.css
+-rw-r--r--   0        0        0   198973 2023-04-21 13:32:27.630473 nicegui-1.2.9/nicegui/static/quasar.prod.css
+-rw-r--r--   0        0        0   509631 2023-04-21 13:32:27.634473 nicegui-1.2.9/nicegui/static/quasar.umd.prod.js
+-rw-r--r--   0        0        0     1510 2023-04-21 13:32:27.634473 nicegui-1.2.9/nicegui/static/sad_face.svg
+-rw-r--r--   0        0        0    45896 2023-04-21 13:32:27.634473 nicegui-1.2.9/nicegui/static/socket.io.min.js
+-rw-r--r--   0        0        0   350399 2023-04-21 13:32:27.634473 nicegui-1.2.9/nicegui/static/tailwindcss.min.js
+-rw-r--r--   0        0        0   128872 2023-04-21 13:32:27.634473 nicegui-1.2.9/nicegui/static/vue.global.prod.js
+-rw-r--r--   0        0        0   107302 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/static/vue.min.js
+-rw-r--r--   0        0        0    44035 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind.py
+-rw-r--r--   0        0        0     4232 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/accent_color.py
+-rw-r--r--   0        0        0      191 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/align_content.py
+-rw-r--r--   0        0        0      132 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/align_items.py
+-rw-r--r--   0        0        0      143 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/align_self.py
+-rw-r--r--   0        0        0      125 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/animation.py
+-rw-r--r--   0        0        0       75 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/appearance.py
+-rw-r--r--   0        0        0      103 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/aspect_ratio.py
+-rw-r--r--   0        0        0      147 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_blur.py
+-rw-r--r--   0        0        0      186 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_brightness.py
+-rw-r--r--   0        0        0      142 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_contrast.py
+-rw-r--r--   0        0        0       87 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_grayscale.py
+-rw-r--r--   0        0        0      130 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_hue_rotate.py
+-rw-r--r--   0        0        0       84 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_invert.py
+-rw-r--r--   0        0        0      217 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_opacity.py
+-rw-r--r--   0        0        0      121 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_saturate.py
+-rw-r--r--   0        0        0       83 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/backdrop_sepia.py
+-rw-r--r--   0        0        0      113 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_attachment.py
+-rw-r--r--   0        0        0      328 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_blend_mode.py
+-rw-r--r--   0        0        0      123 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_clip.py
+-rw-r--r--   0        0        0     4224 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_color.py
+-rw-r--r--   0        0        0      252 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_image.py
+-rw-r--r--   0        0        0      113 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_origin.py
+-rw-r--r--   0        0        0      207 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_position.py
+-rw-r--r--   0        0        0      172 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_repeat.py
+-rw-r--r--   0        0        0      107 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/background_size.py
+-rw-r--r--   0        0        0      139 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/blur.py
+-rw-r--r--   0        0        0       99 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_collapse.py
+-rw-r--r--   0        0        0    41420 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_color.py
+-rw-r--r--   0        0        0     1785 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_radius.py
+-rw-r--r--   0        0        0     1238 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_spacing.py
+-rw-r--r--   0        0        0      145 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_style.py
+-rw-r--r--   0        0        0      532 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/border_width.py
+-rw-r--r--   0        0        0       97 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/box_decoration_break.py
+-rw-r--r--   0        0        0      146 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/box_shadow.py
+-rw-r--r--   0        0        0     4223 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/box_shadow_color.py
+-rw-r--r--   0        0        0       91 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/box_sizing.py
+-rw-r--r--   0        0        0      168 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/break_after.py
+-rw-r--r--   0        0        0      169 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/break_before.py
+-rw-r--r--   0        0        0      127 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/break_inside.py
+-rw-r--r--   0        0        0      178 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/brightness.py
+-rw-r--r--   0        0        0       89 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/caption_side.py
+-rw-r--r--   0        0        0     4219 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/caret_color.py
+-rw-r--r--   0        0        0      107 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/clear.py
+-rw-r--r--   0        0        0      321 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/columns.py
+-rw-r--r--   0        0        0       72 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/content.py
+-rw-r--r--   0        0        0      134 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/contrast.py
+-rw-r--r--   0        0        0      623 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/cursor.py
+-rw-r--r--   0        0        0      443 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/display.py
+-rw-r--r--   0        0        0     4220 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/divide_color.py
+-rw-r--r--   0        0        0      131 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/divide_style.py
+-rw-r--r--   0        0        0      204 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/divide_width.py
+-rw-r--r--   0        0        0      134 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/drop_shadow.py
+-rw-r--r--   0        0        0     4225 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/fill.py
+-rw-r--r--   0        0        0      105 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex.py
+-rw-r--r--   0        0        0      729 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex_basis.py
+-rw-r--r--   0        0        0      126 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex_direction.py
+-rw-r--r--   0        0        0       78 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex_grow.py
+-rw-r--r--   0        0        0       80 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex_shrink.py
+-rw-r--r--   0        0        0      107 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/flex_wrap.py
+-rw-r--r--   0        0        0       96 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/floats.py
+-rw-r--r--   0        0        0      100 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_family.py
+-rw-r--r--   0        0        0      201 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_size.py
+-rw-r--r--   0        0        0      113 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_smoothing.py
+-rw-r--r--   0        0        0       94 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_style.py
+-rw-r--r--   0        0        0      261 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_variant_numeric.py
+-rw-r--r--   0        0        0      192 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/font_weight.py
+-rw-r--r--   0        0        0     1228 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/gap.py
+-rw-r--r--   0        0        0    16445 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/gradient_color_stops.py
+-rw-r--r--   0        0        0       79 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grayscale.py
+-rw-r--r--   0        0        0      112 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_auto_columns.py
+-rw-r--r--   0        0        0      134 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_auto_flow.py
+-rw-r--r--   0        0        0      109 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_auto_rows.py
+-rw-r--r--   0        0        0      677 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_column_start_end.py
+-rw-r--r--   0        0        0      411 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_row_start_end.py
+-rw-r--r--   0        0        0      195 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_template_columns.py
+-rw-r--r--   0        0        0      135 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/grid_template_rows.py
+-rw-r--r--   0        0        0      639 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/height.py
+-rw-r--r--   0        0        0      122 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/hue_rotate.py
+-rw-r--r--   0        0        0       98 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/hyphens.py
+-rw-r--r--   0        0        0       76 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/invert.py
+-rw-r--r--   0        0        0       99 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/isolation.py
+-rw-r--r--   0        0        0      177 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/justify_content.py
+-rw-r--r--   0        0        0      118 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/justify_items.py
+-rw-r--r--   0        0        0      129 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/justify_self.py
+-rw-r--r--   0        0        0      147 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/letter_spacing.py
+-rw-r--r--   0        0        0      128 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/line_clamp.py
+-rw-r--r--   0        0        0      215 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/line_height.py
+-rw-r--r--   0        0        0       79 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/list_style_image.py
+-rw-r--r--   0        0        0       99 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/list_style_position.py
+-rw-r--r--   0        0        0      105 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/list_style_type.py
+-rw-r--r--   0        0        0     4199 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/margin.py
+-rw-r--r--   0        0        0      477 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/max_height.py
+-rw-r--r--   0        0        0      342 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/max_width.py
+-rw-r--r--   0        0        0      130 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/min_height.py
+-rw-r--r--   0        0        0      115 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/min_width.py
+-rw-r--r--   0        0        0      341 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/mix_blend_mode.py
+-rw-r--r--   0        0        0      132 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/object_fit.py
+-rw-r--r--   0        0        0      203 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/object_position.py
+-rw-r--r--   0        0        0      209 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/opacity.py
+-rw-r--r--   0        0        0      206 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/order.py
+-rw-r--r--   0        0        0     4221 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/outline_color.py
+-rw-r--r--   0        0        0      111 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/outline_offset.py
+-rw-r--r--   0        0        0      127 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/outline_style.py
+-rw-r--r--   0        0        0      110 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/outline_width.py
+-rw-r--r--   0        0        0      282 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/overflow.py
+-rw-r--r--   0        0        0      200 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/overscroll_behavior.py
+-rw-r--r--   0        0        0     4066 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/padding.py
+-rw-r--r--   0        0        0      177 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/place_content.py
+-rw-r--r--   0        0        0      132 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/place_items.py
+-rw-r--r--   0        0        0      127 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/place_self.py
+-rw-r--r--   0        0        0       90 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/pointer_events.py
+-rw-r--r--   0        0        0      134 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/position.py
+-rw-r--r--   0        0        0       97 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/resize.py
+-rw-r--r--   0        0        0     4218 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/ring_color.py
+-rw-r--r--   0        0        0     4224 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/ring_offset_color.py
+-rw-r--r--   0        0        0      113 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/ring_offset_width.py
+-rw-r--r--   0        0        0      128 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/ring_width.py
+-rw-r--r--   0        0        0      145 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/rotate.py
+-rw-r--r--   0        0        0      113 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/saturate.py
+-rw-r--r--   0        0        0      410 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scale.py
+-rw-r--r--   0        0        0      100 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/screen_readers.py
+-rw-r--r--   0        0        0       93 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_behavior.py
+-rw-r--r--   0        0        0     4071 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_margin.py
+-rw-r--r--   0        0        0     4072 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_padding.py
+-rw-r--r--   0        0        0      124 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_snap_align.py
+-rw-r--r--   0        0        0       95 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_snap_stop.py
+-rw-r--r--   0        0        0      143 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/scroll_snap_type.py
+-rw-r--r--   0        0        0       75 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/sepia.py
+-rw-r--r--   0        0        0      191 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/skew.py
+-rw-r--r--   0        0        0      927 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/space_between.py
+-rw-r--r--   0        0        0     4227 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/stroke.py
+-rw-r--r--   0        0        0       91 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/stroke_width.py
+-rw-r--r--   0        0        0       89 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/table_layout.py
+-rw-r--r--   0        0        0      140 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/text_align.py
+-rw-r--r--   0        0        0     4218 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/text_color.py
+-rw-r--r--   0        0        0      140 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/text_decoration.py
+-rw-r--r--   0        0        0     4228 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/text_decoration_color.py
+-rw-r--r--   0        0        0      139 2023-04-21 13:32:27.638473 nicegui-1.2.9/nicegui/tailwind_types/text_decoration_style.py
+-rw-r--r--   0        0        0      150 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/text_decoration_thickness.py
+-rw-r--r--   0        0        0      407 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/text_indent.py
+-rw-r--r--   0        0        0      119 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/text_overflow.py
+-rw-r--r--   0        0        0      137 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/text_transform.py
+-rw-r--r--   0        0        0      129 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/text_underline_offset.py
+-rw-r--r--   0        0        0     6299 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/top_right_bottom_left.py
+-rw-r--r--   0        0        0      215 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/touch_action.py
+-rw-r--r--   0        0        0      204 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/transform_origin.py
+-rw-r--r--   0        0        0      165 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/transition_delay.py
+-rw-r--r--   0        0        0      168 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/transition_duration.py
+-rw-r--r--   0        0        0      162 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/transition_property.py
+-rw-r--r--   0        0        0      126 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/transition_timing_function.py
+-rw-r--r--   0        0        0     1074 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/translate.py
+-rw-r--r--   0        0        0      110 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/user_select.py
+-rw-r--r--   0        0        0      180 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/vertical_align.py
+-rw-r--r--   0        0        0      111 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/visibility.py
+-rw-r--r--   0        0        0      154 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/whitespace.py
+-rw-r--r--   0        0        0      772 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/width.py
+-rw-r--r--   0        0        0      122 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/will_change.py
+-rw-r--r--   0        0        0      112 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/word_break.py
+-rw-r--r--   0        0        0      130 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/tailwind_types/z_index.py
+-rw-r--r--   0        0        0     7921 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/templates/index.html
+-rw-r--r--   0        0        0     3859 2023-04-21 13:32:27.642473 nicegui-1.2.9/nicegui/ui.py
+-rw-r--r--   0        0        0     1693 2023-04-21 13:32:40.342454 nicegui-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 nicegui-1.2.9/setup.py
+-rw-r--r--   0        0        0     7364 1970-01-01 00:00:00.000000 nicegui-1.2.9/PKG-INFO
```

### Comparing `nicegui-1.2.8/LICENSE` & `nicegui-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/README.md` & `nicegui-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/app.py` & `nicegui-1.2.9/nicegui/app.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/background_tasks.py` & `nicegui-1.2.9/nicegui/background_tasks.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/binding.py` & `nicegui-1.2.9/nicegui/binding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/client.py` & `nicegui-1.2.9/nicegui/client.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/colors.py` & `nicegui-1.2.9/nicegui/colors.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/dependencies.py` & `nicegui-1.2.9/nicegui/dependencies.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/element.py` & `nicegui-1.2.9/nicegui/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.id = self.client.next_element_id
         self.client.next_element_id += 1
         self.tag = tag
         self._classes: List[str] = []
         self._style: Dict[str, str] = {}
         self._props: Dict[str, Any] = {}
         self._event_listeners: Dict[str, EventListener] = {}
-        self._text: str = ''
+        self._text: Optional[str] = None
         self.slots: Dict[str, Slot] = {}
         self.default_slot = self.add_slot('default')
 
         self.client.elements[self.id] = self
         self.parent_slot: Optional[Slot] = None
         slot_stack = globals.get_slot_stack()
         if slot_stack:
```

### Comparing `nicegui-1.2.8/nicegui/elements/aggrid.js` & `nicegui-1.2.9/nicegui/elements/aggrid.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/aggrid.py` & `nicegui-1.2.9/nicegui/elements/aggrid.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/audio.py` & `nicegui-1.2.9/nicegui/elements/audio.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/avatar.py` & `nicegui-1.2.9/nicegui/elements/avatar.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/badge.py` & `nicegui-1.2.9/nicegui/elements/badge.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/button.py` & `nicegui-1.2.9/nicegui/elements/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Callable, Optional
 
 from ..colors import set_background_color
 from ..events import ClickEventArguments, handle_event
+from .mixins.disableable_element import DisableableElement
 from .mixins.text_element import TextElement
 
 
-class Button(TextElement):
+class Button(TextElement, DisableableElement):
 
     def __init__(self,
                  text: str = '', *,
                  on_click: Optional[Callable] = None,
                  color: Optional[str] = 'primary',
                  ) -> None:
         """Button
```

### Comparing `nicegui-1.2.8/nicegui/elements/card.py` & `nicegui-1.2.9/nicegui/elements/card.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/chart.js` & `nicegui-1.2.9/nicegui/elements/chart.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/chart.py` & `nicegui-1.2.9/nicegui/elements/chart.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/checkbox.py` & `nicegui-1.2.9/nicegui/elements/checkbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.text_element import TextElement
 from .mixins.value_element import ValueElement
 
 
-class Checkbox(TextElement, ValueElement):
+class Checkbox(TextElement, ValueElement, DisableableElement):
 
     def __init__(self, text: str = '', *, value: bool = False, on_change: Optional[Callable] = None) -> None:
         """Checkbox
 
         :param text: the label to display next to the checkbox
         :param value: whether it should be checked initially (default: `False`)
         :param on_change: callback to execute when value changes
```

### Comparing `nicegui-1.2.8/nicegui/elements/choice_element.py` & `nicegui-1.2.9/nicegui/elements/choice_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/color_input.py` & `nicegui-1.2.9/nicegui/elements/color_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Callable, Optional
 
 from nicegui import ui
 
 from .color_picker import ColorPicker
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class ColorInput(ValueElement):
+class ColorInput(ValueElement, DisableableElement):
     LOOPBACK = False
 
     def __init__(self, label: Optional[str] = None, *,
                  placeholder: Optional[str] = None, value: str = '', on_change: Optional[Callable] = None) -> None:
         """Color Input
 
         :param label: displayed label for the color input
```

### Comparing `nicegui-1.2.8/nicegui/elements/color_picker.py` & `nicegui-1.2.9/nicegui/elements/color_picker.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/colors.py` & `nicegui-1.2.9/nicegui/elements/colors.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/date.py` & `nicegui-1.2.9/nicegui/elements/date.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Date(ValueElement):
+class Date(ValueElement, DisableableElement):
     EVENT_ARGS = None
 
     def __init__(self,
                  value: Optional[str] = None,
                  *,
                  mask: str = 'YYYY-MM-DD',
                  on_change: Optional[Callable] = None) -> None:
```

### Comparing `nicegui-1.2.8/nicegui/elements/dialog.py` & `nicegui-1.2.9/nicegui/elements/dialog.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/expansion.py` & `nicegui-1.2.9/nicegui/elements/expansion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Expansion(ValueElement):
+class Expansion(ValueElement, DisableableElement):
 
     def __init__(self, text: Optional[str] = None, *, icon: Optional[str] = None, value: bool = False) -> None:
         '''Expansion Element
 
         Provides an expandable container.
 
         :param text: title text
```

### Comparing `nicegui-1.2.8/nicegui/elements/html.py` & `nicegui-1.2.9/nicegui/elements/html.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/icon.py` & `nicegui-1.2.9/nicegui/elements/icon.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/input.py` & `nicegui-1.2.9/nicegui/elements/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Callable, Dict, Optional
 
 from .icon import Icon
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Input(ValueElement):
+class Input(ValueElement, DisableableElement):
     LOOPBACK = False
 
     def __init__(self,
                  label: Optional[str] = None, *,
                  placeholder: Optional[str] = None,
                  value: str = '',
                  password: bool = False,
```

### Comparing `nicegui-1.2.8/nicegui/elements/interactive_image.js` & `nicegui-1.2.9/nicegui/elements/interactive_image.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/interactive_image.py` & `nicegui-1.2.9/nicegui/elements/interactive_image.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/joystick.py` & `nicegui-1.2.9/nicegui/elements/joystick.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/joystick.vue` & `nicegui-1.2.9/nicegui/elements/joystick.vue`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/keyboard.js` & `nicegui-1.2.9/nicegui/elements/keyboard.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/keyboard.py` & `nicegui-1.2.9/nicegui/elements/keyboard.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/knob.py` & `nicegui-1.2.9/nicegui/elements/knob.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
 from ..colors import set_text_color
 from .label import Label
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Knob(ValueElement):
+class Knob(ValueElement, DisableableElement):
 
     def __init__(self,
                  value: float = 0.0,
                  *,
                  min: float = 0.0,
                  max: float = 1.0,
                  step: float = 0.01,
```

### Comparing `nicegui-1.2.8/nicegui/elements/lib/CSS2DRenderer.js` & `nicegui-1.2.9/nicegui/elements/lib/CSS2DRenderer.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/CSS3DRenderer.js` & `nicegui-1.2.9/nicegui/elements/lib/CSS3DRenderer.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/OrbitControls.js` & `nicegui-1.2.9/nicegui/elements/lib/OrbitControls.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/STLLoader.js` & `nicegui-1.2.9/nicegui/elements/lib/STLLoader.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/ag-grid-community.min.js` & `nicegui-1.2.9/nicegui/elements/lib/ag-grid-community.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts-3d.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts-3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts-more.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/accessibility.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/accessibility.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/annotations-advanced.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/annotations-advanced.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/annotations.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/annotations.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/arc-diagram.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/arc-diagram.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/arrow-symbols.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/arrow-symbols.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/boost-canvas.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/boost-canvas.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/boost.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/boost.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/broken-axis.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/broken-axis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/bullet.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/bullet.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/coloraxis.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/coloraxis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/current-date-indicator.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/current-date-indicator.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/cylinder.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/cylinder.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/data.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/data.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/datagrouping.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/datagrouping.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/debugger.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/debugger.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dependency-wheel.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dependency-wheel.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dotplot.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dotplot.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/drag-panes.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/drag-panes.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/draggable-points.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/draggable-points.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/drilldown.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/drilldown.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/dumbbell.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/dumbbell.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/export-data.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/export-data.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/exporting.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/exporting.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/full-screen.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/full-screen.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/funnel.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/funnel.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/funnel3d.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/funnel3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/gantt.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/gantt.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/grid-axis.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/grid-axis.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/heatmap.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/heatmap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/heikinashi.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/heikinashi.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/histogram-bellcurve.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/hollowcandlestick.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/item-series.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/item-series.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/lollipop.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/lollipop.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/marker-clusters.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/marker-clusters.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/networkgraph.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/networkgraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/no-data-to-display.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/no-data-to-display.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/offline-exporting.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/offline-exporting.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/oldie-polyfills.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/oldie.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/oldie.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/organization.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/organization.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/overlapping-datalabels.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/parallel-coordinates.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pareto.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pareto.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pathfinder.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pathfinder.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pattern-fill.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pattern-fill.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/price-indicator.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/price-indicator.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/pyramid3d.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/pyramid3d.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sankey.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sankey.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/series-label.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/series-label.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/series-on-point.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/series-on-point.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/solid-gauge.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/solid-gauge.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sonification.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sonification.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/static-scale.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/static-scale.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/stock-tools.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/stock-tools.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/stock.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/stock.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/streamgraph.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/streamgraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/sunburst.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/sunburst.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/tilemap.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/tilemap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/timeline.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/timeline.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treegraph.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treegraph.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treegrid.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treegrid.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/treemap.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/treemap.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/variable-pie.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/variable-pie.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/variwide.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/variwide.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/vector.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/vector.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/venn.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/venn.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/windbarb.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/windbarb.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/wordcloud.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/wordcloud.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/highcharts_modules/xrange.js` & `nicegui-1.2.9/nicegui/elements/lib/highcharts_modules/xrange.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/mermaid.min.js` & `nicegui-1.2.9/nicegui/elements/lib/mermaid.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/nipplejs.min.js` & `nicegui-1.2.9/nicegui/elements/lib/nipplejs.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/plotly.min.js` & `nicegui-1.2.9/nicegui/elements/lib/plotly.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/three.min.js` & `nicegui-1.2.9/nicegui/elements/lib/three.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/lib/tween.umd.min.js` & `nicegui-1.2.9/nicegui/elements/lib/tween.umd.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/line_plot.py` & `nicegui-1.2.9/nicegui/elements/line_plot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/link.js` & `nicegui-1.2.9/nicegui/elements/link.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/link.py` & `nicegui-1.2.9/nicegui/elements/link.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/log.js` & `nicegui-1.2.9/nicegui/elements/log.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/log.py` & `nicegui-1.2.9/nicegui/elements/log.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/markdown.js` & `nicegui-1.2.9/nicegui/elements/markdown.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/markdown.py` & `nicegui-1.2.9/nicegui/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/menu.py` & `nicegui-1.2.9/nicegui/elements/menu.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mermaid.py` & `nicegui-1.2.9/nicegui/elements/mermaid.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/content_element.py` & `nicegui-1.2.9/nicegui/elements/mixins/content_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/filter_element.py` & `nicegui-1.2.9/nicegui/elements/mixins/filter_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/source_element.py` & `nicegui-1.2.9/nicegui/elements/mixins/source_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/text_element.py` & `nicegui-1.2.9/nicegui/elements/mixins/text_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/value_element.py` & `nicegui-1.2.9/nicegui/elements/mixins/value_element.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/mixins/visibility.py` & `nicegui-1.2.9/nicegui/elements/mixins/visibility.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/number.py` & `nicegui-1.2.9/nicegui/elements/number.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,72 @@
 from typing import Any, Callable, Dict, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Number(ValueElement):
+class Number(ValueElement, DisableableElement):
     LOOPBACK = False
 
     def __init__(self,
                  label: Optional[str] = None, *,
                  placeholder: Optional[str] = None,
                  value: Optional[float] = None,
+                 min: Optional[float] = None,
+                 max: Optional[float] = None,
+                 step: Optional[float] = None,
+                 prefix: Optional[str] = None,
+                 suffix: Optional[str] = None,
                  format: Optional[str] = None,
                  on_change: Optional[Callable] = None,
                  validation: Dict[str, Callable] = {}) -> None:
         """Number Input
 
         This element is based on Quasar's `QInput <https://quasar.dev/vue-components/input>`_ component.
 
         You can use the `validation` parameter to define a dictionary of validation rules.
         The key of the first rule that fails will be displayed as an error message.
 
         :param label: displayed name for the number input
         :param placeholder: text to show if no value is entered
         :param value: the initial value of the field
+        :param min: the minimum value allowed
+        :param max: the maximum value allowed
+        :param step: the step size for the stepper buttons
+        :param prefix: a prefix to prepend to the displayed value
+        :param suffix: a suffix to append to the displayed value
         :param format: a string like "%.2f" to format the displayed value
         :param on_change: callback to execute when the input is confirmed by leaving the focus
         :param validation: dictionary of validation rules, e.g. ``{'Too small!': lambda value: value < 3}``
         """
         self.format = format
         super().__init__(tag='q-input', value=value, on_value_change=on_change)
         self._props['type'] = 'number'
         if label is not None:
             self._props['label'] = label
         if placeholder is not None:
             self._props['placeholder'] = placeholder
+        if min is not None:
+            self._props['min'] = min
+        if max is not None:
+            self._props['max'] = max
+        if step is not None:
+            self._props['step'] = step
+        if prefix is not None:
+            self._props['prefix'] = prefix
+        if suffix is not None:
+            self._props['suffix'] = suffix
         self.validation = validation
-        self.on('blur', self.update)  # NOTE: to apply format (#736)
+        self.on('blur', self.sanitize)
+
+    def sanitize(self) -> None:
+        value = float(self.value or 0)
+        value = max(value, self._props.get('min', -float('inf')))
+        value = min(value, self._props.get('max', float('inf')))
+        self.set_value(self.format % value if self.format else str(value))
 
     def on_value_change(self, value: Any) -> None:
         super().on_value_change(value)
         for message, check in self.validation.items():
             if not check(value):
                 self.props(f'error error-message="{message}"')
                 break
```

### Comparing `nicegui-1.2.8/nicegui/elements/plotly.py` & `nicegui-1.2.9/nicegui/elements/plotly.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/plotly.vue` & `nicegui-1.2.9/nicegui/elements/plotly.vue`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/progress.py` & `nicegui-1.2.9/nicegui/elements/progress.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/pyplot.py` & `nicegui-1.2.9/nicegui/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/query.js` & `nicegui-1.2.9/nicegui/elements/query.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/query.py` & `nicegui-1.2.9/nicegui/elements/query.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/radio.py` & `nicegui-1.2.9/nicegui/elements/radio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from .choice_element import ChoiceElement
+from .mixins.disableable_element import DisableableElement
 
 
-class Radio(ChoiceElement):
+class Radio(ChoiceElement, DisableableElement):
 
     def __init__(self, options: Union[List, Dict], *, value: Any = None, on_change: Optional[Callable] = None):
         """Radio Selection
 
         The options can be specified as a list of values, or as a dictionary mapping values to labels.
         After manipulating the options, call `update()` to update the options in the UI.
```

### Comparing `nicegui-1.2.8/nicegui/elements/scene.js` & `nicegui-1.2.9/nicegui/elements/scene.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/scene.py` & `nicegui-1.2.9/nicegui/elements/scene.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/scene_object3d.py` & `nicegui-1.2.9/nicegui/elements/scene_object3d.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/scene_objects.py` & `nicegui-1.2.9/nicegui/elements/scene_objects.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/select.js` & `nicegui-1.2.9/nicegui/elements/select.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/select.py` & `nicegui-1.2.9/nicegui/elements/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from nicegui.dependencies import register_component
 
 from .choice_element import ChoiceElement
+from .mixins.disableable_element import DisableableElement
 
 register_component('select', __file__, 'select.js')
 
 
-class Select(ChoiceElement):
+class Select(ChoiceElement, DisableableElement):
 
     def __init__(self, options: Union[List, Dict], *,
                  label: Optional[str] = None,
                  value: Any = None,
                  on_change: Optional[Callable] = None,
                  with_input: bool = False) -> None:
         """Dropdown Selection
```

### Comparing `nicegui-1.2.8/nicegui/elements/slider.py` & `nicegui-1.2.9/nicegui/elements/slider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Slider(ValueElement):
+class Slider(ValueElement, DisableableElement):
 
     def __init__(self, *,
                  min: float,
                  max: float,
                  step: float = 1.0,
                  value: Optional[float] = None,
                  on_change: Optional[Callable] = None) -> None:
```

### Comparing `nicegui-1.2.8/nicegui/elements/spinner.py` & `nicegui-1.2.9/nicegui/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/splitter.py` & `nicegui-1.2.9/nicegui/elements/splitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Callable, Optional, Tuple
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Splitter(ValueElement):
+class Splitter(ValueElement, DisableableElement):
+
     def __init__(self, *,
                  horizontal: Optional[bool] = False,
                  reverse: Optional[bool] = False,
                  limits: Optional[Tuple[float, float]] = (0, 100),
                  value: Optional[float] = 50,
                  on_change: Optional[Callable] = None) -> None:
         """Splitter
```

### Comparing `nicegui-1.2.8/nicegui/elements/switch.py` & `nicegui-1.2.9/nicegui/elements/switch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.text_element import TextElement
 from .mixins.value_element import ValueElement
 
 
-class Switch(TextElement, ValueElement):
+class Switch(TextElement, ValueElement, DisableableElement):
 
     def __init__(self, text: str = '', *, value: bool = False, on_change: Optional[Callable] = None) -> None:
         """Switch
 
         :param text: the label to display next to the switch
         :param value: whether it should be active initially (default: `False`)
         :param on_change: callback which is invoked when state is changed by the user
```

### Comparing `nicegui-1.2.8/nicegui/elements/table.py` & `nicegui-1.2.9/nicegui/elements/table.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/tabs.py` & `nicegui-1.2.9/nicegui/elements/tabs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Callable, Optional
 
 from .. import globals
-from ..element import Element
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
 class Tabs(ValueElement):
 
     def __init__(self, *,
                  value: Any = None,
@@ -18,27 +18,27 @@
         :param value: name of the tab to be initially selected
         :param on_change: callback to be executed when the selected tab changes
         """
         super().__init__(tag='q-tabs', value=value, on_value_change=on_change)
         self.panels: Optional[TabPanels] = None
 
 
-class Tab(Element):
+class Tab(DisableableElement):
 
     def __init__(self, name: str, label: Optional[str] = None, icon: Optional[str] = None) -> None:
         """Tab
 
         This element represents `Quasar's QTab <https://quasar.dev/vue-components/tabs#qtab-api>`_ component.
         It is a child of a `Tabs` element.
 
         :param name: name of the tab (the value of the `Tabs` element)
         :param label: label of the tab (default: `None`, meaning the same as `name`)
         :param icon: icon of the tab (default: `None`)
         """
-        super().__init__('q-tab')
+        super().__init__(tag='q-tab')
         self._props['name'] = name
         self._props['label'] = label if label is not None else name
         if icon:
             self._props['icon'] = icon
         self.tabs = globals.get_slot().parent
 
 
@@ -61,19 +61,19 @@
         :param animated: whether the tab panels should be animated (default: `True`)
         """
         super().__init__(tag='q-tab-panels', value=value, on_value_change=on_change)
         tabs.bind_value(self, 'value')
         self._props['animated'] = animated
 
 
-class TabPanel(Element):
+class TabPanel(DisableableElement):
 
     def __init__(self, name: str) -> None:
         """Tab Panel
 
         This element represents `Quasar's QTabPanel <https://quasar.dev/vue-components/tab-panels#qtabpanel-api>`_ component.
         It is a child of a `TabPanels` element.
 
         :param name: name of the tab panel (the value of the `TabPanels` element)
         """
-        super().__init__('q-tab-panel')
+        super().__init__(tag='q-tab-panel')
         self._props['name'] = name
```

### Comparing `nicegui-1.2.8/nicegui/elements/textarea.py` & `nicegui-1.2.9/nicegui/elements/textarea.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/time.py` & `nicegui-1.2.9/nicegui/elements/time.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Optional
 
+from .mixins.disableable_element import DisableableElement
 from .mixins.value_element import ValueElement
 
 
-class Time(ValueElement):
+class Time(ValueElement, DisableableElement):
 
     def __init__(self,
                  value: Optional[str] = None,
                  *,
                  mask: str = 'HH:mm',
                  on_change: Optional[Callable] = None) -> None:
         """Time Input
```

### Comparing `nicegui-1.2.8/nicegui/elements/toggle.py` & `nicegui-1.2.9/nicegui/elements/toggle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from .choice_element import ChoiceElement
+from .mixins.disableable_element import DisableableElement
 
 
-class Toggle(ChoiceElement):
+class Toggle(ChoiceElement, DisableableElement):
 
     def __init__(self, options: Union[List, Dict], *, value: Any = None, on_change: Optional[Callable] = None) -> None:
         """Toggle
 
         The options can be specified as a list of values, or as a dictionary mapping values to labels.
         After manipulating the options, call `update()` to update the options in the UI.
```

### Comparing `nicegui-1.2.8/nicegui/elements/tree.py` & `nicegui-1.2.9/nicegui/elements/tree.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/elements/upload.py` & `nicegui-1.2.9/nicegui/elements/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Callable, Optional
 
 from fastapi import Request, Response
 
-from ..element import Element
+from ..dependencies import register_component
 from ..events import EventArguments, UploadEventArguments, handle_event
 from ..nicegui import app
+from .mixins.disableable_element import DisableableElement
 
+register_component('upload', __file__, 'upload.js')
 
-class Upload(Element):
+
+class Upload(DisableableElement):
 
     def __init__(self, *,
                  multiple: bool = False,
                  max_file_size: Optional[int] = None,
                  max_total_size: Optional[int] = None,
                  max_files: Optional[int] = None,
                  on_upload: Optional[Callable] = None,
@@ -28,15 +31,15 @@
         :param max_total_size: maximum total size of all files in bytes (default: `0`)
         :param max_files: maximum number of files (default: `0`)
         :param on_upload: callback to execute for each uploaded file (type: nicegui.events.UploadEventArguments)
         :param on_rejected: callback to execute for each rejected file
         :param label: label for the uploader (default: `''`)
         :param auto_upload: automatically upload files when they are selected (default: `False`)
         """
-        super().__init__('q-uploader')
+        super().__init__(tag='upload')
         self._props['multiple'] = multiple
         self._props['label'] = label
         self._props['auto-upload'] = auto_upload
         self._props['url'] = f'/_nicegui/client/{self.client.id}/upload/{self.id}'
 
         if max_file_size is not None:
             self._props['max-file-size'] = max_file_size
```

### Comparing `nicegui-1.2.8/nicegui/elements/video.py` & `nicegui-1.2.9/nicegui/elements/video.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/error.py` & `nicegui-1.2.9/nicegui/error.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/event_listener.py` & `nicegui-1.2.9/nicegui/event_listener.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/events.py` & `nicegui-1.2.9/nicegui/events.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/favicon.py` & `nicegui-1.2.9/nicegui/favicon.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/functions/javascript.py` & `nicegui-1.2.9/nicegui/functions/javascript.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/functions/notify.py` & `nicegui-1.2.9/nicegui/functions/notify.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/functions/open.py` & `nicegui-1.2.9/nicegui/functions/open.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/functions/timer.py` & `nicegui-1.2.9/nicegui/functions/timer.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/globals.py` & `nicegui-1.2.9/nicegui/globals.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/helpers.py` & `nicegui-1.2.9/nicegui/helpers.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/json/__init__.py` & `nicegui-1.2.9/nicegui/json/__init__.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/json/builtin_wrapper.py` & `nicegui-1.2.9/nicegui/json/builtin_wrapper.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/json/orjson_wrapper.py` & `nicegui-1.2.9/nicegui/json/orjson_wrapper.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/native_mode.py` & `nicegui-1.2.9/nicegui/native_mode.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/nicegui.py` & `nicegui-1.2.9/nicegui/nicegui.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from pathlib import Path
 from typing import Dict, Optional
 
 from fastapi import HTTPException, Request
 from fastapi.middleware.gzip import GZipMiddleware
 from fastapi.responses import FileResponse, Response
+from fastapi.staticfiles import StaticFiles
 from fastapi_socketio import SocketManager
 
 from nicegui import json
 from nicegui.json import NiceGUIJSONResponse
 
 from . import __version__, background_tasks, binding, globals, outbox
 from .app import App
@@ -24,33 +25,28 @@
 
 globals.app = app = App(default_response_class=NiceGUIJSONResponse)
 # NOTE we use custom json module which wraps orjson
 socket_manager = SocketManager(app=app, mount_location='/_nicegui_ws/', json=json)
 globals.sio = sio = app.sio
 
 app.add_middleware(GZipMiddleware)
+static_files = StaticFiles(
+    directory=(Path(__file__).parent / 'static').resolve(),
+    follow_symlink=True,
+)
+app.mount(f'/_nicegui/{__version__}/static', static_files, name='static')
 
 globals.index_client = Client(page('/'), shared=True).__enter__()
 
 
 @app.get('/')
 def index(request: Request) -> Response:
     return globals.index_client.build_response(request)
 
 
-@app.get(f'/_nicegui/{__version__}' + '/static/{name}')
-def get_static(name: str):
-    return FileResponse(Path(__file__).parent / 'static' / name)
-
-
-@app.get(f'/_nicegui/{__version__}' + '/static/fonts/{name}')
-def get_static(name: str):
-    return FileResponse(Path(__file__).parent / 'static' / 'fonts' / name)
-
-
 @app.get(f'/_nicegui/{__version__}' + '/dependencies/{id}/{name}')
 def get_dependencies(id: int, name: str):
     if id in js_dependencies and js_dependencies[id].path.exists() and js_dependencies[id].path.name == name:
         return FileResponse(js_dependencies[id].path, media_type='text/javascript')
     raise HTTPException(status_code=404, detail=f'dependency "{name}" with ID {id} not found')
```

### Comparing `nicegui-1.2.8/nicegui/outbox.py` & `nicegui-1.2.9/nicegui/outbox.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/page.py` & `nicegui-1.2.9/nicegui/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         :param path: route of the new page (path must start with '/')
         :param title: optional page title
         :param viewport: optional viewport meta tag content
         :param favicon: optional relative filepath or absolute URL to a favicon (default: `None`, NiceGUI icon will be used)
         :param dark: whether to use Quasar's dark mode (defaults to `dark` argument of `run` command)
         :param response_timeout: maximum time for the decorated function to build the page (default: 3.0)
-        :param **kwargs: additional keyword arguments passed to FastAPI's @app.get method
+        :param kwargs: additional keyword arguments passed to FastAPI's @app.get method
         """
         self.path = path
         self.title = title
         self.viewport = viewport
         self.favicon = favicon
         self.dark = dark
         self.response_timeout = response_timeout
```

### Comparing `nicegui-1.2.8/nicegui/page_layout.py` & `nicegui-1.2.9/nicegui/page_layout.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/run.py` & `nicegui-1.2.9/nicegui/run.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/run_with.py` & `nicegui-1.2.9/nicegui/run_with.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/slot.py` & `nicegui-1.2.9/nicegui/slot.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/favicon.ico` & `nicegui-1.2.9/nicegui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxEIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxFIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxGIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxHIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxIIzIXKMny.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxLIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOkCnqEu92Fr1MmgVxMIzIXKMnyrYk.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmWUlfCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfABc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc4AMP6lQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfBxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCBc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCRc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfChc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOlCnqEu92Fr1MmYUtfCxc4AMP6lbBP.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2` & `nicegui-1.2.9/nicegui/static/fonts/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `nicegui-1.2.9/nicegui/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/fonts.css` & `nicegui-1.2.9/nicegui/static/fonts.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/nicegui.css` & `nicegui-1.2.9/nicegui/static/nicegui.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/quasar.prod.css` & `nicegui-1.2.9/nicegui/static/quasar.prod.css`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/quasar.umd.prod.js` & `nicegui-1.2.9/nicegui/static/quasar.umd.prod.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/sad_face.svg` & `nicegui-1.2.9/nicegui/static/sad_face.svg`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/socket.io.min.js` & `nicegui-1.2.9/nicegui/static/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/tailwindcss.min.js` & `nicegui-1.2.9/nicegui/static/tailwindcss.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/vue.global.prod.js` & `nicegui-1.2.9/nicegui/static/vue.global.prod.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/static/vue.min.js` & `nicegui-1.2.9/nicegui/static/vue.min.js`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind.py` & `nicegui-1.2.9/nicegui/tailwind.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/accent_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/accent_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/background_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/background_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/border_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/border_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/border_radius.py` & `nicegui-1.2.9/nicegui/tailwind_types/border_radius.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/border_spacing.py` & `nicegui-1.2.9/nicegui/tailwind_types/border_spacing.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/border_width.py` & `nicegui-1.2.9/nicegui/tailwind_types/border_width.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/box_shadow_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/box_shadow_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/caret_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/caret_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/cursor.py` & `nicegui-1.2.9/nicegui/tailwind_types/cursor.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/divide_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/divide_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/fill.py` & `nicegui-1.2.9/nicegui/tailwind_types/fill.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/flex_basis.py` & `nicegui-1.2.9/nicegui/tailwind_types/flex_basis.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/gap.py` & `nicegui-1.2.9/nicegui/tailwind_types/gap.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/gradient_color_stops.py` & `nicegui-1.2.9/nicegui/tailwind_types/gradient_color_stops.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/grid_column_start_end.py` & `nicegui-1.2.9/nicegui/tailwind_types/grid_column_start_end.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/height.py` & `nicegui-1.2.9/nicegui/tailwind_types/height.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/margin.py` & `nicegui-1.2.9/nicegui/tailwind_types/margin.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/outline_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/outline_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/padding.py` & `nicegui-1.2.9/nicegui/tailwind_types/padding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/ring_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/ring_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/ring_offset_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/ring_offset_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/scroll_margin.py` & `nicegui-1.2.9/nicegui/tailwind_types/scroll_margin.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/scroll_padding.py` & `nicegui-1.2.9/nicegui/tailwind_types/scroll_padding.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/space_between.py` & `nicegui-1.2.9/nicegui/tailwind_types/space_between.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/stroke.py` & `nicegui-1.2.9/nicegui/tailwind_types/stroke.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/text_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/text_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/text_decoration_color.py` & `nicegui-1.2.9/nicegui/tailwind_types/text_decoration_color.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/top_right_bottom_left.py` & `nicegui-1.2.9/nicegui/tailwind_types/top_right_bottom_left.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/translate.py` & `nicegui-1.2.9/nicegui/tailwind_types/translate.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/tailwind_types/width.py` & `nicegui-1.2.9/nicegui/tailwind_types/width.py`

 * *Files identical despite different names*

### Comparing `nicegui-1.2.8/nicegui/templates/index.html` & `nicegui-1.2.9/nicegui/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 props: { props: { type: Object, default: {} } },
                 template: data.template,
               }, {
                 props: props
               }));
             }
             const children = data.ids.map(id => renderRecursively(elements, id));
-            if (name === 'default' && element.text) {
+            if (name === 'default' && element.text !== null) {
               children.unshift(element.text);
             }
             return [ ...rendered, ...children]
           }
         });
         return Vue.h(Vue.resolveComponent(element.tag), props, slots);
       }
```

### Comparing `nicegui-1.2.8/nicegui/ui.py` & `nicegui-1.2.9/nicegui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .elements.card import CardSection as card_section
 from .elements.chart import Chart as chart
 from .elements.checkbox import Checkbox as checkbox
 from .elements.color_input import ColorInput as color_input
 from .elements.color_picker import ColorPicker as color_picker
 from .elements.colors import Colors as colors
 from .elements.column import Column as column
+from .elements.dark_mode import DarkMode as dark_mode
 from .elements.date import Date as date
 from .elements.dialog import Dialog as dialog
 from .elements.expansion import Expansion as expansion
 from .elements.html import Html as html
 from .elements.icon import Icon as icon
 from .elements.image import Image as image
 from .elements.input import Input as input
@@ -62,14 +63,15 @@
 from .elements.upload import Upload as upload
 from .elements.video import Video as video
 from .functions.download import download
 from .functions.html import add_body_html, add_head_html
 from .functions.javascript import run_javascript
 from .functions.notify import notify
 from .functions.open import open
+from .functions.refreshable import refreshable
 from .functions.timer import Timer as timer
 from .functions.update import update
 from .page import page
 from .page_layout import Drawer as drawer
 from .page_layout import Footer as footer
 from .page_layout import Header as header
 from .page_layout import LeftDrawer as left_drawer
```

### Comparing `nicegui-1.2.8/pyproject.toml` & `nicegui-1.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicegui"
-version = "v1.2.8"
+version = "v1.2.9"
 description = "Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/nicegui"
 keywords = ["gui", "ui", "web", "interface", "live"]
 
@@ -14,15 +14,15 @@
 markdown2 = "^2.4.7"
 Pygments = "^2.9.0"
 uvicorn = {extras = ["standard"], version = "^0.20.0"}
 matplotlib = [
     { version = "^3.5.0", markers = "python_version ~= '3.7'"},
     { version = "^3.6.0", markers = "python_version ~= '3.11.0'"},
 ]
-fastapi = "^0.92"
+fastapi = ">=0.92,<1.0.0"
 fastapi-socketio = "^0.0.10"
 vbuild = "^0.8.1"
 watchfiles = "^0.18.1"
 jinja2 = "^3.1.2"
 python-multipart = "^0.0.6"
 plotly = "^5.13.0"
 orjson = {version = "^3.8.6", markers = "platform_machine != 'i386' and platform_machine != 'i686'"} # orjson does not support 32bit
```

### Comparing `nicegui-1.2.8/setup.py` & `nicegui-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*'],
  'nicegui': ['static/*', 'static/fonts/*', 'templates/*'],
  'nicegui.elements': ['lib/*', 'lib/highcharts_modules/*']}
 
 install_requires = \
 ['Pygments>=2.9.0,<3.0.0',
  'fastapi-socketio>=0.0.10,<0.0.11',
- 'fastapi>=0.92,<0.93',
+ 'fastapi>=0.92,<1.0.0',
  'jinja2>=3.1.2,<4.0.0',
  'markdown2>=2.4.7,<3.0.0',
  'plotly>=5.13.0,<6.0.0',
  'python-multipart>=0.0.6,<0.0.7',
  'pywebview>=4.0.2,<5.0.0',
  'typing-extensions>=3.10.0',
  'uvicorn[standard]>=0.20.0,<0.21.0',
@@ -32,15 +32,15 @@
 {':platform_machine != "i386" and platform_machine != "i686"': ['orjson>=3.8.6,<4.0.0'],
  ':python_version ~= "3.11.0"': ['matplotlib>=3.6.0,<4.0.0'],
  ':python_version ~= "3.7"': ['matplotlib>=3.5.0,<4.0.0',
                               'importlib_metadata>=6.0.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'nicegui',
-    'version': '1.2.8',
+    'version': '1.2.9',
     'description': 'Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots',
     'long_description': '<a href="http://nicegui.io/#about">\n  <img src="https://raw.githubusercontent.com/zauberzeug/nicegui/main/sceenshots/ui-elements-narrow.png"\n    width="200" align="right" alt="Try online!" />\n</a>\n\n# NiceGUI\n\nNiceGUI is an easy-to-use, Python-based UI framework, which shows up in your web browser.\nYou can create buttons, dialogs, Markdown, 3D scenes, plots and much more.\n\nIt is great for micro web apps, dashboards, robotics projects, smart home solutions and similar use cases.\nYou can also use it in development, for example when tweaking/configuring a machine learning algorithm or tuning motor controllers.\n\nNiceGUI is available as [PyPI package](https://pypi.org/project/nicegui/), [Docker image](https://hub.docker.com/r/zauberzeug/nicegui) and on [GitHub](https://github.com/zauberzeug/nicegui).\n\n[![PyPI version](https://badge.fury.io/py/nicegui.svg)](https://pypi.org/project/nicegui/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/nicegui)](https://pypi.org/project/nicegui/)\n[![Docker Pulls](https://img.shields.io/docker/pulls/zauberzeug/nicegui)](https://hub.docker.com/r/zauberzeug/nicegui)<br />\n[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/graphs/commit-activity)\n[![GitHub issues](https://img.shields.io/github/issues/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/issues)\n[![GitHub forks](https://img.shields.io/github/forks/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/network)\n[![GitHub stars](https://img.shields.io/github/stars/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/stargazers)\n[![GitHub license](https://img.shields.io/github/license/zauberzeug/nicegui)](https://github.com/zauberzeug/nicegui/blob/main/LICENSE)\n\n## Features\n\n- browser-based graphical user interface\n- implicit reload on code change\n- standard GUI elements like label, button, checkbox, switch, slider, input, file upload, ...\n- simple grouping with rows, columns, cards and dialogs\n- general-purpose HTML and Markdown elements\n- powerful high-level elements to\n  - plot graphs and charts,\n  - render 3D scenes,\n  - get steering events via virtual joysticks\n  - annotate and overlay images\n  - interact with tables\n  - navigate foldable tree structures\n- built-in timer to refresh data in intervals (even every 10 ms)\n- straight-forward data binding to write even less code\n- notifications, dialogs and menus to provide state of the art user interaction\n- shared and individual web pages\n- ability to add custom routes and data responses\n- capture keyboard input for global shortcuts etc.\n- customize look by defining primary, secondary and accent colors\n- live-cycle events and session data\n- runs in Jupyter Notebooks and allows Python\'s interactive mode\n- auto-complete support for Tailwind CSS\n\n## Installation\n\n```bash\npython3 -m pip install nicegui\n```\n\n## Usage\n\nWrite your nice GUI in a file `main.py`:\n\n```python\nfrom nicegui import ui\n\nui.label(\'Hello NiceGUI!\')\nui.button(\'BUTTON\', on_click=lambda: ui.notify(\'button was pressed\'))\n\nui.run()\n```\n\nLaunch it with:\n\n```bash\npython3 main.py\n```\n\nThe GUI is now available through http://localhost:8080/ in your browser.\nNote: NiceGUI will automatically reload the page when you modify the code.\n\n## Documentation and Examples\n\nThe documentation is hosted at [https://nicegui.io/documentation](https://nicegui.io/documentation) and provides plenty of live demos.\nThe whole content of [https://nicegui.io](https://nicegui.io) is [implemented with NiceGUI itself](https://github.com/zauberzeug/nicegui/blob/main/main.py).\n\nYou may also have a look at our [in-depth examples](https://github.com/zauberzeug/nicegui/tree/main/examples) of what you can do with NiceGUI.\n\n## Why?\n\nWe at [Zauberzeug](https://zauberzeug.com) like [Streamlit](https://streamlit.io/)\nbut find it does [too much magic](https://github.com/zauberzeug/nicegui/issues/1#issuecomment-847413651) when it comes to state handling.\nIn search for an alternative nice library to write simple graphical user interfaces in Python we discovered [JustPy](https://justpy.io/).\nAlthough we liked the approach, it is too "low-level HTML" for our daily usage.\nBut it inspired us to use [Vue](https://vuejs.org/) and [Quasar](https://quasar.dev/) for the frontend.\n\nWe have built on top of [FastAPI](https://fastapi.tiangolo.com/),\nwhich itself is based on the ASGI framework [Starlette](https://www.starlette.io/)\nand the ASGI webserver [Uvicorn](https://www.uvicorn.org/)\nbecause of their great performance and ease of use.\n\n## Contributing\n\nThank you for your interest in contributing to NiceGUI! We are thrilled to have you on board and appreciate your efforts to make this project even better.\n\nAs a growing open-source project, we understand that it takes a community effort to achieve our goals. That\'s why we welcome all kinds of contributions, no matter how small or big they are. Whether it\'s adding new features, fixing bugs, improving documentation, or suggesting new ideas, we believe that every contribution counts and adds value to our project.\n\nWe have provided a detailed guide on how to contribute to NiceGUI in our [CONTRIBUTING.md](https://github.com/zauberzeug/nicegui/blob/main/CONTRIBUTING.md) file. We encourage you to read it carefully before making any contributions to ensure that your work aligns with the project\'s goals and standards.\n\nIf you have any questions or need help with anything, please don\'t hesitate to reach out to us. We are always here to support and guide you through the contribution process.\n\n### Included Web Dependencies\n\nSee [DEPENDENCIES.md](https://github.com/zauberzeug/nicegui/blob/main/DEPENDENCIES.md) for a list of web frameworks NiceGUI depends on.\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zauberzeug/nicegui',
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['nicegui',
 'nicegui.elements', 'nicegui.elements.mixins', 'nicegui.functions',
 'nicegui.json', 'nicegui.tailwind_types'] package_data = \ {'': ['*'],
 'nicegui': ['static/*', 'static/fonts/*', 'templates/*'], 'nicegui.elements':
 ['lib/*', 'lib/highcharts_modules/*']} install_requires = \
 ['Pygments>=2.9.0,<3.0.0', 'fastapi-socketio>=0.0.10,<0.0.11',
-'fastapi>=0.92,<0.93', 'jinja2>=3.1.2,<4.0.0', 'markdown2>=2.4.7,<3.0.0',
+'fastapi>=0.92,<1.0.0', 'jinja2>=3.1.2,<4.0.0', 'markdown2>=2.4.7,<3.0.0',
 'plotly>=5.13.0,<6.0.0', 'python-multipart>=0.0.6,<0.0.7',
 'pywebview>=4.0.2,<5.0.0', 'typing-extensions>=3.10.0', 'uvicorn
 [standard]>=0.20.0,<0.21.0', 'vbuild>=0.8.1,<0.9.0',
 'watchfiles>=0.18.1,<0.19.0'] extras_require = \ {':platform_machine != "i386"
 and platform_machine != "i686"': ['orjson>=3.8.6,<4.0.0'], ':python_version ~=
 "3.11.0"': ['matplotlib>=3.6.0,<4.0.0'], ':python_version ~= "3.7"':
 ['matplotlib>=3.5.0,<4.0.0', 'importlib_metadata>=6.0.0,<7.0.0']} setup_kwargs
-= { 'name': 'nicegui', 'version': '1.2.8', 'description': 'Web User Interface
+= { 'name': 'nicegui', 'version': '1.2.9', 'description': 'Web User Interface
 with Buttons, Dialogs, Markdown, 3D Scences and Plots', 'long_description': '\n
 n_width="200"_align="right"_alt="Try_online!"_/>\n\n\n# NiceGUI\n\nNiceGUI is
 an easy-to-use, Python-based UI framework, which shows up in your web
 browser.\nYou can create buttons, dialogs, Markdown, 3D scenes, plots and much
 more.\n\nIt is great for micro web apps, dashboards, robotics projects, smart
 home solutions and similar use cases.\nYou can also use it in development, for
 example when tweaking/configuring a machine learning algorithm or tuning motor
```

### Comparing `nicegui-1.2.8/PKG-INFO` & `nicegui-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegui
-Version: 1.2.8
+Version: 1.2.9
 Summary: Web User Interface with Buttons, Dialogs, Markdown, 3D Scences and Plots
 Home-page: https://github.com/zauberzeug/nicegui
 License: MIT
 Keywords: gui,ui,web,interface,live
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.7,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pygments (>=2.9.0,<3.0.0)
-Requires-Dist: fastapi (>=0.92,<0.93)
+Requires-Dist: fastapi (>=0.92,<1.0.0)
 Requires-Dist: fastapi-socketio (>=0.0.10,<0.0.11)
 Requires-Dist: importlib_metadata (>=6.0.0,<7.0.0) ; python_version ~= "3.7"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown2 (>=2.4.7,<3.0.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0) ; python_version ~= "3.7"
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0) ; python_version ~= "3.11.0"
 Requires-Dist: orjson (>=3.8.6,<4.0.0) ; platform_machine != "i386" and platform_machine != "i686"
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nicegui Version: 1.2.8 Summary: Web User Interface
+Metadata-Version: 2.1 Name: nicegui Version: 1.2.9 Summary: Web User Interface
 with Buttons, Dialogs, Markdown, 3D Scences and Plots Home-page: https://
 github.com/zauberzeug/nicegui License: MIT Keywords: gui,ui,web,interface,live
 Author: Zauberzeug GmbH Author-email: info@zauberzeug.com Requires-Python:
 >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: Pygments (>=2.9.0,<3.0.0) Requires-Dist: fastapi (>=0.92,<0.93) Requires-
-Dist: fastapi-socketio (>=0.0.10,<0.0.11) Requires-Dist: importlib_metadata
-(>=6.0.0,<7.0.0) ; python_version ~= "3.7" Requires-Dist: jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: markdown2 (>=2.4.7,<3.0.0) Requires-Dist:
-matplotlib (>=3.5.0,<4.0.0) ; python_version ~= "3.7" Requires-Dist: matplotlib
-(>=3.6.0,<4.0.0) ; python_version ~= "3.11.0" Requires-Dist: orjson
+Dist: Pygments (>=2.9.0,<3.0.0) Requires-Dist: fastapi (>=0.92,<1.0.0)
+Requires-Dist: fastapi-socketio (>=0.0.10,<0.0.11) Requires-Dist:
+importlib_metadata (>=6.0.0,<7.0.0) ; python_version ~= "3.7" Requires-Dist:
+jinja2 (>=3.1.2,<4.0.0) Requires-Dist: markdown2 (>=2.4.7,<3.0.0) Requires-
+Dist: matplotlib (>=3.5.0,<4.0.0) ; python_version ~= "3.7" Requires-Dist:
+matplotlib (>=3.6.0,<4.0.0) ; python_version ~= "3.11.0" Requires-Dist: orjson
 (>=3.8.6,<4.0.0) ; platform_machine != "i386" and platform_machine != "i686"
 Requires-Dist: plotly (>=5.13.0,<6.0.0) Requires-Dist: python-multipart
 (>=0.0.6,<0.0.7) Requires-Dist: pywebview (>=4.0.2,<5.0.0) Requires-Dist:
 typing-extensions (>=3.10.0) Requires-Dist: uvicorn[standard]
 (>=0.20.0,<0.21.0) Requires-Dist: vbuild (>=0.8.1,<0.9.0) Requires-Dist:
 watchfiles (>=0.18.1,<0.19.0) Project-URL: Repository, https://github.com/
 zauberzeug/nicegui Description-Content-Type: text/markdown [Try_online!] #
```

