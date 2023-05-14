# Comparing `tmp/pyVLMP-1.0.5.tar.gz` & `tmp/pyVLMP-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVLMP-1.0.5.tar", last modified: Sun May 14 15:11:41 2023, max compression
+gzip compressed data, was "pyVLMP-1.0.6.tar", last modified: Sun May 14 15:25:33 2023, max compression
```

## Comparing `pyVLMP-1.0.5.tar` & `pyVLMP-1.0.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.583156 pyVLMP-1.0.5/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-24 18:33:04.000000 pyVLMP-1.0.5/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 14:59:17.000000 pyVLMP-1.0.5/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-14 15:11:41.583156 pyVLMP-1.0.5/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       69 2023-01-24 18:33:04.000000 pyVLMP-1.0.5/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.563157 pyVLMP-1.0.5/VLMP/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    34280 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/VLMP.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1641 2023-05-09 15:57:22.000000 pyVLMP-1.0.5/VLMP/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6969 2023-05-03 16:45:43.000000 pyVLMP-1.0.5/VLMP/__main__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.563157 pyVLMP-1.0.5/VLMP/components/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.563157 pyVLMP-1.0.5/VLMP/components/globals/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1079 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/globals/NVT.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3340 2023-05-03 16:00:59.000000 pyVLMP-1.0.5/VLMP/components/globals/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.567157 pyVLMP-1.0.5/VLMP/components/integrators/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1657 2023-05-02 14:06:34.000000 pyVLMP-1.0.5/VLMP/components/integrators/BBK.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1630 2023-05-02 14:06:57.000000 pyVLMP-1.0.5/VLMP/components/integrators/EulerMaruyama.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1668 2023-05-02 14:06:52.000000 pyVLMP-1.0.5/VLMP/components/integrators/EulerMaruyamaRigidBody.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1706 2023-05-02 14:07:04.000000 pyVLMP-1.0.5/VLMP/components/integrators/GJF.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4134 2023-05-03 16:01:12.000000 pyVLMP-1.0.5/VLMP/components/integrators/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.567157 pyVLMP-1.0.5/VLMP/components/modelExtensions/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5853 2023-05-03 16:01:25.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1685 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForce.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2071 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1891 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2074 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1866 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2446 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2198 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.567157 pyVLMP-1.0.5/VLMP/components/modelOperations/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6422 2023-05-03 16:01:39.000000 pyVLMP-1.0.5/VLMP/components/modelOperations/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1239 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/modelOperations/setCenterOfMassPosition.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.571157 pyVLMP-1.0.5/VLMP/components/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    27461 2023-04-28 14:56:31.000000 pyVLMP-1.0.5/VLMP/components/models/CORONAVIRUS.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    19017 2023-05-14 15:07:15.000000 pyVLMP-1.0.5/VLMP/components/models/HELIX.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2420 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/KB.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35619 2023-04-28 14:55:03.000000 pyVLMP-1.0.5/VLMP/components/models/MADna.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2699 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/SBCG.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2450 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/SOP.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4218 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/WLC.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6169 2023-05-03 16:01:56.000000 pyVLMP-1.0.5/VLMP/components/models/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.571157 pyVLMP-1.0.5/VLMP/components/models/data/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3895 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/data/CORONAVIRUS.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    38242 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/models/data/MADna.json
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.575157 pyVLMP-1.0.5/VLMP/components/simulationSteps/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7439 2023-05-03 16:02:11.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1495 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/centerOfMassMeasurement.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1802 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/heightMeasurement.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1379 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/info.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1697 2023-05-07 17:55:49.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/patchPolymersMeasurement.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1821 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/savePatchyParticlesState.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1740 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/simulationSteps/saveState.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.575157 pyVLMP-1.0.5/VLMP/components/system/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3054 2023-05-03 15:59:27.000000 pyVLMP-1.0.5/VLMP/components/system/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2218 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/system/backup.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1102 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/system/simulationName.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.579156 pyVLMP-1.0.5/VLMP/components/types/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6496 2023-05-03 16:02:33.000000 pyVLMP-1.0.5/VLMP/components/types/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      992 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/types/basic.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      768 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/types/none.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.579156 pyVLMP-1.0.5/VLMP/components/units/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      891 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/units/KcalMol_A.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3921 2023-05-03 16:03:07.000000 pyVLMP-1.0.5/VLMP/components/units/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      887 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/components/units/none.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.579156 pyVLMP-1.0.5/VLMP/experiments/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15172 2023-05-02 13:54:57.000000 pyVLMP-1.0.5/VLMP/experiments/SurfaceUmbrellaSampling.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/experiments/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.579156 pyVLMP-1.0.5/VLMP/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.5/VLMP/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1784 2023-04-28 14:57:38.000000 pyVLMP-1.0.5/VLMP/utils/bounds.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3529 2023-05-10 16:03:24.000000 pyVLMP-1.0.5/VLMP/utils/utils.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:11:41.583156 pyVLMP-1.0.5/pyVLMP.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-14 15:11:41.000000 pyVLMP-1.0.5/pyVLMP.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2295 2023-05-14 15:11:41.000000 pyVLMP-1.0.5/pyVLMP.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-14 15:11:41.000000 pyVLMP-1.0.5/pyVLMP.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       41 2023-05-14 15:11:41.000000 pyVLMP-1.0.5/pyVLMP.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-14 15:11:41.000000 pyVLMP-1.0.5/pyVLMP.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      756 2023-05-14 15:11:07.000000 pyVLMP-1.0.5/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-14 15:11:41.583156 pyVLMP-1.0.5/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      152 2023-05-03 15:40:43.000000 pyVLMP-1.0.5/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-24 18:33:04.000000 pyVLMP-1.0.6/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 14:59:17.000000 pyVLMP-1.0.6/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       69 2023-01-24 18:33:04.000000 pyVLMP-1.0.6/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    34280 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/VLMP.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1641 2023-05-09 15:57:22.000000 pyVLMP-1.0.6/VLMP/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6969 2023-05-03 16:45:43.000000 pyVLMP-1.0.6/VLMP/__main__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/components/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/components/globals/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1079 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/globals/NVT.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3340 2023-05-03 16:00:59.000000 pyVLMP-1.0.6/VLMP/components/globals/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/components/integrators/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1657 2023-05-02 14:06:34.000000 pyVLMP-1.0.6/VLMP/components/integrators/BBK.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1630 2023-05-02 14:06:57.000000 pyVLMP-1.0.6/VLMP/components/integrators/EulerMaruyama.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1668 2023-05-02 14:06:52.000000 pyVLMP-1.0.6/VLMP/components/integrators/EulerMaruyamaRigidBody.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1706 2023-05-02 14:07:04.000000 pyVLMP-1.0.6/VLMP/components/integrators/GJF.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4134 2023-05-03 16:01:12.000000 pyVLMP-1.0.6/VLMP/components/integrators/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/components/modelExtensions/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5853 2023-05-03 16:01:25.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1685 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForce.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2071 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1891 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2074 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1866 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2446 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2198 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.095770 pyVLMP-1.0.6/VLMP/components/modelOperations/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6422 2023-05-03 16:01:39.000000 pyVLMP-1.0.6/VLMP/components/modelOperations/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1239 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/modelOperations/setCenterOfMassPosition.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    27461 2023-04-28 14:56:31.000000 pyVLMP-1.0.6/VLMP/components/models/CORONAVIRUS.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    19503 2023-05-14 15:23:58.000000 pyVLMP-1.0.6/VLMP/components/models/HELIX.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2420 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/KB.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35619 2023-04-28 14:55:03.000000 pyVLMP-1.0.6/VLMP/components/models/MADna.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2699 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/SBCG.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2450 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/SOP.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4218 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/WLC.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6169 2023-05-03 16:01:56.000000 pyVLMP-1.0.6/VLMP/components/models/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/models/data/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3895 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/data/CORONAVIRUS.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    38242 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/models/data/MADna.json
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/simulationSteps/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7439 2023-05-03 16:02:11.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1495 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/centerOfMassMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1802 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/heightMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1379 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/info.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1697 2023-05-07 17:55:49.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/patchPolymersMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1821 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/savePatchyParticlesState.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1740 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/simulationSteps/saveState.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/system/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3054 2023-05-03 15:59:27.000000 pyVLMP-1.0.6/VLMP/components/system/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2218 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/system/backup.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1102 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/system/simulationName.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/types/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6496 2023-05-03 16:02:33.000000 pyVLMP-1.0.6/VLMP/components/types/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      992 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/types/basic.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      768 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/types/none.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/components/units/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      891 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/units/KcalMol_A.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3921 2023-05-03 16:03:07.000000 pyVLMP-1.0.6/VLMP/components/units/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      887 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/components/units/none.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/experiments/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15172 2023-05-02 13:54:57.000000 pyVLMP-1.0.6/VLMP/experiments/SurfaceUmbrellaSampling.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/experiments/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/VLMP/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.6/VLMP/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1784 2023-04-28 14:57:38.000000 pyVLMP-1.0.6/VLMP/utils/bounds.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3529 2023-05-10 16:03:24.000000 pyVLMP-1.0.6/VLMP/utils/utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/pyVLMP.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-14 15:25:33.000000 pyVLMP-1.0.6/pyVLMP.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2295 2023-05-14 15:25:33.000000 pyVLMP-1.0.6/pyVLMP.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-14 15:25:33.000000 pyVLMP-1.0.6/pyVLMP.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       41 2023-05-14 15:25:33.000000 pyVLMP-1.0.6/pyVLMP.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-14 15:25:33.000000 pyVLMP-1.0.6/pyVLMP.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      756 2023-05-14 15:21:12.000000 pyVLMP-1.0.6/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-14 15:25:33.099770 pyVLMP-1.0.6/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      152 2023-05-03 15:40:43.000000 pyVLMP-1.0.6/setup.py
```

### Comparing `pyVLMP-1.0.5/LICENSE` & `pyVLMP-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/PKG-INFO` & `pyVLMP-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVLMP
-Version: 1.0.5
+Version: 1.0.6
 Summary: Virtual Laboratory for the simulation of Macromolecular Properties
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyVLMP-1.0.5/VLMP/VLMP.py` & `pyVLMP-1.0.6/VLMP/VLMP.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/__init__.py` & `pyVLMP-1.0.6/VLMP/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/__main__.py` & `pyVLMP-1.0.6/VLMP/__main__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/globals/NVT.py` & `pyVLMP-1.0.6/VLMP/components/globals/NVT.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/globals/__init__.py` & `pyVLMP-1.0.6/VLMP/components/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/integrators/BBK.py` & `pyVLMP-1.0.6/VLMP/components/integrators/BBK.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/integrators/EulerMaruyama.py` & `pyVLMP-1.0.6/VLMP/components/integrators/EulerMaruyama.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/integrators/EulerMaruyamaRigidBody.py` & `pyVLMP-1.0.6/VLMP/components/integrators/EulerMaruyamaRigidBody.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/integrators/GJF.py` & `pyVLMP-1.0.6/VLMP/components/integrators/GJF.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/integrators/__init__.py` & `pyVLMP-1.0.6/VLMP/components/integrators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/__init__.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForce.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForce.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py` & `pyVLMP-1.0.6/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelOperations/__init__.py` & `pyVLMP-1.0.6/VLMP/components/modelOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/modelOperations/setCenterOfMassPosition.py` & `pyVLMP-1.0.6/VLMP/components/modelOperations/setCenterOfMassPosition.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/CORONAVIRUS.py` & `pyVLMP-1.0.6/VLMP/components/models/CORONAVIRUS.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/HELIX.py` & `pyVLMP-1.0.6/VLMP/components/models/HELIX.py`

 * *Files 8% similar despite different names*

```diff
@@ -198,14 +198,15 @@
                          availableParameters = {"mode","init",
                                                 "nMonomers","box","bounds",
                                                 "monomerRadius","patchRadius",
                                                 "epsilon_mm",
                                                 "Eb","rc",
                                                 "theta0","phi0",
                                                 "varDst","varTheta","varPhi",
+                                                "stiffnessFactor",
                                                 "Es",
                                                 "beta0",
                                                 "El","Sl",
                                                 "plateTop","plateBottom"},
                          requiredParameters  = {"nMonomers",
                                                 "epsilon_mm",
                                                 "Eb","rc",
@@ -260,14 +261,16 @@
         self.Eb = params["Eb"]
         self.rc = params["rc"]
 
         varDst   = params["varDst"]
         varTheta = params["varTheta"]
         varPhi   = params["varPhi"]
 
+        stiffnessFactor = params.get("stiffnessFactor",1.0)
+
         self.theta0 = params["theta0"]
         self.phi0   = params["phi0"]
 
         if self.mode=="surface":
             #Check parameters Es,beta0,El,Sl are present in params
             surfaceParams = ["Es","beta0","El","Sl"]
             for sPar in surfaceParams:
@@ -286,14 +289,22 @@
         self.Ka = self.__computeKangle(varTheta,abs(self.Eb))
         self.Kd = self.__computeKangle(varPhi,abs(self.Eb))
 
         self.logger.info(f"[HELIX] K bond computed {self.Kb} for variance {varDst}")
         self.logger.info(f"[HELIX] K theta computed {self.Ka} for variance {varTheta}")
         self.logger.info(f"[HELIX] K phi computed {self.Kd} for variance {varPhi}")
 
+        if stiffnessFactor != 1.0:
+            self.logger.info(f"[HELIX] Applying stiffness factor {stiffnessFactor}")
+            self.Ka*=stiffnessFactor
+            self.Kd*=stiffnessFactor
+
+            self.logger.info(f"[HELIX] K theta after stiffness factor {self.Ka}")
+            self.logger.info(f"[HELIX] K phi after stiffness factor {self.Kd}")
+
         if self.Kb < 0 or self.Ka < 0 or self.Kd < 0:
             self.logger.error(f"[HELIX] Negative spring constant: Kb {self.Kb} Ka {self.Ka} Kd {self.Kd}")
             raise Exception("Negative spring constant")
 
         ##############################################
 
         self.logger.info(f"[HELIX] Generating HELIX model with {self.nMonomers} monomers")
```

### Comparing `pyVLMP-1.0.5/VLMP/components/models/KB.py` & `pyVLMP-1.0.6/VLMP/components/models/KB.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/MADna.py` & `pyVLMP-1.0.6/VLMP/components/models/MADna.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/SBCG.py` & `pyVLMP-1.0.6/VLMP/components/models/SBCG.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/SOP.py` & `pyVLMP-1.0.6/VLMP/components/models/SOP.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/WLC.py` & `pyVLMP-1.0.6/VLMP/components/models/WLC.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/__init__.py` & `pyVLMP-1.0.6/VLMP/components/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/data/CORONAVIRUS.json` & `pyVLMP-1.0.6/VLMP/components/models/data/CORONAVIRUS.json`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/models/data/MADna.json` & `pyVLMP-1.0.6/VLMP/components/models/data/MADna.json`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/__init__.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/centerOfMassMeasurement.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/centerOfMassMeasurement.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/heightMeasurement.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/heightMeasurement.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/info.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/info.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/patchPolymersMeasurement.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/patchPolymersMeasurement.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/savePatchyParticlesState.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/savePatchyParticlesState.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/simulationSteps/saveState.py` & `pyVLMP-1.0.6/VLMP/components/simulationSteps/saveState.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/system/__init__.py` & `pyVLMP-1.0.6/VLMP/components/system/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/system/backup.py` & `pyVLMP-1.0.6/VLMP/components/system/backup.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/system/simulationName.py` & `pyVLMP-1.0.6/VLMP/components/system/simulationName.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/types/__init__.py` & `pyVLMP-1.0.6/VLMP/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/types/basic.py` & `pyVLMP-1.0.6/VLMP/components/types/basic.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/types/none.py` & `pyVLMP-1.0.6/VLMP/components/types/none.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/units/KcalMol_A.py` & `pyVLMP-1.0.6/VLMP/components/units/KcalMol_A.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/units/__init__.py` & `pyVLMP-1.0.6/VLMP/components/units/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/components/units/none.py` & `pyVLMP-1.0.6/VLMP/components/units/none.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/experiments/SurfaceUmbrellaSampling.py` & `pyVLMP-1.0.6/VLMP/experiments/SurfaceUmbrellaSampling.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/utils/bounds.py` & `pyVLMP-1.0.6/VLMP/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/VLMP/utils/utils.py` & `pyVLMP-1.0.6/VLMP/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/pyVLMP.egg-info/PKG-INFO` & `pyVLMP-1.0.6/pyVLMP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVLMP
-Version: 1.0.5
+Version: 1.0.6
 Summary: Virtual Laboratory for the simulation of Macromolecular Properties
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyVLMP-1.0.5/pyVLMP.egg-info/SOURCES.txt` & `pyVLMP-1.0.6/pyVLMP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.5/pyproject.toml` & `pyVLMP-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="pyVLMP"
-version="1.0.5"
+version="1.0.6"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "Virtual Laboratory for the simulation of Macromolecular Properties"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

