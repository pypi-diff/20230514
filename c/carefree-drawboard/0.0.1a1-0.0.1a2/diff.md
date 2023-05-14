# Comparing `tmp/carefree-drawboard-0.0.1a1.tar.gz` & `tmp/carefree-drawboard-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.1a1.tar", last modified: Sat May 13 04:50:28 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.1a2.tar", last modified: Sun May 14 11:10:04 2023, max compression
```

## Comparing `carefree-drawboard-0.0.1a1.tar` & `carefree-drawboard-0.0.1a2.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.841035 carefree-drawboard-0.0.1a1/
--rw-rw-rw-   0        0        0    11557 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a1/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a1/MANIFEST.in
--rw-rw-rw-   0        0        0     9112 2023-05-13 04:50:28.842033 carefree-drawboard-0.0.1a1/PKG-INFO
--rw-rw-rw-   0        0        0     8829 2023-05-06 11:47:25.000000 carefree-drawboard-0.0.1a1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.335828 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9112 2023-05-13 04:50:19.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6334 2023-05-13 04:50:28.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 04:50:19.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 04:50:19.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-05-13 04:50:19.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 04:50:19.000000 carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.347792 carefree-drawboard-0.0.1a1/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.373725 carefree-drawboard-0.0.1a1/cfdraw/.web/
--rw-rw-rw-   0        0        0      137 2023-05-12 19:54:40.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1669 2023-05-13 03:53:38.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.399176 carefree-drawboard-0.0.1a1/cfdraw/.web/src/
--rw-rw-rw-   0        0        0     1007 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1470 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     5509 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.433080 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2316 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9398 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1806 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     1979 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0      236 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/i18n.ts
--rw-rw-rw-   0        0        0     8268 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1448 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     5032 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1118 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.439064 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/
--rw-rw-rw-   0        0        0     6591 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icon-loading.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.445047 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      925 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icons/delete.svg
--rw-rw-rw-   0        0        0     6681 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/loading-page.json
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.483943 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0     2740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      640 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFCircularProgress.tsx
--rw-rw-rw-   0        0        0      359 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      235 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.490439 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1484 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      522 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFInput.tsx
--rw-rw-rw-   0        0        0     1382 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFLoadingPage.tsx
--rw-rw-rw-   0        0        0      984 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFLottie.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.495426 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     5223 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1738 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFText.tsx
--rw-rw-rw-   0        0        0      531 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFTextarea.tsx
--rw-rw-rw-   0        0        0      417 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFTooltip.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.517366 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     1329 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useAuth.ts
--rw-rw-rw-   0        0        0     3077 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4410 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     3943 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      669 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5914 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0    10921 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useSetup.ts
--rw-rw-rw-   0        0        0      163 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.549277 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      954 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1466 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2372 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0    10105 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     2343 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/tooltip.ts
--rw-rw-rw-   0        0        0      976 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.553267 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.574214 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     2196 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
--rw-rw-rw-   0        0        0     3027 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2920 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
--rw-rw-rw-   0        0        0     3394 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1909 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
--rw-rw-rw-   0        0        0     2127 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
--rw-rw-rw-   0        0        0     2621 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.614616 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/
--rw-rw-rw-   0        0        0     3760 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
--rw-rw-rw-   0        0        0      714 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4598 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      854 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1083 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1123 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     1352 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
--rw-rw-rw-   0        0        0     8594 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     4927 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2204 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.627581 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.644536 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1116 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
--rw-rw-rw-   0        0        0     2043 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0     2565 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0     2291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     2620 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      720 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7821 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0    10985 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0      214 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/hooks.ts
--rw-rw-rw-   0        0        0     2295 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.653512 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1960 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/cleanup.ts
--rw-rw-rw-   0        0        0     1450 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0     4048 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.659494 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0     1290 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     2921 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.665478 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.682435 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     5025 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1804 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/fields.ts
--rw-rw-rw-   0        0        0     2076 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0      313 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.717853 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0      792 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/debug.ts
--rw-rw-rw-   0        0        0     1495 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0     1107 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     7336 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/pluginsInfo.ts
--rw-rw-rw-   0        0        0     2060 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/pointerEvents.ts
--rw-rw-rw-   0        0        0     1858 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     1692 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/settings.ts
--rw-rw-rw-   0        0        0     9304 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/socket.ts
--rw-rw-rw-   0        0        0     4852 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2054 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/ui.ts
--rw-rw-rw-   0        0        0      501 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/user.ts
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.731816 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0     3876 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1605 2023-05-12 19:54:40.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0     2041 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1949 2023-05-13 04:28:03.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   224022 2023-05-13 03:53:38.000000 carefree-drawboard-0.0.1a1/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      475 2023-05-08 16:30:47.000000 carefree-drawboard-0.0.1a1/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.739793 carefree-drawboard-0.0.1a1/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     4826 2023-05-13 04:28:05.000000 carefree-drawboard-0.0.1a1/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.758742 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      139 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      745 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/assets.py
--rw-rw-rw-   0        0        0      493 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     6862 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     6918 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/queue.py
--rw-rw-rw-   0        0        0     3577 2023-05-13 04:28:05.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     3672 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0     1277 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3518 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2430 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a1/cfdraw/config.py
--rw-rw-rw-   0        0        0     3012 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.766720 carefree-drawboard-0.0.1a1/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      710 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0    13291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.776697 carefree-drawboard-0.0.1a1/cfdraw/plugins/
--rw-rw-rw-   0        0        0       97 2023-05-08 01:07:56.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.786182 carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/
--rw-rw-rw-   0        0        0       52 2023-05-08 01:08:15.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/__init__.py
--rw-rw-rw-   0        0        0     1399 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/node_validator.py
--rw-rw-rw-   0        0        0     1457 2023-05-08 01:08:43.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/sync.py
--rw-rw-rw-   0        0        0     6755 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.788181 carefree-drawboard-0.0.1a1/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     1918 2023-05-08 01:06:37.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.799151 carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       76 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-05-13 04:28:05.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/response.py
--rw-rw-rw-   0        0        0      904 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/send_message.py
--rw-rw-rw-   0        0        0      643 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/timer.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.811119 carefree-drawboard-0.0.1a1/cfdraw/schema/
--rw-rw-rw-   0        0        0       72 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0    18207 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a1/cfdraw/schema/plugins.py
--rw-rw-rw-   0        0        0     1615 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/schema/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-13 04:50:28.839040 carefree-drawboard-0.0.1a1/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     6551 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/data_structures.py
--rw-rw-rw-   0        0        0     2622 2023-05-12 20:16:11.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0     2415 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/misc.py
--rw-rw-rw-   0        0        0      638 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     4036 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2732 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a1/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-05-13 04:50:28.846024 carefree-drawboard-0.0.1a1/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-05-13 04:50:16.000000 carefree-drawboard-0.0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.099800 carefree-drawboard-0.0.1a2/
+-rw-rw-rw-   0        0        0    11557 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a2/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9112 2023-05-14 11:10:04.099800 carefree-drawboard-0.0.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0     8829 2023-05-06 11:47:25.000000 carefree-drawboard-0.0.1a2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.724903 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9112 2023-05-14 11:09:59.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6337 2023-05-14 11:10:03.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 11:09:59.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 11:09:59.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-05-14 11:09:59.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-14 11:09:59.000000 carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.731856 carefree-drawboard-0.0.1a2/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.746816 carefree-drawboard-0.0.1a2/cfdraw/.web/
+-rw-rw-rw-   0        0        0      137 2023-05-12 19:54:40.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1669 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.762773 carefree-drawboard-0.0.1a2/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0     1012 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1470 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     5509 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.785712 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2316 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9398 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1806 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     1979 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0      236 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/i18n.ts
+-rw-rw-rw-   0        0        0     8268 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1448 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     5032 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1118 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.788704 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/
+-rw-rw-rw-   0        0        0     6591 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icon-loading.json
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.792692 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      925 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icons/delete.svg
+-rw-rw-rw-   0        0        0     6681 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/loading-page.json
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.860510 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0     2740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0      359 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      235 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.864499 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1484 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      522 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFInput.tsx
+-rw-rw-rw-   0        0        0     1382 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFLoadingPage.tsx
+-rw-rw-rw-   0        0        0      984 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFLottie.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.869486 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     5223 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1738 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      740 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFText.tsx
+-rw-rw-rw-   0        0        0      531 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFTextarea.tsx
+-rw-rw-rw-   0        0        0      417 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFTooltip.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.889433 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     1329 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useAuth.ts
+-rw-rw-rw-   0        0        0     2976 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useDocumentEvents.ts
+-rw-rw-rw-   0        0        0     3077 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4410 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     3943 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      669 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5914 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0    10902 2023-05-14 10:39:38.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useSetup.ts
+-rw-rw-rw-   0        0        0      163 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.912371 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      954 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1466 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2372 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0    10105 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     2343 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/tooltip.ts
+-rw-rw-rw-   0        0        0      976 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.914364 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.929325 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     2196 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
+-rw-rw-rw-   0        0        0     3027 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2920 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
+-rw-rw-rw-   0        0        0     3394 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1909 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0     2127 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0     2621 2023-05-12 14:52:45.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.952265 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/
+-rw-rw-rw-   0        0        0     3760 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      714 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4598 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      854 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3546 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1083 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1123 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1352 2023-05-12 19:28:28.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     8594 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     4927 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2204 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.961239 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.972211 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1116 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
+-rw-rw-rw-   0        0        0     2043 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0     2565 2023-05-12 20:46:03.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0     2291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     2620 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      720 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7862 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0    10883 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      214 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2295 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.978193 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1960 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/cleanup.ts
+-rw-rw-rw-   0        0        0     1450 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0     4048 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.981362 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1290 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     2921 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.984943 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:03.995945 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     5025 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1804 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/fields.ts
+-rw-rw-rw-   0        0        0     2076 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0      313 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3514 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.017543 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0      792 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0     1107 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     7527 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/pluginsInfo.ts
+-rw-rw-rw-   0        0        0     1968 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     1716 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/settings.ts
+-rw-rw-rw-   0        0        0     9316 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     4852 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2054 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      501 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.027490 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0     3876 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0     1266 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1605 2023-05-12 19:54:40.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0     2053 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     2069 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   224022 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      475 2023-05-08 16:30:47.000000 carefree-drawboard-0.0.1a2/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.032476 carefree-drawboard-0.0.1a2/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     4826 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a2/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.047434 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     7363 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     6918 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     3577 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3991 2023-05-14 10:39:38.000000 carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1277 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3518 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2430 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a2/cfdraw/config.py
+-rw-rw-rw-   0        0        0     3045 2023-05-14 10:23:43.000000 carefree-drawboard-0.0.1a2/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.052423 carefree-drawboard-0.0.1a2/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0    13291 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.058406 carefree-drawboard-0.0.1a2/cfdraw/plugins/
+-rw-rw-rw-   0        0        0       97 2023-05-08 01:07:56.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.063393 carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/
+-rw-rw-rw-   0        0        0       52 2023-05-08 01:08:15.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/__init__.py
+-rw-rw-rw-   0        0        0     1399 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/node_validator.py
+-rw-rw-rw-   0        0        0     1457 2023-05-08 01:08:43.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/sync.py
+-rw-rw-rw-   0        0        0     6755 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.065388 carefree-drawboard-0.0.1a2/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     1918 2023-05-08 01:06:37.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.072369 carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       76 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/response.py
+-rw-rw-rw-   0        0        0      904 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      643 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/timer.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.079374 carefree-drawboard-0.0.1a2/cfdraw/schema/
+-rw-rw-rw-   0        0        0       72 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    18207 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a2/cfdraw/schema/plugins.py
+-rw-rw-rw-   0        0        0     1615 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/schema/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:10:04.097806 carefree-drawboard-0.0.1a2/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     6551 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/data_structures.py
+-rw-rw-rw-   0        0        0     2622 2023-05-12 20:16:11.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     2415 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     4036 2023-05-12 20:35:16.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2732 2023-05-07 12:33:13.000000 carefree-drawboard-0.0.1a2/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-05-14 11:10:04.101766 carefree-drawboard-0.0.1a2/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-05-14 11:08:54.000000 carefree-drawboard-0.0.1a2/setup.py
```

### Comparing `carefree-drawboard-0.0.1a1/LICENSE` & `carefree-drawboard-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/PKG-INFO` & `carefree-drawboard-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.1a1/README.md` & `carefree-drawboard-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.1a1/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.1a2/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 cfdraw/.web/src/components/CFTextarea.tsx
 cfdraw/.web/src/components/CFTooltip.tsx
 cfdraw/.web/src/components/CFIcon/index.scss
 cfdraw/.web/src/components/CFIcon/index.tsx
 cfdraw/.web/src/components/CFSelect/index.scss
 cfdraw/.web/src/components/CFSelect/index.tsx
 cfdraw/.web/src/hooks/useAuth.ts
+cfdraw/.web/src/hooks/useDocumentEvents.ts
 cfdraw/.web/src/hooks/useFileDropper.ts
 cfdraw/.web/src/hooks/useGridLines.ts
 cfdraw/.web/src/hooks/useInitBoard.ts
 cfdraw/.web/src/hooks/usePreventDefaults.ts
 cfdraw/.web/src/hooks/usePython.ts
 cfdraw/.web/src/hooks/useSetup.ts
 cfdraw/.web/src/lang/add.ts
@@ -124,15 +125,14 @@
 cfdraw/.web/src/schema/plugins.ts
 cfdraw/.web/src/schema/requests.ts
 cfdraw/.web/src/stores/debug.ts
 cfdraw/.web/src/stores/gridLines.ts
 cfdraw/.web/src/stores/hooks.ts
 cfdraw/.web/src/stores/meta.ts
 cfdraw/.web/src/stores/pluginsInfo.ts
-cfdraw/.web/src/stores/pointerEvents.ts
 cfdraw/.web/src/stores/projects.ts
 cfdraw/.web/src/stores/settings.ts
 cfdraw/.web/src/stores/socket.ts
 cfdraw/.web/src/stores/theme.ts
 cfdraw/.web/src/stores/ui.ts
 cfdraw/.web/src/stores/user.ts
 cfdraw/.web/src/utils/bem.ts
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/package.json` & `carefree-drawboard-0.0.1a2/cfdraw/.web/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950738916256158%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '~0.5.1-alpha.7', '@carefree0910/core': "*

 * *                   "'~0.5.1-alpha.7', '@carefree0910/native': '~0.5.1-alpha.7', "*

 * *                   "'@carefree0910/svg': '~0.5.1-alpha.7'}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "dependencies": {
-        "@carefree0910/business": "~0.5.1-alpha.6",
-        "@carefree0910/core": "~0.5.1-alpha.6",
-        "@carefree0910/native": "~0.5.1-alpha.6",
-        "@carefree0910/svg": "~0.5.1-alpha.6",
+        "@carefree0910/business": "~0.5.1-alpha.7",
+        "@carefree0910/core": "~0.5.1-alpha.7",
+        "@carefree0910/native": "~0.5.1-alpha.7",
+        "@carefree0910/svg": "~0.5.1-alpha.7",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/App.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
 import { useSetup } from "./hooks/useSetup";
 import { useWebSocket } from "./stores/socket";
-import { usePointerEvents } from "./stores/pointerEvents";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
+import { useDocumentEvents } from "./hooks/useDocumentEvents";
 import CFLoadingPage from "./components/CFLoadingPage";
 import BoardPanel from "./BoardPanel";
 
 function App() {
   useSetup();
   useWebSocket();
   useInitBoard();
   useFileDropper();
   useGridLines();
   usePreventDefaults();
-  usePointerEvents();
+  useDocumentEvents();
 
   return (
     <Flex h="100vh" className="p-editor" direction="column" userSelect="none">
       <Flex w="100%" flex={1}>
         <CFLoadingPage>
           <BoardPanel />
         </CFLoadingPage>
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/_settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/importMeta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icon-loading.json` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icon-loading.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/icons/delete.svg` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/assets/loading-page.json` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/assets/loading-page.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFButton.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFButton.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFCircularProgress.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFCircularProgress.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFInput.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFInput.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFLoadingPage.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFLoadingPage.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFLottie.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFLottie.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFText.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFText.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/components/CFTextarea.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/components/CFTextarea.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useAuth.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useAuth.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/usePreventDefaults.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/usePreventDefaults.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/usePython.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/hooks/useSetup.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/hooks/useSetup.ts`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
   getHash,
   sleep,
 } from "@carefree0910/core";
 import { ABCStore, langStore } from "@carefree0910/business";
 
 import type { IPythonOnSocketMessage, IPythonSocketRequest } from "@/schema/_python";
 import { useReactPluginSettings } from "@/_settings";
-import { cleanURL, getBaseURL } from "@/utils/misc";
-import { IMAGE_PLACEHOLDER, IS_PROD } from "@/utils/constants";
+import { getBaseURL } from "@/utils/misc";
+import { IMAGE_PLACEHOLDER } from "@/utils/constants";
 import { ThemeType, allThemes, themeStore } from "@/stores/theme";
 import { userStore } from "@/stores/user";
 import { debugStore } from "@/stores/debug";
 import { getNewUpdateTime } from "@/stores/projects";
 import { ISettingsStore, settingsStore, useSettingsSynced } from "@/stores/settings";
 import {
   IProject,
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/tooltip.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/tooltip.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/lang/ui.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/PluginGroup.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/PluginGroup.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/QAPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_python/hooks.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_python/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/AddPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/AddPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import { themeStore, useScrollBarSx } from "@/stores/theme";
 import {
   usePluginMessage,
   usePluginIsExpanded,
   setPluginExpanded,
   usePluginGroupIsExpanded,
 } from "@/stores/pluginsInfo";
-import { isInteractingWithBoard } from "@/stores/pointerEvents";
+import { isInteractingWithBoard } from "@/hooks/useDocumentEvents";
 import { parseIStr } from "@/actions/i18n";
 import CFText from "@/components/CFText";
 import { CFIconButton } from "@/components/CFButton";
 import { CFPendingProgress, CFWorkingProgress } from "@/components/CFCircularProgress";
 
 export function getExpandId(id: string): string {
   return `${id}_expand`;
@@ -184,14 +184,15 @@
             setPluginExpanded(id, !expand);
           }
           onFloatingButtonClick?.();
         }}
         opacity={isInvisible ? 0 : 1}
         visibility={isInvisible ? "hidden" : "visible"}
         transition={`${VISIBILITY_TRANSITION}, ${BG_TRANSITION}`}
+        _focus={{ outline: "none" }}
         {...getCommonProps(false)}
         {...props}
         imageProps={{ opacity: iconOpacity }}>
         {taskMessage && isBusy && (
           <Box w={`${iconW}px`} h={`${iconH}px`} position="absolute" left="0px" top="0px">
             {taskMessage.status === "pending" ? (
               <CFPendingProgress
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,14 @@
   useEffect(() => {
     let latest = true;
     const timer = setTimeout(() => {
       renderFilter(info).then((filter) => {
         if (!latest) return;
         if (!filter) {
           setPluginNeedRender(_id, false);
-        } else if (inGroup && !groupExpand && !expand) {
-          setPluginNeedRender(_id, false);
         } else {
           setPluginNeedRender(_id, true);
         }
       });
     }, 0);
     return () => {
       latest = false;
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/cleanup.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/cleanup.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/fields.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/fields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/debug.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/debug.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/pluginsInfo.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/pluginsInfo.ts`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,18 @@
 // hierarchy
 export const usePluginChildren = (groupId: string) =>
   pluginsInfoStore.setDefault("hierarchy", {
     key: groupId,
     hasEffect: false,
     getDefault: () => [],
   });
+export const usePluginParent = (id: string) => {
+  const hierarchy = pluginsInfoStore.hierarchy;
+  return Object.entries(hierarchy).find(([, children]) => children.includes(id))?.[0];
+};
 export const addPluginChild = (groupId: string, id: string) => {
   const children = usePluginChildren(groupId);
   if (!children.includes(id)) {
     runInAction(() => children.push(id));
   }
 };
 // updaters
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/projects.ts`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,26 @@
   uid: string;
   name: string;
   createTime: number;
   updateTime: number;
 }
 type IPartialProjectsStore = Partial<IProjectsStore>;
 class ProjectsStore extends ABCStore<IPartialProjectsStore> implements IPartialProjectsStore {
-  uid?: string;
-  name?: string;
-  createTime?: number;
-  updateTime?: number;
+  uid?: string = undefined;
+  name?: string = undefined;
+  createTime?: number = undefined;
+  updateTime?: number = undefined;
 
   constructor() {
     super();
     makeObservable(this, {
       uid: observable,
       name: observable,
+      createTime: observable,
+      updateTime: observable,
     });
   }
 
   get info(): IPartialProjectsStore {
     return this;
   }
 }
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/settings.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/settings.ts`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,16 @@
   pluginSettings: IMakePlugin<PythonPlugins>[];
   internalSettings?: IInternalSettings;
   boardSettings?: IBoardSettings;
 }
 class SettingsStore extends ABCStore<ISettingsStore> implements ISettingsStore {
   hash: string = "";
   pluginSettings: IMakePlugin<PythonPlugins>[] = [];
-  boardSettings?: IBoardSettings;
-  internalSettings?: IInternalSettings;
+  boardSettings?: IBoardSettings = undefined;
+  internalSettings?: IInternalSettings = undefined;
 
   constructor() {
     super();
     makeObservable(this, {
       hash: observable,
       pluginSettings: observable,
       internalSettings: observable,
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/socket.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/socket.ts`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 export interface ISocketStore {
   socket?: WebSocket;
   shouldTerminate: boolean;
   hooks: Bundle<SocketHook<any>>;
 }
 class SocketStore extends ABCStore<ISocketStore> implements ISocketStore {
-  socket?: WebSocket;
+  socket?: WebSocket = undefined;
   shouldTerminate: boolean = false;
   hooks = new Bundle<SocketHook<any>>([]);
 
   constructor() {
     super();
     makeObservable(this, {
       socket: observable,
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/theme.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/constants.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/constants.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/src/utils/toast.ts`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import { ABCStore, langStore, translate } from "@carefree0910/business";
 import { settingsStore } from "@/stores/settings";
 
 export interface IToastStore {
   timer: any;
 }
 class ToastStore extends ABCStore<IToastStore> implements IToastStore {
-  timer: any;
+  timer: any = undefined;
 
   constructor() {
     super();
     makeObservable(this, {
       timer: observable,
     });
   }
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.1a2/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.1a2/cfdraw/.web/vite.config.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import { defineConfig } from "vite";
+import path from "path";
 import svgr from "vite-plugin-svgr";
 import react from "@vitejs/plugin-react";
 import tsconfigPaths from "vite-tsconfig-paths";
 // import { visualizer } from "rollup-plugin-visualizer";
 
 // https://vitejs.dev/config/
 export default defineConfig({
+  resolve: {
+    alias: [{ find: "@", replacement: path.resolve(__dirname, "src") }],
+  },
   plugins: [
     react(),
     tsconfigPaths(),
     svgr({
       svgrOptions: {
         // svgr options
       },
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.1a2/cfdraw/.web/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -213,41 +213,41 @@
   resolved "https://registry.npmmirror.com/@babel/types/-/types-7.21.5.tgz#18dfbd47c39d3904d5db3d3dc2cc80bedb60e5b6"
   integrity sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==
   dependencies:
     "@babel/helper-string-parser" "^7.21.5"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@~0.5.1-alpha.6":
-  version "0.5.1-alpha.6"
-  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.6.tgz#5702af5f37e47aa48b35fde07352d9c0d4682e82"
-  integrity sha512-PiaPZaju7C5G3pJZ4VsXq3tRtJ+3q9kubeGPIw73P+T/TI0ClXYTxyoL6OOqKV+swlypjRyFHf5dHw1Z2RLXXQ==
+"@carefree0910/business@~0.5.1-alpha.7":
+  version "0.5.1-alpha.7"
+  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.7.tgz#845cff7349c1c8a56335d9d44169fb44d55efee0"
+  integrity sha512-JR+KAzbR70X8JZ36nqSATgJs8MHwsscsOW4jxKbS8H1TAVyNHHQ5y3+NH5RpeLYkxKcLG9ucyrhleITAAJ3JQQ==
   dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.6"
-    "@carefree0910/svg" "^0.5.1-alpha.6"
+    "@carefree0910/core" "^0.5.1-alpha.7"
+    "@carefree0910/svg" "^0.5.1-alpha.7"
 
-"@carefree0910/core@^0.5.1-alpha.6", "@carefree0910/core@~0.5.1-alpha.6":
-  version "0.5.1-alpha.6"
-  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.6.tgz#de51012746b5a573212b858d72700a5c92d951b1"
-  integrity sha512-3hgAgROo2utviZ3F3+sdxNCzLZIJ4ga8ZR7IIe4Fkopbn5i3pjbMaReWhu09bxMFYzHx+GydqgWvAbL9b7ETkw==
+"@carefree0910/core@^0.5.1-alpha.7", "@carefree0910/core@~0.5.1-alpha.7":
+  version "0.5.1-alpha.7"
+  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.7.tgz#5af9f207fa75a32db031f51ddf40461cc9cd539d"
+  integrity sha512-pNTkZ1Lg4+jQVCrKEhC6tkElnYsJ38Jxm9qpjcIOnFlpCCGfTld5LEmtpeYOMtbMSRSe305ENxTilgahTl2y1Q==
 
-"@carefree0910/native@~0.5.1-alpha.6":
-  version "0.5.1-alpha.6"
-  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.6.tgz#683911b0173e51253b90bd10dcead18e60d7497c"
-  integrity sha512-qBsS9atYwuUOC7yd8sTer9zVwi2jInUYsaA/HhWAZjVJebp4KXMBRFFDziYgnjTZdhMfI4S8GsriOvRsTraVIQ==
+"@carefree0910/native@~0.5.1-alpha.7":
+  version "0.5.1-alpha.7"
+  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.7.tgz#d7654a461d2c087f22cd0c68adac4cd5cdb6ca36"
+  integrity sha512-zqrgms0wwYDBY13i+MqxuepowkuF2nrdcf6JtIDOBcR2BQ/yE8fM6cydxmXo+GUV79g7NCWQteaM5YD4UN9aeQ==
   dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.6"
-    "@carefree0910/svg" "^0.5.1-alpha.6"
+    "@carefree0910/core" "^0.5.1-alpha.7"
+    "@carefree0910/svg" "^0.5.1-alpha.7"
 
-"@carefree0910/svg@^0.5.1-alpha.6", "@carefree0910/svg@~0.5.1-alpha.6":
-  version "0.5.1-alpha.6"
-  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.6.tgz#2e011ff43e10a28e292e66c30db27225e659da45"
-  integrity sha512-1tRww/9o33NHc5BtsCYGTe/lN6Dx5HxR75Iz+JW27Fa9Ugvb8+5+qrojbuYk2va+wC1EMJ1OXT1o9XBH6pRJ7g==
+"@carefree0910/svg@^0.5.1-alpha.7", "@carefree0910/svg@~0.5.1-alpha.7":
+  version "0.5.1-alpha.7"
+  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.7.tgz#0801741d01197984c70507895970fe363317c88a"
+  integrity sha512-LW5gowN7UCAGY2gNtKFGEX33dVHU0N0EZ0vxnoDiuR0VSLtq/S9LcXyDO1t36suRzkkfStKd6nHvhwFikyE/dA==
   dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.6"
+    "@carefree0910/core" "^0.5.1-alpha.7"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.npmmirror.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/app.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/assets.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,22 +59,32 @@
                 print_warning("project meta file is not up-to-date")
         except Exception as err:
             print_warning(f"failed to check project meta file: {get_err_msg(err)}")
     if checked:
         return
     project_meta = {}
     for path in existing_projects:
-        with open(path, "r") as f:
-            d = json.load(f)
-        project_meta[d["uid"]] = dict(
-            uid=d["uid"],
-            name=d["name"],
-            createTime=d["createTime"],
-            updateTime=d["updateTime"],
-        )
+        try:
+            with open(path, "r") as f:
+                d = json.load(f)
+            project_meta[d["uid"]] = dict(
+                uid=d["uid"],
+                name=d["name"],
+                createTime=d["createTime"],
+                updateTime=d["updateTime"],
+            )
+        except Exception as err:
+            buggy_folder = upload_project_folder / constants.BUGGY_PROJECT_FOLDER
+            buggy_folder.mkdir(parents=True, exist_ok=True)
+            backup_path = buggy_folder / path.name
+            print_warning(
+                f"failed to load project '{path}', it will be moved to '{backup_path}'"
+                f" ({get_err_msg(err)})"
+            )
+            path.rename(buggy_folder / path.name)
     with open(meta_path, "w") as f:
         json.dump(project_meta, f)
 
 
 def maintain_all_meta(app: IApp) -> None:
     for user_folder in app.config.upload_project_folder.iterdir():
         if user_folder.is_dir():
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/queue.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/queue.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/upload.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/endpoints/websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             if websocket.client_state == WebSocketState.DISCONNECTED:
                 return False
             await websocket.send_text(json.dumps(data.dict()))
             return True
 
         await websocket.accept()
         while True:
+            raw_data = data = None
             try:
                 target_plugin = None
                 raw_data = await websocket.receive_text()
                 data = ISocketRequest(**json.loads(raw_data))
                 if data.isInternal:
                     identifier = data.identifier
                     target_plugin = app.internal_plugins.make(identifier)
@@ -71,15 +72,21 @@
                     )
                     exception = ISocketMessage.make_exception(data.hash, message)
                     if not await send_message(exception):
                         print_error(f"[websocket.loop] {message}")
             except WebSocketDisconnect:
                 break
             except Exception as e:
-                await on_failed(e, data.hash)
+                if data is not None:
+                    req_hash = data.hash
+                elif raw_data is not None and isinstance(raw_data, dict):
+                    req_hash = raw_data.get("hash", "unknown")
+                else:
+                    req_hash = "unknown"
+                await on_failed(e, req_hash)
             finally:
                 del target_plugin
 
 
 class WebsocketEndpoint(IEndpoint):
     def register(self) -> None:
         add_websocket(self.app)
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/app/schema.py` & `carefree-drawboard-0.0.1a2/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/cli.py` & `carefree-drawboard-0.0.1a2/cfdraw/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/config.py` & `carefree-drawboard-0.0.1a2/cfdraw/config.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/constants.py` & `carefree-drawboard-0.0.1a2/cfdraw/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 ## common
 ROOT = Path(os.path.dirname(__file__))
 WEB_ROOT = ROOT / ".web"
 ## upload
 UPLOAD_ROOT = Path("~").expanduser() / ".cache" / "carefree-draw"
 UPLOAD_IMAGE_FOLDER_NAME = ".images"
 UPLOAD_PROJECT_FOLDER_NAME = ".projects"
+BUGGY_PROJECT_FOLDER = ".buggy"
 PROJECT_META_FILE = "_meta.json"
 
 # icons
 TEXT_TO_IMAGE_ICON = "https://user-images.githubusercontent.com/15677328/234642061-98636956-4e3b-44ef-a670-a478bc9eb4ca.svg"
 IMAGE_TO_IMAGE_ICON = "https://user-images.githubusercontent.com/15677328/234642045-0416300a-8475-4afa-8285-88c0eee93c07.svg"
 IMAGE_TO_TEXT_ICON = "https://user-images.githubusercontent.com/15677328/234642056-79e20fc9-0005-4e0e-8365-3285af8803ae.svg"
 CONTROLNET_ICON = IMAGE_TO_IMAGE_ICON
```

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.1a2/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.1a2/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/node_validator.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/node_validator.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/_internal/sync.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/_internal/sync.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/base.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/response.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/response.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/send_message.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/send_message.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.1a2/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.1a2/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.1a2/cfdraw/schema/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/schema/settings.py` & `carefree-drawboard-0.0.1a2/cfdraw/schema/settings.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/console.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/data_structures.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/misc.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/misc.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/server.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/cfdraw/utils/template.py` & `carefree-drawboard-0.0.1a2/cfdraw/utils/template.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a1/setup.py` & `carefree-drawboard-0.0.1a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1-alpha.1"
+VERSION = "0.0.1-alpha.2"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

