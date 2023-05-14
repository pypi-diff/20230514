# Comparing `tmp/pyadlml-0.0.7.8a0.tar.gz` & `tmp/pyadlml-0.0.7.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadlml-0.0.7.8a0.tar", last modified: Sun Nov 13 22:18:03 2022, max compression
+gzip compressed data, was "pyadlml-0.0.7.9a0.tar", last modified: Mon Nov 14 13:29:39 2022, max compression
```

## Comparing `pyadlml-0.0.7.8a0.tar` & `pyadlml-0.0.7.9a0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2020-10-29 09:58:19.000000 pyadlml-0.0.7.8a0/MANIFEST.in
--rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     6164 2022-10-26 18:21:17.000000 pyadlml-0.0.7.8a0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml/
--rw-r--r--   0 chris     (1000) chris     (1000)      774 2022-10-26 19:47:31.000000 pyadlml-0.0.7.8a0/pyadlml/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2735 2021-08-16 09:39:57.000000 pyadlml-0.0.7.8a0/pyadlml/benchmark.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      743 2022-10-21 09:41:03.000000 pyadlml-0.0.7.8a0/pyadlml/constants.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml/dataset/
--rw-r--r--   0 chris     (1000) chris     (1000)      827 2022-10-26 19:48:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-01-16 14:29:28.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3723 2022-11-10 08:12:28.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/_dataset.py
--rw-r--r--   0 chris     (1000) chris     (1000)    17657 2022-11-13 10:03:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    29737 2022-11-10 08:15:15.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7431 2022-10-28 13:22:22.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_core/obj.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-19 16:38:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3511 2022-10-22 16:18:45.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/activity_assistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5714 2022-10-28 21:53:36.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/amsterdam.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7335 2022-11-11 12:45:06.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/aras.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6857 2022-03-26 11:45:38.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/casas_aruba.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4278 2022-10-18 20:14:29.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/homeassistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9878 2022-11-13 10:04:34.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/kasteren_2010.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7216 2022-02-27 20:26:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/mitlab.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1888 2022-02-27 15:21:23.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/tuebingen_2019.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5604 2022-02-27 20:26:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/uci_adl_binary.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:22.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1755 2022-03-26 11:45:38.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/changepoint.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2389 2022-03-26 11:45:38.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/lastfired.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16185 2022-03-26 11:45:38.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/raw.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/dataset/bokeh/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-06-08 12:41:16.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/bokeh/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    26262 2022-02-26 17:55:45.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/bokeh/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13816 2022-11-04 08:18:29.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/io.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-29 16:09:37.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16891 2022-11-11 10:22:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/act_and_devs.py
--rw-r--r--   0 chris     (1000) chris     (1000)    20932 2022-07-19 11:48:50.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    32382 2022-11-11 10:22:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4498 2020-12-25 12:52:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/discrete.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3460 2020-09-02 22:18:42.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/image.py
--rw-r--r--   0 chris     (1000) chris     (1000)    40971 2022-11-11 09:54:13.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:42.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8582 2022-02-27 15:41:43.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    33823 2022-11-13 19:49:51.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/acts_and_devs.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-13 22:17:20.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7895 2022-11-13 09:30:23.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/callbacks.py
--rw-r--r--   0 chris     (1000) chris     (1000)    39517 2022-11-13 09:38:08.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/dashboard.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    36938 2022-11-11 19:28:09.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/layout.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8661 2022-03-26 11:45:39.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/devices.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5782 2022-11-12 16:55:09.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/
--rw-r--r--   0 chris     (1000) chris     (1000)      880 2021-08-19 19:01:44.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14163 2022-11-13 09:16:51.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    18770 2022-11-10 08:13:02.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/acts_and_devs.py
--rw-r--r--   0 chris     (1000) chris     (1000)    20860 2022-11-10 08:13:32.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2529 2020-12-24 16:41:19.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/discrete.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2481 2022-03-26 11:45:38.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/stats/util.py
--rw-r--r--   0 chris     (1000) chris     (1000)    28389 2022-11-13 10:24:28.000000 pyadlml-0.0.7.8a0/pyadlml/dataset/util.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10134 2022-02-27 15:13:21.000000 pyadlml-0.0.7.8a0/pyadlml/feature_extraction.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1786 2020-09-02 22:18:54.000000 pyadlml-0.0.7.8a0/pyadlml/feature_selection.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7825 2021-06-29 14:23:16.000000 pyadlml-0.0.7.8a0/pyadlml/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/model/
--rw-r--r--   0 chris     (1000) chris     (1000)       95 2021-07-03 07:55:55.000000 pyadlml-0.0.7.8a0/pyadlml/model/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14720 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/_model.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.760420 pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11921 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/hmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8911 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/pchmm.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/model/hmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12315 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/_model_categorical.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6056 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3859 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhmm_hp.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6736 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6074 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/hmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9413 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/hmm/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/model/rnn/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-03 07:24:43.000000 pyadlml-0.0.7.8a0/pyadlml/model/rnn/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3398 2021-08-23 09:10:35.000000 pyadlml-0.0.7.8a0/pyadlml/model/rnn/rnn.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/model/transformer/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-08-16 15:10:00.000000 pyadlml-0.0.7.8a0/pyadlml/model/transformer/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1684 2021-08-16 15:10:29.000000 pyadlml-0.0.7.8a0/pyadlml/model/transformer/layers.py
--rw-r--r--   0 chris     (1000) chris     (1000)      705 2020-05-21 17:07:26.000000 pyadlml-0.0.7.8a0/pyadlml/model/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/model/vrnn/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-02-05 21:01:34.000000 pyadlml-0.0.7.8a0/pyadlml/model/vrnn/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)      183 2021-02-05 22:06:01.000000 pyadlml-0.0.7.8a0/pyadlml/model/vrnn/classifying_vrnn.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4513 2021-03-12 12:10:19.000000 pyadlml-0.0.7.8a0/pyadlml/model/vrnn/vrnn.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/model_selection/
--rw-r--r--   0 chris     (1000) chris     (1000)      113 2021-08-16 12:17:10.000000 pyadlml-0.0.7.8a0/pyadlml/model_selection/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    31628 2022-11-10 08:15:51.000000 pyadlml-0.0.7.8a0/pyadlml/model_selection/_search.py
--rw-r--r--   0 chris     (1000) chris     (1000)    19896 2021-08-29 15:00:49.000000 pyadlml-0.0.7.8a0/pyadlml/model_selection/_split.py
--rw-r--r--   0 chris     (1000) chris     (1000)    33208 2022-11-10 08:14:54.000000 pyadlml-0.0.7.8a0/pyadlml/pipeline.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/pyadlml/plot/
--rw-r--r--   0 chris     (1000) chris     (1000)     1784 2022-02-26 21:27:23.000000 pyadlml-0.0.7.8a0/pyadlml/plot/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5984 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/pyadlml/plot/_benchmark.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3935 2020-05-21 17:04:42.000000 pyadlml-0.0.7.8a0/pyadlml/plot/explanation.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2695 2020-05-21 17:04:42.000000 pyadlml-0.0.7.8a0/pyadlml/plot/feature_importance.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6752 2020-05-28 14:58:05.000000 pyadlml-0.0.7.8a0/pyadlml/plot/interpretation.py
--rw-r--r--   0 chris     (1000) chris     (1000)    25582 2022-03-26 11:45:39.000000 pyadlml-0.0.7.8a0/pyadlml/preprocessing.py
--rw-r--r--   0 chris     (1000) chris     (1000)      849 2021-10-28 15:24:21.000000 pyadlml-0.0.7.8a0/pyadlml/stats.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1306 2020-12-24 20:43:33.000000 pyadlml-0.0.7.8a0/pyadlml/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.756420 pyadlml-0.0.7.8a0/pyadlml.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-13 22:18:03.000000 pyadlml-0.0.7.8a0/pyadlml.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     4001 2022-11-13 22:18:03.000000 pyadlml-0.0.7.8a0/pyadlml.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-13 22:18:03.000000 pyadlml-0.0.7.8a0/pyadlml.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      264 2022-11-13 22:18:03.000000 pyadlml-0.0.7.8a0/pyadlml.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       24 2022-11-13 22:18:03.000000 pyadlml-0.0.7.8a0/pyadlml.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.764420 pyadlml-0.0.7.8a0/scripts/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:02:55.000000 pyadlml-0.0.7.8a0/scripts/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1703 2022-02-21 21:37:20.000000 pyadlml-0.0.7.8a0/scripts/generate_dataset_info.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)     1664 2022-11-13 22:17:42.000000 pyadlml-0.0.7.8a0/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/testing/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/testing/models/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/testing/models/hmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5253 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_hass_forwardhmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10706 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_hass_pchmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12916 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_homeassistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7011 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_kasteren.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6855 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_kasteren_pom.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8518 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hmm/testing_pendigits.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-13 22:18:03.768420 pyadlml-0.0.7.8a0/testing/models/hsmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hsmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6932 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hsmm/testing_kasteren_hsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10437 2020-05-21 08:54:05.000000 pyadlml-0.0.7.8a0/testing/models/hsmm/testing_pyhsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11793 2022-02-26 12:12:51.000000 pyadlml-0.0.7.8a0/testing/models/hsmm/testing_ssm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3045 2021-08-22 19:43:50.000000 pyadlml-0.0.7.8a0/testing/test_crossval.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2052 2021-04-27 13:28:35.000000 pyadlml-0.0.7.8a0/testing/test_dataset_amsterdam.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2091 2021-04-28 07:06:03.000000 pyadlml-0.0.7.8a0/testing/test_dataset_aras.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6888 2021-08-14 20:00:22.000000 pyadlml-0.0.7.8a0/testing/test_dataset_base.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1589 2021-04-27 13:36:49.000000 pyadlml-0.0.7.8a0/testing/test_dataset_casas_aruba.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5925 2021-08-14 20:00:22.000000 pyadlml-0.0.7.8a0/testing/test_dataset_dirty.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7272 2021-08-14 20:00:22.000000 pyadlml-0.0.7.8a0/testing/test_dataset_empty_partial.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2816 2021-04-27 13:38:30.000000 pyadlml-0.0.7.8a0/testing/test_dataset_mitlab.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1606 2021-04-28 07:23:55.000000 pyadlml-0.0.7.8a0/testing/test_dataset_tuebingen2019.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2889 2021-04-28 07:23:16.000000 pyadlml-0.0.7.8a0/testing/test_dataset_uci_adl_binary.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1381 2021-03-13 11:57:30.000000 pyadlml-0.0.7.8a0/testing/test_feature_extraction.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1571 2021-04-23 20:32:20.000000 pyadlml-0.0.7.8a0/testing/test_gridsearch.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1890 2021-01-14 11:07:32.000000 pyadlml-0.0.7.8a0/testing/test_imports.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4008 2021-04-23 20:32:20.000000 pyadlml-0.0.7.8a0/testing/test_pipeline.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2730 2021-06-29 09:26:25.000000 pyadlml-0.0.7.8a0/testing/test_preprocessing.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3281 2021-10-28 08:54:13.000000 pyadlml-0.0.7.8a0/testing/test_utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2020-10-29 09:58:19.000000 pyadlml-0.0.7.9a0/MANIFEST.in
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     6164 2022-10-26 18:21:17.000000 pyadlml-0.0.7.9a0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml/
+-rw-r--r--   0 chris     (1000) chris     (1000)      774 2022-10-26 19:47:31.000000 pyadlml-0.0.7.9a0/pyadlml/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2735 2021-08-16 09:39:57.000000 pyadlml-0.0.7.9a0/pyadlml/benchmark.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      743 2022-10-21 09:41:03.000000 pyadlml-0.0.7.9a0/pyadlml/constants.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml/dataset/
+-rw-r--r--   0 chris     (1000) chris     (1000)      827 2022-10-26 19:48:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-01-16 14:29:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3723 2022-11-10 08:12:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/_dataset.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    17657 2022-11-13 10:03:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/activities.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    29737 2022-11-10 08:15:15.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/devices.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7431 2022-10-28 13:22:22.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/obj.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-19 16:38:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3551 2022-11-14 11:15:15.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/activity_assistant.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5714 2022-10-28 21:53:36.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/amsterdam.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7335 2022-11-11 12:45:06.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/aras.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6857 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/casas_aruba.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4278 2022-10-18 20:14:29.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/homeassistant.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9878 2022-11-13 10:04:34.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/kasteren_2010.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7216 2022-02-27 20:26:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/mitlab.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1888 2022-02-27 15:21:23.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/tuebingen_2019.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5604 2022-02-27 20:26:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/uci_adl_binary.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:22.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1755 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/changepoint.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2389 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/lastfired.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    16185 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/raw.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-06-08 12:41:16.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    26262 2022-02-26 17:55:45.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/activities.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13816 2022-11-04 08:18:29.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/io.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-29 16:09:37.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    16891 2022-11-11 10:22:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/act_and_devs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    20932 2022-07-19 11:48:50.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/activities.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    32382 2022-11-11 10:22:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/devices.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4498 2020-12-25 12:52:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/discrete.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3460 2020-09-02 22:18:42.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/image.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    40971 2022-11-11 09:54:13.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:42.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8582 2022-02-27 15:41:43.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/activities.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    34211 2022-11-14 13:19:31.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/acts_and_devs.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-13 22:17:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7895 2022-11-13 09:30:23.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/callbacks.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    39517 2022-11-13 09:38:08.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/dashboard.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    36938 2022-11-11 19:28:09.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/layout.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8661 2022-03-26 11:45:39.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/devices.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5782 2022-11-12 16:55:09.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/
+-rw-r--r--   0 chris     (1000) chris     (1000)      880 2021-08-19 19:01:44.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14163 2022-11-13 09:16:51.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/activities.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    18770 2022-11-10 08:13:02.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/acts_and_devs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    20860 2022-11-10 08:13:32.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/devices.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2529 2020-12-24 16:41:19.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/discrete.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2481 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/util.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    28389 2022-11-13 10:24:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/util.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10134 2022-02-27 15:13:21.000000 pyadlml-0.0.7.9a0/pyadlml/feature_extraction.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1786 2020-09-02 22:18:54.000000 pyadlml-0.0.7.9a0/pyadlml/feature_selection.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7825 2021-06-29 14:23:16.000000 pyadlml-0.0.7.9a0/pyadlml/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/
+-rw-r--r--   0 chris     (1000) chris     (1000)       95 2021-07-03 07:55:55.000000 pyadlml-0.0.7.9a0/pyadlml/model/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14720 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/_model.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    11921 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/hmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8911 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/pchmm.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/hmm/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12315 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/_model_categorical.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6056 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3859 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm_hp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6736 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhsmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6074 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/hmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9413 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/rnn/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-03 07:24:43.000000 pyadlml-0.0.7.9a0/pyadlml/model/rnn/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3398 2021-08-23 09:10:35.000000 pyadlml-0.0.7.9a0/pyadlml/model/rnn/rnn.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/transformer/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-08-16 15:10:00.000000 pyadlml-0.0.7.9a0/pyadlml/model/transformer/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1684 2021-08-16 15:10:29.000000 pyadlml-0.0.7.9a0/pyadlml/model/transformer/layers.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      705 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-02-05 21:01:34.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      183 2021-02-05 22:06:01.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/classifying_vrnn.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4513 2021-03-12 12:10:19.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/vrnn.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model_selection/
+-rw-r--r--   0 chris     (1000) chris     (1000)      113 2021-08-16 12:17:10.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    31628 2022-11-10 08:15:51.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/_search.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    19896 2021-08-29 15:00:49.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/_split.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    33208 2022-11-10 08:14:54.000000 pyadlml-0.0.7.9a0/pyadlml/pipeline.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/pyadlml/plot/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1784 2022-02-26 21:27:23.000000 pyadlml-0.0.7.9a0/pyadlml/plot/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5984 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/plot/_benchmark.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3935 2020-05-21 17:04:42.000000 pyadlml-0.0.7.9a0/pyadlml/plot/explanation.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2695 2020-05-21 17:04:42.000000 pyadlml-0.0.7.9a0/pyadlml/plot/feature_importance.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6752 2020-05-28 14:58:05.000000 pyadlml-0.0.7.9a0/pyadlml/plot/interpretation.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    25582 2022-03-26 11:45:39.000000 pyadlml-0.0.7.9a0/pyadlml/preprocessing.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      849 2021-10-28 15:24:21.000000 pyadlml-0.0.7.9a0/pyadlml/stats.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1306 2020-12-24 20:43:33.000000 pyadlml-0.0.7.9a0/pyadlml/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4001 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      264 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       24 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/scripts/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:02:55.000000 pyadlml-0.0.7.9a0/scripts/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1703 2022-02-21 21:37:20.000000 pyadlml-0.0.7.9a0/scripts/generate_dataset_info.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/setup.cfg
+-rw-r--r--   0 chris     (1000) chris     (1000)     1664 2022-11-14 13:23:30.000000 pyadlml-0.0.7.9a0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/models/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/models/hmm/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5253 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_forwardhmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10706 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_pchmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12916 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_homeassistant.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7011 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6855 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren_pom.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8518 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_pendigits.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/testing/models/hsmm/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6932 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_kasteren_hsmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10437 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_pyhsmm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    11793 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_ssm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3045 2021-08-22 19:43:50.000000 pyadlml-0.0.7.9a0/testing/test_crossval.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2052 2021-04-27 13:28:35.000000 pyadlml-0.0.7.9a0/testing/test_dataset_amsterdam.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2091 2021-04-28 07:06:03.000000 pyadlml-0.0.7.9a0/testing/test_dataset_aras.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6888 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_base.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1589 2021-04-27 13:36:49.000000 pyadlml-0.0.7.9a0/testing/test_dataset_casas_aruba.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5925 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_dirty.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7272 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_empty_partial.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2816 2021-04-27 13:38:30.000000 pyadlml-0.0.7.9a0/testing/test_dataset_mitlab.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1606 2021-04-28 07:23:55.000000 pyadlml-0.0.7.9a0/testing/test_dataset_tuebingen2019.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2889 2021-04-28 07:23:16.000000 pyadlml-0.0.7.9a0/testing/test_dataset_uci_adl_binary.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1381 2021-03-13 11:57:30.000000 pyadlml-0.0.7.9a0/testing/test_feature_extraction.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1571 2021-04-23 20:32:20.000000 pyadlml-0.0.7.9a0/testing/test_gridsearch.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1890 2021-01-14 11:07:32.000000 pyadlml-0.0.7.9a0/testing/test_imports.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4008 2021-04-23 20:32:20.000000 pyadlml-0.0.7.9a0/testing/test_pipeline.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2730 2021-06-29 09:26:25.000000 pyadlml-0.0.7.9a0/testing/test_preprocessing.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3281 2021-10-28 08:54:13.000000 pyadlml-0.0.7.9a0/testing/test_utils.py
```

### Comparing `pyadlml-0.0.7.8a0/PKG-INFO` & `pyadlml-0.0.7.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadlml
-Version: 0.0.7.8a0
+Version: 0.0.7.9a0
 Summary: Sklearn flavored library containing numerous Activity of Daily Livings datasets, preprocessing methods and visualizations.
 Home-page: https://github.com/tcsvn/pyadlml
 Author: Christian Meier
 Author-email: account@meier-lossburg.de
 License: MIT
 Description: # Activities of Daily Living - Machine Learning
         > Contains data preprocessing and visualization methods for ADL datasets.
```

### Comparing `pyadlml-0.0.7.8a0/README.md` & `pyadlml-0.0.7.9a0/README.md`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/__init__.py` & `pyadlml-0.0.7.9a0/pyadlml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/benchmark.py` & `pyadlml-0.0.7.9a0/pyadlml/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/constants.py` & `pyadlml-0.0.7.9a0/pyadlml/constants.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/__init__.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_core/_dataset.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/_dataset.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_core/activities.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/activities.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_core/devices.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/devices.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_core/obj.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/obj.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/activity_assistant.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/activity_assistant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pandas as pd
 from pathlib import Path
-from pyadlml.dataset._core.obj import Data
 from pyadlml.constants import START_TIME, END_TIME, DEVICE, VALUE, TIME, ACTIVITY
 from pyadlml.dataset.io import correct_acts_and_devs
+from pyadlml.dataset.plotly.util import ActivityDict
 
 DATA_NAME = 'devices.csv'
 DEV_MAP_NAME = 'device_map.csv'
 ACT_MAP_NAME = 'activity_map.csv'
 ACT_NAME = 'activities_subject_%s.csv'
 MAP_ID = 'id'
 
@@ -45,15 +45,15 @@
 
 
 def _read_device_list(path_to_file):
     lst_devices = pd.read_csv(path_to_file)
     return list(lst_devices[DEVICE])
 
 # TODO refactor into new dictionary based rep
-def load(folder_path: str, subjects:list=[], retain_corrections=False) -> Data:
+def load(folder_path: str, subjects:list=[], retain_corrections=False) -> dict:
     """
     Loads a dataset generated by activity-assistant from a specified folder.
 
     Parameters
     ----------
     folder_path : str
         The path to the folder where the dataset is located.
@@ -80,26 +80,28 @@
                            Path(folder_path).joinpath(DEV_MAP_NAME))
 
     # get mappings
     lst_dev = _read_device_list(Path(folder_path).joinpath(DEV_MAP_NAME))
     lst_act = _read_activity_list(Path(folder_path).joinpath(ACT_MAP_NAME))
 
     #data = Data(None, df_dev, activity_list=lst_act, device_list=lst_dev)
-    data = dict(
-        df_devices=df_dev,
-        activity_list=lst_act,
-        device_list=lst_dev
-    )
+
 
 
     # If no subjects where specified read the files from the folder following the naming schemata
     if not subjects:
         for fp in Path(folder_path).iterdir():
             if ACT_NAME[:18] in fp.name:
                 subjects.append(fp.name[19:-4])
 
+    act_dct = ActivityDict()
     for subject in subjects:
         df_act = _read_activities(Path(folder_path).joinpath(ACT_NAME%(subject)),
                                   Path(folder_path).joinpath(ACT_MAP_NAME))
-        data[f'df_activities_{subject}'] = df_act
+        act_dct[subject] = df_act
 
-    return data
+    return dict(
+        df_devices=df_dev,
+        device_list=lst_dev,
+        df_activities=act_dct,
+        activity_list=lst_act,
+    )
```

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/amsterdam.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/amsterdam.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/aras.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/aras.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/casas_aruba.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/casas_aruba.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/homeassistant.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/homeassistant.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/kasteren_2010.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/kasteren_2010.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/mitlab.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/mitlab.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/tuebingen_2019.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/tuebingen_2019.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_datasets/uci_adl_binary.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/uci_adl_binary.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/changepoint.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/changepoint.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/lastfired.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/lastfired.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/_representations/raw.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/raw.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/bokeh/activities.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/activities.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/io.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/io.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/act_and_devs.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/act_and_devs.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/activities.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/activities.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/devices.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/devices.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/discrete.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/discrete.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/image.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/matplotlib/util.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/activities.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/activities.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/acts_and_devs.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/acts_and_devs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,24 @@
 from pyadlml.dataset.plotly.activities import _set_compact_title
 from pyadlml.dataset.stats.acts_and_devs import contingency_table_states, contingency_table_events
 from pyadlml.dataset.util import select_timespan, df_difference, activity_order_by, device_order_by, infer_dtypes
 
 
 __all__ = ['activities_and_devices', 'contingency_states', 'contingency_events']
 
+def _dynamic_and_height(nr_subj, nr_devs):
+    # Additional rows for sel. marker
+    m = (350 - 380)/(10 - 12)
+    b = 0
+    possible_rows = nr_subj + nr_devs + (nr_subj + 1)    
+    height = int(m*possible_rows + b)
+    print(f'height: {height} = {m}*{possible_rows} + {b}')
+    return min(height, 1000)
+
+
 
 def _plot_device_states_into_fig(fig: go.Figure, df_devs: pd.DataFrame,  df_devs_usel: pd.DataFrame,
                                  df_devs_outside: pd.DataFrame, dev_order: list, st=None, et=None) -> go.Figure:
     """
     Parameters
     ----------
     df_devs_outside : list of dicts
@@ -544,14 +554,16 @@
     # Get the y-axis and label order
     act_order = activity_order_by(dct_acts_sel.concat(), rule=act_order)
     dev_order = device_order_by(df_devs_sel, rule=dev_order)
 
 
     # determinte visual properties
     nr_devs = len(dev_order)
+    nr_subjs = len(dct_acts)
+    height = _dynamic_and_height(nr_devs, nr_subjs)
     marker_height = 3 if nr_devs > 15 else 5
     y_label_size = _dyn_y_label_size(height, nr_devs)
 
     # Reconstruct outside parts
     df_devs_outside = df_difference(df_devs_sel, df_devs)
     dct_acts_outside = act_difference(dct_acts_sel, dct_acts, st, et)
```

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/callbacks.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/dashboard.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/dashboard/layout.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/devices.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/devices.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/plotly/util.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/__init__.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/activities.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/activities.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/acts_and_devs.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/acts_and_devs.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/devices.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/devices.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/discrete.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/discrete.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/stats/util.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/dataset/util.py` & `pyadlml-0.0.7.9a0/pyadlml/dataset/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/feature_extraction.py` & `pyadlml-0.0.7.9a0/pyadlml/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/feature_selection.py` & `pyadlml-0.0.7.9a0/pyadlml/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/metrics.py` & `pyadlml-0.0.7.9a0/pyadlml/metrics.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/_model.py` & `pyadlml-0.0.7.9a0/pyadlml/model/_model.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/hmm.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/hmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hbhmm/pchmm.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/pchmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/_model_categorical.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/_model_categorical.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhmm.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhmm_hp.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm_hp.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/bhsmm.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhsmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/hmm.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/hmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/hmm/util.py` & `pyadlml-0.0.7.9a0/pyadlml/model/hmm/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/rnn/rnn.py` & `pyadlml-0.0.7.9a0/pyadlml/model/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/transformer/layers.py` & `pyadlml-0.0.7.9a0/pyadlml/model/transformer/layers.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/util.py` & `pyadlml-0.0.7.9a0/pyadlml/model/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model/vrnn/vrnn.py` & `pyadlml-0.0.7.9a0/pyadlml/model/vrnn/vrnn.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model_selection/_search.py` & `pyadlml-0.0.7.9a0/pyadlml/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/model_selection/_split.py` & `pyadlml-0.0.7.9a0/pyadlml/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/pipeline.py` & `pyadlml-0.0.7.9a0/pyadlml/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/plot/__init__.py` & `pyadlml-0.0.7.9a0/pyadlml/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/plot/_benchmark.py` & `pyadlml-0.0.7.9a0/pyadlml/plot/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/plot/explanation.py` & `pyadlml-0.0.7.9a0/pyadlml/plot/explanation.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/plot/feature_importance.py` & `pyadlml-0.0.7.9a0/pyadlml/plot/feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/plot/interpretation.py` & `pyadlml-0.0.7.9a0/pyadlml/plot/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/preprocessing.py` & `pyadlml-0.0.7.9a0/pyadlml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/stats.py` & `pyadlml-0.0.7.9a0/pyadlml/stats.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml/util.py` & `pyadlml-0.0.7.9a0/pyadlml/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/pyadlml.egg-info/PKG-INFO` & `pyadlml-0.0.7.9a0/pyadlml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadlml
-Version: 0.0.7.8a0
+Version: 0.0.7.9a0
 Summary: Sklearn flavored library containing numerous Activity of Daily Livings datasets, preprocessing methods and visualizations.
 Home-page: https://github.com/tcsvn/pyadlml
 Author: Christian Meier
 Author-email: account@meier-lossburg.de
 License: MIT
 Description: # Activities of Daily Living - Machine Learning
         > Contains data preprocessing and visualization methods for ADL datasets.
```

### Comparing `pyadlml-0.0.7.8a0/pyadlml.egg-info/SOURCES.txt` & `pyadlml-0.0.7.9a0/pyadlml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/scripts/generate_dataset_info.py` & `pyadlml-0.0.7.9a0/scripts/generate_dataset_info.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/setup.py` & `pyadlml-0.0.7.9a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 _extras_all = _extras_light + _extras_datavis
 
 
 
 setup_args = dict(
     name="pyadlml",
-    version="0.0.7.8-alpha",
+    version="0.0.7.9-alpha",
     url="https://github.com/tcsvn/pyadlml",
     author="Christian Meier",
     description="Sklearn flavored library containing numerous Activity of Daily Livings datasets, preprocessing methods and visualizations.",
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     author_email="account@meier-lossburg.de",
     license="MIT",
```

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_hass_forwardhmm.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_forwardhmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_hass_pchmm.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_pchmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_homeassistant.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_homeassistant.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_kasteren.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_kasteren_pom.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren_pom.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hmm/testing_pendigits.py` & `pyadlml-0.0.7.9a0/testing/models/hmm/testing_pendigits.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hsmm/testing_kasteren_hsmm.py` & `pyadlml-0.0.7.9a0/testing/models/hsmm/testing_kasteren_hsmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hsmm/testing_pyhsmm.py` & `pyadlml-0.0.7.9a0/testing/models/hsmm/testing_pyhsmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/models/hsmm/testing_ssm.py` & `pyadlml-0.0.7.9a0/testing/models/hsmm/testing_ssm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_crossval.py` & `pyadlml-0.0.7.9a0/testing/test_crossval.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_amsterdam.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_amsterdam.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_aras.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_aras.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_base.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_base.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_casas_aruba.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_casas_aruba.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_dirty.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_dirty.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_empty_partial.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_empty_partial.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_mitlab.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_mitlab.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_tuebingen2019.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_tuebingen2019.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_dataset_uci_adl_binary.py` & `pyadlml-0.0.7.9a0/testing/test_dataset_uci_adl_binary.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_feature_extraction.py` & `pyadlml-0.0.7.9a0/testing/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_gridsearch.py` & `pyadlml-0.0.7.9a0/testing/test_gridsearch.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_imports.py` & `pyadlml-0.0.7.9a0/testing/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_pipeline.py` & `pyadlml-0.0.7.9a0/testing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_preprocessing.py` & `pyadlml-0.0.7.9a0/testing/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.8a0/testing/test_utils.py` & `pyadlml-0.0.7.9a0/testing/test_utils.py`

 * *Files identical despite different names*

