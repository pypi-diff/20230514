# Comparing `tmp/compas_timber-0.2.8.tar.gz` & `tmp/compas_timber-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_timber-0.2.8.tar", last modified: Fri May 12 19:18:37 2023, max compression
+gzip compressed data, was "compas_timber-0.2.9.tar", last modified: Fri May 12 19:50:45 2023, max compression
```

## Comparing `compas_timber-0.2.8.tar` & `compas_timber-0.2.9.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/
--rw-rw-rw-   0        0        0     1028 2023-05-12 19:14:40.000000 compas_timber-0.2.8/AUTHORS.md
--rw-rw-rw-   0        0        0      970 2023-05-12 19:14:40.000000 compas_timber-0.2.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1108 2023-05-12 19:14:40.000000 compas_timber-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      458 2023-05-12 19:14:40.000000 compas_timber-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3745 2023-05-12 19:18:37.282470 compas_timber-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2602 2023-05-12 19:14:40.000000 compas_timber-0.2.8/README.md
--rw-rw-rw-   0        0        0      717 2023-05-12 19:14:40.000000 compas_timber-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0        7 2023-05-12 19:14:40.000000 compas_timber-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0      227 2023-05-12 19:18:37.282470 compas_timber-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2071 2023-05-12 19:14:40.000000 compas_timber-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.188727 compas_timber-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.204354 compas_timber-0.2.8/src/compas_timber/
--rw-rw-rw-   0        0        0      498 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/__init__.py
--rw-rw-rw-   0        0        0      630 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.204354 compas_timber-0.2.8/src/compas_timber/assembly/
--rw-rw-rw-   0        0        0      199 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/assembly/README.md
--rw-rw-rw-   0        0        0      572 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/assembly/__init__.py
--rw-rw-rw-   0        0        0     5999 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/assembly/assembly.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/connections/
--rw-rw-rw-   0        0        0      154 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/README.md
--rw-rw-rw-   0        0        0     1298 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/__init__.py
--rw-rw-rw-   0        0        0     4608 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/joint.py
--rw-rw-rw-   0        0        0     4285 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/l_butt.py
--rw-rw-rw-   0        0        0     5161 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/l_miter.py
--rw-rw-rw-   0        0        0     8588 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/solver.py
--rw-rw-rw-   0        0        0     3870 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/connections/t_butt.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/
--rw-rw-rw-   0        0        0      207 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/components/
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/
--rw-rw-rw-   0        0        0     2268 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/code.py
--rw-rw-rw-   0        0        0      484 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/icon.png
--rw-rw-rw-   0        0        0     1554 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/
--rw-rw-rw-   0        0        0     3561 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/code.py
--rw-rw-rw-   0        0        0      991 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/icon.png
--rw-rw-rw-   0        0        0      742 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/
--rw-rw-rw-   0        0        0      309 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/code.py
--rw-rw-rw-   0        0        0     2049 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/icon.png
--rw-rw-rw-   0        0        0      944 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.219984 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/
--rw-rw-rw-   0        0        0      862 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/code.py
--rw-rw-rw-   0        0        0      828 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/icon.png
--rw-rw-rw-   0        0        0     1226 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/
--rw-rw-rw-   0        0        0     1975 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/code.py
--rw-rw-rw-   0        0        0      890 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/icon.png
--rw-rw-rw-   0        0        0     1470 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/
--rw-rw-rw-   0        0        0      832 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/code.py
--rw-rw-rw-   0        0        0      896 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/icon.png
--rw-rw-rw-   0        0        0      930 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/
--rw-rw-rw-   0        0        0     3148 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/code.py
--rw-rw-rw-   0        0        0      895 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/icon.png
--rw-rw-rw-   0        0        0     1717 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/
--rw-rw-rw-   0        0        0      728 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/code.py
--rw-rw-rw-   0        0        0      895 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/icon.png
--rw-rw-rw-   0        0        0     1153 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/
--rw-rw-rw-   0        0        0     2123 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/code.py
--rw-rw-rw-   0        0        0     1197 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/icon.png
--rw-rw-rw-   0        0        0     1594 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/
--rw-rw-rw-   0        0        0     2469 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/code.py
--rw-rw-rw-   0        0        0      748 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/icon.png
--rw-rw-rw-   0        0        0     1435 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/
--rw-rw-rw-   0        0        0     1112 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/code.py
--rw-rw-rw-   0        0        0     1360 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/icon.png
--rw-rw-rw-   0        0        0     1298 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/
--rw-rw-rw-   0        0        0     3366 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/code.py
--rw-rw-rw-   0        0        0     1770 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/icon.png
--rw-rw-rw-   0        0        0     1725 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/
--rw-rw-rw-   0        0        0     3471 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/code.py
--rw-rw-rw-   0        0        0      691 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/icon.png
--rw-rw-rw-   0        0        0     2097 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.235595 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/
--rw-rw-rw-   0        0        0     1023 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/code.py
--rw-rw-rw-   0        0        0      879 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/icon.png
--rw-rw-rw-   0        0        0     1091 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/
--rw-rw-rw-   0        0        0     1018 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/code.py
--rw-rw-rw-   0        0        0      828 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/icon.png
--rw-rw-rw-   0        0        0      979 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/
--rw-rw-rw-   0        0        0      656 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/code.py
--rw-rw-rw-   0        0        0      945 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/icon.png
--rw-rw-rw-   0        0        0     1007 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/
--rw-rw-rw-   0        0        0     1760 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/code.py
--rw-rw-rw-   0        0        0     1836 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/icon.png
--rw-rw-rw-   0        0        0     1008 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/
--rw-rw-rw-   0        0        0     1700 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/code.py
--rw-rw-rw-   0        0        0     1441 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/icon.png
--rw-rw-rw-   0        0        0      933 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/
--rw-rw-rw-   0        0        0      600 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/code.py
--rw-rw-rw-   0        0        0      841 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/icon.png
--rw-rw-rw-   0        0        0     1204 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/
--rw-rw-rw-   0        0        0     1757 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/code.py
--rw-rw-rw-   0        0        0     1844 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/icon.png
--rw-rw-rw-   0        0        0     1008 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/
--rw-rw-rw-   0        0        0      618 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/code.py
--rw-rw-rw-   0        0        0     1083 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/icon.png
--rw-rw-rw-   0        0        0      716 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/
--rw-rw-rw-   0        0        0     1370 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/code.py
--rw-rw-rw-   0        0        0      806 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/icon.png
--rw-rw-rw-   0        0        0      613 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.251218 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/
--rw-rw-rw-   0        0        0      841 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/code.py
--rw-rw-rw-   0        0        0     1362 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/icon.png
--rw-rw-rw-   0        0        0      601 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.266845 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/
--rw-rw-rw-   0        0        0      246 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/code.py
--rw-rw-rw-   0        0        0      952 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/icon.png
--rw-rw-rw-   0        0        0      699 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/metadata.json
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.266845 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/
--rw-rw-rw-   0        0        0     1158 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/code.py
--rw-rw-rw-   0        0        0      801 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/icon.png
--rw-rw-rw-   0        0        0      586 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/metadata.json
--rw-rw-rw-   0        0        0      196 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/README.md
--rw-rw-rw-   0        0        0      134 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/
--rw-rw-rw-   0        0        0     2338 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Assembly.ghuser
--rw-rw-rw-   0        0        0     2961 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Check.ghuser
--rw-rw-rw-   0        0        0     2132 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Create.ghuser
--rw-rw-rw-   0        0        0     2159 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Delete.ghuser
--rw-rw-rw-   0        0        0     2700 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Get.ghuser
--rw-rw-rw-   0        0        0     2134 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Get_Custom.ghuser
--rw-rw-rw-   0        0        0     2864 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Set.ghuser
--rw-rw-rw-   0        0        0     2139 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Set_Custom.ghuser
--rw-rw-rw-   0        0        0     3187 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_AutomaticJoints.ghuser
--rw-rw-rw-   0        0        0     2860 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Bake_BoxMap.ghuser
--rw-rw-rw-   0        0        0     2829 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_BeamDecompose.ghuser
--rw-rw-rw-   0        0        0     3196 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Beam_fromCurve.ghuser
--rw-rw-rw-   0        0        0     2950 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Beam_fromCurveGuid.ghuser
--rw-rw-rw-   0        0        0     2270 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_FeatureBrepSubtraction.ghuser
--rw-rw-rw-   0        0        0     2148 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_Feature_Trim.ghuser
--rw-rw-rw-   0        0        0     2192 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_FindByGuid.ghuser
--rw-rw-rw-   0        0        0     2444 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_JointDef_LButt.ghuser
--rw-rw-rw-   0        0        0     2237 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_JointDef_LMiter.ghuser
--rw-rw-rw-   0        0        0     2119 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_JointDef_Rule.ghuser
--rw-rw-rw-   0        0        0     2467 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_JointDef_TButt.ghuser
--rw-rw-rw-   0        0        0     1554 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_AttributeName.ghuser
--rw-rw-rw-   0        0        0     1397 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_JointType.ghuser
--rw-rw-rw-   0        0        0     2173 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_ShowAssembly.ghuser
--rw-rw-rw-   0        0        0     1989 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamFrame.ghuser
--rw-rw-rw-   0        0        0     2456 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamIndex.ghuser
--rw-rw-rw-   0        0        0     1880 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamShape.ghuser
--rw-rw-rw-   0        0        0     2025 2023-05-12 19:18:21.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_ShowJointTypes.ghuser
--rw-rw-rw-   0        0        0     2458 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/components/install.py
--rw-rw-rw-   0        0        0      903 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/ghcomponent_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/src/compas_timber/ghpython/ghuser_manual/
--rw-rw-rw-   0        0        0     1554 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_AttributeName.ghuser
--rw-rw-rw-   0        0        0     1397 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_JointType.ghuser
--rw-rw-rw-   0        0        0     5034 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/rhino_object_name_attributes.py
--rw-rw-rw-   0        0        0     6655 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/ghpython/workflow.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/src/compas_timber/parts/
--rw-rw-rw-   0        0        0      155 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/parts/README.md
--rw-rw-rw-   0        0        0      796 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/parts/__init__.py
--rw-rw-rw-   0        0        0    20849 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/parts/beam.py
--rw-rw-rw-   0        0        0       51 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/parts/exceptions.py
--rw-rw-rw-   0        0        0     4784 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/parts/features.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/src/compas_timber/rhino/
--rw-rw-rw-   0        0        0     1925 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/rhino/__init__.py
--rw-rw-rw-   0        0        0      776 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/rhino/install.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.282470 compas_timber-0.2.8/src/compas_timber/utils/
--rw-rw-rw-   0        0        0       26 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/README.md
--rw-rw-rw-   0        0        0      306 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/__init__.py
--rw-rw-rw-   0        0        0     4939 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/compas_extra.py
--rw-rw-rw-   0        0        0     1408 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/helpers.py
--rw-rw-rw-   0        0        0     1884 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/r_tree.py
--rw-rw-rw-   0        0        0     3877 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/rhino_compas.py
--rw-rw-rw-   0        0        0      847 2023-05-12 19:14:40.000000 compas_timber-0.2.8/src/compas_timber/utils/rhinoscript.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:37.204354 compas_timber-0.2.8/src/compas_timber.egg-info/
--rw-rw-rw-   0        0        0     3745 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8744 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 19:18:37.000000 compas_timber-0.2.8/src/compas_timber.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.103425 compas_timber-0.2.9/
+-rw-rw-rw-   0        0        0     1028 2023-05-12 19:47:14.000000 compas_timber-0.2.9/AUTHORS.md
+-rw-rw-rw-   0        0        0     1040 2023-05-12 19:47:14.000000 compas_timber-0.2.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1108 2023-05-12 19:47:14.000000 compas_timber-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      458 2023-05-12 19:47:14.000000 compas_timber-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3786 2023-05-12 19:50:45.103425 compas_timber-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2602 2023-05-12 19:47:14.000000 compas_timber-0.2.9/README.md
+-rw-rw-rw-   0        0        0      717 2023-05-12 19:47:15.000000 compas_timber-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0        7 2023-05-12 19:47:15.000000 compas_timber-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0      227 2023-05-12 19:50:45.103425 compas_timber-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2123 2023-05-12 19:47:15.000000 compas_timber-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.025299 compas_timber-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.025299 compas_timber-0.2.9/src/compas_timber/
+-rw-rw-rw-   0        0        0      498 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/__init__.py
+-rw-rw-rw-   0        0        0      630 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/assembly/
+-rw-rw-rw-   0        0        0      199 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/assembly/README.md
+-rw-rw-rw-   0        0        0      572 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/assembly/__init__.py
+-rw-rw-rw-   0        0        0     5999 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/assembly/assembly.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/connections/
+-rw-rw-rw-   0        0        0      154 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/README.md
+-rw-rw-rw-   0        0        0     1298 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/__init__.py
+-rw-rw-rw-   0        0        0     4608 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/joint.py
+-rw-rw-rw-   0        0        0     4285 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/l_butt.py
+-rw-rw-rw-   0        0        0     5161 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/l_miter.py
+-rw-rw-rw-   0        0        0     8588 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/solver.py
+-rw-rw-rw-   0        0        0     3870 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/connections/t_butt.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/
+-rw-rw-rw-   0        0        0      207 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/components/
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/
+-rw-rw-rw-   0        0        0     2268 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/code.py
+-rw-rw-rw-   0        0        0      484 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/icon.png
+-rw-rw-rw-   0        0        0     1554 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/
+-rw-rw-rw-   0        0        0     3561 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/code.py
+-rw-rw-rw-   0        0        0      991 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/icon.png
+-rw-rw-rw-   0        0        0      742 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/
+-rw-rw-rw-   0        0        0      309 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/code.py
+-rw-rw-rw-   0        0        0     2049 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/icon.png
+-rw-rw-rw-   0        0        0      944 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.040924 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/
+-rw-rw-rw-   0        0        0      862 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/code.py
+-rw-rw-rw-   0        0        0      828 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/icon.png
+-rw-rw-rw-   0        0        0     1226 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/
+-rw-rw-rw-   0        0        0     1975 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/code.py
+-rw-rw-rw-   0        0        0      890 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/icon.png
+-rw-rw-rw-   0        0        0     1470 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/
+-rw-rw-rw-   0        0        0      832 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/code.py
+-rw-rw-rw-   0        0        0      896 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/icon.png
+-rw-rw-rw-   0        0        0      930 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/
+-rw-rw-rw-   0        0        0     3148 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/code.py
+-rw-rw-rw-   0        0        0      895 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/icon.png
+-rw-rw-rw-   0        0        0     1717 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/
+-rw-rw-rw-   0        0        0      728 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/code.py
+-rw-rw-rw-   0        0        0      895 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/icon.png
+-rw-rw-rw-   0        0        0     1153 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/
+-rw-rw-rw-   0        0        0     2123 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/code.py
+-rw-rw-rw-   0        0        0     1197 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/icon.png
+-rw-rw-rw-   0        0        0     1594 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/
+-rw-rw-rw-   0        0        0     2469 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/code.py
+-rw-rw-rw-   0        0        0      748 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/icon.png
+-rw-rw-rw-   0        0        0     1435 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/
+-rw-rw-rw-   0        0        0     1112 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/code.py
+-rw-rw-rw-   0        0        0     1360 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/icon.png
+-rw-rw-rw-   0        0        0     1298 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/
+-rw-rw-rw-   0        0        0     3366 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/code.py
+-rw-rw-rw-   0        0        0     1770 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/icon.png
+-rw-rw-rw-   0        0        0     1725 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/
+-rw-rw-rw-   0        0        0     3471 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/code.py
+-rw-rw-rw-   0        0        0      691 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/icon.png
+-rw-rw-rw-   0        0        0     2097 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/
+-rw-rw-rw-   0        0        0     1023 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/code.py
+-rw-rw-rw-   0        0        0      879 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/icon.png
+-rw-rw-rw-   0        0        0     1091 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.056549 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/
+-rw-rw-rw-   0        0        0     1018 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/code.py
+-rw-rw-rw-   0        0        0      828 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/icon.png
+-rw-rw-rw-   0        0        0      979 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/
+-rw-rw-rw-   0        0        0      656 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/code.py
+-rw-rw-rw-   0        0        0      945 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/icon.png
+-rw-rw-rw-   0        0        0     1007 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/
+-rw-rw-rw-   0        0        0     1760 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/code.py
+-rw-rw-rw-   0        0        0     1836 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/icon.png
+-rw-rw-rw-   0        0        0     1008 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/
+-rw-rw-rw-   0        0        0     1700 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/code.py
+-rw-rw-rw-   0        0        0     1441 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/icon.png
+-rw-rw-rw-   0        0        0      933 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/
+-rw-rw-rw-   0        0        0      600 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/code.py
+-rw-rw-rw-   0        0        0      841 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/icon.png
+-rw-rw-rw-   0        0        0     1204 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/
+-rw-rw-rw-   0        0        0     1757 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/code.py
+-rw-rw-rw-   0        0        0     1844 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/icon.png
+-rw-rw-rw-   0        0        0     1008 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/
+-rw-rw-rw-   0        0        0      618 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/code.py
+-rw-rw-rw-   0        0        0     1083 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/icon.png
+-rw-rw-rw-   0        0        0      716 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/
+-rw-rw-rw-   0        0        0     1370 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/code.py
+-rw-rw-rw-   0        0        0      806 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/icon.png
+-rw-rw-rw-   0        0        0      613 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/
+-rw-rw-rw-   0        0        0      841 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/code.py
+-rw-rw-rw-   0        0        0     1362 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/icon.png
+-rw-rw-rw-   0        0        0      601 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/
+-rw-rw-rw-   0        0        0      246 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/code.py
+-rw-rw-rw-   0        0        0      952 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/icon.png
+-rw-rw-rw-   0        0        0      699 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/metadata.json
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.072175 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/
+-rw-rw-rw-   0        0        0     1158 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/code.py
+-rw-rw-rw-   0        0        0      801 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/icon.png
+-rw-rw-rw-   0        0        0      586 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/metadata.json
+-rw-rw-rw-   0        0        0      196 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/README.md
+-rw-rw-rw-   0        0        0      134 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.087798 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/
+-rw-rw-rw-   0        0        0     2333 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Assembly.ghuser
+-rw-rw-rw-   0        0        0     2960 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Check.ghuser
+-rw-rw-rw-   0        0        0     2129 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Create.ghuser
+-rw-rw-rw-   0        0        0     2158 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Delete.ghuser
+-rw-rw-rw-   0        0        0     2703 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Get.ghuser
+-rw-rw-rw-   0        0        0     2142 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Get_Custom.ghuser
+-rw-rw-rw-   0        0        0     2865 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Set.ghuser
+-rw-rw-rw-   0        0        0     2139 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Attributes_Set_Custom.ghuser
+-rw-rw-rw-   0        0        0     3194 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_AutomaticJoints.ghuser
+-rw-rw-rw-   0        0        0     2860 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Bake_BoxMap.ghuser
+-rw-rw-rw-   0        0        0     2824 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_BeamDecompose.ghuser
+-rw-rw-rw-   0        0        0     3194 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Beam_fromCurve.ghuser
+-rw-rw-rw-   0        0        0     2938 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Beam_fromCurveGuid.ghuser
+-rw-rw-rw-   0        0        0     2273 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_FeatureBrepSubtraction.ghuser
+-rw-rw-rw-   0        0        0     2145 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_Feature_Trim.ghuser
+-rw-rw-rw-   0        0        0     2202 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_FindByGuid.ghuser
+-rw-rw-rw-   0        0        0     2460 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_JointDef_LButt.ghuser
+-rw-rw-rw-   0        0        0     2237 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_JointDef_LMiter.ghuser
+-rw-rw-rw-   0        0        0     2115 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_JointDef_Rule.ghuser
+-rw-rw-rw-   0        0        0     2465 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_JointDef_TButt.ghuser
+-rw-rw-rw-   0        0        0     1554 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_AttributeName.ghuser
+-rw-rw-rw-   0        0        0     1397 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_JointType.ghuser
+-rw-rw-rw-   0        0        0     2176 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_ShowAssembly.ghuser
+-rw-rw-rw-   0        0        0     1982 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamFrame.ghuser
+-rw-rw-rw-   0        0        0     2455 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamIndex.ghuser
+-rw-rw-rw-   0        0        0     1884 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_ShowBeamShape.ghuser
+-rw-rw-rw-   0        0        0     2019 2023-05-12 19:50:33.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_ShowJointTypes.ghuser
+-rw-rw-rw-   0        0        0     2458 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/components/install.py
+-rw-rw-rw-   0        0        0      903 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/ghcomponent_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.087798 compas_timber-0.2.9/src/compas_timber/ghpython/ghuser_manual/
+-rw-rw-rw-   0        0        0     1554 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_AttributeName.ghuser
+-rw-rw-rw-   0        0        0     1397 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_JointType.ghuser
+-rw-rw-rw-   0        0        0     5034 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/rhino_object_name_attributes.py
+-rw-rw-rw-   0        0        0     6655 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/ghpython/workflow.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.087798 compas_timber-0.2.9/src/compas_timber/parts/
+-rw-rw-rw-   0        0        0      155 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/parts/README.md
+-rw-rw-rw-   0        0        0      796 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/parts/__init__.py
+-rw-rw-rw-   0        0        0    20849 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/parts/beam.py
+-rw-rw-rw-   0        0        0       51 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/parts/exceptions.py
+-rw-rw-rw-   0        0        0     4784 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/parts/features.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.087798 compas_timber-0.2.9/src/compas_timber/rhino/
+-rw-rw-rw-   0        0        0     1925 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/rhino/__init__.py
+-rw-rw-rw-   0        0        0      776 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/rhino/install.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.103425 compas_timber-0.2.9/src/compas_timber/utils/
+-rw-rw-rw-   0        0        0       26 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/README.md
+-rw-rw-rw-   0        0        0      306 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/__init__.py
+-rw-rw-rw-   0        0        0     4939 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/compas_extra.py
+-rw-rw-rw-   0        0        0     1408 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/helpers.py
+-rw-rw-rw-   0        0        0     1884 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/r_tree.py
+-rw-rw-rw-   0        0        0     3877 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/rhino_compas.py
+-rw-rw-rw-   0        0        0      847 2023-05-12 19:47:15.000000 compas_timber-0.2.9/src/compas_timber/utils/rhinoscript.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:50:45.025299 compas_timber-0.2.9/src/compas_timber.egg-info/
+-rw-rw-rw-   0        0        0     3786 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8744 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 19:50:44.000000 compas_timber-0.2.9/src/compas_timber.egg-info/top_level.txt
```

### Comparing `compas_timber-0.2.8/AUTHORS.md` & `compas_timber-0.2.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/CHANGELOG.md` & `compas_timber-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.9] 2023-05-12
+
+### Added
+
+### Changed
+
+### Removed
+
+
 ## [0.2.8] 2023-05-12
 
 ### Added
 
 ### Changed
 
 ### Removed
```

### Comparing `compas_timber-0.2.8/LICENSE` & `compas_timber-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/PKG-INFO` & `compas_timber-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_timber
-Version: 0.2.8
+Version: 0.2.9
 Summary: COMPAS package for modeling, designing and fabricating timber assemblies.
 Home-page: https://github.com/gramaziokohler/compas_timber
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # compas_timber
 
 [![Github Actions Build Status](https://github.com/gramaziokohler/compas_timber/workflows/build/badge.svg)](https://github.com/gramaziokohler/compas_timber/actions)
 [![License](https://img.shields.io/github/license/gramaziokohler/compas_timber.svg)](https://pypi.python.org/pypi/compas_timber)
```

### Comparing `compas_timber-0.2.8/README.md` & `compas_timber-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/pyproject.toml` & `compas_timber-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/setup.py` & `compas_timber-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     version=about["__version__"],
     license=about["__license__"],
     description=about["__description__"],
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     long_description=long_description,
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: POSIX",
```

### Comparing `compas_timber-0.2.8/src/compas_timber/__version__.py` & `compas_timber-0.2.9/src/compas_timber/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 __title__ = "compas_timber"
 __description__ = "COMPAS package for modeling, designing and fabricating timber assemblies."
 __url__ = "https://github.com/gramaziokohler/compas_timber"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 __author__ = "Gramazio Kohler Research"
 __author_email__ = "gramaziokohler@arch.ethz.ch"
 __license__ = "MIT license"
 __copyright__ = "Copyright {} Gramazio Kohler Research".format(datetime.today().year)
 
 __all__ = [
     "__author__",
```

### Comparing `compas_timber-0.2.8/src/compas_timber/assembly/__init__.py` & `compas_timber-0.2.9/src/compas_timber/assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/assembly/assembly.py` & `compas_timber-0.2.9/src/compas_timber/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/__init__.py` & `compas_timber-0.2.9/src/compas_timber/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/joint.py` & `compas_timber-0.2.9/src/compas_timber/connections/joint.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/l_butt.py` & `compas_timber-0.2.9/src/compas_timber/connections/l_butt.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/l_miter.py` & `compas_timber-0.2.9/src/compas_timber/connections/l_miter.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/solver.py` & `compas_timber-0.2.9/src/compas_timber/connections/solver.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/connections/t_butt.py` & `compas_timber-0.2.9/src/compas_timber/connections/t_butt.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Assembly/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Assembly/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Check/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Check/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Create/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Create/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Delete/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Delete/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Get_Custom/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Attributes_Set_Custom/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_AutomaticJoints/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_AutomaticJoints/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Bake_BoxMap/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Bake_BoxMap/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_BeamDecompose/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_BeamDecompose/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurve/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurve/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Beam_fromCurveGuid/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FeatureBrepSubtraction/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_Feature_Trim/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_Feature_Trim/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_FindByGuid/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_FindByGuid/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LButt/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LButt/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_LMiter/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_LMiter/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_Rule/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_Rule/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_JointDef_TButt/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_JointDef_TButt/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowAssembly/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowAssembly/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamFrame/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamFrame/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamIndex/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamIndex/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowBeamShape/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowBeamShape/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/code.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/code.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/icon.png` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/icon.png`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/CT_ShowJointTypes/metadata.json` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/CT_ShowJointTypes/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_AttributeName.ghuser` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_AttributeName.ghuser`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_JointType.ghuser` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/ghuser/CT_SelectionList_JointType.ghuser`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/components/install.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/components/install.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/ghcomponent_helpers.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/ghcomponent_helpers.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_AttributeName.ghuser` & `compas_timber-0.2.9/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_AttributeName.ghuser`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_JointType.ghuser` & `compas_timber-0.2.9/src/compas_timber/ghpython/ghuser_manual/CT_SelectionList_JointType.ghuser`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/rhino_object_name_attributes.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/rhino_object_name_attributes.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/ghpython/workflow.py` & `compas_timber-0.2.9/src/compas_timber/ghpython/workflow.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/parts/__init__.py` & `compas_timber-0.2.9/src/compas_timber/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/parts/beam.py` & `compas_timber-0.2.9/src/compas_timber/parts/beam.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/parts/features.py` & `compas_timber-0.2.9/src/compas_timber/parts/features.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/rhino/__init__.py` & `compas_timber-0.2.9/src/compas_timber/rhino/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/rhino/install.py` & `compas_timber-0.2.9/src/compas_timber/rhino/install.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/utils/compas_extra.py` & `compas_timber-0.2.9/src/compas_timber/utils/compas_extra.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/utils/helpers.py` & `compas_timber-0.2.9/src/compas_timber/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/utils/r_tree.py` & `compas_timber-0.2.9/src/compas_timber/utils/r_tree.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/utils/rhino_compas.py` & `compas_timber-0.2.9/src/compas_timber/utils/rhino_compas.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber/utils/rhinoscript.py` & `compas_timber-0.2.9/src/compas_timber/utils/rhinoscript.py`

 * *Files identical despite different names*

### Comparing `compas_timber-0.2.8/src/compas_timber.egg-info/PKG-INFO` & `compas_timber-0.2.9/src/compas_timber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-timber
-Version: 0.2.8
+Version: 0.2.9
 Summary: COMPAS package for modeling, designing and fabricating timber assemblies.
 Home-page: https://github.com/gramaziokohler/compas_timber
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # compas_timber
 
 [![Github Actions Build Status](https://github.com/gramaziokohler/compas_timber/workflows/build/badge.svg)](https://github.com/gramaziokohler/compas_timber/actions)
 [![License](https://img.shields.io/github/license/gramaziokohler/compas_timber.svg)](https://pypi.python.org/pypi/compas_timber)
```

### Comparing `compas_timber-0.2.8/src/compas_timber.egg-info/SOURCES.txt` & `compas_timber-0.2.9/src/compas_timber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

