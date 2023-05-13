# Comparing `tmp/pyresidfp-0.6.4.tar.gz` & `tmp/pyresidfp-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.6.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.4.tar` & `pyresidfp-0.6.5.tar`

### file list

```diff
@@ -1,63 +1,62 @@
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/.gitignore
--rw-r--r--   0        0        0     3761 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/README.md
--rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/PythonSid.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/config.h.in
--rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    10774 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9208 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/README
--rw-r--r--   0        0        0    13758 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/Voice.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     2788 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/resample/test.cpp
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/residfp/version.cc
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/sidcxx11.h
--rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/src/sidcxx14.h
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/.gitignore
+-rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/README.md
+-rw-r--r--   0        0        0     2314 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/PythonSid.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/config.h.in
+-rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    10889 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/README
+-rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/Voice.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/residfp/version.cc
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/sidcxx11.h
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/src/sidcxx14.h
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.5/PKG-INFO
```

### Comparing `pyresidfp-0.6.4/CMakeLists.txt` & `pyresidfp-0.6.5/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,18 +34,22 @@
 " HAVE_BUILTIN_EXPECT)
 
 check_ipo_supported(RESULT IPO_SUPPORTED OUTPUT IPO_ERROR)
 
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_EXTENSIONS OFF)
 set(PACKAGE_VERSION ${PROJECT_VERSION})
-set(RESID_INLINE inline)
-set(RESID_INLINING 1)
+option(ENABLE_INLINING "Enable inlining" ON)
+if(ENABLE_INLINING)
+  set(RESID_INLINE inline)
+  set(RESID_INLINING 1)
+endif()
 set(RESID_BRANCH_HINTS 1)
-set(HAVE_CXX11 1)
+set(HAVE_CXX11 $<COMPILE_FEATURES:cxx_std_11>)
+set(HAVE_CXX14 $<COMPILE_FEATURES:cxx_std_14>)
 
 configure_file(src/residfp/siddefs-fp.h.in siddefs-fp.h)
 configure_file(src/config.h.in config.h)
 
 set(HEADER_FILES
         ${CMAKE_CURRENT_BINARY_DIR}/siddefs-fp.h
         ${CMAKE_CURRENT_BINARY_DIR}/config.h
```

### Comparing `pyresidfp-0.6.4/COPYING` & `pyresidfp-0.6.5/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/README.md` & `pyresidfp-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/pyproject.toml` & `pyresidfp-0.6.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [tool.scikit-build]
 metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
 sdist.include = ["src/pyresidfp/_version.py"]
-sdist.exclude = [".github", "scripts"]
+sdist.exclude = [".github"]
 wheel.packages = ["src/pyresidfp"]
+wheel.install-dir = "pyresidfp"
 minimum-version = "0.3"
 
 [tool.setuptools_scm]
 write_to = "src/pyresidfp/_version.py"
 
 [project]
 name = "pyresidfp"
```

### Comparing `pyresidfp-0.6.4/src/PythonSid.cpp` & `pyresidfp-0.6.5/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/PythonSid.h` & `pyresidfp-0.6.5/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/pyresidfp/__init__.py` & `pyresidfp-0.6.5/src/pyresidfp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,7 +16,13 @@
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from .musical_scale import Tone
 from .registers import AttackDecayBits, ControlBits, ModeVolBits, ReadableRegister, ResFiltBits, SustainReleaseBits, \
     WritableRegister
 from .sound_interface_device import SoundInterfaceDevice, Voice, _VoiceRegister
+from ._version import version, version_tuple, __version__, __version_tuple__
+
+__all__ = [
+    "Tone", "AttackDecayBits", "ControlBits", "ModeVolBits", "ReadableRegister", "ResFiltBits", "SustainReleaseBits",
+    "WritableRegister", "SoundInterfaceDevice", "Voice",
+]
```

### Comparing `pyresidfp-0.6.4/src/pyresidfp/musical_scale.py` & `pyresidfp-0.6.5/src/pyresidfp/musical_scale.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/pyresidfp/registers.py` & `pyresidfp-0.6.5/src/pyresidfp/registers.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.6.5/src/pyresidfp/sound_interface_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import datetime
 import logging
+import typing as t
 from enum import Enum
-from typing import Any, Callable, Dict, Tuple
-
-from _pyresidfp import ChipModel, SID, SamplingMethod
 
+from ._pyresidfp import ChipModel, SID, SamplingMethod
 from .musical_scale import Tone
 from .registers import ReadableRegister, WritableRegister
 
 
 class Voice(Enum):
     """The three voices of an emulated MOS 6581 / MOS 8580"""
     ONE = 0
@@ -55,56 +54,57 @@
         Returns:
             WritableRegister according to register type and voice
         """
         return WritableRegister(self.value + 7 * voice.value)
 
 
 class _Metaclass(type):
-    def __init__(cls, name: str, bases: Tuple[type, ...], attrs: Dict[str, Any]) -> None:
+    def __init__(cls, name: str, bases: t.Tuple[type, ...], attrs: t.Dict[str, t.Any]) -> None:
         super(_Metaclass, cls).__init__(name, bases, attrs)
 
         for register in WritableRegister:
             setter = type(cls)._create_setter(register)
             setattr(cls, register.name,
                     property(fget=None, fset=setter, doc="int: Writable {0:s} 8-bit register".format(register.name)))
 
         for register in ReadableRegister:
             getter = type(cls)._create_getter(register)
             setattr(cls, register.name,
                     property(fget=getter, doc="int: Readable {0:s} 8-bit register".format(register.name)))
 
     @staticmethod
-    def _create_setter(register: WritableRegister) -> Callable[[Any, int], None]:
+    def _create_setter(register: WritableRegister) -> t.Callable[[t.Any, int], None]:
         def setter(self, value: int) -> None:
             self.write_register(register, value)
 
         return setter
 
     @staticmethod
-    def _create_getter(register: ReadableRegister) -> Callable[[Any], int]:
+    def _create_getter(register: ReadableRegister) -> t.Callable[[t.Any], int]:
         def getter(self) -> int:
             return self.read_register(register)
 
         return getter
 
+
 class SoundInterfaceDevice(metaclass=_Metaclass):
     """Emulation for MOS 6581 / MOS 8580 chips."""
 
-    PAL_CLOCK_FREQUENCY = 985248.0
-    NTSC_CLOCK_FREQUENCY = 1022730.0
-    DEFAULT_CLOCK_FREQUENCY = PAL_CLOCK_FREQUENCY
-    DEFAULT_SAMPLING_RATE = 48000.0
-    DEFAULT_SAMPLING_METHOD = SamplingMethod.RESAMPLE
-    DEFAULT_CHIP_MODEL = ChipModel.MOS6581
+    PAL_CLOCK_FREQUENCY: float = 985248.0
+    NTSC_CLOCK_FREQUENCY: float = 1022730.0
+    DEFAULT_CLOCK_FREQUENCY: float = PAL_CLOCK_FREQUENCY
+    DEFAULT_SAMPLING_RATE: float = 48000.0
+    DEFAULT_SAMPLING_METHOD: SamplingMethod = SamplingMethod.RESAMPLE
+    DEFAULT_CHIP_MODEL: ChipModel = ChipModel.MOS6581
 
     def __init__(self,
-                 model: ChipModel = None,
-                 sampling_method: SamplingMethod = None,
-                 clock_frequency: int = None,
-                 sampling_frequency: int = None) -> None:
+                 model: t.Optional[ChipModel] = None,
+                 sampling_method: t.Optional[SamplingMethod] = None,
+                 clock_frequency: t.Optional[int] = None,
+                 sampling_frequency: t.Optional[int] = None) -> None:
         """Creates a new instance."""
         self._log = logging.getLogger(__name__)
         chip_model = model or type(self).DEFAULT_CHIP_MODEL
         sampling_method = sampling_method or type(self).DEFAULT_SAMPLING_METHOD
         clock_frequency = clock_frequency or type(self).DEFAULT_CLOCK_FREQUENCY
         sampling_frequency = sampling_frequency or type(self).DEFAULT_SAMPLING_RATE
         assert 0 < sampling_frequency <= clock_frequency
@@ -246,15 +246,16 @@
 
         Returns:
             list of int containing the sampled output in -32768 to 32767 range
         """
         num_cycles = int(duration.total_seconds() * self.clock_frequency)
         num_samples = int(duration.total_seconds() * self.sampling_frequency)
 
-        self._log.debug("Clock for %f cycles (%f samples estimated) for an interval of %s", num_cycles, num_samples, duration)
+        self._log.debug("Clock for %f cycles (%f samples estimated) for an interval of %s",
+                        num_cycles, num_samples, duration)
 
         # native sample format is signed 16-bit integers in host endianness
         result = self._sid.clock(num_cycles)
 
         self._log.debug("Retrieved %d samples", len(result))
 
         return result
```

### Comparing `pyresidfp-0.6.4/src/pyresidfp.cpp` & `pyresidfp-0.6.5/src/pyresidfp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/COPYING` & `pyresidfp-0.6.5/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Dac.cpp` & `pyresidfp-0.6.5/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Dac.h` & `pyresidfp-0.6.5/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.6.5/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.6.5/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/ExternalFilter.h` & `pyresidfp-0.6.5/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter.cpp` & `pyresidfp-0.6.5/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter.h` & `pyresidfp-0.6.5/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter6581.cpp` & `pyresidfp-0.6.5/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter6581.h` & `pyresidfp-0.6.5/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter8580.cpp` & `pyresidfp-0.6.5/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Filter8580.h` & `pyresidfp-0.6.5/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig.h` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.6.5/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Integrator6581.cpp` & `pyresidfp-0.6.5/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Integrator6581.h` & `pyresidfp-0.6.5/src/residfp/Integrator6581.h`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     assert(kVgt_Vd < (1 << 16));
 
     // VCR current, scaled by m*2^15*2^15 = m*2^30
     const unsigned int If = static_cast<unsigned int>(fmc->getVcr_n_Ids_term(kVgt_Vs)) << 15;
     const unsigned int Ir = static_cast<unsigned int>(fmc->getVcr_n_Ids_term(kVgt_Vd)) << 15;
 #ifdef SLOPE_FACTOR
     const double iVcr = static_cast<double>(If - Ir);
-    const int n_I_vcr = static_cast<int>((iVcr * n) + 0.5);
+    const int n_I_vcr = static_cast<int>(iVcr * n);
 #else
     const int n_I_vcr = If - Ir;
 #endif
 
 #ifdef SLOPE_FACTOR
     // estimate new slope factor based on gate voltage
     const double gamma = 1.0;   // body effect factor
```

### Comparing `pyresidfp-0.6.4/src/residfp/Integrator8580.cpp` & `pyresidfp-0.6.5/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Integrator8580.h` & `pyresidfp-0.6.5/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/OpAmp.cpp` & `pyresidfp-0.6.5/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/OpAmp.h` & `pyresidfp-0.6.5/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Potentiometer.h` & `pyresidfp-0.6.5/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/README` & `pyresidfp-0.6.5/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/SID.cpp` & `pyresidfp-0.6.5/src/residfp/SID.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
  * * The full range of one voice is approximately 1.5V.
  * * The "zero" level rides at approximately 5.0V.
  *
  *
  * zero-x did the measuring on the 8580 (https://sourceforge.net/p/vice-emu/bugs/1036/#c5b3):
  * When it sits on basic from powerup it's at 4.72
  * Run 1.prg and check the output pin level.
- * Then run 2.prg andadjust it until the output level is the same...
+ * Then run 2.prg and adjust it until the output level is the same...
  * 0x94-0xA8 gives me the same 4.72 1.prg shows.
  * On another 8580 it's 0x90-0x9C
  * Third chip 0x94-0xA8
  * Fourth chip 0x90-0xA4
  * On the 8580 that plays digis the output is 4.66 and 0x93 is the only value to reach that.
  * To me that seems as regular 8580s have somewhat wide 0-level range,
  * whereas that digi-compatible 8580 has it very narrow.
```

### Comparing `pyresidfp-0.6.4/src/residfp/SID.h` & `pyresidfp-0.6.5/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Spline.cpp` & `pyresidfp-0.6.5/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Spline.h` & `pyresidfp-0.6.5/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/Voice.h` & `pyresidfp-0.6.5/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/WaveformCalculator.cpp` & `pyresidfp-0.6.5/src/residfp/WaveformCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/WaveformCalculator.h` & `pyresidfp-0.6.5/src/residfp/WaveformCalculator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.6.5/src/residfp/WaveformGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/WaveformGenerator.h` & `pyresidfp-0.6.5/src/residfp/WaveformGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/array.h` & `pyresidfp-0.6.5/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/resample/Resampler.h` & `pyresidfp-0.6.5/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.6.5/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/resample/SincResampler.h` & `pyresidfp-0.6.5/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.6.5/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.6.5/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.6.5/src/residfp/siddefs-fp.h.in`

 * *Files 2% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 #else
 const char* residfp_version_string = "@PACKAGE_VERSION@";
 #endif
 }
 
 // Inlining on/off.
 #cmakedefine01 RESID_INLINING
-#define RESID_INLINE @RESID_INLINE@
+#cmakedefine RESID_INLINE @RESID_INLINE@
 
 #endif // SIDDEFS_FP_H
```

### Comparing `pyresidfp-0.6.4/src/residfp/version.cc` & `pyresidfp-0.6.5/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/sidcxx11.h` & `pyresidfp-0.6.5/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/src/sidcxx14.h` & `pyresidfp-0.6.5/src/sidcxx14.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.4/PKG-INFO` & `pyresidfp-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.4
+Version: 0.6.5
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

