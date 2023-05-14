# Comparing `tmp/datagen_tech-1.9.0rc1.tar.gz` & `tmp/datagen_tech-1.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagen_tech-1.9.0rc1.tar", max compression
+gzip compressed data, was "datagen_tech-1.9.0rc2.tar", max compression
```

## Comparing `datagen_tech-1.9.0rc1.tar` & `datagen_tech-1.9.0rc2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    11354 2022-12-28 14:41:11.697060 datagen_tech-1.9.0rc1/LICENSE
--rw-r--r--   0        0        0     7175 2022-12-28 14:41:11.697199 datagen_tech-1.9.0rc1/README.md
--rw-r--r--   0        0        0     1987 2023-03-30 15:28:15.843294 datagen_tech-1.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0      244 2022-12-25 10:08:42.081571 datagen_tech-1.9.0rc1/src/datagen/__init__.py
--rw-r--r--   0        0        0      447 2023-01-24 14:24:26.735850 datagen_tech-1.9.0rc1/src/datagen/api/__init__.py
--rw-r--r--   0        0        0       42 2023-03-26 09:01:52.298232 datagen_tech-1.9.0rc1/src/datagen/api/assets.py
--rw-r--r--   0        0        0      230 2022-12-25 10:08:42.084256 datagen_tech-1.9.0rc1/src/datagen/api/catalog/__init__.py
--rw-r--r--   0        0        0      355 2023-03-13 15:06:42.405987 datagen_tech-1.9.0rc1/src/datagen/api/catalog/attributes.py
--rw-r--r--   0        0        0    40406 2023-03-19 16:53:42.795114 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/backgrounds.json
--rw-r--r--   0        0        0     3482 2023-02-06 16:46:30.755604 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/beards.json
--rw-r--r--   0        0        0   600982 2023-02-07 09:24:05.035297 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/eyebrows.json
--rw-r--r--   0        0        0    46067 2023-02-12 06:59:13.716940 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/eyes.json
--rw-r--r--   0        0        0     1358 2023-02-06 16:46:30.757951 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/glasses.json
--rw-r--r--   0        0        0    68866 2023-02-20 14:55:17.995340 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hair.json
--rw-r--r--   0        0        0   406568 2023-03-30 14:33:54.272534 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hic/attributes.json
--rw-r--r--   0        0        0  3147694 2023-03-30 14:33:54.277071 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hic/presets.json
--rw-r--r--   0        0        0  6032881 2023-02-06 16:46:25.148161 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/humans/attributes.json
--rw-r--r--   0        0        0 29256791 2023-01-22 11:34:49.658350 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/humans/defaults.json
--rw-r--r--   0        0        0      174 2023-03-16 11:32:41.011645 datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/masks.json
--rw-r--r--   0        0        0     2680 2023-02-02 09:05:36.527979 datagen_tech-1.9.0rc1/src/datagen/api/catalog/containers.py
--rw-r--r--   0        0        0      121 2023-02-02 09:05:36.528188 datagen_tech-1.9.0rc1/src/datagen/api/catalog/hooks/__init__.py
--rw-r--r--   0        0        0      434 2023-03-28 07:24:32.391005 datagen_tech-1.9.0rc1/src/datagen/api/catalog/hooks/hic.py
--rw-r--r--   0        0        0      758 2023-02-02 09:05:36.528562 datagen_tech-1.9.0rc1/src/datagen/api/catalog/hooks/humans.py
--rw-r--r--   0        0        0     9891 2023-03-09 09:15:02.795423 datagen_tech-1.9.0rc1/src/datagen/api/catalog/impl.py
--rw-r--r--   0        0        0        0 2023-01-23 13:07:38.623174 datagen_tech-1.9.0rc1/src/datagen/api/client/__init__.py
--rw-r--r--   0        0        0     1126 2023-03-09 09:15:02.795628 datagen_tech-1.9.0rc1/src/datagen/api/client/containers.py
--rw-r--r--   0        0        0     1750 2023-03-09 09:15:02.795946 datagen_tech-1.9.0rc1/src/datagen/api/client/exceptions.py
--rw-r--r--   0        0        0     3324 2023-03-16 11:32:41.012269 datagen_tech-1.9.0rc1/src/datagen/api/client/schemas.py
--rw-r--r--   0        0        0      891 2023-03-09 09:15:02.796547 datagen_tech-1.9.0rc1/src/datagen/api/client/session.py
--rw-r--r--   0        0        0      267 2023-03-09 09:15:02.796846 datagen_tech-1.9.0rc1/src/datagen/api/containers.py
--rw-r--r--   0        0        0      276 2023-01-23 13:07:38.624232 datagen_tech-1.9.0rc1/src/datagen/api/datapoint/__init__.py
--rw-r--r--   0        0        0     4117 2023-03-30 15:18:02.416624 datagen_tech-1.9.0rc1/src/datagen/api/impl.py
--rw-r--r--   0        0        0        0 2022-11-30 13:20:55.785436 datagen_tech-1.9.0rc1/src/datagen/api/requests/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 13:20:55.785474 datagen_tech-1.9.0rc1/src/datagen/api/requests/datapoint/__init__.py
--rw-r--r--   0        0        0     1377 2023-03-09 09:15:02.797323 datagen_tech-1.9.0rc1/src/datagen/api/requests/datapoint/builder.py
--rw-r--r--   0        0        0      579 2023-03-09 09:15:12.309229 datagen_tech-1.9.0rc1/src/datagen/api/requests/director.py
--rw-r--r--   0        0        0      248 2022-11-20 11:34:39.385633 datagen_tech-1.9.0rc1/src/datagen/components/__init__.py
--rw-r--r--   0        0        0     1348 2022-11-20 11:34:39.385695 datagen_tech-1.9.0rc1/src/datagen/components/camera.py
--rw-r--r--   0        0        0      231 2022-11-20 11:34:39.385769 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/__init__.py
--rw-r--r--   0        0        0      815 2022-11-30 13:20:55.785678 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/container.py
--rw-r--r--   0        0        0        0 2022-11-20 11:34:39.385875 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/__init__.py
--rw-r--r--   0        0        0     2665 2023-02-02 09:05:36.529871 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/base.py
--rw-r--r--   0        0        0      979 2022-11-30 12:59:40.943922 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/hic.py
--rw-r--r--   0        0        0     3180 2023-03-30 13:57:37.832337 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/identities.py
--rw-r--r--   0        0        0     2450 2022-11-20 11:34:39.386109 datagen_tech-1.9.0rc1/src/datagen/components/datapoint/repo.py
--rw-r--r--   0        0        0     2836 2022-11-20 11:34:39.386165 datagen_tech-1.9.0rc1/src/datagen/components/dataset.py
--rw-r--r--   0        0        0     1358 2022-11-20 11:34:39.386219 datagen_tech-1.9.0rc1/src/datagen/components/datasource.py
--rw-r--r--   0        0        0     1547 2022-11-20 11:34:39.386272 datagen_tech-1.9.0rc1/src/datagen/components/scene.py
--rw-r--r--   0        0        0     2405 2022-11-20 11:34:39.386331 datagen_tech-1.9.0rc1/src/datagen/components/sequence.py
--rw-r--r--   0        0        0       30 2023-03-09 09:15:03.204463 datagen_tech-1.9.0rc1/src/datagen/config/__init__.py
--rw-r--r--   0        0        0      204 2023-03-09 09:15:12.307408 datagen_tech-1.9.0rc1/src/datagen/config/config.py
--rw-r--r--   0        0        0      150 2023-03-16 11:32:41.012592 datagen_tech-1.9.0rc1/src/datagen/config/settings.toml
--rw-r--r--   0        0        0      190 2022-11-20 11:34:39.386524 datagen_tech-1.9.0rc1/src/datagen/containers.py
--rw-r--r--   0        0        0        0 2023-03-09 09:15:02.797705 datagen_tech-1.9.0rc1/src/datagen/core/__init__.py
--rw-r--r--   0        0        0      445 2023-03-09 09:15:02.797973 datagen_tech-1.9.0rc1/src/datagen/core/tasks/__init__.py
--rw-r--r--   0        0        0     3399 2023-03-09 09:15:02.798102 datagen_tech-1.9.0rc1/src/datagen/core/tasks/containers.py
--rw-r--r--   0        0        0     4786 2023-03-09 09:15:02.798234 datagen_tech-1.9.0rc1/src/datagen/core/tasks/task.py
--rw-r--r--   0        0        0    14742 2023-03-09 09:15:02.798403 datagen_tech-1.9.0rc1/src/datagen/core/tasks/task_definitions.py
--rw-r--r--   0        0        0      671 2023-03-09 09:15:02.798517 datagen_tech-1.9.0rc1/src/datagen/core/tasks/task_runner.py
--rw-r--r--   0        0        0      216 2023-01-23 13:07:38.625381 datagen_tech-1.9.0rc1/src/datagen/dev/__init__.py
--rw-r--r--   0        0        0      404 2022-12-25 10:08:42.190793 datagen_tech-1.9.0rc1/src/datagen/dev/__version__.py
--rw-r--r--   0        0        0      491 2023-03-09 09:15:02.798890 datagen_tech-1.9.0rc1/src/datagen/dev/logging.py
--rw-r--r--   0        0        0     3352 2023-03-09 09:15:02.799297 datagen_tech-1.9.0rc1/src/datagen/dev/modules.py
--rw-r--r--   0        0        0     1097 2022-12-25 10:08:42.191110 datagen_tech-1.9.0rc1/src/datagen/dev/mutually_exclusive.py
--rw-r--r--   0        0        0     3162 2022-12-04 11:43:43.173438 datagen_tech-1.9.0rc1/src/datagen/dev/plugins.py
--rw-r--r--   0        0        0        0 2022-11-20 11:34:39.386675 datagen_tech-1.9.0rc1/src/datagen/imaging/__init__.py
--rw-r--r--   0        0        0      916 2022-11-20 11:34:39.386731 datagen_tech-1.9.0rc1/src/datagen/imaging/base.py
--rw-r--r--   0        0        0     1133 2022-11-22 17:05:53.880424 datagen_tech-1.9.0rc1/src/datagen/imaging/opencv.py
--rw-r--r--   0        0        0      481 2023-01-23 13:07:38.625964 datagen_tech-1.9.0rc1/src/datagen/impl.py
--rw-r--r--   0        0        0      262 2022-11-20 11:34:39.386911 datagen_tech-1.9.0rc1/src/datagen/modalities/__init__.py
--rw-r--r--   0        0        0     1779 2022-11-20 11:34:39.386963 datagen_tech-1.9.0rc1/src/datagen/modalities/containers.py
--rw-r--r--   0        0        0     2632 2022-11-20 11:34:39.387018 datagen_tech-1.9.0rc1/src/datagen/modalities/descriptors.py
--rw-r--r--   0        0        0      247 2023-01-22 08:41:48.717341 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717367 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/__init__.py
--rw-r--r--   0        0        0      988 2023-01-22 08:41:48.717433 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/camera_metadata.py
--rw-r--r--   0        0        0     2907 2023-01-23 15:48:43.361446 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/containers.py
--rw-r--r--   0        0        0     1670 2023-01-22 08:41:48.717558 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/environments.py
--rw-r--r--   0        0        0      875 2023-01-22 08:41:48.718648 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/lights_metadata.py
--rw-r--r--   0        0        0     2292 2023-01-22 08:41:48.717631 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/segmentation.py
--rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717659 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/common/__init__.py
--rw-r--r--   0        0        0      133 2023-01-22 08:41:48.717718 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/common/identity_label.py
--rw-r--r--   0        0        0     1296 2023-01-22 08:41:48.717776 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/common/ndarray.py
--rw-r--r--   0        0        0      200 2023-01-22 08:41:48.717835 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/common/sixdof.py
--rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717861 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/__init__.py
--rw-r--r--   0        0        0     1309 2023-01-22 08:41:48.717930 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/actor_metadata.py
--rw-r--r--   0        0        0     1225 2023-01-22 08:41:48.717988 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/center_of_geometry.py
--rw-r--r--   0        0        0     1326 2023-01-22 08:41:48.718042 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/containers.py
--rw-r--r--   0        0        0     3431 2023-01-22 08:41:48.718105 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/keypoints.py
--rw-r--r--   0        0        0        1 2023-01-22 08:41:48.718160 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/__init__.py
--rw-r--r--   0        0        0     6156 2023-01-22 08:41:48.718235 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/actor_metadata.py
--rw-r--r--   0        0        0     1807 2023-01-23 15:48:43.355968 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/containers.py
--rw-r--r--   0        0        0      147 2023-01-22 08:41:48.718352 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/face_bounding_box.py
--rw-r--r--   0        0        0        0 2023-01-22 08:41:48.718380 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/__init__.py
--rw-r--r--   0        0        0     1695 2023-01-22 08:41:48.718447 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/base.py
--rw-r--r--   0        0        0      739 2023-01-22 08:41:48.718514 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/v1.py
--rw-r--r--   0        0        0     2237 2023-03-09 09:15:11.104208 datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/v2.py
--rw-r--r--   0        0        0       59 2022-12-25 10:08:42.191244 datagen_tech-1.9.0rc1/src/datagen/utilities/__init__.py
--rw-r--r--   0        0        0      585 2023-01-23 13:45:14.234516 datagen_tech-1.9.0rc1/src/datagen/utilities/arrays.py
--rw-r--r--   0        0        0     7532 2023-03-30 14:19:15.418012 datagen_tech-1.9.0rc1/src/datagen/utilities/camera.py
--rw-r--r--   0        0        0     2461 2022-12-25 10:08:42.191656 datagen_tech-1.9.0rc1/src/datagen/utilities/extrinsics.py
--rw-r--r--   0        0        0    11911 1970-01-01 00:00:00.000000 datagen_tech-1.9.0rc1/setup.py
--rw-r--r--   0        0        0     8818 1970-01-01 00:00:00.000000 datagen_tech-1.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2022-12-28 14:41:11.697060 datagen_tech-1.9.0rc2/LICENSE
+-rw-r--r--   0        0        0     7175 2022-12-28 14:41:11.697199 datagen_tech-1.9.0rc2/README.md
+-rw-r--r--   0        0        0     1982 2023-04-02 08:05:54.339372 datagen_tech-1.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      244 2022-12-25 10:08:42.081571 datagen_tech-1.9.0rc2/src/datagen/__init__.py
+-rw-r--r--   0        0        0      447 2023-01-24 14:24:26.735850 datagen_tech-1.9.0rc2/src/datagen/api/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-26 09:01:52.298232 datagen_tech-1.9.0rc2/src/datagen/api/assets.py
+-rw-r--r--   0        0        0      230 2022-12-25 10:08:42.084256 datagen_tech-1.9.0rc2/src/datagen/api/catalog/__init__.py
+-rw-r--r--   0        0        0      355 2023-03-13 15:06:42.405987 datagen_tech-1.9.0rc2/src/datagen/api/catalog/attributes.py
+-rw-r--r--   0        0        0    40406 2023-03-19 16:53:42.795114 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/backgrounds.json
+-rw-r--r--   0        0        0     3482 2023-02-06 16:46:30.755604 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/beards.json
+-rw-r--r--   0        0        0   600982 2023-02-07 09:24:05.035297 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/eyebrows.json
+-rw-r--r--   0        0        0    46067 2023-02-12 06:59:13.716940 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/eyes.json
+-rw-r--r--   0        0        0     1358 2023-02-06 16:46:30.757951 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/glasses.json
+-rw-r--r--   0        0        0    68866 2023-02-20 14:55:17.995340 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hair.json
+-rw-r--r--   0        0        0   406568 2023-03-30 14:33:54.272534 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hic/attributes.json
+-rw-r--r--   0        0        0  3147694 2023-03-30 14:33:54.277071 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hic/presets.json
+-rw-r--r--   0        0        0  6032881 2023-02-06 16:46:25.148161 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/humans/attributes.json
+-rw-r--r--   0        0        0 29256791 2023-01-22 11:34:49.658350 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/humans/defaults.json
+-rw-r--r--   0        0        0      174 2023-03-16 11:32:41.011645 datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/masks.json
+-rw-r--r--   0        0        0     2680 2023-02-02 09:05:36.527979 datagen_tech-1.9.0rc2/src/datagen/api/catalog/containers.py
+-rw-r--r--   0        0        0      121 2023-02-02 09:05:36.528188 datagen_tech-1.9.0rc2/src/datagen/api/catalog/hooks/__init__.py
+-rw-r--r--   0        0        0      434 2023-03-28 07:24:32.391005 datagen_tech-1.9.0rc2/src/datagen/api/catalog/hooks/hic.py
+-rw-r--r--   0        0        0      758 2023-02-02 09:05:36.528562 datagen_tech-1.9.0rc2/src/datagen/api/catalog/hooks/humans.py
+-rw-r--r--   0        0        0     9891 2023-03-09 09:15:02.795423 datagen_tech-1.9.0rc2/src/datagen/api/catalog/impl.py
+-rw-r--r--   0        0        0        0 2023-01-23 13:07:38.623174 datagen_tech-1.9.0rc2/src/datagen/api/client/__init__.py
+-rw-r--r--   0        0        0     1126 2023-03-09 09:15:02.795628 datagen_tech-1.9.0rc2/src/datagen/api/client/containers.py
+-rw-r--r--   0        0        0     1750 2023-03-09 09:15:02.795946 datagen_tech-1.9.0rc2/src/datagen/api/client/exceptions.py
+-rw-r--r--   0        0        0     3324 2023-03-16 11:32:41.012269 datagen_tech-1.9.0rc2/src/datagen/api/client/schemas.py
+-rw-r--r--   0        0        0      891 2023-03-09 09:15:02.796547 datagen_tech-1.9.0rc2/src/datagen/api/client/session.py
+-rw-r--r--   0        0        0      267 2023-03-09 09:15:02.796846 datagen_tech-1.9.0rc2/src/datagen/api/containers.py
+-rw-r--r--   0        0        0      276 2023-01-23 13:07:38.624232 datagen_tech-1.9.0rc2/src/datagen/api/datapoint/__init__.py
+-rw-r--r--   0        0        0     4614 2023-04-02 07:24:45.378744 datagen_tech-1.9.0rc2/src/datagen/api/impl.py
+-rw-r--r--   0        0        0        0 2022-11-30 13:20:55.785436 datagen_tech-1.9.0rc2/src/datagen/api/requests/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-30 13:20:55.785474 datagen_tech-1.9.0rc2/src/datagen/api/requests/datapoint/__init__.py
+-rw-r--r--   0        0        0     1377 2023-03-09 09:15:02.797323 datagen_tech-1.9.0rc2/src/datagen/api/requests/datapoint/builder.py
+-rw-r--r--   0        0        0      579 2023-03-09 09:15:12.309229 datagen_tech-1.9.0rc2/src/datagen/api/requests/director.py
+-rw-r--r--   0        0        0      248 2022-11-20 11:34:39.385633 datagen_tech-1.9.0rc2/src/datagen/components/__init__.py
+-rw-r--r--   0        0        0     1348 2022-11-20 11:34:39.385695 datagen_tech-1.9.0rc2/src/datagen/components/camera.py
+-rw-r--r--   0        0        0      231 2022-11-20 11:34:39.385769 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/__init__.py
+-rw-r--r--   0        0        0      815 2022-11-30 13:20:55.785678 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/container.py
+-rw-r--r--   0        0        0        0 2022-11-20 11:34:39.385875 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/__init__.py
+-rw-r--r--   0        0        0     2665 2023-02-02 09:05:36.529871 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/base.py
+-rw-r--r--   0        0        0      979 2022-11-30 12:59:40.943922 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/hic.py
+-rw-r--r--   0        0        0     3180 2023-03-30 13:57:37.832337 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/identities.py
+-rw-r--r--   0        0        0     2450 2022-11-20 11:34:39.386109 datagen_tech-1.9.0rc2/src/datagen/components/datapoint/repo.py
+-rw-r--r--   0        0        0     2836 2022-11-20 11:34:39.386165 datagen_tech-1.9.0rc2/src/datagen/components/dataset.py
+-rw-r--r--   0        0        0     1358 2022-11-20 11:34:39.386219 datagen_tech-1.9.0rc2/src/datagen/components/datasource.py
+-rw-r--r--   0        0        0     1547 2022-11-20 11:34:39.386272 datagen_tech-1.9.0rc2/src/datagen/components/scene.py
+-rw-r--r--   0        0        0     2405 2022-11-20 11:34:39.386331 datagen_tech-1.9.0rc2/src/datagen/components/sequence.py
+-rw-r--r--   0        0        0       30 2023-03-09 09:15:03.204463 datagen_tech-1.9.0rc2/src/datagen/config/__init__.py
+-rw-r--r--   0        0        0      204 2023-03-09 09:15:12.307408 datagen_tech-1.9.0rc2/src/datagen/config/config.py
+-rw-r--r--   0        0        0      150 2023-03-16 11:32:41.012592 datagen_tech-1.9.0rc2/src/datagen/config/settings.toml
+-rw-r--r--   0        0        0      190 2022-11-20 11:34:39.386524 datagen_tech-1.9.0rc2/src/datagen/containers.py
+-rw-r--r--   0        0        0        0 2023-03-09 09:15:02.797705 datagen_tech-1.9.0rc2/src/datagen/core/__init__.py
+-rw-r--r--   0        0        0      445 2023-03-09 09:15:02.797973 datagen_tech-1.9.0rc2/src/datagen/core/tasks/__init__.py
+-rw-r--r--   0        0        0     3399 2023-03-09 09:15:02.798102 datagen_tech-1.9.0rc2/src/datagen/core/tasks/containers.py
+-rw-r--r--   0        0        0     4786 2023-03-09 09:15:02.798234 datagen_tech-1.9.0rc2/src/datagen/core/tasks/task.py
+-rw-r--r--   0        0        0    14742 2023-03-09 09:15:02.798403 datagen_tech-1.9.0rc2/src/datagen/core/tasks/task_definitions.py
+-rw-r--r--   0        0        0      671 2023-03-09 09:15:02.798517 datagen_tech-1.9.0rc2/src/datagen/core/tasks/task_runner.py
+-rw-r--r--   0        0        0      216 2023-01-23 13:07:38.625381 datagen_tech-1.9.0rc2/src/datagen/dev/__init__.py
+-rw-r--r--   0        0        0      404 2022-12-25 10:08:42.190793 datagen_tech-1.9.0rc2/src/datagen/dev/__version__.py
+-rw-r--r--   0        0        0      491 2023-03-09 09:15:02.798890 datagen_tech-1.9.0rc2/src/datagen/dev/logging.py
+-rw-r--r--   0        0        0     3352 2023-03-09 09:15:02.799297 datagen_tech-1.9.0rc2/src/datagen/dev/modules.py
+-rw-r--r--   0        0        0     1097 2022-12-25 10:08:42.191110 datagen_tech-1.9.0rc2/src/datagen/dev/mutually_exclusive.py
+-rw-r--r--   0        0        0     3162 2022-12-04 11:43:43.173438 datagen_tech-1.9.0rc2/src/datagen/dev/plugins.py
+-rw-r--r--   0        0        0        0 2022-11-20 11:34:39.386675 datagen_tech-1.9.0rc2/src/datagen/imaging/__init__.py
+-rw-r--r--   0        0        0      916 2022-11-20 11:34:39.386731 datagen_tech-1.9.0rc2/src/datagen/imaging/base.py
+-rw-r--r--   0        0        0     1133 2022-11-22 17:05:53.880424 datagen_tech-1.9.0rc2/src/datagen/imaging/opencv.py
+-rw-r--r--   0        0        0      481 2023-01-23 13:07:38.625964 datagen_tech-1.9.0rc2/src/datagen/impl.py
+-rw-r--r--   0        0        0      262 2022-11-20 11:34:39.386911 datagen_tech-1.9.0rc2/src/datagen/modalities/__init__.py
+-rw-r--r--   0        0        0     1779 2022-11-20 11:34:39.386963 datagen_tech-1.9.0rc2/src/datagen/modalities/containers.py
+-rw-r--r--   0        0        0     2632 2022-11-20 11:34:39.387018 datagen_tech-1.9.0rc2/src/datagen/modalities/descriptors.py
+-rw-r--r--   0        0        0      247 2023-01-22 08:41:48.717341 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717367 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/__init__.py
+-rw-r--r--   0        0        0      988 2023-01-22 08:41:48.717433 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/camera_metadata.py
+-rw-r--r--   0        0        0     2907 2023-01-23 15:48:43.361446 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/containers.py
+-rw-r--r--   0        0        0     1670 2023-01-22 08:41:48.717558 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/environments.py
+-rw-r--r--   0        0        0      875 2023-01-22 08:41:48.718648 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/lights_metadata.py
+-rw-r--r--   0        0        0     2292 2023-01-22 08:41:48.717631 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/segmentation.py
+-rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717659 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/common/__init__.py
+-rw-r--r--   0        0        0      133 2023-01-22 08:41:48.717718 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/common/identity_label.py
+-rw-r--r--   0        0        0     1296 2023-01-22 08:41:48.717776 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/common/ndarray.py
+-rw-r--r--   0        0        0      200 2023-01-22 08:41:48.717835 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/common/sixdof.py
+-rw-r--r--   0        0        0        0 2023-01-22 08:41:48.717861 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/__init__.py
+-rw-r--r--   0        0        0     1309 2023-01-22 08:41:48.717930 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/actor_metadata.py
+-rw-r--r--   0        0        0     1225 2023-01-22 08:41:48.717988 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/center_of_geometry.py
+-rw-r--r--   0        0        0     1326 2023-01-22 08:41:48.718042 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/containers.py
+-rw-r--r--   0        0        0     3431 2023-01-22 08:41:48.718105 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/keypoints.py
+-rw-r--r--   0        0        0        1 2023-01-22 08:41:48.718160 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/__init__.py
+-rw-r--r--   0        0        0     6156 2023-01-22 08:41:48.718235 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/actor_metadata.py
+-rw-r--r--   0        0        0     1807 2023-01-23 15:48:43.355968 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/containers.py
+-rw-r--r--   0        0        0      147 2023-01-22 08:41:48.718352 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/face_bounding_box.py
+-rw-r--r--   0        0        0        0 2023-01-22 08:41:48.718380 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/__init__.py
+-rw-r--r--   0        0        0     1695 2023-01-22 08:41:48.718447 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/base.py
+-rw-r--r--   0        0        0      739 2023-01-22 08:41:48.718514 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/v1.py
+-rw-r--r--   0        0        0     2237 2023-03-09 09:15:11.104208 datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/v2.py
+-rw-r--r--   0        0        0       59 2022-12-25 10:08:42.191244 datagen_tech-1.9.0rc2/src/datagen/utilities/__init__.py
+-rw-r--r--   0        0        0      585 2023-01-23 13:45:14.234516 datagen_tech-1.9.0rc2/src/datagen/utilities/arrays.py
+-rw-r--r--   0        0        0     7568 2023-04-02 07:24:45.379235 datagen_tech-1.9.0rc2/src/datagen/utilities/camera.py
+-rw-r--r--   0        0        0     2461 2022-12-25 10:08:42.191656 datagen_tech-1.9.0rc2/src/datagen/utilities/extrinsics.py
+-rw-r--r--   0        0        0    11906 1970-01-01 00:00:00.000000 datagen_tech-1.9.0rc2/setup.py
+-rw-r--r--   0        0        0     8813 1970-01-01 00:00:00.000000 datagen_tech-1.9.0rc2/PKG-INFO
```

### Comparing `datagen_tech-1.9.0rc1/LICENSE` & `datagen_tech-1.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/README.md` & `datagen_tech-1.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/pyproject.toml` & `datagen_tech-1.9.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagen-tech"
-version = "1.9.0.rc1"
+version = "1.9.0.rc2"
 description = "Datagen SDK"
 readme = "README.md"
 authors = ["Datagen Technologies Ltd."]
 packages = [{ include = "datagen", from ="src"}]
 repository = "https://gitlab.com/datagen1/core/sdk"
 
 [tool.poetry.dependencies]
@@ -26,15 +26,15 @@
 pandas = "^1.1"
 scipy = [
     { "version" = "^1.5", python = "<3.9",  optional = true },
     { "version" = "^1.9", python = "^3.9",  optional = true }
 ]
 requests = "^2.28.1"
 appdirs = "^1.4"
-datagen-protocol-functional = "0.21.1rc232"
+datagen-protocol-functional = "0.21.1"
 aiohttp = "^3.8"
 aiofiles = "^23.1.0"
 asyncio-channel = "^0.9.1"
 nest-asyncio = "^1.5.6"
 
 [tool.poetry.dev-dependencies]
 #datagen-protocol-functional = {path = "../datagen-protocol/projects/functional", develop=true}
```

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/backgrounds.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/backgrounds.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/beards.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/beards.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/eyebrows.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/eyebrows.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/eyes.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/eyes.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/glasses.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/glasses.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hair.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hair.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hic/attributes.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hic/attributes.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/hic/presets.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/hic/presets.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/humans/attributes.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/humans/attributes.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/cache/humans/defaults.json` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/cache/humans/defaults.json`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/hooks/humans.py` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/hooks/humans.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/catalog/impl.py` & `datagen_tech-1.9.0rc2/src/datagen/api/catalog/impl.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/client/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/api/client/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/client/exceptions.py` & `datagen_tech-1.9.0rc2/src/datagen/api/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/client/schemas.py` & `datagen_tech-1.9.0rc2/src/datagen/api/client/schemas.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/client/session.py` & `datagen_tech-1.9.0rc2/src/datagen/api/client/session.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/impl.py` & `datagen_tech-1.9.0rc2/src/datagen/api/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import json
 from pathlib import Path
 from typing import List, Optional, Union
 
-from datagen.api.assets import Background, Camera, DataRequest, Glasses, Human, HumanDatapoint, Light, Mask
+from datagen.api.assets import (
+    Background,
+    Camera,
+    GenerationRequest,
+    DataRequest,
+    SequenceRequest,
+    Glasses,
+    Human,
+    HumanDatapoint,
+    Light,
+    Mask,
+)
 from datagen.api.client.schemas import DataResponse, DataResponseStatus, DownloadRequest, DownloadURL
 from datagen.api.requests.datapoint.builder import HumanDatapointBuilder
 from datagen.api.requests.director import DataRequestDirector
 from datagen.config import settings
 from datagen.core.tasks import TaskContainer
 from datagen.core.tasks.task_runner import TaskRunner
 from datagen.dev.logging import get_logger
@@ -29,26 +40,26 @@
         mask: Optional[Mask] = None,
         background: Optional[Background] = None,
         lights: Optional[List[Light]] = None,
     ) -> HumanDatapoint:
         self._request_director.builder = HumanDatapointBuilder(human, camera, glasses, mask, background, lights)
         return self._request_director.build_datapoint()
 
-    def load(self, path: Union[Path, str]) -> DataRequest:
-        if not isinstance(path, Path):
+    def load(self, path: Union[Path, str]) -> GenerationRequest:
+        if isinstance(path, str):
             path = self._get_request_json_path(path)
-        path = self._get_request_json_path(path)
-        return DataRequest.parse_file(path)
+        request_dict = json.loads(path.read_text())
+        return DataRequest(**request_dict) if "datapoints" in request_dict else SequenceRequest(**request_dict)
 
     def generate(
         self,
-        request: DataRequest,
+        request: GenerationRequest,
         generation_name: str,
     ) -> DataResponse:
-        batches = DatagenAPI.batch_request(request=request)
+        batches = DatagenAPI.batch_request(request)
         return TaskRunner().run(
             task=self._task_container.pipeline_factory.data_generation(number_of_batches=len(batches)),
             data=(batches, generation_name),
         )
 
     def stop(self, generation_id) -> None:
         TaskRunner().run(
@@ -74,31 +85,38 @@
         TaskRunner().run(
             task=self._task_container.pipeline_factory.download(
                 number_of_files=len(urls), remove_tar_files=remove_tar_files
             ),
             data=DownloadRequest(urls=urls, path=dest_folder, dataset_name=dataset_name).batch(),
         )
 
-    def dump(self, request: DataRequest, path: Union[Path, str] = None) -> None:
+    def dump(self, request: GenerationRequest, path: Union[Path, str] = None) -> None:
         if not isinstance(path, Path):
             path = self._get_request_json_path(path)
         path.write_text(json.dumps(request.dict(), indent=3, sort_keys=True))
-        logger.info(
-            f"Request was successfully dumped to path '{path.absolute()}' ({len(request)} datapoints total).",
-        )
+        if isinstance(request, DataRequest):
+            logger.info(
+                f"Request was successfully dumped to path '{path.absolute()}' ({len(request)} datapoints total).",
+            )
+        else:
+            logger.info(
+                f"Request was successfully dumped to path '{path.absolute()}'.",
+            )
 
     def _get_request_json_path(self, path: Optional[str]) -> Path:
         path_ = Path(path) if path else Path.cwd().joinpath(DEFAULT_DATAPOINT_REQUESTS_JSON_NAME)
         if not path_.parent.exists():
             raise FileNotFoundError(f"{path_.parent} folder does not exist, cannot dump requests")
         path_.touch()
         return path_
 
     @staticmethod
-    def batch_request(request: DataRequest) -> List[DataRequest]:
-        batch_size = settings["batch_size"]
+    def batch_request(request: GenerationRequest) -> List[GenerationRequest]:
         batches = []
-        num_of_datapoints = len(request.datapoints)
-        for dp_idx in range(0, num_of_datapoints, batch_size):
-            batches.append(DataRequest(datapoints=request.datapoints[dp_idx : dp_idx + batch_size]))
-
+        if isinstance(request, DataRequest):
+            batch_size = settings["batch_size"]
+            datapoints_num = len(request.datapoints)
+            for dp_idx in range(0, datapoints_num, batch_size):
+                batches.append(DataRequest(datapoints=request.datapoints[dp_idx : dp_idx + batch_size]))
+        elif isinstance(request, SequenceRequest):
+            batches = [request]
         return batches
```

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/requests/datapoint/builder.py` & `datagen_tech-1.9.0rc2/src/datagen/api/requests/datapoint/builder.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/api/requests/director.py` & `datagen_tech-1.9.0rc2/src/datagen/api/requests/director.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/camera.py` & `datagen_tech-1.9.0rc2/src/datagen/components/camera.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datapoint/container.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datapoint/container.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/base.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/base.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/hic.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/hic.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datapoint/entity/identities.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datapoint/entity/identities.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datapoint/repo.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datapoint/repo.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/dataset.py` & `datagen_tech-1.9.0rc2/src/datagen/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/datasource.py` & `datagen_tech-1.9.0rc2/src/datagen/components/datasource.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/scene.py` & `datagen_tech-1.9.0rc2/src/datagen/components/scene.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/components/sequence.py` & `datagen_tech-1.9.0rc2/src/datagen/components/sequence.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/core/tasks/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/core/tasks/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/core/tasks/task.py` & `datagen_tech-1.9.0rc2/src/datagen/core/tasks/task.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/core/tasks/task_definitions.py` & `datagen_tech-1.9.0rc2/src/datagen/core/tasks/task_definitions.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/core/tasks/task_runner.py` & `datagen_tech-1.9.0rc2/src/datagen/core/tasks/task_runner.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/dev/modules.py` & `datagen_tech-1.9.0rc2/src/datagen/dev/modules.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/dev/mutually_exclusive.py` & `datagen_tech-1.9.0rc2/src/datagen/dev/mutually_exclusive.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/dev/plugins.py` & `datagen_tech-1.9.0rc2/src/datagen/dev/plugins.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/imaging/base.py` & `datagen_tech-1.9.0rc2/src/datagen/imaging/base.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/imaging/opencv.py` & `datagen_tech-1.9.0rc2/src/datagen/imaging/opencv.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/descriptors.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/descriptors.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/camera_metadata.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/camera_metadata.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/environments.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/environments.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/lights_metadata.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/lights_metadata.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/base/segmentation.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/base/segmentation.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/common/ndarray.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/common/ndarray.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/actor_metadata.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/actor_metadata.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/center_of_geometry.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/center_of_geometry.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/hic/keypoints.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/hic/keypoints.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/actor_metadata.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/actor_metadata.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/containers.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/containers.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/base.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/base.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/v1.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/v1.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/modalities/textual/identities/keypoints/v2.py` & `datagen_tech-1.9.0rc2/src/datagen/modalities/textual/identities/keypoints/v2.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/utilities/arrays.py` & `datagen_tech-1.9.0rc2/src/datagen/utilities/arrays.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/src/datagen/utilities/camera.py` & `datagen_tech-1.9.0rc2/src/datagen/utilities/camera.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,18 +107,18 @@
         Examples:
             >>> camera = assets.Camera()
             >>> camera.extrinsics.location = assets.Point(x=-0.056, y=-1.985, z=-0.367)
             >>> camera_utils.rotate(camera, look_at_point=assets.Point(x=0., y=0., z=0.1)))
             >>> camera.extrinsics.location
             Point(x=1.641, y=13.246,  z=0.)
         """
-        camera.extrinsics.rotation = self.calculate_rotation(camera, look_at_point=look_at_point)
+        camera.extrinsic_params.rotation = self.calculate_rotation(camera, look_at_point=look_at_point)
 
     def _get_camera_location(self, camera: Union[assets.Camera, P]) -> P:
-        return camera if isinstance(camera, (assets.Point, np.ndarray)) else camera.extrinsics.location
+        return camera if isinstance(camera, (assets.Point, np.ndarray)) else camera.extrinsic_params.location
 
     def get_extrinsic_matrix(self, camera: assets.Camera) -> "np.ndarray":
         """Calculates the extrinsic matrix of the camera.
 
         Args:
             camera (assets.Camera): The camera to get extrinsic matrix for.
 
@@ -137,15 +137,15 @@
         Returns:
             np.ndarray: The rotation matrix of the camera
         """
         extrinsics = self._get_extrinsics_from_camera_asset(camera)
         return extrinsics.rotation.matrix
 
     def _get_extrinsics_from_camera_asset(self, camera: assets.Camera) -> Extrinsics:
-        camera_location, yaw_pitch_roll = to_arrays(camera.extrinsics.location, camera.extrinsics.rotation)
+        camera_location, yaw_pitch_roll = to_arrays(camera.extrinsic_params.location, camera.extrinsic_params.rotation)
         extrinsics = Extrinsics.from_yaw_pitch_roll(camera_location, yaw_pitch_roll)
         return extrinsics
 
     def create_cameras_ring(
         self,
         cameras_num: int,
         cameras_intrinsics: assets.CameraIntrinsicParams,
@@ -183,14 +183,14 @@
         camera_location: assets.Point = None,
     ) -> assets.Camera:
         camera = assets.Camera()
         camera.name = f"Camera_{str(camera_idx).zfill(2)}" if camera_idx else config.assets.camera.name
         if camera_intrinsics:
             camera.intrinsics = camera_intrinsics
         if camera_extrinsics:
-            camera.extrinsics = camera_extrinsics
+            camera.extrinsic_params = camera_extrinsics
         if camera_location:
-            camera.extrinsics.location = camera_location
+            camera.extrinsic_params.location = camera_location
         return camera
 
 
 sys.modules[__name__] = FunctionalModule(functionality=CameraUtils())
```

### Comparing `datagen_tech-1.9.0rc1/src/datagen/utilities/extrinsics.py` & `datagen_tech-1.9.0rc2/src/datagen/utilities/extrinsics.py`

 * *Files identical despite different names*

### Comparing `datagen_tech-1.9.0rc1/setup.py` & `datagen_tech-1.9.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                          'cache/masks.json']}
 
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8,<4.0',
  'appdirs>=1.4,<2.0',
  'asyncio-channel>=0.9.1,<0.10.0',
- 'datagen-protocol-functional==0.21.1rc232',
+ 'datagen-protocol-functional==0.21.1',
  'dependency-injector>4.6',
  'dynaconf>=2.2.3,<3.0.0',
  'importlib-metadata<5.0.0',
  'marshmallow-dataclass>=6',
  'marshmallow-enum>=1.5',
  'nest-asyncio>=1.5.6,<2.0.0',
  'opencv-python>=4.4,<5.0',
@@ -109,15 +109,15 @@
  ':python_version >= "3.9"': ['numpy>=1.20,<2.0'],
  'camera-utils:python_version < "3.9"': ['scipy>=1.5,<2.0', 'scipy>=1.5,<2.0'],
  'camera-utils:python_version >= "3.9" and python_version < "4.0"': ['scipy>=1.9,<2.0',
                                                                      'scipy>=1.9,<2.0']}
 
 setup_kwargs = {
     'name': 'datagen-tech',
-    'version': '1.9.0rc1',
+    'version': '1.9.0rc2',
     'description': 'Datagen SDK',
     'long_description': '# The Datagen SDK Python Package\n\n## About Datagen\n\nDatagen is powering the AI revolution by providing high-performance synthetic data, with a focus on data for human-centric computer vision applications. \n\nDatagen provides a powerful platform that allows you to generate high-quality and high variance, domain-specific, simulated synthetic data, granting you the ability to simulate dynamic humans and objects in their context. With Datagen, CV engineers have unparalleled flexibility to control visual outcomes across a broad spectrum of 3D environments.\n\n## About this package\n\nDatagen has developed a set of Python-based user tools for accessing and loading the rendered images and metadata that you generate on our platform. This package is designed to load our synthetic data into your Python environment, whether as part of your training set or as part of your testing set. \n\nThe abstraction layer we designed gives you access to all of the modalities we offer: facial landmarks, eye gaze vectors, depth and normal maps, and more. \n\n## Installation\n\nBefore installing this package, we recommend that you create a new Conda environment using the following command:\n\n> conda create --name datagen-env\n\nNext, activate the environment using this command:\n\n> conda activate datagen-env\n\nFinally, use this command to install the Datagen package itself:\n\n> pip install datagen-tech\n\n# Using This Package\n\nThis package contains Python objects and functions that are designed to process datasets generated with the Datagen Platform. If you are a Datagen customer, you have already been given access to sample datasets and jupyter notebook tutorials. If you are not a Datagen customer, contact our support team at support@datagen.tech.\n\n## Importing the SDK\n\nTo import the sdk, use the command `import datagen` or, if you prefer, `import datagen as dg`. For the rest of this tutorial we will use the latter.\n\n## Datasets\n\nA "dataset" is any collection of datapoints that were generated on the Datgen platform. Each datapoint is a single visual spectrum image accompanied by visual and textual metadata.\n\n### Loading a dataset\n\nThe `dg.load()` command stores one or more datasets into a `Dataset` object. It can accept any number of target folders at once, merging them into one large dataset so you can conduct operations on all of them together. \n\nThis command is fully backwards-compatible. If you use the platform\'s newest features in your dataset, you can still load that dataset together with older datasets that predate those features.\n\nWhen using this command, you should target the top-level folder of each dataset (the folder that contains one or more subfolders named "scene").  For example:\n\n```\ndataset = dg.load("/path/to/datagen/datasets/eye-gaze-forward", "/path/to/datagen/datasets/expression-smiles")\n```\n\nThe above line of sample code loads a dataset found in a folder named "eye-gaze-forward" as well as a dataset found in a folder named "expression-smiles", merging their datapoints into a single dataset.\n\n### Working with your dataset\n\nYou can iterate over your dataset in three different ways: by scene, by camera, or by datapoint.\n\n### Scenes\n\n#### What is a scene?\n\nA "scene" refers to a 3D environment that contains one or more 3D objects. For example, each scene that is created in our Faces generator consists of a single human face, wearing a specific expression, and located in a static position.\n\nWhen generating a dataset on our Faces platform, you have the option of rendering each scene in multiple ways: through more than one camera, each with different settings; and under more than one lighting scenario, each with different backgrounds. Therefore, depending on the settings you used when you generated this dataset, each scene can be depicted in anywhere between one and over 30 rendered images.\n\n#### The `Scene` object\n\nEach dataset contains an iterable set of `Scene` objects. To retrieve this set, use `dataset.scenes`. To refer to an individual scene in a dataset, use `dataset.scenes[0]`.\n\nThe `Scene` object contains a set of rendered images that all depict the same subject, but from different angles and under different lighting scenarios. Each of these images, along with its metadata, is called a "datapoint". You can access a scene\'s datapoints by subscription:\n\n```\nscene = dataset.scenes[0]\ndatapoint = scene[0]\n```\n\nOr by iterating over the scene:\n\n```\nfor datapoint in scene:\n    ...\n```\n\n**Note:** In older datasets generated by our platform, scenes were previously named "environments". The package supports both formats.\n\n### Cameras\n\n#### What is a camera?\n\nA "camera" refers to a set of rendered images that were taken of a specific scene, from a specific angle, under specific camera settings - but each one shows the scene under a different lighting scenario. When you generated this dataset, you selected one or more lighting scenarios; that selection determines the number of rendered images per camera.\n\n#### The `Camera` object\n\nEach scene contains an iterable list of `Camera` objects. To retrieve this set, use scene`scene.cameras`. To refer to an individual camera in a scene, use `scene.cameras[0]`.\n\nThe `Camera` object contains a set of rendered images that all depict the same subject from the same angle, but under different lighting scenarios. Each of these images, along with its metadata, is called a "datapoint". You can access a camera\'s datapoints by subscription:\n\n```\nscene = dataset.scenes[0]\ncamera = scene.cameras[0]\ndatapoint = camera[0]\n```\n\nOr by iterating over the camera:\n\n```\nfor datapoint in camera:\n    ...\n```\n\n### Datapoints\n\n#### What is a datapoint?\n\nA "datapoint" refers to a single rendered image of a synthetic human subject, along with all of its metadata. That metadata includes all of Datagen\'s modalities: normal and depth maps, facial landmark coordinates, camera and actor metadata, and more.\n\n#### The `Datapoint` object\n\nA `Datapoint` object consists of a visual spectrum image annotated by additional visual and textual data files:\n\n* The visual spectrum image depicts the scene from the point of view of a specific camera under a specific lighting scenario.\n\n* The annotations contain metadata that is specific to that image.\n\nFor example, each `Datapoint` object contains 2D coordinates for facial landmarks, identifying where those landmark can be found in the visual spectrum image.\n\nYou can use tab autocompletion to view the full list of available objects in the `Datapoint` object. For example, you can use the following command to access the visual spectrum image of the subject:\n\n```\nimshow(datapoint.visible_spectrum)\n```\n\nAnd this one to access a normal map of the subject:\n\n```\nimshow(datapoint.normals_map)\n```\n\nTextual annotations are organized in a hierarchy. `datapoint.actor_metadata.face_expression` gives you the description of the subject\'s facial expression, while `datapoint.semantic_segmentation_metadata.nose` gives you the RGB value that represents the nose in the accompanying semantic segmentation map.\n',
     'author': 'Datagen Technologies Ltd.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/datagen1/core/sdk',
```

### Comparing `datagen_tech-1.9.0rc1/PKG-INFO` & `datagen_tech-1.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: datagen-tech
-Version: 1.9.0rc1
+Version: 1.9.0rc2
 Summary: Datagen SDK
 Home-page: https://gitlab.com/datagen1/core/sdk
 Author: Datagen Technologies Ltd.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: camera-utils
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: appdirs (>=1.4,<2.0)
 Requires-Dist: asyncio-channel (>=0.9.1,<0.10.0)
-Requires-Dist: datagen-protocol-functional (==0.21.1rc232)
+Requires-Dist: datagen-protocol-functional (==0.21.1)
 Requires-Dist: dependency-injector (>4.6)
 Requires-Dist: dynaconf (>=2.2.3,<3.0.0)
 Requires-Dist: importlib-metadata (<5.0.0)
 Requires-Dist: marshmallow-dataclass (>=6)
 Requires-Dist: marshmallow-enum (>=1.5)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: numpy (>=1.15,<2.0) ; python_full_version >= "3.6.7" and python_version < "3.7"
```

