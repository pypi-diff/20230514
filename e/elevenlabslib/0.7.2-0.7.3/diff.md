# Comparing `tmp/elevenlabslib-0.7.2.tar.gz` & `tmp/elevenlabslib-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.7.2.tar", last modified: Fri May 12 21:00:33 2023, max compression
+gzip compressed data, was "elevenlabslib-0.7.3.tar", last modified: Sun May 14 14:49:10 2023, max compression
```

## Comparing `elevenlabslib-0.7.2.tar` & `elevenlabslib-0.7.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.711328 elevenlabslib-0.7.2/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-12 21:00:33.711328 elevenlabslib-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.695328 elevenlabslib-0.7.2/elevenlabslib/
--rw-rw-rw-   0        0        0     6467 2023-05-12 20:03:18.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    36906 2023-05-12 20:18:33.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.2/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5874 2023-05-12 21:00:08.000000 elevenlabslib-0.7.2/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.710329 elevenlabslib-0.7.2/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-12 21:00:17.000000 elevenlabslib-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 21:00:33.712328 elevenlabslib-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.944555 elevenlabslib-0.7.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-14 14:49:10.943554 elevenlabslib-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.927556 elevenlabslib-0.7.3/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    15099 2023-05-14 09:41:13.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    37074 2023-05-14 14:34:49.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.3/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5924 2023-05-14 14:15:27.000000 elevenlabslib-0.7.3/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.943554 elevenlabslib-0.7.3/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-14 14:48:50.000000 elevenlabslib-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:49:10.944555 elevenlabslib-0.7.3/setup.cfg
```

### Comparing `elevenlabslib-0.7.2/LICENSE` & `elevenlabslib-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.2/PKG-INFO` & `elevenlabslib-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.2/README.md` & `elevenlabslib-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files 23% similar despite different names*

```diff
@@ -116,26 +116,28 @@
         """
         if self._audioData is None:
             response = _api_get("/history/" + self.historyID + "/audio", self._parentUser.headers)
             self._audioData = response.content
         return self._audioData
 
     def play_audio(self, playInBackground: bool, portaudioDeviceID: Optional[int] = None,
-                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> None:
+                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> sd.OutputStream:
         """
         Plays the audio associated with the history item.
 
         Args:
             playInBackground: a boolean indicating whether the audio should be played in the background
             portaudioDeviceID: an optional integer representing the portaudio device ID to use
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
+
+        Returns:
+            The sounddevice OutputStream of the playback.
         """
-        play_audio_bytes(self.get_audio_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
-        return
+        return play_audio_bytes(self.get_audio_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
     def fetch_feedback(self):
         """
         Fetches the feedback information associated with this generation.
         """
         response = _api_get(f"/history/{self.historyID}", headers=self._parentUser.headers)
         return response.json()["feedback"]
@@ -149,14 +151,18 @@
             feedbackText: Any text you'd like to add as feedback. Only sent if thumbsUp is true, in which case it must be at least 50 characters.
             issueTypes: A list of types of issues this generation falls under. Only sent if thumbsUp is false.
 
         Note:
             The valid values for issueTypes are: emotions, inaccurate_clone, glitches, audio_quality, other
 
             Other values will be ignored.
+
+        Caution:
+            You CANNOT add positive feedback to items that are "too long". I'm afraid there's no specified maximum duration.
+            If an item is too long, a ValueError will be thrown.
         """
         payload = {
             "thumbs_up":thumbsUp,
             "feedback":""
         }
 
         validIssueTypes = ["emotions", "inaccurate_clone", "glitches", "audio_quality", "other"]
@@ -166,16 +172,30 @@
             else:
                 payload[issueType] = False
 
         if thumbsUp:
             if len(feedbackText) < 50:
                 raise ValueError("Error! Positive feedback text must be at least 50 characters!")
             payload["feedback"] = feedbackText
-
-        response = _api_json(f"/history/{self.historyID}/feedback", headers=self._parentUser.headers, jsonData=payload)
+        try:
+            response = _api_json(f"/history/{self.historyID}/feedback", headers=self._parentUser.headers, jsonData=payload)
+        except (requests.exceptions.RequestException, requests.exceptions.HTTPError) as e:
+            try:
+                responseJson = e.response.json()
+                responseStatus = responseJson["detail"]["status"]
+                responseMessage = responseJson["detail"]["message"]
+                # If those keys aren't present it'll error out and raise e anyway.
+            except:
+                raise e
+            if responseStatus == "invalid_feedback" and "Positive feedback can be specified only for short audio" in responseMessage:
+                logging.error("This audio is too long to add positive feedback text, re-sending feedback without the text.")
+                payload["feedback"] = ""
+                response = _api_json(f"/history/{self.historyID}/feedback", headers=self._parentUser.headers, jsonData=payload)
+            else:
+                raise e
         return response
 
     def delete(self):
         """
         Deletes the item from your history.
         """
         response = _api_del("/history/" + self.historyID, self._parentUser.headers)
```

### Comparing `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsSample.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         """
         if self._audioData is None:
             response = _api_get("/voices/" + self._parentVoice.voiceID + "/samples/" + self._sampleID + "/audio", self._parentVoice.linkedUser.headers)
             self._audioData = response.content
         return self._audioData
 
     def play_audio(self, playInBackground: bool, portaudioDeviceID: Optional[int] = None,
-                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> None:
+                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> sd.OutputStream:
         """
         Downloads and plays the audio associated with the sample.
 
         Args:
             playInBackground: a boolean indicating whether the audio should be played in the background
             portaudioDeviceID: an optional integer representing the portaudio device ID to use
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
         """
-        play_audio_bytes(self.get_audio_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
-        return
+        return play_audio_bytes(self.get_audio_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
+
 
     def delete(self):
         """
         Deletes the sample.
         """
         response = _api_del("/voices/" + self._parentVoice.voiceID + "/samples/" + self._sampleID, self._parentVoice.linkedUser.headers)
         self._sampleID = ""
```

### Comparing `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         Args:
             xi_api_key (str): The user's API key.
 
         Raises:
             ValueError: If the API Key is invalid.
         """
         self._xi_api_key = xi_api_key
-        self._headers = default_headers
+        self._headers = dict()
+        for key, value in default_headers.items():
+            self._headers[key] = value
         self._headers["xi-api-key"] = self._xi_api_key
 
         try:
             self.get_available_voices()
         except (requests.exceptions.RequestException, requests.exceptions.HTTPError) as e:
             try:
                 responseJson = e.response.json()
```

### Comparing `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsVoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
 
         return response.content
     def generate_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
-                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> tuple[bytes,str]:
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> tuple[bytes,str, sd.OutputStream]:
         """
         Generate audio bytes from the given prompt and play them using sounddevice.
 
         Tip:
             This function downloads the entire file before playing it back, and even if playInBackground is set, it will halt execution until the file is downloaded.
             If you need faster response times and background downloading and playback, use generate_and_stream_audio.
 
@@ -237,19 +237,19 @@
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
             latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply. See generate_and_stream_audio for more info.
         Returns:
-           A tuple consisting of the bytes of the audio file and its historyID.
+           A tuple consisting of the bytes of the audio file, its historyID and the sounddevice OutputStream, to allow you to pause/stop the playback early.
         """
         audioData, historyID = self.generate_audio(prompt, stability, similarity_boost, model_id, latencyOptimizationLevel)
-        play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
-        return audioData, historyID
+        outputStream = play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
+        return audioData, historyID, outputStream
 
     def generate_and_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
                                 onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> bytes:
         warn("This function is deprecated. Please use generate_play_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
         audioData = self.generate_audio_bytes(prompt, stability, similarity_boost, model_id)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
@@ -323,30 +323,30 @@
         previewURL = self.get_preview_url()
         if previewURL is None:
             raise RuntimeError("No preview URL available!")
         response = requests.get(previewURL, allow_redirects=True)
         return response.content
 
     def play_preview(self, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
-                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> None:
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> sd.OutputStream:
         """
         Plays the preview audio.
 
         Args:
             playInBackground: A bool indicating whether to play the audio in the background.
             portaudioDeviceID: Optional int indicating the device ID to use for audio playback.
         	onPlaybackStart: Function to call once the playback begins
         	onPlaybackEnd: Function to call once the playback ends
 
         Returns:
-            None
+            The sounddevice OutputStream of the playback.
         """
 
-        play_audio_bytes(self.get_preview_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
-        return
+        return play_audio_bytes(self.get_preview_bytes(), playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
+
 
     @property
     def category(self):
         """
         This property indicates the "type" of the voice, whether it's premade, cloned, designed etc.
         """
         return self._category
```

### Comparing `elevenlabslib-0.7.2/elevenlabslib/__init__.py` & `elevenlabslib-0.7.3/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.2/elevenlabslib/helpers.py` & `elevenlabslib-0.7.3/elevenlabslib/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         req.body,
     ))
 
 
 
 
 def play_audio_bytes(audioData:bytes, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
-                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> None:
+                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> sd.OutputStream:
     """
     Plays the given audio and calls the given functions.
     
     Parameters:
          onPlaybackStart: Function to call once the playback begins
          onPlaybackEnd: Function to call once the playback ends
          audioData: The audio to play
@@ -101,14 +101,15 @@
     playbackWrapper = _SDPlaybackWrapper(audioData, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
     if not playInBackground:
         with playbackWrapper.stream:
             playbackWrapper.endPlaybackEvent.wait()
     else:
         playbackWrapper.stream.start()
+        return playbackWrapper.stream
 
 def save_audio_bytes(audioData:bytes, saveLocation:Union[BinaryIO,str], outputFormat) -> None:
     """
         This function saves the audio data to the specified location OR file-like object.
         soundfile is used for the conversion, so it supports any format it does.
 
         Parameters:
```

### Comparing `elevenlabslib-0.7.2/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.7.3/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.2/pyproject.toml` & `elevenlabslib-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

