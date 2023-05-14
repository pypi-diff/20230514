# Comparing `tmp/speech_collator-0.1.4.tar.gz` & `tmp/speech_collator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_collator-0.1.4.tar", last modified: Sun May 14 16:49:17 2023, max compression
+gzip compressed data, was "speech_collator-0.1.5.tar", last modified: Sun May 14 17:06:46 2023, max compression
```

## Comparing `speech_collator-0.1.4.tar` & `speech_collator-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.4/README.md
--rw-r--r--   0        0        0      522 2023-05-14 16:49:17.921406 speech_collator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    15103 2023-05-14 16:31:08.431767 speech_collator-0.1.4/speech_collator/__init__.py
--rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.4/speech_collator/data/dvector-step250000.pt
--rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.4/speech_collator/data/wav2mel.pt
--rw-r--r--   0        0        0     3969 2023-05-14 12:04:42.857714 speech_collator-0.1.4/speech_collator/measures/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.4/speech_collator/measures/snr.py
--rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.4/speech_collator/measures/srmr.py
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.5/README.md
+-rw-r--r--   0        0        0      522 2023-05-14 17:06:46.143043 speech_collator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    15109 2023-05-14 17:05:41.228749 speech_collator-0.1.5/speech_collator/__init__.py
+-rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.5/speech_collator/data/dvector-step250000.pt
+-rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.5/speech_collator/data/wav2mel.pt
+-rw-r--r--   0        0        0     3969 2023-05-14 12:04:42.857714 speech_collator-0.1.5/speech_collator/measures/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.5/speech_collator/measures/snr.py
+-rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.5/speech_collator/measures/srmr.py
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.5/PKG-INFO
```

### Comparing `speech_collator-0.1.4/pyproject.toml` & `speech_collator-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "speech-collator"
-version = "0.1.4"
+version = "0.1.5"
 description = "A collator for speech datasets with different batching strategies and attribute extraction."
 authors = [
     { name = "Christoph Minixhofer", email = "christoph.minixhofer@gmail.com" },
 ]
 dependencies = [
     "numpy<1.24",
     "pyworld>=0.3.3",
```

### Comparing `speech_collator-0.1.4/speech_collator/__init__.py` & `speech_collator-0.1.5/speech_collator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             durations[duration_mask_rm] = 0
             batch[i]["audio"] = audio[~duration_mask_rm_exp]
             new_mel_len = int(np.ceil(len(batch[i]["audio"]) / self.audio_args["hop_length"]))
             # compute mel spectrogram
             mel = self.mel_spectrogram(torch.tensor(batch[i]["audio"]).unsqueeze(0))
             mel = torch.sqrt(mel[0])
             mel = torch.matmul(self.mel_basis, mel)
-            mel = Collator.drc(mel)
+            mel = SpeechCollator.drc(mel)
 
             batch[i]["mel"] = mel.T
             if batch[i]["mel"].shape[0] > new_mel_len:
                 batch[i]["mel"] = batch[i]["mel"][:new_mel_len]
             if batch[i]["mel"].shape[0] < new_mel_len:
                 batch[i]["mel"] = torch.cat([batch[i]["mel"], torch.zeros(1, batch[i]["mel"].shape[1])])
```

### Comparing `speech_collator-0.1.4/speech_collator/data/dvector-step250000.pt` & `speech_collator-0.1.5/speech_collator/data/dvector-step250000.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.4/speech_collator/data/wav2mel.pt` & `speech_collator-0.1.5/speech_collator/data/wav2mel.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.4/speech_collator/measures/__init__.py` & `speech_collator-0.1.5/speech_collator/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.4/speech_collator/measures/snr.py` & `speech_collator-0.1.5/speech_collator/measures/snr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.4/speech_collator/measures/srmr.py` & `speech_collator-0.1.5/speech_collator/measures/srmr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.4/PKG-INFO` & `speech_collator-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech-collator
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collator for speech datasets with different batching strategies and attribute extraction.
 Author-Email: Christoph Minixhofer <christoph.minixhofer@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: numpy<1.24
 Requires-Dist: pyworld>=0.3.3
 Requires-Dist: librosa<0.10
```

