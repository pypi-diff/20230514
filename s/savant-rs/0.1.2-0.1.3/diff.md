# Comparing `tmp/savant_rs-0.1.2.tar.gz` & `tmp/savant_rs-0.1.3.tar.gz`

## Comparing `savant_rs-0.1.2.tar` & `savant_rs-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 savant_rs-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-12 15:17:32.000000 savant_rs-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-12 15:17:32.000000 savant_rs-0.1.2/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-12 15:17:32.000000 savant_rs-0.1.2/LICENSE
--rw-r--r--   0     1001      123      270 2023-05-12 15:17:32.000000 savant_rs-0.1.2/README.md
--rw-r--r--   0     1001      123      769 2023-05-12 15:17:32.000000 savant_rs-0.1.2/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-12 15:17:32.000000 savant_rs-0.1.2/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-12 15:17:32.000000 savant_rs-0.1.2/build.rs
--rw-r--r--   0     1001      123      459 2023-05-12 15:17:32.000000 savant_rs-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123      269 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123      783 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3741 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1108 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123     1018 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123    14168 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/attribute.rs
--rw-r--r--   0     1001      123     1221 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/bbox.rs
--rw-r--r--   0     1001      123      590 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28694 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14354 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6710 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/point.rs
--rw-r--r--   0     1001      123    13870 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1628 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives.rs
--rw-r--r--   0     1001      123     5771 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     5968 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123      512 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/utils.rs
--rw-r--r--   0     1001      123    30961 2023-05-12 15:18:57.000000 savant_rs-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 savant_rs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 savant_rs-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-14 14:45:31.000000 savant_rs-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-14 14:45:31.000000 savant_rs-0.1.3/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-14 14:45:31.000000 savant_rs-0.1.3/LICENSE
+-rw-r--r--   0     1001      123      514 2023-05-14 14:45:31.000000 savant_rs-0.1.3/README.md
+-rw-r--r--   0     1001      123      769 2023-05-14 14:45:31.000000 savant_rs-0.1.3/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-14 14:45:31.000000 savant_rs-0.1.3/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-14 14:45:31.000000 savant_rs-0.1.3/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-14 14:45:31.000000 savant_rs-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123      783 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3741 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1108 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123     1820 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     6394 2023-05-14 14:45:31.000000 savant_rs-0.1.3/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123     1018 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123    14168 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123     1221 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123      590 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2141 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28694 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14354 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6710 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/point.rs
+-rw-r--r--   0     1001      123    13870 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1628 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/primitives.rs
+-rw-r--r--   0     1001      123     5856 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/test.rs
+-rw-r--r--   0     1001      123     1071 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/test_rkyv_tuple.rs
+-rw-r--r--   0     1001      123     2521 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     5968 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123    20581 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     1818 2023-05-14 14:45:31.000000 savant_rs-0.1.3/src/utils.rs
+-rw-r--r--   0     1001      123    36647 2023-05-14 14:46:46.000000 savant_rs-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.3/PKG-INFO
```

### Comparing `savant_rs-0.1.2/Cargo.toml` & `savant_rs-0.1.3/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
@@ -24,18 +24,23 @@
 rayon = "1.7"
 env_logger = "0.10"
 rkyv = { version = "0.7", features = ["validation", "archive_le"] }
 numpy = "0.18"
 pyo3-log = "0.8"
 derive_builder = "0.12"
 num_cpus = "1.15"
+hashbrown = "0.13"
+lazy_static = "1.4"
 
 [dependencies.pyo3]
 version = "0.18"
 
+[dev-dependencies]
+serial_test = "2.0"
+
 [build-dependencies]
 pyo3-build-config = "0.18"
 
 [profile.release]
 opt-level = 3
 
 [profile.bench]
```

### Comparing `savant_rs-0.1.2/.github/workflows/CI.yml` & `savant_rs-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/LICENSE` & `savant_rs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/benches/batch_snapshot.rs` & `savant_rs-0.1.3/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/benches/message_save_load.rs` & `savant_rs-0.1.3/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/python/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.3/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/python/primitives/buf_copy.py` & `savant_rs-0.1.3/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/python/primitives/frame_ops.py` & `savant_rs-0.1.3/python/primitives/frame_ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/python/primitives/polygon_match.py` & `savant_rs-0.1.3/python/primitives/polygon_match.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/lib.rs` & `savant_rs-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/attribute.rs` & `savant_rs-0.1.3/src/primitives/attribute.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/bbox.rs` & `savant_rs-0.1.3/src/primitives/bbox.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/eos.rs` & `savant_rs-0.1.3/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/loader.rs` & `savant_rs-0.1.3/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/saver.rs` & `savant_rs-0.1.3/src/primitives/message/saver.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/video/batch.rs` & `savant_rs-0.1.3/src/primitives/message/video/batch.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/video/frame.rs` & `savant_rs-0.1.3/src/primitives/message/video/frame.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message/video/object.rs` & `savant_rs-0.1.3/src/primitives/message/video/object.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/message.rs` & `savant_rs-0.1.3/src/primitives/message.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/point.rs` & `savant_rs-0.1.3/src/primitives/point.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/polygonal_area.rs` & `savant_rs-0.1.3/src/primitives/polygonal_area.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives/segment.rs` & `savant_rs-0.1.3/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/primitives.rs` & `savant_rs-0.1.3/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/test.rs` & `savant_rs-0.1.3/src/test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -138,8 +138,13 @@
                 ])
                 .build()
                 .unwrap(),
         );
 
         f
     }
+
+    #[inline(always)]
+    pub fn s(a: &str) -> String {
+        a.to_string()
+    }
 }
```

### Comparing `savant_rs-0.1.2/src/test_rkyv_tuple.rs` & `savant_rs-0.1.3/src/test_rkyv_tuple.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/tests_pyo3_access.rs` & `savant_rs-0.1.3/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/src/utils/fps_meter.rs` & `savant_rs-0.1.3/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.2/Cargo.lock` & `savant_rs-0.1.3/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aho-corasick"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
@@ -61,29 +72,41 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "bytecheck"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13fe11640a23eb24562225322cd3e452b93a3d4091d62fab69c70542fcd17d1f"
+checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
 dependencies = [
  "bytecheck_derive",
  "ptr_meta",
  "simdutf8",
 ]
 
 [[package]]
 name = "bytecheck_derive"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e31225543cb46f81a7e224762764f4a6a0f097b1db0b175f69e8065efaa42de5"
+checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -185,14 +208,27 @@
 dependencies = [
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "dashmap"
+version = "5.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+dependencies = [
+ "cfg-if",
+ "hashbrown 0.12.3",
+ "lock_api",
+ "once_cell",
+ "parking_lot_core",
+]
+
+[[package]]
 name = "derive_builder"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
 dependencies = [
  "derive_builder_macro",
 ]
@@ -268,14 +304,97 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
+name = "futures"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-channel"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+]
+
+[[package]]
+name = "futures-core"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+
+[[package]]
+name = "futures-executor"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
+dependencies = [
+ "futures-core",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-io"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+
+[[package]]
+name = "futures-sink"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+
+[[package]]
+name = "futures-task"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+
+[[package]]
+name = "futures-util"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "memchr",
+ "pin-project-lite",
+ "pin-utils",
+ "slab",
+]
+
+[[package]]
 name = "geo"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7d640a4dd1d1c98b45f4653c841a8ec15f461a71b86bc30533ae64c6f20f268"
 dependencies = [
  "float_next_after",
  "geo-types",
@@ -329,15 +448,24 @@
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
- "ahash",
+ "ahash 0.7.6",
+]
+
+[[package]]
+name = "hashbrown"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
+dependencies = [
+ "ahash 0.8.3",
 ]
 
 [[package]]
 name = "heapless"
 version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db04bc24a18b9ea980628ecf00e6c0264f3c1426dac36c00cb49b6fbad8b0743"
@@ -581,14 +709,26 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "pin-project-lite"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+
+[[package]]
+name = "pin-utils"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
@@ -690,14 +830,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
@@ -754,31 +900,34 @@
 checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "rkyv"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21499ed91807f07ae081880aabb2ccc0235e9d88011867d984525e9a4c3cfa3e"
+checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
 dependencies = [
+ "bitvec",
  "bytecheck",
- "hashbrown",
+ "hashbrown 0.12.3",
  "ptr_meta",
  "rend",
  "rkyv_derive",
  "seahash",
+ "tinyvec",
+ "uuid",
 ]
 
 [[package]]
 name = "rkyv_derive"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1c672430eb41556291981f45ca900a0239ad007242d1cb4b4167af842db666"
+checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -831,29 +980,32 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "savant_rs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
+ "hashbrown 0.13.2",
  "itertools",
+ "lazy_static",
  "num_cpus",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "pyo3-log",
  "rayon",
  "rkyv",
  "serde_json",
+ "serial_test",
  "thiserror",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -884,35 +1036,69 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serial_test"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e56dd856803e253c8f298af3f4d7eb0ae5e23a737252cd90bb4f3b435033b2d"
+dependencies = [
+ "dashmap",
+ "futures",
+ "lazy_static",
+ "log",
+ "parking_lot",
+ "serial_test_derive",
+]
+
+[[package]]
+name = "serial_test_derive"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.16",
+]
+
+[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
+name = "slab"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
@@ -944,24 +1130,30 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
@@ -985,30 +1177,51 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
+]
+
+[[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
 ]
 
 [[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "uuid"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
@@ -1174,7 +1387,16 @@
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "wyz"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
```

