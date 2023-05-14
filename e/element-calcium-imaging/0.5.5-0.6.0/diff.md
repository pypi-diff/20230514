# Comparing `tmp/element-calcium-imaging-0.5.5.tar.gz` & `tmp/element-calcium-imaging-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.5.5.tar", last modified: Thu Apr  6 22:06:11 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.6.0.tar", last modified: Sun May 14 01:01:57 2023, max compression
```

## Comparing `element-calcium-imaging-0.5.5.tar` & `element-calcium-imaging-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63065 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    60196 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    70680 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-06 22:06:11.000000 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-06 22:06:11.000000 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 22:06:11.000000 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-06 22:06:11.000000 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 22:06:11.000000 element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 22:06:11.207265 element-calcium-imaging-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-06 22:06:08.000000 element-calcium-imaging-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66658 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74194 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26752 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:01:57.615209 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 01:01:57.000000 element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:01:57.619209 element-calcium-imaging-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 01:01:51.000000 element-calcium-imaging-0.6.0/setup.py
```

### Comparing `element-calcium-imaging-0.5.5/LICENSE` & `element-calcium-imaging-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_no_curation.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 
 @schema
 class MaskType(dj.Lookup):
     """Available labels for segmented masks (e.g. 'soma', 'axon', 'dendrite', 'neuropil').
 
     Attributes:
-        masky_type (str): Mask type.
+        mask_type (str): Mask type.
     """
 
     definition = """# Possible types of a segmented mask
     mask_type: varchar(16)
     """
 
     contents = zip(["soma", "axon", "dendrite", "neuropil", "artefact", "unknown"])
@@ -217,21 +217,21 @@
 @schema
 class ProcessingTask(dj.Manual):
     """A pairing of processing params and scans to be loaded or triggered
 
     This table defines a calcium imaging processing task for a combination of a
     `Scan` and a `ProcessingParamSet` entries, including all the inputs (scan, method,
     method's parameters). The task defined here is then run in the downstream table
-    Processing. This table supports definitions of both loading of pre-generated results
-    and the triggering of new analysis for all supported analysis methods
+    `Processing`. This table supports definitions of both loading of pre-generated results
+    and the triggering of new analysis for all supported analysis methods.
 
     Attributes:
-        scan.Scan (foreign key):
-        ProcessingParamSet (foreign key):
-        processing_output_dir (str):
+        scan.Scan (foreign key): Primary key from scan.Scan.
+        ProcessingParamSet (foreign key): Primary key from ProcessingParamSet.
+        processing_output_dir (str): Output directory of the processed scan relative to the root data directory.
         task_mode (str): One of 'load' (load computed analysis results) or 'trigger'
             (trigger computation).
     """
 
     definition = """# Manual table for defining a processing task ready to be run
     -> scan.Scan
     -> ProcessingParamSet
@@ -534,102 +534,29 @@
 
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
         self.insert1(key)
 
 
-@schema
-class Curation(dj.Manual):
-    """Curated results
-
-    If no curation is applied, the curation_output_dir can be set to
-    the value of processing_output_dir.
-
-    Attributes:
-        Processing (foreign key): Primary key from Processing.
-        curation_id (int): Unique curation ID.
-        curation_time (datetime): Time of generation of this set of curated results.
-        curation_output_dir (str): Output directory of the curated results, relative to
-            root data directory.
-        manual_curation (bool): If True, manual curation has been performed on this
-            result.
-        curation_note (str, optional): Notes about the curation task.
-    """
-
-    definition = """# Curation(s) results
-    -> Processing
-    curation_id: int
-    ---
-    curation_time: datetime  # Time of generation of this set of curated results
-    curation_output_dir: varchar(255)  # Output directory of the curated results, relative to root data directory
-    manual_curation: bool  # Has manual curation been performed on this result?
-    curation_note='': varchar(2000)
-    """
-
-    def create1_from_processing_task(self, key, is_curated=False, curation_note=""):
-        """Create a Curation entry for a given ProcessingTask key.
-
-        Args:
-            key (dict): Primary key set of an entry in the ProcessingTask table.
-            is_curated (bool): When True, indicates a manual curation.
-            curation_note (str): User's note on the specifics of the curation.
-        """
-        if key not in Processing():
-            raise ValueError(
-                f"No corresponding entry in Processing available for: {key};"
-                f"Please run `Processing.populate(key)`"
-            )
-
-        output_dir = (ProcessingTask & key).fetch1("processing_output_dir")
-        method, imaging_dataset = get_loader_result(key, ProcessingTask)
-
-        if method == "suite2p":
-            suite2p_dataset = imaging_dataset
-            curation_time = suite2p_dataset.creation_time
-        elif method == "caiman":
-            caiman_dataset = imaging_dataset
-            curation_time = caiman_dataset.creation_time
-        elif method == "extract":
-            extract_dataset = imaging_dataset
-            curation_time = extract_dataset.creation_time
-        else:
-            raise NotImplementedError("Unknown method: {}".format(method))
-
-        # Synthesize curation_id
-        curation_id = (
-            dj.U().aggr(self & key, n="ifnull(max(curation_id)+1,1)").fetch1("n")
-        )
-        self.insert1(
-            {
-                **key,
-                "curation_id": curation_id,
-                "curation_time": curation_time,
-                "curation_output_dir": output_dir,
-                "manual_curation": is_curated,
-                "curation_note": curation_note,
-            }
-        )
-
-
 # -------------- Motion Correction --------------
 
 
 @schema
 class MotionCorrection(dj.Imported):
     """Results of motion correction shifts performed on the imaging data.
 
     Attributes:
-        Curation (foreign key): Primary key from Curation.
+        Processing (foreign key): Primary key from Processing.
         scan.Channel.proj(motion_correct_channel='channel') (int): Channel used for
             motion correction in this processing task.
     """
 
     definition = """# Results of motion correction
-    -> Curation
+    -> Processing
     ---
     -> scan.Channel.proj(motion_correct_channel='channel') # channel used for motion correction in this processing task
     """
 
     class RigidMotionCorrection(dj.Part):
         """Details of rigid motion correction performed on the imaging data.
 
@@ -743,21 +670,21 @@
         correlation_image=null  : longblob  # correlation map (computed during cell detection)
         max_proj_image=null     : longblob  # max of registered frames
         """
 
     def make(self, key):
         """Populate MotionCorrection with results parsed from analysis outputs"""
 
-        method, imaging_dataset = get_loader_result(key, Curation)
+        method, imaging_dataset = get_loader_result(key, ProcessingTask)
 
         field_keys, _ = (scan.ScanInfo.Field & key).fetch(
             "KEY", "field_z", order_by="field_z"
         )
 
-        if method in ["suite2p", "extract"]:
+        if method == "suite2p":
             suite2p_dataset = imaging_dataset
 
             motion_correct_channel = suite2p_dataset.planes[0].alignment_channel
 
             # ---- iterate through all s2p plane outputs ----
             rigid_correction, nonrigid_correction, nonrigid_blocks = {}, {}, {}
             summary_images = []
@@ -848,15 +775,15 @@
                                 "y_std": np.nanstd(bshift_y),
                                 "x_std": np.nanstd(bshift_x),
                                 "z_std": np.nan,
                             }
 
                 # -- summary images --
                 motion_correction_key = (
-                    scan.ScanInfo.Field * Curation & key & field_keys[plane]
+                    scan.ScanInfo.Field * Processing & key & field_keys[plane]
                 ).fetch1("KEY")
                 summary_images.append(
                     {
                         **motion_correction_key,
                         "ref_image": s2p.ref_image,
                         "average_image": s2p.mean_image,
                         "correlation_image": s2p.correlation_map,
@@ -1073,19 +1000,19 @@
 
 
 @schema
 class Segmentation(dj.Computed):
     """Result of the Segmentation process.
 
     Attributes:
-        Curation (foreign key): Primary key from Curation.
+        Processing (foreign key): Primary key from Processing.
     """
 
     definition = """# Different mask segmentations.
-    -> Curation
+    -> Processing
     """
 
     class Mask(dj.Part):
         """Details of the masks identified from the Segmentation procedure.
 
         Attributes:
             Segmentation (foreign key): Primary key from Segmentation.
@@ -1116,15 +1043,15 @@
         mask_zpix=null     : longblob  # z coordinates in pixels
         mask_weights       : longblob  # weights of the mask at the indices above
         """
 
     def make(self, key):
         """Populate the Segmentation with the results parsed from analysis outputs."""
 
-        method, imaging_dataset = get_loader_result(key, Curation)
+        method, imaging_dataset = get_loader_result(key, ProcessingTask)
 
         if method == "suite2p":
             suite2p_dataset = imaging_dataset
 
             # ---- iterate through all s2p plane outputs ----
             masks, cells = [], []
             for plane, s2p in suite2p_dataset.planes.items():
@@ -1338,15 +1265,15 @@
         fluorescence                : longblob  # Fluorescence trace associated with this mask
         neuropil_fluorescence=null  : longblob  # Neuropil fluorescence trace
         """
 
     def make(self, key):
         """Populate the Fluorescence with the results parsed from analysis outputs."""
 
-        method, imaging_dataset = get_loader_result(key, Curation)
+        method, imaging_dataset = get_loader_result(key, ProcessingTask)
 
         if method == "suite2p":
             suite2p_dataset = imaging_dataset
 
             # ---- iterate through all s2p plane outputs ----
             fluo_traces, fluo_chn2_traces = [], []
             for s2p in suite2p_dataset.planes.values():
@@ -1483,18 +1410,17 @@
             * ProcessingParamSet.proj("processing_method")
             & 'processing_method = "caiman"'
             & 'extraction_method LIKE "caiman%"'
         )
         return suite2p_key_source.proj() + caiman_key_source.proj()
 
     def make(self, key):
-        """Populate the Activity with the results parsed from analysis
-        outputs."""
+        """Populate the Activity with the results parsed from analysis outputs."""
 
-        method, imaging_dataset = get_loader_result(key, Curation)
+        method, imaging_dataset = get_loader_result(key, ProcessingTask)
 
         if method == "suite2p":
             if key["extraction_method"] == "suite2p_deconvolution":
                 suite2p_dataset = imaging_dataset
                 # ---- iterate through all s2p plane outputs ----
                 spikes = [
                     dict(
@@ -1540,14 +1466,128 @@
                     )
                     for mask in caiman_dataset.masks
                 )
         else:
             raise NotImplementedError("Unknown/unimplemented method: {}".format(method))
 
 
+@schema
+class ProcessingQualityMetrics(dj.Computed):
+    """Quality metrics used to evaluate the results of the calcium imaging analysis pipeline.
+
+    Attributes:
+        Fluorescence (foreign key): Primary key from Fluorescence.
+    """
+
+    definition = """
+    -> Fluorescence
+    """
+
+    class Mask(dj.Part):
+        """Quality metrics used to evaluate the masks.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Segmentation.Mask (foreign key): Primary key from Segmentation.Mask.
+            mask_area (float): Mask area in square micrometer.
+            roundness (float): Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+        definition = """
+        -> master
+        -> Segmentation.Mask
+        ---
+        mask_area=null: float  # Mask area in square micrometer.
+        roundness: float       # Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+    class Trace(dj.Part):
+        """Quality metrics used to evaluate the fluorescence traces.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Fluorescence.Trace (foreign key): Primary key from Fluorescence.Trace.
+            skewness (float): Skewness of the fluorescence trace.
+            variance (float): Variance of the fluorescence trace.
+        """
+
+        definition = """
+        -> master
+        -> Fluorescence.Trace
+        ---
+        skewness: float   # Skewness of the fluorescence trace.
+        variance: float   # Variance of the fluorescence trace.
+        """
+
+    def make(self, key):
+        """Populate the ProcessingQualityMetrics table and its part tables."""
+        from scipy.stats import skew
+
+        (
+            mask_xpixs,
+            mask_ypixs,
+            mask_weights,
+            fluorescence,
+            fluo_channels,
+            mask_ids,
+            mask_npix,
+            px_height,
+            px_width,
+            um_height,
+            um_width,
+        ) = (Segmentation.Mask * scan.ScanInfo.Field * Fluorescence.Trace & key).fetch(
+            "mask_xpix",
+            "mask_ypix",
+            "mask_weights",
+            "fluorescence",
+            "fluo_channel",
+            "mask",
+            "mask_npix",
+            "px_height",
+            "px_width",
+            "um_height",
+            "um_width",
+        )
+
+        norm_mean = lambda x: x.mean() / x.max()
+        roundnesses = [
+            norm_mean(np.linalg.eigvals(np.cov(x, y, aweights=w)))
+            for x, y, w in zip(mask_xpixs, mask_ypixs, mask_weights)
+        ]
+
+        fluorescence = np.stack(fluorescence)
+
+        self.insert1(key)
+
+        self.Mask.insert(
+            dict(key, mask=mask_id, mask_area=mask_area, roundness=roundness)
+            for mask_id, mask_area, roundness in zip(
+                mask_ids,
+                mask_npix * (um_height / px_height) * (um_width / px_width),
+                roundnesses,
+            )
+        )
+
+        self.Trace.insert(
+            dict(
+                key,
+                fluo_channel=fluo_channel,
+                mask=mask_id,
+                skewness=skewness,
+                variance=variance,
+            )
+            for fluo_channel, mask_id, skewness, variance in zip(
+                fluo_channels,
+                mask_ids,
+                skew(fluorescence, axis=1),
+                fluorescence.std(axis=1),
+            )
+        )
+
+
 # ---------------- HELPER FUNCTIONS ----------------
 
 
 _table_attribute_mapper = {
     "ProcessingTask": "processing_output_dir",
     "Curation": "curation_output_dir",
 }
```

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 schema = dj.Schema()
 
 _linking_module = None
 
 
 def activate(
-    imaging_schema_name,
-    scan_schema_name=None,
+    imaging_schema_name: str,
+    scan_schema_name: str = None,
     *,
-    create_schema=True,
-    create_tables=True,
-    linking_module=None,
+    create_schema: bool = True,
+    create_tables: bool = True,
+    linking_module: str = None,
 ):
     """Activate this schema.
 
     Args:
         imaging_schema_name (str): Schema name on the database server to activate the
             `imaging` module.
         scan_schema_name (str): Schema name on the database server to activate the
@@ -197,15 +197,15 @@
 
 
 @schema
 class MaskType(dj.Lookup):
     """Available labels for segmented masks (e.g. 'soma', 'axon', 'dendrite', 'neuropil').
 
     Attributes:
-        masky_type (str): Mask type.
+        mask_type (str): Mask type.
     """
 
     definition = """# Possible types of a segmented mask
     mask_type: varchar(16)
     """
 
     contents = zip(["soma", "axon", "dendrite", "neuropil", "artefact", "unknown"])
@@ -221,17 +221,17 @@
     This table defines a calcium imaging processing task for a combination of a
     `Scan` and a `ProcessingParamSet` entries, including all the inputs (scan, method,
     method's parameters). The task defined here is then run in the downstream table
     Processing. This table supports definitions of both loading of pre-generated results
     and the triggering of new analysis for all supported analysis methods
 
     Attributes:
-        scan.Scan (foreign key):
-        ProcessingParamSet (foreign key):
-        processing_output_dir (str):
+        scan.Scan (foreign key): Primary key from scan.Scan.
+        ProcessingParamSet (foreign key): Primary key from ProcessingParamSet.
+        processing_output_dir (str): Output directory of the processed scan relative to the root data directory.
         task_mode (str): One of 'load' (load computed analysis results) or 'trigger'
             (trigger computation).
     """
 
     definition = """# Manual table for defining a processing task ready to be run
     -> scan.Scan
     -> ProcessingParamSet
@@ -534,29 +534,102 @@
 
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
         self.insert1(key)
 
 
+@schema
+class Curation(dj.Manual):
+    """Curated results
+
+    If no curation is applied, the curation_output_dir can be set to
+    the value of processing_output_dir.
+
+    Attributes:
+        Processing (foreign key): Primary key from Processing.
+        curation_id (int): Unique curation ID.
+        curation_time (datetime): Time of generation of this set of curated results.
+        curation_output_dir (str): Output directory of the curated results, relative to
+            root data directory.
+        manual_curation (bool): If True, manual curation has been performed on this
+            result.
+        curation_note (str, optional): Notes about the curation task.
+    """
+
+    definition = """# Curation(s) results
+    -> Processing
+    curation_id: int
+    ---
+    curation_time: datetime  # Time of generation of this set of curated results
+    curation_output_dir: varchar(255)  # Output directory of the curated results, relative to root data directory
+    manual_curation: bool  # Has manual curation been performed on this result?
+    curation_note='': varchar(2000)
+    """
+
+    def create1_from_processing_task(self, key, is_curated=False, curation_note=""):
+        """Create a Curation entry for a given ProcessingTask key.
+
+        Args:
+            key (dict): Primary key set of an entry in the ProcessingTask table.
+            is_curated (bool): When True, indicates a manual curation.
+            curation_note (str): User's note on the specifics of the curation.
+        """
+        if key not in Processing():
+            raise ValueError(
+                f"No corresponding entry in Processing available for: {key};"
+                f"Please run `Processing.populate(key)`"
+            )
+
+        output_dir = (ProcessingTask & key).fetch1("processing_output_dir")
+        method, imaging_dataset = get_loader_result(key, ProcessingTask)
+
+        if method == "suite2p":
+            suite2p_dataset = imaging_dataset
+            curation_time = suite2p_dataset.creation_time
+        elif method == "caiman":
+            caiman_dataset = imaging_dataset
+            curation_time = caiman_dataset.creation_time
+        elif method == "extract":
+            extract_dataset = imaging_dataset
+            curation_time = extract_dataset.creation_time
+        else:
+            raise NotImplementedError("Unknown method: {}".format(method))
+
+        # Synthesize curation_id
+        curation_id = (
+            dj.U().aggr(self & key, n="ifnull(max(curation_id)+1,1)").fetch1("n")
+        )
+        self.insert1(
+            {
+                **key,
+                "curation_id": curation_id,
+                "curation_time": curation_time,
+                "curation_output_dir": output_dir,
+                "manual_curation": is_curated,
+                "curation_note": curation_note,
+            }
+        )
+
+
 # -------------- Motion Correction --------------
 
 
 @schema
 class MotionCorrection(dj.Imported):
     """Results of motion correction shifts performed on the imaging data.
 
     Attributes:
-        Processing (foreign key): Primary key from Processing.
+        Curation (foreign key): Primary key from Curation.
         scan.Channel.proj(motion_correct_channel='channel') (int): Channel used for
             motion correction in this processing task.
     """
 
     definition = """# Results of motion correction
-    -> Processing
+    -> Curation
     ---
     -> scan.Channel.proj(motion_correct_channel='channel') # channel used for motion correction in this processing task
     """
 
     class RigidMotionCorrection(dj.Part):
         """Details of rigid motion correction performed on the imaging data.
 
@@ -669,21 +742,22 @@
         average_image           : longblob  # mean of registered frames
         correlation_image=null  : longblob  # correlation map (computed during cell detection)
         max_proj_image=null     : longblob  # max of registered frames
         """
 
     def make(self, key):
         """Populate MotionCorrection with results parsed from analysis outputs"""
-        method, imaging_dataset = get_loader_result(key, ProcessingTask)
+
+        method, imaging_dataset = get_loader_result(key, Curation)
 
         field_keys, _ = (scan.ScanInfo.Field & key).fetch(
             "KEY", "field_z", order_by="field_z"
         )
 
-        if method == "suite2p":
+        if method in ["suite2p", "extract"]:
             suite2p_dataset = imaging_dataset
 
             motion_correct_channel = suite2p_dataset.planes[0].alignment_channel
 
             # ---- iterate through all s2p plane outputs ----
             rigid_correction, nonrigid_correction, nonrigid_blocks = {}, {}, {}
             summary_images = []
@@ -774,15 +848,15 @@
                                 "y_std": np.nanstd(bshift_y),
                                 "x_std": np.nanstd(bshift_x),
                                 "z_std": np.nan,
                             }
 
                 # -- summary images --
                 motion_correction_key = (
-                    scan.ScanInfo.Field * Processing & key & field_keys[plane]
+                    scan.ScanInfo.Field * Curation & key & field_keys[plane]
                 ).fetch1("KEY")
                 summary_images.append(
                     {
                         **motion_correction_key,
                         "ref_image": s2p.ref_image,
                         "average_image": s2p.mean_image,
                         "correlation_image": s2p.correlation_map,
@@ -999,19 +1073,19 @@
 
 
 @schema
 class Segmentation(dj.Computed):
     """Result of the Segmentation process.
 
     Attributes:
-        Processing (foreign key): Primary key from Processing.
+        Curation (foreign key): Primary key from Curation.
     """
 
     definition = """# Different mask segmentations.
-    -> Processing
+    -> Curation
     """
 
     class Mask(dj.Part):
         """Details of the masks identified from the Segmentation procedure.
 
         Attributes:
             Segmentation (foreign key): Primary key from Segmentation.
@@ -1026,31 +1100,31 @@
             mask_ypix (longblob): Y coordinates in pixels.
             mask_zpix (longblob): Z coordinates in pixels.
             mask_weights (longblob): Weights of the mask at the indices above.
         """
 
         definition = """ # A mask produced by segmentation.
         -> master
-        mask            : smallint
+        mask               : smallint
         ---
         -> scan.Channel.proj(segmentation_channel='channel')  # channel used for segmentation
-        mask_npix       : int       # number of pixels in ROIs
-        mask_center_x   : int       # center x coordinate in pixel
-        mask_center_y   : int       # center y coordinate in pixel
-        mask_center_z   : int       # center z coordinate in pixel
-        mask_xpix       : longblob  # x coordinates in pixels
-        mask_ypix       : longblob  # y coordinates in pixels
-        mask_zpix       : longblob  # z coordinates in pixels
-        mask_weights    : longblob  # weights of the mask at the indices above
+        mask_npix          : int       # number of pixels in ROIs
+        mask_center_x      : int       # center x coordinate in pixel
+        mask_center_y      : int       # center y coordinate in pixel
+        mask_center_z=null : int       # center z coordinate in pixel
+        mask_xpix          : longblob  # x coordinates in pixels
+        mask_ypix          : longblob  # y coordinates in pixels
+        mask_zpix=null     : longblob  # z coordinates in pixels
+        mask_weights       : longblob  # weights of the mask at the indices above
         """
 
     def make(self, key):
         """Populate the Segmentation with the results parsed from analysis outputs."""
 
-        method, imaging_dataset = get_loader_result(key, ProcessingTask)
+        method, imaging_dataset = get_loader_result(key, Curation)
 
         if method == "suite2p":
             suite2p_dataset = imaging_dataset
 
             # ---- iterate through all s2p plane outputs ----
             masks, cells = [], []
             for plane, s2p in suite2p_dataset.planes.items():
@@ -1264,15 +1338,15 @@
         fluorescence                : longblob  # Fluorescence trace associated with this mask
         neuropil_fluorescence=null  : longblob  # Neuropil fluorescence trace
         """
 
     def make(self, key):
         """Populate the Fluorescence with the results parsed from analysis outputs."""
 
-        method, imaging_dataset = get_loader_result(key, ProcessingTask)
+        method, imaging_dataset = get_loader_result(key, Curation)
 
         if method == "suite2p":
             suite2p_dataset = imaging_dataset
 
             # ---- iterate through all s2p plane outputs ----
             fluo_traces, fluo_chn2_traces = [], []
             for s2p in suite2p_dataset.planes.values():
@@ -1409,18 +1483,17 @@
             * ProcessingParamSet.proj("processing_method")
             & 'processing_method = "caiman"'
             & 'extraction_method LIKE "caiman%"'
         )
         return suite2p_key_source.proj() + caiman_key_source.proj()
 
     def make(self, key):
-        """
-        Populate the Activity with the results parsed from analysis outputs.
-        """
-        method, imaging_dataset = get_loader_result(key, ProcessingTask)
+        """Populate the Activity with the results parsed from analysis outputs."""
+
+        method, imaging_dataset = get_loader_result(key, Curation)
 
         if method == "suite2p":
             if key["extraction_method"] == "suite2p_deconvolution":
                 suite2p_dataset = imaging_dataset
                 # ---- iterate through all s2p plane outputs ----
                 spikes = [
                     dict(
@@ -1466,14 +1539,128 @@
                     )
                     for mask in caiman_dataset.masks
                 )
         else:
             raise NotImplementedError("Unknown/unimplemented method: {}".format(method))
 
 
+@schema
+class ProcessingQualityMetrics(dj.Computed):
+    """Quality metrics used to evaluate the results of the calcium imaging analysis pipeline.
+
+    Attributes:
+        Fluorescence (foreign key): Primary key from Fluorescence.
+    """
+
+    definition = """
+    -> Fluorescence
+    """
+
+    class Mask(dj.Part):
+        """Quality metrics used to evaluate the masks.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Segmentation.Mask (foreign key): Primary key from Segmentation.Mask.
+            mask_area (float): Mask area in square micrometer.
+            roundness (float): Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+        definition = """
+        -> master
+        -> Segmentation.Mask
+        ---
+        mask_area=null: float  # Mask area in square micrometer.
+        roundness: float       # Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+    class Trace(dj.Part):
+        """Quality metrics used to evaluate the fluorescence traces.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Fluorescence.Trace (foreign key): Primary key from Fluorescence.Trace.
+            skewness (float): Skewness of the fluorescence trace.
+            variance (float): Variance of the fluorescence trace.
+        """
+
+        definition = """
+        -> master
+        -> Fluorescence.Trace
+        ---
+        skewness: float   # Skewness of the fluorescence trace.
+        variance: float   # Variance of the fluorescence trace.
+        """
+
+    def make(self, key):
+        """Populate the ProcessingQualityMetrics table and its part tables."""
+        from scipy.stats import skew
+
+        (
+            mask_xpixs,
+            mask_ypixs,
+            mask_weights,
+            fluorescence,
+            fluo_channels,
+            mask_ids,
+            mask_npix,
+            px_height,
+            px_width,
+            um_height,
+            um_width,
+        ) = (Segmentation.Mask * scan.ScanInfo.Field * Fluorescence.Trace & key).fetch(
+            "mask_xpix",
+            "mask_ypix",
+            "mask_weights",
+            "fluorescence",
+            "fluo_channel",
+            "mask",
+            "mask_npix",
+            "px_height",
+            "px_width",
+            "um_height",
+            "um_width",
+        )
+
+        norm_mean = lambda x: x.mean() / x.max()
+        roundnesses = [
+            norm_mean(np.linalg.eigvals(np.cov(x, y, aweights=w)))
+            for x, y, w in zip(mask_xpixs, mask_ypixs, mask_weights)
+        ]
+
+        fluorescence = np.stack(fluorescence)
+
+        self.insert1(key)
+
+        self.Mask.insert(
+            dict(key, mask=mask_id, mask_area=mask_area, roundness=roundness)
+            for mask_id, mask_area, roundness in zip(
+                mask_ids,
+                mask_npix * (um_height / px_height) * (um_width / px_width),
+                roundnesses,
+            )
+        )
+
+        self.Trace.insert(
+            dict(
+                key,
+                fluo_channel=fluo_channel,
+                mask=mask_id,
+                skewness=skewness,
+                variance=variance,
+            )
+            for fluo_channel, mask_id, skewness, variance in zip(
+                fluo_channels,
+                mask_ids,
+                skew(fluorescence, axis=1),
+                fluorescence.std(axis=1),
+            )
+        )
+
+
 # ---------------- HELPER FUNCTIONS ----------------
 
 
 _table_attribute_mapper = {
     "ProcessingTask": "processing_output_dir",
     "Curation": "curation_output_dir",
 }
```

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -381,15 +381,15 @@
 
 
 @schema
 class MaskType(dj.Lookup):
     """Available labels for segmented masks (e.g. 'soma', 'axon', 'dendrite', 'neuropil').
 
     Attributes:
-        masky_type (str): Mask type.
+        mask_type (str): Mask type.
     """
 
     definition = """# Possible types of a segmented mask
     mask_type: varchar(16)
     """
 
     contents = zip(["soma", "axon", "dendrite", "neuropil", "artefact", "unknown"])
@@ -405,17 +405,17 @@
     This table defines a calcium imaging processing task for a combination of a
     `Scan` and a `ProcessingParamSet` entries, including all the inputs (scan, method,
     method's parameters). The task defined here is then run in the downstream table
     Processing. This table supports definitions of both loading of pre-generated results
     and the triggering of new analysis for all supported analysis methods
 
     Attributes:
-        Preprocess (foreign key):
-        ProcessingParamSet (foreign key):
-        processing_output_dir (str):
+        Preprocess (foreign key): Primary key from Preprocess.
+        ProcessingParamSet (foreign key): Primary key from ProcessingParamSet.
+        processing_output_dir (str): Output directory of the processed scan relative to the root data directory.
         task_mode (str): One of 'load' (load computed analysis results) or 'trigger'
             (trigger computation).
     """
 
     definition = """# Manual table for defining a processing task ready to be run
     -> Preprocess
     -> ProcessingParamSet
@@ -1429,35 +1429,35 @@
                         "mask_classification_method": "caiman_default_classifier",
                     },
                     allow_direct_insert=True,
                 )
                 MaskClassification.MaskType.insert(
                     cells, ignore_extra_fields=True, allow_direct_insert=True
                 )
-            elif method == "extract":
-                extract_dataset = imaging_dataset
-                masks = [
-                    dict(
-                        **key,
-                        segmentation_channel=0,
-                        mask=mask["mask_id"],
-                        mask_npix=mask["mask_npix"],
-                        mask_center_x=mask["mask_center_x"],
-                        mask_center_y=mask["mask_center_y"],
-                        mask_center_z=mask["mask_center_z"],
-                        mask_xpix=mask["mask_xpix"],
-                        mask_ypix=mask["mask_ypix"],
-                        mask_zpix=mask["mask_zpix"],
-                        mask_weights=mask["mask_weights"],
-                    )
-                    for mask in extract_dataset.load_results()
-                ]
+        elif method == "extract":
+            extract_dataset = imaging_dataset
+            masks = [
+                dict(
+                    **key,
+                    segmentation_channel=0,
+                    mask=mask["mask_id"],
+                    mask_npix=mask["mask_npix"],
+                    mask_center_x=mask["mask_center_x"],
+                    mask_center_y=mask["mask_center_y"],
+                    mask_center_z=mask["mask_center_z"],
+                    mask_xpix=mask["mask_xpix"],
+                    mask_ypix=mask["mask_ypix"],
+                    mask_zpix=mask["mask_zpix"],
+                    mask_weights=mask["mask_weights"],
+                )
+                for mask in extract_dataset.load_results()
+            ]
 
-                self.insert1(key)
-                self.Mask.insert(masks, ignore_extra_fields=True)
+            self.insert1(key)
+            self.Mask.insert(masks, ignore_extra_fields=True)
         else:
             raise NotImplementedError(f"Unknown/unimplemented method: {method}")
 
 
 @schema
 class MaskClassificationMethod(dj.Lookup):
     """Available mask classification methods.
@@ -1690,16 +1690,15 @@
             * ProcessingParamSet.proj("processing_method")
             & 'processing_method = "caiman"'
             & 'extraction_method LIKE "caiman%"'
         )
         return suite2p_key_source.proj() + caiman_key_source.proj()
 
     def make(self, key):
-        """Populate the Activity with the results parsed from analysis
-        outputs."""
+        """Populate the Activity with the results parsed from analysis outputs."""
 
         method, imaging_dataset = get_loader_result(key, Curation)
 
         if method == "suite2p":
             if key["extraction_method"] == "suite2p_deconvolution":
                 suite2p_dataset = imaging_dataset
                 # ---- iterate through all s2p plane outputs ----
@@ -1747,14 +1746,128 @@
                     )
                     for mask in caiman_dataset.masks
                 )
         else:
             raise NotImplementedError("Unknown/unimplemented method: {}".format(method))
 
 
+@schema
+class ProcessingQualityMetrics(dj.Computed):
+    """Quality metrics used to evaluate the results of the calcium imaging analysis pipeline.
+
+    Attributes:
+        Fluorescence (foreign key): Primary key from Fluorescence.
+    """
+
+    definition = """
+    -> Fluorescence
+    """
+
+    class Mask(dj.Part):
+        """Quality metrics used to evaluate the masks.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Segmentation.Mask (foreign key): Primary key from Segmentation.Mask.
+            mask_area (float): Mask area in square micrometer.
+            roundness (float): Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+        definition = """
+        -> master
+        -> Segmentation.Mask
+        ---
+        mask_area=null: float  # Mask area in square micrometer.
+        roundness: float       # Roundness between 0 and 1. Values closer to 1 are rounder.
+        """
+
+    class Trace(dj.Part):
+        """Quality metrics used to evaluate the fluorescence traces.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Fluorescence.Trace (foreign key): Primary key from Fluorescence.Trace.
+            skewness (float): Skewness of the fluorescence trace.
+            variance (float): Variance of the fluorescence trace.
+        """
+
+        definition = """
+        -> master
+        -> Fluorescence.Trace
+        ---
+        skewness: float   # Skewness of the fluorescence trace.
+        variance: float   # Variance of the fluorescence trace.
+        """
+
+    def make(self, key):
+        """Populate the ProcessingQualityMetrics table and its part tables."""
+        from scipy.stats import skew
+
+        (
+            mask_xpixs,
+            mask_ypixs,
+            mask_weights,
+            fluorescence,
+            fluo_channels,
+            mask_ids,
+            mask_npix,
+            px_height,
+            px_width,
+            um_height,
+            um_width,
+        ) = (Segmentation.Mask * scan.ScanInfo.Field * Fluorescence.Trace & key).fetch(
+            "mask_xpix",
+            "mask_ypix",
+            "mask_weights",
+            "fluorescence",
+            "fluo_channel",
+            "mask",
+            "mask_npix",
+            "px_height",
+            "px_width",
+            "um_height",
+            "um_width",
+        )
+
+        norm_mean = lambda x: x.mean() / x.max()
+        roundnesses = [
+            norm_mean(np.linalg.eigvals(np.cov(x, y, aweights=w)))
+            for x, y, w in zip(mask_xpixs, mask_ypixs, mask_weights)
+        ]
+
+        fluorescence = np.stack(fluorescence)
+
+        self.insert1(key)
+
+        self.Mask.insert(
+            dict(key, mask=mask_id, mask_area=mask_area, roundness=roundness)
+            for mask_id, mask_area, roundness in zip(
+                mask_ids,
+                mask_npix * (um_height / px_height) * (um_width / px_width),
+                roundnesses,
+            )
+        )
+
+        self.Trace.insert(
+            dict(
+                key,
+                fluo_channel=fluo_channel,
+                mask=mask_id,
+                skewness=skewness,
+                variance=variance,
+            )
+            for fluo_channel, mask_id, skewness, variance in zip(
+                fluo_channels,
+                mask_ids,
+                skew(fluorescence, axis=1),
+                fluorescence.std(axis=1),
+            )
+        )
+
+
 # ---------------- HELPER FUNCTIONS ----------------
 
 
 _table_attribute_mapper = {
     "ProcessingTask": "processing_output_dir",
     "Curation": "curation_output_dir",
 }
```

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.6.0/element_calcium_imaging/scan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import importlib
 import inspect
 import pathlib
 import re
 from datetime import datetime
 from typing import Union
 
+import numpy as np
 import datajoint as dj
 from element_interface.utils import find_root_directory
 
 schema = dj.schema()
 
 _linking_module = None
 
@@ -329,23 +330,15 @@
             import scanreader
 
             # Read the scan
             scan_filepaths = get_scan_image_files(key)
             scan = scanreader.read_scan(scan_filepaths)
 
             # Insert in ScanInfo
-            x_zero = (
-                scan.motor_position_at_zero[0] if scan.motor_position_at_zero else None
-            )
-            y_zero = (
-                scan.motor_position_at_zero[1] if scan.motor_position_at_zero else None
-            )
-            z_zero = (
-                scan.motor_position_at_zero[2] if scan.motor_position_at_zero else None
-            )
+            x_zero, y_zero, z_zero = scan.motor_position_at_zero or (None, None, None)
 
             self.insert1(
                 dict(
                     key,
                     nfields=scan.num_fields,
                     nchannels=scan.num_channels,
                     nframes=scan.num_frames,
@@ -609,7 +602,100 @@
         # Insert file(s)
         root_dir = find_root_directory(get_imaging_root_data_dir(), scan_filepaths[0])
 
         scan_files = [
             pathlib.Path(f).relative_to(root_dir).as_posix() for f in scan_filepaths
         ]
         self.ScanFile.insert([{**key, "file_path": f} for f in scan_files])
+
+
+@schema
+class ScanQualityMetrics(dj.Computed):
+    """Metrics to assess the quality of the scan.
+
+    Attributes:
+        ScanInfo.Field (foreign key): Primary key from ScanInfo.Field.
+    """
+
+    definition = """
+    -> ScanInfo.Field
+    """
+
+    class Frames(dj.Part):
+        """Metrics used to evaluate each frame.
+
+        Attributes:
+            ScanInfo.Field (foreign key): Primary key from ScanInfo.Field.
+            Channel (foreign key): Primary key from Channel.
+            min_intensity (longblob): Minimum value of each frame.
+            mean_intensity (longblob): Mean value of each frame.
+            max_intensity (longblob): Maximum value of each frame.
+            contrast (longblob): Contrast of each frame (i.e. difference between the 99 and 1 percentiles)
+        """
+
+        definition = """
+        -> master
+        -> Channel
+        ---
+        min_intensity: longblob   # Minimum value of each frame.
+        mean_intensity: longblob  # Mean value of each frame.
+        max_intensity: longblob   # Maximum value of each frame.
+        contrast: longblob        # Contrast of each frame (i.e. difference between the 99 and 1 percentiles)
+        """
+
+    def make(self, key):
+        acq_software, nchannels = (Scan * ScanInfo & key).fetch1(
+            "acq_software", "nchannels"
+        )
+
+        if acq_software == "ScanImage":
+            import scanreader
+
+            # Switch from FYXCT to TCYX
+            data = scanreader.read_scan(get_scan_image_files(key))[
+                key["field_idx"]
+            ].transpose(3, 2, 0, 1)
+        elif acq_software == "Scanbox":
+            from sbxreader import sbx_memmap
+
+            # Switch from TFCYX to TCYX
+            data = sbx_memmap(get_scan_box_files(key))[:, key["field_idx"]]
+        elif acq_software == "NIS":
+            import nd2
+
+            nd2_file = nd2.ND2File(get_nd2_files(key)[0])
+
+            nd2_dims = {k: i for i, k in enumerate(nd2_file.sizes)}
+
+            valid_dimensions = "TZCYX"
+            assert set(nd2_dims) <= set(
+                valid_dimensions
+            ), f"Unknown dimensions {set(nd2_dims)-set(valid_dimensions)} in file {get_nd2_files(key)[0]}."
+
+            # Sort the dimensions in the order of TZCYX, skipping the missing ones.
+            data = nd2_file.asarray().transpose(
+                [nd2_dims[x] for x in valid_dimensions if x in nd2_dims]
+            )
+
+            # Expand array to include the missing dimensions.
+            for i, dim in enumerate("TZC"):
+                if dim not in nd2_dims:
+                    data = np.expand_dims(data, i)
+
+            data = data[:, key["field_idx"]]  # Switch from TFCYX to TCYX
+
+        self.insert1(key)
+
+        for channel in range(nchannels):
+            movie = data[:, channel, :, :]
+
+            self.Frames.insert1(
+                dict(
+                    key,
+                    channel=channel,
+                    min_intensity=movie.min(axis=(1, 2)),
+                    mean_intensity=movie.mean(axis=(1, 2)),
+                    max_intensity=movie.max(axis=(1, 2)),
+                    contrast=np.percentile(movie, 99, axis=(1, 2))
+                    - np.percentile(movie, 1, axis=(1, 2)),
+                )
+            )
```

### Comparing `element-calcium-imaging-0.5.5/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.6.0/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.5.5/setup.py` & `element-calcium-imaging-0.6.0/setup.py`

 * *Files identical despite different names*

