# Comparing `tmp/eegsynth-0.7.4.tar.gz` & `tmp/eegsynth-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eegsynth-0.7.4.tar", last modified: Sat May 13 14:02:58 2023, max compression
+gzip compressed data, was "eegsynth-0.7.5.tar", last modified: Sun May 14 08:05:33 2023, max compression
```

## Comparing `eegsynth-0.7.4.tar` & `eegsynth-0.7.5.tar`

### file list

```diff
@@ -1,272 +1,274 @@
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.560207 eegsynth-0.7.4/
--rw-r--r--   0 roboos     (503) staff       (20)    32472 2023-03-21 19:58:52.000000 eegsynth-0.7.4/LICENSE
--rw-r--r--   0 roboos     (503) staff       (20)     4291 2023-05-13 14:02:58.559710 eegsynth-0.7.4/PKG-INFO
--rw-r--r--   0 roboos     (503) staff       (20)     2698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/README.md
--rwxr-xr-x   0 roboos     (503) staff       (20)    16584 2023-05-13 13:59:05.000000 eegsynth-0.7.4/eegsynth-gui.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.424331 eegsynth-0.7.4/eegsynth.egg-info/
--rw-r--r--   0 roboos     (503) staff       (20)     4291 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/PKG-INFO
--rw-r--r--   0 roboos     (503) staff       (20)     5540 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/SOURCES.txt
--rw-r--r--   0 roboos     (503) staff       (20)        1 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/dependency_links.txt
--rw-r--r--   0 roboos     (503) staff       (20)       44 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/entry_points.txt
--rw-r--r--   0 roboos     (503) staff       (20)      296 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/requires.txt
--rw-r--r--   0 roboos     (503) staff       (20)        9 2023-05-13 14:02:58.000000 eegsynth-0.7.4/eegsynth.egg-info/top_level.txt
--rwxr-xr-x   0 roboos     (503) staff       (20)    13516 2023-05-13 13:58:07.000000 eegsynth-0.7.4/eegsynth.py
--rw-r--r--   0 roboos     (503) staff       (20)     1388 2023-05-04 12:16:58.000000 eegsynth-0.7.4/hook-pylsl.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.433258 eegsynth-0.7.4/lib/
--rw-r--r--   0 roboos     (503) staff       (20)     1656 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/ArtNet.py
--rw-r--r--   0 roboos     (503) staff       (20)     1450 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/DummyRedis.py
--rw-r--r--   0 roboos     (503) staff       (20)    17162 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/EDF.py
--rw-r--r--   0 roboos     (503) staff       (20)    35670 2023-05-02 20:55:48.000000 eegsynth-0.7.4/lib/EEGsynth.py
--rw-r--r--   0 roboos     (503) staff       (20)     1975 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/FakeRedis.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    27618 2023-04-30 19:35:59.000000 eegsynth-0.7.4/lib/FieldTrip.py
--rw-r--r--   0 roboos     (503) staff       (20)      435 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/FieldTrip_test_client.py
--rw-r--r--   0 roboos     (503) staff       (20)      301 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/FieldTrip_test_server.py
--rw-r--r--   0 roboos     (503) staff       (20)     1131 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/Redis_test_client.py
--rw-r--r--   0 roboos     (503) staff       (20)     2193 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/RingBuffer.py
--rw-r--r--   0 roboos     (503) staff       (20)     7184 2023-05-02 18:05:03.000000 eegsynth-0.7.4/lib/ZmqRedis.py
--rw-r--r--   0 roboos     (503) staff       (20)        0 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/__init__.py
--rw-r--r--   0 roboos     (503) staff       (20)    59022 2023-03-21 19:58:52.000000 eegsynth-0.7.4/lib/colormap.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.434141 eegsynth-0.7.4/module/
--rw-r--r--   0 roboos     (503) staff       (20)        0 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/__init__.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.435089 eegsynth-0.7.4/module/accelerometer/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/accelerometer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5707 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/accelerometer/accelerometer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.436377 eegsynth-0.7.4/module/audio2ft/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/audio2ft/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6708 2023-04-29 08:49:58.000000 eegsynth-0.7.4/module/audio2ft/audio2ft.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.437755 eegsynth-0.7.4/module/audiomixer/
--rwxr-xr-x   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/audiomixer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7220 2023-04-29 09:10:40.000000 eegsynth-0.7.4/module/audiomixer/audiomixer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.438528 eegsynth-0.7.4/module/biochill/
--rwxr-xr-x   0 roboos     (503) staff       (20)     7879 2023-04-29 08:15:56.000000 eegsynth-0.7.4/module/biochill/biochill.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.439475 eegsynth-0.7.4/module/bitalino2ft/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/bitalino2ft/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6396 2023-04-29 09:15:26.000000 eegsynth-0.7.4/module/bitalino2ft/bitalino2ft.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.440896 eegsynth-0.7.4/module/brainflow2ft/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/brainflow2ft/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6322 2023-04-29 08:15:56.000000 eegsynth-0.7.4/module/brainflow2ft/brainflow2ft.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.442840 eegsynth-0.7.4/module/buffer/
--rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/buffer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     3468 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/buffer/buffer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.444523 eegsynth-0.7.4/module/clockdivider/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/clockdivider/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5433 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/clockdivider/clockdivider.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.445888 eegsynth-0.7.4/module/clockmultiplier/
--rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/clockmultiplier/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7267 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/clockmultiplier/clockmultiplier.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.448156 eegsynth-0.7.4/module/cogito/
--rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/cogito/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    12302 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/cogito/cogito.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     4202 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/cogito/gtec2wav.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.449585 eegsynth-0.7.4/module/complexity/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/complexity/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8635 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/complexity/complexity.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.450711 eegsynth-0.7.4/module/compressor/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/compressor/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5131 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/compressor/compressor.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.452118 eegsynth-0.7.4/module/csp/
--rw-r--r--   0 roboos     (503) staff       (20)      687 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/csp/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    12865 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/csp/csp.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.453425 eegsynth-0.7.4/module/delaytrigger/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/delaytrigger/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5784 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/delaytrigger/delaytrigger.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.455698 eegsynth-0.7.4/module/demodulatetone/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/demodulatetone/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9517 2023-04-29 09:15:47.000000 eegsynth-0.7.4/module/demodulatetone/demodulatetone.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.457380 eegsynth-0.7.4/module/endorphines/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/endorphines/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9952 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/endorphines/endorphines.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.459262 eegsynth-0.7.4/module/example/
--rw-r--r--   0 roboos     (503) staff       (20)      691 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/example/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     4008 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/example/example.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.461846 eegsynth-0.7.4/module/generateclock/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/generateclock/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    12009 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/generateclock/generateclock.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.463943 eegsynth-0.7.4/module/generatecontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/generatecontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8392 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/generatecontrol/generatecontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.467310 eegsynth-0.7.4/module/generatesignal/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/generatesignal/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    10722 2023-05-02 20:11:22.000000 eegsynth-0.7.4/module/generatesignal/generatesignal.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.468852 eegsynth-0.7.4/module/generatetrigger/
--rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/generatetrigger/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6763 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/generatetrigger/generatetrigger.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.473748 eegsynth-0.7.4/module/geomixer/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/geomixer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8648 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/geomixer/geomixer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.475626 eegsynth-0.7.4/module/heartrate/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/heartrate/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8413 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/heartrate/heartrate.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.477143 eegsynth-0.7.4/module/historycontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/historycontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9494 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/historycontrol/historycontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.478604 eegsynth-0.7.4/module/historysignal/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/historysignal/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9401 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/historysignal/historysignal.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.480566 eegsynth-0.7.4/module/inputcontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      427 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputcontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    17279 2023-05-10 07:50:04.000000 eegsynth-0.7.4/module/inputcontrol/inputcontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.482837 eegsynth-0.7.4/module/inputlsl/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputlsl/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6618 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/inputlsl/inputlsl.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.484144 eegsynth-0.7.4/module/inputmidi/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputmidi/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5264 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/inputmidi/inputmidi.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.485426 eegsynth-0.7.4/module/inputmqtt/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputmqtt/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5957 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/inputmqtt/inputmqtt.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.486824 eegsynth-0.7.4/module/inputosc/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputosc/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8044 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/inputosc/inputosc.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.488674 eegsynth-0.7.4/module/inputzeromq/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/inputzeromq/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     5740 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/inputzeromq/inputzeromq.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.490463 eegsynth-0.7.4/module/keyboard/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/keyboard/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    14634 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/keyboard/keyboard.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.492264 eegsynth-0.7.4/module/launchcontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/launchcontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    13953 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/launchcontrol/launchcontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.493544 eegsynth-0.7.4/module/launchpad/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/launchpad/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    14601 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/launchpad/launchpad.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.495098 eegsynth-0.7.4/module/logging/
--rw-r--r--   0 roboos     (503) staff       (20)      422 2023-04-30 07:48:46.000000 eegsynth-0.7.4/module/logging/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7275 2023-04-30 20:43:41.000000 eegsynth-0.7.4/module/logging/logging.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.496555 eegsynth-0.7.4/module/lsl2ft/
--rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/lsl2ft/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6768 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/lsl2ft/lsl2ft.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.498199 eegsynth-0.7.4/module/modulatetone/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/modulatetone/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    10550 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/modulatetone/modulatetone.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.499814 eegsynth-0.7.4/module/outputartnet/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputartnet/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6639 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputartnet/outputartnet.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.501174 eegsynth-0.7.4/module/outputaudio/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputaudio/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    12350 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputaudio/outputaudio.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.502782 eegsynth-0.7.4/module/outputcvgate/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputcvgate/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    10263 2023-05-07 13:53:03.000000 eegsynth-0.7.4/module/outputcvgate/outputcvgate.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.504248 eegsynth-0.7.4/module/outputdmx/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputdmx/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6984 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputdmx/outputdmx.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.505828 eegsynth-0.7.4/module/outputgpio/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputgpio/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8490 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputgpio/outputgpio.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.507349 eegsynth-0.7.4/module/outputlsl/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputlsl/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7652 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputlsl/outputlsl.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.508686 eegsynth-0.7.4/module/outputmidi/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputmidi/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    13389 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputmidi/outputmidi.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.510079 eegsynth-0.7.4/module/outputmqtt/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputmqtt/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7263 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputmqtt/outputmqtt.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.511387 eegsynth-0.7.4/module/outputosc/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputosc/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7596 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputosc/outputosc.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.512818 eegsynth-0.7.4/module/outputzeromq/
--rwxr-xr-x   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/outputzeromq/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6590 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/outputzeromq/outputzeromq.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.514246 eegsynth-0.7.4/module/pepipiaf/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/pepipiaf/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    25727 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/pepipiaf/pepipiaf.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.515790 eegsynth-0.7.4/module/playbackcontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/playbackcontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6454 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/playbackcontrol/playbackcontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.517084 eegsynth-0.7.4/module/playbacksignal/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/playbacksignal/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9858 2023-05-02 20:53:32.000000 eegsynth-0.7.4/module/playbacksignal/playbacksignal.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.518696 eegsynth-0.7.4/module/plotcontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      426 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/plotcontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7058 2023-04-30 20:43:43.000000 eegsynth-0.7.4/module/plotcontrol/plotcontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.520076 eegsynth-0.7.4/module/plotimage/
--rw-r--r--   0 roboos     (503) staff       (20)      424 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/plotimage/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6780 2023-04-30 20:43:48.000000 eegsynth-0.7.4/module/plotimage/plotimage.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.521677 eegsynth-0.7.4/module/plotsignal/
--rw-r--r--   0 roboos     (503) staff       (20)      425 2023-04-30 19:40:07.000000 eegsynth-0.7.4/module/plotsignal/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    11992 2023-04-30 20:43:51.000000 eegsynth-0.7.4/module/plotsignal/plotsignal.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.523243 eegsynth-0.7.4/module/plotspectral/
--rw-r--r--   0 roboos     (503) staff       (20)      427 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/plotspectral/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    23337 2023-04-30 20:43:55.000000 eegsynth-0.7.4/module/plotspectral/plotspectral.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.525166 eegsynth-0.7.4/module/plottext/
--rw-r--r--   0 roboos     (503) staff       (20)      423 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/plottext/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7894 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/plottext/plottext.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.526437 eegsynth-0.7.4/module/plottopo/
--rw-r--r--   0 roboos     (503) staff       (20)      423 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/plottopo/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8637 2023-04-30 20:44:05.000000 eegsynth-0.7.4/module/plottopo/plottopo.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.527686 eegsynth-0.7.4/module/plottrigger/
--rw-r--r--   0 roboos     (503) staff       (20)      426 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/plottrigger/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8295 2023-04-30 20:44:08.000000 eegsynth-0.7.4/module/plottrigger/plottrigger.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.528304 eegsynth-0.7.4/module/polarbelt/
--rwxr-xr-x   0 roboos     (503) staff       (20)     4608 2023-04-29 08:15:56.000000 eegsynth-0.7.4/module/polarbelt/polarbelt.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.529363 eegsynth-0.7.4/module/postprocessing/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/postprocessing/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6740 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/postprocessing/postprocessing.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.530524 eegsynth-0.7.4/module/preprocessing/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/preprocessing/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    14798 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/preprocessing/preprocessing.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.531984 eegsynth-0.7.4/module/processtrigger/
--rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/processtrigger/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9670 2023-05-02 19:32:40.000000 eegsynth-0.7.4/module/processtrigger/processtrigger.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.533392 eegsynth-0.7.4/module/quantizer/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/quantizer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6181 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/quantizer/quantizer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.534550 eegsynth-0.7.4/module/recordcontrol/
--rw-r--r--   0 roboos     (503) staff       (20)      701 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/recordcontrol/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    10121 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/recordcontrol/recordcontrol.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.535760 eegsynth-0.7.4/module/recordsignal/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/recordsignal/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    11451 2023-05-02 20:50:47.000000 eegsynth-0.7.4/module/recordsignal/recordsignal.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.537197 eegsynth-0.7.4/module/recordtrigger/
--rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/recordtrigger/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8005 2023-05-13 08:01:31.000000 eegsynth-0.7.4/module/recordtrigger/recordtrigger.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.538477 eegsynth-0.7.4/module/redis/
--rw-r--r--   0 roboos     (503) staff       (20)      683 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/redis/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     3599 2023-04-30 20:46:28.000000 eegsynth-0.7.4/module/redis/redis.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.539761 eegsynth-0.7.4/module/rms/
--rw-r--r--   0 roboos     (503) staff       (20)      687 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/rms/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6500 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/rms/rms.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.540935 eegsynth-0.7.4/module/sampler/
--rw-r--r--   0 roboos     (503) staff       (20)      691 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/sampler/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    14409 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/sampler/sampler.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.542044 eegsynth-0.7.4/module/sequencer/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/sequencer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    10356 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/sequencer/sequencer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.543203 eegsynth-0.7.4/module/slewlimiter/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/slewlimiter/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     4470 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/slewlimiter/slewlimiter.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.544528 eegsynth-0.7.4/module/sonification/
--rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/sonification/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    15140 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/sonification/sonification.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.545950 eegsynth-0.7.4/module/spectral/
--rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/spectral/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7528 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/spectral/spectral.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.547629 eegsynth-0.7.4/module/synthesizer/
--rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/synthesizer/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    15026 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/synthesizer/synthesizer.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.549184 eegsynth-0.7.4/module/threshold/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/threshold/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7690 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/threshold/threshold.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.550437 eegsynth-0.7.4/module/unicorn2ft/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/unicorn2ft/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     7588 2023-05-07 13:53:03.000000 eegsynth-0.7.4/module/unicorn2ft/unicorn2ft.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.551882 eegsynth-0.7.4/module/videoprocessing/
--rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-25 11:03:23.000000 eegsynth-0.7.4/module/videoprocessing/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)    17749 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/videoprocessing/videoprocessing.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.554122 eegsynth-0.7.4/module/volcabass/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/volcabass/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9541 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/volcabass/volcabass.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.555617 eegsynth-0.7.4/module/volcabeats/
--rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/volcabeats/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     8370 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/volcabeats/volcabeats.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.557483 eegsynth-0.7.4/module/volcakeys/
--rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/volcakeys/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     9657 2023-04-30 15:10:12.000000 eegsynth-0.7.4/module/volcakeys/volcakeys.py
-drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-13 14:02:58.558932 eegsynth-0.7.4/module/vumeter/
--rw-r--r--   0 roboos     (503) staff       (20)      422 2023-03-21 19:58:52.000000 eegsynth-0.7.4/module/vumeter/__init__.py
--rwxr-xr-x   0 roboos     (503) staff       (20)     6651 2023-04-30 20:44:11.000000 eegsynth-0.7.4/module/vumeter/vumeter.py
--rw-r--r--   0 roboos     (503) staff       (20)       38 2023-05-13 14:02:58.560342 eegsynth-0.7.4/setup.cfg
--rwxr-xr-x   0 roboos     (503) staff       (20)     3541 2023-05-13 13:53:05.000000 eegsynth-0.7.4/setup.py
--rw-r--r--   0 roboos     (503) staff       (20)       20 2023-05-13 13:59:48.000000 eegsynth-0.7.4/version.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.120797 eegsynth-0.7.5/
+-rw-r--r--   0 roboos     (503) staff       (20)    32472 2023-03-21 19:58:52.000000 eegsynth-0.7.5/LICENSE
+-rw-r--r--   0 roboos     (503) staff       (20)     4291 2023-05-14 08:05:33.120395 eegsynth-0.7.5/PKG-INFO
+-rw-r--r--   0 roboos     (503) staff       (20)     2698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/README.md
+-rw-r--r--   0 roboos     (503) staff       (20)        0 2023-05-14 07:49:33.000000 eegsynth-0.7.5/__init__.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.923305 eegsynth-0.7.5/bin/
+-rwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 07:49:33.000000 eegsynth-0.7.5/bin/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    16584 2023-05-14 07:49:33.000000 eegsynth-0.7.5/bin/eegsynth-gui.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    13419 2023-05-14 07:49:33.000000 eegsynth-0.7.5/bin/eegsynth.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.927395 eegsynth-0.7.5/eegsynth.egg-info/
+-rw-r--r--   0 roboos     (503) staff       (20)     4291 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/PKG-INFO
+-rw-r--r--   0 roboos     (503) staff       (20)     5558 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/SOURCES.txt
+-rw-r--r--   0 roboos     (503) staff       (20)        1 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/dependency_links.txt
+-rw-r--r--   0 roboos     (503) staff       (20)       57 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/entry_points.txt
+-rw-r--r--   0 roboos     (503) staff       (20)      309 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/requires.txt
+-rw-r--r--   0 roboos     (503) staff       (20)        9 2023-05-14 08:05:32.000000 eegsynth-0.7.5/eegsynth.egg-info/top_level.txt
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.937385 eegsynth-0.7.5/lib/
+-rw-r--r--   0 roboos     (503) staff       (20)     1656 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/ArtNet.py
+-rw-r--r--   0 roboos     (503) staff       (20)     1450 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/DummyRedis.py
+-rw-r--r--   0 roboos     (503) staff       (20)    17162 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/EDF.py
+-rw-r--r--   0 roboos     (503) staff       (20)    35670 2023-05-02 20:55:48.000000 eegsynth-0.7.5/lib/EEGsynth.py
+-rw-r--r--   0 roboos     (503) staff       (20)     1975 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/FakeRedis.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    27618 2023-04-30 19:35:59.000000 eegsynth-0.7.5/lib/FieldTrip.py
+-rw-r--r--   0 roboos     (503) staff       (20)      435 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/FieldTrip_test_client.py
+-rw-r--r--   0 roboos     (503) staff       (20)      301 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/FieldTrip_test_server.py
+-rw-r--r--   0 roboos     (503) staff       (20)     1131 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/Redis_test_client.py
+-rw-r--r--   0 roboos     (503) staff       (20)     2193 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/RingBuffer.py
+-rw-r--r--   0 roboos     (503) staff       (20)     7184 2023-05-02 18:05:03.000000 eegsynth-0.7.5/lib/ZmqRedis.py
+-rw-r--r--   0 roboos     (503) staff       (20)        0 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/__init__.py
+-rw-r--r--   0 roboos     (503) staff       (20)    59022 2023-03-21 19:58:52.000000 eegsynth-0.7.5/lib/colormap.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.938347 eegsynth-0.7.5/module/
+-rw-r--r--   0 roboos     (503) staff       (20)        0 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/__init__.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.939493 eegsynth-0.7.5/module/accelerometer/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/accelerometer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5707 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/accelerometer/accelerometer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.940771 eegsynth-0.7.5/module/audio2ft/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/audio2ft/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6708 2023-04-29 08:49:58.000000 eegsynth-0.7.5/module/audio2ft/audio2ft.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.942174 eegsynth-0.7.5/module/audiomixer/
+-rwxr-xr-x   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/audiomixer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7220 2023-04-29 09:10:40.000000 eegsynth-0.7.5/module/audiomixer/audiomixer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.942975 eegsynth-0.7.5/module/biochill/
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7879 2023-04-29 08:15:56.000000 eegsynth-0.7.5/module/biochill/biochill.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.944550 eegsynth-0.7.5/module/bitalino2ft/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/bitalino2ft/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6396 2023-04-29 09:15:26.000000 eegsynth-0.7.5/module/bitalino2ft/bitalino2ft.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.945819 eegsynth-0.7.5/module/brainflow2ft/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/brainflow2ft/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6322 2023-04-29 08:15:56.000000 eegsynth-0.7.5/module/brainflow2ft/brainflow2ft.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.949122 eegsynth-0.7.5/module/buffer/
+-rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/buffer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     3468 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/buffer/buffer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.951665 eegsynth-0.7.5/module/clockdivider/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/clockdivider/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5433 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/clockdivider/clockdivider.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.953302 eegsynth-0.7.5/module/clockmultiplier/
+-rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/clockmultiplier/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7267 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/clockmultiplier/clockmultiplier.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.954881 eegsynth-0.7.5/module/cogito/
+-rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/cogito/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    12302 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/cogito/cogito.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     4202 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/cogito/gtec2wav.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.955844 eegsynth-0.7.5/module/complexity/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/complexity/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8635 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/complexity/complexity.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.956806 eegsynth-0.7.5/module/compressor/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/compressor/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5131 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/compressor/compressor.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.957748 eegsynth-0.7.5/module/csp/
+-rw-r--r--   0 roboos     (503) staff       (20)      687 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/csp/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    12865 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/csp/csp.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.958657 eegsynth-0.7.5/module/delaytrigger/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/delaytrigger/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5784 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/delaytrigger/delaytrigger.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.959589 eegsynth-0.7.5/module/demodulatetone/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/demodulatetone/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9517 2023-04-29 09:15:47.000000 eegsynth-0.7.5/module/demodulatetone/demodulatetone.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.960597 eegsynth-0.7.5/module/endorphines/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/endorphines/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9952 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/endorphines/endorphines.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.961505 eegsynth-0.7.5/module/example/
+-rw-r--r--   0 roboos     (503) staff       (20)      691 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/example/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     4008 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/example/example.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.962480 eegsynth-0.7.5/module/generateclock/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/generateclock/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    12009 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/generateclock/generateclock.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.963535 eegsynth-0.7.5/module/generatecontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/generatecontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8392 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/generatecontrol/generatecontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.964578 eegsynth-0.7.5/module/generatesignal/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/generatesignal/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    10722 2023-05-02 20:11:22.000000 eegsynth-0.7.5/module/generatesignal/generatesignal.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.965556 eegsynth-0.7.5/module/generatetrigger/
+-rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/generatetrigger/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6763 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/generatetrigger/generatetrigger.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.966592 eegsynth-0.7.5/module/geomixer/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/geomixer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8648 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/geomixer/geomixer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.967639 eegsynth-0.7.5/module/heartrate/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/heartrate/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8413 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/heartrate/heartrate.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.968585 eegsynth-0.7.5/module/historycontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/historycontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9494 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/historycontrol/historycontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.969456 eegsynth-0.7.5/module/historysignal/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/historysignal/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9401 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/historysignal/historysignal.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.970390 eegsynth-0.7.5/module/inputcontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      427 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputcontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    17279 2023-05-10 07:50:04.000000 eegsynth-0.7.5/module/inputcontrol/inputcontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.971368 eegsynth-0.7.5/module/inputlsl/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputlsl/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6618 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/inputlsl/inputlsl.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.972257 eegsynth-0.7.5/module/inputmidi/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputmidi/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5264 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/inputmidi/inputmidi.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.973143 eegsynth-0.7.5/module/inputmqtt/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputmqtt/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5957 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/inputmqtt/inputmqtt.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.974085 eegsynth-0.7.5/module/inputosc/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputosc/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8044 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/inputosc/inputosc.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.997105 eegsynth-0.7.5/module/inputzeromq/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/inputzeromq/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     5740 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/inputzeromq/inputzeromq.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.998020 eegsynth-0.7.5/module/keyboard/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/keyboard/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    14634 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/keyboard/keyboard.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:32.999277 eegsynth-0.7.5/module/launchcontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/launchcontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    13953 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/launchcontrol/launchcontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.000452 eegsynth-0.7.5/module/launchpad/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/launchpad/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    14601 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/launchpad/launchpad.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.001453 eegsynth-0.7.5/module/logging/
+-rw-r--r--   0 roboos     (503) staff       (20)      422 2023-04-30 07:48:46.000000 eegsynth-0.7.5/module/logging/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7275 2023-04-30 20:43:41.000000 eegsynth-0.7.5/module/logging/logging.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.002396 eegsynth-0.7.5/module/lsl2ft/
+-rw-r--r--   0 roboos     (503) staff       (20)      690 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/lsl2ft/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6768 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/lsl2ft/lsl2ft.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.003356 eegsynth-0.7.5/module/modulatetone/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/modulatetone/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    10550 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/modulatetone/modulatetone.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.004331 eegsynth-0.7.5/module/outputartnet/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputartnet/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6639 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputartnet/outputartnet.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.005293 eegsynth-0.7.5/module/outputaudio/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputaudio/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    12350 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputaudio/outputaudio.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.006224 eegsynth-0.7.5/module/outputcvgate/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputcvgate/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    10263 2023-05-07 13:53:03.000000 eegsynth-0.7.5/module/outputcvgate/outputcvgate.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.007259 eegsynth-0.7.5/module/outputdmx/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputdmx/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6984 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputdmx/outputdmx.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.008141 eegsynth-0.7.5/module/outputgpio/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputgpio/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8490 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputgpio/outputgpio.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.009124 eegsynth-0.7.5/module/outputlsl/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputlsl/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7652 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputlsl/outputlsl.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.010109 eegsynth-0.7.5/module/outputmidi/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputmidi/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    13389 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputmidi/outputmidi.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.011041 eegsynth-0.7.5/module/outputmqtt/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputmqtt/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7263 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputmqtt/outputmqtt.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.012024 eegsynth-0.7.5/module/outputosc/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputosc/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7596 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputosc/outputosc.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.012996 eegsynth-0.7.5/module/outputzeromq/
+-rwxr-xr-x   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/outputzeromq/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6590 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/outputzeromq/outputzeromq.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.014005 eegsynth-0.7.5/module/pepipiaf/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/pepipiaf/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    25727 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/pepipiaf/pepipiaf.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.015186 eegsynth-0.7.5/module/playbackcontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/playbackcontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6454 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/playbackcontrol/playbackcontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.016465 eegsynth-0.7.5/module/playbacksignal/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/playbacksignal/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9858 2023-05-02 20:53:32.000000 eegsynth-0.7.5/module/playbacksignal/playbacksignal.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.017763 eegsynth-0.7.5/module/plotcontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      426 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/plotcontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7058 2023-04-30 20:43:43.000000 eegsynth-0.7.5/module/plotcontrol/plotcontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.018782 eegsynth-0.7.5/module/plotimage/
+-rw-r--r--   0 roboos     (503) staff       (20)      424 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/plotimage/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6780 2023-04-30 20:43:48.000000 eegsynth-0.7.5/module/plotimage/plotimage.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.019756 eegsynth-0.7.5/module/plotsignal/
+-rw-r--r--   0 roboos     (503) staff       (20)      425 2023-04-30 19:40:07.000000 eegsynth-0.7.5/module/plotsignal/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    11992 2023-04-30 20:43:51.000000 eegsynth-0.7.5/module/plotsignal/plotsignal.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.020690 eegsynth-0.7.5/module/plotspectral/
+-rw-r--r--   0 roboos     (503) staff       (20)      427 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/plotspectral/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    23337 2023-04-30 20:43:55.000000 eegsynth-0.7.5/module/plotspectral/plotspectral.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.021765 eegsynth-0.7.5/module/plottext/
+-rw-r--r--   0 roboos     (503) staff       (20)      423 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/plottext/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7894 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/plottext/plottext.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.023110 eegsynth-0.7.5/module/plottopo/
+-rw-r--r--   0 roboos     (503) staff       (20)      423 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/plottopo/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8637 2023-04-30 20:44:05.000000 eegsynth-0.7.5/module/plottopo/plottopo.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.025019 eegsynth-0.7.5/module/plottrigger/
+-rw-r--r--   0 roboos     (503) staff       (20)      426 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/plottrigger/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8295 2023-04-30 20:44:08.000000 eegsynth-0.7.5/module/plottrigger/plottrigger.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.025549 eegsynth-0.7.5/module/polarbelt/
+-rwxr-xr-x   0 roboos     (503) staff       (20)     4608 2023-04-29 08:15:56.000000 eegsynth-0.7.5/module/polarbelt/polarbelt.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.026790 eegsynth-0.7.5/module/postprocessing/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/postprocessing/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6740 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/postprocessing/postprocessing.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.029816 eegsynth-0.7.5/module/preprocessing/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/preprocessing/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    14798 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/preprocessing/preprocessing.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.035866 eegsynth-0.7.5/module/processtrigger/
+-rw-r--r--   0 roboos     (503) staff       (20)      698 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/processtrigger/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9670 2023-05-02 19:32:40.000000 eegsynth-0.7.5/module/processtrigger/processtrigger.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.037074 eegsynth-0.7.5/module/quantizer/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/quantizer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6181 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/quantizer/quantizer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.039114 eegsynth-0.7.5/module/recordcontrol/
+-rw-r--r--   0 roboos     (503) staff       (20)      701 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/recordcontrol/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    10121 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/recordcontrol/recordcontrol.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.041714 eegsynth-0.7.5/module/recordsignal/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/recordsignal/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    11451 2023-05-02 20:50:47.000000 eegsynth-0.7.5/module/recordsignal/recordsignal.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.042736 eegsynth-0.7.5/module/recordtrigger/
+-rw-r--r--   0 roboos     (503) staff       (20)      697 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/recordtrigger/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8005 2023-05-13 08:01:31.000000 eegsynth-0.7.5/module/recordtrigger/recordtrigger.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.043758 eegsynth-0.7.5/module/redis/
+-rw-r--r--   0 roboos     (503) staff       (20)      683 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/redis/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     3599 2023-04-30 20:46:28.000000 eegsynth-0.7.5/module/redis/redis.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.048234 eegsynth-0.7.5/module/rms/
+-rw-r--r--   0 roboos     (503) staff       (20)      687 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/rms/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6500 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/rms/rms.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.049285 eegsynth-0.7.5/module/sampler/
+-rw-r--r--   0 roboos     (503) staff       (20)      691 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/sampler/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    14409 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/sampler/sampler.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.050833 eegsynth-0.7.5/module/sequencer/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/sequencer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    10356 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/sequencer/sequencer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.052639 eegsynth-0.7.5/module/slewlimiter/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/slewlimiter/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     4470 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/slewlimiter/slewlimiter.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.053583 eegsynth-0.7.5/module/sonification/
+-rw-r--r--   0 roboos     (503) staff       (20)      696 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/sonification/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    15140 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/sonification/sonification.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.054729 eegsynth-0.7.5/module/spectral/
+-rw-r--r--   0 roboos     (503) staff       (20)      692 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/spectral/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7528 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/spectral/spectral.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.055986 eegsynth-0.7.5/module/synthesizer/
+-rw-r--r--   0 roboos     (503) staff       (20)      695 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/synthesizer/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    15026 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/synthesizer/synthesizer.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.113269 eegsynth-0.7.5/module/threshold/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/threshold/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7690 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/threshold/threshold.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.114513 eegsynth-0.7.5/module/unicorn2ft/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/unicorn2ft/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     7588 2023-05-07 13:53:03.000000 eegsynth-0.7.5/module/unicorn2ft/unicorn2ft.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.115945 eegsynth-0.7.5/module/videoprocessing/
+-rw-r--r--   0 roboos     (503) staff       (20)      699 2023-03-25 11:03:23.000000 eegsynth-0.7.5/module/videoprocessing/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)    17749 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/videoprocessing/videoprocessing.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.116908 eegsynth-0.7.5/module/volcabass/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/volcabass/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9541 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/volcabass/volcabass.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.118071 eegsynth-0.7.5/module/volcabeats/
+-rw-r--r--   0 roboos     (503) staff       (20)      694 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/volcabeats/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     8370 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/volcabeats/volcabeats.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.118963 eegsynth-0.7.5/module/volcakeys/
+-rw-r--r--   0 roboos     (503) staff       (20)      693 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/volcakeys/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     9657 2023-04-30 15:10:12.000000 eegsynth-0.7.5/module/volcakeys/volcakeys.py
+drwxr-xr-x   0 roboos     (503) staff       (20)        0 2023-05-14 08:05:33.119811 eegsynth-0.7.5/module/vumeter/
+-rw-r--r--   0 roboos     (503) staff       (20)      422 2023-03-21 19:58:52.000000 eegsynth-0.7.5/module/vumeter/__init__.py
+-rwxr-xr-x   0 roboos     (503) staff       (20)     6651 2023-04-30 20:44:11.000000 eegsynth-0.7.5/module/vumeter/vumeter.py
+-rw-r--r--   0 roboos     (503) staff       (20)       38 2023-05-14 08:05:33.120934 eegsynth-0.7.5/setup.cfg
+-rwxr-xr-x   0 roboos     (503) staff       (20)     3589 2023-05-14 07:49:33.000000 eegsynth-0.7.5/setup.py
+-rw-r--r--   0 roboos     (503) staff       (20)       20 2023-05-14 07:49:33.000000 eegsynth-0.7.5/version.py
```

### Comparing `eegsynth-0.7.4/LICENSE` & `eegsynth-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/PKG-INFO` & `eegsynth-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eegsynth
-Version: 0.7.4
+Version: 0.7.5
 Summary: Converting real-time EEG into sounds, music and visual effects
 Home-page: http://www.eegsynth.org
 Author: Robert Oostenveld
 Author-email: r.oostenveld@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://github.com/eegsynth/eegsynth/blob/master/doc/README.md
 Project-URL: Source, https://github.com/eegsynth/eegsynth/
```

### Comparing `eegsynth-0.7.4/README.md` & `eegsynth-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/eegsynth-gui.py` & `eegsynth-0.7.5/bin/eegsynth-gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,21 @@
 from PyQt5.QtWidgets import QApplication, QWidget
 
 path = os.path.dirname(os.path.realpath(__file__))
 file = os.path.split(__file__)[-1]
 name = os.path.splitext(file)[0]
 
 # eegsynth contains the version
-sys.path.insert(0, os.path.join(path))
+sys.path.insert(0, os.path.join(path, '..'))
+from version import __version__
+
 # eegsynth/lib contains shared modules
-sys.path.insert(0, os.path.join(path, 'lib'))
+sys.path.insert(0, os.path.join(path, '../lib'))
 import EEGsynth
 import FieldTrip
-from version import __version__
 
 from module import accelerometer, audio2ft, audiomixer, bitalino2ft, buffer, clockdivider, clockmultiplier, cogito, compressor, csp, delaytrigger, demodulatetone, endorphines, example, generateclock, generatecontrol, generatesignal, generatetrigger, geomixer, heartrate, historycontrol, historysignal, inputcontrol, inputlsl, inputmidi, inputmqtt, inputosc, inputzeromq, keyboard, launchcontrol, launchpad, logging, lsl2ft, modulatetone, outputartnet, outputaudio, outputcvgate, outputdmx, outputlsl, outputmidi, outputmqtt, outputosc, outputzeromq, pepipiaf, playbackcontrol, playbacksignal, plotcontrol, plotimage, plotsignal, plotspectral, plottext, plottopo, plottrigger, postprocessing, preprocessing, processtrigger, redis, quantizer, recordcontrol, recordsignal, recordtrigger, rms, sampler, sequencer, slewlimiter, sonification, spectral, synthesizer, threshold, unicorn2ft, videoprocessing, volcabass, volcabeats, volcakeys, vumeter
 
 # this will contain a list of modules and processes
 modules = []
 processes = []
 
@@ -76,14 +77,15 @@
 
 
 def _start_module(module, args=None):
     # the module starts as soon as it is instantiated
     # optional command-line arguments can be passed to specify the ini file
     module(args)
 
+
 def _loop_once():
     '''Run the main loop once
     '''
     # updating the main figure is done through Qt events
     global monitor, modules, processes
     # remove modules that are not running any more
     keep      = [p.is_alive() for p in processes]
@@ -349,33 +351,32 @@
                 monitor.error('incorrect module', name)
                 return
 
             # pass only the specific ini file
             args['inifile'] = inifile
 
             # pass all other arguments
-            args_to_pass = []
+            args_list = []
             for k, v in args.items():
                 # reformat them back into command-line arguments
-                args_to_pass += ['--' + k.replace('_', '-'), v]
+                args_list += ['--' + k.replace('_', '-'), v]
 
             # give some feedback
-            monitor.success(name + ' ' + ' '.join(args_to_pass))
+            monitor.success(name + ' ' + ' '.join(args_list))
 
-            process = multiprocessing.Process(target=_start_module, args=(module_to_start.Executable, args_to_pass))
+            process = multiprocessing.Process(target=_start_module, args=(module_to_start.Executable, args_list))
             process.start()
 
             # keep track of all modules and processes
             modules.append(fullname)
             processes.append(process)
 
 
 def _main():
     _setup()
-
     try:
         # the icon in the taskbar should not be the python interpreter but the EEGsynth logo
         EEGsynth.appid('org.eegsynth.%s.%s' % (name, __version__))
 
         # initiate the graphical user interface
         app = QApplication(sys.argv)
         app.setWindowIcon(QtGui.QIcon(os.path.join(path, 'doc/figures/logo-128.ico')))
@@ -389,14 +390,16 @@
         # see https://stackoverflow.com/questions/4938723/what-is-the-correct-way-to-make-my-pyqt-application-quit-when-killed-from-the-co/6072360#6072360
         timer = QtCore.QTimer()
         timer.start(100)
         timer.timeout.connect(_loop_once)
         timer.timeout.connect(window.updateLabel)
 
         sys.exit(app.exec_())
+
     except (SystemExit, KeyboardInterrupt, RuntimeError):
         _stop()
 
+
 if __name__ == '__main__':
     multiprocessing.freeze_support()
     multiprocessing.set_start_method('spawn')
     _main()
```

### Comparing `eegsynth-0.7.4/eegsynth.egg-info/PKG-INFO` & `eegsynth-0.7.5/eegsynth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eegsynth
-Version: 0.7.4
+Version: 0.7.5
 Summary: Converting real-time EEG into sounds, music and visual effects
 Home-page: http://www.eegsynth.org
 Author: Robert Oostenveld
 Author-email: r.oostenveld@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://github.com/eegsynth/eegsynth/blob/master/doc/README.md
 Project-URL: Source, https://github.com/eegsynth/eegsynth/
```

### Comparing `eegsynth-0.7.4/eegsynth.egg-info/SOURCES.txt` & `eegsynth-0.7.5/eegsynth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
-./eegsynth-gui.py
-./eegsynth.py
-./hook-pylsl.py
+./__init__.py
 ./version.py
+bin/__init__.py
+bin/eegsynth-gui.py
+bin/eegsynth.py
 eegsynth.egg-info/PKG-INFO
 eegsynth.egg-info/SOURCES.txt
 eegsynth.egg-info/dependency_links.txt
 eegsynth.egg-info/entry_points.txt
 eegsynth.egg-info/requires.txt
 eegsynth.egg-info/top_level.txt
 lib/ArtNet.py
```

### Comparing `eegsynth-0.7.4/eegsynth.py` & `eegsynth-0.7.5/bin/eegsynth.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 from importlib import import_module
 
 path = os.path.dirname(os.path.realpath(__file__))
 file = os.path.split(__file__)[-1]
 name = os.path.splitext(file)[0]
 
 # eegsynth contains the version
-sys.path.insert(0, os.path.join(path))
+sys.path.insert(0, os.path.join(path, '..'))
+from version import __version__
+
 # eegsynth/lib contains shared modules
-sys.path.insert(0, os.path.join(path, 'lib'))
+sys.path.insert(0, os.path.join(path, '../lib'))
 import EEGsynth
 import FieldTrip
-from version import __version__
 
 from module import accelerometer, audio2ft, audiomixer, bitalino2ft, buffer, clockdivider, clockmultiplier, cogito, compressor, csp, delaytrigger, demodulatetone, endorphines, example, generateclock, generatecontrol, generatesignal, generatetrigger, geomixer, heartrate, historycontrol, historysignal, inputcontrol, inputlsl, inputmidi, inputmqtt, inputosc, inputzeromq, keyboard, launchcontrol, launchpad, logging, lsl2ft, modulatetone, outputartnet, outputaudio, outputcvgate, outputdmx, outputlsl, outputmidi, outputmqtt, outputosc, outputzeromq, pepipiaf, playbackcontrol, playbacksignal, plotcontrol, plotimage, plotsignal, plotspectral, plottext, plottopo, plottrigger, postprocessing, preprocessing, processtrigger, redis, quantizer, recordcontrol, recordsignal, recordtrigger, rms, sampler, sequencer, slewlimiter, sonification, spectral, synthesizer, threshold, unicorn2ft, videoprocessing, volcabass, volcabeats, volcakeys, vumeter
 
 # this will contain a list of modules and processes
 modules = []
 processes = []
 
@@ -64,41 +65,37 @@
     parser.add_argument("--general-debug", default=None, help="general debug")
     parser.add_argument("--general-delay", default=None, help="general delay")
     parser.add_argument("--general-logging", default=None, help="general logging, can be 'local' or 'remote'")
     parser.add_argument("--multiprocessing-fork")
     parser.add_argument("inifile", nargs='+', help="configuration file for a patch")
     args = parser.parse_args()
 
-    # this shows the splash screen and can be used to track parameters that have changed
-    monitor = EEGsynth.monitor(name=None, debug=1)
-
     # the first results in a list of lists, the second flattens it
     args.inifile = [glob(x) for x in args.inifile]
     args.inifile = [item for sublist in args.inifile for item in sublist]
 
     if len(args.inifile) == 0:
         raise RuntimeError('You must specify one or multiple ini files.')
 
-    # start with an empty list of files
-    inifiles = []
+    # this shows the splash screen and can be used to track parameters that have changed
+    monitor = EEGsynth.monitor(name=None, debug=1)
 
-    for file_or_dir in args.inifile:
-        if os.path.isfile(file_or_dir):
-            if not file_or_dir.endswith('.ini'):
+    for inifile in args.inifile:
+        if os.path.isfile(inifile):
+            if not inifile.endswith('.ini'):
                 raise RuntimeError('The ini file extension must be .ini')
-            inifiles += [file_or_dir]
         else:
-            raise RuntimeError('Incorrect command line argument ' + file_or_dir)
+            raise RuntimeError('Incorrect command line argument ' + inifile)
 
-    # convert the command-line arguments in a dict
+    # convert the command-line argument namespace into a dict
     args = vars(args)
     # remove empty items
     args = {k: v for k, v in args.items() if v}
 
-    for inifile in inifiles:
+    for inifile in args['inifile']:
         if os.path.splitext(inifile)[1]!='.ini':
             monitor.error('incorrect file', inifile)
             continue
 
         # reconstruct the full path
         inifile = os.path.join(os.getcwd(), inifile)
 
@@ -279,23 +276,23 @@
             monitor.error('incorrect module', name)
             return
 
         # pass only the specific ini file
         args['inifile'] = inifile
 
         # pass all other arguments
-        args_to_pass = []
+        args_list = []
         for k, v in args.items():
             # reformat them back into command-line arguments
-            args_to_pass += ['--' + k.replace('_', '-'), v]
+            args_list += ['--' + k.replace('_', '-'), v]
 
         # give some feedback
-        monitor.success(name + ' ' + ' '.join(args_to_pass))
+        monitor.success(name + ' ' + ' '.join(args_list))
 
-        process = multiprocessing.Process(target=_start_module, args=(module_to_start.Executable, args_to_pass))
+        process = multiprocessing.Process(target=_start_module, args=(module_to_start.Executable, args_list))
 
         # keep track of all modules and processes
         modules.append(fullname)
         processes.append(process)
 
 
 def _start_module(module, args=None):
```

### Comparing `eegsynth-0.7.4/lib/ArtNet.py` & `eegsynth-0.7.5/lib/ArtNet.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/DummyRedis.py` & `eegsynth-0.7.5/lib/DummyRedis.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/EDF.py` & `eegsynth-0.7.5/lib/EDF.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/EEGsynth.py` & `eegsynth-0.7.5/lib/EEGsynth.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/FakeRedis.py` & `eegsynth-0.7.5/lib/FakeRedis.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/FieldTrip.py` & `eegsynth-0.7.5/lib/FieldTrip.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/Redis_test_client.py` & `eegsynth-0.7.5/lib/Redis_test_client.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/RingBuffer.py` & `eegsynth-0.7.5/lib/RingBuffer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/ZmqRedis.py` & `eegsynth-0.7.5/lib/ZmqRedis.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/lib/colormap.py` & `eegsynth-0.7.5/lib/colormap.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/accelerometer/__init__.py` & `eegsynth-0.7.5/module/accelerometer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/accelerometer/accelerometer.py` & `eegsynth-0.7.5/module/accelerometer/accelerometer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/audio2ft/__init__.py` & `eegsynth-0.7.5/module/audio2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/audio2ft/audio2ft.py` & `eegsynth-0.7.5/module/audio2ft/audio2ft.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/audiomixer/__init__.py` & `eegsynth-0.7.5/module/audiomixer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/audiomixer/audiomixer.py` & `eegsynth-0.7.5/module/audiomixer/audiomixer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/biochill/biochill.py` & `eegsynth-0.7.5/module/biochill/biochill.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/bitalino2ft/__init__.py` & `eegsynth-0.7.5/module/bitalino2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/bitalino2ft/bitalino2ft.py` & `eegsynth-0.7.5/module/bitalino2ft/bitalino2ft.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/brainflow2ft/__init__.py` & `eegsynth-0.7.5/module/brainflow2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/brainflow2ft/brainflow2ft.py` & `eegsynth-0.7.5/module/brainflow2ft/brainflow2ft.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/buffer/__init__.py` & `eegsynth-0.7.5/module/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/buffer/buffer.py` & `eegsynth-0.7.5/module/buffer/buffer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/clockdivider/__init__.py` & `eegsynth-0.7.5/module/clockdivider/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/clockdivider/clockdivider.py` & `eegsynth-0.7.5/module/clockdivider/clockdivider.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/clockmultiplier/__init__.py` & `eegsynth-0.7.5/module/clockmultiplier/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/clockmultiplier/clockmultiplier.py` & `eegsynth-0.7.5/module/clockmultiplier/clockmultiplier.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/cogito/__init__.py` & `eegsynth-0.7.5/module/cogito/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/cogito/cogito.py` & `eegsynth-0.7.5/module/cogito/cogito.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/cogito/gtec2wav.py` & `eegsynth-0.7.5/module/cogito/gtec2wav.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/complexity/__init__.py` & `eegsynth-0.7.5/module/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/complexity/complexity.py` & `eegsynth-0.7.5/module/complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/compressor/__init__.py` & `eegsynth-0.7.5/module/compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/compressor/compressor.py` & `eegsynth-0.7.5/module/compressor/compressor.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/csp/__init__.py` & `eegsynth-0.7.5/module/csp/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/csp/csp.py` & `eegsynth-0.7.5/module/csp/csp.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/delaytrigger/__init__.py` & `eegsynth-0.7.5/module/delaytrigger/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/delaytrigger/delaytrigger.py` & `eegsynth-0.7.5/module/delaytrigger/delaytrigger.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/demodulatetone/__init__.py` & `eegsynth-0.7.5/module/demodulatetone/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/demodulatetone/demodulatetone.py` & `eegsynth-0.7.5/module/demodulatetone/demodulatetone.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/endorphines/__init__.py` & `eegsynth-0.7.5/module/endorphines/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/endorphines/endorphines.py` & `eegsynth-0.7.5/module/endorphines/endorphines.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/example/__init__.py` & `eegsynth-0.7.5/module/example/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/example/example.py` & `eegsynth-0.7.5/module/example/example.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generateclock/__init__.py` & `eegsynth-0.7.5/module/generateclock/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generateclock/generateclock.py` & `eegsynth-0.7.5/module/generateclock/generateclock.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatecontrol/__init__.py` & `eegsynth-0.7.5/module/generatecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatecontrol/generatecontrol.py` & `eegsynth-0.7.5/module/generatecontrol/generatecontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatesignal/__init__.py` & `eegsynth-0.7.5/module/generatesignal/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatesignal/generatesignal.py` & `eegsynth-0.7.5/module/generatesignal/generatesignal.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatetrigger/__init__.py` & `eegsynth-0.7.5/module/generatetrigger/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/generatetrigger/generatetrigger.py` & `eegsynth-0.7.5/module/generatetrigger/generatetrigger.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/geomixer/__init__.py` & `eegsynth-0.7.5/module/geomixer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/geomixer/geomixer.py` & `eegsynth-0.7.5/module/geomixer/geomixer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/heartrate/__init__.py` & `eegsynth-0.7.5/module/heartrate/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/heartrate/heartrate.py` & `eegsynth-0.7.5/module/heartrate/heartrate.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/historycontrol/__init__.py` & `eegsynth-0.7.5/module/historycontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/historycontrol/historycontrol.py` & `eegsynth-0.7.5/module/historycontrol/historycontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/historysignal/__init__.py` & `eegsynth-0.7.5/module/historysignal/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/historysignal/historysignal.py` & `eegsynth-0.7.5/module/historysignal/historysignal.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputcontrol/inputcontrol.py` & `eegsynth-0.7.5/module/inputcontrol/inputcontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputlsl/__init__.py` & `eegsynth-0.7.5/module/inputlsl/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputlsl/inputlsl.py` & `eegsynth-0.7.5/module/inputlsl/inputlsl.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputmidi/__init__.py` & `eegsynth-0.7.5/module/inputmidi/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputmidi/inputmidi.py` & `eegsynth-0.7.5/module/inputmidi/inputmidi.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputmqtt/__init__.py` & `eegsynth-0.7.5/module/inputmqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputmqtt/inputmqtt.py` & `eegsynth-0.7.5/module/inputmqtt/inputmqtt.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputosc/__init__.py` & `eegsynth-0.7.5/module/inputosc/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputosc/inputosc.py` & `eegsynth-0.7.5/module/inputosc/inputosc.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputzeromq/__init__.py` & `eegsynth-0.7.5/module/inputzeromq/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/inputzeromq/inputzeromq.py` & `eegsynth-0.7.5/module/inputzeromq/inputzeromq.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/keyboard/__init__.py` & `eegsynth-0.7.5/module/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/keyboard/keyboard.py` & `eegsynth-0.7.5/module/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/launchcontrol/__init__.py` & `eegsynth-0.7.5/module/launchcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/launchcontrol/launchcontrol.py` & `eegsynth-0.7.5/module/launchcontrol/launchcontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/launchpad/__init__.py` & `eegsynth-0.7.5/module/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/launchpad/launchpad.py` & `eegsynth-0.7.5/module/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/logging/logging.py` & `eegsynth-0.7.5/module/logging/logging.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/lsl2ft/__init__.py` & `eegsynth-0.7.5/module/lsl2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/lsl2ft/lsl2ft.py` & `eegsynth-0.7.5/module/lsl2ft/lsl2ft.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/modulatetone/__init__.py` & `eegsynth-0.7.5/module/modulatetone/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/modulatetone/modulatetone.py` & `eegsynth-0.7.5/module/modulatetone/modulatetone.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputartnet/__init__.py` & `eegsynth-0.7.5/module/outputartnet/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputartnet/outputartnet.py` & `eegsynth-0.7.5/module/outputartnet/outputartnet.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputaudio/__init__.py` & `eegsynth-0.7.5/module/outputaudio/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputaudio/outputaudio.py` & `eegsynth-0.7.5/module/outputaudio/outputaudio.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputcvgate/__init__.py` & `eegsynth-0.7.5/module/outputcvgate/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputcvgate/outputcvgate.py` & `eegsynth-0.7.5/module/outputcvgate/outputcvgate.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputdmx/__init__.py` & `eegsynth-0.7.5/module/outputdmx/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputdmx/outputdmx.py` & `eegsynth-0.7.5/module/outputdmx/outputdmx.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputgpio/__init__.py` & `eegsynth-0.7.5/module/outputgpio/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputgpio/outputgpio.py` & `eegsynth-0.7.5/module/outputgpio/outputgpio.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputlsl/__init__.py` & `eegsynth-0.7.5/module/outputlsl/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputlsl/outputlsl.py` & `eegsynth-0.7.5/module/outputlsl/outputlsl.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputmidi/__init__.py` & `eegsynth-0.7.5/module/outputmidi/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputmidi/outputmidi.py` & `eegsynth-0.7.5/module/outputmidi/outputmidi.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputmqtt/__init__.py` & `eegsynth-0.7.5/module/outputmqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputmqtt/outputmqtt.py` & `eegsynth-0.7.5/module/outputmqtt/outputmqtt.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputosc/__init__.py` & `eegsynth-0.7.5/module/outputosc/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputosc/outputosc.py` & `eegsynth-0.7.5/module/outputosc/outputosc.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputzeromq/__init__.py` & `eegsynth-0.7.5/module/outputzeromq/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/outputzeromq/outputzeromq.py` & `eegsynth-0.7.5/module/outputzeromq/outputzeromq.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/pepipiaf/__init__.py` & `eegsynth-0.7.5/module/pepipiaf/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/pepipiaf/pepipiaf.py` & `eegsynth-0.7.5/module/pepipiaf/pepipiaf.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/playbackcontrol/__init__.py` & `eegsynth-0.7.5/module/playbackcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/playbackcontrol/playbackcontrol.py` & `eegsynth-0.7.5/module/playbackcontrol/playbackcontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/playbacksignal/__init__.py` & `eegsynth-0.7.5/module/playbacksignal/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/playbacksignal/playbacksignal.py` & `eegsynth-0.7.5/module/playbacksignal/playbacksignal.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plotcontrol/plotcontrol.py` & `eegsynth-0.7.5/module/plotcontrol/plotcontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plotimage/plotimage.py` & `eegsynth-0.7.5/module/plotimage/plotimage.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plotsignal/plotsignal.py` & `eegsynth-0.7.5/module/plotsignal/plotsignal.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plotspectral/plotspectral.py` & `eegsynth-0.7.5/module/plotspectral/plotspectral.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plottext/plottext.py` & `eegsynth-0.7.5/module/plottext/plottext.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plottopo/plottopo.py` & `eegsynth-0.7.5/module/plottopo/plottopo.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/plottrigger/plottrigger.py` & `eegsynth-0.7.5/module/plottrigger/plottrigger.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/polarbelt/polarbelt.py` & `eegsynth-0.7.5/module/polarbelt/polarbelt.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/postprocessing/__init__.py` & `eegsynth-0.7.5/module/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/postprocessing/postprocessing.py` & `eegsynth-0.7.5/module/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/preprocessing/__init__.py` & `eegsynth-0.7.5/module/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/preprocessing/preprocessing.py` & `eegsynth-0.7.5/module/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/processtrigger/__init__.py` & `eegsynth-0.7.5/module/processtrigger/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/processtrigger/processtrigger.py` & `eegsynth-0.7.5/module/processtrigger/processtrigger.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/quantizer/__init__.py` & `eegsynth-0.7.5/module/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/quantizer/quantizer.py` & `eegsynth-0.7.5/module/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordcontrol/__init__.py` & `eegsynth-0.7.5/module/recordcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordcontrol/recordcontrol.py` & `eegsynth-0.7.5/module/recordcontrol/recordcontrol.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordsignal/__init__.py` & `eegsynth-0.7.5/module/recordsignal/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordsignal/recordsignal.py` & `eegsynth-0.7.5/module/recordsignal/recordsignal.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordtrigger/__init__.py` & `eegsynth-0.7.5/module/recordtrigger/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/recordtrigger/recordtrigger.py` & `eegsynth-0.7.5/module/recordtrigger/recordtrigger.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/redis/__init__.py` & `eegsynth-0.7.5/module/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/redis/redis.py` & `eegsynth-0.7.5/module/redis/redis.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/rms/__init__.py` & `eegsynth-0.7.5/module/rms/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/rms/rms.py` & `eegsynth-0.7.5/module/rms/rms.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sampler/__init__.py` & `eegsynth-0.7.5/module/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sampler/sampler.py` & `eegsynth-0.7.5/module/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sequencer/__init__.py` & `eegsynth-0.7.5/module/sequencer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sequencer/sequencer.py` & `eegsynth-0.7.5/module/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/slewlimiter/__init__.py` & `eegsynth-0.7.5/module/slewlimiter/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/slewlimiter/slewlimiter.py` & `eegsynth-0.7.5/module/slewlimiter/slewlimiter.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sonification/__init__.py` & `eegsynth-0.7.5/module/sonification/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/sonification/sonification.py` & `eegsynth-0.7.5/module/sonification/sonification.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/spectral/__init__.py` & `eegsynth-0.7.5/module/spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/spectral/spectral.py` & `eegsynth-0.7.5/module/spectral/spectral.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/synthesizer/__init__.py` & `eegsynth-0.7.5/module/synthesizer/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/synthesizer/synthesizer.py` & `eegsynth-0.7.5/module/synthesizer/synthesizer.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/threshold/__init__.py` & `eegsynth-0.7.5/module/threshold/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/threshold/threshold.py` & `eegsynth-0.7.5/module/threshold/threshold.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/unicorn2ft/__init__.py` & `eegsynth-0.7.5/module/unicorn2ft/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/unicorn2ft/unicorn2ft.py` & `eegsynth-0.7.5/module/unicorn2ft/unicorn2ft.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/videoprocessing/__init__.py` & `eegsynth-0.7.5/module/videoprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/videoprocessing/videoprocessing.py` & `eegsynth-0.7.5/module/videoprocessing/videoprocessing.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcabass/__init__.py` & `eegsynth-0.7.5/module/volcabass/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcabass/volcabass.py` & `eegsynth-0.7.5/module/volcabass/volcabass.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcabeats/__init__.py` & `eegsynth-0.7.5/module/volcabeats/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcabeats/volcabeats.py` & `eegsynth-0.7.5/module/volcabeats/volcabeats.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcakeys/__init__.py` & `eegsynth-0.7.5/module/volcakeys/__init__.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/volcakeys/volcakeys.py` & `eegsynth-0.7.5/module/volcakeys/volcakeys.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/module/vumeter/vumeter.py` & `eegsynth-0.7.5/module/vumeter/vumeter.py`

 * *Files identical despite different names*

### Comparing `eegsynth-0.7.4/setup.py` & `eegsynth-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,19 @@
         "fuzzywuzzy[speedup]",
         "matplotlib",
         "mido",
         "nilearn",
         "numpy",
         "opencv-python",
         "paho-mqtt",
+        "pandas",
         "pyaudio",
         "pylsl",
-        "pyqtgraph==0.11",
+        "PyQt5",
+        "pyqtgraph==0.12",
         "pyserial",
         "pyzmq",
         "redis",
         "scipy",
         "sklearn",
         "termcolor",
         "wiringpi; platform_machine == 'armv7l'"
@@ -94,11 +96,11 @@
     extras_require={
         ":python_version<'3.5'": ["pyOSC"],
         ":python_version>='3.5'": ["python-rtmidi"],
         ":python_version>='3.5'": ["python-osc"]
     },
     entry_points={
         'console_scripts': [
-            'eegsynth = eegsynth:_main'
+            'eegsynth = eegsynth.bin.eegsynth:_main'
         ],
     },
 )
```

