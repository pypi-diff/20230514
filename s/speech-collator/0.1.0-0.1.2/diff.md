# Comparing `tmp/speech_collator-0.1.0.tar.gz` & `tmp/speech_collator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_collator-0.1.0.tar", last modified: Sun May 14 11:39:32 2023, max compression
+gzip compressed data, was "speech_collator-0.1.2.tar", last modified: Sun May 14 16:39:26 2023, max compression
```

## Comparing `speech_collator-0.1.0.tar` & `speech_collator-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.0/README.md
--rw-r--r--   0        0        0      441 2023-05-14 11:39:32.911376 speech_collator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14161 2023-05-14 11:36:03.003023 speech_collator-0.1.0/speech_collator/__init__.py
--rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.0/speech_collator/data/dvector-step250000.pt
--rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.0/speech_collator/data/wav2mel.pt
--rw-r--r--   0        0        0     3977 2023-05-14 11:35:51.021861 speech_collator-0.1.0/speech_collator/measures/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.0/speech_collator/measures/snr.py
--rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.0/speech_collator/measures/srmr.py
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 speech_collator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.2/README.md
+-rw-r--r--   0        0        0      534 2023-05-14 16:39:26.016014 speech_collator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15103 2023-05-14 16:31:08.431767 speech_collator-0.1.2/speech_collator/__init__.py
+-rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.2/speech_collator/data/dvector-step250000.pt
+-rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.2/speech_collator/data/wav2mel.pt
+-rw-r--r--   0        0        0     3969 2023-05-14 12:04:42.857714 speech_collator-0.1.2/speech_collator/measures/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.2/speech_collator/measures/snr.py
+-rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.2/speech_collator/measures/srmr.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 speech_collator-0.1.2/PKG-INFO
```

### Comparing `speech_collator-0.1.0/speech_collator/__init__.py` & `speech_collator-0.1.2/speech_collator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from torch.nn import ConstantPad1d, ConstantPad2d
 import torchaudio
 from nnAudio.features.mel import MelSpectrogram
 import torchaudio.transforms as AT
 from librosa.filters import mel as librosa_mel
 from time import time
 import pandas as pd
+from tqdm.auto import tqdm
 pd.options.mode.chained_assignment=None
 
 class JitWrapper():
     def __init__(self, path):
         super().__init__()
         self.path = path
         self.model = torch.jit.load(path)
@@ -97,14 +98,15 @@
             fmin=0,
             fmax=8000,
         )
         self.mel_basis = torch.from_numpy(self.mel_basis).float()
         self.include_audio = include_audio
         self.overwrite_max_length = overwrite_max_length
         self.audio_args = audio_args
+        self.pad_value = self.phone2idx["<pad>"]
         if return_keys is None:
             self.return_keys = [
                 "audio",
                 "mel",
                 "phone_durations",
                 "phones",
                 "speaker",
@@ -153,15 +155,15 @@
                 audio = np.pad(audio, (0, max_audio_len - len(audio)))
             elif len(audio) > max_audio_len:
                 audio = audio[:max_audio_len]
             
             duration_permutation = np.argsort(durations+np.random.normal(0, durations.std(), len(durations)))
             duration_mask_rm = durations[duration_permutation].cumsum() >= self.max_frame_length
             duration_mask_rm = duration_mask_rm[np.argsort(duration_permutation)]
-            batch[i]["phones"][duration_mask_rm] = self.phone2idx["MASK"]
+            batch[i]["phones"][duration_mask_rm] = self.phone2idx["<mask>"]
             duration_mask_rm_exp = np.repeat(duration_mask_rm, durations * self.audio_args["hop_length"])
             dur_sum = sum(durations)
             self.num_total += 1
             self.num_masked += 1 if sum(duration_mask_rm) > 0 else 0
             self.percentage_mask_tokens += sum(duration_mask_rm_exp) / len(duration_mask_rm_exp)
             durations[duration_mask_rm] = 0
             batch[i]["audio"] = audio[~duration_mask_rm_exp]
@@ -262,23 +264,23 @@
                         embed = self.dvector.model.embed_utterance(self.wav2mel.model(x["audio"].unsqueeze(0), 22050)).squeeze(0)
                     except RuntimeError:
                         embed = torch.zeros(256)
                     result["dvector"].append(embed)
                 result["dvector"] = torch.stack(result["dvector"])
                 torch.cuda.empty_cache()
         if "audio" in self.return_keys:
-            result["audio"] = pad_sequence([x["audio"] for x in batch], batch_first=True)
+            result["audio"] = pad_sequence([x["audio"] for x in batch], batch_first=True, padding_value=self.pad_value)
         if "mel" in self.return_keys:
-            result["mel"] = pad_sequence([x["mel"] for x in batch], batch_first=True)
+            result["mel"] = pad_sequence([x["mel"] for x in batch], batch_first=True, padding_value=self.pad_value)
         if "phone_durations" in self.return_keys:
-            result["phone_durations"] = pad_sequence([x["phone_durations"] for x in batch], batch_first=True)
+            result["phone_durations"] = pad_sequence([x["phone_durations"] for x in batch], batch_first=True, padding_value=self.pad_value)
         if "durations" in self.return_keys:
-            result["durations"] = pad_sequence([x["durations"] for x in batch], batch_first=True)
+            result["durations"] = pad_sequence([x["durations"] for x in batch], batch_first=True, padding_value=self.pad_value)
         if "phones" in self.return_keys:
-            result["phones"] = pad_sequence([x["phones"] for x in batch], batch_first=True)
+            result["phones"] = pad_sequence([x["phones"] for x in batch], batch_first=True, padding_value=self.pad_value)
         if "speaker" in self.return_keys:
             speakers = [str(x["speaker"]).split("/")[-1] if ("/" in str(x["speaker"])) else x["speaker"] for x in batch]
             # speaker2idx
             result["speaker"] = torch.tensor([self.speaker2idx[x] for x in speakers])
 
         if self.overwrite_max_length and "phone_durations" in self.return_keys and "val_ind" in self.return_keys:
             MAX_FRAMES = self.max_frame_length
@@ -287,16 +289,36 @@
             result["phone_durations"][:, -1] = MAX_FRAMES - result["phone_durations"].sum(-1)
             result["val_ind"] = torch.arange(0, MAX_PHONES).repeat(BATCH_SIZE).reshape(BATCH_SIZE, MAX_PHONES)
             result["val_ind"] = result["val_ind"].flatten().repeat_interleave(result["phone_durations"].flatten(), dim=0).reshape(BATCH_SIZE, MAX_FRAMES)
 
         if self.measures is not None and "measures" in self.return_keys:
             result["measures"] = {}
             for measure in self.measures:
-                result["measures"][measure.name] = pad_sequence([x["measures"][measure.name] for x in batch], batch_first=True)
+                result["measures"][measure.name] = pad_sequence([x["measures"][measure.name] for x in batch], batch_first=True, padding_value=self.pad_value)
         elif "measures" in self.return_keys:
             result["measures"] = None
 
         result = {
             k: v for k, v in result.items() if k in self.return_keys
         }
 
-        return result
+        return result
+
+def create_speaker2idx(dataset, additonal_tokens=["<unk>"]):
+    speaker2idx = {
+        k: v for k, v in zip(additonal_tokens, range(len(additonal_tokens)))
+    }
+    for row in tqdm(dataset):
+        if row["speaker"] not in speaker2idx:
+            speaker2idx[row["speaker"]] = len(speaker2idx)
+    return speaker2idx
+
+def create_phone2idx(dataset, additonal_tokens=["<pad>", "<mask>", "<unk>"]):
+    phone2idx = {
+        k: v for k, v in zip(additonal_tokens, range(len(additonal_tokens)))
+    }
+    for row in tqdm(dataset):
+        for phone in row["phones"]:
+            if phone not in phone2idx:
+                phone2idx[phone] = len(phone2idx)
+    return phone2idx
+
```

### Comparing `speech_collator-0.1.0/speech_collator/data/dvector-step250000.pt` & `speech_collator-0.1.2/speech_collator/data/dvector-step250000.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.0/speech_collator/data/wav2mel.pt` & `speech_collator-0.1.2/speech_collator/data/wav2mel.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.0/speech_collator/measures/__init__.py` & `speech_collator-0.1.2/speech_collator/measures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 import os
 
 import numpy as np
 import pyworld as pw
 import librosa
-import torch
 from scipy import interpolate
 
 from .snr import wada_snr
 from .srmr import srmr
 
 class Measure(ABC):
     def __init__(self, name, description):
@@ -128,8 +127,9 @@
         super().__init__(name, description)
         self.sampling_rate = sampling_rate
         self.win_length = win_length
         self.hop_length = hop_length
 
     def compute(self, audio, durations, silence_mask=None):
         snr, snr_t = wada_snr(audio)
-        return snr_t
+        return snr_t
+
```

### Comparing `speech_collator-0.1.0/speech_collator/measures/snr.py` & `speech_collator-0.1.2/speech_collator/measures/snr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.0/speech_collator/measures/srmr.py` & `speech_collator-0.1.2/speech_collator/measures/srmr.py`

 * *Files identical despite different names*

